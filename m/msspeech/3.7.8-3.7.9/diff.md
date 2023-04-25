# Comparing `tmp/msspeech-3.7.8.tar.gz` & `tmp/msspeech-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msspeech-3.7.8.tar", max compression
+gzip compressed data, was "msspeech-3.7.9.tar", max compression
```

## Comparing `msspeech-3.7.8.tar` & `msspeech-3.7.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2280 2022-10-17 18:04:24.320105 msspeech-3.7.8/README.md
--rw-r--r--   0        0        0    19922 2022-10-17 18:04:24.320105 msspeech-3.7.8/msspeech/__init__.py
--rw-r--r--   0        0        0     2345 2022-10-17 18:04:24.320105 msspeech-3.7.8/msspeech/__main__.py
--rw-r--r--   0        0        0   116279 2022-10-17 18:04:24.324105 msspeech-3.7.8/msspeech/voices_list.json
--rw-r--r--   0        0        0     1153 2022-10-17 18:04:24.324105 msspeech-3.7.8/pyproject.toml
--rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 msspeech-3.7.8/setup.py
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 msspeech-3.7.8/PKG-INFO
+-rw-r--r--   0        0        0     2280 2022-10-18 12:08:34.597736 msspeech-3.7.9/README.md
+-rw-r--r--   0        0        0    20268 2022-10-18 12:08:34.597736 msspeech-3.7.9/msspeech/__init__.py
+-rw-r--r--   0        0        0     2345 2022-10-18 12:08:34.597736 msspeech-3.7.9/msspeech/__main__.py
+-rw-r--r--   0        0        0   116279 2022-10-18 12:08:34.597736 msspeech-3.7.9/msspeech/voices_list.json
+-rw-r--r--   0        0        0     1153 2022-10-18 12:08:34.597736 msspeech-3.7.9/pyproject.toml
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 msspeech-3.7.9/setup.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 msspeech-3.7.9/PKG-INFO
```

### Comparing `msspeech-3.7.8/README.md` & `msspeech-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `msspeech-3.7.8/msspeech/__init__.py` & `msspeech-3.7.9/msspeech/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import aiofiles  # type: ignore
 import os, os.path
 import html
 from typing import Any, List, Dict, Tuple, Optional, Union
 from urllib.parse import urlencode
 import aiohttp
 import json
+import math
 import ssl
 
 bytes_or_str = Union[str, bytes]
 list_of_voices = List[Dict[str, str]]
 
 msspeech_dir: str = os.path.dirname(__file__)
 if getattr(sys, "frozen", False):
@@ -68,34 +69,40 @@
     rate: int = 0
     config_sended: bool = False
 
     def __init__(self):
         """Create class instance"""
 
     @staticmethod
-    def _int_to_str(i: int) -> str:
-        return "+" + str(i) if i >= 0 else str(i)
+    def _normalize_volume(vol:float)->int:
+        return math.ceil(vol*100)
 
     @staticmethod
-    def _float_to_str(f: float) -> str:
-        return "+" + str(f) if f > 0 else str(f)
+    def _int_to_str(i: int) -> str:
+        return "+" + str(i) if i >= 0 else str(i)
 
     async def set_pitch(self, pitch: int) -> None:
-        self.pitch = int(pitch)
+        if abs(int(pitch)) <= 100:
+            self.pitch = int(pitch)
+        else:
+            raise ValueError("The pitch must be a negative or positive integer in the range from -100 to +100 or 0")
 
     async def set_volume(self, volume: float) -> None:
         "Set the speech volume"
         if float(volume) >= 0.1 and float(volume) <= 1.0:
             self.volume = float(volume)
         else:
             raise ValueError("The volume should be a fractional number from 0.1 to 1.0")
 
     async def set_rate(self, rate: int) -> None:
         "Set the speech rate"
-        self.rate = int(rate)
+        if abs(int(rate)) <= 100:
+            self.rate = int(rate)
+        else:
+            raise ValueError("The rate must be a negative or positive integer in the range from -100 to +100 or 0")
 
     async def get_pitch(self) -> int:
         "Get the speech pitch"
         return self.pitch
 
     async def get_volume(self) -> float:
         "Get the speech volume"
@@ -189,15 +196,15 @@
                         + """
 <voice  name='{voiceName}'><prosody pitch='{pitch}Hz' rate ='{rate}%' volume='{volume}'>{text_from_tag}</prosody></voice>
                     """.format(
                             voiceName=voice["ShortName"],
                             text_from_tag=text_from_tag,
                             pitch=default_pitch,
                             rate=self._int_to_str(default_rate),
-                            volume=self._float_to_str(default_volume),
+                            volume=self._normalize_volume(default_volume),
                         ).strip()
                         + open_voice_tag_if_needed
                     )
                     message = re.sub(
                         r"[%]{}[:].*".format(voice_name_from_tag),
                         replaced.replace("\\\\", "\\"),
                         message,
@@ -416,15 +423,15 @@
                 speak_element_close = "</speak>"
                 voice_element_open = """
     <voice  name='{voiceName}'><prosody pitch='{pitch}Hz' rate ='{rate}%' volume='{volume}'>
                 """.strip().format(
                     voiceName=self.voiceName,
                     pitch=self._int_to_str(self.pitch),
                     rate=self._int_to_str(self.rate),
-                    volume=self._float_to_str(self.volume),
+                    volume=self._normalize_volume(self.volume),
                 )
                 voice_element_close = "</prosody></voice>"
                 if (await self.get_voice())["Locale"][0:2].lower() == "ru":  # type: ignore
                     for k, v in {
                         "'": "ъ",
                     }.items():
                         text = text.replace(k, v)
```

