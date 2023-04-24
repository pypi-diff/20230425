# Comparing `tmp/tradchat-0.0.5.tar.gz` & `tmp/tradchat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradchat-0.0.5.tar", last modified: Mon Apr 24 22:25:04 2023, max compression
+gzip compressed data, was "tradchat-0.0.6.tar", last modified: Mon Apr 24 23:45:49 2023, max compression
```

## Comparing `tradchat-0.0.5.tar` & `tradchat-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 22:25:04.780254 tradchat-0.0.5/
--rw-rw-rw-   0        0        0      343 2023-04-24 22:25:04.779258 tradchat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 22:25:04.780254 tradchat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-04-24 22:24:02.000000 tradchat-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:25:04.753326 tradchat-0.0.5/tradchat/
--rw-rw-rw-   0        0        0    22963 2023-04-24 22:24:55.000000 tradchat-0.0.5/tradchat/Server.py
--rw-rw-rw-   0        0        0  4244882 2023-04-24 22:22:19.000000 tradchat-0.0.5/tradchat/zip.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:25:04.778261 tradchat-0.0.5/tradchat.egg-info/
--rw-rw-rw-   0        0        0      343 2023-04-24 22:25:04.000000 tradchat-0.0.5/tradchat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-24 22:25:04.000000 tradchat-0.0.5/tradchat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 22:25:04.000000 tradchat-0.0.5/tradchat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 22:25:04.000000 tradchat-0.0.5/tradchat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 22:25:04.000000 tradchat-0.0.5/tradchat.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-24 23:45:49.184937 tradchat-0.0.6/
+-rw-rw-rw-   0        0        0      343 2023-04-24 23:45:49.184937 tradchat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 23:45:49.184937 tradchat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-04-24 23:45:36.000000 tradchat-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:45:49.120043 tradchat-0.0.6/tradchat/
+-rw-rw-rw-   0        0        0    22960 2023-04-24 23:45:12.000000 tradchat-0.0.6/tradchat/Server.py
+-rw-rw-rw-   0        0        0  4246731 2023-04-24 23:44:42.000000 tradchat-0.0.6/tradchat/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-24 23:45:49.179535 tradchat-0.0.6/tradchat.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-04-24 23:45:48.000000 tradchat-0.0.6/tradchat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-24 23:45:48.000000 tradchat-0.0.6/tradchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 23:45:48.000000 tradchat-0.0.6/tradchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 23:45:48.000000 tradchat-0.0.6/tradchat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 23:45:48.000000 tradchat-0.0.6/tradchat.egg-info/zip-safe
```

### Comparing `tradchat-0.0.5/tradchat/Server.py` & `tradchat-0.0.6/tradchat/Server.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         chatterer = ''
     form = Upload()
     names = []
     for account in accounts:
         names.append(account)
     names.remove(username)
     names.remove('Server')
-    return render_template('messagenger.html', names=str(names), name=username, color=accounts[session['username']][2], gender=accounts[session['username']][1], form=form, chatterer=chatterer)
+    return render_template('messagenger.html', room=accounts[session['username']][6], names=str(names), name=username, color=accounts[session['username']][2], gender=accounts[session['username']][1], form=form, chatterer=chatterer)
 
 
 @app.route('/learnYourFriends/', methods=['POST'])
 def learnYourFriends():
     try:
         print(session['username'])
     except Exception:
@@ -383,34 +383,37 @@
             send_email(email, username)
             Server.send(str(['Message sent successfully', username_he_typed, f'Email sent successfully to {email}']), broadcast=True)
         except Exception:
             Server.send(str(['Something went wrong', username_he_typed]), broadcast=True)
     else:
         Server.send(str(['You are trying to send an email to a username that does not exist', username_he_typed]), broadcast=True)
 
+def delete(account):
+    Server.send(str(["Command", account, "location.replace('/logout/')"]))
+    del accounts[account]
+    file = open('accounts.txt', 'w')
+    for thing in list(str(accounts)):
+        try:
+            file.write(thing)
+        except UnicodeEncodeError:
+            file.write(' _emoji_ ')
+    file.close()
+
 def recv(msg):
     try:
         message = eval(msg)
     except Exception:
         print(f'Error: {msg}')
         return
