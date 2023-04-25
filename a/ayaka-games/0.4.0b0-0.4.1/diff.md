# Comparing `tmp/ayaka_games-0.4.0b0.tar.gz` & `tmp/ayaka_games-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayaka_games-0.4.0b0.tar", max compression
+gzip compressed data, was "ayaka_games-0.4.1.tar", max compression
```

## Comparing `ayaka_games-0.4.0b0.tar` & `ayaka_games-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,32 @@
--rw-r--r--   0        0        0      180 2023-02-03 07:11:40.167080 ayaka_games-0.4.0b0/ayaka_games/__init__.py
--rw-r--r--   0        0        0       50 2023-02-03 07:08:29.961074 ayaka_games-0.4.0b0/ayaka_games/bag/__init__.py
--rw-r--r--   0        0        0      737 2023-02-06 12:49:51.538854 ayaka_games-0.4.0b0/ayaka_games/bag/bag.py
--rw-r--r--   0        0        0     3078 2023-02-06 12:50:01.941313 ayaka_games-0.4.0b0/ayaka_games/bag/reputation.py
--rw-r--r--   0        0        0       37 2023-02-03 07:11:23.037483 ayaka_games-0.4.0b0/ayaka_games/calculate/__init__.py
--rw-r--r--   0        0        0     9352 2023-02-07 01:26:43.149549 ayaka_games-0.4.0b0/ayaka_games/calculate/calculate.py
--rw-r--r--   0        0        0      789 2023-02-03 09:40:30.043506 ayaka_games-0.4.0b0/ayaka_games/calculate/reputation.py
--rw-r--r--   0        0        0       35 2023-02-03 07:10:39.924893 ayaka_games-0.4.0b0/ayaka_games/checkin/__init__.py
--rw-r--r--   0        0        0      892 2023-02-06 12:50:18.149822 ayaka_games-0.4.0b0/ayaka_games/checkin/checkin.py
--rw-r--r--   0        0        0     1327 2023-02-06 12:50:31.264079 ayaka_games-0.4.0b0/ayaka_games/checkin/reputation.py
--rw-r--r--   0        0        0     2378 2023-02-07 01:25:40.538385 ayaka_games-0.4.0b0/ayaka_games/cy_query.py
--rw-r--r--   0        0        0     5465 2023-02-06 12:48:52.330478 ayaka_games-0.4.0b0/ayaka_games/dragon.py
--rw-r--r--   0        0        0     2227 2023-02-07 01:25:53.834010 ayaka_games-0.4.0b0/ayaka_games/genshin_random_event.py
--rw-r--r--   0        0        0     7805 2023-02-07 01:27:00.096157 ayaka_games-0.4.0b0/ayaka_games/get_30.py
--rw-r--r--   0        0        0    14296 2023-02-07 01:26:54.462916 ayaka_games-0.4.0b0/ayaka_games/incan.py
--rw-r--r--   0        0        0     7348 2023-02-06 12:49:15.819196 ayaka_games-0.4.0b0/ayaka_games/mana.py
--rw-r--r--   0        0        0     7680 2023-01-18 02:52:32.885076 ayaka_games-0.4.0b0/ayaka_games/plus_one.py
--rw-r--r--   0        0        0       32 2023-02-03 11:39:07.942473 ayaka_games-0.4.0b0/ayaka_games/pray/__init__.py
--rw-r--r--   0        0        0     1736 2023-02-07 01:25:10.725128 ayaka_games-0.4.0b0/ayaka_games/pray/pray.py
--rw-r--r--   0        0        0     3726 2023-02-03 12:26:55.506113 ayaka_games-0.4.0b0/ayaka_games/pray/reputation.py
--rw-r--r--   0        0        0       34 2023-02-03 03:43:48.950998 ayaka_games-0.4.0b0/ayaka_games/requirements.txt
--rw-r--r--   0        0        0      221 2023-02-06 12:47:09.909773 ayaka_games-0.4.0b0/ayaka_games/utils/__init__.py
--rw-r--r--   0        0        0      877 2023-02-07 00:50:33.842735 ayaka_games-0.4.0b0/ayaka_games/utils/config.py
--rw-r--r--   0        0        0       58 2023-02-06 12:46:57.875297 ayaka_games-0.4.0b0/ayaka_games/utils/database.py
--rw-r--r--   0        0        0     1758 2023-02-07 01:11:07.541949 ayaka_games-0.4.0b0/ayaka_games/utils/download.py
--rw-r--r--   0        0        0     4515 2023-02-06 12:48:15.081987 ayaka_games-0.4.0b0/ayaka_games/utils/reputation.py
--rw-r--r--   0        0        0       66 2023-02-03 08:08:34.636031 ayaka_games-0.4.0b0/ayaka_games/utils/subscribe.py
--rw-r--r--   0        0        0     8997 2023-01-24 11:29:32.902179 ayaka_games-0.4.0b0/ayaka_games/who_is_suspect.py
--rw-r--r--   0        0        0     7411 2023-02-06 12:49:34.763266 ayaka_games-0.4.0b0/ayaka_games/word_tax.py
--rw-r--r--   0        0        0     1091 2022-09-11 11:46:36.868866 ayaka_games-0.4.0b0/LICENSE
--rw-r--r--   0        0        0      460 2023-02-07 01:40:56.512770 ayaka_games-0.4.0b0/pyproject.toml
--rw-r--r--   0        0        0     1474 2023-02-07 01:38:43.261678 ayaka_games-0.4.0b0/readme.md
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 ayaka_games-0.4.0b0/setup.py
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 ayaka_games-0.4.0b0/PKG-INFO
+-rw-r--r--   0        0        0      180 2023-02-09 17:31:06.012072 ayaka_games-0.4.1/ayaka_games/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-03 07:08:29.961074 ayaka_games-0.4.1/ayaka_games/bag/__init__.py
+-rw-r--r--   0        0        0     1821 2023-04-25 02:05:08.426084 ayaka_games-0.4.1/ayaka_games/bag/bag.py
+-rw-r--r--   0        0        0     3091 2023-02-07 02:09:43.440849 ayaka_games-0.4.1/ayaka_games/bag/reputation.py
+-rw-r--r--   0        0        0       37 2023-02-03 07:11:23.037483 ayaka_games-0.4.1/ayaka_games/calculate/__init__.py
+-rw-r--r--   0        0        0     9359 2023-02-07 02:04:33.737097 ayaka_games-0.4.1/ayaka_games/calculate/calculate.py
+-rw-r--r--   0        0        0      748 2023-02-07 02:09:48.158105 ayaka_games-0.4.1/ayaka_games/calculate/reputation.py
+-rw-r--r--   0        0        0       35 2023-02-03 07:10:39.924893 ayaka_games-0.4.1/ayaka_games/checkin/__init__.py
+-rw-r--r--   0        0        0      904 2023-02-07 02:04:44.376617 ayaka_games-0.4.1/ayaka_games/checkin/checkin.py
+-rw-r--r--   0        0        0     1340 2023-02-07 02:09:50.788990 ayaka_games-0.4.1/ayaka_games/checkin/reputation.py
+-rw-r--r--   0        0        0     2386 2023-02-10 14:46:36.813700 ayaka_games-0.4.1/ayaka_games/cy_query.py
+-rw-r--r--   0        0        0     5437 2023-02-07 02:09:23.509651 ayaka_games-0.4.1/ayaka_games/dragon.py
+-rw-r--r--   0        0        0     2235 2023-02-07 02:02:17.598866 ayaka_games-0.4.1/ayaka_games/genshin_random_event.py
+-rw-r--r--   0        0        0     7805 2023-02-07 01:27:00.096157 ayaka_games-0.4.1/ayaka_games/get_30.py
+-rw-r--r--   0        0        0    14296 2023-02-07 01:26:54.462916 ayaka_games-0.4.1/ayaka_games/incan.py
+-rw-r--r--   0        0        0     7283 2023-02-07 02:09:26.784452 ayaka_games-0.4.1/ayaka_games/mana.py
+-rw-r--r--   0        0        0     7680 2023-01-18 02:52:32.885076 ayaka_games-0.4.1/ayaka_games/plus_one.py
+-rw-r--r--   0        0        0       32 2023-02-03 11:39:07.942473 ayaka_games-0.4.1/ayaka_games/pray/__init__.py
+-rw-r--r--   0        0        0     1743 2023-02-07 02:05:11.734395 ayaka_games-0.4.1/ayaka_games/pray/pray.py
+-rw-r--r--   0        0        0     3663 2023-02-07 02:11:04.204563 ayaka_games-0.4.1/ayaka_games/pray/reputation.py
+-rw-r--r--   0        0        0       34 2023-02-03 03:43:48.950998 ayaka_games-0.4.1/ayaka_games/requirements.txt
+-rw-r--r--   0        0        0      195 2023-02-07 02:01:31.517052 ayaka_games-0.4.1/ayaka_games/utils/__init__.py
+-rw-r--r--   0        0        0      877 2023-02-07 00:50:33.842735 ayaka_games-0.4.1/ayaka_games/utils/config.py
+-rw-r--r--   0        0        0     1758 2023-02-07 01:11:07.541949 ayaka_games-0.4.1/ayaka_games/utils/download.py
+-rw-r--r--   0        0        0     4481 2023-02-07 02:23:05.891981 ayaka_games-0.4.1/ayaka_games/utils/reputation.py
+-rw-r--r--   0        0        0       66 2023-02-03 08:08:34.636031 ayaka_games-0.4.1/ayaka_games/utils/subscribe.py
+-rw-r--r--   0        0        0     8997 2023-01-24 11:29:32.902179 ayaka_games-0.4.1/ayaka_games/who_is_suspect.py
+-rw-r--r--   0        0        0     7382 2023-02-07 02:09:38.605816 ayaka_games-0.4.1/ayaka_games/word_tax.py
+-rw-r--r--   0        0        0     1091 2022-09-11 11:46:36.868866 ayaka_games-0.4.1/LICENSE
+-rw-r--r--   0        0        0      458 2023-04-25 02:05:52.829008 ayaka_games-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1072 2023-04-25 01:53:27.538658 ayaka_games-0.4.1/readme.md
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 ayaka_games-0.4.1/PKG-INFO
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/bag/reputation.py` & `ayaka_games-0.4.1/ayaka_games/bag/reputation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from ayaka import get_db
 from .bag import Money
