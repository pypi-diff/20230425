# Comparing `tmp/rubpy-6.1.0.tar.gz` & `tmp/rubpy-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.0.tar", last modified: Mon Apr 24 00:07:29 2023, max compression
+gzip compressed data, was "rubpy-6.1.2.tar", last modified: Mon Apr 24 21:00:50 2023, max compression
```

## Comparing `rubpy-6.1.0.tar` & `rubpy-6.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.222798 rubpy-6.1.0/
--rw-rw-rw-   0        0        0     3347 2023-04-24 00:07:29.207178 rubpy-6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.191556 rubpy-6.1.0/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-24 00:07:06.000000 rubpy-6.1.0/rubpy/__init__.py
--rw-rw-rw-   0        0        0    29264 2023-04-24 00:05:02.000000 rubpy-6.1.0/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.0/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25878 2023-04-24 00:03:50.000000 rubpy-6.1.0/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.0/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.1.0/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.0/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 00:07:29.222798 rubpy-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-04-24 00:06:27.000000 rubpy-6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.953629 rubpy-6.1.2/
+-rw-rw-rw-   0        0        0     3347 2023-04-24 21:00:50.953629 rubpy-6.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.875064 rubpy-6.1.2/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-24 20:58:12.000000 rubpy-6.1.2/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    32368 2023-04-24 20:56:07.000000 rubpy-6.1.2/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.890685 rubpy-6.1.2/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.906332 rubpy-6.1.2/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.2/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.2/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.2/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.937967 rubpy-6.1.2/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.1.2/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.937967 rubpy-6.1.2/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.953629 rubpy-6.1.2/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.2/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.890685 rubpy-6.1.2/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 21:00:50.953629 rubpy-6.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-04-24 20:58:39.000000 rubpy-6.1.2/setup.py
```

### Comparing `rubpy-6.1.0/PKG-INFO` & `rubpy-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.0
+Version: 6.1.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.0/README.md` & `rubpy-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/client.py` & `rubpy-6.1.2/rubpy/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         timeout=20,
         lang_code='fa',
         user_agent=None,
         request_retries=5, *args, **kwargs):
 
         """Client
             Args:
-                session_name (`str` | `rubika.sessions.StringSession`):
+                session_name (`str` | `rubpy.sessions.StringSession`):
                     The file name of the session file that is used
                     if there is a string Given (may be a complete path)
                     or it could be a string session
-                    [rubika.sessions.StringSession]
+                    [rubpy.sessions.StringSession]
 
-                proxy (` rubika.network.Proxies `, optional): To set up a proxy
+                proxy (` rubpy.network.Proxies `, optional): To set up a proxy
 
                 user_agent (`str`, optional):
                     Client uses the web version, You can set the usr-user_agent
 
                 timeout (`int` | `float`, optional):
                     To set the timeout `` default( `20 seconds` )``
 
@@ -53,22 +53,22 @@
         """
 
         if isinstance(session, str):
             session = SQLiteSession(session)
 
         elif not isinstance(session, StringSession):
             raise TypeError('The given session must be a '
-                            'str or [rubika.sessions.StringSession]')
+                            'str or [rubpy.sessions.StringSession]')
 
         if not isinstance(logger, logging.Logger):
             logger = logging.getLogger(logger_name)
 
         if proxy and not isinstance(proxy, Proxies):
             raise TypeError(
-                'The given proxy must be a [rubika.network.Proxies]')
+                'The given proxy must be a [rubpy.network.Proxies]')
 
         self._dcs = None
         self._key = None
         self._auth = None
         self._guid = None
         self._proxy = proxy
         self._logger = logger
@@ -232,15 +232,15 @@
         if isinstance(file, str):
             with open(file, 'wb+') as _file:
                 _file.write(result)
                 return file
 
         return result
 
-# Users Methods
+# ---------------- Users Methods ----------------
 
     async def get_user_info(self, user_guid: str):
         return await self(methods.users.GetUserInfo(user_guid))
 
     async def block_user(self, user_guid: str):
         return await self(methods.users.SetBlockUser(user_guid, 'Block'))
 
@@ -249,15 +249,15 @@
 
     async def delete_user_chat(self, user_guid: str, last_deleted_message_id: str):
         return await self(methods.users.DeleteUserChat(user_guid, last_deleted_message_id))
 
     async def check_user_username(self, username: str):
         return await self(methods.users.CheckUserUsername(username.replace('@', '')))
 
-# Chats Methods
+# ---------------- Chats Methods ----------------
 
     async def upload_avatar(self, object_guid: str, main_file_id: str, thumbnail_file_id: str):
         return await self(methods.chats.UploadAvatar(object_guid, main_file_id, thumbnail_file_id))
 
     async def delete_avatar(self, object_guid: str, avatar_id: str):
         return await self(methods.chats.DeleteAvatar(object_guid, avatar_id))
 
