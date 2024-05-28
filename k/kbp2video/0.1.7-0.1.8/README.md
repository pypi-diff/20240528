# Comparing `tmp/kbp2video-0.1.7.tar.gz` & `tmp/kbp2video-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.7.tar", last modified: Tue May 21 04:39:19 2024, max compression
+gzip compressed data, was "kbp2video-0.1.8.tar", last modified: Tue May 28 18:43:31 2024, max compression
```

## Comparing `kbp2video-0.1.7.tar` & `kbp2video-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.188326 kbp2video-0.1.7/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-05-13 01:35:06.000000 kbp2video-0.1.7/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-21 04:39:19.184992 kbp2video-0.1.7/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-05-13 01:35:06.000000 kbp2video-0.1.7/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.184992 kbp2video-0.1.7/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-21 04:39:02.000000 kbp2video-0.1.7/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    81159 2024-05-21 04:39:02.000000 kbp2video-0.1.7/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.184992 kbp2video-0.1.7/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       65 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      433 2024-05-21 04:39:02.000000 kbp2video-0.1.7/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-21 04:39:19.188326 kbp2video-0.1.7/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-28 18:43:31.477477 kbp2video-0.1.8/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-05-21 05:29:54.000000 kbp2video-0.1.8/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-28 18:43:31.477477 kbp2video-0.1.8/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-05-21 05:29:54.000000 kbp2video-0.1.8/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-28 18:43:31.474144 kbp2video-0.1.8/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-28 18:42:40.000000 kbp2video-0.1.8/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-05-21 05:29:54.000000 kbp2video-0.1.8/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-05-21 05:29:54.000000 kbp2video-0.1.8/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    84205 2024-05-28 18:42:40.000000 kbp2video-0.1.8/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-05-21 05:29:54.000000 kbp2video-0.1.8/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     3824 2024-05-28 18:42:40.000000 kbp2video-0.1.8/kbp2video/progress_window.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-05-21 05:29:54.000000 kbp2video-0.1.8/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-28 18:43:31.477477 kbp2video-0.1.8/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      397 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       65 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-28 18:43:31.000000 kbp2video-0.1.8/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      433 2024-05-21 05:29:54.000000 kbp2video-0.1.8/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-28 18:43:31.477477 kbp2video-0.1.8/setup.cfg
```

### Comparing `kbp2video-0.1.7/LICENSE` & `kbp2video-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.7/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.8/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.7/kbp2video/_gui.py` & `kbp2video-0.1.8/kbp2video/_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import time #sleep
 import fractions
 from PySide6.QtCore import *  # type: ignore
 from PySide6.QtGui import *  # type: ignore
 from PySide6.QtWidgets import *  # type: ignore
 from .utils import ClickLabel, bool2check, check2bool, mimedb
 from .advanced_editor import AdvancedEditor
+from .progress_window import ProgressWindow
 import ffmpeg
 from ._ffmpegcolor import ffmpeg_color
 import enum
 import kbputils
 import io
 import shutil
 from . import __version__
@@ -473,23 +474,26 @@
             print(event)
         event.acceptProposedAction()
 
     def dragLeaveEvent(self, event):
         self.parentWidget().setCurrentIndex(0)
 
 class ConverterSignals(QObject):
+    started = Signal()
     finished = Signal()
-    progress = Signal(int, int)
+    progress = Signal(int, int, str, int, int)
+    error = Signal(str, bool)
     data = Signal(dict)
 
 class Converter(QRunnable):
     def __init__(self, function, *args, **kwargs):
         super().__init__()
         self.signals = ConverterSignals()
         self.function = function
+        self.signals.cancelled = False #TODO: Seems to work, but is this a good idea?
         self.args = args
         self.kwargs = kwargs
 
     @Slot()
     def run(self):
         self.function(self.signals, *self.args, **self.kwargs)
 
@@ -507,22 +511,22 @@
             if version:
                 result['version'] = version
                 result['urls'] = lastversion.latest(repo='ItMightBeKaraoke/kbp2video', pre_ok=True, output_format='assets')
         except:
             result = {'error': traceback.format_exc(limit=2)}
         signals.data.emit(result)
 
