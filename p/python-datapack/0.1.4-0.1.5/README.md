# Comparing `tmp/python_datapack-0.1.4.tar.gz` & `tmp/python_datapack-0.1.5.tar.gz`

## Comparing `python_datapack-0.1.4.tar` & `python_datapack-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.4/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.4/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.4/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.4/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.4/copy_in_local.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15350 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.4/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.4/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.5/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.5/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.5/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.5/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.5/copy_in_local.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.5/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.5/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.5/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.5/PKG-INFO
```

### Comparing `python_datapack-0.1.4/src/python_datapack/__init__.py` & `python_datapack-0.1.5/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/constants.py` & `python_datapack-0.1.5/src/python_datapack/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SIDES: tuple = ("_bottom", "_top", "_front", "_back", "_left", "_right", "_side")	# Sides of a block, used for resource pack
 CUSTOM_BLOCK_VANILLA: str = "minecraft:furnace"			# Vanilla block used as base for custom blocks, must have the "facing" blockstate
 CUSTOM_BLOCK_ALTERNATIVE: str = "minecraft:item_frame"	# Same purpose as previous, but useful for blocks that can be placed on walls or on player's position (ex: flowers)
 CUSTOM_BLOCK_HEAD: str = "minecraft:player_head"		# Same purpose as previous, but useful for blocks does not have a custom model data
 CUSTOM_ITEM_VANILLA: str = "minecraft:command_block"	# Vanilla item used as base for custom items, must not have any survival vanilla behaviour
 DOWNLOAD_VANILLA_ASSETS_RAW = "https://raw.githubusercontent.com/edayot/renders/renders/resourcepack/assets/minecraft/textures/render"
 DOWNLOAD_VANILLA_ASSETS_SOURCE = "https://github.com/edayot/renders/tree/renders/resourcepack/assets/minecraft/textures/render"
-
+CUSTOM_BLOCK_HEAD_CUBE_RADIUS: tuple[int, int, int] = (16, 16, 16)	# Size of the region to check around the player when placing a CUSTOM_BLOCK_HEAD
 
 # Databases
 RESULT_OF_CRAFTING: str = "result_of_crafting"			# Key to a list of recipes to craft the item, ex: "adamantium": {RESULT_OF_CRAFTING: [...]}
 USED_FOR_CRAFTING: str = "used_for_crafting"			# Should not be used unless you are crafting a vanilla item (ex: iyc.chainmail -> chainmail armor)
 CATEGORY: str = "category"								# Key for the category, used for recipes and the manual, ex: CATEGORY:"material" or CATEGORY:"equipment"
 COMMANDS_ON_PLACEMENT: str = "commands_on_placement"	# Key to a list of commands to execute when a custom block is placed, should be a list of strings or a single string (with break lines if multiple commands)
 COMMANDS_ON_BREAK: str = "commands_on_break"			# Key to a list of commands to execute when a custom block is broken, should be a list of strings or a single string (with break lines if multiple commands)
```

### Comparing `python_datapack-0.1.4/src/python_datapack/enhance_config.py` & `python_datapack-0.1.5/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/finalyze.py` & `python_datapack-0.1.5/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/initialize.py` & `python_datapack-0.1.5/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/verify_database.py` & `python_datapack-0.1.5/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.5/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.5/src/python_datapack/datapack/custom_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,31 +167,14 @@
 
 			# Replace item function
 			if block != VANILLA_BLOCK_FOR_ORES:
 				content = f"""
 data modify entity @s Item.components set from storage {config['namespace']}:items all.{item}.components
 data modify entity @s Item.id set from storage {config['namespace']}:items all.{item}.id
 """
