# Comparing `tmp/pyobjc-framework-Quartz-9.1b1.tar.gz` & `tmp/pyobjc-framework-Quartz-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Quartz-9.1b1.tar", last modified: Sun Mar 26 11:34:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-Quartz-9.2.tar", last modified: Wed Jun  7 00:24:24 2023, max compression
```

## Comparing `pyobjc-framework-Quartz-9.1b1.tar` & `pyobjc-framework-Quartz-9.2.tar`

### file list

```diff
@@ -1,613 +1,614 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.489406 pyobjc-framework-Quartz-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.681768 pyobjc-framework-Quartz-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.670396 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.739356 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/
--rw-r--r--   0 ronald     (501) staff       (20)    14356 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/CGImageUtils.py
--rw-r--r--   0 ronald     (501) staff       (20)     1144 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/CGImageView.py
--rw-r--r--   0 ronald     (501) staff       (20)     8876 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/Controller.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.669778 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.744481 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      844 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      592 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    27672 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/keyedobjects.nib
--rwxr-xr-x   0 ronald     (501) staff       (20)    44087 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/demo.png
--rw-r--r--   0 ronald     (501) staff       (20)      160 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      317 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.751053 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.670236 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.756184 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6112 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     8581 2022-02-06 09:24:04.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/MyQuartzView.py
--rw-r--r--   0 ronald     (501) staff       (20)      137 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      186 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.777600 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/
--rw-r--r--   0 ronald     (501) staff       (20)    13262 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/AppDrawing.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.779052 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.792831 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      577 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    11067 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.794978 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/
--rw-r--r--   0 ronald     (501) staff       (20)   570616 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/ptlobos.tif
--rw-r--r--   0 ronald     (501) staff       (20)      929 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/MyAppController.py
--rw-r--r--   0 ronald     (501) staff       (20)     1978 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/MyView.py
--rw-r--r--   0 ronald     (501) staff       (20)      176 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/UIHandling.py
--rw-r--r--   0 ronald     (501) staff       (20)      125 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      318 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      642 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.803435 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/
--rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/00ReadMe.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.853441 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/
--rw-r--r--   0 ronald     (501) staff       (20)     4713 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/CIBevelView.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.671611 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.855015 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      278 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13843 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5263 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/SampleCIView.py
--rw-r--r--   0 ronald     (501) staff       (20)    60668 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/lightball.tiff
--rw-r--r--   0 ronald     (501) staff       (20)      127 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      299 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.861860 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/
--rw-r--r--   0 ronald     (501) staff       (20)   126105 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/CraterLake.jpg
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.672028 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.874222 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      446 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6337 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1687 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/HazeFilterView.py
--rw-r--r--   0 ronald     (501) staff       (20)     2690 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/MyHazeFilter.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/MyHazeRemoval.cikernel
--rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.899498 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/
--rw-r--r--   0 ronald     (501) staff       (20)     3391 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/CIMicroPaintView.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.672575 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.909478 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      199 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      659 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    16513 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5273 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/SampleCIView.py
--rw-r--r--   0 ronald     (501) staff       (20)      132 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      331 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       45 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.930636 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/
--rw-r--r--   0 ronald     (501) staff       (20)      778 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Blank.jpg
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.672993 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.954458 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      205 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5417 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    22393 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Frog.jpg
--rw-r--r--   0 ronald     (501) staff       (20)    12575 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Mask.jpg
--rw-r--r--   0 ronald     (501) staff       (20)    19473 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Rose.jpg
--rw-r--r--   0 ronald     (501) staff       (20)    52596 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Shading.tiff
--rw-r--r--   0 ronald     (501) staff       (20)     8161 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/TransitionSelectorView.py
--rw-r--r--   0 ronald     (501) staff       (20)      104 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      414 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.673247 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.958948 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.673488 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.972191 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     1900 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      581 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    17085 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13455 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/ImageBrowserController.py
--rw-r--r--   0 ronald     (501) staff       (20)     3480 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)      139 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      154 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.673750 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.027397 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/
--rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/00ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)      142 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/AppDelegate.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.028994 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      594 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/Credits.rtf
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.032358 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      522 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      497 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     4266 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.035788 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      971 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      283 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/data.dependency
--rw-r--r--   0 ronald     (501) staff       (20)      588 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9333 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1480 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/Info.plist
--rw-r--r--   0 ronald     (501) staff       (20)     9046 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/MyPDFDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      128 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/main.py
--rw-r--r--   0 ronald     (501) staff       (20)    40799 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/pdfkitviewer.icns
--rw-r--r--   0 ronald     (501) staff       (20)      350 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       64 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.050075 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/
--rw-r--r--   0 ronald     (501) staff       (20)     5229 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/DemoView.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.674795 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.069496 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      449 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      591 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6898 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      798 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/PathDemoController.py
--rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.071068 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/
--rw-r--r--   0 ronald     (501) staff       (20)     3125 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/00ReadMe.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.175869 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/
--rw-r--r--   0 ronald     (501) staff       (20)      225 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/00ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)    12878 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/AppDrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)    23229 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/BitmapContext.py
--rw-r--r--   0 ronald     (501) staff       (20)    14443 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ColorAndGState.py
--rw-r--r--   0 ronald     (501) staff       (20)     2701 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/CoordinateSystem.py
--rw-r--r--   0 ronald     (501) staff       (20)     6108 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/DataProvidersAndConsumers.py
--rw-r--r--   0 ronald     (501) staff       (20)     9416 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/DrawingBasics.py
--rw-r--r--   0 ronald     (501) staff       (20)     7810 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/EPSPrinting.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.678094 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.199238 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      881 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    29571 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    14200 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/FrameworkTextDrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)     1715 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/FrameworkUtilities.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.231007 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/
--rw-r--r--   0 ronald     (501) staff       (20)   103600 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/400x259x8.bw.raw
--rw-r--r--   0 ronald     (501) staff       (20)   104622 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Kitty.pdf
--rw-r--r--   0 ronald     (501) staff       (20)   114900 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/LyingOnDeckNoProfile.JPG
--rw-r--r--   0 ronald     (501) staff       (20)   171918 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Poot.jpg
--rw-r--r--   0 ronald     (501) staff       (20)   172224 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/blendmode.pdf
--rw-r--r--   0 ronald     (501) staff       (20)   360000 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/image-400x300x24.raw
--rw-r--r--   0 ronald     (501) staff       (20)     2783 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/imageturkey.eps
--rw-r--r--   0 ronald     (501) staff       (20)   360000 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/otherimage-400x300x24.raw
--rw-r--r--   0 ronald     (501) staff       (20)   562708 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/ptlobos.tif
--rw-r--r--   0 ronald     (501) staff       (20)    56222 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ImageMasking.py
--rw-r--r--   0 ronald     (501) staff       (20)    32451 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Images.py
--rw-r--r--   0 ronald     (501) staff       (20)     4123 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/MyAppController.py
--rw-r--r--   0 ronald     (501) staff       (20)     4743 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/MyView.py
--rw-r--r--   0 ronald     (501) staff       (20)     5548 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PDFHandling.py
--rw-r--r--   0 ronald     (501) staff       (20)     8689 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PathDrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)    20808 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PatternDrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)    14759 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/QuartzTextDrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)    25324 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Shadings.py
--rw-r--r--   0 ronald     (501) staff       (20)    11397 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ShadowsAndTransparencyLayers.py
--rw-r--r--   0 ronald     (501) staff       (20)     2584 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/UIHandling.py
--rw-r--r--   0 ronald     (501) staff       (20)    10201 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Utilities.py
--rw-r--r--   0 ronald     (501) staff       (20)      808 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      153 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.239787 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.680244 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.241486 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      189 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      590 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13856 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1413 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/MyView.py
--rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      181 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.243012 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/
--rwxr-xr-x   0 ronald     (501) staff       (20)     5841 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/ConfidentialStamper.py
--rw-r--r--   0 ronald     (501) staff       (20)     6585 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/confidential.pdf
--rw-r--r--   0 ronald     (501) staff       (20)    11867 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/multipagedocumenttostamp.pdf
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.244876 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CreatePDFDocument/
--rw-r--r--   0 ronald     (501) staff       (20)     8485 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CreatePDFDocument/CreatePDFDocument.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.248087 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/PSConverterTool/
--rwxr-xr-x   0 ronald     (501) staff       (20)     4761 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/PSConverterTool/PSConverterTool.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.249499 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ParsePageContents/
--rwxr-xr-x   0 ronald     (501) staff       (20)    10134 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ParsePageContents/parse_page_contents.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.681147 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.265699 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/
--rw-r--r--   0 ronald     (501) staff       (20)     7272 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/AppController.py
--rw-r--r--   0 ronald     (501) staff       (20)    11839 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/Chart.qtz
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.681351 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.271045 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      368 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      282 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/data.dependency
--rw-r--r--   0 ronald     (501) staff       (20)      660 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    17025 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)       95 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      288 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       69 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.311669 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/
--rw-r--r--   0 ronald     (501) staff       (20)      521 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/AppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1109 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/Circle.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.682108 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.317719 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2054 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.319694 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      742 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2158 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      491 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/Extras.py
--rw-r--r--   0 ronald     (501) staff       (20)     3118 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/ShadowOffsetView.py
--rw-r--r--   0 ronald     (501) staff       (20)     1823 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/TLayerDemo.py
--rw-r--r--   0 ronald     (501) staff       (20)     5660 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/TLayerView.py
--rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       37 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Examples/TLayer/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:54.691150 pyobjc-framework-Quartz-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.320449 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.323175 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/
--rw-r--r--   0 ronald     (501) staff       (20)     5073 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2532 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/_contextmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)   118696 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.326353 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreVideo/
--rw-r--r--   0 ronald     (501) staff       (20)      971 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreVideo/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    33286 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreVideo/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.337774 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/
--rw-r--r--   0 ronald     (501) staff       (20)    25142 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/PyObjCOverrides.bridgesupport
--rw-r--r--   0 ronald     (501) staff       (20)      791 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    38023 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.366365 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageKit/
--rw-r--r--   0 ronald     (501) staff       (20)     1038 2021-08-01 13:26:17.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    25742 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.368695 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/PDFKit/
--rw-r--r--   0 ronald     (501) staff       (20)      798 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/PDFKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    24598 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/PDFKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.371885 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzComposer/
--rw-r--r--   0 ronald     (501) staff       (20)      846 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzComposer/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    16013 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzComposer/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.374397 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzCore/
--rw-r--r--   0 ronald     (501) staff       (20)     1798 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    57739 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzCore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.388476 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzFilters/
--rw-r--r--   0 ronald     (501) staff       (20)      789 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzFilters/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2569 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzFilters/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.389822 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuickLookUI/
--rw-r--r--   0 ronald     (501) staff       (20)      896 2021-08-01 13:26:14.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuickLookUI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     7728 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuickLookUI/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.1b1/Lib/Quartz/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.393600 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     3204 2023-03-26 11:34:54.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)    23640 2023-03-26 11:34:54.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:34:54.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:53.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:34:54.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:34:54.000000 pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.445833 pyobjc-framework-Quartz-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     5632 2022-06-30 10:21:22.000000 pyobjc-framework-Quartz-9.1b1/Modules/_CVPixelBuffer.m
--rw-r--r--   0 ronald     (501) staff       (20)     1738 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_CoreGraphics_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)      619 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_CoreImage.m
--rw-r--r--   0 ronald     (501) staff       (20)    13643 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/Modules/_CoreImage_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     1087 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Modules/_ImageKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)      598 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_PDFKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      470 2022-06-23 20:38:27.000000 pyobjc-framework-Quartz-9.1b1/Modules/_PDFKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)      669 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Modules/_QuartzCore_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)      623 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_QuickLookUI.m
--rw-r--r--   0 ronald     (501) staff       (20)      228 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/Modules/_QuickLookUI_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)    46846 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/Modules/_callbacks.m
--rw-r--r--   0 ronald     (501) staff       (20)    20447 2021-10-26 08:03:22.000000 pyobjc-framework-Quartz-9.1b1/Modules/_coregraphics.m
--rw-r--r--   0 ronald     (501) staff       (20)     5971 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_doubleindirect.m
--rw-r--r--   0 ronald     (501) staff       (20)      608 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_imagekit.m
--rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/Modules/_quartzcore.m
--rw-r--r--   0 ronald     (501) staff       (20)     5805 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Modules/_sortandmap.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Quartz-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2993 2023-03-26 11:34:56.489110 pyobjc-framework-Quartz-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.889110 pyobjc-framework-Quartz-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1296 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_IKFilterBrowserPanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      246 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_IKFilterBrowserView.py
--rw-r--r--   0 ronald     (501) staff       (20)     1960 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_IKImageView.py
--rw-r--r--   0 ronald     (501) staff       (20)     8183 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1018 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationButtonWidget.py
--rw-r--r--   0 ronald     (501) staff       (20)      297 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationChoiceWidget.py
--rw-r--r--   0 ronald     (501) staff       (20)      472 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationLine.py
--rw-r--r--   0 ronald     (501) staff       (20)      311 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationMarkup.py
--rw-r--r--   0 ronald     (501) staff       (20)      304 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationPopup.py
--rw-r--r--   0 ronald     (501) staff       (20)      781 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationText.py
--rw-r--r--   0 ronald     (501) staff       (20)      856 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFBorder.py
--rw-r--r--   0 ronald     (501) staff       (20)      280 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFOutline.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFSelection.py
--rw-r--r--   0 ronald     (501) staff       (20)      480 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFThumbnailView.py
--rw-r--r--   0 ronald     (501) staff       (20)     2386 2022-06-25 20:12:54.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)      238 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cabase.py
--rw-r--r--   0 ronald     (501) staff       (20)      289 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cacifilteradditions.py
--rw-r--r--   0 ronald     (501) staff       (20)      612 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caconstraintlayoutmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      234 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caedrmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      993 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caemitterbehavior.py
--rw-r--r--   0 ronald     (501) staff       (20)      377 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caemittercell.py
--rw-r--r--   0 ronald     (501) staff       (20)     2097 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caemitterlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      790 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caframeraterange.py
--rw-r--r--   0 ronald     (501) staff       (20)     1060 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cagradientlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     5698 2022-06-25 20:07:48.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_calayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2911 2022-06-25 09:22:55.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_camediatiming.py
--rw-r--r--   0 ronald     (501) staff       (20)      704 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_camediatimingfunction.py
--rw-r--r--   0 ronald     (501) staff       (20)     1144 2022-06-25 20:07:01.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cametallayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      990 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caopengllayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      649 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_carenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      321 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_careplicatorlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      507 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cascrolllayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      875 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cashapelayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1301 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catextlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      885 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catransaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     3297 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catransform3d.py
--rw-r--r--   0 ronald     (501) staff       (20)     1010 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cavaluefunction.py
--rw-r--r--   0 ronald     (501) staff       (20)     4172 2022-06-26 19:52:36.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgaffinetransform.py
--rw-r--r--   0 ronald     (501) staff       (20)      293 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgbase.py
--rw-r--r--   0 ronald     (501) staff       (20)     2678 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgbitmapcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     3432 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1483 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorconversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     1066 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorconvertor.py
--rw-r--r--   0 ronald     (501) staff       (20)    12458 2022-10-21 10:39:53.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorspace.py
--rw-r--r--   0 ronald     (501) staff       (20)    25329 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      870 2021-08-04 09:43:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgconvertcolordatawithformat.py
--rw-r--r--   0 ronald     (501) staff       (20)     2224 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdataconsumer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2194 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdataprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)    14800 2021-04-09 10:15:21.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdirectdisplay.py
--rw-r--r--   0 ronald     (501) staff       (20)      341 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdirectdisplaymetal.py
--rw-r--r--   0 ronald     (501) staff       (20)     2921 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdirectpalette.py
--rw-r--r--   0 ronald     (501) staff       (20)     6180 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplayconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     1373 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplayfade.py
--rw-r--r--   0 ronald     (501) staff       (20)     3049 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplaystream.py
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     6583 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     2308 2021-04-09 10:15:21.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgeventsource.py
--rw-r--r--   0 ronald     (501) staff       (20)     9180 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgeventtypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     6440 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgfont.py
--rw-r--r--   0 ronald     (501) staff       (20)     2085 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgfunction.py
--rw-r--r--   0 ronald     (501) staff       (20)     7600 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cggeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)      247 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgglcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1396 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cggradient.py
--rw-r--r--   0 ronald     (501) staff       (20)     9682 2021-04-09 10:15:21.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1203 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimageanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)     4909 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagedestination.py
--rw-r--r--   0 ronald     (501) staff       (20)     6010 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagemetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)    57177 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimageproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)     3098 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagesource.py
--rw-r--r--   0 ronald     (501) staff       (20)     1937 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cglayer.py
--rw-r--r--   0 ronald     (501) staff       (20)    10069 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpath.py
--rw-r--r--   0 ronald     (501) staff       (20)     2506 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpattern.py
--rw-r--r--   0 ronald     (501) staff       (20)     1709 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     2245 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfcontentstream.py
--rw-r--r--   0 ronald     (501) staff       (20)     7723 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1435 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfdictionary.py
--rw-r--r--   0 ronald     (501) staff       (20)     2687 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     1005 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfobject.py
--rw-r--r--   0 ronald     (501) staff       (20)      646 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfoperatortable.py
--rw-r--r--   0 ronald     (501) staff       (20)      783 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfpage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1991 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfscanner.py
--rw-r--r--   0 ronald     (501) staff       (20)      581 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfstream.py
--rw-r--r--   0 ronald     (501) staff       (20)      454 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfstring.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpsconverter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4788 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgremoteoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1321 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgshading.py
--rw-r--r--   0 ronald     (501) staff       (20)     4072 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgwindow.py
--rw-r--r--   0 ronald     (501) staff       (20)     4884 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgwindowlevel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1042 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cibarcodedescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      184 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cicolor.py
--rw-r--r--   0 ronald     (501) staff       (20)     4410 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cicontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1647 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cidetector.py
--rw-r--r--   0 ronald     (501) staff       (20)     1223 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifeature.py
--rw-r--r--   0 ronald     (501) staff       (20)     7086 2022-06-25 20:09:13.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifilter.py
--rw-r--r--   0 ronald     (501) staff       (20)    66592 2022-06-25 09:22:20.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifilterbuiltins.py
--rw-r--r--   0 ronald     (501) staff       (20)      554 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifiltergenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)      199 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifiltershape.py
--rw-r--r--   0 ronald     (501) staff       (20)     5615 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1691 2022-06-25 09:22:04.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimageprocessor.py
--rw-r--r--   0 ronald     (501) staff       (20)     2103 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimageprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     1306 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cikernel.py
--rw-r--r--   0 ronald     (501) staff       (20)      351 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)      379 2022-06-25 20:08:58.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciplugininterface.py
--rw-r--r--   0 ronald     (501) staff       (20)     4496 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cirawfilter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1980 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cirenderdestination.py
--rw-r--r--   0 ronald     (501) staff       (20)      833 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cisampler.py
--rw-r--r--   0 ronald     (501) staff       (20)      414 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_civector.py
--rw-r--r--   0 ronald     (501) staff       (20)      262 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_coreimagedefines.py
--rw-r--r--   0 ronald     (501) staff       (20)     2914 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvbase.py
--rw-r--r--   0 ronald     (501) staff       (20)     4415 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     5019 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvdisplaylink.py
--rw-r--r--   0 ronald     (501) staff       (20)      379 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvhosttime.py
--rw-r--r--   0 ronald     (501) staff       (20)     7879 2021-10-29 07:58:20.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvimagebuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1085 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvmetaltexture.py
--rw-r--r--   0 ronald     (501) staff       (20)      560 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvmetaltexturecache.py
--rw-r--r--   0 ronald     (501) staff       (20)     1320 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopenglbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1856 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopenglbufferpool.py
--rw-r--r--   0 ronald     (501) staff       (20)     1149 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopengltexture.py
--rw-r--r--   0 ronald     (501) staff       (20)     1237 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopengltexturecache.py
--rw-r--r--   0 ronald     (501) staff       (20)    17721 2021-10-29 07:58:20.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      781 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbufferiosurface.py
--rw-r--r--   0 ronald     (501) staff       (20)     3189 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbufferpool.py
--rw-r--r--   0 ronald     (501) staff       (20)     3761 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelformatdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)     1402 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvreturn.py
--rw-r--r--   0 ronald     (501) staff       (20)     1995 2022-06-25 20:09:59.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikcameradeviceview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1251 2022-06-25 20:09:32.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikdevicebrowserview.py
--rw-r--r--   0 ronald     (501) staff       (20)      713 2022-06-25 09:23:00.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikfilterui.py
--rw-r--r--   0 ronald     (501) staff       (20)     1508 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimagebrowsercell.py
--rw-r--r--   0 ronald     (501) staff       (20)     7390 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimagebrowserview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1222 2022-06-25 20:05:12.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimageeditpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     2049 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikpicturetaker.py
--rw-r--r--   0 ronald     (501) staff       (20)      387 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_iksaveoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1482 2022-06-25 20:08:05.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikscannerdeviceview.py
--rw-r--r--   0 ronald     (501) staff       (20)     2989 2022-06-25 09:23:47.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikslideshow.py
--rw-r--r--   0 ronald     (501) staff       (20)     3705 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_imagekitdeprecated.py
--rw-r--r--   0 ronald     (501) staff       (20)      927 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfactionnamed.py
--rw-r--r--   0 ronald     (501) staff       (20)      300 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfactionresetform.py
--rw-r--r--   0 ronald     (501) staff       (20)      201 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfannotationlink.py
--rw-r--r--   0 ronald     (501) staff       (20)      246 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfannotationstamp.py
--rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfannotationtextwidget.py
--rw-r--r--   0 ronald     (501) staff       (20)     5912 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfannotationutilities.py
--rw-r--r--   0 ronald     (501) staff       (20)      849 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfappearancecharacteristics.py
--rw-r--r--   0 ronald     (501) staff       (20)      244 2021-08-04 10:11:58.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfdestination.py
--rw-r--r--   0 ronald     (501) staff       (20)     5559 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     2442 2022-06-26 21:30:12.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfkitplatform.py
--rw-r--r--   0 ronald     (501) staff       (20)     1213 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfpage.py
--rw-r--r--   0 ronald     (501) staff       (20)      217 2022-06-25 20:10:13.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfpageoverlayviewprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     6115 2022-06-26 21:30:12.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1220 2022-06-25 20:06:37.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_plpreviewpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     3318 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccomposition.py
--rw-r--r--   0 ronald     (501) staff       (20)      776 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionparameterview.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionpickerpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      965 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionpickerview.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionrepository.py
--rw-r--r--   0 ronald     (501) staff       (20)     2964 2022-06-26 19:55:10.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)      420 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcpluginviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      630 2022-06-25 20:12:12.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      908 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcview.py
--rw-r--r--   0 ronald     (501) staff       (20)      989 2022-06-25 20:08:07.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewingcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      229 2022-06-26 21:30:39.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1764 2022-06-25 09:24:26.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      730 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewview.py
--rw-r--r--   0 ronald     (501) staff       (20)      361 2022-04-12 20:05:18.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_quartz.py
--rw-r--r--   0 ronald     (501) staff       (20)      231 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_quartzfilter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1258 2022-10-18 09:54:01.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_quartzfiltermanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      785 2021-08-04 09:06:36.000000 pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_sqlpreviewreply.py
--rw-r--r--   0 ronald     (501) staff       (20)      420 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.903023 pyobjc-framework-Quartz-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)   121787 2022-10-20 21:08:30.000000 pyobjc-framework-Quartz-9.1b1/metadata/CoreGraphics.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    20359 2021-08-15 08:32:12.000000 pyobjc-framework-Quartz-9.1b1/metadata/CoreVideo.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    30897 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.1b1/metadata/ImageIO.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3219 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/ImageKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    14543 2022-10-20 21:08:30.000000 pyobjc-framework-Quartz-9.1b1/metadata/PDFKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     4189 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/QuartzComposer.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    67189 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/QuartzCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      507 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/QuartzFilters.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1356 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/QuickLookUI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1359 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:55.983252 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/
--rw-r--r--   0 ronald     (501) staff       (20)   209211 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   211750 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   223907 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   223907 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   189439 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   204044 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   204782 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   188720 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   190950 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   196616 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   209235 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   211774 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   223931 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   223931 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.019981 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/
--rw-r--r--   0 ronald     (501) staff       (20)   697577 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   697773 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   665671 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   697578 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   697774 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.071509 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/
--rw-r--r--   0 ronald     (501) staff       (20)    58174 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    58535 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60815 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60815 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    44590 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53605 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    55471 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41422 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42902 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43943 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    58175 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    58536 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60816 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60816 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.204961 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/
--rw-r--r--   0 ronald     (501) staff       (20)    78023 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    78366 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80181 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80262 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45215 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    72468 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    75473 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76791 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31000 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    32148 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43265 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    78024 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    78367 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80182 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80263 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.283272 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/
--rw-r--r--   0 ronald     (501) staff       (20)   109729 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   110055 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   111332 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    75428 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   107160 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   107238 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    84915 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    79390 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    66449 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   109730 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   110056 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   111333 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.322075 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/
--rw-r--r--   0 ronald     (501) staff       (20)   181502 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   182255 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   187475 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   187611 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   113728 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   180545 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   180610 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   112401 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   112987 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   181503 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   182256 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   187476 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   187612 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.356326 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/
--rw-r--r--   0 ronald     (501) staff       (20)    60893 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60912 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61198 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60860 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60698 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60896 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60894 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60449 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60777 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60832 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60894 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60913 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61199 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.422963 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/
--rw-r--r--   0 ronald     (501) staff       (20)   193121 2021-10-25 15:33:38.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   193344 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   195644 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   195689 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   260453 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   190737 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   190824 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   135035 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   143939 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   147726 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   193122 2021-10-25 15:33:38.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   193345 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   195645 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   195690 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.462920 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/
--rw-r--r--   0 ronald     (501) staff       (20)     9624 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9643 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9671 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9620 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9637 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9635 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9477 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9477 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9593 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9625 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9644 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9672 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:56.488377 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/
--rw-r--r--   0 ronald     (501) staff       (20)    25148 2021-08-04 10:01:02.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25220 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25355 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16119 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    17243 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    17699 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8568 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10508 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10576 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25149 2021-08-04 10:01:02.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25221 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25356 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:34:56.489681 pyobjc-framework-Quartz-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     3976 2023-03-25 14:20:32.000000 pyobjc-framework-Quartz-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.835265 pyobjc-framework-Quartz-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.908070 pyobjc-framework-Quartz-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.898954 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.938197 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/
+-rw-r--r--   0 ronald     (501) staff       (20)    14356 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/CGImageUtils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1144 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/CGImageView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8876 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/Controller.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.898182 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.941063 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      844 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      592 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    27672 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/keyedobjects.nib
+-rwxr-xr-x   0 ronald     (501) staff       (20)    44087 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/demo.png
+-rw-r--r--   0 ronald     (501) staff       (20)      160 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      317 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.946733 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.898759 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.949062 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6112 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     8581 2022-02-06 09:24:04.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/MyQuartzView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      137 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      186 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.958501 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/
+-rw-r--r--   0 ronald     (501) staff       (20)    13262 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/AppDrawing.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.959054 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.961293 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      577 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    11067 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.961892 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/
+-rw-r--r--   0 ronald     (501) staff       (20)   570616 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/ptlobos.tif
+-rw-r--r--   0 ronald     (501) staff       (20)      929 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/MyAppController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1978 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/MyView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      176 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/UIHandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)      125 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      318 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      642 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.964114 pyobjc-framework-Quartz-9.2/Examples/Core Image/
+-rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/00ReadMe.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.968659 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/
+-rw-r--r--   0 ronald     (501) staff       (20)     4713 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/CIBevelView.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.900519 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.980939 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      278 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13843 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5263 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/SampleCIView.py
+-rw-r--r--   0 ronald     (501) staff       (20)    60668 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/lightball.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)      127 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      299 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.988005 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/
+-rw-r--r--   0 ronald     (501) staff       (20)   126105 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/CraterLake.jpg
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.901076 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.996539 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      446 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6337 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1687 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/HazeFilterView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2690 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/MyHazeFilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/MyHazeRemoval.cikernel
+-rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.004313 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/
+-rw-r--r--   0 ronald     (501) staff       (20)     3391 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/CIMicroPaintView.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.901629 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.007182 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      199 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    16513 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5273 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/SampleCIView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      132 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      331 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.013806 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/
+-rw-r--r--   0 ronald     (501) staff       (20)      778 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Blank.jpg
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.902178 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.015565 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      205 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5417 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    22393 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Frog.jpg
+-rw-r--r--   0 ronald     (501) staff       (20)    12575 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Mask.jpg
+-rw-r--r--   0 ronald     (501) staff       (20)    19473 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Rose.jpg
+-rw-r--r--   0 ronald     (501) staff       (20)    52596 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Shading.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)     8161 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/TransitionSelectorView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      104 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      414 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.902520 pyobjc-framework-Quartz-9.2/Examples/ImageKit/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.019528 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.902867 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.031047 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     1900 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      581 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    17085 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13455 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/ImageBrowserController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3480 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      139 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      154 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.903390 pyobjc-framework-Quartz-9.2/Examples/PDFKit/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.049386 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/
+-rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/00ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      142 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/AppDelegate.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.050755 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      594 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/Credits.rtf
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.062714 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      522 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      497 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     4266 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.067066 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      971 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      283 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/data.dependency
+-rw-r--r--   0 ronald     (501) staff       (20)      588 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9333 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1480 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/Info.plist
+-rw-r--r--   0 ronald     (501) staff       (20)     9046 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/MyPDFDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      128 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)    40799 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/pdfkitviewer.icns
+-rw-r--r--   0 ronald     (501) staff       (20)      350 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       64 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.081472 pyobjc-framework-Quartz-9.2/Examples/PathDemo/
+-rw-r--r--   0 ronald     (501) staff       (20)     5229 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/DemoView.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.904641 pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.084367 pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      449 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      591 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6898 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/PathDemoController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      130 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/PathDemo/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.085281 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/
+-rw-r--r--   0 ronald     (501) staff       (20)     3125 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/00ReadMe.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.112316 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/
+-rw-r--r--   0 ronald     (501) staff       (20)      225 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/00ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    12878 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/AppDrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23229 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/BitmapContext.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14443 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ColorAndGState.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2701 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/CoordinateSystem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6108 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/DataProvidersAndConsumers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9416 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/DrawingBasics.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7810 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/EPSPrinting.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.905475 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.122312 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      881 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    29571 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    14200 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/FrameworkTextDrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1715 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/FrameworkUtilities.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.151810 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/
+-rw-r--r--   0 ronald     (501) staff       (20)   103600 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/400x259x8.bw.raw
+-rw-r--r--   0 ronald     (501) staff       (20)   104622 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Kitty.pdf
+-rw-r--r--   0 ronald     (501) staff       (20)   114900 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/LyingOnDeckNoProfile.JPG
+-rw-r--r--   0 ronald     (501) staff       (20)   171918 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Poot.jpg
+-rw-r--r--   0 ronald     (501) staff       (20)   172224 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/blendmode.pdf
+-rw-r--r--   0 ronald     (501) staff       (20)   360000 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/image-400x300x24.raw
+-rw-r--r--   0 ronald     (501) staff       (20)     2783 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/imageturkey.eps
+-rw-r--r--   0 ronald     (501) staff       (20)   360000 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/otherimage-400x300x24.raw
+-rw-r--r--   0 ronald     (501) staff       (20)   562708 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/ptlobos.tif
+-rw-r--r--   0 ronald     (501) staff       (20)    56222 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ImageMasking.py
+-rw-r--r--   0 ronald     (501) staff       (20)    32451 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Images.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4123 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/MyAppController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4743 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/MyView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5548 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PDFHandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8689 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PathDrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20808 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PatternDrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14759 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/QuartzTextDrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)    25324 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Shadings.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11397 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ShadowsAndTransparencyLayers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2584 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/UIHandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10201 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Utilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)      808 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      153 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.171358 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.906237 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.173644 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      189 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      590 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13856 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1413 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/MyView.py
+-rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      181 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.175557 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/
+-rwxr-xr-x   0 ronald     (501) staff       (20)     5841 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/ConfidentialStamper.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6585 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/confidential.pdf
+-rw-r--r--   0 ronald     (501) staff       (20)    11867 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/multipagedocumenttostamp.pdf
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.176174 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CreatePDFDocument/
+-rw-r--r--   0 ronald     (501) staff       (20)     8485 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CreatePDFDocument/CreatePDFDocument.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.176885 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/PSConverterTool/
+-rwxr-xr-x   0 ronald     (501) staff       (20)     4761 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/PSConverterTool/PSConverterTool.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.177691 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ParsePageContents/
+-rwxr-xr-x   0 ronald     (501) staff       (20)    10134 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ParsePageContents/parse_page_contents.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.907335 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.180509 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/
+-rw-r--r--   0 ronald     (501) staff       (20)     7272 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/AppController.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11839 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/Chart.qtz
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.907864 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.182801 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      368 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/data.dependency
+-rw-r--r--   0 ronald     (501) staff       (20)      660 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    17025 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)       95 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      288 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       69 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.197986 pyobjc-framework-Quartz-9.2/Examples/TLayer/
+-rw-r--r--   0 ronald     (501) staff       (20)      521 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/AppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1109 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/Circle.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.908611 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.207803 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2054 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.212998 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      742 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2158 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      491 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/Extras.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3118 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/ShadowOffsetView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1823 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/TLayerDemo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5660 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/TLayerView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       37 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Examples/TLayer/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Quartz-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:23.911024 pyobjc-framework-Quartz-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.213965 pyobjc-framework-Quartz-9.2/Lib/Quartz/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.217727 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/
+-rw-r--r--   0 ronald     (501) staff       (20)     5073 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2532 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/_contextmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)   118247 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.230554 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreVideo/
+-rw-r--r--   0 ronald     (501) staff       (20)      971 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreVideo/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    33264 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreVideo/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.235292 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/
+-rw-r--r--   0 ronald     (501) staff       (20)    25142 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/PyObjCOverrides.bridgesupport
+-rw-r--r--   0 ronald     (501) staff       (20)      791 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    38023 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.238365 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageKit/
+-rw-r--r--   0 ronald     (501) staff       (20)     1038 2021-08-01 13:26:17.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    25742 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.241011 pyobjc-framework-Quartz-9.2/Lib/Quartz/PDFKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/PDFKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24598 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/PDFKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.250003 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzComposer/
+-rw-r--r--   0 ronald     (501) staff       (20)      846 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzComposer/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16013 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzComposer/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.252302 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzCore/
+-rw-r--r--   0 ronald     (501) staff       (20)     1798 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    57739 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzCore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.254181 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzFilters/
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2021-08-01 13:26:16.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzFilters/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2569 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzFilters/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.255724 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuickLookUI/
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2021-08-01 13:26:14.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuickLookUI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7728 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/QuickLookUI/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1932 2021-08-01 13:26:15.000000 pyobjc-framework-Quartz-9.2/Lib/Quartz/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.258951 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     3202 2023-06-07 00:24:23.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)    23655 2023-06-07 00:24:23.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:24:23.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:53.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:24:23.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:24:23.000000 pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.275947 pyobjc-framework-Quartz-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     5632 2022-06-30 10:21:22.000000 pyobjc-framework-Quartz-9.2/Modules/_CVPixelBuffer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1738 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_CoreGraphics_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)      619 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_CoreImage.m
+-rw-r--r--   0 ronald     (501) staff       (20)    13643 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/Modules/_CoreImage_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1087 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Modules/_ImageKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_PDFKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      470 2022-06-23 20:38:27.000000 pyobjc-framework-Quartz-9.2/Modules/_PDFKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)      669 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Modules/_QuartzCore_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)      623 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_QuickLookUI.m
+-rw-r--r--   0 ronald     (501) staff       (20)      228 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/Modules/_QuickLookUI_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)    46846 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/Modules/_callbacks.m
+-rw-r--r--   0 ronald     (501) staff       (20)    20447 2021-10-26 08:03:22.000000 pyobjc-framework-Quartz-9.2/Modules/_coregraphics.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5971 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_doubleindirect.m
+-rw-r--r--   0 ronald     (501) staff       (20)      608 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_imagekit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/Modules/_quartzcore.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5805 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/Modules/_sortandmap.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Quartz-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2991 2023-06-07 00:24:24.834801 pyobjc-framework-Quartz-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.536974 pyobjc-framework-Quartz-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1296 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_IKFilterBrowserPanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      246 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_IKFilterBrowserView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1960 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_IKImageView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8183 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1018 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationButtonWidget.py
+-rw-r--r--   0 ronald     (501) staff       (20)      297 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationChoiceWidget.py
+-rw-r--r--   0 ronald     (501) staff       (20)      472 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationLine.py
+-rw-r--r--   0 ronald     (501) staff       (20)      311 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationMarkup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      304 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationPopup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationText.py
+-rw-r--r--   0 ronald     (501) staff       (20)      856 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFBorder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      280 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFOutline.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFSelection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      480 2022-10-18 09:53:24.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFThumbnailView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2386 2022-06-25 20:12:54.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cabase.py
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cacifilteradditions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      612 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caconstraintlayoutmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      234 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caedrmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      993 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caemitterbehavior.py
+-rw-r--r--   0 ronald     (501) staff       (20)      377 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caemittercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2097 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caemitterlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      790 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caframeraterange.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1060 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cagradientlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5698 2022-06-25 20:07:48.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_calayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2911 2022-06-25 09:22:55.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_camediatiming.py
+-rw-r--r--   0 ronald     (501) staff       (20)      704 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_camediatimingfunction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1144 2022-06-25 20:07:01.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cametallayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      990 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_caopengllayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      649 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_carenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      321 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_careplicatorlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      507 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cascrolllayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      875 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cashapelayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1301 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_catextlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      885 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_catransaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3297 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_catransform3d.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1010 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cavaluefunction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4172 2022-06-26 19:52:36.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgaffinetransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)      293 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2678 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgbitmapcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3432 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1483 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorconversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1066 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorconvertor.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12458 2022-10-21 10:39:53.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorspace.py
+-rw-r--r--   0 ronald     (501) staff       (20)    25491 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      870 2021-08-04 09:43:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgconvertcolordatawithformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2224 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdataconsumer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2194 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdataprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14800 2021-04-09 10:15:21.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdirectdisplay.py
+-rw-r--r--   0 ronald     (501) staff       (20)      341 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdirectdisplaymetal.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2921 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdirectpalette.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6180 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplayconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1373 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplayfade.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3049 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplaystream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1932 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6583 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2308 2021-04-09 10:15:21.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgeventsource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9180 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgeventtypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6440 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgfont.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2085 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgfunction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7600 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cggeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      247 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgglcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1396 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cggradient.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9834 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1203 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimageanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4909 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagedestination.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6010 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagemetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)    57177 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimageproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3098 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagesource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1937 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cglayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10069 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpath.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2506 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpattern.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1709 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2245 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfcontentstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7723 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1435 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfdictionary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2687 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1005 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      646 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfoperatortable.py
+-rw-r--r--   0 ronald     (501) staff       (20)      783 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfpage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1991 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfscanner.py
+-rw-r--r--   0 ronald     (501) staff       (20)      581 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpsconverter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4788 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgremoteoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1321 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1885 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgshading.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4072 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgwindow.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4884 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgwindowlevel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1042 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cibarcodedescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      184 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cicolor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4410 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cicontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1647 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cidetector.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1223 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifeature.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7086 2022-06-25 20:09:13.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    66592 2022-06-25 09:22:20.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifilterbuiltins.py
+-rw-r--r--   0 ronald     (501) staff       (20)      554 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifiltergenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      199 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifiltershape.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5615 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1691 2022-06-25 09:22:04.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimageprocessor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2103 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimageprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1306 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cikernel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      351 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2022-06-25 20:08:58.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciplugininterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4496 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cirawfilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1980 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cirenderdestination.py
+-rw-r--r--   0 ronald     (501) staff       (20)      833 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cisampler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      414 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_civector.py
+-rw-r--r--   0 ronald     (501) staff       (20)      262 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_coreimagedefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2914 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4415 2021-07-30 09:00:38.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5019 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvdisplaylink.py
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvhosttime.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7879 2021-10-29 07:58:20.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvimagebuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1085 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvmetaltexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)      744 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvmetaltexturecache.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1320 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopenglbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1856 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopenglbufferpool.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1149 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopengltexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1237 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopengltexturecache.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17847 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbufferiosurface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3189 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbufferpool.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3761 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelformatdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1402 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvreturn.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1995 2022-06-25 20:09:59.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikcameradeviceview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1251 2022-06-25 20:09:32.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikdevicebrowserview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      713 2022-06-25 09:23:00.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikfilterui.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1508 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimagebrowsercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7390 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimagebrowserview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1222 2022-06-25 20:05:12.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimageeditpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2049 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikpicturetaker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      387 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_iksaveoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1482 2022-06-25 20:08:05.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikscannerdeviceview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2989 2022-06-25 09:23:47.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikslideshow.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3705 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_imagekitdeprecated.py
+-rw-r--r--   0 ronald     (501) staff       (20)      927 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfactionnamed.py
+-rw-r--r--   0 ronald     (501) staff       (20)      300 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfactionresetform.py
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfannotationlink.py
+-rw-r--r--   0 ronald     (501) staff       (20)      246 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfannotationstamp.py
+-rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfannotationtextwidget.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5912 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfannotationutilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)      849 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfappearancecharacteristics.py
+-rw-r--r--   0 ronald     (501) staff       (20)      244 2021-08-04 10:11:58.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfdestination.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5559 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2442 2022-06-26 21:30:12.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfkitplatform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1213 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfpage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      259 2023-05-04 11:00:07.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfpageoverlayviewprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6115 2022-06-26 21:30:12.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1220 2022-06-25 20:06:37.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_plpreviewpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3318 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccomposition.py
+-rw-r--r--   0 ronald     (501) staff       (20)      776 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionparameterview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionpickerpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      965 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionpickerview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionrepository.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2964 2022-06-26 19:55:10.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)      420 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcpluginviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      630 2022-06-25 20:12:12.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      908 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      989 2022-06-25 20:08:07.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewingcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      229 2022-06-26 21:30:39.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1764 2022-06-25 09:24:26.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      730 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      361 2022-04-12 20:05:18.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_quartz.py
+-rw-r--r--   0 ronald     (501) staff       (20)      231 2021-03-21 10:08:23.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_quartzfilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1258 2022-10-18 09:54:01.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_quartzfiltermanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      785 2021-08-04 09:06:36.000000 pyobjc-framework-Quartz-9.2/PyObjCTest/test_sqlpreviewreply.py
+-rw-r--r--   0 ronald     (501) staff       (20)      420 2021-10-18 19:38:40.000000 pyobjc-framework-Quartz-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.552412 pyobjc-framework-Quartz-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)   121089 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/metadata/CoreGraphics.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21056 2023-05-27 09:46:33.000000 pyobjc-framework-Quartz-9.2/metadata/CoreVideo.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    30897 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.2/metadata/ImageIO.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3219 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/ImageKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    14543 2022-10-20 21:08:30.000000 pyobjc-framework-Quartz-9.2/metadata/PDFKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     4189 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/QuartzComposer.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    67189 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/QuartzCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      507 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/QuartzFilters.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1356 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/QuickLookUI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1359 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.591513 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/
+-rw-r--r--   0 ronald     (501) staff       (20)   209211 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   211750 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   223907 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   223907 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   189439 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   204044 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   204782 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   188720 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   190950 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   196616 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   209235 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   211774 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   223931 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   223931 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.613994 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/
+-rw-r--r--   0 ronald     (501) staff       (20)   697577 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   697773 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   665671 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   697578 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   697774 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.644627 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/
+-rw-r--r--   0 ronald     (501) staff       (20)    58174 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    58535 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60815 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60815 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    44590 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53605 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    55471 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41422 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42902 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43943 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    58175 2022-01-02 11:04:26.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    58536 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60816 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60816 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.679349 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/
+-rw-r--r--   0 ronald     (501) staff       (20)    78023 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    78366 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80181 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80262 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45215 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    72468 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    75473 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76791 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31000 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    32148 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43265 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    78024 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    78367 2022-02-24 08:47:16.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80182 2022-07-08 16:02:54.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80263 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.706325 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/
+-rw-r--r--   0 ronald     (501) staff       (20)   109729 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   110055 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   111332 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    75428 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   107160 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   107238 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    84915 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    79390 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    66449 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   109730 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   110056 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   111333 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.730583 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/
+-rw-r--r--   0 ronald     (501) staff       (20)   181502 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   182255 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   187475 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   187611 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   113728 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   180545 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   180610 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   112401 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   112987 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   181503 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   182256 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   187476 2022-10-18 09:53:23.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   187612 2023-03-24 18:54:07.000000 pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.757628 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/
+-rw-r--r--   0 ronald     (501) staff       (20)    60893 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60912 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61198 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60860 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60698 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60896 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60894 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60449 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60777 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60832 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60894 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60913 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61199 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.790497 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/
+-rw-r--r--   0 ronald     (501) staff       (20)   193121 2021-10-25 15:33:38.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   193344 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   195644 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   195689 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   260453 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   190737 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   190824 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   135035 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   143939 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   147726 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   193122 2021-10-25 15:33:38.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   193345 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   195645 2022-06-15 11:57:00.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   195690 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.803758 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/
+-rw-r--r--   0 ronald     (501) staff       (20)     9624 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9643 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9671 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9620 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9637 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9635 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9477 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9477 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9593 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9625 2021-08-04 10:01:04.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9644 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9672 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:24.833291 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/
+-rw-r--r--   0 ronald     (501) staff       (20)    25148 2021-08-04 10:01:02.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25220 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25355 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16119 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    17243 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    17699 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8568 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10508 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10576 2021-08-04 09:50:01.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25149 2021-08-04 10:01:02.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25221 2022-02-24 08:47:17.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25356 2023-02-19 10:50:35.000000 pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Quartz-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Quartz-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:24:24.835361 pyobjc-framework-Quartz-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     4047 2023-05-29 10:07:47.000000 pyobjc-framework-Quartz-9.2/setup.py
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/CGImageUtils.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/CGImageUtils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/CGImageView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/CGImageView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/Controller.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/Controller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGRotation/demo.png` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGRotation/demo.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/CGShading Demo/MyQuartzView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/CGShading Demo/MyQuartzView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/AppDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/AppDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/ptlobos.tif` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/GraphicsFiles/ptlobos.tif`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/MyAppController.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/MyAppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/MyView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/MyView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Graphics/Quartz2DBasics/summary.txt` & `pyobjc-framework-Quartz-9.2/Examples/Core Graphics/Quartz2DBasics/summary.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/CIBevelView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/CIBevelView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/SampleCIView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/SampleCIView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIBevelSample/lightball.tiff` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIBevelSample/lightball.tiff`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/CraterLake.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/CraterLake.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/HazeFilterView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/HazeFilterView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIHazeFilterSample/MyHazeFilter.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIHazeFilterSample/MyHazeFilter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/CIMicroPaintView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/CIMicroPaintView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CIMicroPaint/SampleCIView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CIMicroPaint/SampleCIView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Blank.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Blank.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Frog.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Frog.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Mask.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Mask.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Rose.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Rose.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/Shading.tiff` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/Shading.tiff`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Core Image/CITransitionSelectorSample/TransitionSelectorView.py` & `pyobjc-framework-Quartz-9.2/Examples/Core Image/CITransitionSelectorSample/TransitionSelectorView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/ImageBrowserController.py` & `pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/ImageBrowserController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/ImageKit/ImageBrowser/ReadMe.txt` & `pyobjc-framework-Quartz-9.2/Examples/ImageKit/ImageBrowser/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/Credits.rtf` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/Credits.rtf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/English.lproj/MyDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/Info.plist` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/Info.plist`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/MyPDFDocument.py` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/MyPDFDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PDFKit/PDFKitViewer/pdfkitviewer.icns` & `pyobjc-framework-Quartz-9.2/Examples/PDFKit/PDFKitViewer/pdfkitviewer.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/DemoView.py` & `pyobjc-framework-Quartz-9.2/Examples/PathDemo/DemoView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/PathDemo/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/PathDemo/PathDemoController.py` & `pyobjc-framework-Quartz-9.2/Examples/PathDemo/PathDemoController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/00ReadMe.txt` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/00ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/AppDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/AppDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/BitmapContext.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/BitmapContext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ColorAndGState.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ColorAndGState.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/CoordinateSystem.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/CoordinateSystem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/DataProvidersAndConsumers.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/DataProvidersAndConsumers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/DrawingBasics.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/DrawingBasics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/EPSPrinting.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/EPSPrinting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/FrameworkTextDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/FrameworkTextDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/FrameworkUtilities.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/FrameworkUtilities.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/400x259x8.bw.raw` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/400x259x8.bw.raw`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Kitty.pdf` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Kitty.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/LyingOnDeckNoProfile.JPG` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/LyingOnDeckNoProfile.JPG`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Poot.jpg` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/Poot.jpg`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/blendmode.pdf` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/blendmode.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/image-400x300x24.raw` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/image-400x300x24.raw`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/imageturkey.eps` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/imageturkey.eps`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/otherimage-400x300x24.raw` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/otherimage-400x300x24.raw`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/ptlobos.tif` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/GraphicsFiles/ptlobos.tif`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ImageMasking.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ImageMasking.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Images.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Images.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/MyAppController.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/MyAppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/MyView.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/MyView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PDFHandling.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PDFHandling.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PathDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PathDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/PatternDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/PatternDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/QuartzTextDrawing.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/QuartzTextDrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Shadings.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Shadings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/ShadowsAndTransparencyLayers.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/ShadowsAndTransparencyLayers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/UIHandling.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/UIHandling.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/Utilities.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/Utilities.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/BasicDrawing/main.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/BasicDrawing/main.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CocoaDrawingShell/MyView.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CocoaDrawingShell/MyView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/ConfidentialStamper.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/ConfidentialStamper.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/confidential.pdf` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/confidential.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ConfidentialStamper/multipagedocumenttostamp.pdf` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ConfidentialStamper/multipagedocumenttostamp.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/CreatePDFDocument/CreatePDFDocument.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/CreatePDFDocument/CreatePDFDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/PSConverterTool/PSConverterTool.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/PSConverterTool/PSConverterTool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/Programming with Quartz/ParsePageContents/parse_page_contents.py` & `pyobjc-framework-Quartz-9.2/Examples/Programming with Quartz/ParsePageContents/parse_page_contents.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/AppController.py` & `pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/AppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/Chart.qtz` & `pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/Chart.qtz`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Quartz-9.2/Examples/QuartzComposer/Chart/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/AppDelegate.py` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/AppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/Circle.py` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/Circle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/classes.nib` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/English.lproj/TLayerDemo.nib/objects.nib` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/English.lproj/TLayerDemo.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/ShadowOffsetView.py` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/ShadowOffsetView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/TLayerDemo.py` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/TLayerDemo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Examples/TLayer/TLayerView.py` & `pyobjc-framework-Quartz-9.2/Examples/TLayer/TLayerView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/LICENSE.txt` & `pyobjc-framework-Quartz-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/_contextmanager.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/_contextmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreGraphics/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreGraphics/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:08 2023
+# Last update: Thu May 18 12:50:52 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -964,15 +964,20 @@
         "",
         {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
     "CGContextSetLineCap": (b"v^{CGContext=}i",),
     "CGImageMaskCreate": (
         b"^{CGImage=}QQQQQ^{CGDataProvider=}^dB",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                6: {"c_array_of_variable_length": True, "type_modifier": "n"}
+            },
+        },
     ),
     "CGContextDrawRadialGradient": (
         b"v^{CGContext=}^{CGGradient=}{CGPoint=dd}d{CGPoint=dd}dI",
     ),
     "CGFontCopyVariations": (
         b"^{__CFDictionary=}^{CGFont=}",
         "",
@@ -1188,14 +1193,15 @@
         {"retval": {"already_cfretained": True}},
     ),
     "CGContextStrokeLineSegments": (
         b"v^{CGContext=}^{CGPoint=dd}Q",
         "",
         {"arguments": {1: {"c_array_length_in_arg": 2, "type_modifier": "n"}}},
     ),
+    "CGContextSetTextMatrix": (b"v^{CGContext=}{CGAffineTransform=dddddd}",),
     "CGImageIsMask": (b"B^{CGImage=}",),
     "CGPDFObjectGetType": (b"i^{CGPDFObject=}",),
     "CGEventSourceGetUserData": (b"q^{__CGEventSource=}",),
     "CGContextSetStrokeColor": (
         b"v^{CGContext=}^d",
         "",
         {"arguments": {1: {"c_array_of_variable_length": True, "type_modifier": "n"}}},
@@ -1243,15 +1249,20 @@
             "arguments": {1: {"type_modifier": "n"}},
         },
     ),
     "CGPaletteGetIndexForColor": (b"I^{_CGDirectPaletteRef=}{CGDeviceColor=fff}",),
     "CGImageCreateWithJPEGDataProvider": (
         b"^{CGImage=}^{CGDataProvider=}^dBi",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                1: {"c_array_of_variable_length": True, "type_modifier": "n"}
+            },
+        },
     ),
     "CGPDFDocumentCreateWithURL": (
         b"^{CGPDFDocument=}^{__CFURL=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGPathAddArcToPoint": (
@@ -1305,19 +1316,15 @@
     "CGPDFScannerPopObject": (
         b"B^{CGPDFScanner=}^^{CGPDFObject=}",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "CGDisplayIsCaptured": (selAorI(b"iI", b"II"),),
     "CGPDFPageRelease": (b"v^{CGPDFPage=}",),
-    "CGDataProviderCreate": (
-        b"^{CGDataProvider=}^v^{CGDataProviderCallbacks=^?^?^?^?}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
+    "CGDisplayStreamStart": (b"i^{CGDisplayStream=}",),
     "CGRectIsEmpty": (b"B{CGRect={CGPoint=dd}{CGSize=dd}}",),
     "CGDisplayMoveCursorToPoint": (b"iI{CGPoint=dd}",),
     "CGPDFScannerPopInteger": (
         b"B^{CGPDFScanner=}^q",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
@@ -1358,22 +1365,14 @@
         b"v^{CGPath=}^{CGAffineTransform=dddddd}{CGRect={CGPoint=dd}{CGSize=dd}}dd",
         "",
         {"arguments": {1: {"type_modifier": "n"}}},
     ),
     "CGRectEqualToRect": (
         b"B{CGRect={CGPoint=dd}{CGSize=dd}}{CGRect={CGPoint=dd}{CGSize=dd}}",
     ),
-    "CGColorConversionInfoCreateFromListWithArguments": (
-        selAorI(
-            b"^{CGColorConversionInfo=}^{__CFDictionary=}^{CGColorSpace=}Ii^c",
-            b"^{CGColorConversionInfo=}^{__CFDictionary=}^{CGColorSpace=}Ii[1{__va_list_tag=II^v^v}]",
-        ),
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CGRectGetMaxY": (b"d{CGRect={CGPoint=dd}{CGSize=dd}}",),
     "CGBitmapContextGetWidth": (b"Q^{CGContext=}",),
     "CGShadingCreateRadial": (
         b"^{CGShading=}^{CGColorSpace=}{CGPoint=dd}d{CGPoint=dd}d^{CGFunction=}BB",
         "",
         {"retval": {"already_cfretained": True}},
     ),
@@ -1689,19 +1688,14 @@
     "CGImageGetBitsPerComponent": (b"Q^{CGImage=}",),
     "CGFontCopyTableTags": (
         b"^{__CFArray=}^{CGFont=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGWaitForScreenRefreshRects": (b"i^^{CGRect={CGPoint=dd}{CGSize=dd}}^I",),
-    "CGDataProviderCreateDirect": (
-        b"^{CGDataProvider=}^vq^{CGDataProviderDirectCallbacks=I^?^?^?^?}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CGDisplayStreamStop": (b"i^{CGDisplayStream=}",),
     "CGShadingRetain": (b"^{CGShading=}^{CGShading=}",),
     "CGBitmapContextGetColorSpace": (b"^{CGColorSpace=}^{CGContext=}",),
     "CGRequestPostEventAccess": (b"B",),
     "CGContextShowTextAtPoint": (
         b"v^{CGContext=}dd^tQ",
         "",
@@ -1801,19 +1795,14 @@
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "CGFunctionCreate": (
         b"^{CGFunction=}^vQ^dQ^d^{CGFunctionCallbacks=I^?^?}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CGDataProviderCreateDirectAccess": (
-        b"^{CGDataProvider=}^vQ^{CGDataProviderDirectAccessCallbacks=^?^?^?^?}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CGPaletteCreateFromPaletteBlendedWithColor": (
         b"^{_CGDirectPaletteRef=}^{_CGDirectPaletteRef=}f{CGDeviceColor=fff}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGContextGetTextMatrix": (b"{CGAffineTransform=dddddd}^{CGContext=}",),
     "CGDisplayModeGetIOFlags": (b"I^{CGDisplayMode=}",),
@@ -2144,15 +2133,20 @@
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGRectGetMidY": (b"d{CGRect={CGPoint=dd}{CGSize=dd}}",),
     "CGImageCreateWithPNGDataProvider": (
         b"^{CGImage=}^{CGDataProvider=}^dBi",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                1: {"c_array_of_variable_length": True, "type_modifier": "n"}
+            },
+        },
     ),
     "CGContextSetTextDrawingMode": (b"v^{CGContext=}i",),
     "CGContextGetUserSpaceToDeviceSpaceTransform": (
         b"{CGAffineTransform=dddddd}^{CGContext=}",
     ),
     "CGDataConsumerCreateWithCFData": (
         b"^{CGDataConsumer=}^{__CFData=}",
@@ -2319,19 +2313,14 @@
             },
         },
     ),
     "CGDisplayIsAsleep": (selAorI(b"iI", b"II"),),
     "CGPSConverterConvert": (
         b"B^{CGPSConverter=}^{CGDataProvider=}^{CGDataConsumer=}^{__CFDictionary=}",
     ),
-    "CGEventCreateSourceFromEvent": (
-        b"^{__CGEventSource=}^{__CGEvent=}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CGDisplayAddressForPosition": (
         b"^vIii",
         "",
         {"retval": {"c_array_of_variable_length": True}},
     ),
     "CGContextConvertPointToDeviceSpace": (b"{CGPoint=dd}^{CGContext=}{CGPoint=dd}",),
     "CGDisplayBounds": (b"{CGRect={CGPoint=dd}{CGSize=dd}}I",),
@@ -2561,22 +2550,25 @@
     "CGPathCreateCopyOfLineBySubtractingPath": (
         b"^{CGPath=}^{CGPath=}^{CGPath=}B",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGColorConverterRelease": (b"v^{CGColorConversionInfo=}",),
     "CGColorSpaceUsesITUR_2100TF": (b"B^{CGColorSpace=}",),
-    "CGDisplayStreamStart": (b"i^{CGDisplayStream=}",),
     "CGDisplayAvailableModes": (b"^{__CFArray=}I",),
     "CGColorCreateGenericGrayGamma2_2": (
         b"^{CGColor=}dd",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CGContextSetTextMatrix": (b"v^{CGContext=}{CGAffineTransform=dddddd}",),
+    "CGEventCreateSourceFromEvent": (
+        b"^{__CGEventSource=}^{__CGEvent=}",
+        "",
+        {"retval": {"already_cfretained": True}},
+    ),
     "CGPostKeyboardEvent": (selAorI(b"iSSi", b"iSSI"),),
     "CGPathCreateCopyBySymmetricDifferenceOfPath": (
         b"^{CGPath=}^{CGPath=}^{CGPath=}B",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CGPDFScannerPopStream": (
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreVideo/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreVideo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/CoreVideo/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/CoreVideo/_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:08 2023
+# Last update: Thu May 18 12:50:52 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -109,15 +109,18 @@
     "CVOpenGLTextureRelease": (b"v^{__CVBuffer=}",),
     "CVPixelBufferPoolRelease": (b"v^{__CVPixelBufferPool=}",),
     "CVPixelBufferPoolGetTypeID": (b"Q",),
     "CVYCbCrMatrixGetIntegerCodePointForString": (b"i^{__CFString=}",),
     "CVPixelBufferCreate": (
         b"i^{__CFAllocator=}QQI^{__CFDictionary=}^^{__CVBuffer=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {5: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "CVOpenGLBufferPoolGetTypeID": (b"Q",),
     "CVPixelBufferFillExtendedPixels": (b"i^{__CVBuffer=}",),
     "CVOpenGLTextureCacheRetain": (
         b"^{__CVOpenGLTextureCache=}^{__CVOpenGLTextureCache=}",
     ),
     "CVOpenGLBufferPoolCreateOpenGLBuffer": (
@@ -153,22 +156,26 @@
     "CVPixelBufferGetBaseAddress": (
         b"^v^{__CVBuffer=}",
         "",
         {"retval": {"c_array_of_variable_length": True}},
     ),
     "CVOpenGLBufferPoolRelease": (b"v^{__CVOpenGLBufferPool=}",),
     "CVPixelBufferLockBaseAddress": (b"i^{__CVBuffer=}Q",),
+    "CVMetalTextureCacheCreateFromImage": (
+        b"i@@@@QQQ^@",
+        "",
+        {"arguments": {7: {"already_cfretained": True, "type_modifier": "o"}}},
+    ),
     "CVOpenGLTextureCacheGetTypeID": (b"Q",),
-    "CVPixelBufferUnlockBaseAddress": (b"i^{__CVBuffer=}Q",),
     "CVMetalTextureCacheCreateTextureFromImage": (
         b"i^{__CFAllocator=}^{__CVMetalTextureCache=}^{__CVBuffer=}^{__CFDictionary=}QQQQ^^{__CVBuffer=}",
         "",
         {
             "retval": {"already_cfretained": True},
-            "arguments": {8: {"type_modifier": "o"}},
+            "arguments": {8: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "CVOpenGLTextureIsFlipped": (b"Z^{__CVBuffer=}",),
     "CVMetalTextureCacheFlush": (b"v^{__CVMetalTextureCache=}Q",),
     "CVPixelBufferPoolCreatePixelBuffer": (
         b"i^{__CFAllocator=}^{__CVPixelBufferPool=}^^{__CVBuffer=}",
         "",
@@ -360,15 +367,18 @@
             }
         },
     ),
     "CVPixelBufferGetIOSurface": (b"^{__IOSurface=}^{__CVBuffer=}",),
     "CVOpenGLTextureCacheCreateTextureFromImage": (
         b"i^{__CFAllocator=}^{__CVOpenGLTextureCache=}^{__CVBuffer=}^{__CFDictionary=}^^{__CVBuffer=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {4: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "CVDisplayLinkCreateWithCGDisplays": (
         b"i^Iq^^{__CVDisplayLink=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
@@ -382,15 +392,18 @@
     ),
     "CVOpenGLTextureGetTypeID": (b"Q",),
     "CVIsCompressedPixelFormatAvailable": (b"ZI",),
     "CVImageBufferIsFlipped": (b"Z^{__CVBuffer=}",),
     "CVBufferCopyAttachment": (
         b"@^{__CVBuffer=}^{__CFString=}^I",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "o"}},
+        },
     ),
     "CVMetalTextureGetTexture": (b"@^{__CVBuffer=}",),
     "CVPixelBufferIsPlanar": (b"Z^{__CVBuffer=}",),
     "CVBufferRemoveAllAttachments": (b"v^{__CVBuffer=}",),
     "CVTransferFunctionGetIntegerCodePointForString": (b"i^{__CFString=}",),
     "CVPixelBufferCreateWithBytes": (
         b"i^{__CFAllocator=}QQI^vQ^?^v^{__CFDictionary=}^^{__CVBuffer=}",
@@ -405,35 +418,15 @@
                     }
                 }
             },
         },
     ),
     "CVMetalTextureGetTypeID": (b"Q",),
     "CVOpenGLBufferPoolRetain": (b"^{__CVOpenGLBufferPool=}^{__CVOpenGLBufferPool=}",),
-    "CVPixelBufferCreateWithPlanarBytes": (
-        b"i^{__CFAllocator=}QQI^vQQ^^v^Q^Q^Q^?^v^{__CFDictionary=}^^{__CVBuffer=}",
-        "",
-        {
-            "retval": {"already_cfretained": True},
-            "arguments": {
-                11: {
-                    "callable": {
-                        "retval": {"type": b"v"},
-                        "arguments": {
-                            0: {"type": b"^v"},
-                            1: {"type": b"^v"},
-                            2: {"type": b"Q"},
-                            3: {"type": b"Q"},
-                            4: {"type": b"^^v"},
-                        },
-                    }
-                }
-            },
-        },
-    ),
+    "CVPixelBufferUnlockBaseAddress": (b"i^{__CVBuffer=}Q",),
     "CVImageBufferGetCleanRect": (b"{CGRect={CGPoint=dd}{CGSize=dd}}^{__CVBuffer=}",),
     "CVImageBufferCreateColorSpaceFromAttachments": (
         b"^{CGColorSpace=}^{__CFDictionary=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CVPixelBufferGetBytesPerRowOfPlane": (b"Q^{__CVBuffer=}Q",),
@@ -461,15 +454,18 @@
     ),
     "CVOpenGLBufferGetAttributes": (b"^{__CFDictionary=}^{__CVBuffer=}",),
     "CVDisplayLinkGetOutputVideoLatency": (b"{_CVTime=qii}^{__CVDisplayLink=}",),
     "CVPixelBufferGetBytesPerRow": (b"Q^{__CVBuffer=}",),
     "CVMetalTextureCacheCreate": (
         b"i^{__CFAllocator=}^{__CFDictionary=}@^{__CFDictionary=}^^{__CVMetalTextureCache=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {4: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "CVPixelBufferGetExtendedPixels": (
         b"v^{__CVBuffer=}^Q^Q^Q^Q",
         "",
         {
             "arguments": {
                 1: {"type_modifier": "o"},
@@ -491,15 +487,18 @@
     "CVGetHostClockFrequency": (b"d", "", {"variadic": False}),
     "CVGetHostClockMinimumTimeDelta": (b"I", "", {"variadic": False}),
     "CVOpenGLBufferRetain": (b"^{__CVBuffer=}^{__CVBuffer=}",),
     "CVMetalTextureIsFlipped": (b"Z^{__CVBuffer=}",),
     "CVOpenGLTextureCacheCreate": (
         b"i^{__CFAllocator=}^{__CFDictionary=}^{_CGLContextObject=}^{_CGLPixelFormatObject=}^{__CFDictionary=}^^{__CVOpenGLTextureCache=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {5: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "CVPixelBufferPoolFlush": (b"v^{__CVPixelBufferPool=}Q",),
     "CVOpenGLTextureGetCleanTexCoords": (b"v^{__CVBuffer=}[2f][2f][2f][2f]",),
 }
 aliases = {
     "CVDIRECT3DSURFACE": "LPDIRECT3DSURFACE9",
     "COREVIDEO_SUPPORTS_OPENGLES": "COREVIDEO_FALSE",
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/PyObjCOverrides.bridgesupport` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/PyObjCOverrides.bridgesupport`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageIO/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageIO/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:08 2023
+# Last update: Thu May 18 12:50:52 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageKit/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/ImageKit/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/ImageKit/_metadata.py`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:09 2023
+# Last update: Thu May 18 12:50:53 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/PDFKit/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/PDFKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/PDFKit/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/PDFKit/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Mar 24 18:23:28 2023
+# Last update: Thu May 18 12:50:53 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzComposer/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzComposer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzComposer/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzComposer/_metadata.py`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:09 2023
+# Last update: Thu May 18 12:50:53 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzCore/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzCore/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzCore/_metadata.py`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:09 2023
+# Last update: Thu May 18 12:50:53 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzFilters/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzFilters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuartzFilters/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuartzFilters/_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:09 2023
+# Last update: Thu May 18 12:50:54 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuickLookUI/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuickLookUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/QuickLookUI/_metadata.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/QuickLookUI/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:30:09 2023
+# Last update: Thu May 18 12:50:54 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/Quartz/__init__.py` & `pyobjc-framework-Quartz-9.2/Lib/Quartz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/PKG-INFO` & `pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Quartz
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the Quartz frameworks on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Quartz,Quartz.QuickLookUI,Quartz.CoreGraphics,Quartz.PDFKit,Quartz.CoreVideo,Quartz.ImageIO,Quartz.QuartzFilters,Quartz.QuartzCore,Quartz.QuartzComposer,Quartz.ImageKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Lib/pyobjc_framework_Quartz.egg-info/SOURCES.txt` & `pyobjc-framework-Quartz-9.2/Lib/pyobjc_framework_Quartz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/Core Graphics/CGRotation/CGImageUtils.py
 Examples/Core Graphics/CGRotation/CGImageView.py
 Examples/Core Graphics/CGRotation/Controller.py
 Examples/Core Graphics/CGRotation/demo.png
 Examples/Core Graphics/CGRotation/main.py
 Examples/Core Graphics/CGRotation/setup.py
