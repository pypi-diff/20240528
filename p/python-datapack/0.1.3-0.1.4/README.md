# Comparing `tmp/python_datapack-0.1.3.tar.gz` & `tmp/python_datapack-0.1.4.tar.gz`

## Comparing `python_datapack-0.1.3.tar` & `python_datapack-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.3/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.3/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.3/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.3/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.3/copy_in_local.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14729 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.3/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.3/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.4/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.4/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.4/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.4/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.4/copy_in_local.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15350 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.4/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.4/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.4/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.4/PKG-INFO
```

### Comparing `python_datapack-0.1.3/src/python_datapack/__init__.py` & `python_datapack-0.1.4/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/constants.py` & `python_datapack-0.1.4/src/python_datapack/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 # Technical constants
 FACES: tuple = ("down", "up", "north", "south", "west", "east")						# Faces of a block, used for resource pack and blocks orientation
 SIDES: tuple = ("_bottom", "_top", "_front", "_back", "_left", "_right", "_side")	# Sides of a block, used for resource pack
 CUSTOM_BLOCK_VANILLA: str = "minecraft:furnace"			# Vanilla block used as base for custom blocks, must have the "facing" blockstate
 CUSTOM_BLOCK_ALTERNATIVE: str = "minecraft:item_frame"	# Same purpose as previous, but useful for blocks that can be placed on walls or on player's position (ex: flowers)
+CUSTOM_BLOCK_HEAD: str = "minecraft:player_head"		# Same purpose as previous, but useful for blocks does not have a custom model data
 CUSTOM_ITEM_VANILLA: str = "minecraft:command_block"	# Vanilla item used as base for custom items, must not have any survival vanilla behaviour
-MODEL_DISPLAY: dict = {"head":{"rotation":[0,0,0],"translation":[0,-30.42,0],"scale":[1.605,1.605,1.605]},"fixed":{"rotation":[-90,0,0],"translation":[0,0,-16],"scale":[2.0075,2.0075,2.0075]}}	# Model display base for custom blocks
 DOWNLOAD_VANILLA_ASSETS_RAW = "https://raw.githubusercontent.com/edayot/renders/renders/resourcepack/assets/minecraft/textures/render"
 DOWNLOAD_VANILLA_ASSETS_SOURCE = "https://github.com/edayot/renders/tree/renders/resourcepack/assets/minecraft/textures/render"
 
 
 # Databases
 RESULT_OF_CRAFTING: str = "result_of_crafting"			# Key to a list of recipes to craft the item, ex: "adamantium": {RESULT_OF_CRAFTING: [...]}
 USED_FOR_CRAFTING: str = "used_for_crafting"			# Should not be used unless you are crafting a vanilla item (ex: iyc.chainmail -> chainmail armor)
 CATEGORY: str = "category"								# Key for the category, used for recipes and the manual, ex: CATEGORY:"material" or CATEGORY:"equipment"
 COMMANDS_ON_PLACEMENT: str = "commands_on_placement"	# Key to a list of commands to execute when a custom block is placed, should be a list of strings or a single string (with break lines if multiple commands)
 COMMANDS_ON_BREAK: str = "commands_on_break"			# Key to a list of commands to execute when a custom block is broken, should be a list of strings or a single string (with break lines if multiple commands)
-VANILLA_BLOCK: str = "vanilla_block"					# Key to a vanilla block that will be placed for custom block interaction, value needs to be a dict with id and block_states given {"id":"minecraft:chest", "block_states": ["facing", "type=single", "waterlogged=false"]}
+VANILLA_BLOCK: str = "vanilla_block"					# Key to a vanilla block that will be placed for custom block interaction, value needs to be a dict like {"id":"minecraft:chest[type=single,waterlogged=false]", "apply_facing": True}
 NO_SILK_TOUCH_DROP: str = "no_silk_touch_drop"			# Key to an item ID that will drop when silk touch is not used. Must be used only when using the vanilla block for ores, ex: "adamantium_fragment" or "minecraft:raw_iron"
 OVERRIDE_MODEL: str = "override_model"					# Key to a dictionnary that will be used to override the whole model