-    def __init__(self, parent, threadpool):
+    def __init__(self, parent):
         super().__init__(QMessageBox.Information, "Check for updates", "Checking for updates...", QMessageBox.StandardButton(QMessageBox.Ok), parent=parent)
         self.runner = Converter(self._lastversion_wrap)
         self.runner.signals.data.connect(self._display_data)
-        threadpool.start(self.runner)
+        QThreadPool.globalInstance().start(self.runner)
     
-    def update_check(parent, threadpool):
-        box = UpdateBox(parent, threadpool)
+    def update_check(parent):
+        box = UpdateBox(parent)
         box.exec()
 
     def _display_data(self, data):
         if 'error' in data:
             self.setWindowTitle("Check for updates: failed!")
             self.setText(f"Failed to check for update:\n{data['error']}")
         elif data:
@@ -538,15 +542,14 @@
 class Ui_MainWindow(QMainWindow):
 
     RELEVANT_FILE_FILTER = "*." + " *.".join(
         "kbp flac wav ogg opus mp3 aac mp4 mkv avi webm mov mpg mpeg jpg jpeg png gif jfif jxl bmp tiff webp".split())
 
     def __init__(self, app):
         super().__init__()
-        self.threadpool = QThreadPool()
         self.app = app
         self.setupUi()
 
     # Convenience method for adding a Qt object as a property in self and and
     # setting its Qt object name
     def bind(self, name, obj):
         setattr(self, name, obj)
@@ -573,28 +576,28 @@
         #self.editmenu.addAction("&Select All", self.select_all)
         self.editmenu.addAction("&Remove Selected", QKeySequence.Delete, self.remove_files_button)
         self.editmenu.addAction("&Add empty row", self.add_row_button)
         self.editmenu.addAction("&Open/Edit Selected Files", QKeySequence.Open, self.remove_files_button)
         self.editmenu.addAction("&Intro/Outro Settings", Qt.CTRL | Qt.Key_Return, self.advanced_button)
         self.helpmenu = self.menubar.addMenu("Help")
         self.helpmenu.addAction("&About", lambda: QMessageBox.about(self, "About kbp2video", f"kbp2video version: {__version__}\n\nUsing:\nkbputils version: {kbputils.__version__}\nffmpeg version: {ffmpeg_version}"))
-        self.helpmenu.addAction("&Check for Updates...", lambda: UpdateBox.update_check(self, self.threadpool))
+        self.helpmenu.addAction("&Check for Updates...", lambda: UpdateBox.update_check(self))
         self.setMenuBar(self.menubar)
 
         self.setStatusBar(self.bind("statusbar", QStatusBar(self)))
 
         # No point in updating the status bar with empty messages
         self.installEventFilter(EventFilter(self, lambda obj, event: True if event.type() == QEvent.StatusTip and not event.tip() else False))
 
         try:
             q = QProcess(program="ffmpeg", arguments=["-version"])
             q.start()
             q.waitForFinished(1000)
             q.setReadChannel(QProcess.StandardOutput)
-            version_line = str(q.readLine()).split()
+            version_line = q.readLine().toStdString().split()
             ffmpeg_version = version_line[i+1] if (i := version_line.index("version")) else 'UNKNOWN'
         except:
             ffmpeg_version = "MISSING/UNKNOWN"
         self.statusbar.showMessage(f"kbp2video {__version__} (kbputils {kbputils.__version__}, ffmpeg {ffmpeg_version})")
 
         QCoreApplication.setOrganizationName("ItMightBeKaraoke")
         QCoreApplication.setApplicationName("kbp2video")
@@ -1137,21 +1140,23 @@
         self.skipBackgrounds.setCheckState(bool2check(self.settings.value("kbp2video/ignore_bg_files_drag_drop", type=bool, defaultValue=False)))
         self.saveSettings()  # Save to disk any new defaults that were used
 
     def runAssConversion(self):
         self.saveSettings()
         converter = Converter(self.conversion_runner, assOnly = True)
         # worker.signals.finished.connect