@@ -289,29 +289,29 @@
 
     async def delete_chat_history(self, object_guid: str):
         return await self(methods.chats.DeleteChatHistory(object_guid))
 
     async def search_chat_messages(self, object_guid: str, search_text: str, type: str = 'Hashtag'):
         return await self(methods.chats.SearchChatMessages(object_guid, search_text, type))
 
-# Extras Methods
+# ---------------- Extras Methods ----------------
 
     async def search_global_objects(self, search_text: str):
-        return await self(methods.chats.SearchGlobalObjects(search_text))
+        return await self(methods.extras.SearchGlobalObjects(search_text))
 
     async def get_abs_objects(self, objects_guids: list):
-        return await self(methods.chats.GetAbsObjects(objects_guids))
+        return await self(methods.extras.GetAbsObjects(objects_guids))
 
     async def get_object_by_username(self, username: str):
-        return await self(methods.chats.GetObjectByUsername(username.replace('@', '')))
+        return await self(methods.extras.GetObjectByUsername(username.replace('@', '')))
 
     async def get_link_from_app_url(self, app_url: str):
-        return await self(methods.chats.GetLinkFromAppUrl(app_url))
+        return await self(methods.extras.GetLinkFromAppUrl(app_url))
 
-# Groups Methods
+# ---------------- Groups Methods ----------------
 
     async def add_group(self, title: str, member_guids: list):
         return await self(methods.groups.AddGroup(title, member_guids))
 
     async def join_group(self, link: str):
         return await self(methods.groups.JoinGroup(link))
 
@@ -388,15 +388,15 @@
 
     async def get_group_admin_access_list(self, group_guid: str, member_guid: str):
         return await self(methods.groups.GetGroupAdminAccessList(group_guid, member_guid))
 
     async def set_group_timer(self, group_guid: str, time: int):
         return await self(methods.groups.EditGroupInfo(group_guid, slow_mode=time, updated_parameters=['slow_mode']))
 
-# Messages Methods
+# ---------------- Messages Methods ----------------
 
     async def send_message(self,
         object_guid: str,
         message=None,
         reply_to_message_id: str = None,
         file_inline=None,
         type: str = methods.messages.File,
@@ -497,24 +497,36 @@
             type: str = 'Regular',
             is_anonymous: bool = True,
             allows_multiple_answers: bool = False,
             correct_option_index: int = 0,
             explanation: str = None,
             reply_to_message_id: int = 0,
     ):
-        return await self(methods.messages.CreatePoll(
-            object_guid,
-            question,
-            options,
-            type,
-            is_anonymous,
-            allows_multiple_answers,
-            correct_option_index,
-            explanation,
-            reply_to_message_id))
+        if type == 'Regular':
+            return await self(methods.messages.CreatePoll(
+                object_guid=object_guid,
+                question=question,
+                options=options,
+                allows_multiple_answers=allows_multiple_answers,
+                is_anonymous=is_anonymous,
+                reply_to_message_id=reply_to_message_id,
+                type=type,
+            ))
+        else:
+            return await self(methods.messages.CreatePoll(
+                object_guid=object_guid,
+                question=question,
+                options=options,
+                allows_multiple_answers=allows_multiple_answers,
+                is_anonymous=is_anonymous,
+                reply_to_message_id=reply_to_message_id,
+                correct_option_index=correct_option_index,
+                explanation=explanation,
+                type=type,
+            ))
 
     async def vote_poll(self, poll_id: str, selection_index: int):
         return await self(methods.messages.VotePoll(poll_id, selection_index))
 
     async def get_poll_status(self, poll_id: str):
         return await self(methods.messages.GetPollStatus(poll_id))
 
@@ -541,34 +553,45 @@
 
     async def get_messages(self, object_guid: str, min_id: int, max_id: int, sort: str = 'FromMin', limit: int = 10):
         return await self(methods.messages.GetMessages(object_guid, min_id, max_id, sort, limit))
 
     async def get_messages_interval(self, object_guid: str, middle_message_id: str):
         return await self(methods.messages.GetMessagesInterval(object_guid, middle_message_id))
 
-# Channels Methods
+# ---------------- Channels Methods ----------------
 
     async def add_channel(self, title: str, description: str = None):
         return await self(methods.channels.AddChannel(title, description))
 
     async def remove_channel(self, channel_guid: str):
         return await self(methods.channels.RemoveChannel(channel_guid))
 
     async def get_channel_info(self, channel_guid: str):
         return await self(methods.channels.GetChannelInfo(channel_guid))
 
     async def edit_channel_info(self,
             channel_guid: str,
-            title: str,
+            title: str = None,
             description: str = None,
-            channel_type: str = 'Public',
+            channel_type: str = None,
             sign_messages: str = None,
     ):