-VANILLA_BLOCK_FOR_ORES: dict = {"id":"minecraft:polished_deepslate","block_states":[]}	# Vanilla block that will be used for an optimization tip for ores, don't ask questions
+VANILLA_BLOCK_FOR_ORES: dict = {"id":"minecraft:polished_deepslate", "apply_facing": False}	# Vanilla block that will be used for an optimization tip for ores, don't ask questions
 NOT_COMPONENTS: list[str] = [							# Keys that should not be considered as components. Used for recipes, loot tables, etc.
 	"id",
 	"wiki",
 	RESULT_OF_CRAFTING,
 	USED_FOR_CRAFTING,
 	CATEGORY,
 	COMMANDS_ON_PLACEMENT,
```

### Comparing `python_datapack-0.1.3/src/python_datapack/enhance_config.py` & `python_datapack-0.1.4/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/finalyze.py` & `python_datapack-0.1.4/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/initialize.py` & `python_datapack-0.1.4/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/verify_database.py` & `python_datapack-0.1.4/src/python_datapack/verify_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 				errors.append(f"'id' key should be a string for '{item}'")
 			elif data["id"] == "minecraft:deepslate":
 				errors.append(f"'id' key should not be 'minecraft:deepslate' for '{item}', it's a reserved ID")
 			
 			# Force VANILLA_BLOCK key for custom blocks
 			elif data["id"] in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE]:
 				if not data.get(VANILLA_BLOCK):
-					errors.append(f"VANILLA_BLOCK key missing for '{item}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
+					errors.append(f"VANILLA_BLOCK key missing for '{item}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"apply_facing\":False}}.")
 				elif not isinstance(data[VANILLA_BLOCK], dict):
-					errors.append(f"VANILLA_BLOCK key should be a dictionary for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
-				elif data[VANILLA_BLOCK].get("block_states", None) == None:
-					errors.append(f"VANILLA_BLOCK key should have a 'block_states' key for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
+					errors.append(f"VANILLA_BLOCK key should be a dictionary for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"apply_facing\":False}}.")
+				elif data[VANILLA_BLOCK].get("apply_facing", None) == None:
+					errors.append(f"VANILLA_BLOCK key should have a 'apply_facing' key to boolean for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"apply_facing\":False}}.")
 
 			# Prevent the use of "container" key for custom blocks
 			elif data["id"] == CUSTOM_BLOCK_VANILLA and data.get("container"):
 				errors.append(f"'container' key should not be used for '{item}', it's a reserved key for custom blocks, prefer using COMMANDS_ON_PLACEMENT key to fill in the container")
 
 		# If a category is present but wrong format, log an error
 		if data.get(CATEGORY) and not isinstance(data[CATEGORY], str):
@@ -142,26 +142,26 @@
 
 						# Check the result count
 						if not recipe.get("result_count") or not isinstance(recipe["result_count"], int):
 							errors.append(f"Recipe #{i} in RESULT_OF_CRAFTING should have an int 'result_count' key for '{item}'")
 
 		# Commands on custom block placement
 		if data.get(COMMANDS_ON_PLACEMENT) and data.get("id"):
-			if data["id"] not in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE]:
+			if data["id"] not in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE, CUSTOM_BLOCK_HEAD]:
 				errors.append(f"COMMANDS_ON_PLACEMENT key should only be used for custom blocks for '{item}'")
 			elif not isinstance(data[COMMANDS_ON_PLACEMENT], (list, str)):
 				errors.append(f"COMMANDS_ON_PLACEMENT key should be a list of string or a string for '{item}'")
 			elif isinstance(data[COMMANDS_ON_PLACEMENT], list):
 				for i, command in enumerate(data[COMMANDS_ON_PLACEMENT]):
 					if not isinstance(command, str):
 						errors.append(f"Command #{i} in COMMANDS_ON_PLACEMENT should be a string for '{item}'")
 		
 		# Commands on custom block break
 		if data.get(COMMANDS_ON_BREAK) and data.get("id"):
-			if data["id"] not in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE]:
+			if data["id"] not in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE, CUSTOM_BLOCK_HEAD]:
 				errors.append(f"COMMANDS_ON_BREAK key should only be used for custom blocks for '{item}'")
 			elif not isinstance(data[COMMANDS_ON_BREAK], (list, str)):
 				errors.append(f"COMMANDS_ON_BREAK key should be a list of string or a string for '{item}'")
 			elif isinstance(data[COMMANDS_ON_BREAK], list):
 				for i, command in enumerate(data[COMMANDS_ON_BREAK]):
 					if not isinstance(command, str):
 						errors.append(f"Command #{i} in COMMANDS_ON_BREAK should be a string for '{item}'")
