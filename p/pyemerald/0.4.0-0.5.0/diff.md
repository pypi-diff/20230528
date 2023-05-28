# Comparing `tmp/pyemerald-0.4.0.tar.gz` & `tmp/pyemerald-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemerald-0.4.0.tar", max compression
+gzip compressed data, was "pyemerald-0.5.0.tar", max compression
```

## Comparing `pyemerald-0.4.0.tar` & `pyemerald-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.4.0/pyemerald/__init__.py
--rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/codec.py
--rw-r--r--   0        0        0      641 2023-05-23 13:28:34.597606 pyemerald-0.4.0/pyemerald/constants.py
--rw-r--r--   0        0        0     1656 2023-05-23 13:28:34.597606 pyemerald-0.4.0/pyemerald/game.py
--rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/items.py
--rw-r--r--   0        0        0     1922 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/level.py
--rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/moves.py
--rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/nature_stats.py
--rw-r--r--   0        0        0    34516 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/pokemon.py
--rw-r--r--   0        0        0    97687 2023-05-26 09:18:23.814630 pyemerald-0.4.0/pyemerald/pokemon_info.py
--rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/raw_section.py
--rw-r--r--   0        0        0     6323 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/save.py
--rw-r--r--   0        0        0     7157 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/section.py
--rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.4.0/pyemerald/utils.py
--rw-r--r--   0        0        0      531 2023-05-26 09:21:29.622887 pyemerald-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2568 2023-05-26 09:23:12.700552 pyemerald-0.4.0/setup.py
--rw-r--r--   0        0        0     2551 2023-05-26 09:23:12.700879 pyemerald-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.5.0/pyemerald/__init__.py
+-rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/codec.py
+-rw-r--r--   0        0        0      641 2023-05-23 13:28:34.597606 pyemerald-0.5.0/pyemerald/constants.py
+-rw-r--r--   0        0        0     1798 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/game.py
+-rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/items.py
+-rw-r--r--   0        0        0     3045 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/level.py
+-rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.5.0/pyemerald/moves.py
+-rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/nature_stats.py
+-rw-r--r--   0        0        0    36653 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/pokemon.py
+-rw-r--r--   0        0        0    98431 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/pokemon_info.py
+-rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.5.0/pyemerald/raw_section.py
+-rw-r--r--   0        0        0     6425 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/save.py
+-rw-r--r--   0        0        0     7257 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/section.py
+-rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.5.0/pyemerald/utils.py
+-rw-r--r--   0        0        0      531 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2568 2023-05-28 13:56:30.968651 pyemerald-0.5.0/setup.py
+-rw-r--r--   0        0        0     2551 2023-05-28 13:56:30.969011 pyemerald-0.5.0/PKG-INFO
```

### Comparing `pyemerald-0.4.0/LICENSE.txt` & `pyemerald-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/README.md` & `pyemerald-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/codec.py` & `pyemerald-0.5.0/pyemerald/codec.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/constants.py` & `pyemerald-0.5.0/pyemerald/constants.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/game.py` & `pyemerald-0.5.0/pyemerald/game.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,10 @@
             raise ValueError(f"Multiple sections with {section_id=}")
 
     def add_pc_item(self, item: Item):
         self.get_section(TeamItemSection).add_pc_item(item)
 
     def add_pc_pokemon(self, pokemon: PCPokemon):
         self.get_section(PCBufferInitSection).add_pc_pokemon(pokemon)
+
+    def insert_pc_pokemon(self, pokemon: PCPokemon, idx: int):
+        self.get_section(PCBufferInitSection).insert_pc_pokemon(pokemon, idx)
```

### Comparing `pyemerald-0.4.0/pyemerald/items.py` & `pyemerald-0.5.0/pyemerald/items.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/level.py` & `pyemerald-0.5.0/pyemerald/level.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,71 +5,113 @@
 from pyemerald.pokemon_info import POKE_INFO
 
 
 class Level:
     def __init__(self, pokemon_name: str):
         self.name = pokemon_name
 
+    @property
+    def exp_type_index(self) -> int:
+        return POKE_INFO[self.name]["exp_type"]
+
     def determine_growth_curve(self):