-    if message[0] == 'I am ordering you to command':
+    if message[0] == 'I am ordering you to send':
         if message[1] == control_panel_password:
             Server.send(message[2], broadcast=True)
-    if message[0] == 'I am ordering you to delete':
+    if message[0] == 'Direct Order':
         if message[1] == control_panel_password:
-            Server.send(str(["Command", message[2], "location.replace('/logout/')"]))
-            del accounts[message[2]]
-            file = open('accounts.txt', 'w')
-            for thing in list(str(accounts)):
-                try:
-                    file.write(thing)
-                except UnicodeEncodeError:
-                    file.write(' _emoji_ ')
-            file.close()
+            eval(message[2])
     if message[0] == "making sure it is alright to send a email":
         if '@' in list(message[1]):#they typed a email
             sending_email_if_the_user_typed_an_email_vs_if_he_typed_a_username(message[1])
             return
         else:#they typed a username
             sending_email_if_the_user_typed_an_username_vs_if_he_typed_a_email(message[1])
             return
```

### Comparing `tradchat-0.0.5/tradchat/zip.py` & `tradchat-0.0.6/tradchat/zip.py`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 4244882 bytes, number of entries: 90
-drwx---     2.0 fat        0 b- stor 23-Apr-24 17:06 static/graphics/
+Zip file size: 4246731 bytes, number of entries: 90
+drwx---     2.0 fat        0 b- stor 23-Apr-24 19:39 static/graphics/
 -rw-a--     2.0 fat    38049 b- defN 23-Apr-13 09:52 static/graphics/audio.png
 -rw-a--     2.0 fat    42948 b- defN 23-Apr-13 09:52 static/graphics/audio2.png
 -rw-a--     2.0 fat     2777 b- defN 23-Apr-13 09:52 static/graphics/back.png
 -rw-a--     2.0 fat     3117 b- defN 23-Apr-13 09:52 static/graphics/back2.png
 -rw-a--     2.0 fat    14427 b- defN 23-Apr-13 09:52 static/graphics/backToMainRoom.png
 -rw-a--     2.0 fat    16239 b- defN 23-Apr-13 09:52 static/graphics/backToMainRoom2.png
 -rw-a--     2.0 fat   144091 b- defN 23-Apr-24 16:58 static/graphics/command.png
 -rw-a--     2.0 fat   207164 b- defN 23-Apr-13 09:52 static/graphics/defaultBoy.png
 -rw-a--     2.0 fat   223165 b- defN 23-Apr-13 09:52 static/graphics/defaultGirl.png
--rw-a--     2.0 fat    10274 b- defN 23-Apr-24 17:05 static/graphics/delete.png
--rw-a--     2.0 fat    11480 b- defN 23-Apr-24 17:06 static/graphics/delete2.png
 -rw-a--     2.0 fat     3522 b- defN 23-Apr-13 09:52 static/graphics/deleteARoom.png
 -rw-a--     2.0 fat     4038 b- defN 23-Apr-13 09:52 static/graphics/deleteARoom2.png
 -rw-a--     2.0 fat    12700 b- defN 23-Apr-13 09:52 static/graphics/deleteRoom.png
 -rw-a--     2.0 fat    13452 b- defN 23-Apr-13 09:52 static/graphics/deleteRoom2.png
+-rw-a--     2.0 fat    10921 b- defN 23-Apr-24 19:37 static/graphics/direct.png
+-rw-a--     2.0 fat    12665 b- defN 23-Apr-24 19:38 static/graphics/direct2.png
 -rw-a--     2.0 fat    62596 b- defN 23-Apr-13 09:52 static/graphics/div.png
 -rw-a--     2.0 fat   383752 b- defN 23-Apr-24 16:38 static/graphics/email.png
 -rw-a--     2.0 fat    10189 b- defN 23-Apr-24 17:03 static/graphics/execute.png
 -rw-a--     2.0 fat    11078 b- defN 23-Apr-24 17:03 static/graphics/execute2.png
 -rw-a--     2.0 fat    21226 b- defN 23-Apr-13 09:52 static/graphics/forgot.png
 -rw-a--     2.0 fat    23886 b- defN 23-Apr-13 09:52 static/graphics/forgot2.png
 -rw-a--     2.0 fat     3024 b- stor 23-Apr-13 09:52 static/graphics/go.png
@@ -57,36 +57,36 @@
 -rw-a--     2.0 fat     3718 b- defN 23-Apr-13 09:52 static/graphics/SignUp1.png
 -rw-a--     2.0 fat     4329 b- defN 23-Apr-13 09:52 static/graphics/SignUp2.png
 -rw-a--     2.0 fat   362098 b- defN 23-Apr-13 09:52 static/graphics/SignupScreen.png
 -rw-a--     2.0 fat   182144 b- defN 23-Apr-13 09:52 static/graphics/SubmitButton1.png
 -rw-a--     2.0 fat   180000 b- defN 23-Apr-13 09:52 static/graphics/SubmitButton2.png
 -rw-a--     2.0 fat   446967 b- defN 23-Apr-13 09:52 static/graphics/trad.png
 drwx---     2.0 fat        0 b- stor 23-Apr-24 16:53 static/JavaScript/
--rw-a--     2.0 fat     1725 t- defN 23-Apr-24 17:56 static/JavaScript/control.js
+-rw-a--     2.0 fat     1707 t- defN 23-Apr-24 19:38 static/JavaScript/control.js
 -rw-a--     2.0 fat     2526 t- defN 23-Apr-24 17:58 static/JavaScript/email.js
--rw-a--     2.0 fat    10380 t- defN 23-Apr-24 18:14 static/JavaScript/gamer.js
+-rw-a--     2.0 fat    10380 t- defN 23-Apr-24 19:44 static/JavaScript/gamer.js
 -rw-a--     2.0 fat     4651 t- defN 23-Apr-24 17:58 static/JavaScript/login.js
--rw-a--     2.0 fat    25836 t- defN 23-Apr-24 18:19 static/JavaScript/mainpage.js
--rw-a--     2.0 fat    13951 t- defN 23-Apr-24 18:19 static/JavaScript/messagenger.js
+-rw-a--     2.0 fat    26473 t- defN 23-Apr-24 19:14 static/JavaScript/mainpage.js
+-rw-a--     2.0 fat    14473 t- defN 23-Apr-24 19:17 static/JavaScript/messagenger.js
 -rw-a--     2.0 fat     3187 t- defN 23-Apr-24 17:59 static/JavaScript/settings.js
 -rw-a--     2.0 fat     3902 t- defN 23-Apr-24 18:00 static/JavaScript/showMe.js
 -rw-a--     2.0 fat     7116 t- defN 23-Apr-24 17:59 static/JavaScript/signup.js
 -rw-a--     2.0 fat   245074 t- defN 23-Apr-13 09:52 static/JavaScript/socket.io.js.map
 -rw-a--     2.0 fat   191054 t- defN 23-Apr-13 09:52 static/JavaScript/socketio.js
 -rw-a--     2.0 fat     2143 t- defN 23-Apr-24 18:00 static/JavaScript/trad.js
 -rw-a--     2.0 fat   156404 b- defN 23-Apr-13 09:52 static/messinger.png
 -rw-a--     2.0 fat    23994 b- defN 22-Apr-29 16:08 static/private.mp3
 -rw-a--     2.0 fat    17322 b- defN 22-Apr-29 16:07 static/public.mp3
-drwx---     2.0 fat        0 b- stor 23-Apr-24 18:21 static/savedPictures/
+drwx---     2.0 fat        0 b- stor 23-Apr-24 19:43 static/savedPictures/
 -rw-a--     2.0 fat   204618 b- defN 23-Apr-13 09:52 static/savedPictures/Server
-drwx---     2.0 fat        0 b- stor 23-Apr-24 18:21 static/sharedAudio/
-drwx---     2.0 fat        0 b- stor 23-Apr-18 14:33 static/sharedPictures/
+drwx---     2.0 fat        0 b- stor 23-Apr-24 19:28 static/sharedAudio/
+drwx---     2.0 fat        0 b- stor 23-Apr-24 19:28 static/sharedPictures/
 -rw-a--     2.0 fat      510 t- defN 23-Apr-24 17:12 templates/control.html
 -rw-a--     2.0 fat      495 t- defN 23-Apr-13 09:52 templates/email.html
 -rw-a--     2.0 fat      466 t- defN 23-Apr-13 09:52 templates/login.html
 -rw-a--     2.0 fat     1487 t- defN 23-Apr-13 09:52 templates/mainpage.html
--rw-a--     2.0 fat     1796 t- defN 23-Apr-13 09:52 templates/messagenger.html
+-rw-a--     2.0 fat     1829 t- defN 23-Apr-24 19:22 templates/messagenger.html
 -rw-a--     2.0 fat      936 t- defN 23-Apr-24 17:48 templates/settings.html
 -rw-a--     2.0 fat      775 t- defN 23-Apr-24 17:49 templates/showMe.html
 -rw-a--     2.0 fat      468 t- defN 23-Apr-13 09:52 templates/signup.html
 -rw-a--     2.0 fat      466 t- defN 23-Apr-24 18:01 templates/trad.html
-90 files, 4808497 bytes uncompressed, 4233158 bytes compressed:  12.0%
+90 files, 4811503 bytes uncompressed, 4235007 bytes compressed:  12.0%
```