### Comparing `msspeech-3.7.8/msspeech/__main__.py` & `msspeech-3.7.9/msspeech/__main__.py`

 * *Files identical despite different names*

### Comparing `msspeech-3.7.8/msspeech/voices_list.json` & `msspeech-3.7.9/msspeech/voices_list.json`

 * *Files identical despite different names*

### Comparing `msspeech-3.7.8/pyproject.toml` & `msspeech-3.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msspeech"
-version = "3.7.8"
+version = "3.7.9"
 description = "not official API for Microsoft speech synthesis from Microsoft Edge web browser read aloud"
 authors = ["Alexey <aleks-samos@yandex.ru>"]
 readme  = "README.md"
 repository  = "https://github.com/alekssamos/msspeech"
 include = ["msspeech/voices_list.json"]
 
 [tool.poetry.dependencies]
```

### Comparing `msspeech-3.7.8/setup.py` & `msspeech-3.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'console_scripts': ['msspeech = msspeech.__main__:main',
                      'msspeech-update-voices = msspeech.__main__:update_voices',
                      'msspeech_update_voices = '
                      'msspeech.__main__:update_voices']}
 
 setup_kwargs = {
     'name': 'msspeech',
-    'version': '3.7.8',
+    'version': '3.7.9',
     'description': 'not official API for Microsoft speech synthesis from Microsoft Edge web browser read aloud',
     'long_description': '# msspeech\nnot official API for Microsoft speech synthesis from Microsoft Edge web browser read aloud\n\n## Installation\n\n`pip install --upgrade msspeech`\n\nor\n\n`poetry add msspeech`\n\n\nAfter updating an already installed library\nTo update the list of voices, run the command in your terminal:\n\n`msspeech-update-voices`\n\nor\n\n`poetry run msspeech-update-voices`\n\n\n## Notes\n### Bad news\n\nSince the first of July 2022,\nthe list of voices and the API as a whole has been very much limited!\n\n### But there is also good news\n\nThey returned back some male voices and added new languages, as well as made support for emotional styles.\nDespite the fact that styles appeared in JSON, you still won\'t be able to use them, SSML does not perceive them.\nSSML is very limited here, so there is no point in supporting it.\n\nThe official documentation is not suitable for this API. It seems this API uses **undocumented** SSML markup.\n\nhttps://docs.microsoft.com/ru-ru/azure/cognitive-services/speech-service/language-support#text-to-speech\n\n## Using\nthe pitch and rate values are set as a percentage from -100 to +100,\nthat is, it can be a negative, positive number, or zero for the default value.\n\nexamples: -30, 40, 0\n\n\nThe volume should be a fractional number from 0.1 to 1.0, but in fact it doesn\'t work for some reason.\n\n\nThe maximum synthesize text length is approximately 31000 characters per request.\n\n### from CLI\n\nsynthesize text:\n\n`msspeech Guy hello --filename audio.mp3`\n\nupdate voices list:\n\n`msspeech-update-voices`\n\n### From python\n```python\nimport asyncio\nfrom msspeech import MSSpeech\n\n\nasync def main():\n\tmss = MSSpeech()\n\tprint("Geting voices...")\n\tvoices = await mss.get_voices_list()\n\tprint("searching Russian voice...")\n\tfor voice in voices:\n\t\tif voice["Locale"] == "ru-RU":\n\t\t\tprint("Russian voice found:", voice["FriendlyName"])\n\t\t\tawait mss.set_voice(voice["Name"])\n\n\n\tprint("*" * 10)\n\tfilename = "audio.mp3"\n\t# with open("s.txt", encoding="UTF8") as f: text:str = f.read()\n\ttext = "Или написать текст здесь"\n\tprint("waiting...")\n\tawait mss.set_rate(1)\n\tawait mss.set_pitch(0)\n\tawait mss.set_volume(1)\n\tawait mss.synthesize(text.strip(), filename)\n\tprint("*"*10)\n\tprint("SUCCESS! OK!")\n\tprint("*"*10)\n\nif __name__ == "__main__":\n\tasyncio.run(main())\n```\n',
     'author': 'Alexey',
     'author_email': 'aleks-samos@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/alekssamos/msspeech',
```

### Comparing `msspeech-3.7.8/PKG-INFO` & `msspeech-3.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msspeech
-Version: 3.7.8
+Version: 3.7.9
 Summary: not official API for Microsoft speech synthesis from Microsoft Edge web browser read aloud
 Home-page: https://github.com/alekssamos/msspeech
 Author: Alexey
 Author-email: aleks-samos@yandex.ru
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

