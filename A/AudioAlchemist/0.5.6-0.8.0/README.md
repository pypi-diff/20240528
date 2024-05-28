# Comparing `tmp/audioalchemist-0.5.6.tar.gz` & `tmp/audioalchemist-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioalchemist-0.5.6.tar", last modified: Thu May 23 02:12:39 2024, max compression
+gzip compressed data, was "audioalchemist-0.8.0.tar", last modified: Tue May 28 00:29:52 2024, max compression
```

## Comparing `audioalchemist-0.5.6.tar` & `audioalchemist-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 02:12:39.184837 audioalchemist-0.5.6/
-drwxrwxrwx   0        0        0        0 2024-05-23 02:12:39.152869 audioalchemist-0.5.6/AudioAlchemist/
--rw-rw-rw-   0        0        0       45 2024-05-23 00:11:59.000000 audioalchemist-0.5.6/AudioAlchemist/__init__.py
--rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.5.6/AudioAlchemist/audio_alchemist.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:12:39.179419 audioalchemist-0.5.6/AudioAlchemist.egg-info/
--rw-rw-rw-   0        0        0     3116 2024-05-23 02:12:38.000000 audioalchemist-0.5.6/AudioAlchemist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-23 02:12:39.000000 audioalchemist-0.5.6/AudioAlchemist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 02:12:38.000000 audioalchemist-0.5.6/AudioAlchemist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 02:12:38.000000 audioalchemist-0.5.6/AudioAlchemist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 02:12:38.000000 audioalchemist-0.5.6/AudioAlchemist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3116 2024-05-23 02:12:39.179419 audioalchemist-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-23 02:12:39.184837 audioalchemist-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1434 2024-05-23 02:11:22.000000 audioalchemist-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:29:52.788771 audioalchemist-0.8.0/
+drwxrwxrwx   0        0        0        0 2024-05-28 00:29:52.779762 audioalchemist-0.8.0/AudioAlchemist/
+-rw-rw-rw-   0        0        0       45 2024-05-23 00:11:59.000000 audioalchemist-0.8.0/AudioAlchemist/__init__.py
+-rw-rw-rw-   0        0        0     2201 2024-05-28 00:28:03.000000 audioalchemist-0.8.0/AudioAlchemist/audio_alchemist.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:29:52.786764 audioalchemist-0.8.0/AudioAlchemist.egg-info/
+-rw-rw-rw-   0        0        0     5623 2024-05-28 00:29:52.000000 audioalchemist-0.8.0/AudioAlchemist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-28 00:29:52.000000 audioalchemist-0.8.0/AudioAlchemist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:29:52.000000 audioalchemist-0.8.0/AudioAlchemist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 00:29:52.000000 audioalchemist-0.8.0/AudioAlchemist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-28 00:29:52.000000 audioalchemist-0.8.0/AudioAlchemist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5623 2024-05-28 00:29:52.788267 audioalchemist-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:29:52.788771 audioalchemist-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2024-05-28 00:28:22.000000 audioalchemist-0.8.0/setup.py
```

### Comparing `audioalchemist-0.5.6/AudioAlchemist/audio_alchemist.py` & `audioalchemist-0.8.0/AudioAlchemist/audio_alchemist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-# from pydub import AudioSegment
-# import glob
-# import pandas as pd
-# filelist = glob.glob('C:/Users/hikar/ds/data/melody/*.wav')
-# i=0
-# # 各CSVファイルを読み込み、連番を追加して再度CSVとして出力
-# for o in filelist:
-#   sourceAudio = AudioSegment.from_file(o,"wav")
-#   # 結果を出力
-#   i+=1
-#   audio="C:/Users/hikar/ds/data/melody/"+str(i)+".mp3"
-#   sourceAudio.export(audio, format="mp3")
-# print("処理が完了しました")
-# def AusioAlchemist(input_folder, output_folder, input_extension, output_extension):
-#   filelist = glob.glob(input_folder)
-#   i = 0
-#   # 各ファイルを読み込み、連番を追加して出力
-#   for file in filelist:
-#     source_audio = pydub.AudioSegment.from_file(file, input_extension)
-#     # 結果を出力
-#     output_file = output_folder + str(i) +"."+ output_extension
-#     source_audio.export(output_file, format=output_extension)
-#     i += 1
-#   print("処理が完了しました")
-
 import pydub
 import glob
+import os
 # import pandas as pd
 
 class AudioAlchemist:
     def __init__(self, input_folder, output_folder, input_extension, output_extension):
         self.input_folder = input_folder
         self.output_folder = output_folder
         self.input_extension = input_extension
         self.output_extension = output_extension
 
-    def process_files(self):
+    def process_files_index(self):
         filelist = glob.glob(self.input_folder)
         i = 0
         # Each file is read and a serial number is added and output
         for file in filelist:
             source_audio = pydub.AudioSegment.from_file(file, self.input_extension)
             # Output the result
             output_file = self.output_folder + str(i) +"."+ self.output_extension
             source_audio.export(output_file, format=self.output_extension)
             i += 1
         print("Processing completed")
+    # Create an instance of the AudioAlchemist class and call the process_files method
 
-# Create an instance of the AudioAlchemist class and call the process_files method
+    def process_files_namekeep(self):
+        # globパターンを修正して、フォルダ内のすべてのファイルを取得
+        filelist = glob.glob(self.input_folder)
+        for file in filelist:
+            # os.path.splitextを使用してファイル名と拡張子を分離
+            filename = os.path.splitext(os.path.basename(file))[0]
+            source_audio = pydub.AudioSegment.from_file(file, format=self.input_extension)
+            # 変換前のファイル名を保持して出力ファイル名を生成
+            output_file = os.path.join(self.output_folder, filename + '.' + self.output_extension)
+            source_audio.export(output_file, format=self.output_extension)
+        print("Processing completed")
 
 # # フォルダパスを設定
 # input_folder = 'C:/Users/hikar/ds/data/melody/*.wav'
 # output_folder = 'C:/Users/hikar/ds/data/melody/'
 # input_extension = "wav"
 # output_extension = "mp3"
 
 # audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
-# audio_alchemist.process_files()
+# audio_alchemist.process_files_index()
 
 # # 変換処理を実行
 # AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
```

### Comparing `audioalchemist-0.5.6/setup.py` & `audioalchemist-0.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# Author: TAKAHASHI Taro <takahashi.taro@takedasystem.com>
-# Copyright (c) 2022- TAKAHASHI Taro
 # Licence: MIT
 
 from setuptools import setup
 
 DESCRIPTION = 'Convert all files directly under the directory to any music file.'
 NAME = 'AudioAlchemist'
 AUTHOR = 'Kohki Suto'
 AUTHOR_EMAIL = 's2222019@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.5.6'
+VERSION = '0.8.0'
 PYTHON_REQUIRES = '>=3.6'
 INSTALL_REQUIRES = [
     "pydub>=0.25.1",
     "ffmpeg>=1.4"
     #ffmpeg-python==0.2.0
 ]
 PACKAGES = [
```