-        exp_type_index = POKE_INFO[self.name]["exp_type"]
-        return EXP_TYPE_MAP[exp_type_index]
+        return EXP_TYPE_MAP[self.exp_type_index]
 
     def calc_exp(self, level: int) -> int:
         """Calculate the experience required for the pokemon
         to reach a certain level"""
         if level > 100:
             raise ValueError("Level cannot be above 100!")
 
         if level < 1:
             raise ValueError("Level cannot be below 0!")
 
         growth_func = self.determine_growth_curve()
 
         return int(growth_func(level))
 
+    def get_level_from_exp(self, exp: int) -> int:
+        """Calculate the level based on experience points"""
+        for row in EXP_TO_LEVEL[self.exp_type_index]:
+            low = row[0]
+            high = row[1]
+            level = row[2]
+            if exp >= low and exp <= high:
+                return level
+
+            if level == 99:
+                # If the function didn't return in the above
+                # if clause exp will be larger than the bounds
+                # for 99, thus level has to be 100
+                return 100
+
 
 def level_erratic(level: int) -> int:
-    if level < 50:
-        return level**3 * (100 - level) / 50
+    if level == 1:
+        return 0
+    elif level < 50:
+        res = level**3 * (100 - level) / 50
     elif level >= 50 and level < 68:
-        return level**3 * (150 - level) / 100
+        res = level**3 * (150 - level) / 100
     elif level >= 68 and level < 98:
-        return level**3 * int((1911 - 10 * level) / 3) / 500
+        res = level**3 * int((1911 - 10 * level) / 3) / 500
     elif level >= 98 and level < 100:
-        return level**3 * (160 - level) / 100
-    return 600_000
+        res = level**3 * (160 - level) / 100
+    else:
+        res = 600_000
+    return int(res)
 
 
 def level_fast(level: int) -> int:
-    return 4 * level**3 / 5
+    if level == 1:
+        return 0
+    return int(4 * level**3 / 5)
 
 
 def level_medium_fast(level: int) -> int:
-    return level**3
+    if level == 1:
+        return 0
+    return int(level**3)
 
 
 def level_medium_slow(level: int) -> int:
-    return 6 / 5 * level**3 - 15 * level**2 + 100 * level - 140
+    if level == 1:
+        return 0
+    return int(6 / 5 * level**3 - 15 * level**2 + 100 * level - 140)
 
 
 def level_slow(level: int) -> int:
-    return 5 / 4 * level**3
+    if level == 1:
+        return 0
+    return int(5 / 4 * level**3)
 
 
 def level_fluctuating(level: int) -> int:
-    if level < 15:
-        return level**3 * (int((level + 1) / 3) + 24)
+    if level == 1:
+        return 0
+    elif level < 15:
+        res = level**3 * (int((level + 1) / 3) + 24) / 50
     elif level >= 15 and level < 36:
-        return level**3 * (level + 14) / 50
+        res = level**3 * (level + 14) / 50
     elif level >= 36 and level < 100:
-        return level**3 * (int(level / 2) + 32) / 50
-    return 1_640_000
+        res = level**3 * (int(level / 2) + 32) / 50
+    else:
+        res = 1_640_000
+    return int(res)
 
 
 EXP_TYPE_MAP = {
     0: level_erratic,
     1: level_fast,
     2: level_medium_fast,
     3: level_medium_slow,
     4: level_slow,
     5: level_fluctuating,
 }
