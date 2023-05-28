# Comparing `tmp/pyemerald-0.5.0.tar.gz` & `tmp/pyemerald-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemerald-0.5.0.tar", max compression
+gzip compressed data, was "pyemerald-0.5.1.tar", max compression
```

## Comparing `pyemerald-0.5.0.tar` & `pyemerald-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.5.0/pyemerald/__init__.py
--rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/codec.py
--rw-r--r--   0        0        0      641 2023-05-23 13:28:34.597606 pyemerald-0.5.0/pyemerald/constants.py
--rw-r--r--   0        0        0     1798 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/game.py
--rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/items.py
--rw-r--r--   0        0        0     3045 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/level.py
--rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.5.0/pyemerald/moves.py
--rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.5.0/pyemerald/nature_stats.py
--rw-r--r--   0        0        0    36653 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/pokemon.py
--rw-r--r--   0        0        0    98431 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/pokemon_info.py
--rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.5.0/pyemerald/raw_section.py
--rw-r--r--   0        0        0     6425 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/save.py
--rw-r--r--   0        0        0     7257 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyemerald/section.py
--rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.5.0/pyemerald/utils.py
--rw-r--r--   0        0        0      531 2023-05-28 13:55:20.016336 pyemerald-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2568 2023-05-28 13:56:30.968651 pyemerald-0.5.0/setup.py
--rw-r--r--   0        0        0     2551 2023-05-28 13:56:30.969011 pyemerald-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.5.1/pyemerald/__init__.py
+-rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/codec.py
+-rw-r--r--   0        0        0      660 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyemerald/constants.py
+-rw-r--r--   0        0        0     1798 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/game.py
+-rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/items.py
+-rw-r--r--   0        0        0     3045 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/level.py
+-rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.5.1/pyemerald/moves.py
+-rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/nature_stats.py
+-rw-r--r--   0        0        0    36653 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/pokemon.py
+-rw-r--r--   0        0        0    98431 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/pokemon_info.py
+-rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.5.1/pyemerald/raw_section.py
+-rw-r--r--   0        0        0     6425 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/save.py
+-rw-r--r--   0        0        0     7141 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyemerald/section.py
+-rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.5.1/pyemerald/utils.py
+-rw-r--r--   0        0        0      531 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2568 2023-05-28 17:51:35.934300 pyemerald-0.5.1/setup.py
+-rw-r--r--   0        0        0     2551 2023-05-28 17:51:35.934617 pyemerald-0.5.1/PKG-INFO
```

### Comparing `pyemerald-0.5.0/LICENSE.txt` & `pyemerald-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/README.md` & `pyemerald-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/codec.py` & `pyemerald-0.5.1/pyemerald/codec.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/constants.py` & `pyemerald-0.5.1/pyemerald/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 BYTES_PER_PARTY_POKEMON = 100
 BYTES_PER_PC_POKEMON = 80
+BYTES_PER_ITEM = 4
 CHECKSUM_STEP_SIZE = 4
 HALL_OF_FAME_OFFSET = 114688
 HALL_OF_FAME_SIZE = 8192
 ITEM_SIZE = 4  # An item consists of 2x2bytes
 MYSTERY_GIFT_OFFSET = 122880
 MYSTERY_GIFT_SIZE = 4096
 N_SECTIONS = 14
```

### Comparing `pyemerald-0.5.0/pyemerald/game.py` & `pyemerald-0.5.1/pyemerald/game.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/items.py` & `pyemerald-0.5.1/pyemerald/items.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/level.py` & `pyemerald-0.5.1/pyemerald/level.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/moves.py` & `pyemerald-0.5.1/pyemerald/moves.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/nature_stats.py` & `pyemerald-0.5.1/pyemerald/nature_stats.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/pokemon.py` & `pyemerald-0.5.1/pyemerald/pokemon.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/pokemon_info.py` & `pyemerald-0.5.1/pyemerald/pokemon_info.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/raw_section.py` & `pyemerald-0.5.1/pyemerald/raw_section.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/save.py` & `pyemerald-0.5.1/pyemerald/save.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyemerald/section.py` & `pyemerald-0.5.1/pyemerald/section.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     Serializable,
     ByteDelta,
 )
 from pyemerald.raw_section import RawSection
 from pyemerald.constants import (
     BYTES_PER_PARTY_POKEMON,
     BYTES_PER_PC_POKEMON,
+    BYTES_PER_ITEM,
     RAW_SECTION_DATA_CONTENT_SIZE,
     PC_ITEM_COUNT,
     ITEM_SIZE,
 )
 from pyemerald.pokemon import Pokemon, PCPokemon
