# Comparing `tmp/QEasyWidgets-0.2.0.tar.gz` & `tmp/QEasyWidgets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.2.0.tar", last modified: Fri May 24 09:19:57 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.2.1.tar", last modified: Tue May 28 05:45:00 2024, max compression
```

## Comparing `QEasyWidgets-0.2.0.tar` & `QEasyWidgets-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.477033 QEasyWidgets-0.2.0/QEasyWidgets/
--rw-rw-rw-   0        0        0    24077 2024-05-24 09:18:44.000000 QEasyWidgets-0.2.0/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0    16782 2024-05-24 09:18:48.000000 QEasyWidgets-0.2.0/QEasyWidgets/QFunctions.py
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.0/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0    83693 2024-05-24 09:19:11.000000 QEasyWidgets-0.2.0/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    29648 2024-05-23 01:55:07.000000 QEasyWidgets-0.2.0/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.2.0/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.0/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.479651 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1570 2024-05-24 09:18:36.000000 QEasyWidgets-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:45:00.272417 QEasyWidgets-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-05-28 05:45:00.272417 QEasyWidgets-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 05:45:00.266459 QEasyWidgets-0.2.1/QEasyWidgets/
+-rw-rw-rw-   0        0        0    28398 2024-05-28 05:44:25.000000 QEasyWidgets-0.2.1/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0    16957 2024-05-28 05:44:27.000000 QEasyWidgets-0.2.1/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.1/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0    83693 2024-05-28 05:44:28.000000 QEasyWidgets-0.2.1/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    29648 2024-05-23 01:55:07.000000 QEasyWidgets-0.2.1/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.2.1/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.1/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:45:00.272417 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-28 05:45:00.000000 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-28 05:45:00.000000 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 05:45:00.000000 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-28 05:45:00.000000 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 05:45:00.000000 QEasyWidgets-0.2.1/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:45:00.272417 QEasyWidgets-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-05-28 05:44:20.000000 QEasyWidgets-0.2.1/setup.py
```

### Comparing `QEasyWidgets-0.2.0/LICENSE` & `QEasyWidgets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/PKG-INFO` & `QEasyWidgets-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.2.1/QEasyWidgets/ComponentsCustomizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from PySide6.QtWidgets import *
 from PySide6.QtMultimedia import QMediaPlayer, QAudioOutput
 
 from .QFunctions import *
 from .Sources import *
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class WidgetBase(QWidget):
     '''
     '''
     resized = Signal()
 
     def __init__(self,
@@ -23,14 +25,16 @@
         '''
         if self.minimumSizeHint() != self.size():
             self.adjustSize()
         '''
         super().resizeEvent(event)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class ButtonBase(QPushButton):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
@@ -47,19 +51,24 @@
             super().setProperty('hasIcon', True)
             self._icon = icon
         else:
             super().setProperty('hasIcon', False)
             self._icon = QIcon()
         super().setStyle(QApplication.style())
 
+    def icon(self) -> QIcon:
+        return Function_ToQIcon(self._icon)
+
     def _drawIcon(self, icon, painter, rect):
         Function_DrawIcon(icon, painter, rect)
 
     def paintEvent(self, e: QPaintEvent) -> None:
         super().paintEvent(e)
+        if self.icon().isNull():
+            return
         Width, Height = self.iconSize().width(), self.iconSize().height()
         #MinWidth, MinHeight = self.minimumSizeHint().width(), self.minimumSizeHint().height()
         LeftX = (self.width() - Width) /2
         TopY = (self.height() - Height) / 2
         Painter = QPainter(self)
         Painter.setRenderHints(QPainter.Antialiasing | QPainter.SmoothPixmapTransform)
         self._drawIcon(self._icon, Painter, QRectF(LeftX, TopY, Width, Height))
@@ -94,14 +103,16 @@
             MenuAction = QAction(text = Action, parent = self)
             MenuAction.triggered.connect(ActionEvents.get(Action))
             Menu.addAction(MenuAction)
             #Menu.addSeparator()
         self.setMenu(Menu)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class SpinBoxBase(QSpinBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
@@ -113,14 +124,15 @@
 
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.SpinBox.Deregistrate(self)
 
+##############################################################################################################################
 
 class DoubleSpinBoxBase(QDoubleSpinBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
@@ -133,14 +145,16 @@
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.SpinBox.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class ComboBoxBase(QComboBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
@@ -153,14 +167,16 @@
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.ComboBox.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class ScrollAreaBase(QScrollArea):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
@@ -168,33 +184,60 @@
 
         StyleSheetBase.ScrollArea.Apply(self)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.ScrollArea.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class TreeWidgetBase(QTreeWidget):
     '''
     '''
     def __init__(self, parent=None):
         super().__init__(parent=parent)
 
+        self.setColumnCount(1)
+
         self.header().setHighlightSections(False)
         self.header().setDefaultAlignment(Qt.AlignCenter)
+        #self.setHeaderHidden(True)
 
         self.setItemDelegate(QStyledItemDelegate(self))
         self.setIconSize(QSize(16, 16))
 
         StyleSheetBase.Tree.Apply(self)
 
+    def drawBranches(self, painter: QPainter, rect: QRect, index: Union[QModelIndex, QPersistentModelIndex]) -> None:
+        #rect.moveLeft(3)
+        super().drawBranches(painter, rect, index)
+
+    def rootItems(self) -> list[QTreeWidgetItem]:
+        RootItems = [self.topLevelItem(Index) for Index in range(0, self.topLevelItemCount())]
+        return RootItems
+
+    def rootItemTexts(self) -> list[str]:
+        RootItemTexts = [RootItem.text(0) for RootItem in self.rootItems()]
+        return RootItemTexts
+
+    def childItems(self, RootItem: QTreeWidgetItem) -> list[QTreeWidgetItem]:
+        ChildItems = [RootItem.child(Index) for Index in range(0, RootItem.childCount())]
+        return ChildItems
+
+    def childItemTexts(self, RootItem: QTreeWidgetItem) -> list[str]:
+        ChildItemTexts = [ChildItem.text(0) for ChildItem in self.childItems(RootItem)]
+        return ChildItemTexts
+
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Tree.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class LabelBase(QLabel):
     '''
     '''
     resized = Signal()
 
     def __init__(self,
@@ -208,14 +251,16 @@
         self.resized.emit()
         super().resizeEvent(event)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Label.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class ToolPage(WidgetBase):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None,
     ):
@@ -320,14 +365,16 @@
     def indexOf(self, widget: QWidget) -> int:
         return self.Pages.index(widget if isinstance(widget, ToolPage) else Function_FindParentUI(widget, ToolPage))
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.ToolBox.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class TableBase(QTableView):
     '''
     '''
     sorted = Signal()
 
     def __init__(self,
@@ -466,14 +513,16 @@
         while self.rowCount() > 0:
             self.removeRow(0)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Table.Deregistrate(self)
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class LineEdit(QLineEdit):
     '''
     '''
     focusedIn = Signal()
     focusedOut = Signal()
 
@@ -596,14 +645,16 @@
 
     def Alert(self, Enable: bool, Content: Optional[str] = None) -> None:
         self.IsAlerted = Enable
         StyleSheetBase.Edit.Apply(self)
         self.showToolTip(Content) if Enable else self.hideToolTip()
 
 ##############################################################################################################################
+##############################################################################################################################
+##############################################################################################################################
 
 class MediaPlayerBase(QWidget):
     '''
     '''
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
 
@@ -651,8 +702,10 @@
         self.MediaPlayer.stop()
         self.MediaPlayer.setSource('')
         #self.MediaPlayer.deleteLater()
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Player.Deregistrate(self)
 
+##############################################################################################################################
+##############################################################################################################################
 ##############################################################################################################################
```

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.2.1/QEasyWidgets/QFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,23 @@
     '''
     if isinstance(icon, IconBase):
         icon.paint(painter, rect, EasyTheme.THEME)
     else:
         icon = QIcon(icon)
         icon.paint(painter, QRectF(rect).toRect(), Qt.AlignCenter, state = QIcon.Off)
 
+
+def Function_ToQIcon(
+    icon: Union[str, QIcon, IconBase]
+):
+    if isinstance(icon, IconBase):
+        return icon.create()
+    else:
+        return QIcon(icon)
+
 ##############################################################################################################################
 
 class Language:
     '''
     '''
     ZH = 'Chinese'
     EN = 'English'
```

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.2.1/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/Sources.py` & `QEasyWidgets-0.2.1/QEasyWidgets/Sources.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/Utils.py` & `QEasyWidgets-0.2.1/QEasyWidgets/Utils.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.2.1/QEasyWidgets/WindowCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.2.1/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.2.0/README.md` & `QEasyWidgets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.2.0/setup.py` & `QEasyWidgets-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.2.0',
+    version = '0.2.1',
     description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
```

