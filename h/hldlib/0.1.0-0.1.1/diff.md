# Comparing `tmp/hldlib-0.1.0.tar.gz` & `tmp/hldlib-0.1.1.tar.gz`

## Comparing `hldlib-0.1.0.tar` & `hldlib-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 hldlib-0.1.0/examples/enemy_randomizer.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hldlib-0.1.0/examples/hlddir.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hldlib-0.1.0/examples/transfer_savefile.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hldbasics.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hlddirections.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hlderror.py
--rw-r--r--   0        0        0    11471 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hldlevel.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hldobjects.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hldsavefile.py
--rw-r--r--   0        0        0    15928 2020-02-02 00:00:00.000000 hldlib-0.1.0/src/hldlib/hldtype.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 hldlib-0.1.0/tests/hldbasics_test.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hldlib-0.1.0/tests/hldlevel_test.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hldlib-0.1.0/tests/hldobj_test.py
--rw-r--r--   0        0        0    20215 2020-02-02 00:00:00.000000 hldlib-0.1.0/tests/hldsavefile_test.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 hldlib-0.1.0/.gitignore
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hldlib-0.1.0/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hldlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 hldlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 hldlib-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 hldlib-0.1.1/examples/enemy_randomizer.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hldlib-0.1.1/examples/hlddir.txt
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hldlib-0.1.1/examples/transfer_savefile.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hldbasics.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hlddirections.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hlderror.py
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hldlevel.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hldobjects.py
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hldsavefile.py
+-rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 hldlib-0.1.1/src/hldlib/hldtype.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 hldlib-0.1.1/tests/hldbasics_test.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 hldlib-0.1.1/tests/hldlevel_test.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hldlib-0.1.1/tests/hldobj_test.py
+-rw-r--r--   0        0        0    20108 2020-02-02 00:00:00.000000 hldlib-0.1.1/tests/hldsavefile_test.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 hldlib-0.1.1/.gitignore
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hldlib-0.1.1/README.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hldlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 hldlib-0.1.1/PKG-INFO
```

### Comparing `hldlib-0.1.0/examples/enemy_randomizer.py` & `hldlib-0.1.1/examples/enemy_randomizer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from hldlib import default_load, find_path, HLDType
-import random
-
-def main():
-
-    list_of_enemies = [
-        "slime", "Birdman", "SmallCrystalSpider", "spider", "Grumpshroom",
-        "Wolf", "dirk",  "SpiralBombFrog", "RifleDirk",
-        "NinjaStarFrog", "TanukiGun", "CultBird", "missiledirk", "TanukiSword",
-        "Melty", "GhostBeamBird", "Leaper", "Dirkommander", "BlaDirk", "CrystalBaby"
-    ]
-
-    # Here we load all levels from path/North, path/East, path/..., path/Abyss
-    # find_path will search for the hlddir.txt file and read the first line there
-    levels = default_load(find_path())
-
-    for level in levels:
-        for obj in level.objects:
-            if obj.type == HLDType.SPAWNER:
-                if obj.attrs["-1"] in list_of_enemies and obj.attrs["-1"] != "Birdman":
-                    # Here we found an object that is of a type of Spawner (all enemies are from spawners for some reason)
-                    # In a Spawner "-1" attribute is the type of objcect to spawn so we choose a random enemy type
-                    # We are only looking for Spawners that will spawn enemies (i.e. from list_of_enemies)
-                    # and that will not spawn a Birdman (having them randomized can break arenas)
-                    #
-                    # So we assign a random enemy to "-1"
-                    # and we normalize other attributes (having them not normalized can break arenas too)
-                    obj.attrs["-1"] = random.choice(list_of_enemies)
-                    obj.attrs["-2"] = 0
-                    obj.attrs["-4"] = 1
-                    obj.attrs["-5"] = 0
-                    obj.attrs["-6"] = -1
-                    obj.attrs["-7"] = 0
-                    obj.attrs["-8"] = 0
-
-    # And in the end we dump all the changed levels
-    # NOTE: dump_all dumps levels in directories named after their direction
-    # So dump_all(path) will dump all levels with direction HLDDirection.NORTH in path/North
-    levels.dump_all("out")
-
-
-if __name__ == "__main__":
-    main()
+from hldlib import default_load, find_path, HLDType
+import random
+
+def main():
+
+    list_of_enemies = [
+        "slime", "Birdman", "SmallCrystalSpider", "spider", "Grumpshroom",
+        "Wolf", "dirk",  "SpiralBombFrog", "RifleDirk",
+        "NinjaStarFrog", "TanukiGun", "CultBird", "missiledirk", "TanukiSword",
+        "Melty", "GhostBeamBird", "Leaper", "Dirkommander", "BlaDirk", "CrystalBaby"
+    ]
+
+    # Here we load all levels from path/North, path/East, path/..., path/Abyss
+    # find_path will search for the hlddir.txt file and read the first line there
+    levels = default_load(find_path())
+
+    for level in levels:
+        for obj in level.objects:
+            if obj.type == HLDType.SPAWNER:
+                if obj.attrs["-1"] in list_of_enemies and obj.attrs["-1"] != "Birdman":
+                    # Here we found an object that is of a type of Spawner (all enemies are from spawners for some reason)
+                    # In a Spawner "-1" attribute is the type of objcect to spawn so we choose a random enemy type
+                    # We are only looking for Spawners that will spawn enemies (i.e. from list_of_enemies)
+                    # and that will not spawn a Birdman (having them randomized can break arenas)
+                    #
+                    # So we assign a random enemy to "-1"
+                    # and we normalize other attributes (having them not normalized can break arenas too)
+                    obj.attrs["-1"] = random.choice(list_of_enemies)
+                    obj.attrs["-2"] = 0
+                    obj.attrs["-4"] = 1
+                    obj.attrs["-5"] = 0
+                    obj.attrs["-6"] = -1
+                    obj.attrs["-7"] = 0
+                    obj.attrs["-8"] = 0
+
+    # And in the end we dump all the changed levels
+    # NOTE: dump_all dumps levels in directories named after their direction
+    # So dump_all(path) will dump all levels with direction HLDDirection.NORTH in path/North
+    levels.dump_all("out")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hldlib-0.1.0/examples/transfer_savefile.py` & `hldlib-0.1.1/examples/transfer_savefile.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from hldlib import HLDSaveFile
-
-def main():
-    # old_savefile is the savefile we want to transfer to a new machine
-    # new_savefile is a savefile from the new machine
-    old_savefile = HLDSaveFile.load("C://SavefileFrom.sav")
-    new_savefile = HLDSaveFile.load("C://SavefileTo.sav")
-
-    # In HLD savefiles are machine specific 
-    # So we transplant the new header to the old savefile
-    old_savefile.header = new_savefile.header
-
-    # And we dump the new ready-to-use savefile
-    old_savefile.dump("C://SavefileDone.sav")
-
-
-if __name__ == "__main__":
-    main()
+from hldlib import HLDSaveFile
+
+def main():
+    # old_savefile is the savefile we want to transfer to a new machine
+    # new_savefile is a savefile from the new machine
+    old_savefile = HLDSaveFile.load("C://SavefileFrom.sav")
+    new_savefile = HLDSaveFile.load("C://SavefileTo.sav")
+
+    # In HLD savefiles are machine specific 
+    # So we transplant the new header to the old savefile
+    old_savefile.header = new_savefile.header
+
+    # And we dump the new ready-to-use savefile
+    old_savefile.dump("C://SavefileDone.sav")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hldlib-0.1.0/src/hldlib/hldbasics.py` & `hldlib-0.1.1/src/hldlib/hldbasics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from pathlib import Path
-from hldlib.hldlevel import HLDLevel, HLDHolder
-from hldlib.hlderror import HLDError
-from hldlib.hlddirections import HLDDirection
-from typing import Iterable
-import os
-
-def find_path(textfile_name: str = "hlddir.txt", where_to_search: str | Path = ".") -> str:
-    """
-    An easy way to retrive a stored path. Searches in the specified directory and all subdirectories.
-    """
-    for dir_path, _, file_names in os.walk(where_to_search):
-        for file_name in file_names:
-            if file_name.lower() == textfile_name:
-                with open(os.path.join(dir_path, file_name)) as hld_dir_file:
-                    return hld_dir_file.readline().rstrip()
-    raise HLDError(f"No {textfile_name} found.")
-
-def get_levels(path: str | Path, dirs: Iterable[str]):
-    for directory in dirs:
-        for level in [level for level in os.listdir(os.path.join(path, directory)) if level.endswith(".lvl")]:
-            filepath: str = os.path.join(path, directory, level)
-            yield filepath, directory, level
-
-def default_load(path: str | Path) -> HLDHolder:
-    """
-    Default load method for loading levels from the basic HLD .lvl file structure.
-    
-    Gets all levels from path/North, path/East, path/..., path/Abyss
-    """
-    loaded = HLDHolder()
-    for level_path, _, _ in get_levels(path, HLDDirection):
-        lvl = HLDLevel.load(level_path)
-        loaded.append(lvl)
-    return loaded
-
-class Counter:
-    """
-    A simple counter class. Useful for creating new HLDObj's and giving them unique IDs.
-    """
-    def __init__(self, val: int = 10000):
-        self._val = val
-
-    def use(self) -> int:
-        self._val += 1
-        return self._val
+from pathlib import Path
+from hldlib.hldlevel import HLDLevel, HLDHolder
+from hldlib.hlderror import HLDError
+from hldlib.hlddirections import HLDDirection
+from typing import Iterable
+import os
+
+def find_path(textfile_name: str = "hlddir.txt", where_to_search: str | Path = ".") -> str:
+    """
+    An easy way to retrive a stored path. Searches in the specified directory and all subdirectories.
+    """
+    for dir_path, _, file_names in os.walk(where_to_search):
+        for file_name in file_names:
+            if file_name.lower() == textfile_name:
+                with open(os.path.join(dir_path, file_name)) as hld_dir_file:
+                    return hld_dir_file.readline().rstrip()
+    raise HLDError(f"No {textfile_name} found.")
+
+def get_levels(path: str | Path, dirs: Iterable[str]):
+    for directory in dirs:
+        for level in [level for level in os.listdir(os.path.join(path, directory)) if level.endswith(".lvl")]:
+            filepath: str = os.path.join(path, directory, level)
+            yield filepath, directory, level
+
+def default_load(path: str | Path) -> HLDHolder:
+    """
+    Default load method for loading levels from the basic HLD .lvl file structure.
+    
+    Gets all levels from path/North, path/East, path/..., path/Abyss
+    """
+    loaded = HLDHolder()
+    for level_path, _, _ in get_levels(path, HLDDirection):
+        lvl = HLDLevel.load(level_path)
+        loaded.append(lvl)
+    return loaded
+
+class Counter:
+    """
+    A simple counter class. Useful for creating new HLDObj's and giving them unique IDs.
+    """
+    def __init__(self, val: int = 10000):
+        self._val = val
+
+    def use(self) -> int:
+        self._val += 1
+        return self._val
```

### Comparing `hldlib-0.1.0/src/hldlib/hldlevel.py` & `hldlib-0.1.1/src/hldlib/hldlevel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,306 +1,305 @@
-import os
-from pathlib import Path
-import re
-from hldlib.hldobjects import HLDObj, _int_float_str_convert
-from hldlib.hlddirections import HLDDirection
-from hldlib.hlderror import HLDError
-from typing import Self
-
-
-class HLDLevel:
-    """
-    A python representation of a HLD level.
-    """
-
-    def __init__(self, name: str, date: float, layer_names: dict, room_settings: dict, objects: list[HLDObj], direction: HLDDirection) -> None:
-        self.name = name
-        self.date = date
-        self.layer_names = layer_names
-        self.room_settings = room_settings
-        self.objects = objects
-        self.direction = direction
-    
-    @classmethod
-    def load(cls, path: str | Path, direction: HLDDirection | None = None) -> Self:
-        """
-        Loads a level from path. If the direction is not set, uses the directory name as direction.
-        """
-        name = os.path.basename(path)
-        if not direction:
-            direction = HLDDirection(os.path.basename(os.path.dirname(path)))
-        with open(path, "r") as f:
-            return cls.from_string(f.read(), name, direction)
-
-    @classmethod    
-    def from_string(cls, string: str, name: str, direction: HLDDirection) -> Self:
-        """
-        Loads a level from a string.
-        """
-        lines = string.split("\n")
-        layer_names = {}
-        room_settings = {}
-        objects = []
-        i = 0
-
-        while not (match := re.match(r"(?:DATE|VERSION),(?P<date>.*?),", lines[i])): i += 1
-        date = float(match.group("date")); i += 1
-        while not (match := re.search(r"layerName,(?P<id>.*?),(?P<name>.*?),", lines[i])): i += 1
-        while (match := re.search(r"layerName,(?P<id>.*?),(?P<name>.*?),", lines[i])):
-            layer_names[int(match.group("id"))] = match.group("name")
-            i += 1
-        while not (match := re.search(r",floorSpr,", lines[i])): i += 1
-        split_line = list(map(_int_float_str_convert, lines[i].lstrip().split(",")[:-1]))
-        sketch = split_line[-4:]
-        rest_of_settings = iter(split_line[:-4])
-        for x in rest_of_settings:
-            room_settings[x] = next(rest_of_settings)
-        room_settings[sketch[0]] = [sketch[1], sketch[2], sketch[3]]
-        i += 1
-        for line in lines[i:]:
-            if re.search(r"obj,.*?,.*?,", line): objects.append(HLDObj.from_string(line))
-        
-        return cls(date=date, layer_names=layer_names, room_settings=room_settings, objects=objects, name=name, direction=direction)
-    
-
-    def dump(self, path: str | Path) -> None:
-        """
-        Dumps the level to path. Uses levels name as the dumped file name.
-        """
-        os.makedirs(path, exist_ok=True)
-        with open(os.path.join(path, self.name), "w") as file:
-            file.write(self.to_string())
-    
-    def to_string(self) -> str:
-        """
-        Gets the level in a string form. Can be used to write to a file.
-        """
-        return f"DATE,{self.date}," +\
-                "\n\t " + "\n\t ".join([f"layerName,{key},{value}," for key, value in self.layer_names.items()]) +\
-                "\n\t " + ",".join([f"{key},{value}" for key, value in self.room_settings.items() if key != "sketchalpha"]) +\
-                    f",sketchalpha,{','.join(list(map(str, self.room_settings['sketchalpha'])))}," +\
-                "".join([obj.to_string() for obj in self.objects])
-    
-
-    def __eq__(self, other: Self) -> bool:
-        if other.__class__ is not self.__class__: return False
-        return self.__dict__ == other.__dict__
-
-
-class HLDHolder(list[HLDLevel]):
-    """
-    A convenient list for levels with the ability to dump all levels.
-    """
-    def dump_all(self, path: str) -> None:
-        """
-        Dumps all levels.
-
-        NOTE: uses level direction as the dump directory name.
-        So dump_all(path) will dump all levels with direction HLDDirection.NORTH in path/North
-        """
-        for level in self:
-            level.dump(os.path.join(path, level.direction))
-
-level_names_and_ids: list[tuple[str, int]] = [
-    ("rm_IN_01_brokenshallows.lvl", 46),
-    ("rm_IN_02_Tutorial.lvl", 47),
-    ("rm_IN_03_Tut_Combat.lvl", 48),
-    ("rm_IN_HorizonCliff.lvl", 49),
-    ("rm_IN_HalucinationDeath.lvl", 50),
-    ("rm_IN_Drifterfire.lvl", 51),
-    ("rm_IN_BlackWaitRoom.lvl", 52),
-    ("rm_IN_BackerTablet.lvl", 53),
-    ("rm_INL_Secrets.lvl", 55),
-    ("rm_LIN_Gaps.lvl", 56),
-    ("rm_LIN_Combat.lvl", 57),
-    ("rm_C_DrifterWorkshop.lvl", 60),
-    ("rm_C_Central.lvl", 61),
-    ("rm_C_Dregs_N.lvl", 62),
-    ("rm_C_Dregs_S.lvl", 63),
-    ("rm_C_Dregs_E.lvl", 64),
-    ("rm_C_Dregs_W.lvl", 65),
-    ("rm_C_Ven_Apoth.lvl", 66),
-    ("rm_C_Ven_Dash.lvl", 67),
-    ("rm_C_Ven_Gun.lvl", 68),
-    ("rm_C_Ven_Spec.lvl", 69),
-    ("rm_C_Ven_SDojo.lvl", 70),
-    ("rm_CArena.lvl", 71),
-    ("rm_PAX_Staging.lvl", 72),
-    ("rm_PAX_arena1.lvl", 73),
-    ("rm_PAX_arena2.lvl", 74),
-    ("rm_PAX_arenaE.lvl", 75),
-    ("rm_PAX_arenaW.lvl", 76),
-    ("rm_PAX_arenaAll.lvl", 77),
-    ("rm_C_BackerTabletX.lvl", 78),
-    ("rm_TelevatorShaft.lvl", 79),
-    ("rm_NL_EntrancePath.lvl", 84),
-    ("rm_NX_TitanVista.lvl", 85),
-    ("rm_NX_NorthHall.lvl", 86),
-    ("rm_NL_CaveVAULT.lvl", 87),
-    ("rm_NX_AfterTitan.lvl", 88),
-    ("rm_NC_NPCHatchery.lvl", 89),
-    ("rm_NX_ShrinePath.lvl", 90),
-    ("rm_NL_ShrinePath2VAULT.lvl", 91),
-    ("rm_NX_Cave01.lvl", 92),
-    ("rm_NX_ShrinePath_2.lvl", 93),
-    ("rm_NX_MoonCourtyard.lvl", 94),
-    ("rm_NX_TowerLock.lvl", 95),
-    ("rm_NC_CliffCampfire.lvl", 96),
-    ("rm_NL_ToBrokenShallows.lvl", 97),
-    ("rm_NX_Stairs03.lvl", 98),
-    ("rm_NL_WarpRoom.lvl", 100),
-    ("rm_NL_CrushWarpHall.lvl", 101),
-    ("rm_NL_CrushTransition.lvl", 102),
-    ("rm_NL_CrushBackLoop.lvl", 103),
-    ("rm_NC_CrushArena.lvl", 104),
-    ("rm_NL_DropSpiralOpen.lvl", 106),
-    ("rm_NL_DropPits.lvl", 107),
-    ("rm_NL_DropBlockCultFight.lvl", 108),
-    ("rm_NL_DropArena.lvl", 109),
-    ("rm_NL_GapOpening.lvl", 111),
-    ("rm_NX_GapWide.lvl", 112),
-    ("rm_NL_GapHallway.lvl", 113),
-    ("rm_NL_RisingArena.lvl", 114),
-    ("rm_NX_CathedralEntrance.lvl", 116),
-    ("rm_NX_CathedralHall.lvl", 117),
-    ("rm_NL_AltarThrone.lvl", 118),
-    ("rm_NX_SpiralStaircase.lvl", 119),
-    ("rm_NX_LibrarianTablet.lvl", 120),
-    ("rm_NX_JerkPope.lvl", 121),
-    ("rm_NL_StairAscent.lvl", 123),
-    ("rm_NL_CrushArena.lvl", 124),
-    ("rm_SX_SouthOpening.lvl", 128),
-    ("rm_CH_CTemplate.lvl", 129),
-    ("rm_SX_TowerSouth.lvl", 130),
-    ("rm_SX_NPC.lvl", 131),
-    ("rm_S_Gauntlet_Elevator.lvl", 132),
-    ("rm_CH_BGunPillars.lvl", 133),
-    ("rm_CH_BFinal.lvl", 134),
-    ("rm_S_GauntletEnd.lvl", 135),
-    ("rm_CH_BDirkDemolition.lvl", 137),
-    ("rm_CH_TABigOne.lvl", 139),
-    ("rm_CH_CGateBlock.lvl", 140),
-    ("rm_CH_BMadDash.lvl", 141),
-    ("rm_CH_TLongestRoad.lvl", 142),
-    ("rm_S_BulletBaker.lvl", 143),
-    ("rm_CH_CEndHall.lvl", 144),
-    ("rm_CH_CTurnHall.lvl", 146),
-    ("rm_CH_Bfps.lvl", 147),
-    ("rm_CH_CBigggns.lvl", 148),
-    ("rm_CH_CSpawnGround.lvl", 149),
-    ("rm_S_CountAculard.lvl", 150),
-    ("rm_CH_ACorner.lvl", 152),
-    ("rm_CH_BDirkDeluge.lvl", 154),
-    ("rm_CH_BPods.lvl", 155),
-    ("rm_CH_BGunDirkDash.lvl", 156),
-    ("rm_S_MarkScythe.lvl", 157),
-    ("rm_S_GauntletLinkup.lvl", 158),
-    ("rm_CH_APillarBird.lvl", 160),
-    ("rm_CH_CSpiral.lvl", 161),
-    ("rm_CH_TBirdStandoff.lvl", 162),
-    ("rm_CH_BLeaperFall.lvl", 163),
-    ("rm_S_BennyArrow.lvl", 164),
-    ("rm_S_GauntletTitanFinale.lvl", 165),
-    ("rm_EA_EastOpening.lvl", 171),
-    ("rm_EC_SwordBridge.lvl", 172),
-    ("rm_EL_FlameElevatorEnter.lvl", 173),
-    ("rm_EA_WaterTunnelLAB.lvl", 174),
-    ("rm_EC_ThePlaza.lvl", 175),
-    ("rm_EC_NPCDrugDen.lvl", 176),
-    ("rm_EX_TowerEast.lvl", 177),
-    ("rm_EB_BogStreet.lvl", 178),
-    ("rm_EC_PlazaToLoop.lvl", 179),
-    ("rm_EL_MegaHugeLAB.lvl", 181),
-    ("rm_EB_MeltyMashArena.lvl", 182),
-    ("rm_EB_FlamePitLAB.lvl", 183),
-    ("rm_EL_FlameElevatorExit.lvl", 184),
-    ("rm_EB_DeadOtterWalk.lvl", 185),
-    ("rm_EC_PlazaAccessLAB.lvl", 187),
-    ("rm_EC_DocksLab.lvl", 188),
-    ("rm_EX_DocksCampfire.lvl", 189),
-    ("rm_EV_DocksBridge.lvl", 190),
-    ("rm_EL_FrogArena.lvl", 191),
-    ("rm_EC_BigBogLAB.lvl", 193),
-    ("rm_EA_BogTempleCamp.lvl", 194),
-    ("rm_EA_FrogBoss.lvl", 195),
-    ("rm_EC_TempleIshVault.lvl", 196),
-    ("rm_EC_EastLoop.lvl", 198),
-    ("rm_EC_LoopLAB.lvl", 199),
-    ("rm_EB_MeltyLeaperArena.lvl", 200),
-    ("rm_EC_PlazaToDocks.lvl", 202),
-    ("rm_EA_DockFightLab.lvl", 203),
-    ("rm_EB_UnderOtterBigRifleRumble.lvl", 204),
-    ("rm_EB_CleanersHole.lvl", 205),
-    ("rm_WA_Entrance.lvl", 209),
-    ("rm_WL_PrisonHALVAULT.lvl", 210),
-    ("rm_WA_Deadwood.lvl", 211),
-    ("rm_WA_DeadwoodS1.lvl", 212),
-    ("rm_WA_Grotto_buffIntro.lvl", 213),
-    ("rm_WC_WindingWood.lvl", 214),
-    ("rm_WC_GrottoNPC.lvl", 215),
-    ("rm_WL_NPCTreehouse.lvl", 216),
-    ("rm_WC_MiniLab.lvl", 217),
-    ("rm_WT_TheWood.lvl", 218),
-    ("rm_WA_EntSwitch.lvl", 219),
-    ("rm_WC_MeadowoodCorner.lvl", 220),
-    ("rm_WB_TreeTreachery.lvl", 222),
-    ("rm_WL_WestDrifterVault.lvl", 223),
-    ("rm_WT_SlowLab.lvl", 225),
-    ("rm_WC_CliffsideCellsRedux.lvl", 226),
-    ("rm_WC_PrisonHAL.lvl", 227),
-    ("rm_WC_ThinForest.lvl", 229),
-    ("rm_WC_SimplePath.lvl", 230),
-    ("rm_WC_CrystalLake.lvl", 231),
-    ("rm_WC_CrystalLakeVault.lvl", 232),
-    ("rm_WC_PrisonHallEnd.lvl", 233),
-    ("rm_WC_ThinForestLow.lvl", 234),
-    ("rm_WC_ThinForestLowSecret.lvl", 235),
-    ("rm_WA_TitanFalls.lvl", 236),
-    ("rm_WA_Vale.lvl", 238),
-    ("rm_WC_BigMeadow.lvl", 239),
-    ("rm_WC_BigMeadowVAULT.lvl", 240),
-    ("rm_WC_MeadowCaveCrossing.lvl", 241),
-    ("rm_WB_BigBattle.lvl", 242),
-    ("rm_WB_TanukiTrouble.lvl", 243),
-    ("rm_WC_RuinClearing.lvl", 244),
-    ("rm_WX_Boss.lvl", 245),
-    ("rm_WA_TowerEnter.lvl", 246),
-    ("rm_WA_MultiEntranceLab.lvl", 247),
-    ("rm_WA_CrsytalDescent.lvl", 248),
-    ("rm_WA_GrottoX.lvl", 250),
-    ("rm_WB_CrystalQueen.lvl", 251),
-    ("rm_WT_ProtoGrid.lvl", 252),
-    ("rm_WV_PuzzlePalaceNEW.lvl", 253),
-    ("rm_A_ElevatorShaftUpper.lvl", 256),
-    ("rm_A_ElevatorShaft.lvl", 257),
-    ("rm_A_PreDownward.lvl", 258),
-    ("rm_A_Downward.lvl", 259),
-    ("rm_A_DownwardDead.lvl", 260),
-    ("rm_A_DownwardDeadRevisit.lvl", 261),
-    ("rm_A_EmberRoom.lvl", 262),
-    ("rm_BossRush_Hub.lvl", 265),
-    ("rm_BossRush_FrogBoss.lvl", 266),
-    ("rm_BossRush_JerkPope.lvl", 267),
-    ("rm_BossRush_General.lvl", 268),
-    ("rm_BossRush_BulletBaker.lvl", 269),
-    ("rm_BossRush_CountAculard.lvl", 270),
-    ("rm_BossRush_MarkScythe.lvl", 271),
-    ("rm_BossRush_BennyArrow.lvl", 272),
-    ("rm_BossRush_Ember.lvl", 273),
-    ("rm_C_DrifterWorkshop.lvl", 276)
-]
-
-def get_id_from_name(name: str) -> int:
-    """
-    A way to convert internal level ID to its name.
-    """
-    for namee, idd in level_names_and_ids:
-        if namee == name: return idd
-    raise HLDError(f"No such level named {name}.")
-
-def get_name_from_id(id_: int) -> str:
-    """
-    A way to convert level name to its internal ID.
-    """
-    for namee, idd in level_names_and_ids:
-        if idd == id_: return namee
-    raise HLDError(f"No such level with id {id_}.")
+import os
+from pathlib import Path
+import re
+from hldlib.hldobjects import HLDObj, _int_float_str_convert
+from hldlib.hlddirections import HLDDirection
+from hldlib.hlderror import HLDError
+
+
+class HLDLevel:
+    """
+    A python representation of a HLD level.
+    """
+
+    def __init__(self, name: str, date: float, layer_names: dict, room_settings: dict, objects: list[HLDObj], direction: HLDDirection) -> None:
+        self.name = name
+        self.date = date
+        self.layer_names = layer_names
+        self.room_settings = room_settings
+        self.objects = objects
+        self.direction = direction
+    
+    @classmethod
+    def load(cls, path: str | Path, direction: HLDDirection | None = None):
+        """
+        Loads a level from path. If the direction is not set, uses the directory name as direction.
+        """
+        name = os.path.basename(path)
+        if not direction:
+            direction = HLDDirection(os.path.basename(os.path.dirname(path)))
+        with open(path, "r") as f:
+            return cls.from_string(f.read(), name, direction)
+
+    @classmethod    
+    def from_string(cls, string: str, name: str, direction: HLDDirection):
+        """
+        Loads a level from a string.
+        """
+        lines = string.split("\n")
+        layer_names = {}
+        room_settings = {}
+        objects = []
+        i = 0
+
+        while not (match := re.match(r"(?:DATE|VERSION),(?P<date>.*?),", lines[i])): i += 1
+        date = float(match.group("date")); i += 1
+        while not (match := re.search(r"layerName,(?P<id>.*?),(?P<name>.*?),", lines[i])): i += 1
+        while (match := re.search(r"layerName,(?P<id>.*?),(?P<name>.*?),", lines[i])):
+            layer_names[int(match.group("id"))] = match.group("name")
+            i += 1
+        while not (match := re.search(r",floorSpr,", lines[i])): i += 1
+        split_line = list(map(_int_float_str_convert, lines[i].lstrip().split(",")[:-1]))
+        sketch = split_line[-4:]
+        rest_of_settings = iter(split_line[:-4])
+        for x in rest_of_settings:
+            room_settings[x] = next(rest_of_settings)
+        room_settings[sketch[0]] = [sketch[1], sketch[2], sketch[3]]
+        i += 1
+        for line in lines[i:]:
+            if re.search(r"obj,.*?,.*?,", line): objects.append(HLDObj.from_string(line))
+        
+        return cls(date=date, layer_names=layer_names, room_settings=room_settings, objects=objects, name=name, direction=direction)
+    
+
+    def dump(self, path: str | Path) -> None:
+        """
+        Dumps the level to path. Uses levels name as the dumped file name.
+        """
+        os.makedirs(path, exist_ok=True)
+        with open(os.path.join(path, self.name), "w") as file:
+            file.write(self.to_string())
+    
+    def to_string(self) -> str:
+        """
+        Gets the level in a string form. Can be used to write to a file.
+        """
+        return f"DATE,{self.date}," +\
+                "\n\t " + "\n\t ".join([f"layerName,{key},{value}," for key, value in self.layer_names.items()]) +\
+                "\n\t " + ",".join([f"{key},{value}" for key, value in self.room_settings.items() if key != "sketchalpha"]) +\
+                    f",sketchalpha,{','.join(list(map(str, self.room_settings['sketchalpha'])))}," +\
+                "".join([obj.to_string() for obj in self.objects])
+    
+
+    def __eq__(self, other) -> bool:
+        if other.__class__ is not self.__class__: return False
+        return self.__dict__ == other.__dict__
+
+
+class HLDHolder(list[HLDLevel]):
+    """
+    A convenient list for levels with the ability to dump all levels.
+    """
+    def dump_all(self, path: str) -> None:
+        """
+        Dumps all levels.
+
+        NOTE: uses level direction as the dump directory name.
+        So dump_all(path) will dump all levels with direction HLDDirection.NORTH in path/North
+        """
+        for level in self:
+            level.dump(os.path.join(path, level.direction))
+
+level_names_and_ids: list[tuple[str, int]] = [
+    ("rm_IN_01_brokenshallows.lvl", 46),
+    ("rm_IN_02_Tutorial.lvl", 47),
+    ("rm_IN_03_Tut_Combat.lvl", 48),
+    ("rm_IN_HorizonCliff.lvl", 49),
+    ("rm_IN_HalucinationDeath.lvl", 50),
+    ("rm_IN_Drifterfire.lvl", 51),
+    ("rm_IN_BlackWaitRoom.lvl", 52),
+    ("rm_IN_BackerTablet.lvl", 53),
+    ("rm_INL_Secrets.lvl", 55),
+    ("rm_LIN_Gaps.lvl", 56),
+    ("rm_LIN_Combat.lvl", 57),
+    ("rm_C_DrifterWorkshop.lvl", 60),
+    ("rm_C_Central.lvl", 61),
+    ("rm_C_Dregs_N.lvl", 62),
+    ("rm_C_Dregs_S.lvl", 63),
+    ("rm_C_Dregs_E.lvl", 64),
+    ("rm_C_Dregs_W.lvl", 65),
+    ("rm_C_Ven_Apoth.lvl", 66),
+    ("rm_C_Ven_Dash.lvl", 67),
+    ("rm_C_Ven_Gun.lvl", 68),
+    ("rm_C_Ven_Spec.lvl", 69),
+    ("rm_C_Ven_SDojo.lvl", 70),
+    ("rm_CArena.lvl", 71),
+    ("rm_PAX_Staging.lvl", 72),
+    ("rm_PAX_arena1.lvl", 73),
+    ("rm_PAX_arena2.lvl", 74),
+    ("rm_PAX_arenaE.lvl", 75),
+    ("rm_PAX_arenaW.lvl", 76),
+    ("rm_PAX_arenaAll.lvl", 77),
+    ("rm_C_BackerTabletX.lvl", 78),
+    ("rm_TelevatorShaft.lvl", 79),
+    ("rm_NL_EntrancePath.lvl", 84),
+    ("rm_NX_TitanVista.lvl", 85),
+    ("rm_NX_NorthHall.lvl", 86),
+    ("rm_NL_CaveVAULT.lvl", 87),
+    ("rm_NX_AfterTitan.lvl", 88),
+    ("rm_NC_NPCHatchery.lvl", 89),
+    ("rm_NX_ShrinePath.lvl", 90),
+    ("rm_NL_ShrinePath2VAULT.lvl", 91),
+    ("rm_NX_Cave01.lvl", 92),
+    ("rm_NX_ShrinePath_2.lvl", 93),
+    ("rm_NX_MoonCourtyard.lvl", 94),
+    ("rm_NX_TowerLock.lvl", 95),
+    ("rm_NC_CliffCampfire.lvl", 96),
+    ("rm_NL_ToBrokenShallows.lvl", 97),
+    ("rm_NX_Stairs03.lvl", 98),
+    ("rm_NL_WarpRoom.lvl", 100),
+    ("rm_NL_CrushWarpHall.lvl", 101),
+    ("rm_NL_CrushTransition.lvl", 102),
+    ("rm_NL_CrushBackLoop.lvl", 103),
+    ("rm_NC_CrushArena.lvl", 104),
+    ("rm_NL_DropSpiralOpen.lvl", 106),
+    ("rm_NL_DropPits.lvl", 107),
+    ("rm_NL_DropBlockCultFight.lvl", 108),
+    ("rm_NL_DropArena.lvl", 109),
+    ("rm_NL_GapOpening.lvl", 111),
+    ("rm_NX_GapWide.lvl", 112),
+    ("rm_NL_GapHallway.lvl", 113),
+    ("rm_NL_RisingArena.lvl", 114),
+    ("rm_NX_CathedralEntrance.lvl", 116),
+    ("rm_NX_CathedralHall.lvl", 117),
+    ("rm_NL_AltarThrone.lvl", 118),
+    ("rm_NX_SpiralStaircase.lvl", 119),
+    ("rm_NX_LibrarianTablet.lvl", 120),
+    ("rm_NX_JerkPope.lvl", 121),
+    ("rm_NL_StairAscent.lvl", 123),
+    ("rm_NL_CrushArena.lvl", 124),
+    ("rm_SX_SouthOpening.lvl", 128),
+    ("rm_CH_CTemplate.lvl", 129),
+    ("rm_SX_TowerSouth.lvl", 130),
+    ("rm_SX_NPC.lvl", 131),
+    ("rm_S_Gauntlet_Elevator.lvl", 132),
+    ("rm_CH_BGunPillars.lvl", 133),
+    ("rm_CH_BFinal.lvl", 134),
+    ("rm_S_GauntletEnd.lvl", 135),
+    ("rm_CH_BDirkDemolition.lvl", 137),
+    ("rm_CH_TABigOne.lvl", 139),
+    ("rm_CH_CGateBlock.lvl", 140),
+    ("rm_CH_BMadDash.lvl", 141),
+    ("rm_CH_TLongestRoad.lvl", 142),
+    ("rm_S_BulletBaker.lvl", 143),
+    ("rm_CH_CEndHall.lvl", 144),
+    ("rm_CH_CTurnHall.lvl", 146),
+    ("rm_CH_Bfps.lvl", 147),
+    ("rm_CH_CBigggns.lvl", 148),
+    ("rm_CH_CSpawnGround.lvl", 149),
+    ("rm_S_CountAculard.lvl", 150),
+    ("rm_CH_ACorner.lvl", 152),
+    ("rm_CH_BDirkDeluge.lvl", 154),
+    ("rm_CH_BPods.lvl", 155),
+    ("rm_CH_BGunDirkDash.lvl", 156),
+    ("rm_S_MarkScythe.lvl", 157),
+    ("rm_S_GauntletLinkup.lvl", 158),
+    ("rm_CH_APillarBird.lvl", 160),
+    ("rm_CH_CSpiral.lvl", 161),
+    ("rm_CH_TBirdStandoff.lvl", 162),
+    ("rm_CH_BLeaperFall.lvl", 163),
+    ("rm_S_BennyArrow.lvl", 164),
+    ("rm_S_GauntletTitanFinale.lvl", 165),
+    ("rm_EA_EastOpening.lvl", 171),
+    ("rm_EC_SwordBridge.lvl", 172),
+    ("rm_EL_FlameElevatorEnter.lvl", 173),
+    ("rm_EA_WaterTunnelLAB.lvl", 174),
+    ("rm_EC_ThePlaza.lvl", 175),
+    ("rm_EC_NPCDrugDen.lvl", 176),
+    ("rm_EX_TowerEast.lvl", 177),
+    ("rm_EB_BogStreet.lvl", 178),
+    ("rm_EC_PlazaToLoop.lvl", 179),
+    ("rm_EL_MegaHugeLAB.lvl", 181),
+    ("rm_EB_MeltyMashArena.lvl", 182),
+    ("rm_EB_FlamePitLAB.lvl", 183),
+    ("rm_EL_FlameElevatorExit.lvl", 184),
+    ("rm_EB_DeadOtterWalk.lvl", 185),
+    ("rm_EC_PlazaAccessLAB.lvl", 187),
+    ("rm_EC_DocksLab.lvl", 188),
+    ("rm_EX_DocksCampfire.lvl", 189),
+    ("rm_EV_DocksBridge.lvl", 190),
+    ("rm_EL_FrogArena.lvl", 191),
+    ("rm_EC_BigBogLAB.lvl", 193),
+    ("rm_EA_BogTempleCamp.lvl", 194),
+    ("rm_EA_FrogBoss.lvl", 195),
+    ("rm_EC_TempleIshVault.lvl", 196),
+    ("rm_EC_EastLoop.lvl", 198),
+    ("rm_EC_LoopLAB.lvl", 199),
+    ("rm_EB_MeltyLeaperArena.lvl", 200),
+    ("rm_EC_PlazaToDocks.lvl", 202),
+    ("rm_EA_DockFightLab.lvl", 203),
+    ("rm_EB_UnderOtterBigRifleRumble.lvl", 204),
+    ("rm_EB_CleanersHole.lvl", 205),
+    ("rm_WA_Entrance.lvl", 209),
+    ("rm_WL_PrisonHALVAULT.lvl", 210),
+    ("rm_WA_Deadwood.lvl", 211),
+    ("rm_WA_DeadwoodS1.lvl", 212),
+    ("rm_WA_Grotto_buffIntro.lvl", 213),
+    ("rm_WC_WindingWood.lvl", 214),
+    ("rm_WC_GrottoNPC.lvl", 215),
+    ("rm_WL_NPCTreehouse.lvl", 216),
+    ("rm_WC_MiniLab.lvl", 217),
+    ("rm_WT_TheWood.lvl", 218),
+    ("rm_WA_EntSwitch.lvl", 219),
+    ("rm_WC_MeadowoodCorner.lvl", 220),
+    ("rm_WB_TreeTreachery.lvl", 222),
+    ("rm_WL_WestDrifterVault.lvl", 223),
+    ("rm_WT_SlowLab.lvl", 225),
+    ("rm_WC_CliffsideCellsRedux.lvl", 226),
+    ("rm_WC_PrisonHAL.lvl", 227),
+    ("rm_WC_ThinForest.lvl", 229),
+    ("rm_WC_SimplePath.lvl", 230),
+    ("rm_WC_CrystalLake.lvl", 231),
+    ("rm_WC_CrystalLakeVault.lvl", 232),
+    ("rm_WC_PrisonHallEnd.lvl", 233),
+    ("rm_WC_ThinForestLow.lvl", 234),
+    ("rm_WC_ThinForestLowSecret.lvl", 235),
+    ("rm_WA_TitanFalls.lvl", 236),
+    ("rm_WA_Vale.lvl", 238),
+    ("rm_WC_BigMeadow.lvl", 239),
+    ("rm_WC_BigMeadowVAULT.lvl", 240),
+    ("rm_WC_MeadowCaveCrossing.lvl", 241),
+    ("rm_WB_BigBattle.lvl", 242),
+    ("rm_WB_TanukiTrouble.lvl", 243),
+    ("rm_WC_RuinClearing.lvl", 244),
+    ("rm_WX_Boss.lvl", 245),
+    ("rm_WA_TowerEnter.lvl", 246),
+    ("rm_WA_MultiEntranceLab.lvl", 247),
+    ("rm_WA_CrsytalDescent.lvl", 248),
+    ("rm_WA_GrottoX.lvl", 250),
+    ("rm_WB_CrystalQueen.lvl", 251),
+    ("rm_WT_ProtoGrid.lvl", 252),
+    ("rm_WV_PuzzlePalaceNEW.lvl", 253),
+    ("rm_A_ElevatorShaftUpper.lvl", 256),
+    ("rm_A_ElevatorShaft.lvl", 257),
+    ("rm_A_PreDownward.lvl", 258),
+    ("rm_A_Downward.lvl", 259),
+    ("rm_A_DownwardDead.lvl", 260),
+    ("rm_A_DownwardDeadRevisit.lvl", 261),
+    ("rm_A_EmberRoom.lvl", 262),
+    ("rm_BossRush_Hub.lvl", 265),
+    ("rm_BossRush_FrogBoss.lvl", 266),
+    ("rm_BossRush_JerkPope.lvl", 267),
+    ("rm_BossRush_General.lvl", 268),
+    ("rm_BossRush_BulletBaker.lvl", 269),
+    ("rm_BossRush_CountAculard.lvl", 270),
+    ("rm_BossRush_MarkScythe.lvl", 271),
+    ("rm_BossRush_BennyArrow.lvl", 272),
+    ("rm_BossRush_Ember.lvl", 273),
+    ("rm_C_DrifterWorkshop.lvl", 276)
+]
+
+def get_id_from_name(name: str) -> int:
+    """
+    A way to convert internal level ID to its name.
+    """
+    for namee, idd in level_names_and_ids:
+        if namee == name: return idd
+    raise HLDError(f"No such level named {name}.")
+
+def get_name_from_id(id_: int) -> str:
+    """
+    A way to convert level name to its internal ID.
+    """
+    for namee, idd in level_names_and_ids:
+        if idd == id_: return namee
+    raise HLDError(f"No such level with id {id_}.")
```

### Comparing `hldlib-0.1.0/src/hldlib/hldsavefile.py` & `hldlib-0.1.1/src/hldlib/hldsavefile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import base64
-import json
-from dataclasses import dataclass, fields
-from pathlib import Path
-from typing import Any, Self
-
-
-def trailing_join(iter: list[str], join_string: str, trail_if_len_gt: int = 0) -> str:
-    
-    return join_string.join(iter)+ join_string * (len(iter) > trail_if_len_gt)
-    
-class sflist(list[str]):
-    """
-    A pyhton list representation of a HLD list.
-    """
-    
-    @classmethod
-    def from_string(cls, string: str):
-        return cls(string.split("+")[:-1])
-    def to_string(self) -> str:
-        return trailing_join(self, "+")
-
-class sfdict(dict[str, list[str]]):
-    """
-    A pyhton dict representation of a HLD dict.
-    """
-
-    @classmethod
-    def from_string(cls, string: str) -> Self:
-        to_return = {}
-        pairs = string.split(">")
-        for pair in pairs[:-1]:
-            s_pair = pair.split("=")
-            key = s_pair[0]
-            value = s_pair[1].split("&")
-            if len(value) > 1: value = value[:-1]
-            to_return[key] = value
-        return cls(**to_return)
-    def to_string(self) -> str:
-        return trailing_join([f"{key}={trailing_join(value, '&')}" for key, value in self.items() if value], ">")
-
-@dataclass
-class HLDSaveFile:
-    """
-    A python representation of a savefile.
-
-    For field documentation please consult tihs: https://github.com/springsylvi/HLD-Save-Editor/blob/master/save_format.txt
-    """
-    badass: float
-    mapMod: sfdict
-    dateTime: float
-    healthUp: float
-    cl: sfdict
-    destruct: sfdict
-    values: sfdict
-    gunReminderTimes: float
-    fireplaceSave: float
-    checkHP: float
-    compShell: float
-    cSwords: sflist
-    cape: float
-    halluc: float
-    newcomerHoardeMessageShown: float
-    tutHeal: float
-    noSpawn: sflist
-    checkY: float
-    specialUp: float
-    checkBat: float
-    noviceMode: float
-    successfulHealTimes: float
-    cCapes: sflist
-    CH: float
-    gear: float
-    checkCID: float
-    rooms: sflist
-    permaS: sfdict
-    checkRoom: float
-    wellMap: sflist
-    cShells: sflist
-    eq01: float
-    tablet: sflist
-    successfulWarpTimes: float
-    skill: sflist
-    bosses: sfdict
-    scK: sfdict
-    warp: sflist
-    hasMap: float
-    events: sflist
-    gearReminderTimes: float
-    enemies: sfdict
-    scUp: sflist
-    checkX: float
-    bossGearbits: sflist
-    cues: sflist
-    playT: float
-    well: sflist
-    sc: sflist
-    drifterkey: float
-    successfulCollectTimes: float
-    checkAmmo: float
-    checkStash: float
-    charDeaths: float
-    eq00: float
-    healthKits: sflist
-    sword: float
-    gameName: str
-
-    header: str
-
-    @classmethod
-    def _auto_type(cls, value: Any, strtype) -> sfdict | sflist | float | str:
-        strtype = strtype.__name__
-        type_map = {
-            "sfdict": sfdict.from_string,
-            "sflist": sflist.from_string,
-            "float": float,
-            "str": str
-        }
-        return type_map[strtype](value)
-
-    @classmethod
-    def load(cls, path: str | Path) -> Self:
-        """
-        Loads a savefile from path.
-        """
-        with open(path, "r") as in_:
-            text = in_.read()
-            return cls.from_string(text)
-
-    @classmethod
-    def from_string(cls, string: str) -> Self:
-        """
-        Creates a savefile from an encoded string.
-        """
-        save_dict: dict = json.loads(
-            base64.standard_b64decode(string[80:])[:-1]
-        )
-    
-        if not "eq00" in save_dict: save_dict["eq00"] = 0.
-        if not "eq01" in save_dict: save_dict["eq01"] = 0.
-        save_dict["header"] = string[:80]
-
-        for field in fields(cls):
-            save_dict[field.name] = cls._auto_type(save_dict[field.name], field.type)  
-        return cls(**save_dict)
-
-    def dump(self, path: str | Path) -> None:
-        """
-        Dumps the savefile to path.
-        """
-        with open(path, "w") as out:
-            out.write(self.to_string())
-    
-    def to_string(self) -> str:
-        """
-        Gets the encoded string from the savefile.
-        """
-        jsoned, header = self.to_json_string(indent=0)
-        encoded_body = header + str(base64.standard_b64encode(bytes(jsoned + "\x00", "utf8")) , "utf-8")
-        return encoded_body
-    
-    def to_json_string(self, indent: int = 0) -> tuple[str, str]:
-        """
-        An inbetween step for to_string(). Can be used for debugging.
-        """
-        save_dict = self.__dict__.copy()
-        header = save_dict.pop("header")
-        for key, value in save_dict.items():
-            if isinstance(value, (sfdict, sflist)): save_dict[key] = value.to_string()
-        if save_dict["eq00"] == 0.: save_dict.pop("eq00")
-        if save_dict["eq01"] == 0.: save_dict.pop("eq01")
-        return (json.dumps(save_dict, indent=indent), header)
-
-    def debug_dump(self, path: str | Path) -> None:
-        """
-        Dumps an unencoded savefile to path.
-        """
-        with open(path, "w") as out:
-            jsoned, _ = self.to_json_string(indent=4)
-            out.write(jsoned)
+import base64
+import json
+from dataclasses import dataclass, fields
+from pathlib import Path
+from typing import Any
+
+
+def trailing_join(iter: list[str], join_string: str, trail_if_len_gt: int = 0) -> str:
+    
+    return join_string.join(iter)+ join_string * (len(iter) > trail_if_len_gt)
+    
+class sflist(list[str]):
+    """
+    A pyhton list representation of a HLD list.
+    """
+    
+    @classmethod
+    def from_string(cls, string: str):
+        return cls(string.split("+")[:-1])
+    def to_string(self) -> str:
+        return trailing_join(self, "+")
+
+class sfdict(dict[str, list[str]]):
+    """
+    A pyhton dict representation of a HLD dict.
+    """
+
+    @classmethod
+    def from_string(cls, string: str):
+        to_return = {}
+        pairs = string.split(">")
+        for pair in pairs[:-1]:
+            s_pair = pair.split("=")
+            key = s_pair[0]
+            value = s_pair[1].split("&")
+            if len(value) > 1: value = value[:-1]
+            to_return[key] = value
+        return cls(**to_return)
+    def to_string(self) -> str:
+        return trailing_join([f"{key}={trailing_join(value, '&')}" for key, value in self.items() if value], ">")
+
+@dataclass
+class HLDSaveFile:
+    """
+    A python representation of a savefile.
+
+    For field documentation please consult tihs: https://github.com/springsylvi/HLD-Save-Editor/blob/master/save_format.txt
+    """
+    badass: float
+    mapMod: sfdict
+    dateTime: float
+    healthUp: float
+    cl: sfdict
+    destruct: sfdict
+    values: sfdict
+    gunReminderTimes: float
+    fireplaceSave: float
+    checkHP: float
+    compShell: float
+    cSwords: sflist
+    cape: float
+    halluc: float
+    newcomerHoardeMessageShown: float
+    tutHeal: float
+    noSpawn: sflist
+    checkY: float
+    specialUp: float
+    checkBat: float
+    noviceMode: float
+    successfulHealTimes: float
+    cCapes: sflist
+    CH: float
+    gear: float
+    checkCID: float
+    rooms: sflist
+    permaS: sfdict
+    checkRoom: float
+    wellMap: sflist
+    cShells: sflist
+    eq01: float
+    tablet: sflist
+    successfulWarpTimes: float
+    skill: sflist
+    bosses: sfdict
+    scK: sfdict
+    warp: sflist
+    hasMap: float
+    events: sflist
+    gearReminderTimes: float
+    enemies: sfdict
+    scUp: sflist
+    checkX: float
+    bossGearbits: sflist
+    cues: sflist
+    playT: float
+    well: sflist
+    sc: sflist
+    drifterkey: float
+    successfulCollectTimes: float
+    checkAmmo: float
+    checkStash: float
+    charDeaths: float
+    eq00: float
+    healthKits: sflist
+    sword: float
+    gameName: str
+
+    header: str
+
+    @classmethod
+    def _auto_type(cls, value: Any, strtype) -> sfdict | sflist | float | str:
+        strtype = strtype.__name__
+        type_map = {
+            "sfdict": sfdict.from_string,
+            "sflist": sflist.from_string,
+            "float": float,
+            "str": str
+        }
+        return type_map[strtype](value)
+
+    @classmethod
+    def load(cls, path: str | Path):
+        """
+        Loads a savefile from path.
+        """
+        with open(path, "r") as in_:
+            text = in_.read()
+            return cls.from_string(text)
+
+    @classmethod
+    def from_string(cls, string: str):
+        """
+        Creates a savefile from an encoded string.
+        """
+        save_dict: dict = json.loads(
+            base64.standard_b64decode(string[80:])[:-1]
+        )
+    
+        if not "eq00" in save_dict: save_dict["eq00"] = 0.
+        if not "eq01" in save_dict: save_dict["eq01"] = 0.
+        save_dict["header"] = string[:80]
+
+        for field in fields(cls):
+            save_dict[field.name] = cls._auto_type(save_dict[field.name], field.type)  
+        return cls(**save_dict)
+
+    def dump(self, path: str | Path) -> None:
+        """
+        Dumps the savefile to path.
+        """
+        with open(path, "w") as out:
+            out.write(self.to_string())
+    
+    def to_string(self) -> str:
+        """
+        Gets the encoded string from the savefile.
+        """
+        jsoned, header = self.to_json_string(indent=0)
+        encoded_body = header + str(base64.standard_b64encode(bytes(jsoned + "\x00", "utf8")) , "utf-8")
+        return encoded_body
+    
+    def to_json_string(self, indent: int = 0) -> tuple[str, str]:
+        """
+        An inbetween step for to_string(). Can be used for debugging.
+        """
+        save_dict = self.__dict__.copy()
+        header = save_dict.pop("header")
+        for key, value in save_dict.items():
+            if isinstance(value, (sfdict, sflist)): save_dict[key] = value.to_string()
+        if save_dict["eq00"] == 0.: save_dict.pop("eq00")
+        if save_dict["eq01"] == 0.: save_dict.pop("eq01")
+        return (json.dumps(save_dict, indent=indent), header)
+
+    def debug_dump(self, path: str | Path) -> None:
+        """
+        Dumps an unencoded savefile to path.
+        """
+        with open(path, "w") as out:
+            jsoned, _ = self.to_json_string(indent=4)
+            out.write(jsoned)
```

### Comparing `hldlib-0.1.0/tests/hldbasics_test.py` & `hldlib-0.1.1/tests/hldbasics_test.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from pathlib import Path
-
-import pytest
-from hldlib import Counter, find_path, HLDError, default_load, HLDLevel, HLDObj, HLDDirection
-
-def test_counter(): # Why?
-    a = Counter(1)
-    assert a.use() == 2
-    assert a.use() == 3
-    assert a.use() == 4
-
-def test_find_path(tmp_path: Path):
-    with pytest.raises(HLDError):
-        find_path("hlddir.txt", tmp_path)
-    sub = tmp_path / "sub"; sub.mkdir()
-    hlddir = sub / "hlddir.txt"
-    hlddir.write_text("C://...")
-    assert find_path("hlddir.txt", tmp_path) == "C://..."
-
-def test_default_load(tmp_path: Path):
-
-    level = HLDLevel(
-        name="rm_A_Test.lvl",
-        date=50000.00,
-        layer_names={
-            0: "Door",
-            1: "Block",
-            2: "Veg",
-            3: "Obj",
-            4: "Wall"
-        },
-        room_settings={
-            "lb": 0,
-            "bg": "<undefined>",
-            "floorSpr": "bg_C_Floor_Dregs",
-            "bri": 1,
-            "liteOff": 0,
-            "over": "bg_C_Dregs_N_Overlay",
-            "overPit": 0,
-            "wallsTop": 1,
-            "shadows": 1,
-            "flrOutline": 1,
-            "flrOC": 16777215,
-            "flrOSpr": "<undefined>",
-            "wallO": 0,
-            "w": 1024,
-            "h": 1888,
-            "sketchalpha": [
-                0.5,
-                1,
-                0
-            ]
-        },
-        objects=[
-            HLDObj.from_string("obj,Spawner,5643,522,717,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,2261,540,719,3,-999999,++,-1=CrateBig,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,4066,480,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,7726,464,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,1324,464,752,3,-999999,++,-1=MultiHitCrate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-        ],
-        direction=HLDDirection.ABYSS
-    )
-
-    north = tmp_path / "North"; north.mkdir(); level.dump(north) 
-    east = tmp_path / "East"; east.mkdir(); level.dump(east) 
-    west = tmp_path / "West"; west.mkdir(); level.dump(west) 
-    south = tmp_path / "South"; south.mkdir(); level.dump(south) 
-    central = tmp_path / "Central"; central.mkdir(); level.dump(central) 
-    intro = tmp_path / "Intro"; intro.mkdir(); level.dump(intro) 
-    abyss = tmp_path / "Abyss"; abyss.mkdir(); level.dump(abyss) 
-
-    loaded = default_load(tmp_path)
-    assert len(loaded) == 7
+from pathlib import Path
+
+import pytest
+from hldlib import Counter, find_path, HLDError, default_load, HLDLevel, HLDObj, HLDDirection
+
+def test_counter(): # Why?
+    a = Counter(1)
+    assert a.use() == 2
+    assert a.use() == 3
+    assert a.use() == 4
+
+def test_find_path(tmp_path: Path):
+    with pytest.raises(HLDError):
+        find_path("hlddir.txt", tmp_path)
+    sub = tmp_path / "sub"; sub.mkdir()
+    hlddir = sub / "hlddir.txt"
+    hlddir.write_text("C://...")
+    assert find_path("hlddir.txt", tmp_path) == "C://..."
+
+def test_default_load(tmp_path: Path):
+
+    level = HLDLevel(
+        name="rm_A_Test.lvl",
+        date=50000.00,
+        layer_names={
+            0: "Door",
+            1: "Block",
+            2: "Veg",
+            3: "Obj",
+            4: "Wall"
+        },
+        room_settings={
+            "lb": 0,
+            "bg": "<undefined>",
+            "floorSpr": "bg_C_Floor_Dregs",
+            "bri": 1,
+            "liteOff": 0,
+            "over": "bg_C_Dregs_N_Overlay",
+            "overPit": 0,
+            "wallsTop": 1,
+            "shadows": 1,
+            "flrOutline": 1,
+            "flrOC": 16777215,
+            "flrOSpr": "<undefined>",
+            "wallO": 0,
+            "w": 1024,
+            "h": 1888,
+            "sketchalpha": [
+                0.5,
+                1,
+                0
+            ]
+        },
+        objects=[
+            HLDObj.from_string("obj,Spawner,5643,522,717,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,2261,540,719,3,-999999,++,-1=CrateBig,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,4066,480,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,7726,464,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,1324,464,752,3,-999999,++,-1=MultiHitCrate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+        ],
+        direction=HLDDirection.ABYSS
+    )
+
+    north = tmp_path / "North"; north.mkdir(); level.dump(north) 
+    east = tmp_path / "East"; east.mkdir(); level.dump(east) 
+    west = tmp_path / "West"; west.mkdir(); level.dump(west) 
+    south = tmp_path / "South"; south.mkdir(); level.dump(south) 
+    central = tmp_path / "Central"; central.mkdir(); level.dump(central) 
+    intro = tmp_path / "Intro"; intro.mkdir(); level.dump(intro) 
+    abyss = tmp_path / "Abyss"; abyss.mkdir(); level.dump(abyss) 
+
+    loaded = default_load(tmp_path)
+    assert len(loaded) == 7
     assert loaded[0].direction != loaded[1].direction
```

### Comparing `hldlib-0.1.0/tests/hldlevel_test.py` & `hldlib-0.1.1/tests/hldlevel_test.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from pathlib import Path
-from hldlib import HLDDirection, HLDLevel, HLDObj, get_id_from_name, get_name_from_id, HLDError
-from os.path import join as p_join
-import copy
-import pytest
-
-@pytest.fixture
-def testing_level() -> HLDLevel:
-    return HLDLevel(
-        name="rm_A_Test.lvl",
-        date=50000.00,
-        layer_names={
-            0: "Door",
-            1: "Block",
-            2: "Veg",
-            3: "Obj",
-            4: "Wall"
-        },
-        room_settings={
-            "lb": 0,
-            "bg": "<undefined>",
-            "floorSpr": "bg_C_Floor_Dregs",
-            "bri": 1,
-            "liteOff": 0,
-            "over": "bg_C_Dregs_N_Overlay",
-            "overPit": 0,
-            "wallsTop": 1,
-            "shadows": 1,
-            "flrOutline": 1,
-            "flrOC": 16777215,
-            "flrOSpr": "<undefined>",
-            "wallO": 0,
-            "w": 1024,
-            "h": 1888,
-            "sketchalpha": [
-                0.5,
-                1,
-                0
-            ]
-        },
-        objects=[
-            HLDObj.from_string("obj,Spawner,5643,522,717,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,2261,540,719,3,-999999,++,-1=CrateBig,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,4066,480,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,7726,464,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-            HLDObj.from_string("obj,Spawner,1324,464,752,3,-999999,++,-1=MultiHitCrate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
-        ],
-        direction=HLDDirection.ABYSS
-    )
-
-
-def test_dump_and_load(tmp_path: Path, testing_level: HLDLevel):
-    testing_level.dump(tmp_path)
-    dumped_level = HLDLevel.load(p_join(tmp_path, testing_level.name), HLDDirection.ABYSS)
-    assert testing_level == dumped_level
-
-def test_load_errors(tmp_path: Path, testing_level: HLDLevel):
-
-    level1 = copy.deepcopy(testing_level)
-    level1.layer_names = {}
-    level1.name = "rm_A_Test1.lvl"
-    level1.dump(tmp_path)
-
-    level2 = copy.deepcopy(testing_level)
-    level2.date = '' # type: ignore
-    level2.name = "rm_A_Test2.lvl"
-    level2.dump(tmp_path)
-
-    level3 = copy.deepcopy(testing_level)
-    level3.room_settings = {}
-    level3.name = "rm_A_Test3.lvl"
-
-    with pytest.raises(IndexError):
-        HLDLevel.load(p_join(tmp_path, level1.name), HLDDirection.ABYSS)
-
-    with pytest.raises(ValueError):
-        HLDLevel.load(p_join(tmp_path, level2.name), HLDDirection.ABYSS)
-        
-    with pytest.raises(KeyError):
-        level3.dump(tmp_path)
-
-def test_get_ids_and_names():
-    assert get_id_from_name("rm_IN_01_brokenshallows.lvl") == 46
-    assert get_name_from_id(46) == "rm_IN_01_brokenshallows.lvl"
-
-def test_ids_and_names_errors():
-    with pytest.raises(HLDError):
-        get_id_from_name("rm_A_DoesntExist.lvl")
-    with pytest.raises(HLDError):
+from pathlib import Path
+from hldlib import HLDDirection, HLDLevel, HLDObj, get_id_from_name, get_name_from_id, HLDError
+from os.path import join as p_join
+import copy
+import pytest
+
+@pytest.fixture
+def testing_level() -> HLDLevel:
+    return HLDLevel(
+        name="rm_A_Test.lvl",
+        date=50000.00,
+        layer_names={
+            0: "Door",
+            1: "Block",
+            2: "Veg",
+            3: "Obj",
+            4: "Wall"
+        },
+        room_settings={
+            "lb": 0,
+            "bg": "<undefined>",
+            "floorSpr": "bg_C_Floor_Dregs",
+            "bri": 1,
+            "liteOff": 0,
+            "over": "bg_C_Dregs_N_Overlay",
+            "overPit": 0,
+            "wallsTop": 1,
+            "shadows": 1,
+            "flrOutline": 1,
+            "flrOC": 16777215,
+            "flrOSpr": "<undefined>",
+            "wallO": 0,
+            "w": 1024,
+            "h": 1888,
+            "sketchalpha": [
+                0.5,
+                1,
+                0
+            ]
+        },
+        objects=[
+            HLDObj.from_string("obj,Spawner,5643,522,717,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,2261,540,719,3,-999999,++,-1=CrateBig,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,4066,480,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,7726,464,728,3,-999999,++,-1=Crate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+            HLDObj.from_string("obj,Spawner,1324,464,752,3,-999999,++,-1=MultiHitCrate,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"),
+        ],
+        direction=HLDDirection.ABYSS
+    )
+
+
+def test_dump_and_load(tmp_path: Path, testing_level: HLDLevel):
+    testing_level.dump(tmp_path)
+    dumped_level = HLDLevel.load(p_join(tmp_path, testing_level.name), HLDDirection.ABYSS)
+    assert testing_level == dumped_level
+
+def test_load_errors(tmp_path: Path, testing_level: HLDLevel):
+
+    level1 = copy.deepcopy(testing_level)
+    level1.layer_names = {}
+    level1.name = "rm_A_Test1.lvl"
+    level1.dump(tmp_path)
+
+    level2 = copy.deepcopy(testing_level)
+    level2.date = '' # type: ignore
+    level2.name = "rm_A_Test2.lvl"
+    level2.dump(tmp_path)
+
+    level3 = copy.deepcopy(testing_level)
+    level3.room_settings = {}
+    level3.name = "rm_A_Test3.lvl"
+
+    with pytest.raises(IndexError):
+        HLDLevel.load(p_join(tmp_path, level1.name), HLDDirection.ABYSS)
+
+    with pytest.raises(ValueError):
+        HLDLevel.load(p_join(tmp_path, level2.name), HLDDirection.ABYSS)
+        
+    with pytest.raises(KeyError):
+        level3.dump(tmp_path)
+
+def test_get_ids_and_names():
+    assert get_id_from_name("rm_IN_01_brokenshallows.lvl") == 46
+    assert get_name_from_id(46) == "rm_IN_01_brokenshallows.lvl"
+
+def test_ids_and_names_errors():
+    with pytest.raises(HLDError):
+        get_id_from_name("rm_A_DoesntExist.lvl")
+    with pytest.raises(HLDError):
         get_name_from_id(0)
```

### Comparing `hldlib-0.1.0/tests/hldobj_test.py` & `hldlib-0.1.1/tests/hldobj_test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from hldlib import HLDObj, HLDType, HLDError
-import pytest
-
-
-@pytest.fixture
-def obj_string() -> str:
-    return "obj,Spawner,593,536,352,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"
-
-def test_from_string(obj_string: str):
-    obj = HLDObj.from_string(obj_string)
-    assert obj.type == HLDType.SPAWNER
-    assert obj.uid == 593
-    assert obj.x == 536
-    assert obj.y == 352
-    assert obj.layer == 6
-    assert obj.dependencies == "-999999"
-    assert obj.attrs == \
-    {
-        "-1": "dirk",
-        "-2": -999999,
-        "-4": 1,
-        "-5": 0,
-        "-6": -1,
-        "-7": 0,
-        "-8": 0,
-    }
-
-def test_from_string_errors():
-    with pytest.raises(HLDError):
-        HLDObj.from_string("")
-    with pytest.raises(HLDError):
-        HLDObj.from_string(",obj,Spawner,593,536,352,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,")
-    with pytest.raises(HLDError):
-        HLDObj.from_string("obj,Spawner,593,536,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,")
-
-def test_to_string(obj_string: str):
-    obj = HLDObj.from_string(obj_string)
-    assert obj_string == obj.to_string().strip().replace("//", "") 
+from hldlib import HLDObj, HLDType, HLDError
+import pytest
+
+
+@pytest.fixture
+def obj_string() -> str:
+    return "obj,Spawner,593,536,352,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,"
+
+def test_from_string(obj_string: str):
+    obj = HLDObj.from_string(obj_string)
+    assert obj.type == HLDType.SPAWNER
+    assert obj.uid == 593
+    assert obj.x == 536
+    assert obj.y == 352
+    assert obj.layer == 6
+    assert obj.dependencies == "-999999"
+    assert obj.attrs == \
+    {
+        "-1": "dirk",
+        "-2": -999999,
+        "-4": 1,
+        "-5": 0,
+        "-6": -1,
+        "-7": 0,
+        "-8": 0,
+    }
+
+def test_from_string_errors():
+    with pytest.raises(HLDError):
+        HLDObj.from_string("")
+    with pytest.raises(HLDError):
+        HLDObj.from_string(",obj,Spawner,593,536,352,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,")
+    with pytest.raises(HLDError):
+        HLDObj.from_string("obj,Spawner,593,536,6,-999999,++,-1=dirk,-2=-999999,-4=1,-5=0,-6=-1,-7=0,-8=0,")
+
+def test_to_string(obj_string: str):
+    obj = HLDObj.from_string(obj_string)
+    assert obj_string == obj.to_string().strip().replace("//", "")
```

### Comparing `hldlib-0.1.0/tests/hldsavefile_test.py` & `hldlib-0.1.1/tests/hldsavefile_test.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from pathlib import Path
-from hldlib import HLDSaveFile, hldsavefile
-from os.path import join as p_join
-import pytest
-
-
-@pytest.fixture
-def testing_savefile() -> HLDSaveFile:
-    return HLDSaveFile.from_string("67eb87838659be77713bcdb237b0420a59d817df6eb7cd347d4b75823c138d6876d36e4eab448002eyJiYWRhc3MiOiAwLjAsICJtYXBNb2QiOiAiMTMyPTImPjE0ND0yJj4xNjE9MiY+MTgxPTImPjEwNj0yJj4xMDk9MiY+MTk0PTImPjIyNj0yJj4xODM9MiY+MTc0PTImPjE2MD0yJj4yMTg9MiY+OTU9MiY+MTA0PTImPjIyMD0yJj4yMTA9MiY+IiwgImRhdGVUaW1lIjogNDQ5ODAuNTI0MTI2LCAiaGVhbHRoVXAiOiAwLjAsICJjbCI6ICI5PTEwMTM4NyYxODUyNjcmMjA2MTM5JjI2Njc4NCY+MTM9LTE1MTg4NTEmPjc9LTI1NTEwMCYtMTg3OTA1Ji0xNjczMjYmLTUzMzkyJj42PS0xODk1NDgxJi0xMDQ3NDMwJi05MzI0NzEmLTkwMjIxMiY+OD0tNTU1Mjc5Ji0zOTg2MzUmLTM4NjQ1NyYtNjc2MzU3Jj4iLCAiZGVzdHJ1Y3QiOiAiLTM2MjI0Nj0xNjMmMzcuMjEmPjE4MjYxMj0yMTgmMzAuODQmPi0xOTc3OTEzPTIyMCYyNC42NCY+MTk1Mjk3PTIxOSYzMC40MyY+LTM2ODk5OT0xNjMmMzcuMjEmPjIwNDUwNT0yMjAmMjQuNjQmPjIwNDA1OD0yMjAmMjQuNjQmPjIwNTkwNz0yMjAmMjQuNjQmPjIwMzA3MT0yMjAmMjQuNjQmPi0xODIxODkwPTE3OCYxNS44MiY+LTY0OTEwPTE5MyYxNi4xMCY+LTE5NzkwMDE9MjA5JjMxLjg0Jj4tMTgyODY4ND0xNzEmMTkuMjkmPjE4MTM3Nj0yMTgmMzAuODQmPi0yMTU1NDE9MTc4JjE1LjgyJj4tMjE1MTIyPTE3OCYxNS44MiY+LTIxNDY5MT0xNzgmMTUuODImPi0yMTYyODI9MTc4JjE1LjgyJj4tMTgzNjE3Nj0xNjMmMzcuMjEmPi0xODI4MDIwPTE3MSYxOS4yOSY+MjAxMDk2PTIyMCYyNC42NCY+LTE3Nzk0MDg9MjIwJjI0LjY0Jj4tNDg2MTA9MTk1JjE3LjI5Jj4tMTc4MDI0MT0yMTkmMzAuNDMmPjIwNzQzNT0yMjAmMjQuNjQmPi0xOTE1ODQ1PTg0JjIuNzcmPi0zNTcwNzA9MTY0JjM4LjU1Jj4tMjEzNjY1PTE3OCYxNS44MiY+LTI1MzY3Mj0xNzQmMTguNTYmPjE4MjEwND0yMTgmMzAuODQmPjkxNTc2PTIwOSYzMS44NCY+LTIxMjE0MT0xNzgmMTUuODImPi0zNTQzNDg9MTY0JjM4LjU1Jj4xNDczNDg9MjE0JjMxLjI4Jj4tMjE3MTMzPTE3OCYxNS44MiY+OTQ1MDY9MjA5JjMxLjg0Jj4tMjEyMDI0PTE3OCYxNS44MiY+LTI1MjIwNj0xNzQmMTguNTYmPi0zNzMzOTU9MTYyJjM2Ljk4Jj4xODU1MjU9MjE4JjMwLjg0Jj4tMTk1MzYwNT00NiY4LjM1Jj4tMjcxOTUxPTE3MiYxOS4wNCY+LTI1NTc5Nz0xNzQmMTguNTYmPi0yMTI4MDM9MTc4JjE1LjgyJj4xODMyNDA9MjE4JjMwLjg0Jj4tMTgyMTYwNz0xNzgmMTUuODImPjE4NTM5Mz0yMTgmMzAuODQmPi0zNTY3MTY9MTY0JjM4LjU1Jj4tMjg3MjMyPTE3MSYxOS4yOSY+MTQ2OTcwPTIxNCYzMS4yOCY+LTE3Nzk4Mjc9MjIwJjI0LjY0Jj4yMDQ2MzY9MjIwJjI0LjY0Jj4xOTQ4NDA9MjE5JjMwLjQzJj4tMzUzMDY2PTE2NCYzOC41NSY+MTgyNDE4PTIxOCYzMC44NCY+MjA1ODYyPTIyMCYyNC42NCY+LTQyMzg3PTE5NSYxNy4yOSY+LTE3NzQyNjM9MjI1JjMwLjE1Jj4tMjE3MDUzPTE3OCYxNS44MiY+MjA0NTM1PTIyMCYyNC42NCY+LTM1MzI4Mj0xNjQmMzguNTUmPi0xNzgxNjk5PTIxOCYzMC44NCY+MTg3NTM3PTIxOCYzMC44NCY+LTE4MDUxMzg9MTk0JjE3LjQ3Jj4yMDc3NDM9MjIwJjI0LjY0Jj4tNjI0MTY9MTkzJjE2LjEwJj4tMjEzNDAyPTE3OCYxNS44MiY+LTM2MzM2Nz0xNjMmMzcuMjEmPi0yMTgwODQ9MTc4JjE1LjgyJj4tMzc1NTE0PTE2MiYzNi45OCY+LTY3NDcxPTE5MyYxNi4xMCY+LTE1MzI5NzY9NDYmOC4zNSY+MjAzOTA4PTIyMCYyNC42NCY+LTIxNTc5Mz0xNzgmMTUuODImPi0yMTIwNTM9MTc4JjE1LjgyJj4yMDM3NjM9MjIwJjI0LjY0Jj4tMzYyMzQ4PTE2MyYzNy4yMSY+MjAxNDI4PTIyMCYyNC42NCY+MTg0MTU1PTIxOCYzMC44NCY+MTgzOTM5PTIxOCYzMC44NCY+MTQ1MjUzPTIxNCYzMS4yOCY+MTQ1NzkyPTIxNCYzMS4yOCY+LTQ4NTUyPTE5NSYxNy4yOSY+LTI3NDcyMz0xNzImMTkuMDQmPiIsICJ2YWx1ZXMiOiAiVmFsdWViYWRhc3NPZmZpY2VTdGF0ZT0yPiIsICJndW5SZW1pbmRlclRpbWVzIjogMC4wLCAiZmlyZXBsYWNlU2F2ZSI6IDAuMCwgImNoZWNrSFAiOiA1LjAsICJjb21wU2hlbGwiOiAwLjAsICJjU3dvcmRzIjogIjArIiwgImNhcGUiOiAwLjAsICJoYWxsdWMiOiAwLjAsICJuZXdjb21lckhvYXJkZU1lc3NhZ2VTaG93biI6IDAuMCwgInR1dEhlYWwiOiAwLjAsICJub1NwYXduIjogIi0xMDk3OTU0Ky0xNDU1MDQrLTE4NzExNjUrIiwgImNoZWNrWSI6IDYwOC4wLCAic3BlY2lhbFVwIjogMC4wLCAiY2hlY2tCYXQiOiAxMDAuMCwgIm5vdmljZU1vZGUiOiAwLjAsICJzdWNjZXNzZnVsSGVhbFRpbWVzIjogNS4wLCAiY0NhcGVzIjogIjArIiwgIkNIIjogMC4wLCAiZ2VhciI6IDAuMCwgImNoZWNrQ0lEIjogNjI0NTMxLjAsICJyb29tcyI6ICI0Nis3OSs0Nys0OCs0OSs1MCs1Mys2MSs2Mis4NCs4NSs4OCs5MCs5Mis5Mys5NCsxMDQrOTUrMTA2KzEwNysxMDgrMTA5Kzk2Kzk3KzY0KzE3MSsxNzIrMTczKzE3NCsxNzUrMTc3KzE4MSsxODIrMTgzKzE4NCsxODUrMTc4KzE5MysxOTQrMTk1KzE5Nis2NSsyMDkrMjEwKzIxMSsyMTQrMjE4KzIxOSsyMjArMjI1KzIyNisyMzgrMjQ4KzI0NysyNDYrNjMrMTI4KzEzMCsxNDQrMTUyKzE2MCsxNjErMTYyKzE2MysxNjQrMTY1KzEzMisyNTYrMjU3KzI1OCsyNTkrMjYyKyIsICJwZXJtYVMiOiAiLTEwNDc5NDA9Mj4tNjkyMjMyPTI+LTEzODcwNTY9Mj4tNjk3MzYxPTI+LTE4MzM1Mz0yPjM4Mzk4OT0yPiIsICJjaGVja1Jvb20iOiAyNjIuMCwgIndlbGxNYXAiOiAiMSswKzIrMysiLCAiY1NoZWxscyI6ICIwKyIsICJ0YWJsZXQiOiAiIiwgInN1Y2Nlc3NmdWxXYXJwVGltZXMiOiAwLjAsICJza2lsbCI6ICIiLCAiYm9zc2VzIjogIjMuMjA9MzExJjIyNiY+IiwgInNjSyI6ICIxPTExPiIsICJ3YXJwIjogIjArMiszKyIsICJoYXNNYXAiOiAwLjAsICJldmVudHMiOiAiLTE1MzQyMTQrLTE1MTc2NjkrLTE0OTc2NjQrLTI1MjY5NCstMjI2OTc1Ky0xODA2NTkrLTE3NDg1NCstMTgyNDUzMystNDU2NzcrMjUzNDI2KzM4NTUwMSstMzk2MjcyKy0zNDQ5MjIrNTg2NjY2KzYyNjc3NisiLCAiZ2VhclJlbWluZGVyVGltZXMiOiAwLjAsICJlbmVtaWVzIjogIi0xODY4Mzk9MTgxJjEyLjE0Jj4tMTg2MjcxPTE4MSYxMi4xNCY+MjU1NTk4PTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjUxNiY2OTgmLTEmPjI1MTYxOD0yMjUmMzAuMTUmc3ByX1JpZmxlRGlya0RlYWQmMSY0OTUmNzIwJi0xJj4tMjEyODI1PTE3OCYxNS44MiZzcHJfTmluamFGcm9nRGVhZCYxJjczMyYxNjImLTEmPi0xNjM0MDk9MTgzJjE0LjQ1Jj4yMDI5NTk9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjY3MSYzNzMmMSY+LTkxNDgwMT0xMDgmNy42MyZzcHJfQ3VsdEJpcmREZWFkJjEmNTgyJjIzOSYtMSY+LTE5NTEyNzA9NDgmOS4xMCZzcHJfUmlmbGVEaXJrRGVhZCYxJjExODcmMTA5MCYxJj4yNTU4MzI9MjI1JjMwLjE1JnNwcl9TbWFsbENyeXN0YWxTcGlkZXJEZWFkJjEmNTk3JjY4NiYxJj4tMTkzNzQwNj02MiYyLjM3JnNwcl9EaXJrRGVhZCYxJjUyMiYzNzgmLTEmPi0xNjY3MTg9MTgzJjE0LjQ1JnNwcl9SaWZsZURpcmtEZWFkJjEmNjcyJjkxNyYtMSY+NDcxMDUyPTI0NyYyOS41OCY+LTE4NTc1Mj0xODEmMTIuMTQmPi02Mzc3OT0xOTMmMTYuMTAmc3ByX1JpZmxlRGlya0RlYWQmMSYxMDk3JjE0NzMmLTEmPi0xMzQ2Mjk3PTY1JjMyLjA4JnNwcl9TcGlkZXJEZWFkJjEmOTYmNDM0JjEmPjIwMjQ4Mz0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmMzAzJjI0NCYxJj4yMDQyNjc9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjUxMCYzNTImLTEmPi0xNTIzMzAwPTQ3JjguNzEmc3ByX0RpcmtEZWFkJjEmNzgxJjU0MCYtMSY+NDc3NzQ4PTI0NyYyOS41OCY+MjU1NzcyPTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjU5NiY2OTAmLTEmPi0xNjg2ODY9MTgzJjE0LjQ1Jj4tMzk3NDQ3PTE2MCYzNi4xNiZzcHJfTWlzc2lsZURpcmtEZWFkJjEmMjcyJjg5MyYtMSY+LTkzODU3Mz0xMDYmNy4wNiZzcHJfUmlmbGVEaXJrRGVhZCYxJjM2OSY0MTcmMSY+MjU2ODk3PTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjgxNCY2ODMmMSY+LTE1MTgzODE9NDgmOS4xMCZzcHJfRGlya0RlYWQmMSYxMjAyJjExMTMmLTEmPjIwNTYxOT0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNjE5JjMzMyYxJj4yMDEyODM9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjY1NCYzNzYmMSY+LTM4NzczOD0xNjEmMzYuNTQmc3ByX1JpZmxlRGlya0RlYWQmMSY0MDgmMTQ2Ji0xJj4tMTgxNjUyMj0xODMmMTQuNDUmPjE4NTYzNT0yMTgmMzAuODQmc3ByX1RhbnVraURlYWQmMSYxMTk2JjEwNjImLTEmPjIwNDA4MD0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNTYyJjM0MiYxJj4tMTgxNjcxMz0xODMmMTQuNDUmPi0xMzc1ODg2PTYyJjIuMzcmc3ByX0RpcmtEZWFkJjEmNTA0JjQwNSYtMSY+LTE2NDc1Mj0xODMmMTQuNDUmc3ByX1JpZmxlRGlya0RlYWQmMSY0NTYmNzc5JjEmPi0xODE2MTM3PTE4MyYxNC40NSZzcHJfUmlmbGVEaXJrRGVhZCYxJjY0MSYxMDg4Ji0xJj4tNjI1NjY9MTkzJjE2LjEwJnNwcl9EaXJrRGVhZCYxJjEyODcmMTQ1NCYtMSY+MjAyMzE1PTIyMCYyNC42NCZzcHJfV29sZkRlYWQmMSY1MDcmMzcxJi0xJj4xNDI1Mjk9MjE0JjMxLjI4JnNwcl9EaXJrRGVhZCYxJjEyMjgmOTkzJi0xJj4tMTgyMTUxMT0xNzgmMTUuODImc3ByX05pbmphRnJvZ0RlYWQmMSY2OTEmMTk5JjEmPi0xNzc0NjAxPTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjc2MSY2NjAmMSY+LTE2ODUzND0xODMmMTQuNDUmPi0xMzU2MjU5PTY0JjE5LjYzJnNwcl9TcGlkZXJEZWFkJjEmNDIxJjIyNSYxJj4tMjE3NTYwPTE3OCYxNS44MiZzcHJfSmFyRnJvZ0RlYWQmMSY4ODcmMzE5JjEmPi0xNjc3MTc9MTgzJjE0LjQ1JnNwcl9SaWZsZURpcmtEZWNhcEJvdHRvbSYxJjQ1NiY3NjEmLTEmPi05MzQ5MDQ9MTA2JjcuMDYmc3ByX1JpZmxlRGlya0RlYWQmMSYzNTYmNDQ5JjEmPjI1NTQ2MD0yMjUmMzAuMTUmc3ByX1JpZmxlRGlya0RlYWQmMSY2MjMmNjc2JjEmPi02MzY3OT0xOTMmMTYuMTAmc3ByX0RpcmtEZWFkJjEmMTM0NiYxNDQ2Ji0xJj4tMTgzNjc0MT0xNjMmMzcuMjEmPjIwMzg2Mj0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNjUyJjM1OCYtMSY+MjAzMDY2PTIyMCYyNC42NCZzcHJfV29sZkRlYWQmMSY1MDcmMzQwJjEmPi0yMTIzNTM9MTc4JjE1LjgyJnNwcl9KYXJGcm9nRGVhZCYxJjkyMSYyMDEmLTEmPi0xMzUzMzk4PTY0JjE5LjYzJnNwcl9TcGlkZXJEZWFkJjEmNDAzJjIxNCYxJj4yNTEyNTk9MjI1JjMwLjE1JnNwcl9TbWFsbENyeXN0YWxTcGlkZXJEZWFkJjEmODMyJjY5NCYxJj4tMTY1MzAxPTE4MyYxNC40NSZzcHJfRGlya0RlYWQmMSY2NDgmODk3Ji0xJj4tMTY1MzQ2PTE4MyYxNC40NSZzcHJfUmlmbGVEaXJrRGVhZCYxJjY3MyYxMDg4JjEmPi0xNTE0NTMyPTQ4JjkuMTAmc3ByX0RpcmtEZWFkJjEmMTI0NSYxMDk0Ji0xJj4tMTY0MzQ3PTE4MyYxNC40NSY+IiwgInNjVXAiOiAiIiwgImNoZWNrWCI6IDM0Ny4wLCAiYm9zc0dlYXJiaXRzIjogIiIsICJjdWVzIjogIi0xMDkyMDE5Ky0xMDkyNTE3Ky0xMDczMzY2Ky0xMDU1NTc2Ky0yNzYxMjYrLTE4MTQxMjcrLTE0NzU0NystMjE0MDI3Ky03MTYwOTIrIiwgInBsYXlUIjogNDEuMCwgIndlbGwiOiAiMSswKzIrMysiLCAic2MiOiAiMSsiLCAiZHJpZnRlcmtleSI6IDAuMCwgInN1Y2Nlc3NmdWxDb2xsZWN0VGltZXMiOiAwLjAsICJjaGVja0FtbW8iOiAwLjAsICJjaGVja1N0YXNoIjogMS4wLCAiY2hhckRlYXRocyI6IDEyLjAsICJlcTAwIjogMS4wLCAiaGVhbHRoS2l0cyI6ICItMTUzMzYzOSstMTUyNzIxMistMTUyNzA0MSstOTM0OTUxKy0xMzUzNDYzKy0xNjY3OTgrLTE3ODY2NCstNjM3OTErLTUzODM2KzE0NjIyNSstMTc3NDIyMistMzg3OTAzKy0zNjc2MjErLTM0MjM0NistNjczMjA3KyIsICJzd29yZCI6IDAuMCwgImdhbWVOYW1lIjogIlEifSA=")
-
-def test_load(testing_savefile: HLDSaveFile):
-    assert testing_savefile.badass == 0.
-    assert testing_savefile.mapMod == {"132": ["2"], "144": ["2"], "161": ["2"], "181": ["2"], "106": ["2"], "109": ["2"], "194": ["2"], "226": ["2"], "183": ["2"], "174": ["2"], "160": ["2"], "218": ["2"], "95": ["2"], "104": ["2"], "220": ["2"], "210": ["2"]}
-    assert testing_savefile.dateTime == 44980.524126
-    assert testing_savefile.healthUp == 0.
-    assert testing_savefile.cl == {"9": ["101387", "185267", "206139", "266784"], "13": ["-1518851"], "7": ["-255100", "-187905", "-167326", "-53392"], "6": ["-1895481", "-1047430", "-932471", "-902212"], "8": ["-555279", "-398635", "-386457", "-676357"]}
-    assert testing_savefile.destruct == {"-362246": ["163", "37.21"], "182612": ["218", "30.84"], "-1977913": ["220", "24.64"], "195297": ["219", "30.43"], "-368999": ["163", "37.21"], "204505": ["220", "24.64"], "204058": ["220", "24.64"], "205907": ["220", "24.64"], "203071": ["220", "24.64"], "-1821890": ["178", "15.82"], "-64910": ["193", "16.10"], "-1979001": ["209", "31.84"], "-1828684": ["171", "19.29"], "181376": ["218", "30.84"], "-215541": ["178", "15.82"], "-215122": ["178", "15.82"], "-214691": ["178", "15.82"], "-216282": ["178", "15.82"], "-1836176": ["163", "37.21"], "-1828020": ["171", "19.29"], "201096": ["220", "24.64"], "-1779408": ["220", "24.64"], "-48610": ["195", "17.29"], "-1780241": ["219", "30.43"], "207435": ["220", "24.64"], "-1915845": ["84", "2.77"], "-357070": ["164", "38.55"], "-213665": ["178", "15.82"], "-253672": ["174", "18.56"], "182104": ["218", "30.84"], "91576": ["209", "31.84"], "-212141": ["178", "15.82"], "-354348": ["164", "38.55"], "147348": ["214", "31.28"], "-217133": ["178", "15.82"], "94506": ["209", "31.84"], "-212024": ["178", "15.82"], "-252206": ["174", "18.56"], "-373395": ["162", "36.98"], "185525": ["218", "30.84"], "-1953605": ["46", "8.35"], "-271951": ["172", "19.04"], "-255797": ["174", "18.56"], "-212803": ["178", "15.82"], "183240": ["218", "30.84"], "-1821607": ["178", "15.82"], "185393": ["218", "30.84"], "-356716": ["164", "38.55"], "-287232": ["171", "19.29"], "146970": ["214", "31.28"], "-1779827": ["220", "24.64"], "204636": ["220", "24.64"], "194840": ["219", "30.43"], "-353066": ["164", "38.55"], "182418": ["218", "30.84"], "205862": ["220", "24.64"], "-42387": ["195", "17.29"], "-1774263": ["225", "30.15"], "-217053": ["178", "15.82"], "204535": ["220", "24.64"], "-353282": ["164", "38.55"], "-1781699": ["218", "30.84"], "187537": ["218", "30.84"], "-1805138": ["194", "17.47"], "207743": ["220", "24.64"], "-62416": ["193", "16.10"], "-213402": ["178", "15.82"], "-363367": ["163", "37.21"], "-218084": ["178", "15.82"], "-375514": ["162", "36.98"], "-67471": ["193", "16.10"], "-1532976": ["46", "8.35"], "203908": ["220", "24.64"], "-215793": ["178", "15.82"], "-212053": ["178", "15.82"], "203763": ["220", "24.64"], "-362348": ["163", "37.21"], "201428": ["220", "24.64"], "184155": ["218", "30.84"], "183939": ["218", "30.84"], "145253": ["214", "31.28"], "145792": ["214", "31.28"], "-48552": ["195", "17.29"], "-274723": ["172", "19.04"]}
-    assert testing_savefile.values == {'ValuebadassOfficeState': ['2']}
-    assert testing_savefile.gunReminderTimes == 0.
-    assert testing_savefile.fireplaceSave == 0.
-    assert testing_savefile.checkHP == 5.
-    assert testing_savefile.compShell == 0.
-    assert testing_savefile.cSwords == ["0"]
-    assert testing_savefile.cape == 0.
-    assert testing_savefile.halluc == 0.
-    assert testing_savefile.newcomerHoardeMessageShown == 0.
-    assert testing_savefile.tutHeal == 0.
-    assert testing_savefile.noSpawn == ['-1097954', '-145504', '-1871165']
-    assert testing_savefile.checkY == 608.
-    assert testing_savefile.specialUp == 0.
-    assert testing_savefile.checkBat == 100.
-    assert testing_savefile.noviceMode == 0.
-    assert testing_savefile.successfulHealTimes == 5.
-    assert testing_savefile.cCapes == ["0"]
-    assert testing_savefile.CH == 0.
-    assert testing_savefile.gear == 0.
-    assert testing_savefile.checkCID == 624531.
-    assert testing_savefile.rooms == ["46", "79", "47", "48", "49", "50", "53", "61", "62", "84", "85", "88", "90", "92", "93", "94", "104", "95", "106", "107", "108", "109", "96", "97", "64", "171", "172", "173", "174", "175", "177", "181", "182", "183", "184", "185", "178", "193", "194", "195", "196", "65", "209", "210", "211", "214", "218", "219", "220", "225", "226", "238", "248", "247", "246", "63", "128", "130", "144", "152", "160", "161", "162", "163", "164", "165", "132", "256", "257", "258", "259", "262"]
-    assert testing_savefile.permaS == {"-1047940": ["2"], "-692232": ["2"], "-1387056": ["2"], "-697361": ["2"], "-183353": ["2"], "383989": ["2"]}
-    assert testing_savefile.checkRoom == 262.
-    assert testing_savefile.wellMap == ["1", "0", "2", "3"]
-    assert testing_savefile.cShells == ["0"]
-    assert testing_savefile.eq01 == 0.
-    assert testing_savefile.tablet == []
-    assert testing_savefile.successfulWarpTimes == 0.
-    assert testing_savefile.skill == []
-    assert testing_savefile.bosses == {'3.20': ['311', '226']}
-    assert testing_savefile.scK == {'1': ['11']}
-    assert testing_savefile.warp == ['0', '2', '3']
-    assert testing_savefile.hasMap == 0.
-    assert testing_savefile.events == ["-1534214", "-1517669", "-1497664", "-252694", "-226975", "-180659", "-174854", "-1824533", "-45677", "253426", "385501", "-396272", "-344922", "586666", "626776"]
-    assert testing_savefile.gearReminderTimes == 0.
-    assert testing_savefile.enemies == {"-186839": ["181", "12.14"], "-186271": ["181", "12.14"], "255598": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "516", "698", "-1"], "251618": ["225", "30.15", "spr_RifleDirkDead", "1", "495", "720", "-1"], "-212825": ["178", "15.82", "spr_NinjaFrogDead", "1", "733", "162", "-1"], "-163409": ["183", "14.45"], "202959": ["220", "24.64", "spr_WolfDead", "1", "671", "373", "1"], "-914801": ["108", "7.63", "spr_CultBirdDead", "1", "582", "239", "-1"], "-1951270": ["48", "9.10", "spr_RifleDirkDead", "1", "1187", "1090", "1"], "255832": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "597", "686", "1"], "-1937406": ["62", "2.37", "spr_DirkDead", "1", "522", "378", "-1"], "-166718": ["183", "14.45", "spr_RifleDirkDead", "1", "672", "917", "-1"], "471052": ["247", "29.58"], "-185752": ["181", "12.14"], "-63779": ["193", "16.10", "spr_RifleDirkDead", "1", "1097", "1473", "-1"], "-1346297": ["65", "32.08", "spr_SpiderDead", "1", "96", "434", "1"], "202483": ["220", "24.64", "spr_WolfDead", "1", "303", "244", "1"], "204267": ["220", "24.64", "spr_WolfDead", "1", "510", "352", "-1"], "-1523300": ["47", "8.71", "spr_DirkDead", "1", "781", "540", "-1"], "477748": ["247", "29.58"], "255772": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "596", "690", "-1"], "-168686": ["183", "14.45"], "-397447": ["160", "36.16", "spr_MissileDirkDead", "1", "272", "893", "-1"], "-938573": ["106", "7.06", "spr_RifleDirkDead", "1", "369", "417", "1"], "256897": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "814", "683", "1"], "-1518381": ["48", "9.10", "spr_DirkDead", "1", "1202", "1113", "-1"], "205619": ["220", "24.64", "spr_WolfDead", "1", "619", "333", "1"], "201283": ["220", "24.64", "spr_WolfDead", "1", "654", "376", "1"], "-387738": ["161", "36.54", "spr_RifleDirkDead", "1", "408", "146", "-1"], "-1816522": ["183", "14.45"], "185635": ["218", "30.84", "spr_TanukiDead", "1", "1196", "1062", "-1"], "204080": ["220", "24.64", "spr_WolfDead", "1", "562", "342", "1"], "-1816713": ["183", "14.45"], "-1375886": ["62", "2.37", "spr_DirkDead", "1", "504", "405", "-1"], "-164752": ["183", "14.45", "spr_RifleDirkDead", "1", "456", "779", "1"], "-1816137": ["183", "14.45", "spr_RifleDirkDead", "1", "641", "1088", "-1"], "-62566": ["193", "16.10", "spr_DirkDead", "1", "1287", "1454", "-1"], "202315": ["220", "24.64", "spr_WolfDead", "1", "507", "371", "-1"], "142529": ["214", "31.28", "spr_DirkDead", "1", "1228", "993", "-1"], "-1821511": ["178", "15.82", "spr_NinjaFrogDead", "1", "691", "199", "1"], "-1774601": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "761", "660", "1"], "-168534": ["183", "14.45"], "-1356259": ["64", "19.63", "spr_SpiderDead", "1", "421", "225", "1"], "-217560": ["178", "15.82", "spr_JarFrogDead", "1", "887", "319", "1"], "-167717": ["183", "14.45", "spr_RifleDirkDecapBottom", "1", "456", "761", "-1"], "-934904": ["106", "7.06", "spr_RifleDirkDead", "1", "356", "449", "1"], "255460": ["225", "30.15", "spr_RifleDirkDead", "1", "623", "676", "1"], "-63679": ["193", "16.10", "spr_DirkDead", "1", "1346", "1446", "-1"], "-1836741": ["163", "37.21"], "203862": ["220", "24.64", "spr_WolfDead", "1", "652", "358", "-1"], "203066": ["220", "24.64", "spr_WolfDead", "1", "507", "340", "1"], "-212353": ["178", "15.82", "spr_JarFrogDead", "1", "921", "201", "-1"], "-1353398": ["64", "19.63", "spr_SpiderDead", "1", "403", "214", "1"], "251259": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "832", "694", "1"], "-165301": ["183", "14.45", "spr_DirkDead", "1", "648", "897", "-1"], "-165346": ["183", "14.45", "spr_RifleDirkDead", "1", "673", "1088", "1"], "-1514532": ["48", "9.10", "spr_DirkDead", "1", "1245", "1094", "-1"], "-164347": ["183", "14.45"]}
-    assert testing_savefile.scUp == []
-    assert testing_savefile.checkX == 347.
-    assert testing_savefile.bossGearbits == []
-    assert testing_savefile.cues == ["-1092019", "-1092517", "-1073366", "-1055576", "-276126", "-1814127", "-147547", "-214027", "-716092"]
-    assert testing_savefile.playT == 41.
-    assert testing_savefile.well == ['1', '0', '2', '3']
-    assert testing_savefile.sc == ["1"]
-    assert testing_savefile.drifterkey == 0.
-    assert testing_savefile.successfulCollectTimes == 0.
-    assert testing_savefile.checkAmmo == 0.
-    assert testing_savefile.checkStash == 1.
-    assert testing_savefile.charDeaths == 12.
-    assert testing_savefile.eq00 == 1.
-    assert testing_savefile.healthKits == ["-1533639", "-1527212", "-1527041", "-934951", "-1353463", "-166798", "-178664", "-63791", "-53836", "146225", "-1774222", "-387903", "-367621", "-342346", "-673207"]
-    assert testing_savefile.sword == 0.
-    assert testing_savefile.gameName == "Q"
-
-def test_dump_and_load(tmp_path: Path, testing_savefile: HLDSaveFile):
-    testing_savefile.dump(p_join(tmp_path, "hello.sav"))
-    dumped_savefile = HLDSaveFile.load(p_join(tmp_path, "hello.sav"))
-    assert testing_savefile == dumped_savefile
-
-def test_dump_and_load_error(tmp_path: Path, testing_savefile: HLDSaveFile):
-    with pytest.raises(Exception):
-        testing_savefile.badass = ['1', '0', '2', '3'] # type: ignore
-        testing_savefile.dump(p_join(tmp_path, "hello.sav"))
-        HLDSaveFile.load(p_join(tmp_path, "hello.sav"))
-
-def test_sflist():
-    testing_sflist = hldsavefile.sflist.from_string("1+2+3+4+")
-    testing_sflist.append("5")
-    assert testing_sflist.to_string() == "1+2+3+4+5+"
-
-    testing_sflist = hldsavefile.sflist.from_string("1+2+3+4+")
-    testing_sflist.remove("2")
-    assert testing_sflist.to_string() == "1+3+4+"
-
-    testing_sflist = hldsavefile.sflist.from_string("")
-    assert testing_sflist.to_string() == ""
-
-    testing_sflist = hldsavefile.sflist.from_string("1+")
-    assert testing_sflist.to_string() == "1+"
-
-def test_sfdict():
-    testing_sflist = hldsavefile.sfdict.from_string("1=1&2&3&>2=4&5&6&>")
-    assert testing_sflist["1"] == ["1", "2", "3"]
-
-    testing_sflist["3"] = ["7", "8", "9"]
-    assert testing_sflist.to_string() == "1=1&2&3&>2=4&5&6&>3=7&8&9&>"
-
-    testing_sflist = hldsavefile.sfdict()
-    assert testing_sflist.to_string() == ""
-
-    testing_sflist = hldsavefile.sfdict({"1": ["1"]})
+from pathlib import Path
+from hldlib import HLDSaveFile, hldsavefile
+from os.path import join as p_join
+import pytest
+
+
+@pytest.fixture
+def testing_savefile() -> HLDSaveFile:
+    return HLDSaveFile.from_string("67eb87838659be77713bcdb237b0420a59d817df6eb7cd347d4b75823c138d6876d36e4eab448002eyJiYWRhc3MiOiAwLjAsICJtYXBNb2QiOiAiMTMyPTImPjE0ND0yJj4xNjE9MiY+MTgxPTImPjEwNj0yJj4xMDk9MiY+MTk0PTImPjIyNj0yJj4xODM9MiY+MTc0PTImPjE2MD0yJj4yMTg9MiY+OTU9MiY+MTA0PTImPjIyMD0yJj4yMTA9MiY+IiwgImRhdGVUaW1lIjogNDQ5ODAuNTI0MTI2LCAiaGVhbHRoVXAiOiAwLjAsICJjbCI6ICI5PTEwMTM4NyYxODUyNjcmMjA2MTM5JjI2Njc4NCY+MTM9LTE1MTg4NTEmPjc9LTI1NTEwMCYtMTg3OTA1Ji0xNjczMjYmLTUzMzkyJj42PS0xODk1NDgxJi0xMDQ3NDMwJi05MzI0NzEmLTkwMjIxMiY+OD0tNTU1Mjc5Ji0zOTg2MzUmLTM4NjQ1NyYtNjc2MzU3Jj4iLCAiZGVzdHJ1Y3QiOiAiLTM2MjI0Nj0xNjMmMzcuMjEmPjE4MjYxMj0yMTgmMzAuODQmPi0xOTc3OTEzPTIyMCYyNC42NCY+MTk1Mjk3PTIxOSYzMC40MyY+LTM2ODk5OT0xNjMmMzcuMjEmPjIwNDUwNT0yMjAmMjQuNjQmPjIwNDA1OD0yMjAmMjQuNjQmPjIwNTkwNz0yMjAmMjQuNjQmPjIwMzA3MT0yMjAmMjQuNjQmPi0xODIxODkwPTE3OCYxNS44MiY+LTY0OTEwPTE5MyYxNi4xMCY+LTE5NzkwMDE9MjA5JjMxLjg0Jj4tMTgyODY4ND0xNzEmMTkuMjkmPjE4MTM3Nj0yMTgmMzAuODQmPi0yMTU1NDE9MTc4JjE1LjgyJj4tMjE1MTIyPTE3OCYxNS44MiY+LTIxNDY5MT0xNzgmMTUuODImPi0yMTYyODI9MTc4JjE1LjgyJj4tMTgzNjE3Nj0xNjMmMzcuMjEmPi0xODI4MDIwPTE3MSYxOS4yOSY+MjAxMDk2PTIyMCYyNC42NCY+LTE3Nzk0MDg9MjIwJjI0LjY0Jj4tNDg2MTA9MTk1JjE3LjI5Jj4tMTc4MDI0MT0yMTkmMzAuNDMmPjIwNzQzNT0yMjAmMjQuNjQmPi0xOTE1ODQ1PTg0JjIuNzcmPi0zNTcwNzA9MTY0JjM4LjU1Jj4tMjEzNjY1PTE3OCYxNS44MiY+LTI1MzY3Mj0xNzQmMTguNTYmPjE4MjEwND0yMTgmMzAuODQmPjkxNTc2PTIwOSYzMS44NCY+LTIxMjE0MT0xNzgmMTUuODImPi0zNTQzNDg9MTY0JjM4LjU1Jj4xNDczNDg9MjE0JjMxLjI4Jj4tMjE3MTMzPTE3OCYxNS44MiY+OTQ1MDY9MjA5JjMxLjg0Jj4tMjEyMDI0PTE3OCYxNS44MiY+LTI1MjIwNj0xNzQmMTguNTYmPi0zNzMzOTU9MTYyJjM2Ljk4Jj4xODU1MjU9MjE4JjMwLjg0Jj4tMTk1MzYwNT00NiY4LjM1Jj4tMjcxOTUxPTE3MiYxOS4wNCY+LTI1NTc5Nz0xNzQmMTguNTYmPi0yMTI4MDM9MTc4JjE1LjgyJj4xODMyNDA9MjE4JjMwLjg0Jj4tMTgyMTYwNz0xNzgmMTUuODImPjE4NTM5Mz0yMTgmMzAuODQmPi0zNTY3MTY9MTY0JjM4LjU1Jj4tMjg3MjMyPTE3MSYxOS4yOSY+MTQ2OTcwPTIxNCYzMS4yOCY+LTE3Nzk4Mjc9MjIwJjI0LjY0Jj4yMDQ2MzY9MjIwJjI0LjY0Jj4xOTQ4NDA9MjE5JjMwLjQzJj4tMzUzMDY2PTE2NCYzOC41NSY+MTgyNDE4PTIxOCYzMC44NCY+MjA1ODYyPTIyMCYyNC42NCY+LTQyMzg3PTE5NSYxNy4yOSY+LTE3NzQyNjM9MjI1JjMwLjE1Jj4tMjE3MDUzPTE3OCYxNS44MiY+MjA0NTM1PTIyMCYyNC42NCY+LTM1MzI4Mj0xNjQmMzguNTUmPi0xNzgxNjk5PTIxOCYzMC44NCY+MTg3NTM3PTIxOCYzMC44NCY+LTE4MDUxMzg9MTk0JjE3LjQ3Jj4yMDc3NDM9MjIwJjI0LjY0Jj4tNjI0MTY9MTkzJjE2LjEwJj4tMjEzNDAyPTE3OCYxNS44MiY+LTM2MzM2Nz0xNjMmMzcuMjEmPi0yMTgwODQ9MTc4JjE1LjgyJj4tMzc1NTE0PTE2MiYzNi45OCY+LTY3NDcxPTE5MyYxNi4xMCY+LTE1MzI5NzY9NDYmOC4zNSY+MjAzOTA4PTIyMCYyNC42NCY+LTIxNTc5Mz0xNzgmMTUuODImPi0yMTIwNTM9MTc4JjE1LjgyJj4yMDM3NjM9MjIwJjI0LjY0Jj4tMzYyMzQ4PTE2MyYzNy4yMSY+MjAxNDI4PTIyMCYyNC42NCY+MTg0MTU1PTIxOCYzMC44NCY+MTgzOTM5PTIxOCYzMC44NCY+MTQ1MjUzPTIxNCYzMS4yOCY+MTQ1NzkyPTIxNCYzMS4yOCY+LTQ4NTUyPTE5NSYxNy4yOSY+LTI3NDcyMz0xNzImMTkuMDQmPiIsICJ2YWx1ZXMiOiAiVmFsdWViYWRhc3NPZmZpY2VTdGF0ZT0yPiIsICJndW5SZW1pbmRlclRpbWVzIjogMC4wLCAiZmlyZXBsYWNlU2F2ZSI6IDAuMCwgImNoZWNrSFAiOiA1LjAsICJjb21wU2hlbGwiOiAwLjAsICJjU3dvcmRzIjogIjArIiwgImNhcGUiOiAwLjAsICJoYWxsdWMiOiAwLjAsICJuZXdjb21lckhvYXJkZU1lc3NhZ2VTaG93biI6IDAuMCwgInR1dEhlYWwiOiAwLjAsICJub1NwYXduIjogIi0xMDk3OTU0Ky0xNDU1MDQrLTE4NzExNjUrIiwgImNoZWNrWSI6IDYwOC4wLCAic3BlY2lhbFVwIjogMC4wLCAiY2hlY2tCYXQiOiAxMDAuMCwgIm5vdmljZU1vZGUiOiAwLjAsICJzdWNjZXNzZnVsSGVhbFRpbWVzIjogNS4wLCAiY0NhcGVzIjogIjArIiwgIkNIIjogMC4wLCAiZ2VhciI6IDAuMCwgImNoZWNrQ0lEIjogNjI0NTMxLjAsICJyb29tcyI6ICI0Nis3OSs0Nys0OCs0OSs1MCs1Mys2MSs2Mis4NCs4NSs4OCs5MCs5Mis5Mys5NCsxMDQrOTUrMTA2KzEwNysxMDgrMTA5Kzk2Kzk3KzY0KzE3MSsxNzIrMTczKzE3NCsxNzUrMTc3KzE4MSsxODIrMTgzKzE4NCsxODUrMTc4KzE5MysxOTQrMTk1KzE5Nis2NSsyMDkrMjEwKzIxMSsyMTQrMjE4KzIxOSsyMjArMjI1KzIyNisyMzgrMjQ4KzI0NysyNDYrNjMrMTI4KzEzMCsxNDQrMTUyKzE2MCsxNjErMTYyKzE2MysxNjQrMTY1KzEzMisyNTYrMjU3KzI1OCsyNTkrMjYyKyIsICJwZXJtYVMiOiAiLTEwNDc5NDA9Mj4tNjkyMjMyPTI+LTEzODcwNTY9Mj4tNjk3MzYxPTI+LTE4MzM1Mz0yPjM4Mzk4OT0yPiIsICJjaGVja1Jvb20iOiAyNjIuMCwgIndlbGxNYXAiOiAiMSswKzIrMysiLCAiY1NoZWxscyI6ICIwKyIsICJ0YWJsZXQiOiAiIiwgInN1Y2Nlc3NmdWxXYXJwVGltZXMiOiAwLjAsICJza2lsbCI6ICIiLCAiYm9zc2VzIjogIjMuMjA9MzExJjIyNiY+IiwgInNjSyI6ICIxPTExPiIsICJ3YXJwIjogIjArMiszKyIsICJoYXNNYXAiOiAwLjAsICJldmVudHMiOiAiLTE1MzQyMTQrLTE1MTc2NjkrLTE0OTc2NjQrLTI1MjY5NCstMjI2OTc1Ky0xODA2NTkrLTE3NDg1NCstMTgyNDUzMystNDU2NzcrMjUzNDI2KzM4NTUwMSstMzk2MjcyKy0zNDQ5MjIrNTg2NjY2KzYyNjc3NisiLCAiZ2VhclJlbWluZGVyVGltZXMiOiAwLjAsICJlbmVtaWVzIjogIi0xODY4Mzk9MTgxJjEyLjE0Jj4tMTg2MjcxPTE4MSYxMi4xNCY+MjU1NTk4PTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjUxNiY2OTgmLTEmPjI1MTYxOD0yMjUmMzAuMTUmc3ByX1JpZmxlRGlya0RlYWQmMSY0OTUmNzIwJi0xJj4tMjEyODI1PTE3OCYxNS44MiZzcHJfTmluamFGcm9nRGVhZCYxJjczMyYxNjImLTEmPi0xNjM0MDk9MTgzJjE0LjQ1Jj4yMDI5NTk9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjY3MSYzNzMmMSY+LTkxNDgwMT0xMDgmNy42MyZzcHJfQ3VsdEJpcmREZWFkJjEmNTgyJjIzOSYtMSY+LTE5NTEyNzA9NDgmOS4xMCZzcHJfUmlmbGVEaXJrRGVhZCYxJjExODcmMTA5MCYxJj4yNTU4MzI9MjI1JjMwLjE1JnNwcl9TbWFsbENyeXN0YWxTcGlkZXJEZWFkJjEmNTk3JjY4NiYxJj4tMTkzNzQwNj02MiYyLjM3JnNwcl9EaXJrRGVhZCYxJjUyMiYzNzgmLTEmPi0xNjY3MTg9MTgzJjE0LjQ1JnNwcl9SaWZsZURpcmtEZWFkJjEmNjcyJjkxNyYtMSY+NDcxMDUyPTI0NyYyOS41OCY+LTE4NTc1Mj0xODEmMTIuMTQmPi02Mzc3OT0xOTMmMTYuMTAmc3ByX1JpZmxlRGlya0RlYWQmMSYxMDk3JjE0NzMmLTEmPi0xMzQ2Mjk3PTY1JjMyLjA4JnNwcl9TcGlkZXJEZWFkJjEmOTYmNDM0JjEmPjIwMjQ4Mz0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmMzAzJjI0NCYxJj4yMDQyNjc9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjUxMCYzNTImLTEmPi0xNTIzMzAwPTQ3JjguNzEmc3ByX0RpcmtEZWFkJjEmNzgxJjU0MCYtMSY+NDc3NzQ4PTI0NyYyOS41OCY+MjU1NzcyPTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjU5NiY2OTAmLTEmPi0xNjg2ODY9MTgzJjE0LjQ1Jj4tMzk3NDQ3PTE2MCYzNi4xNiZzcHJfTWlzc2lsZURpcmtEZWFkJjEmMjcyJjg5MyYtMSY+LTkzODU3Mz0xMDYmNy4wNiZzcHJfUmlmbGVEaXJrRGVhZCYxJjM2OSY0MTcmMSY+MjU2ODk3PTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjgxNCY2ODMmMSY+LTE1MTgzODE9NDgmOS4xMCZzcHJfRGlya0RlYWQmMSYxMjAyJjExMTMmLTEmPjIwNTYxOT0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNjE5JjMzMyYxJj4yMDEyODM9MjIwJjI0LjY0JnNwcl9Xb2xmRGVhZCYxJjY1NCYzNzYmMSY+LTM4NzczOD0xNjEmMzYuNTQmc3ByX1JpZmxlRGlya0RlYWQmMSY0MDgmMTQ2Ji0xJj4tMTgxNjUyMj0xODMmMTQuNDUmPjE4NTYzNT0yMTgmMzAuODQmc3ByX1RhbnVraURlYWQmMSYxMTk2JjEwNjImLTEmPjIwNDA4MD0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNTYyJjM0MiYxJj4tMTgxNjcxMz0xODMmMTQuNDUmPi0xMzc1ODg2PTYyJjIuMzcmc3ByX0RpcmtEZWFkJjEmNTA0JjQwNSYtMSY+LTE2NDc1Mj0xODMmMTQuNDUmc3ByX1JpZmxlRGlya0RlYWQmMSY0NTYmNzc5JjEmPi0xODE2MTM3PTE4MyYxNC40NSZzcHJfUmlmbGVEaXJrRGVhZCYxJjY0MSYxMDg4Ji0xJj4tNjI1NjY9MTkzJjE2LjEwJnNwcl9EaXJrRGVhZCYxJjEyODcmMTQ1NCYtMSY+MjAyMzE1PTIyMCYyNC42NCZzcHJfV29sZkRlYWQmMSY1MDcmMzcxJi0xJj4xNDI1Mjk9MjE0JjMxLjI4JnNwcl9EaXJrRGVhZCYxJjEyMjgmOTkzJi0xJj4tMTgyMTUxMT0xNzgmMTUuODImc3ByX05pbmphRnJvZ0RlYWQmMSY2OTEmMTk5JjEmPi0xNzc0NjAxPTIyNSYzMC4xNSZzcHJfU21hbGxDcnlzdGFsU3BpZGVyRGVhZCYxJjc2MSY2NjAmMSY+LTE2ODUzND0xODMmMTQuNDUmPi0xMzU2MjU5PTY0JjE5LjYzJnNwcl9TcGlkZXJEZWFkJjEmNDIxJjIyNSYxJj4tMjE3NTYwPTE3OCYxNS44MiZzcHJfSmFyRnJvZ0RlYWQmMSY4ODcmMzE5JjEmPi0xNjc3MTc9MTgzJjE0LjQ1JnNwcl9SaWZsZURpcmtEZWNhcEJvdHRvbSYxJjQ1NiY3NjEmLTEmPi05MzQ5MDQ9MTA2JjcuMDYmc3ByX1JpZmxlRGlya0RlYWQmMSYzNTYmNDQ5JjEmPjI1NTQ2MD0yMjUmMzAuMTUmc3ByX1JpZmxlRGlya0RlYWQmMSY2MjMmNjc2JjEmPi02MzY3OT0xOTMmMTYuMTAmc3ByX0RpcmtEZWFkJjEmMTM0NiYxNDQ2Ji0xJj4tMTgzNjc0MT0xNjMmMzcuMjEmPjIwMzg2Mj0yMjAmMjQuNjQmc3ByX1dvbGZEZWFkJjEmNjUyJjM1OCYtMSY+MjAzMDY2PTIyMCYyNC42NCZzcHJfV29sZkRlYWQmMSY1MDcmMzQwJjEmPi0yMTIzNTM9MTc4JjE1LjgyJnNwcl9KYXJGcm9nRGVhZCYxJjkyMSYyMDEmLTEmPi0xMzUzMzk4PTY0JjE5LjYzJnNwcl9TcGlkZXJEZWFkJjEmNDAzJjIxNCYxJj4yNTEyNTk9MjI1JjMwLjE1JnNwcl9TbWFsbENyeXN0YWxTcGlkZXJEZWFkJjEmODMyJjY5NCYxJj4tMTY1MzAxPTE4MyYxNC40NSZzcHJfRGlya0RlYWQmMSY2NDgmODk3Ji0xJj4tMTY1MzQ2PTE4MyYxNC40NSZzcHJfUmlmbGVEaXJrRGVhZCYxJjY3MyYxMDg4JjEmPi0xNTE0NTMyPTQ4JjkuMTAmc3ByX0RpcmtEZWFkJjEmMTI0NSYxMDk0Ji0xJj4tMTY0MzQ3PTE4MyYxNC40NSY+IiwgInNjVXAiOiAiIiwgImNoZWNrWCI6IDM0Ny4wLCAiYm9zc0dlYXJiaXRzIjogIiIsICJjdWVzIjogIi0xMDkyMDE5Ky0xMDkyNTE3Ky0xMDczMzY2Ky0xMDU1NTc2Ky0yNzYxMjYrLTE4MTQxMjcrLTE0NzU0NystMjE0MDI3Ky03MTYwOTIrIiwgInBsYXlUIjogNDEuMCwgIndlbGwiOiAiMSswKzIrMysiLCAic2MiOiAiMSsiLCAiZHJpZnRlcmtleSI6IDAuMCwgInN1Y2Nlc3NmdWxDb2xsZWN0VGltZXMiOiAwLjAsICJjaGVja0FtbW8iOiAwLjAsICJjaGVja1N0YXNoIjogMS4wLCAiY2hhckRlYXRocyI6IDEyLjAsICJlcTAwIjogMS4wLCAiaGVhbHRoS2l0cyI6ICItMTUzMzYzOSstMTUyNzIxMistMTUyNzA0MSstOTM0OTUxKy0xMzUzNDYzKy0xNjY3OTgrLTE3ODY2NCstNjM3OTErLTUzODM2KzE0NjIyNSstMTc3NDIyMistMzg3OTAzKy0zNjc2MjErLTM0MjM0NistNjczMjA3KyIsICJzd29yZCI6IDAuMCwgImdhbWVOYW1lIjogIlEifSA=")
+
+def test_load(testing_savefile: HLDSaveFile):
+    assert testing_savefile.badass == 0.
+    assert testing_savefile.mapMod == {"132": ["2"], "144": ["2"], "161": ["2"], "181": ["2"], "106": ["2"], "109": ["2"], "194": ["2"], "226": ["2"], "183": ["2"], "174": ["2"], "160": ["2"], "218": ["2"], "95": ["2"], "104": ["2"], "220": ["2"], "210": ["2"]}
+    assert testing_savefile.dateTime == 44980.524126
+    assert testing_savefile.healthUp == 0.
+    assert testing_savefile.cl == {"9": ["101387", "185267", "206139", "266784"], "13": ["-1518851"], "7": ["-255100", "-187905", "-167326", "-53392"], "6": ["-1895481", "-1047430", "-932471", "-902212"], "8": ["-555279", "-398635", "-386457", "-676357"]}
+    assert testing_savefile.destruct == {"-362246": ["163", "37.21"], "182612": ["218", "30.84"], "-1977913": ["220", "24.64"], "195297": ["219", "30.43"], "-368999": ["163", "37.21"], "204505": ["220", "24.64"], "204058": ["220", "24.64"], "205907": ["220", "24.64"], "203071": ["220", "24.64"], "-1821890": ["178", "15.82"], "-64910": ["193", "16.10"], "-1979001": ["209", "31.84"], "-1828684": ["171", "19.29"], "181376": ["218", "30.84"], "-215541": ["178", "15.82"], "-215122": ["178", "15.82"], "-214691": ["178", "15.82"], "-216282": ["178", "15.82"], "-1836176": ["163", "37.21"], "-1828020": ["171", "19.29"], "201096": ["220", "24.64"], "-1779408": ["220", "24.64"], "-48610": ["195", "17.29"], "-1780241": ["219", "30.43"], "207435": ["220", "24.64"], "-1915845": ["84", "2.77"], "-357070": ["164", "38.55"], "-213665": ["178", "15.82"], "-253672": ["174", "18.56"], "182104": ["218", "30.84"], "91576": ["209", "31.84"], "-212141": ["178", "15.82"], "-354348": ["164", "38.55"], "147348": ["214", "31.28"], "-217133": ["178", "15.82"], "94506": ["209", "31.84"], "-212024": ["178", "15.82"], "-252206": ["174", "18.56"], "-373395": ["162", "36.98"], "185525": ["218", "30.84"], "-1953605": ["46", "8.35"], "-271951": ["172", "19.04"], "-255797": ["174", "18.56"], "-212803": ["178", "15.82"], "183240": ["218", "30.84"], "-1821607": ["178", "15.82"], "185393": ["218", "30.84"], "-356716": ["164", "38.55"], "-287232": ["171", "19.29"], "146970": ["214", "31.28"], "-1779827": ["220", "24.64"], "204636": ["220", "24.64"], "194840": ["219", "30.43"], "-353066": ["164", "38.55"], "182418": ["218", "30.84"], "205862": ["220", "24.64"], "-42387": ["195", "17.29"], "-1774263": ["225", "30.15"], "-217053": ["178", "15.82"], "204535": ["220", "24.64"], "-353282": ["164", "38.55"], "-1781699": ["218", "30.84"], "187537": ["218", "30.84"], "-1805138": ["194", "17.47"], "207743": ["220", "24.64"], "-62416": ["193", "16.10"], "-213402": ["178", "15.82"], "-363367": ["163", "37.21"], "-218084": ["178", "15.82"], "-375514": ["162", "36.98"], "-67471": ["193", "16.10"], "-1532976": ["46", "8.35"], "203908": ["220", "24.64"], "-215793": ["178", "15.82"], "-212053": ["178", "15.82"], "203763": ["220", "24.64"], "-362348": ["163", "37.21"], "201428": ["220", "24.64"], "184155": ["218", "30.84"], "183939": ["218", "30.84"], "145253": ["214", "31.28"], "145792": ["214", "31.28"], "-48552": ["195", "17.29"], "-274723": ["172", "19.04"]}
+    assert testing_savefile.values == {'ValuebadassOfficeState': ['2']}
+    assert testing_savefile.gunReminderTimes == 0.
+    assert testing_savefile.fireplaceSave == 0.
+    assert testing_savefile.checkHP == 5.
+    assert testing_savefile.compShell == 0.
+    assert testing_savefile.cSwords == ["0"]
+    assert testing_savefile.cape == 0.
+    assert testing_savefile.halluc == 0.
+    assert testing_savefile.newcomerHoardeMessageShown == 0.
+    assert testing_savefile.tutHeal == 0.
+    assert testing_savefile.noSpawn == ['-1097954', '-145504', '-1871165']
+    assert testing_savefile.checkY == 608.
+    assert testing_savefile.specialUp == 0.
+    assert testing_savefile.checkBat == 100.
+    assert testing_savefile.noviceMode == 0.
+    assert testing_savefile.successfulHealTimes == 5.
+    assert testing_savefile.cCapes == ["0"]
+    assert testing_savefile.CH == 0.
+    assert testing_savefile.gear == 0.
+    assert testing_savefile.checkCID == 624531.
+    assert testing_savefile.rooms == ["46", "79", "47", "48", "49", "50", "53", "61", "62", "84", "85", "88", "90", "92", "93", "94", "104", "95", "106", "107", "108", "109", "96", "97", "64", "171", "172", "173", "174", "175", "177", "181", "182", "183", "184", "185", "178", "193", "194", "195", "196", "65", "209", "210", "211", "214", "218", "219", "220", "225", "226", "238", "248", "247", "246", "63", "128", "130", "144", "152", "160", "161", "162", "163", "164", "165", "132", "256", "257", "258", "259", "262"]
+    assert testing_savefile.permaS == {"-1047940": ["2"], "-692232": ["2"], "-1387056": ["2"], "-697361": ["2"], "-183353": ["2"], "383989": ["2"]}
+    assert testing_savefile.checkRoom == 262.
+    assert testing_savefile.wellMap == ["1", "0", "2", "3"]
+    assert testing_savefile.cShells == ["0"]
+    assert testing_savefile.eq01 == 0.
+    assert testing_savefile.tablet == []
+    assert testing_savefile.successfulWarpTimes == 0.
+    assert testing_savefile.skill == []
+    assert testing_savefile.bosses == {'3.20': ['311', '226']}
+    assert testing_savefile.scK == {'1': ['11']}
+    assert testing_savefile.warp == ['0', '2', '3']
+    assert testing_savefile.hasMap == 0.
+    assert testing_savefile.events == ["-1534214", "-1517669", "-1497664", "-252694", "-226975", "-180659", "-174854", "-1824533", "-45677", "253426", "385501", "-396272", "-344922", "586666", "626776"]
+    assert testing_savefile.gearReminderTimes == 0.
+    assert testing_savefile.enemies == {"-186839": ["181", "12.14"], "-186271": ["181", "12.14"], "255598": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "516", "698", "-1"], "251618": ["225", "30.15", "spr_RifleDirkDead", "1", "495", "720", "-1"], "-212825": ["178", "15.82", "spr_NinjaFrogDead", "1", "733", "162", "-1"], "-163409": ["183", "14.45"], "202959": ["220", "24.64", "spr_WolfDead", "1", "671", "373", "1"], "-914801": ["108", "7.63", "spr_CultBirdDead", "1", "582", "239", "-1"], "-1951270": ["48", "9.10", "spr_RifleDirkDead", "1", "1187", "1090", "1"], "255832": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "597", "686", "1"], "-1937406": ["62", "2.37", "spr_DirkDead", "1", "522", "378", "-1"], "-166718": ["183", "14.45", "spr_RifleDirkDead", "1", "672", "917", "-1"], "471052": ["247", "29.58"], "-185752": ["181", "12.14"], "-63779": ["193", "16.10", "spr_RifleDirkDead", "1", "1097", "1473", "-1"], "-1346297": ["65", "32.08", "spr_SpiderDead", "1", "96", "434", "1"], "202483": ["220", "24.64", "spr_WolfDead", "1", "303", "244", "1"], "204267": ["220", "24.64", "spr_WolfDead", "1", "510", "352", "-1"], "-1523300": ["47", "8.71", "spr_DirkDead", "1", "781", "540", "-1"], "477748": ["247", "29.58"], "255772": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "596", "690", "-1"], "-168686": ["183", "14.45"], "-397447": ["160", "36.16", "spr_MissileDirkDead", "1", "272", "893", "-1"], "-938573": ["106", "7.06", "spr_RifleDirkDead", "1", "369", "417", "1"], "256897": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "814", "683", "1"], "-1518381": ["48", "9.10", "spr_DirkDead", "1", "1202", "1113", "-1"], "205619": ["220", "24.64", "spr_WolfDead", "1", "619", "333", "1"], "201283": ["220", "24.64", "spr_WolfDead", "1", "654", "376", "1"], "-387738": ["161", "36.54", "spr_RifleDirkDead", "1", "408", "146", "-1"], "-1816522": ["183", "14.45"], "185635": ["218", "30.84", "spr_TanukiDead", "1", "1196", "1062", "-1"], "204080": ["220", "24.64", "spr_WolfDead", "1", "562", "342", "1"], "-1816713": ["183", "14.45"], "-1375886": ["62", "2.37", "spr_DirkDead", "1", "504", "405", "-1"], "-164752": ["183", "14.45", "spr_RifleDirkDead", "1", "456", "779", "1"], "-1816137": ["183", "14.45", "spr_RifleDirkDead", "1", "641", "1088", "-1"], "-62566": ["193", "16.10", "spr_DirkDead", "1", "1287", "1454", "-1"], "202315": ["220", "24.64", "spr_WolfDead", "1", "507", "371", "-1"], "142529": ["214", "31.28", "spr_DirkDead", "1", "1228", "993", "-1"], "-1821511": ["178", "15.82", "spr_NinjaFrogDead", "1", "691", "199", "1"], "-1774601": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "761", "660", "1"], "-168534": ["183", "14.45"], "-1356259": ["64", "19.63", "spr_SpiderDead", "1", "421", "225", "1"], "-217560": ["178", "15.82", "spr_JarFrogDead", "1", "887", "319", "1"], "-167717": ["183", "14.45", "spr_RifleDirkDecapBottom", "1", "456", "761", "-1"], "-934904": ["106", "7.06", "spr_RifleDirkDead", "1", "356", "449", "1"], "255460": ["225", "30.15", "spr_RifleDirkDead", "1", "623", "676", "1"], "-63679": ["193", "16.10", "spr_DirkDead", "1", "1346", "1446", "-1"], "-1836741": ["163", "37.21"], "203862": ["220", "24.64", "spr_WolfDead", "1", "652", "358", "-1"], "203066": ["220", "24.64", "spr_WolfDead", "1", "507", "340", "1"], "-212353": ["178", "15.82", "spr_JarFrogDead", "1", "921", "201", "-1"], "-1353398": ["64", "19.63", "spr_SpiderDead", "1", "403", "214", "1"], "251259": ["225", "30.15", "spr_SmallCrystalSpiderDead", "1", "832", "694", "1"], "-165301": ["183", "14.45", "spr_DirkDead", "1", "648", "897", "-1"], "-165346": ["183", "14.45", "spr_RifleDirkDead", "1", "673", "1088", "1"], "-1514532": ["48", "9.10", "spr_DirkDead", "1", "1245", "1094", "-1"], "-164347": ["183", "14.45"]}
+    assert testing_savefile.scUp == []
+    assert testing_savefile.checkX == 347.
+    assert testing_savefile.bossGearbits == []
+    assert testing_savefile.cues == ["-1092019", "-1092517", "-1073366", "-1055576", "-276126", "-1814127", "-147547", "-214027", "-716092"]
+    assert testing_savefile.playT == 41.
+    assert testing_savefile.well == ['1', '0', '2', '3']
+    assert testing_savefile.sc == ["1"]
+    assert testing_savefile.drifterkey == 0.
+    assert testing_savefile.successfulCollectTimes == 0.
+    assert testing_savefile.checkAmmo == 0.
+    assert testing_savefile.checkStash == 1.
+    assert testing_savefile.charDeaths == 12.
+    assert testing_savefile.eq00 == 1.
+    assert testing_savefile.healthKits == ["-1533639", "-1527212", "-1527041", "-934951", "-1353463", "-166798", "-178664", "-63791", "-53836", "146225", "-1774222", "-387903", "-367621", "-342346", "-673207"]
+    assert testing_savefile.sword == 0.
+    assert testing_savefile.gameName == "Q"
+
+def test_dump_and_load(tmp_path: Path, testing_savefile: HLDSaveFile):
+    testing_savefile.dump(p_join(tmp_path, "hello.sav"))
+    dumped_savefile = HLDSaveFile.load(p_join(tmp_path, "hello.sav"))
+    assert testing_savefile == dumped_savefile
+
+def test_dump_and_load_error(tmp_path: Path, testing_savefile: HLDSaveFile):
+    with pytest.raises(Exception):
+        testing_savefile.badass = ['1', '0', '2', '3'] # type: ignore
+        testing_savefile.dump(p_join(tmp_path, "hello.sav"))
+        HLDSaveFile.load(p_join(tmp_path, "hello.sav"))
+
+def test_sflist():
+    testing_sflist = hldsavefile.sflist.from_string("1+2+3+4+")
+    testing_sflist.append("5")
+    assert testing_sflist.to_string() == "1+2+3+4+5+"
+
+    testing_sflist = hldsavefile.sflist.from_string("1+2+3+4+")
+    testing_sflist.remove("2")
+    assert testing_sflist.to_string() == "1+3+4+"
+
+    testing_sflist = hldsavefile.sflist.from_string("")
+    assert testing_sflist.to_string() == ""
+
+    testing_sflist = hldsavefile.sflist.from_string("1+")
+    assert testing_sflist.to_string() == "1+"
+
+def test_sfdict():
+    testing_sflist = hldsavefile.sfdict.from_string("1=1&2&3&>2=4&5&6&>")
+    assert testing_sflist["1"] == ["1", "2", "3"]
+
+    testing_sflist["3"] = ["7", "8", "9"]
+    assert testing_sflist.to_string() == "1=1&2&3&>2=4&5&6&>3=7&8&9&>"
+
+    testing_sflist = hldsavefile.sfdict()
+    assert testing_sflist.to_string() == ""
+
+    testing_sflist = hldsavefile.sfdict({"1": ["1"]})
     assert testing_sflist.to_string() == "1=1&>"
```