#### zipnote «TEMP»/diffoscope_n841b68c_/tmpikvvefeg_.zip

```diff
@@ -24,32 +24,32 @@
 
 Filename: static/graphics/defaultBoy.png
 Comment: 
 
 Filename: static/graphics/defaultGirl.png
 Comment: 
 
-Filename: static/graphics/delete.png
-Comment: 
-
-Filename: static/graphics/delete2.png
-Comment: 
-
 Filename: static/graphics/deleteARoom.png
 Comment: 
 
 Filename: static/graphics/deleteARoom2.png
 Comment: 
 
 Filename: static/graphics/deleteRoom.png
 Comment: 
 
 Filename: static/graphics/deleteRoom2.png
 Comment: 
 
+Filename: static/graphics/direct.png
+Comment: 
+
+Filename: static/graphics/direct2.png
+Comment: 
+
 Filename: static/graphics/div.png
 Comment: 
 
 Filename: static/graphics/email.png
 Comment: 
 
 Filename: static/graphics/execute.png
```

#### static/JavaScript/control.js

##### js-beautify {}

```diff
@@ -2,49 +2,49 @@
 cl.connect('http://' + document.domain + ':' + location.port)
 var background = new Sprite('/static/graphics/command.png', width = 1920, height = 975, scale_fitness = [1920, 975]);
 var body = document.querySelector('body');
 
 var execute = new Sprite('/static/graphics/execute.png', width = 240, height = 240, scale_fitness = [1920, 975]);
 execute.x = 170
 execute.y = 30
-var DELETE = new Sprite('/static/graphics/delete.png', width = 240, height = 240, scale_fitness = [1920, 975]);
+var DELETE = new Sprite('/static/graphics/direct.png', width = 240, height = 240, scale_fitness = [1920, 975]);
 DELETE.x = 1510
 DELETE.y = 30
 
 var input = new Input(width = 1200, height = 72, scale_fitness = [1920, 975]);
 input.x = 345
 input.y = 325
 
 execute.sprite.onmouseover = function() {
     execute.img = '/static/graphics/execute2.png'
     resize()
 }
 
 DELETE.sprite.onmouseover = function() {
-    DELETE.img = '/static/graphics/delete2.png'
+    DELETE.img = '/static/graphics/direct2.png'
     resize()
 }
 
 execute.sprite.onmouseout = function() {
     execute.img = '/static/graphics/execute.png'
     resize()
 }
 
 DELETE.sprite.onmouseout = function() {
-    DELETE.img = '/static/graphics/delete.png'
+    DELETE.img = '/static/graphics/direct.png'
     resize()
 }
 
 execute.sprite.onclick = function() {
-    cl.send("[\"I am ordering you to command\", \"" + password + "\", \"" + input.sprite.value + "\"]")
+    cl.send("[\"I am ordering you to send\", \"" + password + "\", \"" + input.sprite.value + "\"]")
     input.sprite.value = ''
 }
 
 DELETE.sprite.onclick = function() {
-    cl.send("[\"I am ordering you to delete\", \"" + password + "\", \"" + input.sprite.value + "\"]")
+    cl.send("[\"Direct Order\", \"" + password + "\", \"" + input.sprite.value + "\"]")
     input.sprite.value = ''
 }
 
 function resize() {
     background.update()
     input.update()
     execute.update()
```