```

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_CVPixelBuffer.m` & `pyobjc-framework-Quartz-9.2/Modules/_CVPixelBuffer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_CoreGraphics_inlines.m` & `pyobjc-framework-Quartz-9.2/Modules/_CoreGraphics_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_CoreImage.m` & `pyobjc-framework-Quartz-9.2/Modules/_CoreImage.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_CoreImage_protocols.m` & `pyobjc-framework-Quartz-9.2/Modules/_CoreImage_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_ImageKit_protocols.m` & `pyobjc-framework-Quartz-9.2/Modules/_ImageKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_PDFKit.m` & `pyobjc-framework-Quartz-9.2/Modules/_PDFKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_QuartzCore_protocols.m` & `pyobjc-framework-Quartz-9.2/Modules/_QuartzCore_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_QuickLookUI.m` & `pyobjc-framework-Quartz-9.2/Modules/_QuickLookUI.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_callbacks.m` & `pyobjc-framework-Quartz-9.2/Modules/_callbacks.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_coregraphics.m` & `pyobjc-framework-Quartz-9.2/Modules/_coregraphics.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_doubleindirect.m` & `pyobjc-framework-Quartz-9.2/Modules/_doubleindirect.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_imagekit.m` & `pyobjc-framework-Quartz-9.2/Modules/_imagekit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_quartzcore.m` & `pyobjc-framework-Quartz-9.2/Modules/_quartzcore.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/_sortandmap.m` & `pyobjc-framework-Quartz-9.2/Modules/_sortandmap.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Quartz-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Quartz-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PKG-INFO` & `pyobjc-framework-Quartz-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Quartz
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the Quartz frameworks on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Quartz,Quartz.QuickLookUI,Quartz.CoreGraphics,Quartz.PDFKit,Quartz.CoreVideo,Quartz.ImageIO,Quartz.QuartzFilters,Quartz.QuartzCore,Quartz.QuartzComposer,Quartz.ImageKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_IKFilterBrowserPanel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_IKFilterBrowserPanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_IKImageView.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_IKImageView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotation.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationButtonWidget.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationButtonWidget.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFAnnotationText.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFAnnotationText.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_PDFBorder.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_PDFBorder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caanimation.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caconstraintlayoutmanager.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caconstraintlayoutmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caemitterbehavior.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caemitterbehavior.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caemitterlayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caemitterlayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caframeraterange.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caframeraterange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cagradientlayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cagradientlayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_calayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_calayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_camediatiming.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_camediatiming.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_camediatimingfunction.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_camediatimingfunction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cametallayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cametallayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_caopengllayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_caopengllayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_carenderer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_carenderer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cashapelayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cashapelayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catextlayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_catextlayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catransaction.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_catransaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_catransform3d.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_catransform3d.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cavaluefunction.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cavaluefunction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgaffinetransform.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgaffinetransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgbitmapcontext.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgbitmapcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolor.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorconversion.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorconversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorconvertor.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorconvertor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcolorspace.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcolorspace.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgcontext.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgcontext.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,16 @@
                 data = fp.read()
 
             provider = Quartz.CGDataProviderCreateWithCFData(data)
             image = Quartz.CGImageCreateWithJPEGDataProvider(
                 provider, None, True, Quartz.kCGRenderingIntentDefault
             )
             self.assertIsInstance(image, Quartz.CGImageRef)
+            self.assertArgIsIn(Quartz.CGImageCreateWithJPEGDataProvider, 1)
+            self.assertArgIsVariableSize(Quartz.CGImageCreateWithJPEGDataProvider, 1)
 
             Quartz.CGContextDrawTiledImage(context, ((0, 0), (10, 10)), image)
 
             font = Quartz.CGFontCreateWithFontName("Helvetica")
             self.assertIsInstance(font, Quartz.CGFontRef)
             Quartz.CGContextSetFont(context, font)
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgconvertcolordatawithformat.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgconvertcolordatawithformat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdataconsumer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdataconsumer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdataprovider.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdataprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdirectdisplay.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdirectdisplay.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdirectpalette.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdirectpalette.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplayconfiguration.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplayconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplayfade.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplayfade.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgdisplaystream.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgdisplaystream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgerror.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgevent.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgeventsource.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgeventsource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgeventtypes.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgeventtypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgfont.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgfont.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgfunction.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgfunction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cggeometry.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cggeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cggradient.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cggradient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimage.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
         if not os.path.exists(fname):
             self.fail("test image doesn't exist")
 
         with open(fname, "rb") as fp:
             data = fp.read()
         provider = Quartz.CGDataProviderCreateWithCFData(data)
         self.assertResultIsCFRetained(Quartz.CGImageCreateWithPNGDataProvider)
+        self.assertArgIsIn(Quartz.CGImageCreateWithPNGDataProvider, 1)
+        self.assertArgIsVariableSize(Quartz.CGImageCreateWithPNGDataProvider, 1)
         self.assertArgHasType(Quartz.CGImageCreateWithPNGDataProvider, 2, objc._C_BOOL)
         v = Quartz.CGImageCreateWithPNGDataProvider(
             provider, None, True, Quartz.kCGRenderingIntentDefault
         )
         self.assertIsInstance(v, Quartz.CGImageRef)
 
         self.assertResultIsCFRetained(Quartz.CGImageCreateWithImageInRect)
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimageanimation.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimageanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagedestination.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagedestination.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagemetadata.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagemetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimageproperties.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimageproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgimagesource.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgimagesource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cglayer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cglayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpath.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpattern.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpattern.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfarray.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfcontentstream.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfcontentstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfcontext.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfdictionary.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfdictionary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfdocument.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfobject.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfoperatortable.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfoperatortable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfpage.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfpage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfscanner.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfscanner.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgpdfstream.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgpdfstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgremoteoperation.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgremoteoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgsession.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgshading.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgshading.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgwindow.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgwindow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cgwindowlevel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cgwindowlevel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cibarcodedescriptor.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cibarcodedescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cicontext.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cicontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cidetector.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cidetector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifeature.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifeature.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifilter.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifilter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifilterbuiltins.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifilterbuiltins.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cifiltergenerator.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cifiltergenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimage.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimageprocessor.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimageprocessor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ciimageprovider.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ciimageprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cikernel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cikernel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cirawfilter.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cirawfilter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cirenderdestination.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cirenderdestination.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cisampler.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cisampler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvbase.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvbase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvbuffer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvdisplaylink.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvdisplaylink.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvimagebuffer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvimagebuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvmetaltexture.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvmetaltexture.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvmetaltexturecache.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvmetaltexturecache.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,10 +7,12 @@
     def testConstants10_11(self):
         self.assertIsInstance(Quartz.kCVMetalTextureCacheMaximumTextureAgeKey, str)
 
     @min_os_level("10.11")
     def testFunctions10_11(self):
         self.assertIsInstance(Quartz.CVMetalTextureCacheGetTypeID(), int)
 
-        Quartz.CVMetalTextureCacheCreate
+        self.assertArgIsOut(Quartz.CVMetalTextureCacheCreate, 4)
+        self.assertArgIsCFRetained(Quartz.CVMetalTextureCacheCreate, 4)
         self.assertArgIsOut(Quartz.CVMetalTextureCacheCreateTextureFromImage, 8)
+        self.assertArgIsCFRetained(Quartz.CVMetalTextureCacheCreateTextureFromImage, 8)
         Quartz.CVMetalTextureCacheFlush
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopenglbuffer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopenglbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopenglbufferpool.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopenglbufferpool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopengltexture.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopengltexture.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvopengltexturecache.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvopengltexturecache.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbuffer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbuffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,17 @@
         self.assertEqual(len(v), 4)
         for i in range(4):
             self.assertIsInstance(v[i], int)
 
         rv = Quartz.CVPixelBufferFillExtendedPixels(buf)
         self.assertIsInstance(rv, int)
 
+        self.assertArgIsOut(Quartz.CVPixelBufferCreate, 5)
+        self.assertArgIsCFRetained(Quartz.CVPixelBufferCreate, 5)
+
     @expectedFailure
     def testManual(self):
         self.fail("CVPixelBufferCreate requires manual wrapper")
         self.fail("CVPixelBufferCreateWithBytes requires manual wrapper")
         self.fail("CVPixelBufferCreateWithPlanarBytes requires manual wrapper")
 
     def makeBuffer(self):
```

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbufferiosurface.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbufferiosurface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelbufferpool.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelbufferpool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvpixelformatdescription.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvpixelformatdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_cvreturn.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_cvreturn.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikcameradeviceview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikcameradeviceview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikdevicebrowserview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikdevicebrowserview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikfilterui.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikfilterui.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimagebrowsercell.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimagebrowsercell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimagebrowserview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimagebrowserview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikimageeditpanel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikimageeditpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikpicturetaker.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikpicturetaker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikscannerdeviceview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikscannerdeviceview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_ikslideshow.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_ikslideshow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_imagekitdeprecated.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_imagekitdeprecated.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfactionnamed.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfactionnamed.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfannotationutilities.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfannotationutilities.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfappearancecharacteristics.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfappearancecharacteristics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfdocument.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfkitplatform.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfkitplatform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfpage.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfpage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_pdfview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_pdfview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_plpreviewpanel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_plpreviewpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccomposition.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccomposition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionparameterview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionparameterview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qccompositionpickerview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qccompositionpickerview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcplugin.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcplugin.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcrenderer.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcrenderer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qcview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qcview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewingcontroller.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewingcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewpanel.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_qlpreviewview.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_qlpreviewview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_quartzfiltermanager.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_quartzfiltermanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/PyObjCTest/test_sqlpreviewreply.py` & `pyobjc-framework-Quartz-9.2/PyObjCTest/test_sqlpreviewreply.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/CoreGraphics.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/CoreGraphics.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -391,14 +391,15 @@
     "ignore": true,
     "retval": {
      "already_cfretained": true
     },
     "variadic": true
    },
    "CGColorConversionInfoCreateFromListWithArguments": {
+    "ignore": true,
     "retval": {
      "already_cfretained": true
     }
    },
    "CGColorConversionInfoCreateWithOptions": {
     "retval": {
      "already_cfretained": true
@@ -641,29 +642,33 @@
    },
    "CGDataProviderCopyData": {
     "retval": {
      "already_cfretained": true
     }
    },
    "CGDataProviderCreate": {
+    "ignore": true,
     "retval": {
      "already_cfretained": true
     }
    },
    "CGDataProviderCreateDirect": {
+    "ignore": true,
     "retval": {
      "already_cfretained": true
     }
    },
    "CGDataProviderCreateDirectAccess": {
+    "ignore": true,
     "retval": {
      "already_cfretained": true
     }
    },
    "CGDataProviderCreateSequential": {
+    "ignore": true,
     "retval": {
      "already_cfretained": true
     }
    },
    "CGDataProviderCreateWithCFData": {
     "retval": {
      "already_cfretained": true
@@ -938,21 +943,14 @@
    "CGDisplayStreamUpdateGetMovedRectsDelta": {
     "args": {
      "0": {},
      "1": {},
      "2": {}
     }
    },
-   "CGDisplayStreamUpdateGetRects": {
-    "args": {
-     "0": {},
-     "2": {}
-    },
-    "retval": {}
-   },
    "CGDisplaySwitchToMode": {
     "args": {
      "1": {}
     }
    },
    "CGEventCreate": {
     "args": {
@@ -1649,23 +1647,14 @@
     "args": {
      "0": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
-   "CGImageCreateWithJPEGDataProvider": {
-    "args": {
-     "0": {},
-     "1": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
    "CGImageCreateWithMask": {
     "args": {
      "0": {},
      "1": {}
     },
     "retval": {
      "already_cfretained": true
@@ -1679,15 +1668,15 @@
     "retval": {
      "already_cfretained": true
     }
    },
    "CGImageCreateWithPNGDataProvider": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "type_modifier": "n", "c_array_of_variable_length": true}
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CGImageGetAlphaInfo": {
     "args": {
@@ -1772,15 +1761,15 @@
     "args": {
      "0": {}
     }
    },
    "CGImageMaskCreate": {
     "args": {
      "5": {},
-     "6": {}
+     "6": { "type_modifier": "n", "c_array_of_variable_length": true }
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CGImageRelease": {
     "args": {
@@ -4328,41 +4317,14 @@
     "args": {
      "0": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
-   "CGDataProviderCreate": {
-    "args": {
-     "0": {},
-     "1": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
-   "CGDataProviderCreateDirect": {
-    "args": {
-     "0": {},
-     "2": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
-   "CGDataProviderCreateDirectAccess": {
-    "args": {
-     "0": {},
-     "2": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
    "CGDataProviderCreateSequential": {
     "args": {
      "0": {},
      "1": {}
     },
     "retval": {
      "already_cfretained": true
@@ -5443,15 +5405,15 @@
     "retval": {
      "already_cfretained": true
     }
    },
    "CGImageCreateWithJPEGDataProvider": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "c_array_of_variable_length": true, "type_modifier": "n" }
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CGImageCreateWithMask": {
     "args": {
@@ -5467,23 +5429,14 @@
      "0": {},
      "1": { "c_array_of_variable_length": true, "type_modifier": "n" }
     },
     "retval": {
      "already_cfretained": true
     }
    },
-   "CGImageCreateWithPNGDataProvider": {
-    "args": {
-     "0": {},
-     "1": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
    "CGImageGetAlphaInfo": {
     "args": {
      "0": {}
     }
    },
    "CGImageGetBitmapInfo": {
     "args": {
@@ -5544,23 +5497,14 @@
     }
    },
    "CGImageIsMask": {
     "args": {
      "0": {}
     }
    },
-   "CGImageMaskCreate": {
-    "args": {
-     "5": {},
-     "6": {}
-    },
-    "retval": {
-     "already_cfretained": true
-    }
-   },
    "CGImageRelease": {
     "args": {
      "0": {}
     }
    },
    "CGImageRetain": {
     "args": {
```

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/CoreVideo.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/CoreVideo.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,34 @@
     "gettypeid_func": "CVPixelBufferGetTypeID",
     "typestr": "^{__CVPixelBuffer=}"
    }
   },
   "classes": {},
   "formal_protocols": {},
   "functions": {
+   "CVMetalTextureCacheCreateFromImage": {
+    "args": {
+     "0": { "type_override": "@" },
+     "1": { "type_override": "@" },
+     "2": { "type_override": "@" },
+     "3": { "type_override": "@" },
+     "4": { "type_override": "Q" },
+     "5": { "type_override": "Q" },
+     "6": { "type_override": "Q" },
+     "7": { "type_override": "^@", "already_cfretained": true, "type_modifier": "o" }
+    },
+    "retval": {
+     "type_override": "i"
+    }
+   },
+   "CVBufferCopyAttachment": {
+    "args": {
+     "2": { "type_modifier": "o" }
+    }
+   },
    "CVYCbCrMatrixGetIntegerCodePointForString": {
     "args": {
      "0": { "typestr": "^{__CFString=}" }
     },
     "retval": { "typestr": "i" }
    },
    "CVColorPrimariesGetIntegerCodePointForString": {
@@ -150,33 +170,29 @@
      "1": { "typestr": "L" }
     },
     "retval": { "typestr": "v" }
    },
    "CVMetalTextureCacheCreate": {
     "retval": { "typestr": "i" },
     "args": {
-     "0": { "typestr": "@" },
-     "1": { "typestr": "@" },
-     "2": { "typestr": "@" },
-     "3": { "typestr": "@" },
-     "4": { "typestr": "^{__CVBuffer=}" }
+     "4": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVMetalTextureCacheCreateTextureFromImage": {
     "retval": { "typestr": "i" },
     "args": {
      "0": { "typestr": "@" },
      "1": { "typestr": "@" },
      "2": { "typestr": "^{__CVBuffer=}" },
      "3": { "typestr": "@" },
      "4": { "typestr": "Q" },
      "5": { "typestr": "L" },
      "6": { "typestr": "L" },
      "7": { "typestr": "L" },
-     "8": { "typestr": "^^{__CVBuffer=}", "type_modifier": "o" }
+     "8": { "typestr": "^^{__CVBuffer=}", "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVDisplayLinkSetOutputHandler": {
     "retval": { "typestr": "i" },
     "args": {
      "0": { "typestr": "^{__CVDisplayLink=}" },
      "1": { "typestr": "@?" ,
@@ -530,24 +546,24 @@
    "CVOpenGLTextureCacheCreate": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "3": {},
      "4": {},
-     "5": {}
+     "5": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVOpenGLTextureCacheCreateTextureFromImage": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "3": {},
-     "4": {}
+     "4": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVOpenGLTextureCacheFlush": {
     "args": {
      "0": {}
     }
    },
@@ -593,15 +609,15 @@
     },
     "retval": {}
    },
    "CVPixelBufferCreate": {
     "args": {
      "0": {},
      "4": {},
-     "5": {}
+     "5": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVPixelBufferCreateResolvedAttributesDictionary": {
     "args": {
      "0": {},
      "1": {},
      "2": { "type_modifier": "o", "already_cfretained": true  }
@@ -654,14 +670,15 @@
      "0": {},
      "1": {},
      "2": {},
      "3": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVPixelBufferCreateWithPlanarBytes": {
+    "ignore": true,
     "args": {
      "0": {},
      "4": {},
      "7": {},
      "8": {},
      "9": {},
      "10": {},
@@ -705,15 +722,15 @@
          false
         ]
        }
       }
      },
      "12": {},
      "13": {},
-     "14": {}
+     "14": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CVPixelBufferFillExtendedPixels": {
     "args": {
      "0": {}
     }
    },
```

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/ImageIO.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/ImageIO.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/ImageKit.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/ImageKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/PDFKit.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/PDFKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/QuartzComposer.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/QuartzComposer.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/QuartzCore.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/QuartzCore.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/QuickLookUI.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/QuickLookUI.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/metadata.ini` & `pyobjc-framework-Quartz-9.2/metadata/metadata.ini`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-12.1.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-12.1.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreGraphics/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreGraphics/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreImage/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreImage/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-12.1.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-12.1.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.CoreVideo/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.CoreVideo/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.14.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageIO/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageIO/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.ImageKit/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.ImageKit/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.PDFKit/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.PDFKit/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.14.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzComposer/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzComposer/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-13.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzCore/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzCore/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuartzFilters/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuartzFilters/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/arm64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.10.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.15.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.16.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.6.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.7.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-10.8.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-12.0.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-12.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/metadata/raw.QuickLookUI/x86_64-13.3.fwinfo` & `pyobjc-framework-Quartz-9.2/metadata/raw.QuickLookUI/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Quartz-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Quartz-9.1b1/setup.py` & `pyobjc-framework-Quartz-9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,28 @@
 ---
 
 * Add wrapper for ``CGBitmapContextCreateWithData``
 
 """
 
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
 
 subpackages = [
     f"Quartz.{fn}"
     for fn in os.listdir("Lib/Quartz")
     if os.path.exists(os.path.join("Lib/Quartz", fn, "__init__.py"))
 ]
 
-VERSION = "9.1b1"
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-Quartz",
     description="Wrappers for the Quartz frameworks on macOS",
     packages=["Quartz"] + subpackages,
     ext_modules=[
         # CoreVideo
```

