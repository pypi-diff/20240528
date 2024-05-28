# Comparing `tmp/minecraft_resource_pack-1.4.2.tar.gz` & `tmp/minecraft_resource_pack-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_resource_pack-1.4.2.tar", last modified: Wed May  1 11:21:50 2024, max compression
+gzip compressed data, was "minecraft_resource_pack-1.4.3.tar", last modified: Tue May 28 08:05:24 2024, max compression
```

## Comparing `minecraft_resource_pack-1.4.2.tar` & `minecraft_resource_pack-1.4.3.tar`

### file list

```diff
@@ -1,507 +1,507 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/
--rw-rw-rw-   0        0        0     6954 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      206 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      876 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/
--rw-rw-rw-   0        0        0      910 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/
--rw-rw-rw-   0        0        0       43 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      194 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
--rw-rw-rw-   0        0        0      518 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/minecraft_model_reader/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/
--rw-rw-rw-   0        0        0      186 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/
--rw-rw-rw-   0        0        0        0 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/__init__.py
--rw-rw-rw-   0        0        0    18894 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/block.py
--rw-rw-rw-   0        0        0     6410 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/comment_json.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/
--rw-rw-rw-   0        0        0      189 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/__init__.py
--rw-rw-rw-   0        0        0      176 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_no.png
--rw-rw-rw-   0        0        0    11085 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_pack_java.png
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/
--rw-rw-rw-   0        0        0        0 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/
--rw-rw-rw-   0        0        0       35 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/__init__.py
--rw-rw-rw-   0        0        0    13839 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/block_mesh.py
--rw-rw-rw-   0        0        0     4764 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/cube.py
--rw-rw-rw-   0        0        0      545 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/missing_block.py
--rw-rw-rw-   0        0        0      507 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/util.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/
--rw-rw-rw-   0        0        0     1908 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/
--rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/__init__.py
--rw-rw-rw-   0        0        0     1128 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack.py
--rw-rw-rw-   0        0        0     2908 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/
--rw-rw-rw-   0        0        0      111 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/
--rw-rw-rw-   0        0        0      967 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
--rw-rw-rw-   0        0        0      555 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
--rw-rw-rw-   0        0        0    32642 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.142941 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/
--rw-rw-rw-   0        0        0      580 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
--rw-rw-rw-   0        0        0      408 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
--rw-rw-rw-   0        0        0      927 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
--rw-rw-rw-   0        0        0      428 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
--rw-rw-rw-   0        0        0  2864161 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
--rw-rw-rw-   0        0        0     1065 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
--rw-rw-rw-   0        0        0     1027 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
--rw-rw-rw-   0        0        0      905 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
--rw-rw-rw-   0        0        0      736 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
--rw-rw-rw-   0        0        0     1099 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
--rw-rw-rw-   0        0        0     1443 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
--rw-rw-rw-   0        0        0     1439 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
--rw-rw-rw-   0        0        0     5340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
--rw-rw-rw-   0        0        0      449 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
--rw-rw-rw-   0        0        0      373 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
--rw-rw-rw-   0        0        0      781 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
--rw-rw-rw-   0        0        0      688 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
--rw-rw-rw-   0        0        0     1179 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
--rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
--rw-rw-rw-   0        0        0     1225 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
--rw-rw-rw-   0        0        0      666 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
--rw-rw-rw-   0        0        0      644 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
--rw-rw-rw-   0        0        0      654 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
--rw-rw-rw-   0        0        0     1616 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
--rw-rw-rw-   0        0        0     1620 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
--rw-rw-rw-   0        0        0     1264 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
--rw-rw-rw-   0        0        0      364 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
--rw-rw-rw-   0        0        0      822 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
--rw-rw-rw-   0        0        0      912 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
--rw-rw-rw-   0        0        0      333 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
--rw-rw-rw-   0        0        0     1976 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
--rw-rw-rw-   0        0        0     1318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
--rw-rw-rw-   0        0        0     2160 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
--rw-rw-rw-   0        0        0      654 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
--rw-rw-rw-   0        0        0      984 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
--rw-rw-rw-   0        0        0     1008 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
--rw-rw-rw-   0        0        0      374 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
--rw-rw-rw-   0        0        0      365 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
--rw-rw-rw-   0        0        0      334 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
--rw-rw-rw-   0        0        0     1506 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
--rw-rw-rw-   0        0        0     1079 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
--rw-rw-rw-   0        0        0      444 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
--rw-rw-rw-   0        0        0     1209 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
--rw-rw-rw-   0        0        0      448 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
--rw-rw-rw-   0        0        0     1477 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
--rw-rw-rw-   0        0        0      645 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
--rw-rw-rw-   0        0        0      876 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
--rw-rw-rw-   0        0        0    23188 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
--rw-rw-rw-   0        0        0     5220 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
--rw-rw-rw-   0        0        0     1441 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
--rw-rw-rw-   0        0        0    13724 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
--rw-rw-rw-   0        0        0      446 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/
--rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/__init__.py
--rw-rw-rw-   0        0        0     7022 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/download_resources.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.205439 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
--rw-rw-rw-   0        0        0     1137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
--rw-rw-rw-   0        0        0      318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
--rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
--rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
--rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
--rw-rw-rw-   0        0        0      888 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
--rw-rw-rw-   0        0        0     1265 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
--rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
--rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
--rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
--rw-rw-rw-   0        0        0      282 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
--rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
--rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
--rw-rw-rw-   0        0        0      947 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
--rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
--rw-rw-rw-   0        0        0      725 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
--rw-rw-rw-   0        0        0      346 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
--rw-rw-rw-   0        0        0      725 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
--rw-rw-rw-   0        0        0      346 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
--rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
--rw-rw-rw-   0        0        0     1201 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
--rw-rw-rw-   0        0        0      701 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
--rw-rw-rw-   0        0        0      334 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
--rw-rw-rw-   0        0        0     1105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
--rw-rw-rw-   0        0        0      310 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
--rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
--rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
--rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
--rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
--rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
--rw-rw-rw-   0        0        0     1137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
--rw-rw-rw-   0        0        0      669 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
--rw-rw-rw-   0        0        0      318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
--rw-rw-rw-   0        0        0     1281 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
--rw-rw-rw-   0        0        0      984 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
--rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
--rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
--rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
--rw-rw-rw-   0        0        0     1393 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
--rw-rw-rw-   0        0        0      358 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
--rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
--rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
--rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.236684 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.267935 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/
--rw-rw-rw-   0        0        0     1862 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
--rw-rw-rw-   0        0        0     1874 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
--rw-rw-rw-   0        0        0     1865 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
--rw-rw-rw-   0        0        0     1871 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
--rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
--rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
--rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
--rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
--rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
--rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
--rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
--rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
--rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
--rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.283563 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
--rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
--rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
--rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
--rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
--rw-rw-rw-   0        0        0       85 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
--rw-rw-rw-   0        0        0       85 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
--rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
--rw-rw-rw-   0        0        0       81 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
--rw-rw-rw-   0        0        0       81 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
--rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
--rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
--rw-rw-rw-   0        0        0     1525 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
--rw-rw-rw-   0        0        0     1535 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
--rw-rw-rw-   0        0        0     1610 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
--rw-rw-rw-   0        0        0     1507 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
--rw-rw-rw-   0        0        0     2669 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
--rw-rw-rw-   0        0        0     1592 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
--rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
--rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
--rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
--rw-rw-rw-   0        0        0     1855 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
--rw-rw-rw-   0        0        0      115 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
--rw-rw-rw-   0        0        0     1537 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
--rw-rw-rw-   0        0        0      117 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
--rw-rw-rw-   0        0        0     1527 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
--rw-rw-rw-   0        0        0      579 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
--rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
--rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
--rw-rw-rw-   0        0        0      109 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
--rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.299188 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
--rw-rw-rw-   0        0        0     4816 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
--rw-rw-rw-   0        0        0     4831 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
--rw-rw-rw-   0        0        0     4810 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
--rw-rw-rw-   0        0        0     4824 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
--rw-rw-rw-   0        0        0      592 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
--rw-rw-rw-   0        0        0      660 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
--rw-rw-rw-   0        0        0      657 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
--rw-rw-rw-   0        0        0      659 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
--rw-rw-rw-   0        0        0      656 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
--rw-rw-rw-   0        0        0      660 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
--rw-rw-rw-   0        0        0      657 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
--rw-rw-rw-   0        0        0      659 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
--rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
--rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
--rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
--rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
--rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
--rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
--rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
--rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
--rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.314816 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/
--rw-rw-rw-   0        0        0       96 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
--rw-rw-rw-   0        0        0     3870 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
--rw-rw-rw-   0        0        0      559 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
--rw-rw-rw-   0        0        0      559 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
--rw-rw-rw-   0        0        0       87 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
--rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
--rw-rw-rw-   0        0        0       95 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
--rw-rw-rw-   0        0        0      134 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.314816 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
--rw-rw-rw-   0        0        0      163 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
--rw-rw-rw-   0        0        0      163 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
--rw-rw-rw-   0        0        0      157 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
--rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
--rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
--rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
--rw-rw-rw-   0        0        0      149 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
--rw-rw-rw-   0        0        0      141 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
--rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
--rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
--rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
--rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
--rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
--rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
--rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
--rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
--rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
--rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
--rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
--rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
--rw-rw-rw-   0        0        0     1184 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
--rw-rw-rw-   0        0        0     1173 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
--rw-rw-rw-   0        0        0     1167 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
--rw-rw-rw-   0        0        0     1171 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
--rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
--rw-rw-rw-   0        0        0      147 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
--rw-rw-rw-   0        0        0      106 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
--rw-rw-rw-   0        0        0      116 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
--rw-rw-rw-   0        0        0      118 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
--rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
--rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
--rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
--rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
--rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
--rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
--rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
--rw-rw-rw-   0        0        0       96 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
--rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
--rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
--rw-rw-rw-   0        0        0     1208 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
--rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
--rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
--rw-rw-rw-   0        0        0      137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
--rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
--rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
--rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
--rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
--rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
--rw-rw-rw-   0        0        0      588 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
--rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
--rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
--rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
--rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.361687 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.361687 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/
--rw-rw-rw-   0        0        0     2769 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
--rw-rw-rw-   0        0        0     3786 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
--rw-rw-rw-   0        0        0     3707 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
--rw-rw-rw-   0        0        0     3813 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
--rw-rw-rw-   0        0        0     3518 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
--rw-rw-rw-   0        0        0     3751 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
--rw-rw-rw-   0        0        0     4220 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
--rw-rw-rw-   0        0        0     3953 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
--rw-rw-rw-   0        0        0     4151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
--rw-rw-rw-   0        0        0     4178 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
--rw-rw-rw-   0        0        0     4298 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
--rw-rw-rw-   0        0        0     4205 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
--rw-rw-rw-   0        0        0     4056 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
--rw-rw-rw-   0        0        0     3790 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
--rw-rw-rw-   0        0        0     3985 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
--rw-rw-rw-   0        0        0     4457 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
--rw-rw-rw-   0        0        0      651 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
--rw-rw-rw-   0        0        0     1265 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
--rw-rw-rw-   0        0        0      213 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
--rw-rw-rw-   0        0        0     1286 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
--rw-rw-rw-   0        0        0     1405 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
--rw-rw-rw-   0        0        0      927 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
--rw-rw-rw-   0        0        0      117 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
--rw-rw-rw-   0        0        0    22749 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
--rw-rw-rw-   0        0        0     1687 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack.py
--rw-rw-rw-   0        0        0    22312 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
--rw-rw-rw-   0        0        0      299 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/
--rw-rw-rw-   0        0        0      876 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    48947 2024-05-01 11:21:50.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      177 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0     1190 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      142 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/
+-rw-rw-rw-   0        0        0     6954 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      206 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      963 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/
+-rw-rw-rw-   0        0        0      910 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/__pyinstaller/
+-rw-rw-rw-   0        0        0       56 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      194 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
+-rw-rw-rw-   0        0        0      518 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/minecraft_model_reader/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/
+-rw-rw-rw-   0        0        0      202 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/amulet/
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/amulet/__init__.py
+-rw-rw-rw-   0        0        0    18577 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/amulet/block.py
+-rw-rw-rw-   0        0        0     6401 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/comment_json.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/image/
+-rw-rw-rw-   0        0        0      189 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/image/__init__.py
+-rw-rw-rw-   0        0        0      176 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/image/missing_no.png
+-rw-rw-rw-   0        0        0    11085 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/image/missing_pack_java.png
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/
+-rw-rw-rw-   0        0        0       35 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/__init__.py
+-rw-rw-rw-   0        0        0    15198 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/block_mesh.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/cube.py
+-rw-rw-rw-   0        0        0      545 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/missing_block.py
+-rw-rw-rw-   0        0        0      605 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/util.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/
+-rw-rw-rw-   0        0        0     2259 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/
+-rw-rw-rw-   0        0        0      105 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/__init__.py
+-rw-rw-rw-   0        0        0     1143 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/resource_pack.py
+-rw-rw-rw-   0        0        0     3015 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.499862 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/
+-rw-rw-rw-   0        0        0      111 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.515493 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/
+-rw-rw-rw-   0        0        0      967 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
+-rw-rw-rw-   0        0        0      555 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
+-rw-rw-rw-   0        0        0    32642 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.515493 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.515493 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/
+-rw-rw-rw-   0        0        0      580 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
+-rw-rw-rw-   0        0        0      408 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
+-rw-rw-rw-   0        0        0      927 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
+-rw-rw-rw-   0        0        0      428 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
+-rw-rw-rw-   0        0        0  2864161 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.531113 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
+-rw-rw-rw-   0        0        0     1077 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
+-rw-rw-rw-   0        0        0     1043 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
+-rw-rw-rw-   0        0        0      877 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
+-rw-rw-rw-   0        0        0      708 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
+-rw-rw-rw-   0        0        0     1178 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
+-rw-rw-rw-   0        0        0     1493 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
+-rw-rw-rw-   0        0        0     1481 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
+-rw-rw-rw-   0        0        0     5358 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
+-rw-rw-rw-   0        0        0      449 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
+-rw-rw-rw-   0        0        0      345 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
+-rw-rw-rw-   0        0        0     1005 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
+-rw-rw-rw-   0        0        0      660 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
+-rw-rw-rw-   0        0        0     1145 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
+-rw-rw-rw-   0        0        0      340 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
+-rw-rw-rw-   0        0        0     1197 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
+-rw-rw-rw-   0        0        0      638 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
+-rw-rw-rw-   0        0        0      616 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
+-rw-rw-rw-   0        0        0      626 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
+-rw-rw-rw-   0        0        0     1634 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
+-rw-rw-rw-   0        0        0     1638 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
+-rw-rw-rw-   0        0        0     1230 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
+-rw-rw-rw-   0        0        0      337 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
+-rw-rw-rw-   0        0        0     1035 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
+-rw-rw-rw-   0        0        0      892 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
+-rw-rw-rw-   0        0        0      305 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
+-rw-rw-rw-   0        0        0     2051 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
+-rw-rw-rw-   0        0        0     1284 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
+-rw-rw-rw-   0        0        0     2194 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
+-rw-rw-rw-   0        0        0      626 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
+-rw-rw-rw-   0        0        0      956 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
+-rw-rw-rw-   0        0        0      980 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
+-rw-rw-rw-   0        0        0      374 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
+-rw-rw-rw-   0        0        0      365 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
+-rw-rw-rw-   0        0        0      306 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
+-rw-rw-rw-   0        0        0     1546 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
+-rw-rw-rw-   0        0        0     1051 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
+-rw-rw-rw-   0        0        0      444 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
+-rw-rw-rw-   0        0        0     1175 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
+-rw-rw-rw-   0        0        0      448 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
+-rw-rw-rw-   0        0        0     1457 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
+-rw-rw-rw-   0        0        0      617 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
+-rw-rw-rw-   0        0        0      997 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
+-rw-rw-rw-   0        0        0    23188 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
+-rw-rw-rw-   0        0        0     5311 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
+-rw-rw-rw-   0        0        0     1646 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
+-rw-rw-rw-   0        0        0    15235 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      454 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.531113 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/
+-rw-rw-rw-   0        0        0      105 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/__init__.py
+-rw-rw-rw-   0        0        0     7269 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/download_resources.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.531113 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.577992 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
+-rw-rw-rw-   0        0        0     1137 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
+-rw-rw-rw-   0        0        0      318 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
+-rw-rw-rw-   0        0        0      888 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
+-rw-rw-rw-   0        0        0     1265 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
+-rw-rw-rw-   0        0        0     1169 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1249 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
+-rw-rw-rw-   0        0        0      282 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
+-rw-rw-rw-   0        0        0      947 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
+-rw-rw-rw-   0        0        0     1249 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
+-rw-rw-rw-   0        0        0      725 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
+-rw-rw-rw-   0        0        0      346 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
+-rw-rw-rw-   0        0        0      725 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
+-rw-rw-rw-   0        0        0      346 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
+-rw-rw-rw-   0        0        0     1201 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
+-rw-rw-rw-   0        0        0      701 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
+-rw-rw-rw-   0        0        0      334 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
+-rw-rw-rw-   0        0        0     1105 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
+-rw-rw-rw-   0        0        0      310 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1185 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
+-rw-rw-rw-   0        0        0     1185 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
+-rw-rw-rw-   0        0        0     1137 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
+-rw-rw-rw-   0        0        0      669 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
+-rw-rw-rw-   0        0        0      318 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
+-rw-rw-rw-   0        0        0     1281 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
+-rw-rw-rw-   0        0        0      984 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
+-rw-rw-rw-   0        0        0     1153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
+-rw-rw-rw-   0        0        0     1393 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
+-rw-rw-rw-   0        0        0      358 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1185 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.609238 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.640488 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/
+-rw-rw-rw-   0        0        0     1862 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
+-rw-rw-rw-   0        0        0     1874 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
+-rw-rw-rw-   0        0        0     1865 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
+-rw-rw-rw-   0        0        0     1871 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
+-rw-rw-rw-   0        0        0      107 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
+-rw-rw-rw-   0        0        0      104 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
+-rw-rw-rw-   0        0        0      104 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
+-rw-rw-rw-   0        0        0      104 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
+-rw-rw-rw-   0        0        0      104 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
+-rw-rw-rw-   0        0        0      100 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
+-rw-rw-rw-   0        0        0      100 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
+-rw-rw-rw-   0        0        0      100 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
+-rw-rw-rw-   0        0        0      100 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.656121 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
+-rw-rw-rw-   0        0        0       88 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
+-rw-rw-rw-   0        0        0       88 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
+-rw-rw-rw-   0        0        0       88 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
+-rw-rw-rw-   0        0        0       88 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
+-rw-rw-rw-   0        0        0       85 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
+-rw-rw-rw-   0        0        0       85 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
+-rw-rw-rw-   0        0        0       81 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
+-rw-rw-rw-   0        0        0       81 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
+-rw-rw-rw-   0        0        0     1525 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
+-rw-rw-rw-   0        0        0     1535 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
+-rw-rw-rw-   0        0        0     1610 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
+-rw-rw-rw-   0        0        0     1507 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
+-rw-rw-rw-   0        0        0     2669 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
+-rw-rw-rw-   0        0        0     1592 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
+-rw-rw-rw-   0        0        0      153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
+-rw-rw-rw-   0        0        0      105 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
+-rw-rw-rw-   0        0        0     1855 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
+-rw-rw-rw-   0        0        0      115 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
+-rw-rw-rw-   0        0        0     1537 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
+-rw-rw-rw-   0        0        0      117 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
+-rw-rw-rw-   0        0        0     1527 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
+-rw-rw-rw-   0        0        0      579 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
+-rw-rw-rw-   0        0        0      139 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
+-rw-rw-rw-   0        0        0      104 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
+-rw-rw-rw-   0        0        0      109 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.671743 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
+-rw-rw-rw-   0        0        0     4816 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
+-rw-rw-rw-   0        0        0     4831 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
+-rw-rw-rw-   0        0        0     4810 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
+-rw-rw-rw-   0        0        0     4824 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
+-rw-rw-rw-   0        0        0      592 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
+-rw-rw-rw-   0        0        0      660 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
+-rw-rw-rw-   0        0        0      657 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
+-rw-rw-rw-   0        0        0      659 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
+-rw-rw-rw-   0        0        0      656 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
+-rw-rw-rw-   0        0        0      660 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
+-rw-rw-rw-   0        0        0      657 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
+-rw-rw-rw-   0        0        0      659 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
+-rw-rw-rw-   0        0        0       90 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
+-rw-rw-rw-   0        0        0       90 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
+-rw-rw-rw-   0        0        0       90 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
+-rw-rw-rw-   0        0        0       90 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
+-rw-rw-rw-   0        0        0      108 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
+-rw-rw-rw-   0        0        0      108 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
+-rw-rw-rw-   0        0        0      108 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
+-rw-rw-rw-   0        0        0      108 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.671743 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/
+-rw-rw-rw-   0        0        0       96 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
+-rw-rw-rw-   0        0        0     3870 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
+-rw-rw-rw-   0        0        0      559 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
+-rw-rw-rw-   0        0        0      559 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
+-rw-rw-rw-   0        0        0       87 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
+-rw-rw-rw-   0        0        0      105 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
+-rw-rw-rw-   0        0        0       95 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
+-rw-rw-rw-   0        0        0      134 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.687368 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
+-rw-rw-rw-   0        0        0      163 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
+-rw-rw-rw-   0        0        0      163 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
+-rw-rw-rw-   0        0        0      157 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
+-rw-rw-rw-   0        0        0      155 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
+-rw-rw-rw-   0        0        0      149 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
+-rw-rw-rw-   0        0        0      141 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.702989 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
+-rw-rw-rw-   0        0        0      125 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
+-rw-rw-rw-   0        0        0      125 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
+-rw-rw-rw-   0        0        0      125 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
+-rw-rw-rw-   0        0        0      125 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
+-rw-rw-rw-   0        0        0      129 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
+-rw-rw-rw-   0        0        0      129 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
+-rw-rw-rw-   0        0        0      129 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
+-rw-rw-rw-   0        0        0      129 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
+-rw-rw-rw-   0        0        0      121 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
+-rw-rw-rw-   0        0        0      121 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
+-rw-rw-rw-   0        0        0      121 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
+-rw-rw-rw-   0        0        0      121 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
+-rw-rw-rw-   0        0        0     1184 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
+-rw-rw-rw-   0        0        0     1173 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
+-rw-rw-rw-   0        0        0     1167 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
+-rw-rw-rw-   0        0        0     1171 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
+-rw-rw-rw-   0        0        0      147 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
+-rw-rw-rw-   0        0        0      106 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
+-rw-rw-rw-   0        0        0      116 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
+-rw-rw-rw-   0        0        0      118 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.718613 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
+-rw-rw-rw-   0        0        0       97 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
+-rw-rw-rw-   0        0        0       97 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
+-rw-rw-rw-   0        0        0       97 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
+-rw-rw-rw-   0        0        0      103 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
+-rw-rw-rw-   0        0        0       97 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
+-rw-rw-rw-   0        0        0      100 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
+-rw-rw-rw-   0        0        0       97 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
+-rw-rw-rw-   0        0        0       96 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
+-rw-rw-rw-   0        0        0       98 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
+-rw-rw-rw-   0        0        0       99 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
+-rw-rw-rw-   0        0        0     1208 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.718613 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
+-rw-rw-rw-   0        0        0      135 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
+-rw-rw-rw-   0        0        0      133 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
+-rw-rw-rw-   0        0        0      137 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
+-rw-rw-rw-   0        0        0      139 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
+-rw-rw-rw-   0        0        0      135 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
+-rw-rw-rw-   0        0        0      139 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
+-rw-rw-rw-   0        0        0      129 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
+-rw-rw-rw-   0        0        0      135 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
+-rw-rw-rw-   0        0        0      588 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
+-rw-rw-rw-   0        0        0      135 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
+-rw-rw-rw-   0        0        0      135 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
+-rw-rw-rw-   0        0        0      153 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.484247 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.718613 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/
+-rw-rw-rw-   0        0        0     2769 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
+-rw-rw-rw-   0        0        0     3786 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
+-rw-rw-rw-   0        0        0     3707 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
+-rw-rw-rw-   0        0        0     3813 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
+-rw-rw-rw-   0        0        0     3518 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
+-rw-rw-rw-   0        0        0     3751 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
+-rw-rw-rw-   0        0        0     4220 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
+-rw-rw-rw-   0        0        0     3953 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
+-rw-rw-rw-   0        0        0     4151 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
+-rw-rw-rw-   0        0        0     4178 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
+-rw-rw-rw-   0        0        0     4298 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
+-rw-rw-rw-   0        0        0     4205 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
+-rw-rw-rw-   0        0        0     4056 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
+-rw-rw-rw-   0        0        0     3790 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
+-rw-rw-rw-   0        0        0     3985 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
+-rw-rw-rw-   0        0        0     4457 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
+-rw-rw-rw-   0        0        0      651 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
+-rw-rw-rw-   0        0        0     1265 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
+-rw-rw-rw-   0        0        0      213 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
+-rw-rw-rw-   0        0        0     1286 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
+-rw-rw-rw-   0        0        0     1405 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
+-rw-rw-rw-   0        0        0      927 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
+-rw-rw-rw-   0        0        0      117 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
+-rw-rw-rw-   0        0        0    22749 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
+-rw-rw-rw-   0        0        0     1702 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/resource_pack.py
+-rw-rw-rw-   0        0        0    22937 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      314 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/
+-rw-rw-rw-   0        0        0      963 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    48947 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 08:05:23.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      200 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-28 08:05:24.000000 minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1217 2024-05-28 08:05:24.734244 minecraft_resource_pack-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      142 2024-05-28 08:04:46.000000 minecraft_resource_pack-1.4.3/setup.py
```

### Comparing `minecraft_resource_pack-1.4.2/LICENSE` & `minecraft_resource_pack-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/PKG-INFO` & `minecraft_resource_pack-1.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-resource-pack
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python library reading Minecraft's various resource pack formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,9 @@
 Provides-Extra: docs
 Requires-Dist: Sphinx>=1.7.4; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.3.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=0.3.1; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: black>=22.3; extra == "dev"
 Requires-Dist: pre_commit>=1.11.1; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-pyinstaller; extra == "dev"
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/__init__.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/block.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/amulet/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from sys import getsizeof
 import re