-        self.threadpool.start(converter)
+        QThreadPool.globalInstance().start(converter)
 
     def runConversion(self):
         self.saveSettings()
         converter = Converter(self.conversion_runner)
         # worker.signals.finished.connect
-        self.threadpool.start(converter)
+        QThreadPool.globalInstance().start(converter)
+        if not ProgressWindow.showProgressWindow(self.tableWidget.rowCount(), converter.signals, self):
+            converter.signals.cancelled = True
 
     def resolved_output_dir(self, kbp):
         if check2bool(self.relative):
 
             # If relative is set, assume .ass dir is the output dir because we
             # no longer know the project file
             if kbp.endswith(".ass"):
@@ -1211,14 +1216,15 @@
                 QMessageBox.Yes | QMessageBox.No))
 
     @Slot(str, str)
     def info(self, title, text):
         QMessageBox.information(self, title, text)
 
     def conversion_runner(self, signals, assOnly = False):
+        signals.started.emit()
         unsupported_message = False
         kbputils_options = {}
         ratio, border = self.get_aspect_ratio()
         if ratio[0] is None or border is None:
             QMetaObject.invokeMethod(
                 self,
                 'info', 
@@ -1254,26 +1260,28 @@
             kbputils_options['offset'] = self.offset.value()
         if self.transparencyBox.checkState() != Qt.Checked:
             kbputils_options['transparency'] = False
         if self.ktBox.checkState() == Qt.Checked:
             kbputils_options['allow_kt'] = True
         kbputils_options['overflow'] = kbputils.AssOverflow[self.overflowBox.currentText().replace(" ", "_").upper()]
         conversion_errors = False
+        ffmpeg_processes = []
         for row in range(self.tableWidget.rowCount()):
             kbp_table_item = self.tableWidget.item(row, TrackTableColumn.KBP_ASS.value)
             kbp_obj = kbp_table_item.data(Qt.UserRole) or kbp_table_item.text()
             kbp = str(kbp_obj)
             audio = self.tableWidget.filename(row, TrackTableColumn.Audio.value)
             background = self.tableWidget.filename(row, TrackTableColumn.Background.value)
             advanced = self.tableWidget.item(row, TrackTableColumn.Advanced.value).data(Qt.UserRole) or {}
             print(f"Retrieved Advanced settings for {kbp}:")
             print(advanced)
             if not kbp:
                 continue
             self.statusbar.showMessage(f"Converting file {row+1} of {self.tableWidget.rowCount()} ({kbp})")
+            signals.progress.emit(row, self.tableWidget.rowCount(), kbp, 0, 0)
             background_type = None
             if not background:
                 pass
             elif background.startswith("color:"):
                 background = background[6:].strip(" #")
                 background_type = 0
             elif (mimename := self.filedrop.mimedb.mimeTypeForFile(background).name()).startswith('image/'):
@@ -1289,61 +1297,75 @@
 
             # Handle manually-typed filename. TODO: convert earlier, when the text value is updated
             if not isinstance(kbp_obj, KBPASSWrapper):
                 try:
                     kbp_obj = KBPASSWrapper(kbp_obj)
                 except:
                     conversion_errors = True
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info', 
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Failed to process file"),
-                        Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info', 
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Failed to process file"),
+                    #    Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
+                    signals.error.emit(f"Failed to process file\n{kbp}\n\nError Output:\n{traceback.format_exc()}", True)
                     continue
             if hasattr(kbp_obj, "kbp_path"):
                 print("Converting the new way")
                 print(kbputils_options)
                 try:
                     data = kbp_obj.ass_data(**kbputils_options)
                 except:
                     conversion_errors = True
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info', 
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Failed to process kbp"),
-                        Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info', 
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Failed to process kbp"),
+                    #    Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}"))
+                    signals.error.emit(f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}", True)
                     continue
             else: # kbp_obj is a KBPASSWrapper with a .ass file
                 if any(x in kbp for x in ":;,'=\""):
                     print("Already .ass file, but needs new filename for ffmpeg")
                     QFile(kbp).copy(assfile)
                 else:
                     print("Using existing .ass file")
                     assfile = kbp
                     
             # QDir is inconsistent. Needs to be static to check existence, and
             # mkdir needs to be run from an instantiated instance in the parent
             # directory, not worth the hassle
             if not os.path.isdir(outdir := self.resolved_output_dir(kbp)):
-                os.mkdir(outdir)
+                try:
+                    os.mkdir(outdir)
+                except:
+                    conversion_errors = True
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info', 
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Failed to create output folder"),
+                    #    Q_ARG(str, f"Failed to create missing output folder\n{outdir}\n\nError Output:\n{traceback.format_exc()}"))
+                    signals.error.emit(f"Failed to create output folder\n{outdir}\nassociated with .kbp file\n{kbp}\n\nError Output:\n{traceback.format_exc()}", True)
+                    continue
 
             # File was converted and .ass file needs to be written
             if kbp.endswith(".kbp"):
                 f = QFile(assfile)
                 if f.exists():
                     answer = QMessageBox.StandardButton(QMetaObject.invokeMethod(
                         self,
                         'yesno',
                         Qt.BlockingQueuedConnection,
                         Q_RETURN_ARG(int),
                         Q_ARG(str, "Replace file?"),
                         Q_ARG(str, f"Overwrite {assfile}?")))
                     if answer != QMessageBox.Yes:
+                        signals.error.emit(f"Skipped {kbp} per user request (.ass file exists)", True)
                         continue
                 if not f.open(QIODevice.WriteOnly | QIODevice.Text):
                     continue
                 out = QTextStream(f)
                 out << data
                 f.close()
                 if assOnly:
@@ -1365,54 +1387,54 @@
                 background_video = ffmpeg.input(background, loop=1, framerate=60)
             elif background_type == 2:
                 # Pull the dimensions of the first video stream found in the file
                 try:
                     bginfo = ffmpeg.probe(background)
                 except:
                     conversion_errors = True
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info',
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Unable to process background video"),
-                        Q_ARG(str, f"Unable to determine the resolution of file\n{background}\n{traceback.format_exc()}"))
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info',
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Unable to process background video"),
+                    #    Q_ARG(str, f"Unable to determine the resolution of file\n{background}\n{traceback.format_exc()}"))
+                    signals.error.emit(f"Skipped {kbp}:\nUnable to determine the resolution of background file\n{background}\n{traceback.format_exc()}", True)
                     continue
                 bg_size = next(QSize(x['width'],x['height']) for x in bginfo['streams'] if x['codec_type'] == 'video')
                 background_video = ffmpeg.input(background).video
 