+        updated_parameters = []
+
+        if title:
+            updated_parameters.append('title')
+        if description:
+            updated_parameters.append('description')
+        if channel_type:
+            updated_parameters.append('channel_type')
+        if sign_messages:
+            updated_parameters.append('sign_messages')
+
         return await self(methods.channels.EditChannelInfo(
-            channel_guid, title, description, channel_type, sign_messages))
+            channel_guid, updated_parameters, title, description, channel_type, sign_messages))
 
     async def join_channel(self, channel_guid: str):
         return await self(methods.channels.JoinChannelAction(channel_guid, 'Join'))
 
     async def leave_channel(self, channel_guid: str):
         return await self(methods.channels.JoinChannelAction(channel_guid, 'Remove'))
 
@@ -607,38 +630,52 @@
 
     async def set_channel_link(self, channel_guid: str):
         return await self(methods.channels.SetChannelLink(channel_guid))
 
     async def get_channel_admin_access_list(self, channel_guid: str, member_guid: str):
         return await self(methods.channels.GetChannelAdminAccessList(channel_guid, member_guid))
 
-# Contacts Methods
+# ---------------- Contacts Methods ----------------
 
     async def delete_contact(self, user_guid: str):
         return await self(methods.contacts.DeleteContact(user_guid))
 
     async def add_address_book(self, phone: str, first_name: str, last_name: str = ''):
         return await self(methods.contacts.AddAddressBook(phone, first_name, last_name))
 
     async def get_contacts_updates(self, state: int = None):
         return await self(methods.contacts.GetContactsUpdates(state))
 
     async def get_contacts(self, start_id: int = None):
         return await self(methods.contacts.GetContacts(start_id))
 
-# Settings Methods
+# ---------------- Settings Methods ----------------
 
     async def set_setting(self,
             show_my_last_online: str = None,
             show_my_phone_number: str = None,
             show_my_profile_photo: str = None,
             link_forward_message: str = None,
             can_join_chat_by: str = None
     ):