-from pyemerald.items import Item, ITEM_INDEX_TO_NAME
+from pyemerald.items import Item
 
 ######## Codecs ########
 class TrainerInfoCodec(Codec):
     def __init__(self, section_class: Type["Serializable"]):
         fields = [
             ByteFieldCodec("name", str, 0, 7),
             ByteFieldCodec("gender", int, 8, 1),
@@ -122,25 +123,27 @@
         # we need to create parse 6 * 100 bytes
         party = []
         for i in range(6):
             cur_pokemon_bytes = team.party[
                 BYTES_PER_PARTY_POKEMON * i : BYTES_PER_PARTY_POKEMON * (i + 1)
             ]
 
-            if cur_pokemon_bytes != TeamItemSection.null_pokemon:
+            if cur_pokemon_bytes != TeamItemSection.null_pokemon():
                 party.append(Pokemon.from_bytes(cur_pokemon_bytes))
 
         team.party = party
 
         # PC items
         pc_items = []
         for i in range(PC_ITEM_COUNT):
             cur_item_bytes = team.pc_items[ITEM_SIZE * i : ITEM_SIZE * (i + 1)]
-            item = Item.from_bytes(cur_item_bytes)
-            pc_items.append(item)
+            if cur_item_bytes != TeamItemSection.null_item():
+
+                item = Item.from_bytes(cur_item_bytes)
+                pc_items.append(item)
 
         team.pc_items = pc_items
 
         return team
 
     def to_bytes(self) -> bytes:
 
@@ -154,32 +157,28 @@
         for member in cur_obj.party:
             buffer += member.to_bytes()
         cur_obj.party = bytes(buffer)
 
         return super(TeamItemSection, cur_obj).to_bytes()
 
     def add_pc_item(self, item: Item):
-        cnt_act_items = 0
-        next_index = 0
-        for idx, cur_item in enumerate(self.pc_items):
-            if cur_item.name != ITEM_INDEX_TO_NAME[0]:
-                cnt_act_items += 1
-            else:
-                next_index = idx
-                break
 
-        if cnt_act_items >= PC_ITEM_COUNT:
-            raise ValueError("Cannot add more PC Items")
+        if len(self.pc_items) < PC_ITEM_COUNT:
+            self.pc_items.append(item)
         else:
-            self.pc_items[next_index] = item
+            raise ValueError("Cannot add more PC Items")
 
     @staticmethod
     def null_pokemon():
         return BYTES_PER_PARTY_POKEMON * b"\x00"
 
+    @staticmethod
+    def null_item():
+        return BYTES_PER_ITEM * b"\x00"
+
 
 @dataclass
 class PCBufferSection(BaseSection):
     pokemon: List[Pokemon]
 
 
 @dataclass
```

### Comparing `pyemerald-0.5.0/pyemerald/utils.py` & `pyemerald-0.5.1/pyemerald/utils.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.0/pyproject.toml` & `pyemerald-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyemerald"
-version = "0.5.0"
+version = "0.5.1"
 description = "A package to modify save files from Pokemon Emerald"
 authors = ["matkvist <kvistanalytics@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/magnetos_son/pyemerald"
 
 [tool.poetry.dependencies]
```

### Comparing `pyemerald-0.5.0/setup.py` & `pyemerald-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pyemerald']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyemerald',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A package to modify save files from Pokemon Emerald',
     'long_description': '# pyemerald\n\nPyemerald is a python package which lets you modify save files from Pokemon Emerald (Sapphire, Ruby, Leaf Green and Fire Red to come). It lets you modify Pokemon in your team and on the PC, and lets you modify items on the PC. It can also be used to inspect a Pokemons attributes like EV\'s (IV\'s to come).\n\nOther and more advanced projects exist e.g. [pkHex](https://projectpokemon.org/home/files/file/1-pkhex/) which inspired this project. However, it annoyed me that I was unable to run pkHex on Linux, and thus pyemerald was created.\n\nPlease make sure to never overwrite your original save file, as this software could accidentially make an invalid save file. You are responsible for using the software correctly.\n## Installation\n\nPyemerald can be installed from pypi with the following command:\n\n```\npip install pyemerald\n```\n\nIt has no dependencies so it should be a simple install.\n\n## Usage\n\nSeveral examples are available in the `examples` folder. But basically it works by loading an `.sav` file using a `Save` object, which can then emit a `Game` object that is modifiable. Once modification is done, the `Game` object is passed back to the `Save` object and saved to a new file (Please always save to a new file, so you don\'t accidentially delete your current save file!).\n\n```python\nfrom pyemerald.save import Save\nfrom pyemerald.pokemon import PCPokemon\nfrom pyemerald.moves import Move\n\nsave = Save.from_file("data/marie_treecko_pokedex_pc.sav")\n\ngame = save.to_game()\n\n# Simple create pokemon\nflygon = PCPokemon.from_name(\n    name="Flygon",\n    level=48,\n    move_1=Move.from_name("Thunder"),\n    move_2=Move.from_name("Thunder Punch"),\n    move_3=Move.from_name("Ice Beam"),\n    move_4=Move.from_name("Fly"),\n)\n\n# Add Pokemon to user PC\ngame.add_pc_pokemon(flygon)\n\n# Put modification back to the Save Object\nsave.update_from_game(game)\n\n# Write new Save file\nsave.to_file("data/emerald.sav")\n\n```\n',
     'author': 'matkvist',
     'author_email': 'kvistanalytics@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/magnetos_son/pyemerald',
```

### Comparing `pyemerald-0.5.0/PKG-INFO` & `pyemerald-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemerald
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package to modify save files from Pokemon Emerald
 Home-page: https://gitlab.com/magnetos_son/pyemerald
 License: MIT
 Author: matkvist
 Author-email: kvistanalytics@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