-				"""
-# Replace the item by the ore if the player is holding a silk touch pickaxe
-execute if score #is_silk_touch simplenergy.data matches 1 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.deepslate_simplunium_ore
-
-# Replace the item by the raw form if the player is not holding a silk touch pickaxe
-execute if score #is_silk_touch simplenergy.data matches 0 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.raw_simplunium
-execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data = #item_count simplenergy.data
-execute if score #is_silk_touch simplenergy.data matches 0 store result score #temp simplenergy.data run data get entity @s UUID[1]
-execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #temp simplenergy.data %= #4 simplenergy.data
-execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players add #temp simplenergy.data 1
-execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data *= #temp simplenergy.data
-execute if score #is_silk_touch simplenergy.data matches 0 store result entity @e[type=item,nbt={Age:0s,Item:{tag:{simplenergy:{raw_simplunium:1b}}}},limit=1,sort=nearest,distance=..1] Item.Count byte 1 run scoreboard players get #count simplenergy.data
-
-# Remove the block
-kill @s
-
-"""
 			else:
 				no_silk_touch_drop = data[NO_SILK_TOUCH_DROP]
 				if ':' in no_silk_touch_drop:
 					silk_text = f'execute if score #is_silk_touch {config["namespace"]}.data matches 0 run data modify entity @s Item.id set value "{no_silk_touch_drop}"'
 				else:
 					silk_text = f"execute if score #is_silk_touch {config['namespace']}.data matches 0 run data modify entity @s Item.id set from storage {config['namespace']}:items all.{no_silk_touch_drop}.id"
 					silk_text += f"\nexecute if score #is_silk_touch {config['namespace']}.data matches 0 run data modify entity @s Item.components set from storage {config['namespace']}:items all.{no_silk_touch_drop}.components"
@@ -250,10 +233,32 @@
 scoreboard players set #is_silk_touch {config['namespace']}.data 0
 execute store result score #item_count {config['namespace']}.data run data get entity @s Item.count
 execute store success score #is_silk_touch {config['namespace']}.data if data entity @s Item.components."minecraft:custom_data".common_signals.silk_touch
 
 # Try to destroy the block
 execute as @e[tag={config['namespace']}.custom_block,dx=0,dy=0,dz=0] at @s run function {config['namespace']}:custom_blocks/destroy
 """)
+	
+
+
+	## Custom blocks using player_head
+	for item, data in config['database'].items():
+		if data["id"] == CUSTOM_BLOCK_HEAD and data.get(VANILLA_BLOCK):
+
+			# Make advancement
+			predicate = {"criteria":{"requirement":{"trigger":"minecraft:placed_block","conditions":{"location": [{"condition": "minecraft:location_check","predicate": {"block": {}}}]}}},"requirements":[["requirement"]],"rewards":{}}
+			predicate["criteria"]["requirement"]["conditions"]["location"][0]["predicate"]["block"]["nbt"] = json.dumps({"components":{"minecraft:custom_data":data.get("custom_data", {})}})
+			predicate["rewards"]["function"] = f"{config['namespace']}:custom_blocks/_player_head/search_{item}"
+			write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/advancement/custom_block_head/{item}.json", super_json_dump(predicate, max_level = -1))
+
+			# Make search function
+			content = "# Search where the head has been placed\n"
+			mid_x, mid_y, mid_z = [x // 2 for x in CUSTOM_BLOCK_HEAD_CUBE_RADIUS]
+			for x in range(-mid_x, mid_x + 1):
+				for y in range(-mid_y, mid_y + 1):
+					for z in range(-mid_z, mid_z + 1):
+						content += f"execute positioned ~{x} ~{y} ~{z} if data block ~ ~ ~ components.\"minecraft:custom_data\".{config['namespace']}.{item} run function {config['namespace']}:custom_blocks/{item}/place_main\n"
+			content += f"\n# Advancement\nadvancement revoke @s only {config['namespace']}:custom_block_head/{item}\n\n"
+			write_to_file(f"{config['datapack_functions']}/custom_blocks/_player_head/search_{item}.mcfunction", content)
 
 	info("All customs blocks are now placeable and destroyable!")
```

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.5/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.5/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.5/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.5/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/main.py` & `python_datapack-0.1.5/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.5/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.5/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/main.py` & `python_datapack-0.1.5/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.5/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/utils.py` & `python_datapack-0.1.5/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.5/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.5/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.5/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.5/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/resource_pack/main.py` & `python_datapack-0.1.5/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.5/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.5/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.5/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.5/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/io.py` & `python_datapack-0.1.5/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.5/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/print.py` & `python_datapack-0.1.5/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/src/python_datapack/utils/weld.py` & `python_datapack-0.1.5/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/LICENSE` & `python_datapack-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.4/pyproject.toml` & `python_datapack-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.4/PKG-INFO` & `python_datapack-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

