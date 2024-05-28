# Comparing `tmp/ufo2ft-3.2.3.tar.gz` & `tmp/ufo2ft-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufo2ft-3.2.3.tar", last modified: Fri May 17 10:30:14 2024, max compression
+gzip compressed data, was "ufo2ft-3.2.4.tar", last modified: Tue May 28 15:38:49 2024, max compression
```

## Comparing `ufo2ft-3.2.3.tar` & `ufo2ft-3.2.4.tar`

### file list

```diff
@@ -1,1205 +1,1205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.580708 ufo2ft-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.408708 ufo2ft-3.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.428708 ufo2ft-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.408708 ufo2ft-3.2.3/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.432708 ufo2ft-3.2.3/Lib/ufo2ft/
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.432708 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/baseCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/interpolatableOTFCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/interpolatableTTFCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/otfCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/ttfCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/variableCFF2sCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/_compilers/variableTTFsCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureCompiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.432708 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/baseFeatureWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/cursFeatureWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/gdefFeatureWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    47293 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/kernFeatureWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19989 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/kernFeatureWriter2.py
--rw-r--r--   0 runner    (1001) docker     (127)    39587 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/markFeatureWriter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.436708 ufo2ft-3.2.3/Lib/ufo2ft/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/cubicToQuadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/decomposeComponents.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/decomposeTransformedComponents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/dottedCircle.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/dottedCircleFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/explodeColorLayerGlyphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/flattenComponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/propagateAnchors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/removeOverlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/reverseContourDirection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/skipExportGlyphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/sortContours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/filters/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16933 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/fontInfoData.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/infoCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    40095 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/instantiator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/instructionCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/maxContextCalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    74350 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/outlineCompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/postProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21475 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/preProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/Lib/ufo2ft/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.580708 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    62484 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 10:30:14.000000 ufo2ft-3.2.3/Lib/ufo2ft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-17 10:30:14.580708 ufo2ft-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 10:30:14.584708 ufo2ft-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.436708 ufo2ft-3.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.444708 ufo2ft-3.2.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.444708 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.444708 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.below.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.glif
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ttx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.448708 ufo2ft-3.2.3/tests/data/Bug108.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.448708 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/Bug108_included.fea
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.448708 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.448708 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/a.color1.glif
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/a.color2.glif
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.448708 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb.loclV_I_E_T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb_tildecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/o.glif
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/ocircumflextilde.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/tildecomb.loclV_I_E_T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/ColorTest.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color2/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTest.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.452708 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/a.color1.glif
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/a.color2.glif
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_different_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_no_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_same_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/no_component.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_different_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_no_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_same_transform.glif
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/no_component.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.456708 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/graphemejoinercomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/uniF_F_F_C_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/xxx.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DSv5/
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight-TTF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    30783 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight_Width-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    32421 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight_Width-TTF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Width-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20259 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Width-TTF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSerifVariable_Width-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    17084 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/MutatorSerifVariable_Width-TTF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DSv5/test_v5_MutatorSans_and_Serif.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.460708 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.464708 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.464708 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.464708 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.464708 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.464708 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufoz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufoz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.468708 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.472708 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/acutecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/dotbelowcomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.472708 ufo2ft-3.2.3/tests/data/IncompatibleMasters/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/IncompatibleMasters.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.472708 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.476708 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/d.glif
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/f.glif
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.476708 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.476708 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/d.glif
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/f.glif
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.476708 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.476708 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.480708 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.480708 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.480708 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.480708 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.484708 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/dotabovecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/edotabove.glif
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/s.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.484708 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.484708 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/dotabovecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/edotabove.glif
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/s.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.484708 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ttx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.484708 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.416708 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/data/com.github.googlei18n.ufo2ft.mtiFeatures/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/data/com.github.googlei18n.ufo2ft.mtiFeatures/GSUB.mti
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/acutecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.488708 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/acutecomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/ae.glif
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.492708 ufo2ft-3.2.3/tests/data/MutatorSans/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-weight-only.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-width-only.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.492708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.500708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.500708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.500708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.508708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.508708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.508708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.508708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.512708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.516708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.520708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.524708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    18792 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.528708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans_missing.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans_no_default.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSansLite/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.536708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.540708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.540708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.540708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.540708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.540708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.544708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.548708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.552708 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/d.glif
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/d.glif
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/space.glif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/NestedComponents.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/glyphs/o.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/glyphs/o.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/OTestFont.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.556708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/contents.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/contents.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/A_stroke.glif
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/highspacingdot-deva.glif
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/ka-deva.glif
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/ra-deva.glif
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.424708 ufo2ft-3.2.3/tests/data/SwapGlyphNames/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.560708 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.564708 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.564708 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.564708 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-CFF-compreffor.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-CFF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-CFF2-cffsubr.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-CFF2-compreffor.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-CFF2-post3.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOptimize-CFF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOptimize-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-CFF-pathops.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18283 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-CFF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-TTF-pathops.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-TTF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-Specialized-CFF.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-Specialized-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-TTF-post3.ttx
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont-not-allQuadratic.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ttx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.564708 ufo2ft-3.2.3/tests/data/TestFont.ufo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.424708 ufo2ft-3.2.3/tests/data/TestFont.ufo/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.564708 ufo2ft-3.2.3/tests/data/TestFont.ufo/data/com.github.fonttools.ttx/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/data/com.github.fonttools.ttx/CUST.ttx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.568708 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/_notdef.glif
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/b.glif
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/c.glif
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/d.glif
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/e.glif
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/f.glif
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/g.glif
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/h.glif
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/i.glif
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/j.glif
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/k.glif
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/l.glif
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestFont.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.568708 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.bot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.ext.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.glif
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size1.glif
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size2.glif
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size3.glif
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size4.glif
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.top.glif
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.bot.glif
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.ext.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.glif
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size1.glif
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size2.glif
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size3.glif
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size4.glif
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.top.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/glyphs/alef-ar.fina.glif
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-MyFontVF1.ttx
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-MyFontVF2.ttx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/glyphs/alef-ar.fina.glif
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarFont.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.572708 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.576708 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/alef-ar.fina.glif
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/dotabove-ar.glif
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.glif
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/metainfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.576708 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.576708 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/a.glif
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/alef-ar.fina.glif
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/dotabove-ar.glif
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/gravecmb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/layerinfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.glif
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/space.glif
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVarfea.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-cffsubr.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-post3.ttx
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-sparse-notdefGlyph.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-useProductionNames.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2.ttx
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-not-allQuadratic.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20112 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-post3.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20989 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-useProductionNames.ttx
--rw-r--r--   0 runner    (1001) docker     (127)    20793 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/TestVariableFont-TTF.ttx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.576708 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.576708 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/I_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/I_acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/acute.glif
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/glyphs/romanthree.glif
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureCompiler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.580708 ufo2ft-3.2.3/tests/featureWriters/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/ast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/cursFeatureWriter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/featureWriters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/gdefFeatureWriter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/kernFeatureWriter2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    67051 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/kernFeatureWriter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    60802 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/markFeatureWriter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/featureWriters/variableFeatureWriter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:14.580708 ufo2ft-3.2.3/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/decomposeComponents_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/decomposeTransformedComponents_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/dottedCircle_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/explodeColorLayerGlyphs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/flattenComponents_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/propagateAnchors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/sortContours_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/filters/transformations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/fontInfoData_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/infoCompiler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27402 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/instantiator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/instructionCompiler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23862 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    50298 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/outlineCompiler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/preProcessor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/testSupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tests/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 10:30:07.000000 ufo2ft-3.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.809224 ufo2ft-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.629222 ufo2ft-3.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.653223 ufo2ft-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.629222 ufo2ft-3.2.4/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.657223 ufo2ft-3.2.4/Lib/ufo2ft/
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.657223 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/baseCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/interpolatableOTFCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/interpolatableTTFCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/otfCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/ttfCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/variableCFF2sCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/_compilers/variableTTFsCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureCompiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.661223 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17870 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/baseFeatureWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/cursFeatureWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/gdefFeatureWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/kernFeatureWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22845 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/kernFeatureWriter2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39587 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/markFeatureWriter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.661223 ufo2ft-3.2.4/Lib/ufo2ft/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/cubicToQuadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/decomposeComponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/decomposeTransformedComponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/dottedCircle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/dottedCircleFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/explodeColorLayerGlyphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/flattenComponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/propagateAnchors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/removeOverlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/reverseContourDirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/skipExportGlyphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/sortContours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/filters/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16933 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/fontInfoData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/infoCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40095 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/instantiator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/instructionCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/maxContextCalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74350 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/outlineCompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/postProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21475 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/preProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/Lib/ufo2ft/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.805224 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    62484 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 15:38:49.000000 ufo2ft-3.2.4/Lib/ufo2ft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-28 15:38:49.809224 ufo2ft-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 15:38:49.809224 ufo2ft-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.665223 ufo2ft-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.673223 ufo2ft-3.2.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.673223 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.673223 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.below.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ttx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.673223 ufo2ft-3.2.4/tests/data/Bug108.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/Bug108_included.fea
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/a.color1.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/a.color2.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb.loclV_I_E_T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb_tildecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/o.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/ocircumflextilde.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/tildecomb.loclV_I_E_T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.677223 ufo2ft-3.2.4/tests/data/ColorTest.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.681223 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.681223 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.681223 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color2/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTest.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.681223 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.681223 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/a.color1.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/a.color2.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_different_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_no_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_same_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/no_component.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_different_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_no_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/component_same_transform.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/no_component.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.685223 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/graphemejoinercomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/uniF_F_F_C_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/xxx.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DSv5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight-TTF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    30783 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight_Width-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    32421 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight_Width-TTF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Width-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20259 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Width-TTF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSerifVariable_Width-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    17084 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/MutatorSerifVariable_Width-TTF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DSv5/test_v5_MutatorSans_and_Serif.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.689223 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.693223 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.693223 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.693223 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.693223 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.693223 ufo2ft-3.2.4/tests/data/DesignspaceTest/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufoz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.697223 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.701223 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/acutecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/dotbelowcomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.701223 ufo2ft-3.2.4/tests/data/IncompatibleMasters/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/IncompatibleMasters.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.701223 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.701223 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/d.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/f.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.701223 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/d.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/f.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.705223 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/dotabovecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/edotabove.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/s.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/dotabovecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/edotabove.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/s.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ttx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.637223 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.709223 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/data/com.github.googlei18n.ufo2ft.mtiFeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/data/com.github.googlei18n.ufo2ft.mtiFeatures/GSUB.mti
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.713223 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.713223 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.713223 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/acutecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.713223 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.713223 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/acutecomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/ae.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.717223 ufo2ft-3.2.4/tests/data/MutatorSans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-width-only.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.717223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.725223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.725223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.725223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.733223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.733223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.733223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.733223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.737223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.741223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.745223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.749223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    18792 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.753223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans_missing.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans_no_default.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSansLite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.761223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.765223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.765223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.765223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.765223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.765223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.769224 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.773223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    16116 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.777223 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/d.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/d.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/space.glif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs.M_edium/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/NestedComponents.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/glyphs/o.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.781224 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/glyphs/o.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/OTestFont.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/contents.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{151}/contents.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/A_stroke.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs.{170}/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.785224 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.789224 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/highspacingdot-deva.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/ka-deva.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/ra-deva.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.649223 ufo2ft-3.2.4/tests/data/SwapGlyphNames/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.789224 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.789224 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.789224 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.789224 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-CFF-compreffor.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-CFF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-CFF2-cffsubr.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-CFF2-compreffor.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-CFF2-post3.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOptimize-CFF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOptimize-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-CFF-pathops.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18283 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-CFF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-TTF-pathops.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-TTF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-Specialized-CFF.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-Specialized-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-TTF-post3.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont-not-allQuadratic.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ttx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.793223 ufo2ft-3.2.4/tests/data/TestFont.ufo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.649223 ufo2ft-3.2.4/tests/data/TestFont.ufo/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.793223 ufo2ft-3.2.4/tests/data/TestFont.ufo/data/com.github.fonttools.ttx/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/data/com.github.fonttools.ttx/CUST.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.793223 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/_notdef.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/b.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/c.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/d.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/e.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/f.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/g.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/h.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/i.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/j.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/k.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/l.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestFont.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.793223 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.797224 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.bot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.ext.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size1.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size2.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size3.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size4.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.top.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.bot.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.ext.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size1.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size2.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size3.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.size4.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.top.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.797224 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.797224 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/glyphs/alef-ar.fina.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-MyFontVF1.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-MyFontVF2.ttx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.797224 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.797224 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/glyphs/alef-ar.fina.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarFont.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.801224 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.801224 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/alef-ar.fina.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/dotabove-ar.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/metainfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.801224 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.801224 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/a.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/alef-ar.fina.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/dotabove-ar.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/gravecmb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/layerinfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/space.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVarfea.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-cffsubr.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-post3.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-sparse-notdefGlyph.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    17687 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-useProductionNames.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    17503 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-not-allQuadratic.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    20389 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-post3.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-useProductionNames.ttx
+-rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/TestVariableFont-TTF.ttx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.805224 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.805224 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/I_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/I_acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/acute.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/glyphs/romanthree.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureCompiler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.805224 ufo2ft-3.2.4/tests/featureWriters/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/ast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/cursFeatureWriter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/featureWriters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/gdefFeatureWriter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/kernFeatureWriter2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67051 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/kernFeatureWriter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60802 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/markFeatureWriter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/featureWriters/variableFeatureWriter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:49.805224 ufo2ft-3.2.4/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/decomposeComponents_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/decomposeTransformedComponents_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/dottedCircle_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/explodeColorLayerGlyphs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/flattenComponents_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/propagateAnchors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/sortContours_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/filters/transformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/fontInfoData_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/infoCompiler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27402 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/instantiator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/instructionCompiler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23862 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50298 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/outlineCompiler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/preProcessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/testSupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tests/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-28 15:38:43.000000 ufo2ft-3.2.4/tox.ini
```

### Comparing `ufo2ft-3.2.3/.coveragerc` & `ufo2ft-3.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/.github/workflows/ci.yml` & `ufo2ft-3.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/LICENSE` & `ufo2ft-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/__init__.py` & `ufo2ft-3.2.4/Lib/ufo2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/baseCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/baseCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/interpolatableOTFCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/interpolatableOTFCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/interpolatableTTFCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/interpolatableTTFCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/otfCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/otfCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/ttfCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/ttfCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/variableCFF2sCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/variableCFF2sCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/_compilers/variableTTFsCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/_compilers/variableTTFsCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/constants.py` & `ufo2ft-3.2.4/Lib/ufo2ft/constants.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/__init__.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/__init__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/__main__.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/__main__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/ast.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/ast.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/baseFeatureWriter.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/baseFeatureWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,19 @@
        if present, or it will add a new one at the end of all features.
     Subclasses can set a different default mode or define a different
     set of `_SUPPORTED_MODES`.
 
     The `options` class attribute contains a mapping of option
     names with their default values. These can be overridden on an
     instance by passing keyword arguments to the constructor.