-from ..utils import subscribe, set_over_type_reputaion, db
+from ..utils import subscribe, set_over_type_reputaion
 
+db = get_db("ayaka_games")
 
 @subscribe.cls_property_watch
 class MoneyAnalyse(db.UserDBBase, table=True):
-    __tablename__ = "money_analyse"
 
     fail_down_cnt: int = 0
     '''金币从正跌负的次数'''
     rise_up_cnt: int = 0
     '''金币从负回正的次数'''
     sum_get: int = 0
     '''累计获得金币'''
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/calculate/calculate.py` & `ayaka_games-0.4.1/ayaka_games/calculate/calculate.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import re
 from random import choice
 from pydantic import BaseModel
 from loguru import logger
 from ayaka import AyakaCat, load_data_from_file
 from .reputation import CalculateAnalyse
 from ..bag import Money
-from ..utils import downloader, config, db
+from ..utils import downloader, config
 
-cat = AyakaCat("24点",db=db)
+cat = AyakaCat("24点",db="ayaka_games")
 cat.help = '''
 加、减、乘、除、次方，5种运算符可用
 给出4个1-9范围内的数字，请通过以上运算符算出24点
 同时还有48点等其他模式可选，欢迎挑战
 '''
 
 questions_bin: dict[int, dict[str, list[str]]] = {}
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/calculate/reputation.py` & `ayaka_games-0.4.1/ayaka_games/calculate/reputation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ..utils import subscribe, AnalyseBase, set_over_type_reputaion
 
 
 @subscribe.cls_property_watch
 class CalculateAnalyse(AnalyseBase, table=True):