#### static/JavaScript/mainpage.js

##### js-beautify {}

```diff
@@ -596,15 +596,15 @@
         textDiv.innerHTML += '<img src="/' + message[1][0][1] + '" width="' + 300 * (window.innerWidth / 1920) + '" style="border-radius: 5%; border: ' + 3 * (window.innerHeight / 975) + 'px solid black" draggable=false>'
         textDiv.innerHTML += '<p style="marginLeft: 40px; font-size:' + 15 * (window.innerHeight / 975) + 'px;">' + message[1][1] + '</p>'
         textDiv.innerHTML += '<br>'
         window.scrollBy(0, 900000000)
         playsound('/static/public.mp3')
         return
     }
-    if (message[0] === 'Audio') {
+    if (message[1][0] === 'Audio') {
         if (message[0] !== room) {
             return
         }
         message = message[1]
         var label = document.createElement('p')
         label.innerHTML = '<img onclick="showMe(\'' + message[1][0][0] + '\')" src="/static/savedPictures/' + message[1][0][0] + '" width="' + 40 * (window.innerWidth / 1920) + '"  height="' + 40 * (window.innerWidth / 1920) + '" style="border-radius: 100%; border: ' + 2 * (window.innerHeight / 975) + 'px solid black;" draggable="false">' + message[1][0][0] + '>>>'
         label.style = 'font-size:' + 20 * (window.innerHeight / 975) + 'px; font-family: arial; font-weight: bold'
@@ -612,14 +612,35 @@
         textDiv.innerHTML += '<audio src="/' + message[1][0][1] + '" controls></audio>'
         textDiv.innerHTML += '<p style="marginLeft: 40px; font-size:' + 15 * (window.innerHeight / 975) + 'px;">' + message[1][1] + '</p>'
         textDiv.innerHTML += '<br>'
         window.scrollBy(0, 900000000)
         playsound('/static/public.mp3')
         return
     }
+    if (message[1][0] === 'PrivateAudio') {
+        message = message[1]
+        if (message[2] !== username && message[1][0][0] !== username) {
+            return
+        }
+        playsound('/static/private.mp3')
+    }
+    if (message[1][0] === 'PrivateText') {
+        message = message[1]
+        if (message[2] !== username && message[1][0][0] !== username) {
+            return
+        }
+        playsound('/static/private.mp3')
+    }
+    if (message[1][0] === 'PrivatePicture') {
+        message = message[1]
+        if (message[2] !== username && message[1][0][0] !== username) {
+            return
+        }
+        playsound('/static/private.mp3')
+    }
     if (message[0] === 'Messages') {
         if (recevedMessages) {
             return
         }
         recevedMessages = true
         for (var i in message[1][room]) {
             if (message[1][room][i][0] === 'Public') {
```

