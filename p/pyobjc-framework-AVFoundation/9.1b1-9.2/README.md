# Comparing `tmp/pyobjc-framework-AVFoundation-9.1b1.tar.gz` & `tmp/pyobjc-framework-AVFoundation-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AVFoundation-9.1b1.tar", last modified: Sun Mar 26 11:12:04 2023, max compression
+gzip compressed data, was "pyobjc-framework-AVFoundation-9.2.tar", last modified: Wed Jun  7 00:04:16 2023, max compression
```

## Comparing `pyobjc-framework-AVFoundation-9.1b1.tar` & `pyobjc-framework-AVFoundation-9.2.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:04.529595 pyobjc-framework-AVFoundation-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:03.799621 pyobjc-framework-AVFoundation-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:03.833278 pyobjc-framework-AVFoundation-9.1b1/Lib/AVFoundation/
--rw-r--r--   0 ronald     (501) staff       (20)      904 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/AVFoundation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   343699 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/AVFoundation/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:03.876294 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-03-26 11:12:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     5639 2023-03-26 11:12:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:12:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      148 2023-03-26 11:12:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:12:03.000000 pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AVFoundation-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:03.919423 pyobjc-framework-AVFoundation-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      934 2021-10-18 19:38:40.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation.m
--rw-r--r--   0 ronald     (501) staff       (20)     6516 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_AVAudioBuffer.m
--rw-r--r--   0 ronald     (501) staff       (20)     1676 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     2937 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-AVFoundation-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1908 2023-03-26 11:12:04.528503 pyobjc-framework-AVFoundation-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:04.386498 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1139 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_AVCaptionConversionValidator.py
--rw-r--r--   0 ronald     (501) staff       (20)     1065 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_AVSemanticSegmentationMatte.py
--rw-r--r--   0 ronald     (501) staff       (20)      594 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)     6035 2022-06-25 20:16:52.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avasset.py
--rw-r--r--   0 ronald     (501) staff       (20)      335 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetcache.py
--rw-r--r--   0 ronald     (501) staff       (20)     3022 2022-06-25 20:16:58.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetdownloadtask.py
--rw-r--r--   0 ronald     (501) staff       (20)     5731 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetexportsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     2163 2022-10-29 11:02:15.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetimagegenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)      670 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetplaybackassistant.py
--rw-r--r--   0 ronald     (501) staff       (20)     1483 2022-10-29 11:55:05.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetreader.py
--rw-r--r--   0 ronald     (501) staff       (20)      796 2022-06-25 20:07:53.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetreaderoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     3643 2022-10-29 09:43:09.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetresourceloader.py
--rw-r--r--   0 ronald     (501) staff       (20)      379 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetsegmentreport.py
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetstoragemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     2805 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassettrack.py
--rw-r--r--   0 ronald     (501) staff       (20)      172 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassettrackgroup.py
--rw-r--r--   0 ronald     (501) staff       (20)      249 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassettracksegment.py
--rw-r--r--   0 ronald     (501) staff       (20)     2712 2022-06-25 08:57:26.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetwriter.py
--rw-r--r--   0 ronald     (501) staff       (20)     2756 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetwriterinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1509 2022-06-25 08:56:46.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avasynchronouskeyvalueloading.py
--rw-r--r--   0 ronald     (501) staff       (20)      962 2021-07-31 09:08:03.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiobuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      258 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiochannellayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     2362 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioconverter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4140 2022-10-29 11:35:11.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioengine.py
--rw-r--r--   0 ronald     (501) staff       (20)     1278 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioenvironmentnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1554 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiofile.py
--rw-r--r--   0 ronald     (501) staff       (20)     1729 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioformat.py
--rw-r--r--   0 ronald     (501) staff       (20)     1522 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioionode.py
--rw-r--r--   0 ronald     (501) staff       (20)      953 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiomix.py
--rw-r--r--   0 ronald     (501) staff       (20)     4264 2022-06-25 08:56:13.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiomixing.py
--rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudionode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1666 2022-06-25 20:10:31.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     3010 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioplayernode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1045 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioprocessingsettings.py
--rw-r--r--   0 ronald     (501) staff       (20)     1441 2022-06-25 20:11:17.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiorecorder.py
--rw-r--r--   0 ronald     (501) staff       (20)      780 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioroutingarbiter.py
--rw-r--r--   0 ronald     (501) staff       (20)     6490 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosequencer.py
--rw-r--r--   0 ronald     (501) staff       (20)     4269 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosession.py
--rw-r--r--   0 ronald     (501) staff       (20)     4379 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosessiontypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     2385 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosetting.py
--rw-r--r--   0 ronald     (501) staff       (20)     2810 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosink.py
--rw-r--r--   0 ronald     (501) staff       (20)      482 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosourcenode.py
--rw-r--r--   0 ronald     (501) staff       (20)      550 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiotime.py
--rw-r--r--   0 ronald     (501) staff       (20)     2024 2022-01-02 11:04:26.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiotypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      602 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounit.py
--rw-r--r--   0 ronald     (501) staff       (20)     2125 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitcomponent.py
--rw-r--r--   0 ronald     (501) staff       (20)      325 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiouniteffect.py
--rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiouniteq.py
--rw-r--r--   0 ronald     (501) staff       (20)      331 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitgenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)     1264 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitreverb.py
--rw-r--r--   0 ronald     (501) staff       (20)      967 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitsampler.py
--rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounittimeeffect.py
--rw-r--r--   0 ronald     (501) staff       (20)      337 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounittimeffect.py
--rw-r--r--   0 ronald     (501) staff       (20)      521 2022-10-29 10:59:48.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcameracalibrationdata.py
--rw-r--r--   0 ronald     (501) staff       (20)     5298 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaption.py
--rw-r--r--   0 ronald     (501) staff       (20)      558 2021-07-31 08:55:29.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptionformatconformer.py
--rw-r--r--   0 ronald     (501) staff       (20)      377 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptionrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      593 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptionsettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      340 2022-06-25 20:08:13.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptureaudiodataoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)      832 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturedeskviewapplication.py
--rw-r--r--   0 ronald     (501) staff       (20)    15137 2023-03-24 18:54:07.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturedevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1859 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturefileoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     2544 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptureinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     2689 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptureoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1262 2022-10-29 11:56:38.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturephotooutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     6621 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturesession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturesessionpreset.py
--rw-r--r--   0 ronald     (501) staff       (20)      890 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturestillimageoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)      895 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturevideodataoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturevideopreviewlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2553 2022-10-29 11:25:38.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcomposition.py
--rw-r--r--   0 ronald     (501) staff       (20)     1393 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcompositiontrack.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcompositiontracksegment.py
--rw-r--r--   0 ronald     (501) staff       (20)     5414 2022-10-29 09:45:06.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcontentkeysession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avdepthdata.py
--rw-r--r--   0 ronald     (501) staff       (20)     7206 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_averror.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avfoundation.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avgeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)     5294 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmediaformat.py
--rw-r--r--   0 ronald     (501) staff       (20)      342 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmediaselection.py
--rw-r--r--   0 ronald     (501) staff       (20)      462 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmediaselectiongroup.py
--rw-r--r--   0 ronald     (501) staff       (20)    27493 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataformat.py
--rw-r--r--   0 ronald     (501) staff       (20)    35642 2022-10-29 09:44:48.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataidentifiers.py
--rw-r--r--   0 ronald     (501) staff       (20)      690 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2960 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataobject.py
--rw-r--r--   0 ronald     (501) staff       (20)      631 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmidiplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     4814 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmovie.py
--rw-r--r--   0 ronald     (501) staff       (20)     2640 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmovietrack.py
--rw-r--r--   0 ronald     (501) staff       (20)     4577 2022-10-29 11:38:33.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmusicevents.py
--rw-r--r--   0 ronald     (501) staff       (20)     1131 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avoutputsettingsassistant.py
--rw-r--r--   0 ronald     (501) staff       (20)     1175 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avoutputsettingsassistent.py
--rw-r--r--   0 ronald     (501) staff       (20)     3788 2022-06-25 20:14:35.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplaybackcoordinator.py
--rw-r--r--   0 ronald     (501) staff       (20)     7262 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     3676 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayerinterstitialeventcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     5241 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      284 2022-06-25 20:16:40.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemmediadatacollector.py
--rw-r--r--   0 ronald     (501) staff       (20)     2108 2022-06-25 20:12:25.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1324 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemprotectedcontentaddition.py
--rw-r--r--   0 ronald     (501) staff       (20)     1394 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemprotectedcontentadditions.py
--rw-r--r--   0 ronald     (501) staff       (20)      505 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemtrack.py
--rw-r--r--   0 ronald     (501) staff       (20)      423 2022-06-26 10:16:33.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayerlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      508 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayerlooper.py
--rw-r--r--   0 ronald     (501) staff       (20)      699 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avportraitmatte.py
--rw-r--r--   0 ronald     (501) staff       (20)     1526 2022-06-25 20:13:25.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avqueuedsamplebufferrendering.py
--rw-r--r--   0 ronald     (501) staff       (20)      755 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avroutedetector.py
--rw-r--r--   0 ronald     (501) staff       (20)     1179 2021-08-14 10:34:11.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferaudiorenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2545 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferdisplaylayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1303 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebuffergenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)     1184 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferrendersynchronizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2490 2022-01-02 11:04:26.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplecursor.py
--rw-r--r--   0 ronald     (501) staff       (20)     4319 2022-06-26 10:16:33.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avspeechsynthesis.py
--rw-r--r--   0 ronald     (501) staff       (20)      629 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avspeechsynthesisprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      255 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avutilities.py
--rw-r--r--   0 ronald     (501) staff       (20)     2213 2022-06-25 20:16:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideocompositing.py
--rw-r--r--   0 ronald     (501) staff       (20)     6923 2022-10-29 09:41:40.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideocomposition.py
--rw-r--r--   0 ronald     (501) staff       (20)     7080 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideosettings.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:04.390088 pyobjc-framework-AVFoundation-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    84490 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/AVFoundation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      131 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:12:04.520238 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)  1031608 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1046756 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1093045 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1095610 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   605514 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   912509 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   950766 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1070282 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1109522 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1031609 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1046757 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1093046 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1095611 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AVFoundation-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:12:04.529722 pyobjc-framework-AVFoundation-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1544 2023-03-25 14:20:30.000000 pyobjc-framework-AVFoundation-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.273894 pyobjc-framework-AVFoundation-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.010029 pyobjc-framework-AVFoundation-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.015624 pyobjc-framework-AVFoundation-9.2/Lib/AVFoundation/
+-rw-r--r--   0 ronald     (501) staff       (20)      904 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.2/Lib/AVFoundation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   343699 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/Lib/AVFoundation/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.019777 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-06-07 00:04:16.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     5654 2023-06-07 00:04:16.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:04:15.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:03.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      138 2023-06-07 00:04:15.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:04:15.000000 pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AVFoundation-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.023372 pyobjc-framework-AVFoundation-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      934 2021-10-18 19:38:40.000000 pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6516 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_AVAudioBuffer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1676 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2937 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-AVFoundation-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-06-07 00:04:16.273471 pyobjc-framework-AVFoundation-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.171781 pyobjc-framework-AVFoundation-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1139 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_AVCaptionConversionValidator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1065 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_AVSemanticSegmentationMatte.py
+-rw-r--r--   0 ronald     (501) staff       (20)      594 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6035 2022-06-25 20:16:52.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avasset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      335 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetcache.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3022 2022-06-25 20:16:58.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetdownloadtask.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5731 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetexportsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2163 2022-10-29 11:02:15.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetimagegenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      670 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetplaybackassistant.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1483 2022-10-29 11:55:05.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetreader.py
+-rw-r--r--   0 ronald     (501) staff       (20)      796 2022-06-25 20:07:53.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetreaderoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3643 2022-10-29 09:43:09.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetresourceloader.py
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetsegmentreport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetstoragemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2805 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassettrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)      172 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassettrackgroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      249 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassettracksegment.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2712 2022-06-25 08:57:26.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetwriter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2756 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetwriterinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1509 2022-06-25 08:56:46.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avasynchronouskeyvalueloading.py
+-rw-r--r--   0 ronald     (501) staff       (20)      962 2021-07-31 09:08:03.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiobuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      258 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiochannellayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2362 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioconverter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4140 2022-10-29 11:35:11.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioengine.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1278 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioenvironmentnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1554 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1729 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1522 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioionode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      953 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiomix.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4264 2022-06-25 08:56:13.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiomixing.py
+-rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudionode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1666 2022-06-25 20:10:31.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3010 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioplayernode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1045 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioprocessingsettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1441 2022-06-25 20:11:17.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiorecorder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      780 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioroutingarbiter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6490 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosequencer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4269 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4379 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosessiontypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2385 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosetting.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2810 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosink.py
+-rw-r--r--   0 ronald     (501) staff       (20)      482 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosourcenode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      550 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiotime.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2024 2022-01-02 11:04:26.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiotypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2125 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitcomponent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      325 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiouniteffect.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiouniteq.py
+-rw-r--r--   0 ronald     (501) staff       (20)      331 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitgenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1264 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitreverb.py
+-rw-r--r--   0 ronald     (501) staff       (20)      967 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitsampler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounittimeeffect.py
+-rw-r--r--   0 ronald     (501) staff       (20)      337 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounittimeffect.py
+-rw-r--r--   0 ronald     (501) staff       (20)      521 2022-10-29 10:59:48.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcameracalibrationdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5298 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaption.py
+-rw-r--r--   0 ronald     (501) staff       (20)      558 2021-07-31 08:55:29.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptionformatconformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      377 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptionrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      593 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptionsettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      340 2022-06-25 20:08:13.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptureaudiodataoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      832 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturedeskviewapplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)    15137 2023-03-24 18:54:07.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturedevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1859 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturefileoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2544 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptureinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2689 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptureoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1262 2022-10-29 11:56:38.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturephotooutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6621 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturesession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturesessionpreset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      890 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturestillimageoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      895 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturevideodataoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturevideopreviewlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2553 2022-10-29 11:25:38.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcomposition.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1393 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcompositiontrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcompositiontracksegment.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5414 2022-10-29 09:45:06.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcontentkeysession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avdepthdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7206 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_averror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avfoundation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avgeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5294 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmediaformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)      342 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmediaselection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      462 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmediaselectiongroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27627 2023-05-04 11:00:07.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)    35642 2022-10-29 09:44:48.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataidentifiers.py
+-rw-r--r--   0 ronald     (501) staff       (20)      690 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2960 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      631 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmidiplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4814 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmovie.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2640 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmovietrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4577 2022-10-29 11:38:33.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmusicevents.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1131 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avoutputsettingsassistant.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1175 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avoutputsettingsassistent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3788 2022-06-25 20:14:35.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplaybackcoordinator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7262 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3676 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayerinterstitialeventcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5241 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      284 2022-06-25 20:16:40.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemmediadatacollector.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2108 2022-06-25 20:12:25.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1324 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemprotectedcontentaddition.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1394 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemprotectedcontentadditions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      505 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemtrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)      423 2022-06-26 10:16:33.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayerlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      508 2022-02-24 08:47:16.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayerlooper.py
+-rw-r--r--   0 ronald     (501) staff       (20)      699 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avportraitmatte.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1526 2022-06-25 20:13:25.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avqueuedsamplebufferrendering.py
+-rw-r--r--   0 ronald     (501) staff       (20)      755 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avroutedetector.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1179 2021-08-14 10:34:11.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferaudiorenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2545 2021-07-30 09:00:36.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferdisplaylayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1303 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebuffergenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1184 2021-03-21 10:08:22.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferrendersynchronizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2490 2022-01-02 11:04:26.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplecursor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4319 2022-06-26 10:16:33.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avspeechsynthesis.py
+-rw-r--r--   0 ronald     (501) staff       (20)      629 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avspeechsynthesisprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      255 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avutilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2213 2022-06-25 20:16:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideocompositing.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6923 2022-10-29 09:41:40.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideocomposition.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7080 2022-06-23 11:03:27.000000 pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideosettings.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.178115 pyobjc-framework-AVFoundation-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    84490 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/metadata/AVFoundation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      131 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:04:16.269786 pyobjc-framework-AVFoundation-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)  1031608 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1046756 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1093045 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1095610 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   605514 2020-11-30 18:45:14.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   912509 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   950766 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1070282 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1109522 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1031609 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1046757 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1093046 2022-10-18 09:53:23.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1095611 2023-02-19 10:50:34.000000 pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AVFoundation-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AVFoundation-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:04:16.274006 pyobjc-framework-AVFoundation-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1616 2023-05-29 10:07:45.000000 pyobjc-framework-AVFoundation-9.2/setup.py
```

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Lib/AVFoundation/__init__.py` & `pyobjc-framework-AVFoundation-9.2/Lib/AVFoundation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Lib/AVFoundation/_metadata.py` & `pyobjc-framework-AVFoundation-9.2/Lib/AVFoundation/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/PKG-INFO` & `pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AVFoundation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AVFoundation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AVFoundation
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Lib/pyobjc_framework_AVFoundation.egg-info/SOURCES.txt` & `pyobjc-framework-AVFoundation-9.2/Lib/pyobjc_framework_AVFoundation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AVFoundation/__init__.py
 Lib/AVFoundation/_metadata.py
 Lib/pyobjc_framework_AVFoundation.egg-info/PKG-INFO
 Lib/pyobjc_framework_AVFoundation.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AVFoundation.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AVFoundation.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AVFoundation-9.1b1/License.txt` & `pyobjc-framework-AVFoundation-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation.m` & `pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_AVAudioBuffer.m` & `pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_AVAudioBuffer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_inlines.m` & `pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/_AVFoundation_protocols.m` & `pyobjc-framework-AVFoundation-9.2/Modules/_AVFoundation_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-AVFoundation-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-AVFoundation-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PKG-INFO` & `pyobjc-framework-AVFoundation-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AVFoundation
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AVFoundation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AVFoundation
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_AVCaptionConversionValidator.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_AVCaptionConversionValidator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_AVSemanticSegmentationMatte.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_AVSemanticSegmentationMatte.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avanimation.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avasset.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avasset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetdownloadtask.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetdownloadtask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetexportsession.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetexportsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetimagegenerator.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetimagegenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetplaybackassistant.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetplaybackassistant.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetreader.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetreader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetreaderoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetreaderoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetresourceloader.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetresourceloader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassettrack.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassettrack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetwriter.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetwriter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avassetwriterinput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avassetwriterinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avasynchronouskeyvalueloading.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avasynchronouskeyvalueloading.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiobuffer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiobuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioconverter.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioconverter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioengine.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioengine.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioenvironmentnode.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioenvironmentnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiofile.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioformat.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioformat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioionode.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioionode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiomix.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiomix.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiomixing.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiomixing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioplayer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioplayernode.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioplayernode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioprocessingsettings.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioprocessingsettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiorecorder.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiorecorder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudioroutingarbiter.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudioroutingarbiter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosequencer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosequencer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosession.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosessiontypes.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosessiontypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosetting.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosetting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiosettings.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiosettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiotime.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiotime.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiotypes.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiotypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounit.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitcomponent.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitcomponent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiouniteq.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiouniteq.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitreverb.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitreverb.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avaudiounitsampler.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avaudiounitsampler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcameracalibrationdata.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcameracalibrationdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaption.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaption.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptionformatconformer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptionformatconformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptionsettings.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptionsettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturedeskviewapplication.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturedeskviewapplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturedevice.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturedevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturefileoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturefileoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptureinput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptureinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcaptureoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcaptureoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturephotooutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturephotooutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturesession.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturesession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturesessionpreset.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturesessionpreset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturestillimageoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturestillimageoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcapturevideodataoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcapturevideodataoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcomposition.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcomposition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcompositiontrack.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcompositiontrack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avcontentkeysession.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avcontentkeysession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avdepthdata.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avdepthdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_averror.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_averror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmediaformat.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmediaformat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataformat.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,16 +450,18 @@
     def testConstants10_11(self):
         self.assertIsInstance(
             AVFoundation.AVMetadataQuickTimeMetadataKeyContentIdentifier, str
         )
         self.assertIsInstance(AVFoundation.AVMetadataID3MetadataKeyCommercial, str)
         self.assertIsInstance(AVFoundation.AVMetadataExtraAttributeInfoKey, str)
 
-    @min_os_level("10.11.3")
+    @min_os_level("10.12")
     def testConstants10_11_3(self):
+        # The documentation says this value is availaable on 10.11.3, but testing
+        # shows the value isn't available in 10.11.6.
         self.assertIsInstance(AVFoundation.AVMetadataKeySpaceHLSDateRange, str)
 
     @min_os_level("10.12")
     def testConstants10_12(self):
         self.assertIsInstance(AVFoundation.AVMetadataISOUserDataKeyDate, str)
 
     @min_os_level("10.13")
```

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataidentifiers.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataidentifiers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataitem.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmetadataobject.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmetadataobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmidiplayer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmidiplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmovie.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmovie.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmovietrack.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmovietrack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avmusicevents.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avmusicevents.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avoutputsettingsassistant.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avoutputsettingsassistant.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avoutputsettingsassistent.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avoutputsettingsassistent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplaybackcoordinator.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplaybackcoordinator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayerinterstitialeventcontroller.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayerinterstitialeventcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritem.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemoutput.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemoutput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemprotectedcontentaddition.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemprotectedcontentaddition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avplayeritemprotectedcontentadditions.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avplayeritemprotectedcontentadditions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avportraitmatte.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avportraitmatte.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avqueuedsamplebufferrendering.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avqueuedsamplebufferrendering.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avroutedetector.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avroutedetector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferaudiorenderer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferaudiorenderer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferdisplaylayer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferdisplaylayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebuffergenerator.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebuffergenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplebufferrendersynchronizer.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplebufferrendersynchronizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avsamplecursor.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avsamplecursor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avspeechsynthesis.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avspeechsynthesis.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avspeechsynthesisprovider.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avspeechsynthesisprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideocompositing.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideocompositing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideocomposition.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideocomposition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/PyObjCTest/test_avvideosettings.py` & `pyobjc-framework-AVFoundation-9.2/PyObjCTest/test_avvideosettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/AVFoundation.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/AVFoundation.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-AVFoundation-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AVFoundation-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AVFoundation-9.1b1/setup.py` & `pyobjc-framework-AVFoundation-9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 import os
 
-from pyobjc_setup import Extension, setup
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-AVFoundation",
     description="Wrappers for the framework AVFoundation on macOS",
     min_os_level="10.7",
     packages=["AVFoundation"],
     ext_modules=[
```