+        updated_parameters = []
+
+        if show_my_last_online:
+            updated_parameters.append('show_my_last_online')
+        if show_my_phone_number:
+            updated_parameters.append('show_my_phone_number')
+        if show_my_profile_photo:
+            updated_parameters.append('show_my_profile_photo')
+        if link_forward_message:
+            updated_parameters.append('link_forward_message')
+        if can_join_chat_by:
+            updated_parameters.append('can_join_chat_by')
+
         return await self(methods.settings.SetSetting(
+            updated_parameters,
             show_my_last_online,
             show_my_phone_number,
             show_my_profile_photo,
             link_forward_message,
             can_join_chat_by))
 
     async def add_folder(self,
@@ -658,36 +695,72 @@
 
     async def edit_folder(self,
             include_chat_types: list = None,
             exclude_chat_types: list = None,
             include_object_guids: list = None,
             exclude_object_guids: list = None
     ):
+        updated_parameters = []
+
+        if include_chat_types:
+            updated_parameters.append('include_chat_types')
+        if exclude_chat_types:
+            updated_parameters.append('exclude_chat_types')
+        if include_object_guids:
+            updated_parameters.append('include_object_guids')
+        if exclude_object_guids:
+            updated_parameters.append('exclude_object_guids')
+
         return await self(methods.contacts.EditFolder(
+            updated_parameters,
             include_chat_types,
             exclude_chat_types,
             include_object_guids,
             exclude_object_guids))
 
     async def delete_folder(self, folder_id: str):
         return await self(methods.contacts.DeleteFolder(folder_id))
 
     async def update_profile(self, first_name: str = None, last_name: str = None, bio: str = None):
-        return await self(methods.contacts.UpdateProfile(first_name, last_name, bio))
+        updated_parameters = []
+
+        if first_name:
+            updated_parameters.append('first_name')
+        if last_name:
+            updated_parameters.append('last_name')
+        if bio:
+            updated_parameters.append('bio')
+
+        return await self(methods.contacts.UpdateProfile(updated_parameters, first_name, last_name, bio))
 
     async def update_username(self, username: str):
         return await self(methods.contacts.UpdateUsername(username))
 
+    async def get_two_passcode_status(self):
+        return await self(methods.contacts.GetTwoPasscodeStatus())
+
+    async def get_suggested_folders(self):
+        return await self(methods.contacts.GetSuggestedFolders())
+
+    async def get_privacy_setting(self):
+        return await self(methods.contacts.GetPrivacySetting())
+
+    async def get_blocked_users(self):
+        return await self(methods.contacts.GetBlockedUsers())
+
+    async def get_my_sessions(self):
+        return await self(methods.contacts.GetMySessions())
+
     async def terminate_session(self, session_key: str):
         return await self(methods.contacts.TerminateSession(session_key))
 
     async def setup_two_step_verification(self, password: str, hint: str, recovery_email: str):
         return await self(methods.contacts.SetupTwoStepVerification(password, hint, recovery_email))
 
-# Stickers Methods
+# ---------------- Stickers Methods ----------------
 
     async def get_my_sticker_sets(self):
         return await self(methods.stickers.GetMyStickerSets())
 
     async def search_stickers(self, search_text: str = '', start_id: int = None):
         return await self(methods.stickers.SearchStickers(search_text, start_id))
 
@@ -696,12 +769,12 @@
 
     async def action_on_sticker_set(self, sticker_set_id: str, action: str = 'Add'):
         return await self(methods.stickers.ActionOnStickerSet(sticker_set_id, action))
 
     async def get_stickers_by_emoji(self, emoji: str, suggest_by: str = 'Add'):
         return await self(methods.stickers.GetStickersByEmoji(emoji, suggest_by))
 
-    async def GetStickersBySetIDs(self, sticker_set_ids: list):
+    async def get_stickers_by_set_IDs(self, sticker_set_ids: list):
         return await self(methods.stickers.GetStickersBySetIDs(sticker_set_ids))
 
-    async def GetTrendStickerSets(self, start_id: int = None):
+    async def get_trend_sticker_sets(self, start_id: int = None):
         return await self(methods.stickers.GetTrendStickerSets(start_id))
```

### Comparing `rubpy-6.1.0/rubpy/crypto/crypto.py` & `rubpy-6.1.2/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/gadgets/classino.py` & `rubpy-6.1.2/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/gadgets/exceptions.py` & `rubpy-6.1.2/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/gadgets/grouping.py` & `rubpy-6.1.2/rubpy/gadgets/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,23 +284,23 @@
                 "message_ids": {"types": ["int", "str", "list"], "func": "to_array"},
                 "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"}
             }
         },
         "CreatePoll": {
             "params": {
                 "object_guid": {"types": "str"},
-                "question": {"types": "str", "func": "to_metadata", "unpack": True},
+                "question": {"types": "str",  },
                 "options": {"types": "list", "minimum": 2},
                 "type": {"types": ["str", "optional"], "alloweds": ["Quiz", "Regular"], "default": "Regular"},
-                "is_anonymous": {"types": ["bool", "optional"], "default": True},
-                "allows_multiple_answers": {"types": ["bool", "optional"], "default": False},
-                "correct_option_index": {"types": ["str", "int", "optional"], "default": 0, "func": "to_number"},
+                "is_anonymous": {"types": ["bool", "optional"]},
+                "allows_multiple_answers": {"types": ["bool", "optional"]},
+                "correct_option_index": {"types": ["str", "int", "optional"], "func": "to_number"},
                 "explanation": {"types": ["str", "optional"]},
-                "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"},
-                "reply_to_message_id": {"types": "int"}, "default": 0
+                "reply_to_message_id": {"types": ["int", "optional"], "default": 0},
+                "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"}
             }
         },
         "VotePoll": {
             "params": {
                 "poll_id": {"types": "str"},
                 "selection_index": {"types": ["int", "str"], "func": "to_number"}
             }
@@ -386,15 +386,15 @@
         "EditChannelInfo": {
             "updated_parameters": True,
             "params": {
                 "channel_guid": {"types": "str"},
                 "updated_parameters": {"types": ["list"], "alloweds": ["title", "description", "channel_type", "sign_messages"]},
                 "title": {"types": "str"},
                 "description": {"types": ["str", "optional"]},
-                "channel_type": {"types": ["str", "optional"], "alloweds": ["Public", "Private"]},
+                "channel_type": {"types": ["str", "optional"], "alloweds": ["Public", "Private"], "default": "Public" },
                 "sign_messages": {"types": ["str", "optional"]}
             }
         },
         "JoinChannelAction": {
             "params": {
                 "channel_guid": {"types": "str"},
                 "action": {"types": ["str", "optional"], "alloweds": ["Join", "Remove", "Archive"], "default": "Join"}
```

### Comparing `rubpy-6.1.0/rubpy/gadgets/methods.py` & `rubpy-6.1.2/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.2/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/network/connection.py` & `rubpy-6.1.2/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/network/proxies.py` & `rubpy-6.1.2/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.2/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/sessions/stringSession.py` & `rubpy-6.1.2/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/structs/handlers.py` & `rubpy-6.1.2/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/structs/models.py` & `rubpy-6.1.2/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/structs/results.py` & `rubpy-6.1.2/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy/structs/struct.py` & `rubpy-6.1.2/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.2/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.0
+Version: 6.1.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.0/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.2/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.0/setup.py` & `rubpy-6.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.0',
+    version = '6.1.2',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