-from typing import Dict, Iterable, Tuple, Union
+from typing import Iterable, Union, Optional, Any
 import amulet_nbt
 
 PropertyValueType = Union[
     amulet_nbt.TAG_Byte,
     amulet_nbt.TAG_Short,
     amulet_nbt.TAG_Int,
     amulet_nbt.TAG_Long,
     amulet_nbt.TAG_String,
 ]
-PropertyType = Dict[str, PropertyValueType]
+PropertyType = dict[str, PropertyValueType]
 
 PropertyDataTypes = (
     amulet_nbt.TAG_Byte,
     amulet_nbt.TAG_Short,
     amulet_nbt.TAG_Int,
     amulet_nbt.TAG_Long,
     amulet_nbt.TAG_String,
@@ -104,49 +104,49 @@
     )
     properties_regex = re.compile(r"(?:,(?P<name>[a-z0-9_]+)=(?P<value>[a-z0-9_]+))")
 
     def __init__(
         self,
         namespace: str,
         base_name: str,
-        properties: PropertyType = None,
-        extra_blocks: Union[Block, Iterable[Block]] = None,
+        properties: Optional[PropertyType] = None,
+        extra_blocks: Union[Block, Iterable[Block], None] = None,
     ):
         assert (isinstance(namespace, str) or namespace is None) and isinstance(
             base_name, str
         ), f"namespace and base_name must be strings {namespace} {base_name}"
         self._namespace = namespace
         self._base_name = base_name
         self._namespaced_name = f"{namespace}:{base_name}"
 
-        self._blockstate = None
-        self._snbt_blockstate = None
-        self._full_blockstate = None
+        self._blockstate: Optional[str] = None
+        self._snbt_blockstate: Optional[str] = None
+        self._full_blockstate: Optional[str] = None
 
         if properties is None:
             properties = {}
         assert isinstance(properties, dict) and all(
             isinstance(val, PropertyDataTypes) for val in properties.values()
         ), properties
 
         self._properties = properties
-        self._extra_blocks = ()
+        self._extra_blocks: tuple[Block, ...] = ()
         if extra_blocks:
             if isinstance(extra_blocks, Block):
                 extra_blocks = [extra_blocks]
             self._extra_blocks = tuple(extra_blocks)
 
     @classmethod
-    def from_string_blockstate(cls, blockstate: str):
+    def from_string_blockstate(cls, blockstate: str) -> Block:
         """Parse a Java format blockstate where values are all strings and populate a Block class with the data."""
         namespace, block_name, properties = cls.parse_blockstate_string(blockstate)
         return cls(namespace, block_name, properties)
 
     @classmethod
-    def from_snbt_blockstate(cls, blockstate: str):
+    def from_snbt_blockstate(cls, blockstate: str) -> Block:
         """Parse a blockstate where values are SNBT of any type and populate a Block class with the data."""
         namespace, block_name, properties = cls.parse_blockstate_string(
             blockstate, True
         )
         return cls(namespace, block_name, properties)
 
     @property
@@ -189,22 +189,23 @@
     def blockstate(self) -> str:
         """The Java blockstate string of this Block object (Eg: `minecraft:stone`, `minecraft:oak_log[axis=x]`)
         Note if there are extra blocks this will only show the base block.
         Note this will only contain properties with TAG_String values.
         :return: The blockstate string
         """
         if self._blockstate is None:
-            self._blockstate = self.namespaced_name
+            blockstate = self.namespaced_name
             if self.properties:
                 props = [
                     f"{key}={value.py_data}"
                     for key, value in sorted(self.properties.items())
                     if isinstance(value, amulet_nbt.TAG_String)
                 ]
