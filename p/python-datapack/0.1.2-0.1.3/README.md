# Comparing `tmp/python_datapack-0.1.2.tar.gz` & `tmp/python_datapack-0.1.3.tar.gz`

## Comparing `python_datapack-0.1.2.tar` & `python_datapack-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.2/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.2/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.2/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.2/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.2/copy_in_local.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14732 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.2/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.2/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.2/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.3/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.3/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.3/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.3/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.3/copy_in_local.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14729 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.3/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.3/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.3/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.3/PKG-INFO
```

### Comparing `python_datapack-0.1.2/src/python_datapack/__init__.py` & `python_datapack-0.1.3/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/constants.py` & `python_datapack-0.1.3/src/python_datapack/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 # Databases
 RESULT_OF_CRAFTING: str = "result_of_crafting"			# Key to a list of recipes to craft the item, ex: "adamantium": {RESULT_OF_CRAFTING: [...]}
 USED_FOR_CRAFTING: str = "used_for_crafting"			# Should not be used unless you are crafting a vanilla item (ex: iyc.chainmail -> chainmail armor)
 CATEGORY: str = "category"								# Key for the category, used for recipes and the manual, ex: CATEGORY:"material" or CATEGORY:"equipment"
 COMMANDS_ON_PLACEMENT: str = "commands_on_placement"	# Key to a list of commands to execute when a custom block is placed, should be a list of strings or a single string (with break lines if multiple commands)
 COMMANDS_ON_BREAK: str = "commands_on_break"			# Key to a list of commands to execute when a custom block is broken, should be a list of strings or a single string (with break lines if multiple commands)
-VANILLA_BLOCK: str = "vanilla_block"					# Key to a vanilla block that will be placed for custom block interaction, value can either a string of a dict {"id":"minecraft:chest", "block_states": ["facing", "type=single", "waterlogged=false"]}
-VANILLA_BLOCK_FOR_ORES: str = "minecraft:polished_deepslate"	# Vanilla block that will be used for an optimization tip for ores, don't ask questions
+VANILLA_BLOCK: str = "vanilla_block"					# Key to a vanilla block that will be placed for custom block interaction, value needs to be a dict with id and block_states given {"id":"minecraft:chest", "block_states": ["facing", "type=single", "waterlogged=false"]}
 NO_SILK_TOUCH_DROP: str = "no_silk_touch_drop"			# Key to an item ID that will drop when silk touch is not used. Must be used only when using the vanilla block for ores, ex: "adamantium_fragment" or "minecraft:raw_iron"
 OVERRIDE_MODEL: str = "override_model"					# Key to a dictionnary that will be used to override the whole model
