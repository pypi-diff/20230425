# Comparing `tmp/discordlevelingcard-0.4.8.tar.gz` & `tmp/discordlevelingcard-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordlevelingcard-0.4.8.tar", max compression
+gzip compressed data, was "discordlevelingcard-0.4.9.tar", max compression
```

## Comparing `discordlevelingcard-0.4.8.tar` & `discordlevelingcard-0.4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       71 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.8/DiscordLevelingCard/__init__.py
--rw-r--r--   0        0        0      842 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.8/DiscordLevelingCard/assets/curveborder.png
--rw-r--r--   0        0        0     2596 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.8/DiscordLevelingCard/assets/curvedoverlay.png
--rw-r--r--   0        0        0    60288 2023-01-08 10:51:38.103076 discordlevelingcard-0.4.8/DiscordLevelingCard/assets/levelfont.otf
--rw-r--r--   0        0        0     9742 2023-01-08 10:51:38.118707 discordlevelingcard-0.4.8/DiscordLevelingCard/assets/mask_circle.jpg
--rw-r--r--   0        0        0     6394 2023-01-08 10:51:38.118707 discordlevelingcard-0.4.8/DiscordLevelingCard/assets/overlay1.png
--rw-r--r--   0        0        0     2590 2023-01-24 08:45:29.025994 discordlevelingcard-0.4.8/DiscordLevelingCard/card_settings.py
--rw-r--r--   0        0        0    10960 2023-01-08 11:15:18.842661 discordlevelingcard-0.4.8/DiscordLevelingCard/discord_card.py
--rw-r--r--   0        0        0      531 2023-01-08 10:51:38.212709 discordlevelingcard-0.4.8/DiscordLevelingCard/error.py
--rw-r--r--   0        0        0     1083 2023-01-08 11:22:52.135512 discordlevelingcard-0.4.8/LICENSE
--rw-r--r--   0        0        0      888 2023-01-24 08:46:02.485939 discordlevelingcard-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4304 2023-01-08 11:32:26.731147 discordlevelingcard-0.4.8/README.md
--rw-r--r--   0        0        0     5106 2023-01-24 08:46:38.454386 discordlevelingcard-0.4.8/setup.py
--rw-r--r--   0        0        0     5043 2023-01-24 08:46:38.454386 discordlevelingcard-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.9/DiscordLevelingCard/__init__.py
+-rw-r--r--   0        0        0      842 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.9/DiscordLevelingCard/assets/curveborder.png
+-rw-r--r--   0        0        0     2596 2023-01-08 10:51:38.071812 discordlevelingcard-0.4.9/DiscordLevelingCard/assets/curvedoverlay.png
+-rw-r--r--   0        0        0    60288 2023-01-08 10:51:38.103076 discordlevelingcard-0.4.9/DiscordLevelingCard/assets/levelfont.otf
+-rw-r--r--   0        0        0     9742 2023-01-08 10:51:38.118707 discordlevelingcard-0.4.9/DiscordLevelingCard/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     6394 2023-01-08 10:51:38.118707 discordlevelingcard-0.4.9/DiscordLevelingCard/assets/overlay1.png
+-rw-r--r--   0        0        0     2590 2023-01-24 08:45:29.025994 discordlevelingcard-0.4.9/DiscordLevelingCard/card_settings.py
+-rw-r--r--   0        0        0    11170 2023-04-25 07:01:16.766267 discordlevelingcard-0.4.9/DiscordLevelingCard/discord_card.py
+-rw-r--r--   0        0        0      531 2023-01-08 10:51:38.212709 discordlevelingcard-0.4.9/DiscordLevelingCard/error.py
+-rw-r--r--   0        0        0     1083 2023-01-08 11:22:52.135512 discordlevelingcard-0.4.9/LICENSE
+-rw-r--r--   0        0        0      888 2023-04-25 07:03:26.041304 discordlevelingcard-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4358 2023-04-25 07:00:16.480431 discordlevelingcard-0.4.9/README.md
+-rw-r--r--   0        0        0     5160 2023-04-25 07:04:12.164740 discordlevelingcard-0.4.9/setup.py
+-rw-r--r--   0        0        0     5097 2023-04-25 07:04:12.164740 discordlevelingcard-0.4.9/PKG-INFO
```

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/assets/curveborder.png` & `discordlevelingcard-0.4.9/DiscordLevelingCard/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/assets/curvedoverlay.png` & `discordlevelingcard-0.4.9/DiscordLevelingCard/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/assets/levelfont.otf` & `discordlevelingcard-0.4.9/DiscordLevelingCard/assets/levelfont.otf`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/assets/mask_circle.jpg` & `discordlevelingcard-0.4.9/DiscordLevelingCard/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/assets/overlay1.png` & `discordlevelingcard-0.4.9/DiscordLevelingCard/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/card_settings.py` & `discordlevelingcard-0.4.9/DiscordLevelingCard/card_settings.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/discord_card.py` & `discordlevelingcard-0.4.9/DiscordLevelingCard/discord_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,16 @@
         ![card](https://cdn.discordapp.com/attachments/907213435358547968/1019966057294860328/final.png)
         """
         path = str(Path(__file__).parent)
 
         if isinstance(self.avatar, str):
             if self.avatar.startswith("http"):
                 self.avatar = await RankCard._image(self.avatar)
+        elif isinstance(self.avatar, Image.Image):
+            pass
         else:
             raise TypeError(f"avatar must be a url, not {type(self.avatar)}") 
 
         self.avatar = self.avatar.resize((170,170))
 
         overlay = Image.open(path + "/assets/overlay1.png")
         background = Image.new("RGBA", overlay.size)
@@ -180,14 +182,16 @@
         ![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)
         """
         path = str(Path(__file__).parent)
 
         if isinstance(self.avatar, str):
             if self.avatar.startswith("http"):
                 self.avatar = await RankCard._image(self.avatar)
+        elif isinstance(self.avatar, Image.Image):
+            pass
         else:
             raise TypeError(f"avatar must be a url, not {type(self.avatar)}") 
 
         background = Image.new("RGB", (1000, 333), self.background_color)
         background.paste(Image.new("RGB", (950, 333-50), "#2f3136"), (25, 25) )
 
         avatar = self.avatar.resize((260, 260))
@@ -239,14 +243,16 @@
         ![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)
         """
         path = str(Path(__file__).parent)
 
         if isinstance(self.avatar, str):
             if self.avatar.startswith("http"):
                 self.avatar = await RankCard._image(self.avatar)
+        elif isinstance(self.avatar, Image.Image):
+            pass
         else:
             raise TypeError(f"avatar must be a url, not {type(self.avatar)}") 
 
         background = self.background.resize((1000, 333))
         cut = Image.new("RGBA", (950, 333-50) , (0, 0, 0, 200))
         background.paste(cut, (25, 25) ,cut)
```

### Comparing `discordlevelingcard-0.4.8/DiscordLevelingCard/error.py` & `discordlevelingcard-0.4.9/DiscordLevelingCard/error.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/LICENSE` & `discordlevelingcard-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.4.8/pyproject.toml` & `discordlevelingcard-0.4.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordlevelingcard"
-version = "0.4.8"
+version = "0.4.9"
 readme = "README.md"
 description = "A library with leveling cards for your discord bot."
 repository = "https://github.com/krishsharma0413/DiscordLevelingCard"
 authors = ["Reset <krishsharma0413@gmail.com>"]
 license = "MIT"
 keywords = [
     "discord", "leveling", "card",
```

### Comparing `discordlevelingcard-0.4.8/README.md` & `discordlevelingcard-0.4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 [![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)
 
 ## card preview
 
 `card1`
 
-![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)
+![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)
 
 
 `card2`
-![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)
+![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)
 
 
 `card3` *same as card2 but with background*
 ![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)
 
 
 <br>
@@ -153,15 +153,15 @@
 RankCard.card1()
 ```
 
 `returns` - `bytes` which can directly be used within `discord.File` class.
 
 
 
-![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)
+![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)
 
 <br>
 
 </details>
 
 
 <details>
@@ -173,15 +173,15 @@
 RankCard.card2()
 ```
 
 `returns` - `bytes` which can directly be used within `discord.File` class.
 
 
 
-![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)
+![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)
 
 <br>
 
 </details>
 
 
 <details>
```

### Comparing `discordlevelingcard-0.4.8/setup.py` & `discordlevelingcard-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'DiscordLevelingCard': ['assets/*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0', 'aiohttp>=3.8.1,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'discordlevelingcard',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'A library with leveling cards for your discord bot.',
-    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n## card preview\n\n`card1`\n\n![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)\n\n\n`card2`\n![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)\n\n\n`card3` *same as card2 but with background*\n![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)\n\n\n<br>\n\n## installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n## How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n## Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)\n\n<br>\n\n</details>\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
+    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n## card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)\n\n\n<br>\n\n## installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n## How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n## Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)\n\n<br>\n\n</details>\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
     'author': 'Reset',
     'author_email': 'krishsharma0413@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/krishsharma0413/DiscordLevelingCard',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `discordlevelingcard-0.4.8/PKG-INFO` & `discordlevelingcard-0.4.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordlevelingcard
-Version: 0.4.8
+Version: 0.4.9
 Summary: A library with leveling cards for your discord bot.
 Home-page: https://github.com/krishsharma0413/DiscordLevelingCard
 License: MIT
 Keywords: discord,leveling,card,image,discord.py,disnake,nextcord,rank,ranking,level,discord-bot,bot,discord-leveling,level-card,discord-leveling-card,discord-rank-card
 Author: Reset
 Author-email: krishsharma0413@gmail.com
 Requires-Python: >=3.8,<4
@@ -24,19 +24,19 @@
 
 [![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)
 
 ## card preview
 
 `card1`
 
-![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)
+![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)
 
 
 `card2`
-![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)
+![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)
 
 
 `card3` *same as card2 but with background*
 ![card](https://cdn.discordapp.com/attachments/1018936393659076668/1022149875544113172/rank.png)
 
 
 <br>
@@ -174,15 +174,15 @@
 RankCard.card1()
 ```
 
 `returns` - `bytes` which can directly be used within `discord.File` class.
 
 
 
-![card1](https://cdn.discordapp.com/attachments/907213435358547968/994620579816681572/unknown.png)
+![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)
 
 <br>
 
 </details>
 
 
 <details>
@@ -194,15 +194,15 @@
 RankCard.card2()
 ```
 
 `returns` - `bytes` which can directly be used within `discord.File` class.
 
 
 
-![card](https://cdn.discordapp.com/attachments/907213435358547968/1020968412144480316/final.png)
+![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)
 
 <br>
 
 </details>
 
 
 <details>
```