-                self._blockstate += f"[{','.join(props)}]"
+                blockstate += f"[{','.join(props)}]"
+            self._blockstate = blockstate
         return self._blockstate
 
     @property
     def snbt_blockstate(self) -> str:
         """The SNBT blockstate string of this Block object (Eg: `minecraft:bell[attachment="standing",direction=0,toggle_bit=0b]`)
         Note if there are extra blocks this will only show the base block.
         :return: The blockstate string
@@ -244,45 +245,47 @@
             return Block(
                 namespace=self.namespace,
                 base_name=self.base_name,
                 properties=self.properties,
             )
 
     @property
-    def extra_blocks(self) -> Tuple[Block, ...]:
+    def extra_blocks(self) -> tuple[Block, ...]:
         """
         Returns a tuple of the extra blocks contained in the Block instance
 
         :return: A tuple of Block objects
         """
         return self._extra_blocks
 
     @property
-    def block_tuple(self) -> Tuple[Block, ...]:
+    def block_tuple(self) -> tuple[Block, ...]:
         """
         Returns the stack of blocks represented by this object as a tuple.
         This is a tuple of base_block and extra_blocks
         :return: A tuple of Block objects
         """
         return (self.base_block,) + self.extra_blocks
 
     @staticmethod
     def parse_blockstate_string(
         blockstate: str, snbt: bool = False
-    ) -> Tuple[str, str, PropertyType]:
+    ) -> tuple[str, str, PropertyType]:
         """Parse a blockstate string and return the data.
 
         :param blockstate: The blockstate to parse
         :param snbt: Are the property values in SNBT format. If false all values will be `TAG_String`s
         :return: namespace, block_name, properties
         """
         if snbt:
             match = Block.snbt_blockstate_regex.match(blockstate)
         else:
             match = Block.blockstate_regex.match(blockstate)
+        if match is None:
+            raise ValueError
         namespace = match.group("namespace") or "minecraft"
         base_name = match.group("base_name")
 
         if match.group("property_name") is not None:
             properties = {match.group("property_name"): match.group("property_value")}
             properties_string = match.group("properties")
             if properties_string is not None:
@@ -320,38 +323,38 @@
 
     def __repr__(self) -> str:
         """
         :return: The base blockstate string of the Block object along with the blockstate strings of included extra blocks
         """
         return f"Block({', '.join([str(b) for b in (self, *self.extra_blocks)])})"
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._extra_blocks) + 1
 
-    def __eq__(self, other: Block) -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Checks the equality of this Block object to another Block object
 
         :param other: The Block object to check against
         :return: True if the Blocks objects are equal, False otherwise
         """
-        if self.__class__ != other.__class__:
-            return False
+        if not isinstance(other, Block):
+            return NotImplemented
 
         return (
             self.namespaced_name == other.namespaced_name
             and self.properties == other.properties
             and self.extra_blocks == other.extra_blocks
         )
 
     def __gt__(self, other: Block) -> bool:
         """
         Allows blocks to be sorted so numpy.unique can be used on them
         """
-        if self.__class__ != other.__class__:
+        if not isinstance(other, Block):
             return NotImplemented
         return hash(self).__gt__(hash(other))
 
     def __hash__(self) -> int:
         """
         Hashes the Block object
 
@@ -478,27 +481,12 @@
         return Block(
             namespace=self.namespace,
             base_name=self.base_name,
             properties=self.properties,
             extra_blocks=[*self.extra_blocks[: layer - 1], *self.extra_blocks[layer:]],
         )
 
-    def __sizeof__(self):
-        size = (
-            getsizeof(self._namespace)
-            + getsizeof(self._base_name)
-            + getsizeof(self._namespaced_name)
-            + getsizeof(self._properties)
-            + getsizeof(self._blockstate)
-            + getsizeof(self._extra_blocks)
-            + getsizeof(self._snbt_blockstate)
-            + getsizeof(self._full_blockstate)
-        )
-        for eb in self.extra_blocks:
-            size += getsizeof(eb)
-        return size
-
 
 # some blocks that probably will not change. Keeping these in one place will make them easier to change if they do.
 UniversalAirBlock = Block("universal_minecraft", "air")
 # do not rely on this staying the same.
 UniversalAirLikeBlocks = (UniversalAirBlock, Block("universal_minecraft", "cave_air"))
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/comment_json.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/comment_json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,189 +1,188 @@
-import json
-from typing import TextIO
+from json import JSONDecodeError, loads as json_loads
+from typing import TextIO, Union
 
 """
 Some of the Bedrock json files contain comments which is not valid JSON and the standard json parser
 will throw errors. This will first try and use the vanilla json parser and fall back to the slower version if that fails.
 """
 
 
-class CommentJSONDecodeError(json.JSONDecodeError):
+JSONValue = Union[str, int, float, bool, None, "JSONDict", "JSONList"]
+JSONDict = dict[str, JSONValue]
+JSONList = list[JSONValue]
+
+
+class CommentJSONDecodeError(JSONDecodeError):
     pass
 
 
-def from_file(path: str):
+def from_file(path: str) -> JSONValue:
     with open(path) as f:
         return load(f)
 
 
-def load(obj: TextIO):
+def load(obj: TextIO) -> JSONValue:
     return loads(obj.read())
 
 
-def loads(s: str):
+def loads(s: str) -> JSONValue:
     try:
-        return json.loads(s)
-    except json.JSONDecodeError:
+        return json_loads(s)  # type: ignore
+    except JSONDecodeError:
         return _loads(s)
 
 
-def _loads(_json):
+def _loads(text: str) -> JSONValue:
     # given a valid MinecraftJSON string will return the values as python objects
     # in this context MinecraftJSON is standard JSON but with comment blocks and
     # line comments that would normally be illegal in standard JSON
     _number = set("0123456789-")
     _float = set("0123456789-.")
     _whitespace = set(" \t\r\n")
 
-    def strip_whitespace(_json, index):
+    def strip_whitespace(index: int) -> int:
         # skips whitespace characters (<space>, <tab>, <charrage return> and <newline>)
         # as well as block comments and line comments
-        while _json[index] in _whitespace:
+        while text[index] in _whitespace:
             index += 1
-        if _json[index] == "/":
-            if _json[index + 1] == "/":
+        if text[index] == "/":
+            if text[index + 1] == "/":
                 index += 2
-                while _json[index] != "\n":
+                while text[index] != "\n":
                     index += 1
-                index = strip_whitespace(_json, index)
-            elif _json[index + 1] == "*":
+                index = strip_whitespace(index)
+            elif text[index + 1] == "*":
                 index += 2
-                while _json[index : index + 2] != "*/":
+                while text[index : index + 2] != "*/":
                     index += 1
-                    if index + 1 >= len(_json):
-                        raise json.JSONDecodeError(
-                            "expected */ but reached the end of file", _json, index
+                    if index + 1 >= len(text):
+                        raise JSONDecodeError(
+                            "expected */ but reached the end of file", text, index
                         )
                 index += 2
-                index = strip_whitespace(_json, index)
+                index = strip_whitespace(index)
             else:
-                raise json.JSONDecodeError(
-                    f"unexpected / at index {index}", _json, index
-                )
+                raise JSONDecodeError(f"unexpected / at index {index}", text, index)
         return index
 
-    def parse_json_recursive(_json, index=0):
-        index = strip_whitespace(_json, index)
-        if _json[index] == "{":
+    def parse_json_recursive(index: int = 0) -> tuple[JSONValue, int]:
+        index = strip_whitespace(index)
+        if text[index] == "{":
             index += 1
             # dictionary
             json_obj = {}
             repeat = True
             while repeat:
-                index = strip_whitespace(_json, index)
+                index = strip_whitespace(index)
                 # }"
-                if _json[index] == '"':
+                if text[index] == '"':
                     index += 1
                     key = ""
-                    while _json[index] != '"':
-                        key += _json[index]
+                    while text[index] != '"':
+                        key += text[index]
                         index += 1
                     index += 1
 
-                    index = strip_whitespace(_json, index)
+                    index = strip_whitespace(index)
 
-                    if _json[index] == ":":
+                    if text[index] == ":":
                         index += 1
                     else:
-                        raise json.JSONDecodeError(
-                            f"expected : got {_json[index]} at index {index}",
-                            _json,
+                        raise JSONDecodeError(
+                            f"expected : got {text[index]} at index {index}",
+                            text,
                             index,
                         )
 
-                    index = strip_whitespace(_json, index)
+                    index = strip_whitespace(index)
 
-                    json_obj[key], index = parse_json_recursive(_json, index)
+                    json_obj[key], index = parse_json_recursive(index)
 
-                    index = strip_whitespace(_json, index)
+                    index = strip_whitespace(index)
 
-                    if _json[index] == ",":
+                    if text[index] == ",":
                         index += 1
                     else:
                         repeat = False
                 else:
                     repeat = False
 
-            if index >= len(_json):
-                raise json.JSONDecodeError(
-                    "expected } but reached end of file", _json, index
-                )
-            elif _json[index] == "}":
+            if index >= len(text):
+                raise JSONDecodeError("expected } but reached end of file", text, index)
+            elif text[index] == "}":
                 index += 1
             else:
-                raise json.JSONDecodeError(
-                    f"expected }} got {_json[index]} at index {index}", _json, index
+                raise JSONDecodeError(
+                    f"expected }} got {text[index]} at index {index}", text, index
                 )
             return json_obj, index
 
-        elif _json[index] == "[":
+        elif text[index] == "[":
             index += 1
             # list
-            json_obj = []
-            index = strip_whitespace(_json, index)
-            repeat = _json[index] != "]"
+            json_array = []
+            index = strip_whitespace(index)
+            repeat = text[index] != "]"
             while repeat:
-                val, index = parse_json_recursive(_json, index)
-                json_obj.append(val)
+                val, index = parse_json_recursive(index)
+                json_array.append(val)
 
-                index = strip_whitespace(_json, index)
+                index = strip_whitespace(index)
 
-                if _json[index] == ",":
+                if text[index] == ",":
                     index += 1
                 else:
                     repeat = False
-                index = strip_whitespace(_json, index)
+                index = strip_whitespace(index)
 
-            if index >= len(_json):
-                raise json.JSONDecodeError(
-                    "expected ] but reached end of file", _json, index
-                )
-            elif _json[index] == "]":
+            if index >= len(text):
+                raise JSONDecodeError("expected ] but reached end of file", text, index)
+            elif text[index] == "]":
                 index += 1
             else:
-                raise json.JSONDecodeError(
-                    f"expected ] got {_json[index]} at index {index}", _json, index
+                raise JSONDecodeError(
+                    f"expected ] got {text[index]} at index {index}", text, index
                 )
-            return json_obj, index
+            return json_array, index
 
-        elif _json[index] == '"':
+        elif text[index] == '"':
             index += 1
             # string
             json_obj_list = []
-            while _json[index] != '"':
-                json_obj_list.append(_json[index])
+            while text[index] != '"':
+                json_obj_list.append(text[index])
                 index += 1
             index += 1
             return "".join(json_obj_list), index
 
-        elif _json[index] in _number:
+        elif text[index] in _number:
             # number
             json_obj_list = []
-            while _json[index] in _float:
-                json_obj_list += _json[index]
+            while text[index] in _float:
+                json_obj_list += text[index]
                 index += 1
             if "." in json_obj_list:
                 return float("".join(json_obj_list)), index
             else:
                 return int("".join(json_obj_list)), index
 
-        elif _json[index] == "n" and _json[index : index + 4] == "null":
+        elif text[index] == "n" and text[index : index + 4] == "null":
             index += 4
             return None, index
 
-        elif _json[index] == "t" and _json[index : index + 4] == "true":
+        elif text[index] == "t" and text[index : index + 4] == "true":
             index += 4
             return True, index
 
-        elif _json[index] == "f" and _json[index : index + 5] == "false":
+        elif text[index] == "f" and text[index : index + 5] == "false":
             index += 5
             return False, index
         else:
-            raise json.JSONDecodeError(
-                f'unexpected key {_json[index]} at {index}. Expected {{, [, ", num, null, true or false',
-                _json,
+            raise JSONDecodeError(
+                f'unexpected key {text[index]} at {index}. Expected {{, [, ", num, null, true or false',
+                text,
                 index,
             )
 
     # call recursive function and pass back python object
-    return parse_json_recursive(_json)[0]
+    return parse_json_recursive()[0]
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_pack_java.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/image/missing_pack_java.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/block_mesh.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/block_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,147 @@
-from typing import Dict, Tuple, Union, Iterable, Optional
+from __future__ import annotations
+from typing import Optional, Any
+from collections.abc import Iterable
 import numpy
+import itertools
+from enum import IntEnum
 
 from minecraft_model_reader.api.mesh.util import rotate_3d
 
 FACE_KEYS = {"down", "up", "north", "east", "south", "west", None}
 
 
-def _create_cull_map() -> Dict[Tuple[int, int], Dict[Optional[str], Optional[str]]]:
+def _create_cull_map() -> dict[tuple[int, int], dict[Optional[str], Optional[str]]]:
     cull_remap_ = {}
     roty_map = ["north", "east", "south", "west"]
     for roty in range(-3, 4):
         for rotx in range(-3, 4):
             roty_map_rotated = roty_map[roty:] + roty_map[:roty]
             rotx_map = [roty_map_rotated[0], "down", roty_map_rotated[2], "up"]
             rotx_map_rotated = rotx_map[rotx:] + rotx_map[:rotx]
             roty_remap = dict(zip(roty_map, roty_map_rotated))
             rotx_remap = dict(zip(rotx_map, rotx_map_rotated))
-            cull_remap_[(roty, rotx)] = {
-                key: rotx_remap.get(roty_remap.get(key, key), roty_remap.get(key, key))
-                for key in FACE_KEYS
-            }
+            cull_remap_value: dict[Optional[str], Optional[str]] = {}
+            cull_remap_[(roty, rotx)] = cull_remap_value
+            for key in FACE_KEYS:
+                if key is None:
+                    cull_remap_value[key] = None
+                else:
+                    roty_value = roty_remap.get(key, key)
+                    cull_remap_value[key] = rotx_remap.get(roty_value, roty_value)
     return cull_remap_
 
 
 cull_remap_all = _create_cull_map()
 
 
+class Transparency(IntEnum):
+    FullOpaque = 0  # the block is a full block with opaque textures
+    FullTranslucent = (
+        1  # the block is a full block with transparent/translucent textures
+    )
+    Partial = 2  # the block is not a full block
+
+
 class BlockMesh:
     """Class for storing model data"""
 
     @classmethod
-    def merge(cls, models: Iterable["BlockMesh"]) -> "BlockMesh":
-        textures = []
+    def merge(cls, models: Iterable[BlockMesh]) -> BlockMesh:
+        textures_src: list[str] = []
         texture_count = 0
-        vert_count = {side: 0 for side in FACE_KEYS}
-        verts = {side: [] for side in FACE_KEYS}
-        tverts = {side: [] for side in FACE_KEYS}
-        tint_verts = {side: [] for side in FACE_KEYS}
-        faces = {side: [] for side in FACE_KEYS}
-        texture_indexes = {side: [] for side in FACE_KEYS}
-        transparent = 2
+        vert_count: dict[Optional[str], int] = {side: 0 for side in FACE_KEYS}
+        verts_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        tverts_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        tint_verts_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        faces_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        texture_indexes_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        transparent: Transparency = Transparency.Partial
 
+        cull_dir: Optional[str]
         for temp_model in models:
             for cull_dir in temp_model.faces.keys():
-                verts[cull_dir].append(temp_model.verts[cull_dir])
-                tverts[cull_dir].append(temp_model.texture_coords[cull_dir])
-                tint_verts[cull_dir].append(temp_model.tint_verts[cull_dir])
+                verts_src[cull_dir].append(temp_model.verts[cull_dir])
+                tverts_src[cull_dir].append(temp_model.texture_coords[cull_dir])
+                tint_verts_src[cull_dir].append(temp_model.tint_verts[cull_dir])
                 face_table = temp_model.faces[cull_dir].copy()
                 texture_index = temp_model.texture_index[cull_dir].copy()
                 face_table += vert_count[cull_dir]
                 texture_index += texture_count
-                faces[cull_dir].append(face_table)
-                texture_indexes[cull_dir].append(texture_index)
+                faces_src[cull_dir].append(face_table)
+                texture_indexes_src[cull_dir].append(texture_index)
 
                 vert_count[cull_dir] += int(
                     temp_model.verts[cull_dir].shape[0] / temp_model.face_mode
                 )
 
-            textures += temp_model.textures
+            textures_src += temp_model.textures
             texture_count += len(temp_model.textures)
             transparent = min(transparent, temp_model.is_transparent)
 
-        if textures:
-            textures, texture_index_map = numpy.unique(
-                textures, return_inverse=True, axis=0
+        if textures_src:
+            textures_, texture_index_map = numpy.unique(
+                textures_src, return_inverse=True, axis=0
             )
+            textures = tuple(textures_)
             texture_index_map = texture_index_map.astype(numpy.uint32)
-            textures = list(textures)
         else:
+            textures = ()
             texture_index_map = numpy.array([], dtype=numpy.uint8)
 
-        remove_faces = []
-        for cull_dir, face_table in faces.items():
-            if verts[cull_dir]:
-                verts[cull_dir] = numpy.concatenate(verts[cull_dir], axis=None)
-                tverts[cull_dir] = numpy.concatenate(tverts[cull_dir], axis=None)
-                tint_verts[cull_dir] = numpy.concatenate(
-                    tint_verts[cull_dir], axis=None
-                )
-            else:
-                verts[cull_dir] = numpy.zeros((0, 3), float)
-                tverts[cull_dir] = numpy.zeros((0, 2), float)
-                tint_verts[cull_dir] = numpy.zeros(0, float)
-
-            if face_table:
-                faces[cull_dir] = numpy.concatenate(face_table, axis=None)
+        verts: dict[Optional[str], numpy.ndarray] = {}
+        tverts: dict[Optional[str], numpy.ndarray] = {}
+        tint_verts: dict[Optional[str], numpy.ndarray] = {}
+        faces: dict[Optional[str], numpy.ndarray] = {}
+        texture_indexes: dict[Optional[str], numpy.ndarray] = {}
+
+        for cull_dir in FACE_KEYS:
+            if faces_src[cull_dir]:
+                faces[cull_dir] = numpy.concatenate(faces_src[cull_dir], axis=None)
                 texture_indexes[cull_dir] = texture_index_map[
-                    numpy.concatenate(texture_indexes[cull_dir], axis=None)
+                    numpy.concatenate(texture_indexes_src[cull_dir], axis=None)
                 ]
-            else:
-                remove_faces.append(cull_dir)
-
-        for cull_dir in remove_faces:
-            del faces[cull_dir]
-            del verts[cull_dir]
-            del tverts[cull_dir]
-            del texture_indexes[cull_dir]
+                if verts_src[cull_dir]:
+                    verts[cull_dir] = numpy.concatenate(verts_src[cull_dir], axis=None)
+                    tverts[cull_dir] = numpy.concatenate(
+                        tverts_src[cull_dir], axis=None
+                    )
+                    tint_verts[cull_dir] = numpy.concatenate(
+                        tint_verts_src[cull_dir], axis=None
+                    )
+                else:
+                    verts[cull_dir] = numpy.zeros((0, 3), float)
+                    tverts[cull_dir] = numpy.zeros((0, 2), float)
+                    tint_verts[cull_dir] = numpy.zeros(0, float)
 
         return cls(
             3, verts, tverts, tint_verts, faces, texture_indexes, textures, transparent
         )
 
     def __init__(
         self,
         face_width: int,
-        verts: Dict[Union[str, None], numpy.ndarray],
-        texture_coords: Dict[Union[str, None], numpy.ndarray],
-        tint_verts: Dict[Union[str, None], numpy.ndarray],
-        # normals: Dict[Union[str, None], numpy.ndarray],
-        faces: Dict[Union[str, None], numpy.ndarray],
-        texture_index: Dict[Union[str, None], numpy.ndarray],
-        textures: Tuple[str, ...],
-        transparency: int,
+        verts: dict[Optional[str], numpy.ndarray],
+        texture_coords: dict[Optional[str], numpy.ndarray],
+        tint_verts: dict[Optional[str], numpy.ndarray],
+        # normals: dict[Optional[str], numpy.ndarray],
+        faces: dict[Optional[str], numpy.ndarray],
+        texture_index: dict[Optional[str], numpy.ndarray],
+        textures: tuple[str, ...],
+        transparency: Transparency,
     ):
         """
 
         :param face_width: the number of vertices per face (3 or 4)
         :param verts: a numpy float array containing the vert data. One line per vertex
         :param texture_coords: a numpy float array containing the texture coordinate data. One line per vertex
         :param tint_verts: a numpy bool array if the vertex should have a tint applied to it. One line per vertex