+
+    Combining manually written and automatically generated feature code
+    can be achieved by using the `# Automatic Code` insertion marker
+    inside the feature code. Automatically generated code for the
+    respective feature is added in that spot.
     """
 
     tableTag = None
     features = frozenset()
     mode = "skip"
     insertFeatureMarker = INSERT_FEATURE_MARKER
     options = {}
@@ -413,17 +418,21 @@
     def _getAnchor(self, glyphName, anchorName, anchor=None):
         if self.context.isVariable:
             designspace = self.context.font
             x_value = VariableScalar()
             y_value = VariableScalar()
             found = False
             for source in designspace.sources:
-                if glyphName not in source.font:
+                if source.layerName is None:
+                    layer = source.font
+                else:
+                    layer = source.font.layers[source.layerName]
+                if glyphName not in layer:
                     continue
-                glyph = source.font[glyphName]
+                glyph = layer[glyphName]
                 for anchor in glyph.anchors:
                     if anchor.name == anchorName:
                         location = get_userspace_location(designspace, source.location)
                         x_value.add_value(location, otRound(anchor.x))
                         y_value.add_value(location, otRound(anchor.y))
                         found = True
             if not found:
```

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/cursFeatureWriter.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/cursFeatureWriter.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/gdefFeatureWriter.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/gdefFeatureWriter.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/kernFeatureWriter.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/kernFeatureWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,21 @@
 
     def getKerningPairs(
         self,
         side1Classes: Mapping[str, tuple[str, ...]],
         side2Classes: Mapping[str, tuple[str, ...]],
     ) -> list[KerningPair]:
         if self.context.isVariable:
-            return self.getVariableKerningPairs(side1Classes, side2Classes)
+            return self.getVariableKerningPairs(
+                self.context.font,
+                side1Classes,
+                side2Classes,
+                self.context.glyphSet,
+                self.options,
+            )
 
         glyphSet = self.context.glyphSet
         font = self.context.font
         kerning = font.kerning
         quantization = self.options.quantization
 
         kerning: Mapping[tuple[str, str], float] = font.kerning
@@ -428,22 +434,23 @@
             if secondIsClass:
                 side2 = side2Classes[side2]
             value = quantize(value, quantization)
             result.append(KerningPair(side1, side2, value))
 
         return result
 
+    @staticmethod
     def getVariableKerningPairs(
-        self,
+        designspace: DesignSpaceDocument,
         side1Classes: Mapping[str, tuple[str, ...]],
         side2Classes: Mapping[str, tuple[str, ...]],
+        glyphSet: Mapping[str, str],
+        options: SimpleNamespace,
     ) -> list[KerningPair]:
-        designspace: DesignSpaceDocument = self.context.font
-        glyphSet = self.context.glyphSet
-        quantization = self.options.quantization
+        quantization = options.quantization
 
         # Gather utility variables for faster kerning lookups.
         # TODO: Do we construct these in code elsewhere?
         assert not (set(side1Classes) & set(side2Classes))
         unified_groups = {**side1Classes, **side2Classes}
 
         glyphToFirstGroup = {
```

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/kernFeatureWriter2.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/kernFeatureWriter2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """Old implementation of KernFeatureWriter as of ufo2ft v2.30.0 for backward compat."""
 
+from __future__ import annotations
+
 from types import SimpleNamespace
+from typing import Mapping
 
 from fontTools import unicodedata
+from fontTools.designspaceLib import DesignSpaceDocument
 
 from ufo2ft.constants import INDIC_SCRIPTS, USE_SCRIPTS
 from ufo2ft.featureWriters import BaseFeatureWriter, ast
+from ufo2ft.featureWriters.kernFeatureWriter import (
+    KernFeatureWriter as NewKernFeatureWriter,
+)
 from ufo2ft.util import classifyGlyphs, quantize, unicodeScriptDirection
 
 SIDE1_PREFIX = "public.kern1."
 SIDE2_PREFIX = "public.kern2."
 
 # In HarfBuzz the 'dist' feature is automatically enabled for these shapers:
 #   src/hb-ot-shape-complex-myanmar.cc
@@ -109,15 +116,17 @@
     tableTag = "GPOS"
     features = frozenset(["kern", "dist"])
     options = dict(ignoreMarks=True, quantization=1)
 
     def setContext(self, font, feaFile, compiler=None):
         ctx = super().setContext(font, feaFile, compiler=compiler)
         ctx.gdefClasses = self.getGDEFGlyphClasses()
-        ctx.kerning = self.getKerningData(font, feaFile, self.getOrderedGlyphSet())
+        ctx.kerning = self.getKerningData(
+            font, self.options, feaFile, self.getOrderedGlyphSet()
+        )
 
         feaScripts = ast.getScriptLanguageSystems(feaFile)
         ctx.scriptGroups = self._groupScriptsByTagAndDirection(feaScripts)
 
         return ctx
 
     def shouldContinue(self):
@@ -164,29 +173,36 @@
             classDefs=newClassDefs,
             lookups=lookupGroups,
             features=[features[tag] for tag in ["kern", "dist"] if tag in features],
         )
         return True
 
     @classmethod
-    def getKerningData(cls, font, feaFile=None, glyphSet=None):
+    def getKerningData(cls, font, options, feaFile=None, glyphSet=None):
         side1Classes, side2Classes = cls.getKerningClasses(font, feaFile, glyphSet)
-        pairs = cls.getKerningPairs(font, side1Classes, side2Classes, glyphSet)
+        pairs = cls.getKerningPairs(font, side1Classes, side2Classes, glyphSet, options)
         return SimpleNamespace(
             side1Classes=side1Classes, side2Classes=side2Classes, pairs=pairs
         )
 
     @staticmethod
     def getKerningGroups(font, glyphSet=None):
         if glyphSet:
             allGlyphs = set(glyphSet.keys())
         else:
             allGlyphs = set(font.keys())
         side1Groups = {}
         side2Groups = {}
+
+        if isinstance(font, DesignSpaceDocument):
+            default_font = font.findDefault()
+            assert default_font is not None
+            font = default_font.font
+            assert font is not None
+
         for name, members in font.groups.items():
             # prune non-existent or skipped glyphs
             members = [g for g in members if g in allGlyphs]
             if not members:
                 # skip empty groups
                 continue
             # skip groups without UFO3 public.kern{1,2} prefix
@@ -204,15 +220,75 @@
         )
         side2Classes = ast.makeGlyphClassDefinitions(
             side2Groups, feaFile, stripPrefix="public."
         )
         return side1Classes, side2Classes
 
     @staticmethod
-    def getKerningPairs(font, side1Classes, side2Classes, glyphSet=None):
+    def getKerningPairs(font, side1Classes, side2Classes, glyphSet=None, options=None):
+        if isinstance(font, DesignSpaceDocument):
+            # Reuse the newer kern writers variable kerning extractor. Repack
+            # some arguments and the return type for this.
+            side1ClassesRaw: Mapping[str, tuple[str, ...]] = {
+                group_name: tuple(
+                    glyph
+                    for glyphs in glyph_defs.glyphSet()
+                    for glyph in glyphs.glyphSet()
+                )
+                for group_name, glyph_defs in side1Classes.items()
+            }
+            side2ClassesRaw: Mapping[str, tuple[str, ...]] = {
+                group_name: tuple(
+                    glyph
+                    for glyphs in glyph_defs.glyphSet()
+                    for glyph in glyphs.glyphSet()
+                )
+                for group_name, glyph_defs in side2Classes.items()
+            }
+            pairs = NewKernFeatureWriter.getVariableKerningPairs(
+                font,
+                side1ClassesRaw,
+                side2ClassesRaw,
+                glyphSet or {},
+                options or SimpleNamespace(**KernFeatureWriter.options),
+            )
+            pairs.sort()
+            side1toClass: Mapping[tuple[str, ...], ast.GlyphClassDefinition] = {
+                tuple(
+                    glyph
+                    for glyphs in glyph_defs.glyphSet()
+                    for glyph in glyphs.glyphSet()
+                ): glyph_defs
+                for glyph_defs in side1Classes.values()
+            }
+            side2toClass: Mapping[tuple[str, ...], ast.GlyphClassDefinition] = {
+                tuple(
+                    glyph
+                    for glyphs in glyph_defs.glyphSet()
+                    for glyph in glyphs.glyphSet()
+                ): glyph_defs
+                for glyph_defs in side2Classes.values()
+            }
+            return [
+                KerningPair(
+                    (
+                        side1toClass[pair.side1]
+                        if isinstance(pair.side1, tuple)
+                        else pair.side1
+                    ),
+                    (
+                        side2toClass[pair.side2]
+                        if isinstance(pair.side2, tuple)
+                        else pair.side2
+                    ),
+                    pair.value,
+                )
+                for pair in pairs
+            ]
+
         if glyphSet:
             allGlyphs = set(glyphSet.keys())
         else:
             allGlyphs = set(font.keys())
         kerning = font.kerning
 
         pairsByFlags = {}
```

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/featureWriters/markFeatureWriter.py` & `ufo2ft-3.2.4/Lib/ufo2ft/featureWriters/markFeatureWriter.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/__init__.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/__main__.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/__main__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/base.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/base.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/cubicToQuadratic.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/cubicToQuadratic.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/decomposeComponents.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/decomposeComponents.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/decomposeTransformedComponents.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/decomposeTransformedComponents.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/dottedCircle.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/dottedCircle.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/explodeColorLayerGlyphs.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/explodeColorLayerGlyphs.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/flattenComponents.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/flattenComponents.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/propagateAnchors.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/propagateAnchors.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/removeOverlaps.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/removeOverlaps.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/skipExportGlyphs.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/skipExportGlyphs.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/sortContours.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/sortContours.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/filters/transformations.py` & `ufo2ft-3.2.4/Lib/ufo2ft/filters/transformations.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/fontInfoData.py` & `ufo2ft-3.2.4/Lib/ufo2ft/fontInfoData.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/infoCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/infoCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/instantiator.py` & `ufo2ft-3.2.4/Lib/ufo2ft/instantiator.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/instructionCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/instructionCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/outlineCompiler.py` & `ufo2ft-3.2.4/Lib/ufo2ft/outlineCompiler.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/postProcessor.py` & `ufo2ft-3.2.4/Lib/ufo2ft/postProcessor.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/preProcessor.py` & `ufo2ft-3.2.4/Lib/ufo2ft/preProcessor.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft/util.py` & `ufo2ft-3.2.4/Lib/ufo2ft/util.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft.egg-info/PKG-INFO` & `ufo2ft-3.2.4/Lib/ufo2ft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufo2ft
-Version: 3.2.3
+Version: 3.2.4
 Summary: A bridge between UFOs and FontTools.
 Home-page: https://github.com/googlefonts/ufo2ft
 Author: Tal Leming, James Godfrey-Kittle
 Author-email: tal@typesupply.com
 Maintainer: Cosimo Lupo
 Maintainer-email: cosimo@anthrotype.com
 License: MIT
```

### Comparing `ufo2ft-3.2.3/Lib/ufo2ft.egg-info/SOURCES.txt` & `ufo2ft-3.2.4/Lib/ufo2ft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/PKG-INFO` & `ufo2ft-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufo2ft
-Version: 3.2.3
+Version: 3.2.4
 Summary: A bridge between UFOs and FontTools.
 Home-page: https://github.com/googlefonts/ufo2ft
 Author: Tal Leming, James Godfrey-Kittle
 Author-email: tal@typesupply.com
 Maintainer: Cosimo Lupo
 Maintainer-email: cosimo@anthrotype.com
 License: MIT
```

### Comparing `ufo2ft-3.2.3/README.rst` & `ufo2ft-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/setup.py` & `ufo2ft-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/conftest.py` & `ufo2ft-3.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.B_R_A_C_K_E_T_.varA_lt01.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.B_R_A_C_K_E_T_.varA_lt01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.below.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.below.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/ka-oriya.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/lV_ocalicM_atra-oriya.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.B_R_A_C_K_E_T_.varA_lt01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.glif` & `ufo2ft-3.2.4/tests/data/Alternates-Regular.ufo/glyphs/uuM_atra-oriya.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Bug108.ttx` & `ufo2ft-3.2.4/tests/data/Bug108.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Bug108.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/Bug108.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/Bug108.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/Bug108.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/glyphs/a.color1.glif` & `ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/glyphs/a.color1.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/COLRv1Test.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/COLRv1Test.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb.loclV_I_E_T_.glif` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/circumflexcomb.loclV_I_E_T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/o.glif` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/o.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/glyphs/tildecomb.loclV_I_E_T_.glif` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/glyphs/tildecomb.loclV_I_E_T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/CantarellAnchorPropagation.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/CantarellAnchorPropagation.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/b.glif` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs/c.glif` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/a.glif` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/b.glif` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/glyphs.color1/c.glif` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/glyphs.color1/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTest.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/ColorTest.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/glyphs/a.color1.glif` & `ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/glyphs/a.color1.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ColorTestRaw.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/ColorTestRaw.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_different_transform.glif` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_different_transform.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_same_transform.glif` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/component_same_transform.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Bold.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Bold.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ComponentTransformTest-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/ComponentTransformTest-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/graphemejoinercomb.glif` & `ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/graphemejoinercomb.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/glyphs/uniF_F_F_C_.glif` & `ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/glyphs/uniF_F_F_C_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/ContourOrderTest.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/ContourOrderTest.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight-TTF.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight-TTF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight_Width-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight_Width-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Weight_Width-TTF.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Weight_Width-TTF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Width-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Width-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSansVariable_Width-TTF.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSansVariable_Width-TTF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSerifVariable_Width-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSerifVariable_Width-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/MutatorSerifVariable_Width-TTF.ttx` & `ufo2ft-3.2.4/tests/data/DSv5/MutatorSerifVariable_Width-TTF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DSv5/test_v5_MutatorSans_and_Serif.designspace` & `ufo2ft-3.2.4/tests/data/DSv5/test_v5_MutatorSans_and_Serif.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif` & `ufo2ft-3.2.4/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/DesignspaceTest.designspace` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Bold.ufoz` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Bold.ufoz`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Light.ufoz` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Light.ufoz`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DesignspaceTest/MyFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DesignspaceTest/MyFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/a.glif` & `ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/c.glif` & `ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/glyphs/dotbelowcomb.glif` & `ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/glyphs/dotbelowcomb.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/DottedCircleTest.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/DottedCircleTest.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/IncompatibleMasters.designspace` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/IncompatibleMasters.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/b.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/c.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/d.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/d.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/groups.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/groups.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Bold.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Bold.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/b.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/c.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/d.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/d.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/groups.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/groups.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/IncompatibleMasters/NewFont-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/IncompatibleMasters/NewFont-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace` & `ufo2ft-3.2.4/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/_notdef.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/_notdef.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/a.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Bold.ufo/glyphs/s.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Bold.ufo/glyphs/s.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/_notdef.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/_notdef.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/a.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs/s.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs/s.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/e.glif` & `ufo2ft-3.2.4/tests/data/LayerFont-Regular.ufo/glyphs.M_edium/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MTIFeatures.ttx` & `ufo2ft-3.2.4/tests/data/MTIFeatures.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MTIFeatures.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MTIFeatures.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/a.glif` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/acutecomb.glif` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/acutecomb.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClasses.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClasses.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/acutecomb.glif` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/acutecomb.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/ae.glif` & `ufo2ft-3.2.4/tests/data/MultipleAnchorClassesConflict.ufo/glyphs/ae.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/LICENSE` & `ufo2ft-3.2.4/tests/data/MutatorSans/LICENSE`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-weight-only.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-weight-only.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-width-only.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-width-only.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans_missing.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans_missing.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSans/MutatorSans_no_default.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSans/MutatorSans_no_default.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/LICENSE` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/LICENSE`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/b.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/d.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/d.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Bold.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/NestedComponents-Bold.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/b.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/b.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/c.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/c.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/d.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/d.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/NestedComponents-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/NestedComponents.designspace` & `ufo2ft-3.2.4/tests/data/NestedComponents.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/OTestFont-Bold.ufo/glyphs/o.glif` & `ufo2ft-3.2.4/tests/data/OTestFont-Bold.ufo/glyphs/o.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/OTestFont-Regular.ufo/glyphs/o.glif` & `ufo2ft-3.2.4/tests/data/OTestFont-Regular.ufo/glyphs/o.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/OTestFont.designspace` & `ufo2ft-3.2.4/tests/data/OTestFont.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Bold.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_.glif` & `ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest-Regular.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SkipExportGlyphsTest.designspace` & `ufo2ft-3.2.4/tests/data/SkipExportGlyphsTest.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/highspacingdot-deva.glif` & `ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/highspacingdot-deva.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SpacingCombiningTest-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/SpacingCombiningTest-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/A.ufo/kerning.plist` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/A.ufo/kerning.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif` & `ufo2ft-3.2.4/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-CFF-compreffor.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-CFF-compreffor.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-CFF.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-CFF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-CFF2-cffsubr.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-CFF2-cffsubr.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-CFF2-compreffor.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-CFF2-compreffor.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-CFF2-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-CFF2-post3.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOptimize-CFF.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOptimize-CFF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOptimize-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOptimize-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-CFF-pathops.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-CFF-pathops.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-CFF.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-CFF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-TTF-pathops.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-TTF-pathops.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-NoOverlaps-TTF.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-NoOverlaps-TTF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-Specialized-CFF.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-Specialized-CFF.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-Specialized-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-Specialized-CFF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-TTF-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-TTF-post3.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont-not-allQuadratic.ttx` & `ufo2ft-3.2.4/tests/data/TestFont-not-allQuadratic.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ttx` & `ufo2ft-3.2.4/tests/data/TestFont.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/d.glif` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/d.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/e.glif` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/e.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/glyphs/f.glif` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/glyphs/f.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestFont.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/TestFont.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.bot.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.bot.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size1.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size1.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size2.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size2.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size3.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size3.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size4.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenleft.size4.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.glif` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/glyphs/parenright.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestMathFont-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/TestMathFont-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarFont-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarFont-MyFontVF1.ttx` & `ufo2ft-3.2.4/tests/data/TestVarFont-MyFontVF1.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarFont-MyFontVF2.ttx` & `ufo2ft-3.2.4/tests/data/TestVarFont-MyFontVF2.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarFont-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarFont-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarFont.designspace` & `ufo2ft-3.2.4/tests/data/TestVarFont.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/alef-ar.fina.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/alef-ar.fina.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/dotabove-ar.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/dotabove-ar.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/glyphs/peh-ar.init.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Bold.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Bold.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/alef-ar.fina.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/alef-ar.fina.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/contents.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/dotabove-ar.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/dotabove-ar.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/layerinfo.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/layerinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.B_R_A_C_K_E_T_.varA_lt01.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.glif` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/glyphs/peh-ar.init.glif`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea-Regular.ufo/lib.plist` & `ufo2ft-3.2.4/tests/data/TestVarfea-Regular.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea.designspace` & `ufo2ft-3.2.4/tests/data/TestVarfea.designspace`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVarfea.glyphs` & `ufo2ft-3.2.4/tests/data/TestVarfea.glyphs`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-cffsubr.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-cffsubr.ttx`

 * *Files 2% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-cffsubr.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-cffsubr.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="OTTO" ttLibVersion="4.44">
+<ttFont sfntVersion="OTTO" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="a"/>
     <GlyphID id="2" name="e"/>
     <GlyphID id="3" name="s"/>
     <GlyphID id="4" name="dotabovecomb"/>
@@ -282,31 +282,39 @@
       <ClassDef glyph="dotabovecomb" class="3"/>
       <ClassDef glyph="e" class="1"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -360,20 +368,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-post3.ttx`

 * *Files 2% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-post3.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="OTTO" ttLibVersion="4.44">
+<ttFont sfntVersion="OTTO" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="a"/>
     <GlyphID id="2" name="e"/>
     <GlyphID id="3" name="s"/>
     <GlyphID id="4" name="uni0307"/>
@@ -268,31 +268,39 @@
       <ClassDef glyph="e" class="1"/>
       <ClassDef glyph="uni0307" class="3"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -346,20 +354,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-sparse-notdefGlyph.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-sparse-notdefGlyph.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-useProductionNames.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-useProductionNames.ttx`

 * *Files 2% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2-useProductionNames.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2-useProductionNames.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="OTTO" ttLibVersion="4.44">
+<ttFont sfntVersion="OTTO" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="uni0061"/>
     <GlyphID id="2" name="uni0065"/>
     <GlyphID id="3" name="uni0073"/>
     <GlyphID id="4" name="uni0307"/>
@@ -285,31 +285,39 @@
       <ClassDef glyph="uni0065" class="1"/>
       <ClassDef glyph="uni0307" class="3"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -363,20 +371,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2.ttx`

 * *Files 1% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-CFF2.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-CFF2.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="OTTO" ttLibVersion="4.44">
+<ttFont sfntVersion="OTTO" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="a"/>
     <GlyphID id="2" name="e"/>
     <GlyphID id="3" name="s"/>
     <GlyphID id="4" name="dotabovecomb"/>
@@ -282,31 +282,39 @@
       <ClassDef glyph="dotabovecomb" class="3"/>
       <ClassDef glyph="e" class="1"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -360,20 +368,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-not-allQuadratic.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-not-allQuadratic.ttx`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-post3.ttx`

 * *Files 0% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-post3.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-post3.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.44">
+<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="a"/>
     <GlyphID id="2" name="e"/>
     <GlyphID id="3" name="s"/>
     <GlyphID id="4" name="uni0307"/>
@@ -275,31 +275,39 @@
       <ClassDef glyph="e" class="1"/>
       <ClassDef glyph="uni0307" class="3"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -353,20 +361,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-useProductionNames.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-useProductionNames.ttx`

 * *Files 0% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF-useProductionNames.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF-useProductionNames.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.44">
+<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="uni0061"/>
     <GlyphID id="2" name="uni0065"/>
     <GlyphID id="3" name="uni0073"/>
     <GlyphID id="4" name="uni0307"/>
@@ -292,31 +292,39 @@
       <ClassDef glyph="uni0065" class="1"/>
       <ClassDef glyph="uni0307" class="3"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -370,20 +378,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF.ttx`

 * *Files 0% similar despite different names*

#### Comparing `ufo2ft-3.2.3/tests/data/TestVariableFont-TTF.ttx` & `ufo2ft-3.2.4/tests/data/TestVariableFont-TTF.ttx`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.44">
+<ttFont sfntVersion="\x00\x01\x00\x00" ttLibVersion="4.51">
   <GlyphOrder>
     <!-- The 'id' attribute is only for humans; it is ignored when parsed. -->
     <GlyphID id="0" name=".notdef"/>
     <GlyphID id="1" name="a"/>
     <GlyphID id="2" name="e"/>
     <GlyphID id="3" name="s"/>
     <GlyphID id="4" name="dotabovecomb"/>
@@ -289,31 +289,39 @@
       <ClassDef glyph="dotabovecomb" class="3"/>
       <ClassDef glyph="e" class="1"/>
     </GlyphClassDef>
     <VarStore Format="1">
       <Format value="1"/>
       <VarRegionList>
         <!-- RegionAxisCount=1 -->
-        <!-- RegionCount=1 -->
+        <!-- RegionCount=2 -->
         <Region index="0">
           <VarRegionAxis index="0">
+            <StartCoord value="0.0"/>
+            <PeakCoord value="0.36365"/>
+            <EndCoord value="1.0"/>
+          </VarRegionAxis>
+        </Region>
+        <Region index="1">
+          <VarRegionAxis index="0">
             <StartCoord value="0.36365"/>
             <PeakCoord value="1.0"/>
             <EndCoord value="1.0"/>
           </VarRegionAxis>
         </Region>
       </VarRegionList>
       <!-- VarDataCount=1 -->
       <VarData index="0">
         <!-- ItemCount=2 -->
         <NumShorts value="0"/>
-        <!-- VarRegionCount=1 -->
+        <!-- VarRegionCount=2 -->
         <VarRegionIndex index="0" value="0"/>
-        <Item index="0" value="[1]"/>
-        <Item index="1" value="[88]"/>
+        <VarRegionIndex index="1" value="1"/>
+        <Item index="0" value="[11, 88]"/>
+        <Item index="1" value="[89, 1]"/>
       </VarData>
     </VarStore>
   </GDEF>
   <GPOS>
     <Version value="0x00010000"/>
     <ScriptList>
       <!-- ScriptCount=1 -->
@@ -367,20 +375,20 @@
             <!-- BaseCount=1 -->
             <BaseRecord index="0">
               <BaseAnchor index="0" Format="3">
                 <XCoordinate value="314"/>
                 <YCoordinate value="556"/>
                 <XDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="0"/>
+                  <EndSize value="1"/>
                   <DeltaFormat value="32768"/>
                 </XDeviceTable>
                 <YDeviceTable>
                   <StartSize value="0"/>
-                  <EndSize value="1"/>
+                  <EndSize value="0"/>
                   <DeltaFormat value="32768"/>
                 </YDeviceTable>
               </BaseAnchor>
             </BaseRecord>
           </BaseArray>
         </MarkBasePos>
       </Lookup>
```

### Comparing `ufo2ft-3.2.3/tests/data/UseMyMetrics.ufo/fontinfo.plist` & `ufo2ft-3.2.4/tests/data/UseMyMetrics.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureCompiler_test.py` & `ufo2ft-3.2.4/tests/featureCompiler_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/__init__.py` & `ufo2ft-3.2.4/tests/featureWriters/__init__.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/ast_test.py` & `ufo2ft-3.2.4/tests/featureWriters/ast_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/cursFeatureWriter_test.py` & `ufo2ft-3.2.4/tests/featureWriters/cursFeatureWriter_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/featureWriters_test.py` & `ufo2ft-3.2.4/tests/featureWriters/featureWriters_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/gdefFeatureWriter_test.py` & `ufo2ft-3.2.4/tests/featureWriters/gdefFeatureWriter_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/kernFeatureWriter2_test.py` & `ufo2ft-3.2.4/tests/featureWriters/kernFeatureWriter2_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/kernFeatureWriter_test.py` & `ufo2ft-3.2.4/tests/featureWriters/kernFeatureWriter_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/featureWriters/markFeatureWriter_test.py` & `ufo2ft-3.2.4/tests/featureWriters/markFeatureWriter_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/decomposeComponents_test.py` & `ufo2ft-3.2.4/tests/filters/decomposeComponents_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/decomposeTransformedComponents_test.py` & `ufo2ft-3.2.4/tests/filters/decomposeTransformedComponents_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/dottedCircle_test.py` & `ufo2ft-3.2.4/tests/filters/dottedCircle_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/explodeColorLayerGlyphs_test.py` & `ufo2ft-3.2.4/tests/filters/explodeColorLayerGlyphs_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/filters_test.py` & `ufo2ft-3.2.4/tests/filters/filters_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/flattenComponents_test.py` & `ufo2ft-3.2.4/tests/filters/flattenComponents_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/propagateAnchors_test.py` & `ufo2ft-3.2.4/tests/filters/propagateAnchors_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/sortContours_test.py` & `ufo2ft-3.2.4/tests/filters/sortContours_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/filters/transformations_test.py` & `ufo2ft-3.2.4/tests/filters/transformations_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/fontInfoData_test.py` & `ufo2ft-3.2.4/tests/fontInfoData_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/infoCompiler_test.py` & `ufo2ft-3.2.4/tests/infoCompiler_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/instantiator_test.py` & `ufo2ft-3.2.4/tests/instantiator_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/instructionCompiler_test.py` & `ufo2ft-3.2.4/tests/instructionCompiler_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/integration_test.py` & `ufo2ft-3.2.4/tests/integration_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             feature liga {
                 sub a e s s by s;
             } liga;
 
             feature mark {
                 lookup mark2base {
                     pos base e
-                        <anchor (wght=350:314 wght=450:314 wght=625:315) (wght=350:556 wght=450:556 wght=625:644)> mark @MC_top;
+                        <anchor (wght=350:314 wght=450:403 wght=625:315) (wght=350:556 wght=450:567 wght=625:644)> mark @MC_top;
                 } mark2base;
 
             } mark;
         """  # noqa: B950
         )
 
     @pytest.mark.parametrize(
```

### Comparing `ufo2ft-3.2.3/tests/outlineCompiler_test.py` & `ufo2ft-3.2.4/tests/outlineCompiler_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/preProcessor_test.py` & `ufo2ft-3.2.4/tests/preProcessor_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/testSupport.py` & `ufo2ft-3.2.4/tests/testSupport.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tests/util_test.py` & `ufo2ft-3.2.4/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `ufo2ft-3.2.3/tox.ini` & `ufo2ft-3.2.4/tox.ini`

 * *Files identical despite different names*