-            song_length = None
+            try:
+                song_length = ffmpeg.probe(audio)['format']['duration']
+                song_length_float = float(song_length)
+            except:
+                conversion_errors = True
+                #QMetaObject.invokeMethod(
+                #    self,
+                #    'info',
+                #    Qt.AutoConnection,
+                #    Q_ARG(str, "Unable to process audio"),
+                #    Q_ARG(str, f"Unable to process audio file\n{audio}\n{traceback.format_exc()}"))
+                signals.error.emit(f"Skipped {kbp}:\nUnable to process audio file\n{audio}\n{traceback.format_exc()}", True)
+                continue
+            song_length_us = int(song_length_float * 1e6)
             # TODO figure out time/frame for outro
             for x in ("intro", "outro"):
                 if f"{x}_enable" in advanced and advanced[f"{x}_enable"]:
-                    if not song_length:
-                        try:
-                            song_length = ffmpeg.probe(audio)['format']['duration']
-                        except:
-                            conversion_errors = True
-                            QMetaObject.invokeMethod(
-                                self,
-                                'info',
-                                Qt.AutoConnection,
-                                Q_ARG(str, "Unable to process audio"),
-                                Q_ARG(str, f"Unable to process audio file\n{audio}\n{traceback.format_exc()}"))
-                            # See continue after this loop that skips iteration of outer loop
-                            song_length = -1
-                            break
                     # TODO: alpha, sound?
                     opts = {}
                     if self.filedrop.mimedb.mimeTypeForFile(advanced[f"{x}_file"]).name().startswith('image/'):
                         opts["loop"]=1
                         opts["framerate"]=60
                     # TODO skip scale if matching?
                     # TODO set x/y if mismatched aspect ratio?
                     overlay = ffmpeg.input(advanced[f"{x}_file"], t=advanced[f"{x}_length"], **opts).filter_(
                         "scale", s=f"{bg_size.width()}x{bg_size.height()}")
                     if x == "outro":
                         #leadin = ffmpeg_color("000000", s=f"{bg_size.width()}x{bg_size.height()}", r=60, d=(float(song_length) - float(advanced[f"{x}_length"].split(":")[1]))).filter_("format", "rgba")