@@ -169,115 +195,119 @@
             and isinstance(val, numpy.ndarray)
             and numpy.issubdtype(val.dtype, numpy.unsignedinteger)
             and val.ndim == 1
             and val.shape[0] == faces[key].shape[0] / face_width
             for key, val in texture_index.items()
         ), "The format of texture index is incorrect"
 
-        assert isinstance(textures, (list, tuple)) and all(
+        assert isinstance(textures, Iterable) and all(
             isinstance(texture, str) for texture in textures
         ), "The format of the textures is incorrect"
 
         self._face_mode = face_width
         self._verts = verts
         self._texture_coords = texture_coords
         self._tint_verts = tint_verts
-        self._vert_tables = None
+        self._vert_tables: Optional[dict[Optional[str], numpy.ndarray]] = None
 
         self._faces = faces
         self._texture_index = texture_index
         self._textures = tuple(textures)
         self._transparency = transparency
 
-        [a.setflags(write=False) for a in self._verts.values()]
-        [a.setflags(write=False) for a in self._texture_coords.values()]
-        [a.setflags(write=False) for a in self._faces.values()]
-        [a.setflags(write=False) for a in self._texture_index.values()]
+        for array in itertools.chain(
+            self._verts.values(),
+            self._texture_coords.values(),
+            self._faces.values(),
+            self._texture_index.values(),
+        ):
+            array.setflags(write=False)
 
     @property
     def face_mode(self) -> int:
         """The number of vertices per face"""
         return self._face_mode
 
     @property
-    def vert_tables(self) -> Dict[str, numpy.ndarray]:
+    def vert_tables(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary of cull dir -> the flat vert table containing vertices, texture coords and (in the future) normals"""
         if self._vert_tables is None:
             self._vert_tables = {
                 key: numpy.hstack(
                     (
                         self._verts[key].reshape(-1, self._face_mode),
                         self._texture_coords[key].reshape(-1, 2),
                         # TODO: add in face normals
                     )
                 ).ravel()
                 for key in self._verts.keys()
             }
-            [a.setflags(write=False) for a in self._vert_tables.values()]
+            for array in self._vert_tables.values():
+                array.setflags(write=False)
         return self._vert_tables
 
     @property
-    def verts(self) -> Dict[str, numpy.ndarray]:
+    def verts(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary mapping face cull direction to the vertex table for that direction.
         The vertex table is a flat numpy array who's length is a multiple of 3.
         x,y,z coordinates."""
         return self._verts
 
     @property
-    def texture_coords(self) -> Dict[str, numpy.ndarray]:
+    def texture_coords(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary mapping face cull direction to the texture coords table for that direction.
         The texture coords table is a flat numpy array who's length is a multiple of 2.
         tx, ty"""
         return self._texture_coords
 
     @property
-    def tint_verts(self) -> Dict[str, numpy.ndarray]:
+    def tint_verts(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary mapping face cull direction to the tint table for that direction.
         The tint table is a flat numpy bool array with three values per vertex.
         """
         return self._tint_verts
 
     @property
-    def faces(self) -> Dict[str, numpy.ndarray]:
+    def faces(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary mapping face cull direction to the face table for that direction.
         The face table is a flat numpy array of multiple 3 or 4 depending on face_mode.
         First 3 or 4 columns index into the verts table.
         Last column indexes into textures."""
         return self._faces
 
     @property
-    def texture_index(self) -> Dict[str, numpy.ndarray]:
+    def texture_index(self) -> dict[Optional[str], numpy.ndarray]:
         """A dictionary mapping face cull direction to the face table for that direction.
         The face table is a flat numpy array of multiple 2 indexing into textures."""
         return self._texture_index
 
     @property
-    def textures(self) -> Tuple[str, ...]:
+    def textures(self) -> tuple[str, ...]:
         """A list of all the texture paths."""
         return self._textures
 
     @property
     def is_opaque(self) -> bool:
         """
         If the model covers all surrounding blocks.
         Also takes into account texture transparency.
         """
         return not self._transparency
 
     @property
-    def is_transparent(self) -> int:
+    def is_transparent(self) -> Transparency:
         """
         The transparency mode of the block
         0 - the block is a full block with opaque textures
         1 - the block is a full block with transparent/translucent textures
         2 - the block is not a full block
         """
         return self._transparency
 
-    def rotate(self, rotx: int, roty: int) -> "BlockMesh":
+    def rotate(self, rotx: int, roty: int) -> BlockMesh:
         """Create a rotated version of this block model. Culling directions are also rotated.
         rotx and roty must be ints in the range -3 to 3 inclusive."""
         if rotx or roty and (roty, rotx) in cull_remap_all:
             cull_remap = cull_remap_all[(roty, rotx)]
             return BlockMesh(
                 self.face_mode,
                 {
@@ -314,18 +344,19 @@
                     for cull_dir in self.texture_index
                 },
                 self.textures,
                 self.is_transparent,
             )
         return self
 
-    def __eq__(self, other: "BlockMesh"):
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, BlockMesh):
+            return NotImplemented
         return (
-            isinstance(other, BlockMesh)
-            and self.face_mode == other.face_mode
+            self.face_mode == other.face_mode
             and all(
                 obj1.keys() == obj2.keys()
                 and all(numpy.array_equal(obj1[key], obj2[key]) for key in obj1.keys())
                 for obj1, obj2 in (
                     (self.verts, other.verts),
                     (self.texture_coords, other.texture_coords),
                     (self.tint_verts, other.tint_verts),
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/cube.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/cube.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Dict, Tuple, Optional
+from typing import Optional
 import numpy
 import itertools
 
-from minecraft_model_reader.api.mesh.block.block_mesh import FACE_KEYS, BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 
-BoundsType = Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]
-TextureUVType = Tuple[
-    Tuple[float, float, float, float],
-    Tuple[float, float, float, float],
-    Tuple[float, float, float, float],
-    Tuple[float, float, float, float],
-    Tuple[float, float, float, float],
-    Tuple[float, float, float, float],
+BoundsType = tuple[tuple[float, float], tuple[float, float], tuple[float, float]]
+TextureUVType = tuple[
+    tuple[float, float, float, float],
+    tuple[float, float, float, float],
+    tuple[float, float, float, float],
+    tuple[float, float, float, float],
+    tuple[float, float, float, float],
+    tuple[float, float, float, float],
 ]
 
 
 unit_box_coordinates = numpy.array(
     list(itertools.product((0, 1), (0, 1), (0, 1)))
 )  # X, Y, Z
 cube_face_lut = (
@@ -66,50 +66,50 @@
 def get_cube(
     down: str,
     up: str,
     north: str,
     east: str,
     south: str,
     west: str,
-    transparency=0,
-    tint: Tuple[int, int, int] = (1, 1, 1),
+    transparency: Transparency = Transparency.FullOpaque,
+    tint: tuple[int, int, int] = (1, 1, 1),
     bounds: BoundsType = ((0, 1), (0, 1), (0, 1)),
     texture_uv: TextureUVType = ((0, 0, 1, 1),) * 6,
-    do_not_cull: Tuple[bool, bool, bool, bool, bool, bool] = (
+    do_not_cull: tuple[bool, bool, bool, bool, bool, bool] = (
         False,
         False,
         False,
         False,
         False,
         False,
     ),
-):
+) -> BlockMesh:
     box_coordinates = numpy.array(list(itertools.product(*bounds)))
-    _texture_uv: Dict[Optional[str], numpy.ndarray] = {
+    _texture_uv: dict[Optional[str], numpy.ndarray] = {
         face: numpy.array(texture_uv[i], float) for i, face in enumerate(cube_face_lut)
     }
-    _verts: Dict[Optional[str], numpy.ndarray] = {}
-    _texture_coords: Dict[Optional[str], numpy.ndarray] = {}
-    _tint_verts: Dict[Optional[str], numpy.ndarray] = {}
-    _tri_faces: Dict[Optional[str], numpy.ndarray] = {}
+    _verts: dict[Optional[str], numpy.ndarray] = {}
+    _texture_coords: dict[Optional[str], numpy.ndarray] = {}
+    _tint_verts: dict[Optional[str], numpy.ndarray] = {}
+    _tri_faces: dict[Optional[str], numpy.ndarray] = {}
     for _face_dir in cube_face_lut:
         _verts[_face_dir] = box_coordinates[
             cube_face_lut[_face_dir]
         ].ravel()  # vertex coordinates for this face
         _texture_coords[_face_dir] = _texture_uv[_face_dir][
             uv_rotation_lut
         ]  # texture vertices
         _tint_verts[_face_dir] = numpy.full((4, 3), tint, dtype=float).ravel()
         _tri_faces[_face_dir] = tri_face
 
-    texture_paths, texture_index = numpy.unique(
+    texture_paths_arr, texture_index = numpy.unique(
         (down, up, north, east, south, west), return_inverse=True
     )
-    texture_paths = tuple(texture_paths)
-    _tri_texture_index: Dict[str, numpy.ndarray] = {
+    texture_paths = tuple(texture_paths_arr)
+    _tri_texture_index: dict[Optional[str], numpy.ndarray] = {
         side: numpy.full(2, texture_index[side_index], dtype=numpy.uint32)
         for side_index, side in enumerate(cube_face_lut)
     }
 
     if any(do_not_cull):
         do_not_cull_faces = tuple(
             face for face, not_cull in zip(cube_face_lut, do_not_cull) if not_cull
@@ -139,11 +139,11 @@
 def get_unit_cube(
     down: str,
     up: str,
     north: str,
     east: str,
     south: str,
     west: str,
-    transparency: int = 0,
-    tint: Tuple[int, int, int] = (1, 1, 1),
+    transparency: Transparency = Transparency.FullOpaque,
+    tint: tuple[int, int, int] = (1, 1, 1),
 ) -> BlockMesh:
     return get_cube(down, up, north, east, south, west, transparency, tint)
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/missing_block.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/mesh/block/missing_block.py`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/__init__.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 from minecraft_model_reader.api.resource_pack.bedrock import (
     BedrockResourcePack,
     BedrockResourcePackManager,
 )
 from .unknown_resource_pack import UnknownResourcePack
 
 
-def load_resource_pack(resource_pack_path: str):
+def load_resource_pack(resource_pack_path: str) -> BaseResourcePack:
     if JavaResourcePack.is_valid(resource_pack_path):
         return JavaResourcePack(resource_pack_path)
     elif BedrockResourcePack.is_valid(resource_pack_path):
         return BedrockResourcePack(resource_pack_path)
     else:
         return UnknownResourcePack(resource_pack_path)
 
 
 def load_resource_pack_manager(
-    resource_packs: Iterable[Union[str, BaseResourcePack]], load=True
+    resource_packs: Iterable[Union[str, BaseResourcePack]], load: bool = True
 ) -> BaseResourcePackManager:
-    resource_packs_out = []
+    resource_packs_out: list[BaseResourcePack] = []
     for resource_pack in resource_packs:
         if isinstance(resource_pack, str):
             resource_pack = load_resource_pack(resource_pack)
         if (
             not isinstance(resource_pack, UnknownResourcePack)
             and resource_pack.valid_pack
         ):
@@ -40,13 +40,23 @@
                     resource_packs_out.append(resource_pack)
             else:
                 resource_packs_out.append(resource_pack)
 
     resource_packs = resource_packs_out
     if resource_packs:
         if isinstance(resource_packs[0], JavaResourcePack):
-            return JavaResourcePackManager(resource_packs, load)
+            return JavaResourcePackManager(
+                [pack for pack in resource_packs if isinstance(pack, JavaResourcePack)],
+                load,
+            )
         elif isinstance(resource_packs[0], BedrockResourcePack):
-            return BedrockResourcePackManager(resource_packs, load)
+            return BedrockResourcePackManager(
+                [
+                    pack
+                    for pack in resource_packs
+                    if isinstance(pack, BedrockResourcePack)
+                ],
+                load,
+            )
 
     raise NotImplementedError
     # return UnknownResourcePackManager()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/resource_pack.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
     def __init__(self, root_dir: str):
         self._valid_pack = False
         self._root_dir = root_dir
         self._pack_description = ""
         self._pack_icon = default_pack_icon_path
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         raise NotImplementedError
 
     @staticmethod
-    def is_valid(pack_path: str):
+    def is_valid(pack_path: str) -> bool:
         raise NotImplementedError
 
     @property
     def valid_pack(self) -> bool:
         """bool - does the pack meet the minimum requirements to be a resource pack"""
         return self._valid_pack
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-from typing import List, Dict, Tuple, Generator, Optional
-import os
+from typing import Optional, Iterator, TypeVar, Generic
 import json
 import copy
 
 from minecraft_model_reader.api import Block, BlockMesh
 from minecraft_model_reader.api.resource_pack.base.resource_pack import BaseResourcePack
 from minecraft_model_reader.api.image import missing_no_path
 from minecraft_model_reader.api.mesh.block.missing_block import get_missing_block
 
+PackT = TypeVar("PackT", bound=BaseResourcePack)
 
-class BaseResourcePackManager:
+
+class BaseResourcePackManager(Generic[PackT]):
     """The base class that all resource pack managers must inherit from. Defines the base api."""
 
-    def __init__(self):
-        self._packs: List[BaseResourcePack] = []
-        self._missing_block = None
-        self._texture_is_transparent = {}
-        self._cached_models: Dict[Block, BlockMesh] = {}
+    def __init__(self) -> None:
+        self._packs: list[PackT] = []
+        self._missing_block: Optional[BlockMesh] = None
+        self._texture_is_transparent: dict[str, tuple[float, bool]] = {}
+        self._cached_models: dict[Block, BlockMesh] = {}
 
     @property
-    def pack_paths(self):
+    def pack_paths(self) -> list[str]:
         return [pack.root_dir for pack in self._packs]
 
-    def _unload(self):
+    def _unload(self) -> None:
         """Clear all loaded resources."""
         self._texture_is_transparent.clear()
         self._cached_models.clear()
 
-    def _load_transparency_cache(self, path: str):
+    def _load_transparency_cache(self, path: str) -> None:
         try:
             with open(path) as f:
                 self._texture_is_transparent = json.load(f)
         except:
             pass
 
-    def _load_iter(self) -> Generator[float, None, None]:
+    def _load_iter(self) -> Iterator[float]:
         """Load resources."""
         raise NotImplementedError
 
-    def reload(self) -> Generator[float, None, None]:
+    def reload(self) -> Iterator[float]:
         """Unload and reload resources"""
         self._unload()
         yield from self._load_iter()
 
     @property
     def missing_no(self) -> str:
         """The path to the missing_no image"""
@@ -51,15 +52,15 @@
     @property
     def missing_block(self) -> BlockMesh:
         if self._missing_block is None:
             self._missing_block = get_missing_block(self)
         return self._missing_block
 
     @property
-    def textures(self) -> Tuple[str, ...]:
+    def textures(self) -> tuple[str, ...]:
         """Returns a tuple of all the texture paths in the resource pack."""
         raise NotImplementedError
 
     def get_texture_path(self, namespace: Optional[str], relative_path: str) -> str:
         """Get the absolute texture path from the namespace and relative path pair"""
         raise NotImplementedError
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import importlib
 import pkgutil
-import minecraft_model_reader
 
 from .base_blockshape import BaseBlockShape
 
-BlockShapeClasses = {}
+BlockShapeClasses: dict[str, BaseBlockShape] = {}
 _class_names = set()
 
 
-def _load_blockshape(module_name: str):
+def _load_blockshape(module_name: str) -> None:
     blockshape_module = importlib.import_module(module_name)
     if hasattr(blockshape_module, "BlockShape"):
         blockshape = getattr(blockshape_module, "BlockShape")
         if isinstance(blockshape, BaseBlockShape):
             if blockshape.blockshape in BlockShapeClasses:
                 print(f"Name conflict with blockshape {blockshape.blockshape}")
             if blockshape.__class__.__name__ in _class_names:
                 print(f"Duplicate class name {blockshape.__class__.__name__}")
             else:
                 _class_names.add(blockshape.__class__.__name__)
             BlockShapeClasses[blockshape.blockshape] = blockshape
 
 
-def _load_blockshapes():
+def _load_blockshapes() -> None:
     package_prefix = __name__ + "."
 
     for _, name, _ in pkgutil.walk_packages(__path__, package_prefix):
         _load_blockshape(name)
 
 
 _load_blockshapes()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import Tuple
-
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.base_blockshape import (
     BaseBlockShape,
 )
 
 
 class Air(BaseBlockShape):
@@ -19,19 +17,19 @@
     def texture_index(self, block: Block, aux_value: int) -> int:
         """The texture index to use within the list for the given Block"""
         return 0
 
     def get_block_model(
         self,
         block: Block,
-        up: str,
         down: str,
+        up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
-        return BlockMesh(3, {}, {}, {}, {}, {}, (), 2)
+        return BlockMesh(3, {}, {}, {}, {}, {}, (), Transparency.Partial)
 
 
 BlockShape = Air()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.mesh.block import BlockMesh
 from minecraft_model_reader.api import Block
 
 
 class BaseBlockShape:
     @property
     def blockshape(self) -> str:
@@ -16,16 +14,16 @@
     def texture_index(self, block: Block, aux_value: int) -> int:
         """The texture index to use within the list for the given Block"""
         raise NotImplementedError
 
     def get_block_model(
         self,
         block: Block,
-        up: str,
         down: str,
+        up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         raise NotImplementedError
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from typing import Tuple
+from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api import Block
+from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
+import amulet_nbt
 
-from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cross_texture import (
-    Cross,
-)
-from minecraft_model_reader.api import Block, BlockMesh
 
+class Door(Cube):
+    def is_valid(self, block: Block) -> bool:
+        return isinstance(block.properties.get("upper_block_bit"), amulet_nbt.TAG_Byte)
 
-class BubbleColumn(Cross):
     @property
     def blockshape(self) -> str:
-        return "bubble_column"
+        return "door"
+
+    def texture_index(self, block: Block, aux_value: int) -> int:
+        return 0
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
+        if block.properties["upper_block_bit"].py_data:
+            return super().get_block_model(
+                block, north, north, north, north, north, north, transparency
+            )
         return super().get_block_model(
-            block, north, north, north, north, north, north, transparency
+            block, down, down, down, down, down, down, transparency
         )
 
 
-BlockShape = BubbleColumn()
+BlockShape = Door()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
-from minecraft_model_reader.api.mesh.block import BlockMesh
 import amulet_nbt
 
 
-class Cake(PartialBlock):
+class Slab(PartialBlock):
     def is_valid(self, block: Block) -> bool:
-        return isinstance(block.properties.get("bite_counter"), amulet_nbt.TAG_Int)
+        return isinstance(block.properties.get("top_slot_bit"), amulet_nbt.TAG_Byte)
 
     @property
     def blockshape(self) -> str:
-        return "cake"
+        return "slab"
+
+    def texture_index(self, block: Block, aux_value: int) -> int:
+        """The texture index to use within the list for the given Block"""
+        return aux_value % 8
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
-        return (
-            (1 / 16 + block.properties["bite_counter"].py_data * 2 / 16, 15 / 16),
-            (0, 0.5),
-            (1 / 16, 15 / 16),
-        )
-
-    def texture_index(self, block: Block, aux_value: int) -> int:
-        return min(block.properties["bite_counter"].py_data, 1)
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
+        if block.properties["top_slot_bit"].py_data:
+            return (0, 1), (1 / 2, 1), (0, 1)
+        else:
+            return (0, 1), (0, 1 / 2), (0, 1)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
-        return False, True, True, True, True, True
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
+        return False, True, False, False, False, False
 
 
-BlockShape = Cake()
+BlockShape = Slab()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Any
 
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.mesh.block import BlockMesh
 
@@ -10,35 +10,37 @@
 class Chest(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "chest"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (1 / 16, 15 / 16), (0, 14 / 16), (1 / 16, 15 / 16)
 
     def texture_index(self, block: Block, aux_value: int) -> int:
         return 0
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, True, True, True, True
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
-        modify_uv=True,
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        modify_uv: bool = True,
+        *args: Any,
+        **kwargs: Any
     ) -> BlockMesh:
         rotation = {2: 2, 3: 0, 4: 1, 5: 3}.get(
             block.properties["facing_direction"].py_data, 0
         )
 
         return (
             super()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Any
 
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.mesh.block import BlockMesh
 import amulet_nbt
@@ -17,31 +17,33 @@
         return "comparator"
 
     def texture_index(self, block: Block, aux_value: int) -> int:
         return (aux_value >> 3) & 1
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (0, 1), (0, 2 / 16), (0, 1)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, False, False, False, False
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        *args: Any,
+        **kwargs: Any
     ) -> BlockMesh:
         return (
             super()
             .get_block_model(block, down, up, north, east, south, west, transparency)
             .rotate(0, block.properties["direction"].py_data)
         )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Tuple
 import numpy
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.base_blockshape import (
     BaseBlockShape,
 )
 
 
 class Cross(BaseBlockShape):
@@ -18,27 +17,27 @@
         return True
 
     def texture_index(self, block: Block, aux_value: int) -> int:
         """The texture index to use within the list for the given Block"""
         return aux_value % 16
 
     @property
-    def tint(self) -> Tuple[float, float, float]:
+    def tint(self) -> tuple[float, float, float]:
         return 1, 1, 1
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         return BlockMesh(
             3,
             {
                 None: numpy.array(
                     [
                         0.0625,
@@ -176,12 +175,12 @@
                         0,
                         0,
                     ],
                     numpy.uint32,
                 )
             },
             (up,),
-            2,
+            Transparency.Partial,
         )
 
 
 BlockShape = Cross()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-from typing import Tuple
+from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.flat_wall import (
+    FlatWall,
+)
+from minecraft_model_reader.api import Block, BlockMesh
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
-from minecraft_model_reader.api import Block
-from minecraft_model_reader.api.mesh.block.cube import get_unit_cube
-from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.default import Default
 
-
-class Cube(Default):
+class Ladder(FlatWall):
     @property
     def blockshape(self) -> str:
-        return "cube"
+        return "ladder"
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        modify_uv: bool = True,
     ) -> BlockMesh:
-        return get_unit_cube(down, up, north, east, south, west, int(any(transparency)))
+        rotation = {2: 2, 3: 0, 4: 1, 5: 3}.get(
+            block.properties["facing_direction"].py_data, 0
+        )
+
+        return (
+            super()
+            .get_block_model(block, down, up, north, east, south, west, transparency)
+            .rotate(0, rotation)
+        )
 
 
-BlockShape = Cube()
+BlockShape = Ladder()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.mesh.block import BlockMesh
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.mesh.block.cube import get_unit_cube
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.base_blockshape import (
     BaseBlockShape,
 )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from typing import Tuple, Dict
-
 from minecraft_model_reader.api.mesh.block import BlockMesh
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
 import amulet_nbt
 
 
-class Door(Cube):
+class Tree(Cube):
     def is_valid(self, block: Block) -> bool:
-        return isinstance(block.properties.get("upper_block_bit"), amulet_nbt.TAG_Byte)
+        return isinstance(block.properties.get("pillar_axis"), amulet_nbt.TAG_String)
 
     @property
     def blockshape(self) -> str:
-        return "door"
+        return "tree"
 
     def texture_index(self, block: Block, aux_value: int) -> int:
-        return 0
+        return aux_value % 4
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
-        if block.properties["upper_block_bit"].py_data:
-            return super().get_block_model(
-                block, north, north, north, north, north, north, transparency
-            )
-        return super().get_block_model(
-            block, down, down, down, down, down, down, transparency
+        axis: str = block.properties["pillar_axis"].py_data
+
+        model = super().get_block_model(
+            block, down, up, north, east, south, west, transparency
         )
+        if axis == "x":
+            return model.rotate(1, 1)
+        elif axis == "z":
+            return model.rotate(1, 2)
+        return model
 
 
-BlockShape = Door()
+BlockShape = Tree()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cross_texture import (
     Cross,
 )
 from minecraft_model_reader.api import Block, BlockMesh
 import amulet_nbt
 
 
@@ -23,15 +21,15 @@
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         if block.properties["upper_block_bit"].py_data:
             return super().get_block_model(block, up, up, up, up, up, up, transparency)
         else:
             return super().get_block_model(
                 block, down, down, down, down, down, down, transparency
             )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 
 
 class EnchantingTable(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "enchanting_table"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (0, 1), (0, 12 / 16), (0, 1)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, False, False, False, False
 
 
 BlockShape = EnchantingTable()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 
 
 class FarmLand(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "farmland"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (0, 1), (0, 15 / 16), (0, 1)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, False, False, False, False
 
 
 BlockShape = FarmLand()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 
 
 class Fence(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "fence"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (6 / 16, 1 - 6 / 16), (0, 1), (6 / 16, 1 - 6 / 16)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, False, True, True, True, True
 
 
 BlockShape = Fence()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from typing import Tuple
 import numpy
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.default import Default
 
 
 class Flat(Default):
     @property
-    def tint(self) -> Tuple[float, float, float]:
+    def tint(self) -> tuple[float, float, float]:
         return 1, 1, 1
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         return BlockMesh(
             3,
             {
                 None: numpy.array(
                     [
                         0.0,
@@ -48,9 +47,9 @@
                     [0.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0, 0.0], numpy.float32
                 )
             },
             {None: numpy.array(self.tint * 4, numpy.float32)},
             {None: numpy.array([0, 1, 2, 0, 2, 3], numpy.uint32)},
             {None: numpy.array([0, 0], numpy.uint32)},
             (up,),
-            2,
+            Transparency.Partial,
         )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from typing import Tuple
 import numpy
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.default import Default
 
 
 class FlatWall(Default):
     @property
-    def tint(self) -> Tuple[float, float, float]:
+    def tint(self) -> tuple[float, float, float]:
         return 1, 1, 1
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         return BlockMesh(
             3,
             {
                 None: numpy.array(
                     [
                         0.0,
@@ -48,9 +47,9 @@
                     [0.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0, 0.0], numpy.float32
                 )
             },
             {None: numpy.array(self.tint * 4, numpy.float32)},
             {None: numpy.array([0, 1, 2, 0, 2, 3], numpy.uint32)},
             {None: numpy.array([0, 0], numpy.uint32)},
             (up,),
-            2,
+            Transparency.Partial,
         )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple, Dict
-
 from minecraft_model_reader.api.mesh.block import BlockMesh
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
 import amulet_nbt
 
 
 class Furnace(Cube):
@@ -14,27 +12,27 @@
     def blockshape(self) -> str:
         return "furnace"
 
     def texture_index(self, block: Block, aux_value: int) -> int:
         return 0
 
     @property
-    def rotation_map(self) -> Dict[int, int]:
+    def rotation_map(self) -> dict[int, int]:
         return {2: 2, 3: 0, 4: 1, 5: 3}
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         rotation = self.rotation_map.get(
             block.properties["facing_direction"].py_data, 0
         )
 
         return (
             super()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from typing import Tuple
-
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.mesh.block.cube import get_unit_cube
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
 
 
-class GreenCube(Cube):
+class Water(Cube):
     @property
     def blockshape(self) -> str:
-        return "greencube"
+        return "water"
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
         return get_unit_cube(
-            down, up, north, east, south, west, int(any(transparency)), (0, 1, 0)
+            down,
+            down,
+            down,
+            down,
+            down,
+            down,
+            (
+                Transparency.FullTranslucent
+                if transparency[0]
+                else Transparency.FullOpaque
+            ),
         )
 
 
-BlockShape = GreenCube()
+BlockShape = Water()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-from typing import Tuple
+from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api import Block
+from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
+import amulet_nbt
 
-from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.flat_wall import (
-    FlatWall,
-)
-from minecraft_model_reader.api import Block, BlockMesh
 
+class Piston(Cube):
+    def is_valid(self, block: Block) -> bool:
+        return isinstance(block.properties.get("facing_direction"), amulet_nbt.TAG_Int)
 
-class Ladder(FlatWall):
     @property
     def blockshape(self) -> str:
-        return "ladder"
+        return "piston"
+
+    def texture_index(self, block: Block, aux_value: int) -> int:
+        return 0
+
+    @property
+    def rotation_map(self) -> dict[int, tuple[int, int]]:
+        return {0: (2, 0), 1: (0, 0), 2: (1, 2), 3: (1, 0), 4: (1, 1), 5: (1, 3)}
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
-        modify_uv=True,
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
-        rotation = {2: 2, 3: 0, 4: 1, 5: 3}.get(
-            block.properties["facing_direction"].py_data, 0
+        rotation = self.rotation_map.get(
+            block.properties["facing_direction"].py_data, (0, 0)
         )
 
         return (
             super()
             .get_block_model(block, down, up, north, east, south, west, transparency)
-            .rotate(0, rotation)
+            .rotate(*rotation)
         )
 
 
-BlockShape = Ladder()
+BlockShape = Piston()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Tuple
+from typing import Optional
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, Transparency
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.mesh.block.cube import get_cube
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.default import Default
 
-BoundsType = Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]
-DoNotCullType = Tuple[bool, bool, bool, bool, bool, bool]
+BoundsType = tuple[tuple[float, float], tuple[float, float], tuple[float, float]]
+DoNotCullType = tuple[bool, bool, bool, bool, bool, bool]
 
 
 class PartialBlock(Default):
     def bounds(self, block: Block) -> BoundsType:
         return (0, 1), (0, 1), (0, 1)
 
     @property
@@ -22,18 +22,18 @@
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
-        modify_uv=True,
-        bounds: BoundsType = None,
-        do_not_cull: DoNotCullType = None,
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        modify_uv: bool = True,
+        bounds: Optional[BoundsType] = None,
+        do_not_cull: Optional[DoNotCullType] = None,
     ) -> BlockMesh:
         bounds = bounds or self.bounds(block)
         if modify_uv:
             uv = (
                 (bounds[0][0], bounds[2][0], bounds[0][1], bounds[2][1]),
                 (bounds[0][0], bounds[2][0], bounds[0][1], bounds[2][1]),
                 (bounds[0][0], 1 - bounds[1][1], bounds[0][1], 1 - bounds[1][0]),
@@ -46,12 +46,12 @@
         return get_cube(
             down,
             up,
             north,
             east,
             south,
             west,
-            2,
+            Transparency.Partial,
             bounds=bounds,
             texture_uv=uv,
             do_not_cull=do_not_cull or self.do_not_cull,
         )
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-from typing import Tuple, Dict
-
-from minecraft_model_reader.api.mesh.block import BlockMesh
-from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
+from minecraft_model_reader.api import Block, BlockMesh
 import amulet_nbt
 
 
-class Piston(Cube):
+class Pumpkin(Cube):
     def is_valid(self, block: Block) -> bool:
-        return isinstance(block.properties.get("facing_direction"), amulet_nbt.TAG_Int)
+        return isinstance(block.properties.get("direction"), amulet_nbt.TAG_Int)
 
     @property
     def blockshape(self) -> str:
-        return "piston"
+        return "pumpkin"
 
     def texture_index(self, block: Block, aux_value: int) -> int:
-        return 0
-
-    @property
-    def rotation_map(self) -> Dict[int, Tuple[int, int]]:
-        return {0: (2, 0), 1: (0, 0), 2: (1, 2), 3: (1, 0), 4: (1, 1), 5: (1, 3)}
+        return 2
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
-        rotation = self.rotation_map.get(
-            block.properties["facing_direction"].py_data, (0, 0)
-        )
-
         return (
             super()
             .get_block_model(block, down, up, north, east, south, west, transparency)
-            .rotate(*rotation)
+            .rotate(0, block.properties["direction"].py_data)
         )
 
 
-BlockShape = Piston()
+BlockShape = Pumpkin()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Tuple, Dict
-
+from typing import Any
 from minecraft_model_reader.api.mesh.block import BlockMesh
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 import amulet_nbt
 
@@ -16,27 +15,29 @@
     def blockshape(self) -> str:
         return "piston_arm"
 
     def texture_index(self, block: Block, aux_value: int) -> int:
         return 0
 
     @property
-    def rotation_map(self) -> Dict[int, Tuple[int, int]]:
+    def rotation_map(self) -> dict[int, tuple[int, int]]:
         return {0: (2, 0), 1: (0, 0), 2: (1, 2), 3: (1, 0), 4: (1, 1), 5: (1, 3)}
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        *args: Any,
+        **kwargs: Any
     ) -> BlockMesh:
         rotation = self.rotation_map.get(
             block.properties["facing_direction"].py_data, (0, 0)
         )
 
         return BlockMesh.merge(
             [
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 
 
 class PortalFrame(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "portal_frame"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (0, 1), (0, 13 / 16), (0, 1)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, False, False, False, False
 
 
 BlockShape = PortalFrame()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 import amulet_nbt
 
 
@@ -13,19 +11,19 @@
 
     @property
     def blockshape(self) -> str:
         return "pressure_plate"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         if block.properties["redstone_signal"].py_data >= 1:
             return (1 / 16, 15 / 16), (0, 1 / 32), (1 / 16, 15 / 16)
         else:
             return (1 / 16, 15 / 16), (0, 1 / 16), (1 / 16, 15 / 16)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, True, True, True, True, True
 
 
 BlockShape = PressurePlate()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from typing import Tuple
-
-from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
-    PartialBlock,
+from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.flat_wall import (
+    FlatWall,
 )
-from minecraft_model_reader.api import Block
-from minecraft_model_reader.api.mesh.block import BlockMesh
+from minecraft_model_reader.api import Block, BlockMesh
 import amulet_nbt
 
 
-class Repeater(PartialBlock):
+class Vine(FlatWall):
     def is_valid(self, block: Block) -> bool:
-        return isinstance(block.properties.get("direction"), amulet_nbt.TAG_Int)
+        return isinstance(
+            block.properties.get("vine_direction_bits"), amulet_nbt.TAG_Int
+        )
 
     @property
     def blockshape(self) -> str:
-        return "repeater"
-
-    def texture_index(self, block: Block, aux_value: int) -> int:
-        if block.base_name == "powered_repeater":
-            return 1
-        else:
-            return 0
-
-    def bounds(
-        self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
-        return (0, 1), (0, 2 / 16), (0, 1)
+        return "vine"
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
-        return False, True, False, False, False, False
+    def tint(self) -> tuple[float, float, float]:
+        return 0, 1, 0
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
+        modify_uv: bool = True,
     ) -> BlockMesh:
-        return (
-            super()
-            .get_block_model(block, down, up, north, east, south, west, transparency)
-            .rotate(0, block.properties["direction"].py_data)
-        )
+        models = []
+        data: int = block.properties["vine_direction_bits"].py_data
+        if data:
+            model = super().get_block_model(
+                block, down, up, north, east, south, west, transparency
+            )
+            if data & 1:
+                models.append(model.rotate(0, 2))
+            if data & 2:
+                models.append(model.rotate(0, 3))
+            if data & 4:
+                models.append(model.rotate(0, 0))
+            if data & 8:
+                models.append(model.rotate(0, 1))
+        return BlockMesh.merge(models)
 
 
-BlockShape = Repeater()
+BlockShape = Vine()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,28 @@
-from typing import Tuple, Dict
+from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cross_texture import (
+    Cross,
+)
+from minecraft_model_reader.api import Block, BlockMesh
 
-from minecraft_model_reader.api.mesh.block import BlockMesh
-from minecraft_model_reader.api import Block
-from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.cube import Cube
-import amulet_nbt
-
-
-class Tree(Cube):
-    def is_valid(self, block: Block) -> bool:
-        return isinstance(block.properties.get("pillar_axis"), amulet_nbt.TAG_String)
 
+class BubbleColumn(Cross):
     @property
     def blockshape(self) -> str:
-        return "tree"
-
-    def texture_index(self, block: Block, aux_value: int) -> int:
-        return aux_value % 4
+        return "bubble_column"
 
     def get_block_model(
         self,
         block: Block,
         down: str,
         up: str,
         north: str,
         east: str,
         south: str,
         west: str,
-        transparency: Tuple[bool, bool, bool, bool, bool, bool],
+        transparency: tuple[bool, bool, bool, bool, bool, bool],
     ) -> BlockMesh:
-        axis: str = block.properties["pillar_axis"].py_data
-
-        model = super().get_block_model(
-            block, down, up, north, east, south, west, transparency
+        return super().get_block_model(
+            block, north, north, north, north, north, north, transparency
         )
-        if axis == "x":
-            return model.rotate(1, 1)
-        elif axis == "z":
-            return model.rotate(1, 2)
-        return model
 
 
-BlockShape = Tree()
+BlockShape = BubbleColumn()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from minecraft_model_reader.api.resource_pack.bedrock.blockshapes.partial_block import (
     PartialBlock,
 )
 from minecraft_model_reader.api import Block
 
 
 class Wall(PartialBlock):
     @property
     def blockshape(self) -> str:
         return "wall"
 
     def bounds(
         self, block: Block
-    ) -> Tuple[Tuple[float, float], Tuple[float, float], Tuple[float, float]]:
+    ) -> tuple[tuple[float, float], tuple[float, float], tuple[float, float]]:
         return (4 / 16, 12 / 16), (0, 1), (4 / 16, 12 / 16)
 
     @property
-    def do_not_cull(self) -> Tuple[bool, bool, bool, bool, bool, bool]:
+    def do_not_cull(self) -> tuple[bool, bool, bool, bool, bool, bool]:
         return False, False, True, True, True, True
 
 
 BlockShape = Wall()
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 
 # import shutil
 # import zipfile
 # import json
 # from urllib.request import urlopen
 # import io
-from typing import Generator, Optional
+from typing import Generator, Optional, TypeVar, Any
 import logging
 
 from minecraft_model_reader.api.resource_pack import BedrockResourcePack
 
+T = TypeVar("T")
+
 log = logging.getLogger(__name__)
 
 
-def generator_unpacker(gen: Generator):
+def generator_unpacker(gen: Generator[Any, Any, T]) -> T:
     try:
         while True:
             next(gen)
     except StopIteration as e:
-        return e.value
+        return e.value  # type: ignore
 
 
 def get_latest() -> BedrockResourcePack:
     return generator_unpacker(get_latest_iter())
 
 
 def get_latest_iter() -> Generator[float, None, BedrockResourcePack]:
@@ -63,15 +65,15 @@
     if _bedrock_vanilla_fix is None:
         _bedrock_vanilla_fix = BedrockResourcePack(
             os.path.join(os.path.dirname(__file__), "bedrock_vanilla_fix")
         )
     return _bedrock_vanilla_fix
 
 
-def get_bedrock_vanilla_latest():
+def get_bedrock_vanilla_latest() -> BedrockResourcePack:
     global _bedrock_vanilla_latest
     if _bedrock_vanilla_latest is None:
         _bedrock_vanilla_latest = get_latest()
     return _bedrock_vanilla_latest
 
 
 def get_bedrock_vanilla_latest_iter() -> Generator[float, None, BedrockResourcePack]:
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 import json
 
 from minecraft_model_reader.api.resource_pack.base import BaseResourcePack
 from minecraft_model_reader.api import comment_json
 
 
 class BedrockResourcePack(BaseResourcePack):
-    """A class to hold the bare bones information about the resource pack.
+    """A class to hold the bare-bones information about the resource pack.
     Holds the pack format, description and if the pack is valid.
     This information can be used in a viewer to display the packs to the user."""
 
     def __init__(self, resource_pack_path: str):
         super().__init__(resource_pack_path)
         meta_path = os.path.join(resource_pack_path, "manifest.json")
         if os.path.isfile(meta_path):
             try:
                 with open(meta_path) as f:
                     pack_mcmeta = comment_json.load(f)
             except json.JSONDecodeError:
                 pass
             else:
-                if "header" in pack_mcmeta and "description" in pack_mcmeta["header"]:
-                    self._pack_description = str(pack_mcmeta["header"]["description"])
-                    self._valid_pack = True
+                if isinstance(pack_mcmeta, dict):
+                    header = pack_mcmeta.get("header", None)
+                    if isinstance(header, dict):
+                        description = header.get("description", None)
+                        if isinstance(description, str):
+                            self._pack_description = description
+                            self._valid_pack = True
 
         pack_icon_path = os.path.join(resource_pack_path, "pack_icon.png")
         if os.path.isfile(pack_icon_path):
             self._pack_icon = pack_icon_path
 
     @staticmethod
-    def is_valid(pack_path: str):
+    def is_valid(pack_path: str) -> bool:
         return os.path.isfile(os.path.join(pack_path, "manifest.json"))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"BedrockResourcePack({self._root_dir})"
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,64 @@
 import os
 import json
-from typing import Union, Dict, Tuple, Iterable, Generator, Optional
+from typing import Union, Iterable, Generator, Optional, TypedDict, Literal, Any
 from PIL import Image
 import numpy
 
 from minecraft_model_reader.api import Block, comment_json
 from minecraft_model_reader.api.resource_pack import BaseResourcePackManager
 from minecraft_model_reader.api.resource_pack.bedrock import BedrockResourcePack
 from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh
 from .blockshapes import BlockShapeClasses
 
 
-def _load_data() -> Tuple[
-    Dict[str, str],
-    Dict[
+class NumericalProperty(TypedDict):
+    name: str
+    type: Union[Literal["byte"], Literal["int"]]
+    value: int
+
+
+class StrProperty(TypedDict):
+    name: str
+    type: Literal["string"]
+    value: str
+
+
+class StateDict(TypedDict):
+    name: str
+    data: int
+    states: list[Union[NumericalProperty, StrProperty]]
+
+
+class BlockPaletteDict(TypedDict):
+    blocks: list[StateDict]
+
+
+def _load_data() -> tuple[
+    dict[str, str],
+    dict[
         str,
-        Tuple[Tuple[Tuple[str, str], ...], Dict[Tuple[Union[str, int], ...], int]],
+        tuple[
+            tuple[tuple[str, Union[int, str]], ...],
+            dict[tuple[Union[str, int], ...], int],
+        ],
     ],
 ]:
     with open(os.path.join(os.path.dirname(__file__), "blockshapes.json")) as f:
-        _block_shapes = comment_json.load(f)
+        _block_shapes: dict[str, str] = comment_json.load(f)  # type: ignore
 
-    _aux_values = {}
+    _aux_values: dict[
+        str,
+        tuple[
+            tuple[tuple[str, Union[int, str]], ...],
+            dict[tuple[Union[str, int], ...], int],
+        ],
+    ] = {}
     with open(os.path.join(os.path.dirname(__file__), "block_palette.json")) as f:
-        _block_palette = comment_json.load(f)
+        _block_palette: BlockPaletteDict = comment_json.load(f)  # type: ignore
     for block in _block_palette["blocks"]:
         data = block["data"]
         name = block["name"]
         if name not in _aux_values:
             _aux_values[name] = (
                 tuple((state["name"], state["value"]) for state in block["states"]),
                 {},
@@ -61,42 +92,42 @@
 class BedrockResourcePackManager(BaseResourcePackManager):
     """A class to load and handle the data from the packs.
     Packs are given as a list with the later packs overwriting the earlier ones."""
 
     def __init__(
         self,
         resource_packs: Union[BedrockResourcePack, Iterable[BedrockResourcePack]],
-        load=True,
-    ):
+        load: bool = True,
+    ) -> None:
         super().__init__()
-        self._block_shapes: Dict[str, str] = {}  # block string to block shape
-        self._blocks: Dict[str, Union[Dict[str, str], str, None]] = (
+        self._block_shapes: dict[str, str] = {}  # block string to block shape
+        self._blocks: dict[str, Union[dict[str, str], str, None]] = (
             {}
         )  # block string to short texture ids
-        self._terrain_texture: Dict[str, Tuple[str, ...]] = (
+        self._terrain_texture: dict[str, tuple[str, ...]] = (
             {}
         )  # texture ids to list of relative paths. Each relates to a different data value.
-        self._textures: Dict[str, str] = {}  # relative path to texture path
+        self._textures: dict[str, str] = {}  # relative path to texture path
         self._all_textures = None
 
-        self._texture_is_transparent: Dict[str, Tuple[int, bool]] = {}
+        self._texture_is_transparent: dict[str, tuple[float, bool]] = {}
 
         if isinstance(resource_packs, (list, tuple)):
             self._packs = [
                 rp for rp in resource_packs if isinstance(rp, BedrockResourcePack)
             ]
         elif isinstance(resource_packs, BedrockResourcePack):
             self._packs = [resource_packs]
         else:
             raise Exception(f"Invalid format {resource_packs}")
         if load:
             for _ in self.reload():
                 pass
 
-    def _unload(self):
+    def _unload(self) -> None:
         """Clear all loaded resources."""
         super()._unload()
         self._block_shapes.clear()
         self._blocks.clear()
         self._terrain_texture.clear()
         self._textures.clear()
         self._all_textures = None
@@ -105,26 +136,26 @@
         if os.path.isfile(texture_path + ".png"):
             texture_path += ".png"
         elif os.path.isfile(texture_path + ".tga"):
             texture_path += ".tga"
         else:
             texture_path = self.missing_no
         if (
-            os.stat(texture_path)[8]
+            os.stat(texture_path).st_mtime
             != self._texture_is_transparent.get(texture_path, [0])[0]
         ):
             im: Image.Image = Image.open(texture_path)
             if im.mode == "RGBA":
                 alpha = numpy.array(im.getchannel("A").getdata())
-                texture_is_transparent = numpy.any(alpha != 255)
+                texture_is_transparent = bool(numpy.any(alpha != 255))
             else:
                 texture_is_transparent = False
 
             self._texture_is_transparent[texture_path] = (
-                os.stat(texture_path)[8],
+                os.stat(texture_path).st_mtime,
                 bool(texture_is_transparent),
             )
         return texture_path
 
     def _load_iter(self) -> Generator[float, None, None]:
         self._block_shapes.update(BlockShapes)  # add the default block shapes
 
@@ -159,28 +190,31 @@
                             isinstance(terrain_texture, dict)
                             and "texture_data" in terrain_texture
                             and isinstance(terrain_texture["texture_data"], dict)
                         ):
                             sub_progress = pack_progress
                             image_count = len(terrain_texture["texture_data"])
 
-                            def get_texture(_relative_path):
+                            def get_texture(_relative_path: Any) -> str:
                                 if isinstance(_relative_path, dict):
                                     _relative_path = _relative_path.get(
                                         "path", "misssingno"
                                     )
+                                    assert isinstance(_relative_path, str)
                                 if isinstance(_relative_path, str):
                                     full_path = self._check_texture(
                                         os.path.join(pack.root_dir, _relative_path)
                                     )
                                     if _relative_path in self._textures:
                                         if full_path != self.missing_no:
                                             self._textures[_relative_path] = full_path
                                     else:
                                         self._textures[_relative_path] = full_path
+                                else:
+                                    raise TypeError
                                 return _relative_path
 
                             for image_index, (texture_id, data) in enumerate(
                                 terrain_texture["texture_data"].items()
                             ):
                                 if (
                                     isinstance(texture_id, str)
@@ -214,26 +248,35 @@
                             model_count = len(blocks)
                             for model_index, (block_id, data) in enumerate(
                                 blocks.items()
                             ):
                                 if isinstance(block_id, str) and isinstance(data, dict):
                                     if ":" not in block_id:
                                         block_id = "minecraft:" + block_id
-                                    self._blocks[block_id] = data.get("textures")
+                                    textures = data.get("textures")
+                                    if textures is None or isinstance(textures, str):
+                                        self._blocks[block_id] = textures
+                                    elif isinstance(textures, dict) and all(
+                                        isinstance(v, str) for v in textures.values()
+                                    ):
+                                        self._blocks[block_id] = textures  # type: ignore  # TODO: improve this with TypeGuard
+                                    else:
+                                        raise TypeError
+
                                 yield sub_progress + (model_index) / (
                                     model_count * pack_count * 2
                                 )
             yield pack_progress + 1
 
         os.makedirs(os.path.dirname(transparency_cache_path), exist_ok=True)
         with open(transparency_cache_path, "w") as f:
             json.dump(self._texture_is_transparent, f)
 
     @property
-    def textures(self) -> Tuple[str, ...]:
+    def textures(self) -> tuple[str, ...]:
         """Returns a tuple of all the texture paths in the resource pack."""
         return tuple(self._textures.values())
 
     def get_texture_path(self, namespace: Optional[str], relative_path: str) -> str:
         """Get the absolute texture path from the namespace and relative path pair"""
         if relative_path in self._textures:
             return self._textures[relative_path]
@@ -304,14 +347,14 @@
 
             return block_shape_class.get_block_model(
                 block, down, up, north, east, south, west, transparent
             )
 
         return self.missing_block
 
-    def _get_texture(self, texture_id: str, index: int):
+    def _get_texture(self, texture_id: str, index: int) -> str:
         texture = self.missing_no
         if texture_id in self._terrain_texture:
             texture_list = self._terrain_texture[texture_id]
             if len(texture_list) > index:
                 texture = self.get_texture_path(None, texture_list[index])
         return texture
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/download_resources.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/download_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import shutil
 import zipfile
 import json
 from urllib.request import urlopen, Request
 import io
-from typing import Generator, List
+from typing import Generator, TypeVar, Any, Optional
 import logging
 
 from minecraft_model_reader.api.resource_pack import JavaResourcePack
 
+T = TypeVar("T")
+
 log = logging.getLogger(__name__)
 
-launcher_manifest = None
+launcher_manifest: Optional[dict] = None
 INCLUDE_SNAPSHOT = False
 
 
 def get_launcher_manifest() -> dict:
     global launcher_manifest
     if launcher_manifest is None:
         log.info("Downloading java launcher manifest file.")
@@ -23,20 +25,20 @@
             "https://launchermeta.mojang.com/mc/game/version_manifest.json", timeout=20
         ) as manifest:
             launcher_manifest = json.load(manifest)
         log.info("Finished downloading java launcher manifest file.")
     return launcher_manifest
 
 
-def generator_unpacker(gen: Generator):
+def generator_unpacker(gen: Generator[Any, Any, T]) -> T:
     try:
         while True:
             next(gen)
     except StopIteration as e:
-        return e.value
+        return e.value  # type: ignore
 
 
 def get_latest() -> JavaResourcePack:
     return generator_unpacker(get_latest_iter())
 
 
 def get_latest_iter() -> Generator[float, None, JavaResourcePack]:
@@ -69,47 +71,47 @@
             has_new_pack = old_version == new_version
 
         if not has_new_pack:
             yield from _remove_and_download_iter(vanilla_rp_path, new_version)
     return JavaResourcePack(vanilla_rp_path)
 
 
-_java_vanilla_fix = None
-_java_vanilla_latest = None
+_java_vanilla_fix: Optional[JavaResourcePack] = None
+_java_vanilla_latest: Optional[JavaResourcePack] = None
 
 
-def get_java_vanilla_fix():
+def get_java_vanilla_fix() -> JavaResourcePack:
     global _java_vanilla_fix
     if _java_vanilla_fix is None:
         _java_vanilla_fix = JavaResourcePack(
             os.path.join(os.path.dirname(__file__), "java_vanilla_fix")
         )
     return _java_vanilla_fix
 
 
-def get_java_vanilla_latest():
+def get_java_vanilla_latest() -> JavaResourcePack:
     global _java_vanilla_latest
     if _java_vanilla_latest is None:
         _java_vanilla_latest = get_latest()
     return _java_vanilla_latest
 
 
 def get_java_vanilla_latest_iter() -> Generator[float, None, JavaResourcePack]:
     global _java_vanilla_latest
     if _java_vanilla_latest is None:
         _java_vanilla_latest = yield from get_latest_iter()
     return _java_vanilla_latest
 
 
-def _remove_and_download(path, version):
+def _remove_and_download(path: str, version: str) -> None:
     for _ in _remove_and_download_iter(path, version):
         pass
 
 
-def _remove_and_download_iter(path, version) -> Generator[float, None, None]:
+def _remove_and_download_iter(path: str, version: str) -> Generator[float, None, None]:
     # try downloading the new resources to a temporary location
     temp_path = os.path.join(os.path.dirname(path), "_temp_")
     # clear the temporary location
     if os.path.isfile(temp_path):
         os.remove(temp_path)
     elif os.path.isdir(temp_path):
         shutil.rmtree(temp_path, ignore_errors=True)
@@ -144,20 +146,20 @@
         if content_length == content_length_found:
             break
     else:
         raise RuntimeError(f"Failed to download")
     return b"".join(content)
 
 
-def download_resources(path, version):
+def download_resources(path: str, version: str) -> None:
     generator_unpacker(download_resources_iter(path, version))
 
 
 def download_resources_iter(
-    path, version, chunk_size=4096
+    path: str, version: str, chunk_size: int = 4096
 ) -> Generator[float, None, None]:
     log.info(f"Downloading Java resource pack for version {version}")
     version_url = next(
         (v["url"] for v in get_launcher_manifest()["versions"] if v["id"] == version),
         None,
     )
     if version_url is None:
@@ -172,15 +174,15 @@
         try:
             while True:
                 yield next(downloader) / 2
         except StopIteration as e:
             data = e.value
 
         client = zipfile.ZipFile(io.BytesIO(data))
-        paths: List[str] = [
+        paths: list[str] = [
             fpath for fpath in client.namelist() if fpath.startswith("assets/")
         ]
         path_count = len(paths)
         for path_index, fpath in enumerate(paths):
             if not path_index % 30:
                 yield path_index / (path_count * 2) + 0.5
             if fpath.endswith("/"):
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/resource_pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
                         self._valid_pack = True
 
         pack_icon_path = os.path.join(resource_pack_path, "pack.png")
         if os.path.isfile(pack_icon_path):
             self._pack_icon = pack_icon_path
 
     @staticmethod
-    def is_valid(pack_path: str):
+    def is_valid(pack_path: str) -> bool:
         return os.path.isfile(os.path.join(pack_path, "pack.mcmeta"))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"JavaResourcePack({self._root_dir})"
 
     @property
     def pack_format(self) -> int:
         """int - pack format number"""
         return self._pack_format
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py` & `minecraft_resource_pack-1.4.3/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import os
 import json
 import copy
-from typing import Union, Dict, Tuple, Iterable, Generator
+from typing import Union, Iterable, Iterator, Optional
 from PIL import Image
 import numpy
 import glob
 import itertools
 import logging
 
 import amulet_nbt
 
 from minecraft_model_reader.api import Block
 from minecraft_model_reader.api.resource_pack import BaseResourcePackManager
 from minecraft_model_reader.api.resource_pack.java import JavaResourcePack
-from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh, FACE_KEYS
+from minecraft_model_reader.api.mesh.block.block_mesh import (
+    BlockMesh,
+    FACE_KEYS,
+    Transparency,
+)
 from minecraft_model_reader.api.mesh.util import rotate_3d
 from minecraft_model_reader.api.mesh.block.cube import (
     cube_face_lut,
     uv_rotation_lut,
     tri_face,
 )
 
@@ -32,51 +36,49 @@
     "gui",
     "map",
     "mob_effect",
     "particle",
 }
 
 
-class JavaResourcePackManager(BaseResourcePackManager):
+class JavaResourcePackManager(BaseResourcePackManager[JavaResourcePack]):
     """A class to load and handle the data from the packs.
     Packs are given as a list with the later packs overwriting the earlier ones."""
 
     def __init__(
         self,
         resource_packs: Union[JavaResourcePack, Iterable[JavaResourcePack]],
-        load=True,
-    ):
+        load: bool = True,
+    ) -> None:
         super().__init__()
-        self._blockstate_files: Dict[Tuple[str, str], dict] = {}
-        self._textures: Dict[Tuple[str, str], str] = {}
-        self._texture_is_transparent: Dict[str, Tuple[int, bool]] = {}
-        self._model_files: Dict[Tuple[str, str], dict] = {}
-        if isinstance(resource_packs, (list, tuple)):
-            self._packs = [
-                rp for rp in resource_packs if isinstance(rp, JavaResourcePack)
-            ]
+        self._blockstate_files: dict[tuple[str, str], dict] = {}
+        self._textures: dict[tuple[str, str], str] = {}
+        self._texture_is_transparent: dict[str, tuple[float, bool]] = {}
+        self._model_files: dict[tuple[str, str], dict] = {}
+        if isinstance(resource_packs, Iterable):
+            self._packs = list(resource_packs)
         elif isinstance(resource_packs, JavaResourcePack):
             self._packs = [resource_packs]
         else:
             raise Exception(f"Invalid format {resource_packs}")
         if load:
             for _ in self.reload():
                 pass
 
-    def _unload(self):
+    def _unload(self) -> None:
         """Clear all loaded resources."""
         super()._unload()
         self._blockstate_files.clear()
         self._textures.clear()
         self._texture_is_transparent.clear()
         self._model_files.clear()
 
-    def _load_iter(self) -> Generator[float, None, None]:
-        blockstate_file_paths: Dict[Tuple[str, str], str] = {}
-        model_file_paths: Dict[Tuple[str, str], str] = {}
+    def _load_iter(self) -> Iterator[float]:
+        blockstate_file_paths: dict[tuple[str, str], str] = {}
+        model_file_paths: dict[tuple[str, str], str] = {}
 
         transparency_cache_path = os.path.join(
             os.environ["CACHE_DIR"], "resource_packs", "java", "transparency_cache.json"
         )
         self._load_transparency_cache(transparency_cache_path)
 
         self._textures[("minecraft", "missing_no")] = self.missing_no
@@ -110,27 +112,27 @@
                     _, namespace, _, *rel_path_list = os.path.normpath(
                         os.path.relpath(texture_path, pack.root_dir)
                     ).split(os.sep)
                     if rel_path_list[0] not in UselessImageGroups:
                         rel_path = "/".join(rel_path_list)[:-4]
                         self._textures[(namespace, rel_path)] = texture_path
                         if (
-                            os.stat(texture_path)[8]
+                            os.stat(texture_path).st_mtime
                             != self._texture_is_transparent.get(texture_path, [0])[0]
                         ):
                             im: Image.Image = Image.open(texture_path)
                             if im.mode == "RGBA":
                                 alpha = numpy.array(im.getchannel("A").getdata())
-                                texture_is_transparent = numpy.any(alpha != 255)
+                                texture_is_transparent = bool(numpy.any(alpha != 255))
                             else:
                                 texture_is_transparent = False
 
                             self._texture_is_transparent[texture_path] = (
-                                os.stat(texture_path)[8],
-                                bool(texture_is_transparent),
+                                os.stat(texture_path).st_mtime,
+                                texture_is_transparent,
                             )
                     yield sub_progress + image_index / (image_count * pack_count * 3)
 
                 blockstate_paths = glob.glob(
                     os.path.join(
                         glob.escape(pack.root_dir),
                         "assets",
@@ -190,28 +192,30 @@
             with open(path) as fi:
                 try:
                     self._model_files[key] = json.load(fi)
                 except json.JSONDecodeError:
                     log.error(f"Failed to parse model file file {path}")
 
     @property
-    def textures(self) -> Tuple[str, ...]:
+    def textures(self) -> tuple[str, ...]:
         """Returns a tuple of all the texture paths in the resource pack."""
         return tuple(self._textures.values())
 
-    def get_texture_path(self, namespace: str, relative_path: str) -> str:
+    def get_texture_path(self, namespace: Optional[str], relative_path: str) -> str:
         """Get the absolute texture path from the namespace and relative path pair"""
+        if namespace is None:
+            return self.missing_no
         key = (namespace, relative_path)
         if key in self._textures:
             return self._textures[key]
         else:
             return self.missing_no
 
     @staticmethod
-    def parse_state_val(val) -> list:
+    def parse_state_val(val: Union[str, bool]) -> list:
         """Convert the json block state format into a consistent format."""
         if isinstance(val, str):
             return [amulet_nbt.TAG_String(v) for v in val.split("|")]
         elif isinstance(val, bool):
             return [
                 amulet_nbt.TAG_String("true") if val else amulet_nbt.TAG_String("false")
             ]
@@ -292,15 +296,17 @@
                     except Exception as e:
                         log.error(f"Failed to parse block state for {block}\n{e}")
 
                 return BlockMesh.merge(models)
 
         return self.missing_block
 
-    def _load_blockstate_model(self, blockstate_value: Union[dict, list]) -> BlockMesh:
+    def _load_blockstate_model(
+        self, blockstate_value: Union[dict, list[dict]]
+    ) -> BlockMesh:
         """Load the model(s) associated with a block state and apply rotations if needed."""
         if isinstance(blockstate_value, list):
             blockstate_value = blockstate_value[0]
         if "model" not in blockstate_value:
             return self.missing_block
         model_path = blockstate_value["model"]
         rotx = int(blockstate_value.get("x", 0) // 90)
@@ -318,21 +324,31 @@
         java_model = self._recursive_load_block_model(model_path)
 
         # set up some variables
         texture_dict = {}
         textures = []
         texture_count = 0
         vert_count = {side: 0 for side in FACE_KEYS}
-        verts = {side: [] for side in FACE_KEYS}
-        tverts = {side: [] for side in FACE_KEYS}
-        tint_verts = {side: [] for side in FACE_KEYS}
-        faces = {side: [] for side in FACE_KEYS}
-
-        texture_indexes = {side: [] for side in FACE_KEYS}
-        transparent = 2
+        verts_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        tverts_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+        tint_verts_src: dict[Optional[str], list[float]] = {
+            side: [] for side in FACE_KEYS
+        }
+        faces_src: dict[Optional[str], list[numpy.ndarray]] = {
+            side: [] for side in FACE_KEYS
+        }
+
+        texture_indexes_src: dict[Optional[str], list[int]] = {
+            side: [] for side in FACE_KEYS
+        }
+        transparent = Transparency.Partial
 
         if java_model.get("textures", {}) and not java_model.get("elements"):
             return self.missing_block
 
         for element in java_model.get("elements", {}):
             # iterate through elements (one cube per element)
             element_faces = element.get("faces", {})
@@ -344,15 +360,15 @@
                 and element.get("to", [16, 16, 16]) == [16, 16, 16]
                 and element.get("from", [0, 0, 0]) == [0, 0, 0]
                 and len(element_faces) >= 6
             ):
                 # if the block is not yet defined as a solid block
                 # and this element is a full size element
                 # check if the texture is opaque
-                transparent = 1
+                transparent = Transparency.FullTranslucent
                 check_faces = True
             else:
                 check_faces = False
 
             # lower and upper box coordinates
             corners = numpy.sort(
                 numpy.array(
@@ -435,67 +451,70 @@
                             angles[0] = -angle
                         elif axis == "y":
                             angles[1] = -angle
                         elif axis == "z":
                             angles[2] = -angle
                         face_verts = rotate_3d(face_verts, *angles, *origin)
 
-                    verts[cull_dir].append(
+                    verts_src[cull_dir].append(
                         face_verts
                     )  # vertex coordinates for this face
 
-                    tverts[cull_dir].append(
+                    tverts_src[cull_dir].append(
                         texture_uv[uv_slice].reshape((-1, 2))  # texture vertices
                     )
                     if "tintindex" in element_faces[face_dir]:
-                        tint_verts[cull_dir] += [
+                        tint_verts_src[cull_dir] += [
                             0,
                             1,
                             0,
                         ] * 4  # TODO: set this up for each supported block
                     else:
-                        tint_verts[cull_dir] += [1, 1, 1] * 4
+                        tint_verts_src[cull_dir] += [1, 1, 1] * 4
 
                     # merge the face indexes and texture index
                     face_table = tri_face + vert_count[cull_dir]
-                    texture_indexes[cull_dir] += [texture_index, texture_index]
+                    texture_indexes_src[cull_dir] += [texture_index, texture_index]
 
                     # faces stored under cull direction because this is the criteria to render them or not
-                    faces[cull_dir].append(face_table)
+                    faces_src[cull_dir].append(face_table)
 
                     vert_count[cull_dir] += 4
 
             if opaque_face_count == 6:
-                transparent = 0
+                transparent = Transparency.FullOpaque
 
-        remove_faces = []
-        for cull_dir, face_array in faces.items():
+        verts: dict[Optional[str], numpy.ndarray] = {}
+        tverts: dict[Optional[str], numpy.ndarray] = {}
+        tint_verts: dict[Optional[str], numpy.ndarray] = {}
+        faces: dict[Optional[str], numpy.ndarray] = {}
+        texture_indexes: dict[Optional[str], numpy.ndarray] = {}
+
+        for cull_dir in FACE_KEYS:
+            face_array = faces_src[cull_dir]
             if len(face_array) > 0:
                 faces[cull_dir] = numpy.concatenate(face_array, axis=None)
                 tint_verts[cull_dir] = numpy.concatenate(
-                    tint_verts[cull_dir], axis=None
+                    tint_verts_src[cull_dir], axis=None
                 )
-                verts[cull_dir] = numpy.concatenate(verts[cull_dir], axis=None)
-                tverts[cull_dir] = numpy.concatenate(tverts[cull_dir], axis=None)
+                verts[cull_dir] = numpy.concatenate(verts_src[cull_dir], axis=None)
+                tverts[cull_dir] = numpy.concatenate(tverts_src[cull_dir], axis=None)
                 texture_indexes[cull_dir] = numpy.array(
-                    texture_indexes[cull_dir], dtype=numpy.uint32
+                    texture_indexes_src[cull_dir], dtype=numpy.uint32
                 )
-            else:
-                remove_faces.append(cull_dir)
-
-        for cull_dir in remove_faces:
-            del faces[cull_dir]
-            del tint_verts[cull_dir]
-            del verts[cull_dir]
-            del tverts[cull_dir]
-            del texture_indexes[cull_dir]
-        textures = tuple(textures)
 
         return BlockMesh(
-            3, verts, tverts, tint_verts, faces, texture_indexes, textures, transparent
+            3,
+            verts,
+            tverts,
+            tint_verts,
+            faces,
+            texture_indexes,
+            tuple(textures),
+            transparent,
         )
 
     def _recursive_load_block_model(self, model_path: str) -> dict:
         """Load a model json file and recursively load and merge the parent entries into one json file."""
         model_path_list = model_path.split(":", 1)
         if len(model_path_list) == 2:
             namespace, model_path = model_path_list
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/PKG-INFO` & `minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-resource-pack
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python library reading Minecraft's various resource pack formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,9 @@
 Provides-Extra: docs
 Requires-Dist: Sphinx>=1.7.4; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.3.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=0.3.1; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: black>=22.3; extra == "dev"
 Requires-Dist: pre_commit>=1.11.1; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-pyinstaller; extra == "dev"
```

### Comparing `minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/SOURCES.txt` & `minecraft_resource_pack-1.4.3/minecraft_resource_pack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_resource_pack-1.4.2/setup.cfg` & `minecraft_resource_pack-1.4.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -45,31 +45,33 @@
 000002c0: 5370 6869 6e78 3e3d 312e 372e 340d 0a09  Sphinx>=1.7.4...
 000002d0: 7370 6869 6e78 2d61 7574 6f64 6f63 2d74  sphinx-autodoc-t
 000002e0: 7970 6568 696e 7473 3e3d 312e 332e 300d  ypehints>=1.3.0.
 000002f0: 0a09 7370 6869 6e78 5f72 7464 5f74 6865  ..sphinx_rtd_the
 00000300: 6d65 3e3d 302e 332e 310d 0a64 6576 203d  me>=0.3.1..dev =
 00000310: 200d 0a09 626c 6163 6b3e 3d32 322e 330d   ...black>=22.3.
 00000320: 0a09 7072 655f 636f 6d6d 6974 3e3d 312e  ..pre_commit>=1.
-00000330: 3131 2e31 0d0a 0d0a 5b6f 7074 696f 6e73  11.1....[options
-00000340: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000350: 7079 696e 7374 616c 6c65 7234 3020 3d20  pyinstaller40 = 
-00000360: 0d0a 0968 6f6f 6b2d 6469 7273 203d 206d  ...hook-dirs = m
-00000370: 696e 6563 7261 6674 5f6d 6f64 656c 5f72  inecraft_model_r
-00000380: 6561 6465 722e 5f5f 7079 696e 7374 616c  eader.__pyinstal
-00000390: 6c65 723a 6765 745f 686f 6f6b 5f64 6972  ler:get_hook_dir
-000003a0: 730d 0a0d 0a5b 7665 7273 696f 6e65 6572  s....[versioneer
-000003b0: 5d0d 0a56 4353 203d 2067 6974 0d0a 7374  ]..VCS = git..st
-000003c0: 796c 6520 3d20 7065 7034 3430 0d0a 7665  yle = pep440..ve
-000003d0: 7273 696f 6e66 696c 655f 736f 7572 6365  rsionfile_source
-000003e0: 203d 206d 696e 6563 7261 6674 5f6d 6f64   = minecraft_mod
-000003f0: 656c 5f72 6561 6465 722f 5f76 6572 7369  el_reader/_versi
-00000400: 6f6e 2e70 790d 0a76 6572 7369 6f6e 6669  on.py..versionfi
-00000410: 6c65 5f62 7569 6c64 203d 206d 696e 6563  le_build = minec
-00000420: 7261 6674 5f6d 6f64 656c 5f72 6561 6465  raft_model_reade
-00000430: 722f 5f76 6572 7369 6f6e 2e70 790d 0a74  r/_version.py..t
-00000440: 6167 5f70 7265 6669 7820 3d20 0d0a 7061  ag_prefix = ..pa
-00000450: 7265 6e74 6469 725f 7072 6566 6978 203d  rentdir_prefix =
-00000460: 206d 696e 6563 7261 6674 5f6d 6f64 656c   minecraft_model
-00000470: 5f72 6561 6465 722d 0d0a 0d0a 5b65 6767  _reader-....[egg
-00000480: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000490: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004a0: 2030 0d0a 0d0a                            0....
+00000330: 3131 2e31 0d0a 096d 7970 790d 0a09 7479  11.1...mypy...ty
+00000340: 7065 732d 7079 696e 7374 616c 6c65 720d  pes-pyinstaller.
+00000350: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
+00000360: 795f 706f 696e 7473 5d0d 0a70 7969 6e73  y_points]..pyins
+00000370: 7461 6c6c 6572 3430 203d 200d 0a09 686f  taller40 = ...ho
+00000380: 6f6b 2d64 6972 7320 3d20 6d69 6e65 6372  ok-dirs = minecr
+00000390: 6166 745f 6d6f 6465 6c5f 7265 6164 6572  aft_model_reader
+000003a0: 2e5f 5f70 7969 6e73 7461 6c6c 6572 3a67  .__pyinstaller:g
+000003b0: 6574 5f68 6f6f 6b5f 6469 7273 0d0a 0d0a  et_hook_dirs....
+000003c0: 5b76 6572 7369 6f6e 6565 725d 0d0a 5643  [versioneer]..VC
+000003d0: 5320 3d20 6769 740d 0a73 7479 6c65 203d  S = git..style =
+000003e0: 2070 6570 3434 300d 0a76 6572 7369 6f6e   pep440..version
+000003f0: 6669 6c65 5f73 6f75 7263 6520 3d20 6d69  file_source = mi
+00000400: 6e65 6372 6166 745f 6d6f 6465 6c5f 7265  necraft_model_re
+00000410: 6164 6572 2f5f 7665 7273 696f 6e2e 7079  ader/_version.py
+00000420: 0d0a 7665 7273 696f 6e66 696c 655f 6275  ..versionfile_bu
+00000430: 696c 6420 3d20 6d69 6e65 6372 6166 745f  ild = minecraft_
+00000440: 6d6f 6465 6c5f 7265 6164 6572 2f5f 7665  model_reader/_ve
+00000450: 7273 696f 6e2e 7079 0d0a 7461 675f 7072  rsion.py..tag_pr
+00000460: 6566 6978 203d 200d 0a70 6172 656e 7464  efix = ..parentd
+00000470: 6972 5f70 7265 6669 7820 3d20 6d69 6e65  ir_prefix = mine
+00000480: 6372 6166 745f 6d6f 6465 6c5f 7265 6164  craft_model_read
+00000490: 6572 2d0d 0a0d 0a5b 6567 675f 696e 666f  er-....[egg_info
+000004a0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000004b0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000004c0: 0a                                       .
```