```

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.4/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.4/src/python_datapack/datapack/custom_blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,88 +2,103 @@
 # Imports
 from ..utils.io import *
 from ..utils.print import *
 from ..constants import *
 
 def main(config: dict):
 
+	# Predicates
+	FACING = ["north", "east", "south", "west"]
+	for face in FACING:
+		predicate = {"condition":"minecraft:location_check","predicate":{"block":{"state":{"facing":face}}}}
+		write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/predicate/facing/{face}.json", super_json_dump(predicate))
+
+	# Get rotation function
+	write_to_file(f"{config['datapack_functions']}/custom_blocks/get_rotation.mcfunction", f"""
+# Set up score
+scoreboard players set #rotation {config['namespace']}.data 0
+
+# Player case
+execute if score #rotation {config['namespace']}.data matches 0 if entity @s[y_rotation=-46..45] run scoreboard players set #rotation {config['namespace']}.data 1
+execute if score #rotation {config['namespace']}.data matches 0 if entity @s[y_rotation=45..135] run scoreboard players set #rotation {config['namespace']}.data 2
+execute if score #rotation {config['namespace']}.data matches 0 if entity @s[y_rotation=135..225] run scoreboard players set #rotation {config['namespace']}.data 3
+execute if score #rotation {config['namespace']}.data matches 0 if entity @s[y_rotation=225..315] run scoreboard players set #rotation {config['namespace']}.data 4
+
+# Predicate case
+execute if score #rotation {config['namespace']}.data matches 0 if predicate {config['namespace']}:facing/north run scoreboard players set #rotation {config['namespace']}.data 1
+execute if score #rotation {config['namespace']}.data matches 0 if predicate {config['namespace']}:facing/east run scoreboard players set #rotation {config['namespace']}.data 2
+execute if score #rotation {config['namespace']}.data matches 0 if predicate {config['namespace']}:facing/south run scoreboard players set #rotation {config['namespace']}.data 3
+execute if score #rotation {config['namespace']}.data matches 0 if predicate {config['namespace']}:facing/west run scoreboard players set #rotation {config['namespace']}.data 4
+# No more cases for now
+
+""")
+	APPLY_FACING = f"""
+# Apply rotation
+execute if score #rotation {config['namespace']}.data matches 1 run data modify entity @s Rotation[0] set value 180.0f
+execute if score #rotation {config['namespace']}.data matches 2 run data modify entity @s Rotation[0] set value 270.0f
+execute if score #rotation {config['namespace']}.data matches 3 run data modify entity @s Rotation[0] set value 0.0f
+execute if score #rotation {config['namespace']}.data matches 4 run data modify entity @s Rotation[0] set value 90.0f
+"""
+
 	# For each custom block
 	unique_blocks = set()
 	for item, data in config['database'].items():
 
 		# Custom block
 		if data.get(VANILLA_BLOCK):
 			block = data[VANILLA_BLOCK]
 			path = f"{config['datapack_functions']}/custom_blocks/{item}"
 
 			## Place function	
-			# Place block
-			if isinstance(block, str):
-				content = f"setblock ~ ~ ~ {block}\n"
+			content = ""
+			block_id = block["id"]
+			if block["apply_facing"]:
+				content += f"function {config['namespace']}:custom_blocks/get_rotation\n"
+				block_states = []
+				if '[' in block_id:
+					block_states = block_id.split('[')[1][:-1].split(',')
+					block_id = block_id.split('[')[0]
+				for face in ["north", "east", "south", "west"]:
+					content += f"execute if predicate {config['namespace']}:facing/{face} run setblock ~ ~ ~ {block_id}[facing={face}," + ",".join(block_states) + "]\n"
 			else:
-
-				# Handle block states
-				content = ""
-				states = block.get("block_states", [])
-				block = block["id"]
-				if "facing" in states:
-					other_states = [state for state in states if state != "facing"]
-
-					# For each face, make a different setblock depending on the vanilla block facing
-					for face in FACES[2:]:
-						content += f"execute if block ~ ~ ~ {CUSTOM_BLOCK_VANILLA}[facing={face}] run setblock ~ ~ ~ {block}[facing={face}"
-
-						# Add the other states to the block
-						for state in other_states:
-							content += f",{state}"
-						content += "]\n"
-				else:
-					# Simple setblock with all block states
-					content += f"setblock ~ ~ ~ {block}[" + ",".join(states) + "]\n"
+				# Simple setblock
+				content += f"setblock ~ ~ ~ {block_id}\n"
 			
 			# Summon item display and call secondary function
 			content += f"execute align xyz positioned ~.5 ~.5 ~.5 summon item_display at @s run function {config['namespace']}:custom_blocks/{item}/place_secondary\n"
+
+			# Add temporary tags and call main function
+			content = f"tag @s add {config['namespace']}.placer\n" + content + f"tag @s remove {config['namespace']}.placer\n"
 			write_to_file(f"{path}/place_main.mcfunction", content)
 
 			## Secondary function
-			unique_blocks.add(block)
-			block = block.replace(":","_")
+			block_id = block_id.split('[')[0].split('{')[0]
+			unique_blocks.add(block_id)
+			block_id = block_id.replace(":","_")
 			set_custom_model_data = ""
 			if data.get("custom_model_data"):
 				set_custom_model_data = f"item replace entity @s container.0 with {CUSTOM_BLOCK_VANILLA}[minecraft:custom_model_data={data['custom_model_data']}]\n"
 			content = f"""
 # Add convention and utils tags, and the custom block tag
 tag @s add global.ignore
 tag @s add global.ignore.kill
 tag @s add smithed.entity
 tag @s add smithed.block
 tag @s add {config['namespace']}.custom_block
 tag @s add {config['namespace']}.{item}
-tag @s add {config['namespace']}.vanilla.{block}
+tag @s add {config['namespace']}.vanilla.{block_id}
 
 # Modify item display entity to match the custom block
 {set_custom_model_data}data modify entity @s transformation.scale set value [1.002f,1.008f,1.002f]
 data modify entity @s transformation.translation[1] set value 0.003f
 data modify entity @s brightness set value {{block:15,sky:15}}
-
-## Check if the block have rotation
-# Furnace case
-scoreboard players set #rotation {config['namespace']}.data 0
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=north] run data modify entity @s Rotation[0] set value 180.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=east] run data modify entity @s Rotation[0] set value 270.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=south] run data modify entity @s Rotation[0] set value 0.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=west] run data modify entity @s Rotation[0] set value 90.0f
-# Iron trapdoor case
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=north] run data modify entity @s Rotation[0] set value 180.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=east] run data modify entity @s Rotation[0] set value 270.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=south] run data modify entity @s Rotation[0] set value 0.0f
-execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=west] run data modify entity @s Rotation[0] set value 90.0f
-# No more cases for now
-
 """
+			if block["apply_facing"]:
+				content += APPLY_FACING
+
 			# Add the commands on placement if any
 			if COMMANDS_ON_PLACEMENT in data:
 				if isinstance(data[COMMANDS_ON_PLACEMENT], list):
 					content += "\n".join(data[COMMANDS_ON_PLACEMENT]) + "\n"
 				else:
 					content += f"{data[COMMANDS_ON_PLACEMENT]}\n"
 				
@@ -103,51 +118,48 @@
 
 	# Sort unique blocks
 	unique_blocks = sorted(list(unique_blocks))
 
 	## Destroy functions
 	# For each unique block, if the vanilla block is missing, call the destroy function for the group
 	content = "\n"
-	for block in unique_blocks:
-		block_underscore = block.replace(":","_")
-		content += f"execute if entity @s[tag={config['namespace']}.vanilla.{block_underscore}] unless block ~ ~ ~ {block} run function {config['namespace']}:custom_blocks/_groups/{block_underscore}\n"
+	for block_id in unique_blocks:
+		block_underscore = block_id.replace(":","_")
+		content += f"execute if entity @s[tag={config['namespace']}.vanilla.{block_underscore}] unless block ~ ~ ~ {block_id} run function {config['namespace']}:custom_blocks/_groups/{block_underscore}\n"
 	write_to_file(f"{config['datapack_functions']}/custom_blocks/destroy.mcfunction", content + "\n")
 
 	# For each unique block, make the group function
-	for block in unique_blocks:
-		block_underscore = block.replace(":","_")
+	for block_id in unique_blocks:
+		block_underscore = block_id.replace(":","_")
 		content = "\n"
 
 		# For every custom block, add a tag check for destroy if it's the right vanilla block
 		for item, data in config['database'].items():
 			if data.get(VANILLA_BLOCK):
 
 				# Get the vanilla block
-				this_block = data[VANILLA_BLOCK]
-				if isinstance(this_block, dict):
-					this_block = this_block["id"]
+				this_block = data[VANILLA_BLOCK]["id"].split('[')[0].split('{')[0]
 				this_block = this_block.replace(":","_")
 
 				# Add the line if it's the same vanilla block
 				if this_block == block_underscore:
 					content += f"execute if entity @s[tag={config['namespace']}.{item}] run function {config['namespace']}:custom_blocks/{item}/destroy\n"
 		write_to_file(f"{config['datapack_functions']}/custom_blocks/_groups/{block_underscore}.mcfunction", content + "\n")
 
 	# For each custom block, make it's destroy function
 	for item, data in config['database'].items():
 		if data.get(VANILLA_BLOCK):
 			block = data[VANILLA_BLOCK]
 			path = f"{config['datapack_functions']}/custom_blocks/{item}"
-			if isinstance(block, dict):
-				block = block["id"]
+			block_id = block["id"].split('[')[0].split('{')[0]
 			
 			# Destroy function
 			content = f"""
 # Replace the item with the custom one
-execute as @e[type=item,nbt={{Item:{{id:"{block}"}}}},limit=1,sort=nearest,distance=..1] run function {config['namespace']}:custom_blocks/{item}/replace_item
+execute as @e[type=item,nbt={{Item:{{id:"{block_id}"}}}},limit=1,sort=nearest,distance=..1] run function {config['namespace']}:custom_blocks/{item}/replace_item
 """
 			# Add the commands on break if any
 			if COMMANDS_ON_BREAK in data:
 				if isinstance(data[COMMANDS_ON_BREAK], list):
 					content += "\n".join(data[COMMANDS_ON_BREAK]) + "\n"
 				else:
 					content += f"{data[COMMANDS_ON_BREAK]}\n"
```

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.4/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.4/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.4/src/python_datapack/datapack/loading.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,16 @@
 	for item, data in config['database'].items():
 		mc_data = {"id":"","count":1, "components":{"custom_model_data":-1}}
 		for k, v in data.items():
 			if k not in NOT_COMPONENTS:
 				mc_data["components"][k] = v
 			elif k == "id":
 				mc_data[k] = v