-                        leadin = ffmpeg.input(f"color=color=000000:r=60:s={bg_size.width()}x{bg_size.height()}", f="lavfi", t=(float(song_length) - float(advanced[f"{x}_length"].split(":")[1])))
+                        leadin = ffmpeg.input(f"color=color=000000:r=60:s={bg_size.width()}x{bg_size.height()}", f="lavfi", t=(song_length_float - float(advanced[f"{x}_length"].split(":")[1])))
                         overlay = leadin.concat(overlay)
                     for y in ("In", "Out"):
                         if float(advanced[f"{x}_fade{y}"].split(":")[1]):
                             # TODO: minutes
                             fade_settings = {}
                             print(advanced[f"{x}_black"])
                             if not advanced[f"{x}_black"] or (x, y) == ("intro", "Out") or (x, y) == ("outro", "In"):
@@ -1420,43 +1442,40 @@
                             if x == "intro":
                                 if y == "In":
                                     fade_settings["st"] = 0
                                 else:
                                     fade_settings["st"] = float(advanced[f"{x}_length"].split(":")[1]) - float(advanced[f"{x}_fadeOut"].split(":")[1])
                             else:
                                 if y == "Out":
-                                    fade_settings["st"] = float(song_length) - float(advanced[f"{x}_fadeOut"].split(":")[1])
+                                    fade_settings["st"] = song_length_float - float(advanced[f"{x}_fadeOut"].split(":")[1])
                                 else:
-                                    fade_settings["st"] = float(song_length) - float(advanced[f"{x}_length"].split(":")[1])
+                                    fade_settings["st"] = song_length_float - float(advanced[f"{x}_length"].split(":")[1])
                             overlay = overlay.filter_("fade", t=y.lower(), d=advanced[f"{x}_fade{y}"].split(":")[1], **fade_settings)
                     background_video = background_video.overlay(overlay, eof_action=("pass" if x == "intro" else "repeat"))
 
-            # Broke from inner loop after error
-            if song_length == -1:
-                continue
-
             audio_stream = ffmpeg.input(audio).audio
             if background_type == 1 or background_type == 2:
                 if not bg_size:
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info',
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Unsupported Background file"),
-                        Q_ARG(str, f"Unable to determine the resolution of file\n{background}"))
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info',
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Unsupported Background file"),
+                    #    Q_ARG(str, f"Unable to determine the resolution of file\n{background}"))
+                    signals.error.emit(f"Skipped {kbp}:\nUnable to determine the resolution of background file\n{background}\n{traceback.format_exc()}", True)
                     continue
                 if self.overrideBGResolution.checkState == Qt.Checked and not unsupported_message:
-                    QMetaObject.invokeMethod(
-                        self,
-                        'info',
-                        Qt.AutoConnection,
-                        Q_ARG(str, "Unsupported Option"),
-                        Q_ARG(str, f"Override background resolution option not supported yet!"))
+                    #QMetaObject.invokeMethod(
+                    #    self,
+                    #    'info',
+                    #    Qt.AutoConnection,
+                    #    Q_ARG(str, "Unsupported Option"),
+                    #    Q_ARG(str, f"Override background resolution option not supported yet!"))
+                    signals.error.emit(f"Unsupported option Override Background selected, ignoring", False)
                     unsupported_message = True