-    __tablename__ = "calculate_analyse"
 
     check_ans_cnt: int = 0
     '''查看答案次数'''
 
 
 set_over_type_reputaion(
     cls_attr=CalculateAnalyse.total_cnt,
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/checkin/checkin.py` & `ayaka_games-0.4.1/ayaka_games/checkin/checkin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''
     签到模块
 '''
 import datetime
 from ayaka import AyakaCat
 from ..bag import Money
-from ..utils import config, subscribe, db
+from ..utils import config, subscribe
 
-cat = AyakaCat('签到',db=db)
+cat = AyakaCat('签到', db="ayaka_games")
 
 
 @subscribe.cls_property_watch
-class Checkin(db.UserDBBase, table=True):
+class Checkin(cat.db.UserDBBase, table=True):
     last_date: str = ""
 
 
 @cat.on_cmd(cmds=['checkin', '签到'], always=True)
 async def checkin():
     date = str(datetime.datetime.now().date())
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/cy_query.py` & `ayaka_games-0.4.1/ayaka_games/cy_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
     成语查询
 '''
 from random import choice, sample
 from ayaka import AyakaCat, load_data_from_file
-from .utils import downloader, db
+from .utils import downloader
 
-cat = AyakaCat("成语查询",db=db)
+cat = AyakaCat("成语查询", db="ayaka_games")
 cat.help = '''
 有效提高群文学氛围
 
 数据来源：成语大全（20104条成语数据）
 '''
 
 search_dict = {}
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/dragon.py` & `ayaka_games-0.4.1/ayaka_games/dragon.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import re
 from random import choice
 from pypinyin import lazy_pinyin
 from pydantic import BaseModel
 from sqlmodel import Field, select, desc
 from ayaka import AyakaCat, load_data_from_file
 from .bag import Money
-from .utils import downloader, config, db
+from .utils import downloader, config
 
-cat = AyakaCat("接龙管理", db=db)
+cat = AyakaCat("接龙管理", db="ayaka_games")
 cat.help = '''接龙，在聊天时静默运行'''
 
 
 class Dragon(BaseModel):
     '''接龙词库'''
     name: str
     use: bool = True
@@ -43,17 +43,16 @@
         p = lazy_pinyin(word)[-1]
         words: list[str] = self.pinyin_dict.get(p)
         if not words:
             return ""
         return choice(words)
 
 
-class DragonUserData(db.UserDBBase, table=True):
+class DragonUserData(cat.db.UserDBBase, table=True):
     '''用户数据'''
-    __tablename__ = "dragon_user_data"
     dragon_name: str = Field(primary_key=True)
     cnt: int = 0
 
     @classmethod
     def get_or_create(cls, dragon_name: str):
         return cls._get_or_create(
             dragon_name=dragon_name,
@@ -102,15 +101,15 @@
 
             # 成功接龙
             if last and word:
                 p1 = lazy_pinyin(last)[-1]
                 p2 = lazy_pinyin(word)[0]
                 if p1 == p2:
                     # 修改金钱
-                    usermoney = Money.get_or_create(cat.group.id,cat.user.id)
+                    usermoney = Money.get_or_create(cat.group.id, cat.user.id)
                     usermoney.money += config.dragon_reward
                     await cat.send(f"[{cat.user.name}] 接龙成功！奖励{config.dragon_reward}金")
 
                     # 修改记录
                     user_data = DragonUserData.get_or_create(dragon.name)
                     user_data.cnt += 1
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/genshin_random_event.py` & `ayaka_games-0.4.1/ayaka_games/genshin_random_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
     原神随机事件
 '''
 from random import choice
 from typing import Literal
 from pydantic import BaseModel
 from ayaka import AyakaCat, load_data_from_file
-from .utils import downloader, db
+from .utils import downloader
 
-cat = AyakaCat("原神随机事件",db=db)
+cat = AyakaCat("原神随机事件", db="ayaka_games")
 
 
 class Group(BaseModel):
     type: Literal["Group"] = "Group"
     rules: list[str]
     parts: list["Part"]
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/get_30.py` & `ayaka_games-0.4.1/ayaka_games/get_30.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/incan.py` & `ayaka_games-0.4.1/ayaka_games/incan.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/mana.py` & `ayaka_games-0.4.1/ayaka_games/mana.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from asyncio import sleep
 from random import randint
 from ayaka import AyakaCat
 from .bag import Money
-from .utils import db
 
 god_names = ['欢愉', '悼亡', '深渊', '智慧']
 
-cat = AyakaCat('mana',db=db)
+cat = AyakaCat('mana', db="ayaka_games")
 cat.help = '''
 ===== m a n a =====
 欢愉、悼亡、深渊、智慧
 ===== ======= =====
 '''
 
 
-class ManaGod(db.GroupDBBase, table=True):
-    __tablename__ = "mana_god"
+class ManaGod(cat.db.GroupDBBase, table=True):
     name: str = "欢愉"
     power: int = 1
     cnt: int = 0
     mana: int = 0
 
     def say(self):
         words = {
@@ -40,16 +38,15 @@
 
         rs = words[self.name]
         r = rs[randint(0, len(rs)-1)]
         c = cs[self.name]
         return f"{r} {c} {self.power}"
 
 
-class UserMana(db.UserDBBase, table=True):
-    __tablename__ = "user_mana"
+class UserMana(cat.db.UserDBBase, table=True):
     mana: int = 10
 
 
 def change_god(god_name: str, god: ManaGod):
     god.name = god_name
     god.power = randint(1, 13)
     god.cnt = 0
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/plus_one.py` & `ayaka_games-0.4.1/ayaka_games/plus_one.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/pray/pray.py` & `ayaka_games-0.4.1/ayaka_games/pray/pray.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from random import randint
 from ayaka import AyakaCat
 from .reputation import PrayerAnalyse, BePrayedAnalyse
 from ..bag import Money
-from ..utils import config, db
+from ..utils import config
 
-cat = AyakaCat("pray", db=db)
+cat = AyakaCat("pray", db="ayaka_games")
 cat.help = '祈福'
 
 all_wegiht = 0
 for item in config.pray:
     all_wegiht += item.weight
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/pray/reputation.py` & `ayaka_games-0.4.1/ayaka_games/pray/reputation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from ..utils import subscribe, set_over_type_reputaion, AnalyseBase
 
 
 @subscribe.cls_property_watch
 class PrayerAnalyse(AnalyseBase, table=True):
-    __tablename__ = "prayer"
 
     total_money: int = 0
     '''通过祈祷，总共使他人获得的金币数'''
 
 
 @subscribe.cls_property_watch
 class BePrayedAnalyse(AnalyseBase, table=True):
-    __tablename__ = "be_prayed"
 
     total_money: int = 0
     '''因他人祈祷，总共获得的金币数'''
 
 
 set_over_type_reputaion(
     cls_attr=PrayerAnalyse.total_money,
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/utils/config.py` & `ayaka_games-0.4.1/ayaka_games/utils/config.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/utils/download.py` & `ayaka_games-0.4.1/ayaka_games/utils/download.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/utils/reputation.py` & `ayaka_games-0.4.1/ayaka_games/utils/reputation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import datetime
 from sqlmodel import Field, select
-from ayaka import AyakaCat, get_adapter
+from ayaka import AyakaCat
 from .subscribe import subscribe
-from .database import db
 
-cat = AyakaCat("成就", db=db)
-adapter = get_adapter()
+cat = AyakaCat("成就", db="ayaka_games")
+UserDBBase = cat.db.UserDBBase
 
 
-class AnalyseBase(db.UserDBBase):
+class AnalyseBase(UserDBBase):
     '''可以继承，统计一些基本的信息'''
     total_cnt: int = 0
     '''总次数'''
 
     done_cnt: int = 0
     '''成功次数'''
     done_combo: int = 0
@@ -49,29 +48,31 @@
 
         if self.last_done < 0:
             self.fail_combo += 1
 
         self.last_done = -1
 
 
-class Reputation(db.UserDBBase, table=True):
+class Reputation(UserDBBase, table=True):
     name: str = Field(primary_key=True)
     label: str = Field(primary_key=True)
     desc: str
     rank: int
     time: str
 
     @property
     def info(self):
         return f"[{self.name}] {'★'*self.rank}\n{self.desc}"
 
     @classmethod
     def get_user_all_reputation(cls, group_id: str, user_id: str):
-        stmt = select(cls).filter_by(group_id=group_id,
-                                     user_id=user_id).order_by(cls.label, cls.rank)
+        stmt = select(cls).filter_by(
+            group_id=group_id,
+            user_id=user_id
+        ).order_by(cls.label, cls.rank)
         cursor = cat.db_session.exec(stmt)
         return cursor.all()
 
     @classmethod
     async def add(cls, group_id: str, user_id: str, label: str, name: str, desc: str, rank: int):
         '''添加并发送成就'''
         statement = select(cls).filter_by(
@@ -121,15 +122,15 @@
 
 def set_over_type_reputaion(cls_attr, rs: list[tuple[str, str, int]], reverse: bool = False, label: str | None = None):
     '''超过型成就'''
     if label is None:
         label = str(cls_attr)
 
     @subscribe.on_change(cls_attr)
-    async def _(old_value: int, new_value: int, ca: db.UserDBBase):
+    async def _(old_value: int, new_value: int, ca: UserDBBase):
         if reverse:
             old_value = -old_value
             new_value = -new_value
 
         gid = ca.group_id
         uid = ca.user_id
 
@@ -141,15 +142,15 @@
 
 def set_zero_type_reputaion(cls_attr, rs: list[tuple[str, str, int]], label: str | None = None, zero: int = 0):
     '''归零型成就'''
     if label is None:
         label = str(cls_attr)
 
     @subscribe.on_change(cls_attr)
-    async def _(old_value: int, new_value: int, ca: db.UserDBBase):
+    async def _(old_value: int, new_value: int, ca: UserDBBase):
         gid = ca.group_id
         uid = ca.user_id
 
         for i, r in enumerate(rs):
             N = r[2]
             if old_value >= N and new_value <= zero:
                 await Reputation.add(gid, uid, label, r[0], r[1], i+1)
```

### Comparing `ayaka_games-0.4.0b0/ayaka_games/who_is_suspect.py` & `ayaka_games-0.4.1/ayaka_games/who_is_suspect.py`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/ayaka_games/word_tax.py` & `ayaka_games-0.4.1/ayaka_games/word_tax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from random import sample
 from time import time
 from pydantic import BaseModel
 from sqlmodel import Field, select
 from ayaka import AyakaCat, load_data_from_file
 from .bag import Money
-from .utils import downloader, config,db
+from .utils import downloader, config
 
-cat = AyakaCat("文字税",db=db)
+cat = AyakaCat("文字税", db="ayaka_games")
 cat.help = '''知识付费（doge
 
 注意：只有买了文字的人之间才会相互交税，其他人不受影响'''
 
 words: list[str] = []
 
 
 @downloader.on_finish
 async def finish():
     path = downloader.BASE_DIR / "文字税.txt"
     words.extend(load_data_from_file(path))
 
 
-class UserWord(db.UserDBBase, table=True):
-    __tablename__ = "word_tax"
+class UserWord(cat.db.UserDBBase, table=True):
     word: str = Field(primary_key=True)
     uname: str = ""
     time: int = 0
 
-class GroupWord(db.GroupDBBase, table=True):
-    __tablename__ = "word_tax_group"
+
+class GroupWord(cat.db.GroupDBBase, table=True):
     words: str = ""
     time: int = 0
 
 
 def get_user_words(group_id: str):
     stmt = select(UserWord).filter_by(group_id=group_id)
     cursor = cat.db_session.exec(stmt)
@@ -214,15 +213,16 @@
     if not check_dict:
         return
 
     user_moneys: dict[int, Money] = {}
     for users in check_dict.values():
         for u in users:
             if u.user_id not in user_moneys:
-                user_moneys[u.user_id] = Money.get_or_create(u.group_id, u.user_id)
+                user_moneys[u.user_id] = Money.get_or_create(
+                    u.group_id, u.user_id)
     user_moneys[cat.user.id] = Money.get_or_create(cat.group.id, cat.user.id)
 
     for w in check_dict.keys():
         msg = msg.replace(w, f"[{w}]")
     infos = [msg]
 
     for w, users in check_dict.items():
```

### Comparing `ayaka_games-0.4.0b0/LICENSE` & `ayaka_games-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayaka_games-0.4.0b0/readme.md` & `ayaka_games-0.4.1/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 
-# Ayaka小游戏合集 - 0.4.0
+# Ayaka小游戏合集 - 0.4.1
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ayaka_games)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/ayaka_games)
 ![PyPI - License](https://img.shields.io/pypi/l/ayaka_games)
 ![PyPI](https://img.shields.io/pypi/v/ayaka_games)
 
 开发进度 10/10
@@ -21,42 +21,16 @@
 
 也可将其作为console程序离线运行，便于调试
 
 ## 文档
 
 https://bridgel.github.io/ayaka_games/
 
-## 历史遗留问题
-
-如果你之前安装过`nonebot_plugin_ayaka_games`，请先确保它卸载干净
-
-```
-pip uninstall nonebot_plugin_ayaka_games
-pip uninstall nonebot_plugin_ayaka
-```
-
-## 安装
-
-```
-pip install ayaka_games
-```
-
-## 作为console程序离线运行
-
-```py
-# run.py
-import ayaka.adapters.console as cat
-
-# 加载插件
-import ayaka_games
-
-if __name__ == "__main__":
-    cat.run()
-```
+## nb2安装
 
 ```
-python run.py
+nb plugin install ayaka_games
 ```
 
 ## 其他
 
 本插件的前身：[nonebot_plugin_ayaka_games](https://github.com/bridgeL/nonebot-plugin-ayaka-games)
```

### Comparing `ayaka_games-0.4.0b0/PKG-INFO` & `ayaka_games-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayaka-games
-Version: 0.4.0b0
+Version: 0.4.1
 Summary: ayaka小游戏合集
 Home-page: https://github.com/bridgeL/ayaka_games
 License: MIT
 Author: Su
 Author-email: wxlxy316@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Requires-Dist: ayaka (>=0.0.4.0,<0.0.5.0)
 Requires-Dist: pypinyin (>=0.47.1)
 Project-URL: Repository, https://github.com/bridgeL/ayaka_games
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-# Ayaka小游戏合集 - 0.4.0
+# Ayaka小游戏合集 - 0.4.1
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ayaka_games)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/ayaka_games)
 ![PyPI - License](https://img.shields.io/pypi/l/ayaka_games)
 ![PyPI](https://img.shields.io/pypi/v/ayaka_games)
 
 开发进度 10/10
@@ -39,43 +39,17 @@
 
 也可将其作为console程序离线运行，便于调试
 
 ## 文档
 
 https://bridgel.github.io/ayaka_games/
 
-## 历史遗留问题
-
-如果你之前安装过`nonebot_plugin_ayaka_games`，请先确保它卸载干净
-
-```
-pip uninstall nonebot_plugin_ayaka_games
-pip uninstall nonebot_plugin_ayaka
-```
-
-## 安装
-
-```
-pip install ayaka_games
-```
-
-## 作为console程序离线运行
-
-```py
-# run.py
-import ayaka.adapters.console as cat
-
-# 加载插件
-import ayaka_games
-
-if __name__ == "__main__":
-    cat.run()
-```
+## nb2安装
 
 ```
-python run.py
+nb plugin install ayaka_games
 ```
 
 ## 其他
 
 本插件的前身：[nonebot_plugin_ayaka_games](https://github.com/bridgeL/nonebot-plugin-ayaka-games)
```