+
+# Calculate table for reverse lookup exp -> level
+EXP_TO_LEVEL = {
+    idx: [
+        (level_func(level), level_func(level + 1) - 1, level) for level in range(1, 100)
+    ]
+    for idx, level_func in EXP_TYPE_MAP.items()
+}
```

### Comparing `pyemerald-0.4.0/pyemerald/moves.py` & `pyemerald-0.5.0/pyemerald/moves.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/nature_stats.py` & `pyemerald-0.5.0/pyemerald/nature_stats.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/pokemon.py` & `pyemerald-0.5.0/pyemerald/pokemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Module implementing all logic related to a Pokemon
 e.g. Stats, moves, original trainer etc.
 """
 from typing import Type, List, Union, ClassVar, Optional, Dict
 from dataclasses import dataclass
 import random
+import copy
 import string
 from pyemerald.codec import (
     Codec,
     ByteFieldCodec,
     bytes_to_int,
     int_to_bytes,
     Serializable,
     ByteDeltaField,
 )
 from pyemerald.constants import POKEMON_DATA_SUBSTRUCT_SIZE
 from pyemerald.moves import INT_TO_MOVE, MOVE_TO_INT, Move
 from pyemerald.items import Item
-from pyemerald.pokemon_info import POKE_INFO
+from pyemerald.pokemon_info import PokemonInfo
 from pyemerald.level import Level
 from pyemerald.utils import get_bits_by_position
 from pyemerald.nature_stats import Stat, Nature
 
 
 class PCPokemonCodec(Codec):
     def __init__(self, section_class: Type["Serializable"]):
@@ -660,15 +661,15 @@
             feel=feel,
         )
 
         level_calc = Level(name)
         experience = level_calc.calc_exp(level)
 
         growth = PokemonDataGrowth(
-            species=POKE_INFO[name]["id"],
+            species=PokemonInfo.from_name(name).id,
             item_held=item_held.index if item_held is not None else 0,
             experience=experience,
             pp_bonus=pp_bonus,
             friendship=friendship,
             unknown=b"\x00\x00",
         )
 
@@ -821,15 +822,26 @@
         return PCPokemon.calc_checksum(self.pokemon_data.to_bytes_unencrypted())
 
     @checksum.setter
     def checksum(self, value):
         self.raw_checksum = value
 
     @property
-    def species(self):
+    def pokemon_info(self) -> PokemonInfo:
+        # Get species ID
+        _id = self.species
+        return PokemonInfo.from_id(_id)
+
+    @property
+    def name(self) -> str:
+        poke_info = self.pokemon_info
+        return poke_info.name
+
+    @property
+    def species(self) -> int:
         return self.pokemon_data.get_struct_by_type(PokemonDataGrowth).species
 
     @species.setter
     def species(self, value):
         self.pokemon_data.get_struct_by_type(PokemonDataGrowth).species = value
 
     @property
@@ -837,14 +849,19 @@
         return self.pokemon_data.get_struct_by_type(PokemonDataGrowth).species
 
     @experience.setter
     def experience(self, value):
         self.pokemon_data.get_struct_by_type(PokemonDataGrowth).experience = value
 
     @property
+    def get_level(self) -> int:
+        level_obj = Level(self.name)
+        return level_obj.get_level_from_exp(self.experience)
+
+    @property
     def move_1(self):
         return self._get_move(1)
 
     @property
     def move_2(self):
         return self._get_move(2)
 
@@ -1062,32 +1079,81 @@
         # Add values specific for this class
         values["status_condition"] = 0
 
         # Nature
         nature = Nature.from_personality_value(values["personality_value"])
 
         # Calc stats
-        poke_info = POKE_INFO[name]
-        hp_stat = Stat("hp", poke_info["hp"], iv_hp, ev_hp, level)
-        attack_stat = Stat("attack", poke_info["attack"], iv_attack, ev_attack, level)
-        defense_stat = Stat(
-            "defense", poke_info["defense"], iv_defense, ev_defense, level
-        )
-        speed_stat = Stat("speed", poke_info["speed"], iv_speed, ev_speed, level)
+        poke_info = PokemonInfo.from_name(name)
+        hp_stat = Stat("hp", poke_info.hp, iv_hp, ev_hp, level)
+        attack_stat = Stat("attack", poke_info.attack, iv_attack, ev_attack, level)
+        defense_stat = Stat("defense", poke_info.defense, iv_defense, ev_defense, level)
+        speed_stat = Stat("speed", poke_info.speed, iv_speed, ev_speed, level)
         sp_attack_stat = Stat(
-            "sp_attack", poke_info["sp_attack"], iv_sp_attack, ev_sp_attack, level
+            "sp_attack", poke_info.sp_attack, iv_sp_attack, ev_sp_attack, level
         )
         sp_defense_stat = Stat(
-            "sp_defense", poke_info["sp_defense"], iv_sp_defense, ev_sp_defense, level
+            "sp_defense", poke_info.sp_defense, iv_sp_defense, ev_sp_defense, level
         )
 
         values["level"] = level
         values["pokerus"] = 255
         values["current_hp"] = hp_stat.total_stat(nature=nature)
         values["total_hp"] = hp_stat.total_stat(nature=nature)
         values["attack"] = attack_stat.total_stat(nature=nature)
         values["defense"] = defense_stat.total_stat(nature=nature)
         values["speed"] = speed_stat.total_stat(nature=nature)
         values["sp_attack"] = sp_attack_stat.total_stat(nature=nature)
         values["sp_defense"] = sp_defense_stat.total_stat(nature=nature)
 
         return cls(**values)
+
+    def to_pc_pokemon(self) -> PCPokemon:
+
+        # Get EV
+        evs = self.pokemon_data.get_struct_by_type(PokemonDataEV)
+
+        # Get misc
+        misc = self.pokemon_data.get_struct_by_type(PokemonDataMisc)
+
+        # Get IV
+        ivs = misc.ivs_egg
+
+        # Get Growth data
+        growth = self.pokemon_data.get_struct_by_type(PokemonDataGrowth)
+
+        values = {
+            "name": self.name,
+            "level": self.get_level,
+            "move_1": self.move_1,
+            "move_2": self.move_2,
+            "move_3": self.move_3,
+            "move_4": self.move_4,
+            "ev_hp": evs.hp,
+            "ev_attack": evs.attack,
+            "ev_defense": evs.defense,
+            "ev_speed": evs.speed,
+            "ev_sp_attack": evs.sp_attack,
+            "ev_sp_defense": evs.sp_defense,
+            "iv_hp": ivs.hp,
+            "iv_attack": ivs.attack,
+            "iv_defense": ivs.defense,
+            "iv_speed": ivs.speed,
+            "iv_sp_attack": ivs.sp_attack,
+            "iv_sp_defense": ivs.sp_defense,
+            "coolness": evs.coolness,
+            "beauty": evs.beauty,
+            "cuteness": evs.cuteness,
+            "smartness": evs.smartness,
+            "toughness": evs.toughness,
+            "feel": evs.feel,
+            "item_held": Item.from_number(growth.item_held, 1),
+            "friendship": growth.friendship,
+            "pp_bonus": growth.pp_bonus,
+            "pokerus": misc.pokerus,
+            "nickname": self.nickname,
+            "personality_value": self.personality_value,
+            "original_trainer_id": self.original_trainer_id,
+            "original_trainer_name": self.original_trainer_name,
+        }
+
+        return PCPokemon.from_name(**values)
```

### Comparing `pyemerald-0.4.0/pyemerald/pokemon_info.py` & `pyemerald-0.5.0/pyemerald/pokemon_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+from dataclasses import dataclass
+from typing import Optional
+import copy
+
+
+@dataclass
+class PokemonInfo:
+    name: str
+    id: int
+    type_1: str
+    type_2: Optional[str]
+    exp_type: int
+    hp: int
+    attack: int
+    defense: int
+    speed: int
+    sp_attack: int
+    sp_defense: int
+
+    @classmethod
+    def from_name(cls, name: str) -> "PokemonInfo":
+        values = POKE_INFO[name]
+        values["name"] = name
+        return cls(**values)
+
+    @classmethod
+    def from_id(cls, _id: int) -> "PokemonInfo":
+        values = POKE_INFO_ID[_id]
+        values["id"] = _id
+        return cls(**values)
+
+
 POKE_INFO = {
     "Bulbasaur": {
         "id": 1,
         "type_1": "Grass",
         "type_2": None,
         "exp_type": 3,
         "hp": 45,
@@ -4628,7 +4660,13 @@
         "attack": 50,
         "defense": 70,
         "speed": 65,
         "sp_attack": 95,
         "sp_defense": 80,
     },
 }
+
+POKE_INFO_ID = {}
+for k, v in copy.deepcopy(POKE_INFO).items():
+    v["name"] = k
+    _id = v.pop("id")
+    POKE_INFO_ID[_id] = v
```

### Comparing `pyemerald-0.4.0/pyemerald/raw_section.py` & `pyemerald-0.5.0/pyemerald/raw_section.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyemerald/save.py` & `pyemerald-0.5.0/pyemerald/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,18 +125,15 @@
     updated: bool = False
 
     def __post_init__(self):
         if len(self.slots) > 2:
             raise ValueError("No more than two slots!")
 
     @classmethod
-    def from_file(cls, path: str) -> "Save":
-        with open(path, "rb") as f:
-            data = f.read()
-
+    def from_bytes(cls, data: bytes) -> "Save":
         slot0 = Slot.from_bytes(data[:SLOT_SIZE])
         slot1 = Slot.from_bytes(data[SLOT_SIZE : SLOT_SIZE * 2])
 
         hall_of_fame = data[
             HALL_OF_FAME_OFFSET : HALL_OF_FAME_OFFSET + HALL_OF_FAME_SIZE
         ]
         mystery_gift = data[
@@ -149,14 +146,21 @@
         return Save(
             slots=[slot0, slot1],
             hall_of_fame=hall_of_fame,
             mystery_gift=mystery_gift,
             recorded_battle=recorded_battle,
         )
 
+    @classmethod
+    def from_file(cls, path: str) -> "Save":
+        with open(path, "rb") as f:
+            data = f.read()
+
+        return cls.from_bytes(data)
+
     def to_bytes(self) -> bytes:
 
         buffer = b""
         for slot in self.slots:
             buffer += slot.to_bytes()
 
         buffer += self.hall_of_fame
```

### Comparing `pyemerald-0.4.0/pyemerald/section.py` & `pyemerald-0.5.0/pyemerald/section.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,17 @@
         pc.pokemon = pokemon
 
         return pc
 
     def add_pc_pokemon(self, pokemon: PCPokemon):
         self.pokemon.append(pokemon)
 
+    def insert_pc_pokemon(self, pokemon: PCPokemon, idx: int):
+        self.pokemon[idx] = pokemon
+
 
 # This mapping determines which RawSection's are converted
 # to BaseSection implementations
 SECTION_ID_TO_TYPE_MAPPING = {
     0: TrainerInfoSection,
     1: TeamItemSection,
     2: None,
```

### Comparing `pyemerald-0.4.0/pyemerald/utils.py` & `pyemerald-0.5.0/pyemerald/utils.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.4.0/pyproject.toml` & `pyemerald-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyemerald"
-version = "0.4.0"
+version = "0.5.0"
 description = "A package to modify save files from Pokemon Emerald"
 authors = ["matkvist <kvistanalytics@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/magnetos_son/pyemerald"
 
 [tool.poetry.dependencies]
```

### Comparing `pyemerald-0.4.0/setup.py` & `pyemerald-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pyemerald']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyemerald',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'A package to modify save files from Pokemon Emerald',
     'long_description': '# pyemerald\n\nPyemerald is a python package which lets you modify save files from Pokemon Emerald (Sapphire, Ruby, Leaf Green and Fire Red to come). It lets you modify Pokemon in your team and on the PC, and lets you modify items on the PC. It can also be used to inspect a Pokemons attributes like EV\'s (IV\'s to come).\n\nOther and more advanced projects exist e.g. [pkHex](https://projectpokemon.org/home/files/file/1-pkhex/) which inspired this project. However, it annoyed me that I was unable to run pkHex on Linux, and thus pyemerald was created.\n\nPlease make sure to never overwrite your original save file, as this software could accidentially make an invalid save file. You are responsible for using the software correctly.\n## Installation\n\nPyemerald can be installed from pypi with the following command:\n\n```\npip install pyemerald\n```\n\nIt has no dependencies so it should be a simple install.\n\n## Usage\n\nSeveral examples are available in the `examples` folder. But basically it works by loading an `.sav` file using a `Save` object, which can then emit a `Game` object that is modifiable. Once modification is done, the `Game` object is passed back to the `Save` object and saved to a new file (Please always save to a new file, so you don\'t accidentially delete your current save file!).\n\n```python\nfrom pyemerald.save import Save\nfrom pyemerald.pokemon import PCPokemon\nfrom pyemerald.moves import Move\n\nsave = Save.from_file("data/marie_treecko_pokedex_pc.sav")\n\ngame = save.to_game()\n\n# Simple create pokemon\nflygon = PCPokemon.from_name(\n    name="Flygon",\n    level=48,\n    move_1=Move.from_name("Thunder"),\n    move_2=Move.from_name("Thunder Punch"),\n    move_3=Move.from_name("Ice Beam"),\n    move_4=Move.from_name("Fly"),\n)\n\n# Add Pokemon to user PC\ngame.add_pc_pokemon(flygon)\n\n# Put modification back to the Save Object\nsave.update_from_game(game)\n\n# Write new Save file\nsave.to_file("data/emerald.sav")\n\n```\n',
     'author': 'matkvist',
     'author_email': 'kvistanalytics@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/magnetos_son/pyemerald',
```

### Comparing `pyemerald-0.4.0/PKG-INFO` & `pyemerald-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemerald
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package to modify save files from Pokemon Emerald
 Home-page: https://gitlab.com/magnetos_son/pyemerald
 License: MIT
 Author: matkvist
 Author-email: kvistanalytics@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