-                    continue
 
             bg_ratio = fractions.Fraction(bg_size.width(), bg_size.height())
             ass_ratio = fractions.Fraction(width, border and 216 or 192)
             if bg_ratio > ass_ratio:
                 # letterbox sides
                 ass_size = QSize(round(bg_size.height() * ass_ratio), bg_size.height())
                 # ass_move = f":x={round((bg_size.width() - ass_size.width())/2)}"
@@ -1501,31 +1520,55 @@
                 output_options["row-mt"] = 1 # Speeds up encode for most multicore systems
 
             output_options.update({
                 "pix_fmt": "yuv420p",
                 "c:a": self.acodecBox.currentText(),
                 "c:v": self.vcodecBox.currentText(),
                 "hide_banner": None,
+                "progress": "-",
+                "loglevel": "warning"
             })
             # TODO: determine if it's best to leave this as a QProcess, or use ffmpeg.run() and have it POpen itself
             ffmpeg_options = ffmpeg.output(filtered_video, audio_stream, self.vidFile(kbp), **output_options).overwrite_output().get_args()
             print(f'cd "{os.path.dirname(assfile)}"')
             print("ffmpeg" + " " + " ".join(f'"{x}"' for x in ffmpeg_options))
             q = QProcess(program="ffmpeg", arguments=ffmpeg_options, workingDirectory=os.path.dirname(assfile))
+            q.setReadChannel(QProcess.StandardOutput)
+            ffmpeg_processes.append((kbp, song_length_us, q))
+
+        for row, (kbp, song_length_us, q) in enumerate(ffmpeg_processes):
             q.start()
-            q.waitForFinished(-1)
+            q.waitForStarted(-1)
+            while not q.waitForFinished(100):
+                if signals.cancelled:
+                    self.statusbar.showMessage(f"Conversion cancelled during file {row+1} of {len(ffmpeg_processes)}!")
+                    signals.finished.emit()
+                    return
+                while q.canReadLine():
+                    if (ffmpeg_out_line := q.readLine().toStdString()).startswith("out_time_us="):
+                        try:
+                            out_time = int(ffmpeg_out_line.split("=")[1])
+                        except:
+                            pass # TODO: maybe switch to throbber if ffmpeg isn't outputting progress properly?
+                        else:
+                            signals.progress.emit(row, len(ffmpeg_processes), kbp, out_time, song_length_us)
+
             if q.exitStatus() != QProcess.NormalExit or q.exitCode() != 0:
                 conversion_errors = True
-                QMetaObject.invokeMethod(
-                    self,
-                    'info',
-                    Qt.AutoConnection,
-                    Q_ARG(str, "Failed to convert file"),
-                    Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}"))
+                #QMetaObject.invokeMethod(
+                #    self,
+                #    'info',
+                #    Qt.AutoConnection,
+                #    Q_ARG(str, "Failed to convert file"),
+                #    Q_ARG(str, f"Failed to process file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}"))
+                signals.error.emit(f"Failed to process file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}", True)
+                print(q.exitStatus())
+                print(q.exitCode())
 
+            signals.progress.emit(row, len(ffmpeg_processes), kbp, song_length_us, song_length_us)
         
         self.statusbar.showMessage(f"Conversion completed{' (with errors)' if conversion_errors else ''}!")
         signals.finished.emit()
 
     def retranslateUi(self):
         self.setWindowTitle(QCoreApplication.translate(
             "MainWindow", "KBP to Video", None))
```

### Comparing `kbp2video-0.1.7/kbp2video/advanced_editor.py` & `kbp2video-0.1.8/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.7/kbp2video/utils.py` & `kbp2video-0.1.8/kbp2video/utils.py`

 * *Files identical despite different names*