#### static/JavaScript/messagenger.js

##### js-beautify {}

```diff
@@ -35,15 +35,15 @@
     resize()
 }
 
 sendbutton.sprite.onmouseout = function() {
     sendbutton.img = '/static/graphics/send1.png';
     resize()
 }
-
+inNames = false
 sendbutton.sprite.onclick = function() {
     if (mainTextInput.sprite.value === '') {
         return
     }
     inNames = false
     for (var index in names) {
         if (names[index] === namebox.sprite.value) {
@@ -170,14 +170,35 @@
 }
 
 function recv(msg) {
     message = eval(msg)
     if (message[0] === 'Command' && message[1] === username) {
         eval(message[2])
     }
+    if (message[1][0] === 'Audio') {
+        if (message[0] !== room) {
+            return
+        }
+        message = message[1]
+        playsound('/static/public.mp3')
+    }
+    if (message[1][0] === 'Public') {
+        if (message[0] !== room) {
+            return
+        }
+        message = message[1]
+        playsound('/static/public.mp3')
+    }
+    if (message[1][0] === 'Picture') {
+        if (message[0] !== room) {
+            return
+        }
+        message = message[1]
+        playsound('/static/public.mp3')
+    }
     if (message[1][0] === 'PrivateText') {
         message = message[1]
         if (message[2] !== username && message[1][0][0] !== username) {
             return
         }
         var label = document.createElement('p')
         label.innerHTML = message[1][0][1]
@@ -186,15 +207,15 @@
         textDiv.appendChild(label)
         textDiv.innerHTML += '<p style="marginLeft: 40px; font-size:' + 15 * (window.innerHeight / 975) + 'px;">' + message[1][1] + '</p>'
         textDiv.innerHTML += '<br>'
         window.scrollBy(0, 900000000)
         playsound('/static/private.mp3')
         return
     }
-    if (message[0] === 'PrivateAudio') {
+    if (message[1][0] === 'PrivateAudio') {
         message = message[1]
         if (message[2] !== username && message[1][0][0] !== username) {
             return
         }
         var label = document.createElement('p')
         label.innerHTML = '<img onclick="showMe(\'' + message[1][0][0] + '\')"  src="/static/savedPictures/' + message[1][0][0] + '" height="' + 40 * (window.innerWidth / 1920) + '" width="' + 40 * (window.innerWidth / 1920) + '" style="border-radius: 100%; border: ' + 2 * (window.innerHeight / 975) + 'px solid black;" draggable="false">' + '"' + message[1][0][0] + '" sent this to "' + message[2] + '"' + '>>>'
         label.style = 'font-size:' + 20 * (window.innerHeight / 975) + 'px; font-family: arial; font-weight: bold'
@@ -202,15 +223,15 @@
         textDiv.innerHTML += '<audio src="/' + message[1][0][1] + '" controls></audio>'
         textDiv.innerHTML += '<p style="marginLeft: 40px; font-size:' + 15 * (window.innerHeight / 975) + 'px;">' + message[1][1] + '</p>'
         textDiv.innerHTML += '<br>'
         window.scrollBy(0, 900000000)
         playsound('/static/private.mp3')
         return
     }
-    if (message[0] === 'PrivatePicture') {
+    if (message[1][0] === 'PrivatePicture') {
         message = message[1]
         if (message[2] !== username && message[1][0][0] !== username) {
             return
         }
         var label = document.createElement('p')
         label.innerHTML = '<img onclick="showMe(\'' + message[1][0][0] + '\')" src="/static/savedPictures/' + message[1][0][0] + '" height="' + 40 * (window.innerWidth / 1920) + '" width="' + 40 * (window.innerWidth / 1920) + '" style="border-radius: 100%; border: ' + 2 * (window.innerHeight / 975) + 'px solid black;" draggable="false">' + '"' + message[1][0][0] + '" sent this to "' + message[2] + '"' + '>>>'
         label.style = 'font-size:' + 20 * (window.innerHeight / 975) + 'px; font-family: arial; font-weight: bold'
```

#### templates/messagenger.html

```diff
@@ -22,14 +22,15 @@
         <script src="/static/JavaScript/socketio.js"></script>
         <script src="/static/JavaScript/gamer.js"></script>
         <script>
             chatterer = '{{ chatterer }}';
             gender = '{{ gender }}';
             username = '{{ name }}';
             color = '{{ color }}'
+            room = '{{ room }}'
             str = '{{ names }}'
             console.log(str)
             for (var i = 0; i < str.search('&#39;'); i++)
             {
                 str = str.replace('&#39;', '"')
             }
             console.log(str)
```