+VANILLA_BLOCK_FOR_ORES: dict = {"id":"minecraft:polished_deepslate","block_states":[]}	# Vanilla block that will be used for an optimization tip for ores, don't ask questions
 NOT_COMPONENTS: list[str] = [							# Keys that should not be considered as components. Used for recipes, loot tables, etc.
 	"id",
 	"wiki",
 	RESULT_OF_CRAFTING,
 	USED_FOR_CRAFTING,
 	CATEGORY,
 	COMMANDS_ON_PLACEMENT,
```

### Comparing `python_datapack-0.1.2/src/python_datapack/enhance_config.py` & `python_datapack-0.1.3/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/finalyze.py` & `python_datapack-0.1.3/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/initialize.py` & `python_datapack-0.1.3/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/verify_database.py` & `python_datapack-0.1.3/src/python_datapack/verify_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,21 @@
 		else:
 			if not isinstance(data["id"], str):
 				errors.append(f"'id' key should be a string for '{item}'")
 			elif data["id"] == "minecraft:deepslate":
 				errors.append(f"'id' key should not be 'minecraft:deepslate' for '{item}', it's a reserved ID")
 			
 			# Force VANILLA_BLOCK key for custom blocks
-			elif data["id"] in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE] and not data.get(VANILLA_BLOCK):
-				errors.append(f"VANILLA_BLOCK key missing for '{item}', needed format: VANILLA_BLOCK: \"minecraft:stone\"")
+			elif data["id"] in [CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE]:
+				if not data.get(VANILLA_BLOCK):
+					errors.append(f"VANILLA_BLOCK key missing for '{item}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
+				elif not isinstance(data[VANILLA_BLOCK], dict):
+					errors.append(f"VANILLA_BLOCK key should be a dictionary for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
+				elif data[VANILLA_BLOCK].get("block_states", None) == None:
+					errors.append(f"VANILLA_BLOCK key should have a 'block_states' key for '{item}', found '{data[VANILLA_BLOCK]}', needed format: VANILLA_BLOCK: {{\"id\":\"minecraft:stone\", \"block_states\":[]}},\n add 'facing' to the block_states list if you want to use block rotation.")
 
 			# Prevent the use of "container" key for custom blocks
 			elif data["id"] == CUSTOM_BLOCK_VANILLA and data.get("container"):
 				errors.append(f"'container' key should not be used for '{item}', it's a reserved key for custom blocks, prefer using COMMANDS_ON_PLACEMENT key to fill in the container")
 
 		# If a category is present but wrong format, log an error
 		if data.get(CATEGORY) and not isinstance(data[CATEGORY], str):
```

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.3/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.3/src/python_datapack/datapack/custom_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 			# Place block
 			if isinstance(block, str):
 				content = f"setblock ~ ~ ~ {block}\n"
 			else:
 
 				# Handle block states
 				content = ""
-				states = block.get("block_states")
-				states = [] if not states else states
+				states = block.get("block_states", [])
 				block = block["id"]
 				if "facing" in states:
 					other_states = [state for state in states if state != "facing"]
 
 					# For each face, make a different setblock depending on the vanilla block facing
 					for face in FACES[2:]:
 						content += f"execute if block ~ ~ ~ {CUSTOM_BLOCK_VANILLA}[facing={face}] run setblock ~ ~ ~ {block}[facing={face}"
@@ -46,15 +45,15 @@
 			write_to_file(f"{path}/place_main.mcfunction", content)
 
 			## Secondary function
 			unique_blocks.add(block)
 			block = block.replace(":","_")
 			set_custom_model_data = ""
 			if data.get("custom_model_data"):
-				set_custom_model_data = f"item replace entity @s container.0 with deepslate[minecraft:custom_model_data={data['custom_model_data']}]\n"
+				set_custom_model_data = f"item replace entity @s container.0 with {CUSTOM_BLOCK_VANILLA}[minecraft:custom_model_data={data['custom_model_data']}]\n"
 			content = f"""
 # Add convention and utils tags, and the custom block tag
 tag @s add global.ignore
 tag @s add global.ignore.kill
 tag @s add smithed.entity
 tag @s add smithed.block
 tag @s add {config['namespace']}.custom_block
@@ -207,21 +206,22 @@
 	for block in unique_blocks:
 		block_underscore = block.replace(":","_")
 		predicate = {"condition": "minecraft:entity_properties", "entity": "this", "predicate": { "nbt": f"{{Tags:[\"iyc.vanilla.{block_underscore}\"]}}", "location": { "block": { "blocks": [block] }}}}
 		advanced_predicate["terms"].append(predicate)
 	write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/predicate/advanced_check_vanilla_blocks.json", super_json_dump(advanced_predicate))
 
 	# Write a destroy check every 2 ticks, every second, and every 5 seconds
+	ore_vanilla_block = VANILLA_BLOCK_FOR_ORES["id"].replace(':', '_')
 	write_to_file(f"{config['datapack_functions']}/tick_2.mcfunction", f"""
 # 2 ticks destroy detection
-execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
+execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{ore_vanilla_block},predicate=!{config['namespace']}:check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
 """)
 	write_to_file(f"{config['datapack_functions']}/second.mcfunction", f"""
 # 1 second break detection
-execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
+execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{ore_vanilla_block},predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
 """)
 	write_to_file(f"{config['datapack_functions']}/second_5.mcfunction", f"""
 # 5 seconds break detection
 execute as @e[type=item_display,tag={config['namespace']}.custom_block,predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
 """)
```

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.3/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.3/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.3/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.3/src/python_datapack/datapack/loot_tables.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 		write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/loot_table/i/{config['namespace']}_manual.json", super_json_dump(loot_table, max_level = -1), overwrite = True)
 
 	# Make a give all command that gives chests with all the items
 	CHEST_SIZE = 27
 	total_chests = (len(config['database']) + CHEST_SIZE - 1) // CHEST_SIZE
 	lore = json.dumps(config['source_lore']).replace('"', "'")
 	chests = []
-	database_copy = config['database'].copy()
+	database_copy = list(config['database'].items())
 	for i in range(total_chests):
 		chest_contents = []
 	
 		# For each slot of the chest, append an item and remove it from the copy
 		for j in range(CHEST_SIZE):
 			if not database_copy:
 				break
-			item, data = database_copy.popitem()
+			item, data = database_copy.pop(0)
 			data = data.copy()
 			id = data.get("id")
 			for k in NOT_COMPONENTS:	# Remove non-component data
 				if data.get(k):
 					del data[k]
 			json_content = super_json_dump(data, max_level = 0).replace("\n","")
 			chest_contents.append(f'{{slot:{j},item:{{count:1,id:"{id}",components:{json_content}}}}}')
```

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/main.py` & `python_datapack-0.1.3/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.3/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.3/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/main.py` & `python_datapack-0.1.3/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.3/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/utils.py` & `python_datapack-0.1.3/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.3/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.3/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.3/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.3/src/python_datapack/resource_pack/item_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,19 +115,14 @@
 				source = f"{config['textures_folder']}/{texture_path}.png"
 				destination = f"{dest_base_textu}/{texture_path}.png"
 				super_copy(source, destination)
 			
 		# Write content
 		write_to_file(f"{dest_base_model}/{item}{on_off}.json", super_json_dump(content, max_level = 4))
 
-		# Generate placed models for item_display if it's a block
-		if block_or_item == "block":
-			dest_base_model = f"{config['build_resource_pack']}/assets/{config['namespace']}/models/{block_or_item}/for_item_display"
-			content["display"] = MODEL_DISPLAY
-			write_to_file(f"{dest_base_model}/{item}{on_off}.json", super_json_dump(content, max_level = 4))
 
 
 def main(config: dict):
 
 	# For each item,
 	used_textures = set()
 	for item, data in config['database'].items():
```

### Comparing `python_datapack-0.1.2/src/python_datapack/resource_pack/main.py` & `python_datapack-0.1.3/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.3/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.3/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,23 +41,17 @@
 		content["overrides"].sort(key=lambda x: x["predicate"]["custom_model_data"])
 		write_to_file(
 			f"{config['build_resource_pack']}/assets/minecraft/models/item/{id}.json",
 			super_json_dump(content).replace('{"','{ "').replace('"}','" }').replace(',"', ', "')
 		)
 
 
-	# Generate deepslate models
-	content = {"parent": "block/deepslate"}
-	content["overrides"] = []
-	for item, data in config['database'].items():
-		if data.get("id") in (CUSTOM_BLOCK_VANILLA, CUSTOM_BLOCK_ALTERNATIVE) and data.get("custom_model_data"):
-			content["overrides"].append({"predicate": { "custom_model_data": data["custom_model_data"]}, "model": f"{config['namespace']}:block/for_item_display/{item}" })
-	content["overrides"].append({"predicate": { "custom_model_data": 2010000}, "model": f"minecraft:item/none"})
-	content["overrides"].sort(key=lambda x: x["predicate"]["custom_model_data"])
+	# Generate Common Signals item model
+	content = super_json_dump({"parent": "block/deepslate", "overrides": [{"predicate": { "custom_model_data": 2010000}, "model": f"minecraft:item/none"}]})
 	write_to_file(
 		f"{config['build_resource_pack']}/assets/minecraft/models/item/deepslate.json",
-		super_json_dump(content).replace('{"','{ "').replace('"}','" }').replace(',"', ', "')
-	)
+		content.replace('{"','{ "').replace('"}','" }').replace(',"', ', "')
+	)	
 	write_to_file(f"{config['build_resource_pack']}/assets/minecraft/models/item/none.json", "{}")
 
 	info("Vanilla models created")
```

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.3/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.3/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/io.py` & `python_datapack-0.1.3/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.3/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/print.py` & `python_datapack-0.1.3/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/src/python_datapack/utils/weld.py` & `python_datapack-0.1.3/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/LICENSE` & `python_datapack-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.2/pyproject.toml` & `python_datapack-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.2/PKG-INFO` & `python_datapack-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