+		if mc_data["components"]["custom_model_data"] == -1:
+			del mc_data["components"]["custom_model_data"]
 		items_storage += f"data modify storage {config['namespace']}:items all.{item} set value " + super_json_dump(mc_data, max_level = 0)
 		pass
 
 	write_to_file(f"{config['datapack_functions']}/load/confirm_load.mcfunction", f"""
 tellraw @a[tag=convention.debug] {{"text":"[Loaded {config['datapack_name']} v{config['version']}]","color":"green"}}
 
 scoreboard objectives add {config['namespace']}.private dummy
```

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.4/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/main.py` & `python_datapack-0.1.4/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.4/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.4/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/main.py` & `python_datapack-0.1.4/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.4/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/utils.py` & `python_datapack-0.1.4/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.4/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.4/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.4/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.4/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/resource_pack/main.py` & `python_datapack-0.1.4/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.4/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.4/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from ..constants import *
 
 def main(config: dict):
 
 	# Get every vanilla IDs
 	vanilla_ids = set()
 	for v in config['database'].values():
-		vanilla_ids.add(v.get("id", "").replace("minecraft:", ""))
+		if v.get("custom_model_data"):
+			vanilla_ids.add(v.get("id", "").replace("minecraft:", ""))
 
 	# For each vanilla ID, create the json model file
 	blocks = [CUSTOM_BLOCK_VANILLA, CUSTOM_ITEM_VANILLA]
 	blocks = [x.replace("minecraft:", "") for x in blocks]
 	for id in vanilla_ids:
 		block_or_item = "block" if id in blocks else "item"
 		if id == CUSTOM_ITEM_VANILLA.replace("minecraft:", ""):
```

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.4/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.4/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/io.py` & `python_datapack-0.1.4/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.4/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/print.py` & `python_datapack-0.1.4/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/src/python_datapack/utils/weld.py` & `python_datapack-0.1.4/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/LICENSE` & `python_datapack-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.3/pyproject.toml` & `python_datapack-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.3/PKG-INFO` & `python_datapack-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

