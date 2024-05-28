# Comparing `tmp/nxsrecselector-3.39.0.tar.gz` & `tmp/nxsrecselector-3.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.39.0.tar", last modified: Thu Jan 25 13:50:01 2024, max compression
+gzip compressed data, was "nxsrecselector-3.40.0.tar", last modified: Tue May 28 07:07:10 2024, max compression
```

## Comparing `nxsrecselector-3.39.0.tar` & `nxsrecselector-3.40.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-01-25 13:50:01.175167 nxsrecselector-3.39.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.39.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.39.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.39.0/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2024-01-25 13:50:01.175167 nxsrecselector-3.39.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.39.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-01-25 13:50:01.171167 nxsrecselector-3.39.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2023-11-08 19:25:43.000000 nxsrecselector-3.39.0/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   113758 2024-01-25 13:48:01.000000 nxsrecselector-3.39.0/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-01-25 13:50:01.175167 nxsrecselector-3.39.0/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    25288 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23951 2024-01-25 13:48:01.000000 nxsrecselector-3.39.0/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20060 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    76606 2024-01-25 13:48:01.000000 nxsrecselector-3.39.0/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    61815 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2024-01-25 13:48:01.000000 nxsrecselector-3.39.0/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16786 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    46944 2024-01-25 13:48:01.000000 nxsrecselector-3.39.0/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5799 2023-11-13 08:11:24.000000 nxsrecselector-3.39.0/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29585 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-11-08 19:25:10.000000 nxsrecselector-3.39.0/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-01-25 13:50:01.175167 nxsrecselector-3.39.0/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2024-01-25 13:50:01.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2024-01-25 13:50:01.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-01-25 13:50:01.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2024-01-25 13:50:01.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2024-01-25 13:50:01.000000 nxsrecselector-3.39.0/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2024-01-25 13:50:01.175167 nxsrecselector-3.39.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4035 2023-06-29 15:14:01.000000 nxsrecselector-3.39.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-28 07:07:10.773605 nxsrecselector-3.40.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.40.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.40.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.40.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5449 2024-05-28 07:07:10.773605 nxsrecselector-3.40.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.40.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-28 07:07:10.769605 nxsrecselector-3.40.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2023-11-08 19:25:43.000000 nxsrecselector-3.40.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   113774 2024-05-28 07:06:11.000000 nxsrecselector-3.40.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-28 07:07:10.773605 nxsrecselector-3.40.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25288 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23951 2024-01-25 13:48:01.000000 nxsrecselector-3.40.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20060 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    76606 2024-01-25 13:48:01.000000 nxsrecselector-3.40.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    61868 2024-05-28 07:03:45.000000 nxsrecselector-3.40.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2024-05-28 07:03:45.000000 nxsrecselector-3.40.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16786 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46944 2024-01-25 13:48:01.000000 nxsrecselector-3.40.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5799 2023-11-13 08:11:24.000000 nxsrecselector-3.40.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29585 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-11-08 19:25:10.000000 nxsrecselector-3.40.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-28 07:07:10.773605 nxsrecselector-3.40.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5449 2024-05-28 07:07:10.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2024-05-28 07:07:10.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-05-28 07:07:10.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2024-05-28 07:07:10.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2024-05-28 07:07:10.000000 nxsrecselector-3.40.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2024-05-28 07:07:10.773605 nxsrecselector-3.40.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4036 2024-05-28 07:04:02.000000 nxsrecselector-3.40.0/setup.py
```

### Comparing `nxsrecselector-3.39.0/COPYRIGHT` & `nxsrecselector-3.40.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/NXSRecSelector` & `nxsrecselector-3.40.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/README.rst` & `nxsrecselector-3.40.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/man/NXSRecSelector.1` & `nxsrecselector-3.40.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/man/nxsrecconfig.1` & `nxsrecselector-3.40.0/man/nxsrecconfig.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSRECCONFIG" "1" "Jan 25, 2024" "3.39" "NXSRecSelector"
-.SH NAME
-nxsrecconfig \- nxsrecconfig Documentation
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSRECCONFIG" "1" "May 28, 2024" "3.40" "NXSRecSelector"
+.SH NAME
+nxsrecconfig \- nxsrecconfig Documentation
 .sp
 \fI\%\fP
 \fI\%\fP
 \fI\%\fP
 \fI\%\fP
 .sp
 Authors: Jan Kotanski
@@ -314,27 +314,27 @@
 .SH NXSRECCONFIG PACKAGE
 .SS Submodules
 .SS nxsrecconfig.CheckerThread module
 .sp
 Component CheckerThread \- thread which checks tango server attributes
 .INDENT 0.0
 .TP
-.B nxsrecconfig.CheckerThread.ATTRIBUTESTOCHECK = [\(aqValue\(aq, \(aqPosition\(aq, \(aqCounts\(aq, \(aqData\(aq, \(aqVoltage\(aq, \(aqEnergy\(aq, \(aqSampleTime\(aq]
+.B nxsrecconfig.CheckerThread.ATTRIBUTESTOCHECK  =  [\(aqValue\(aq, \(aqPosition\(aq, \(aqCounts\(aq, \(aqData\(aq, \(aqVoltage\(aq, \(aqEnergy\(aq, \(aqSampleTime\(aq]
 (\fI\%list\fP < \fI\%str\fP>) default attributes to check
 .UNINDENT
 .INDENT 0.0
 .TP
-.B exception nxsrecconfig.CheckerThread.AlarmStateError
+.B exception  nxsrecconfig.CheckerThread.AlarmStateError
 Bases: \fI\%Exception\fP
 .sp
 Alarm State Exception class
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.CheckerThread.CheckerItem(name)
+.B class  nxsrecconfig.CheckerThread.CheckerItem(name)
 Bases: \fI\%list\fP
 .sp
 Checker list Item
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -360,16 +360,16 @@
 .TP
 .B name
 (\fI\%str\fP) checker name
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.CheckerThread.CheckerThread(index, queue)
-Bases: \fI\%threading.Thread\fP
+.B class  nxsrecconfig.CheckerThread.CheckerThread(index, queue)
+Bases: \fI\%Thread\fP
 .sp
 Single CheckerThread
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Brief
@@ -407,29 +407,29 @@
 .TP
 .B tangoSourceWarningStates
 (\fI\%list\fP <\fI\%str\fP>) tango datasources warning states
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B exception nxsrecconfig.CheckerThread.FaultStateError
+.B exception  nxsrecconfig.CheckerThread.FaultStateError
 Bases: \fI\%Exception\fP
 .sp
 Fault State Exception class
 .UNINDENT
 .INDENT 0.0
 .TP
-.B exception nxsrecconfig.CheckerThread.OffStateError
+.B exception  nxsrecconfig.CheckerThread.OffStateError
 Bases: \fI\%Exception\fP
 .sp
 Off State Exception class
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.CheckerThread.TangoDSItem(name=None, device=None, attr=None)
+.B class  nxsrecconfig.CheckerThread.TangoDSItem(name=None, device=None, attr=None)
 Bases: \fI\%object\fP
 .sp
 Tango DataSource item
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -460,15 +460,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.Converter module
 .sp
 Selection version converter
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.Converter(ver)
+.B class  nxsrecconfig.Converter.Converter(ver)
 Bases: \fI\%object\fP
 .sp
 selection version converter
 .sp
 contstructor
 .INDENT 7.0
 .TP
@@ -477,15 +477,15 @@
 .UNINDENT
 .INDENT 7.0
 .TP
 .B allkeys(selection)
 .INDENT 7.0
 .TP
 .B Parameters
-\fBselection\fP (\fInxsrecconfig.Selection.Selection\fP) – selection dictionary object
+\fBselection\fP (\fI\%nxsrecconfig.Selection.Selection\fP) – selection dictionary object
 .TP
 .B Returns
 selection keys
 .TP
 .B Return type
 \fI\%set\fP
 .UNINDENT
@@ -523,37 +523,37 @@
 .INDENT 7.0
 .TP
 .B up
 (\fI\%list\fP <\fI\%ConverterXtoY\fP>) converter up sequence
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod version(selection)
+.B classmethod  version(selection)
 .INDENT 7.0
 .TP
 .B fetches selection version and converts it
 into (major, minor, patch)
 .UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
-\fBselection\fP (\fInxsrecconfig.Selection.Selection\fP) – selection dictionary object
+\fBselection\fP (\fI\%nxsrecconfig.Selection.Selection\fP) – selection dictionary object
 .TP
 .B Returns
 (major, minor, patch) tuple with integers
 .TP
 .B Return type
 (\fI\%int\fP , \fI\%int\fP , \fI\%int\fP)
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.Converter1to2
-Bases: \fI\%nxsrecconfig.Converter.ConverterXtoY\fP
+.B class  nxsrecconfig.Converter.Converter1to2
+Bases: \fI\%ConverterXtoY\fP
 .sp
 Selection converter from version 1 to 2
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B convert(selection)
@@ -573,16 +573,16 @@
 .TP
 .B pnames
 (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) names of properties
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.Converter2to1
-Bases: \fI\%nxsrecconfig.Converter.ConverterXtoY\fP
+.B class  nxsrecconfig.Converter.Converter2to1
+Bases: \fI\%ConverterXtoY\fP
 .sp
 Selection converter from version 2 to 1
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B convert(selection)
@@ -602,16 +602,16 @@
 .TP
 .B pnames
 (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) names of properties
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.Converter2to3
-Bases: \fI\%nxsrecconfig.Converter.ConverterXtoY\fP
+.B class  nxsrecconfig.Converter.Converter2to3
+Bases: \fI\%ConverterXtoY\fP
 .sp
 Selection converter from version 2 to 3
 .sp
 converter
 .INDENT 7.0
 .TP
 .B convert(selection)
@@ -642,16 +642,16 @@
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.Converter3to2
-Bases: \fI\%nxsrecconfig.Converter.ConverterXtoY\fP
+.B class  nxsrecconfig.Converter.Converter3to2
+Bases: \fI\%ConverterXtoY\fP
 .sp
 Selection converter from version 3 to 2
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B convert(selection)
@@ -706,15 +706,15 @@
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Converter.ConverterXtoY
+.B class  nxsrecconfig.Converter.ConverterXtoY
 Bases: \fI\%object\fP
 .sp
 virtual selection version converter
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -733,15 +733,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.Describer module
 .sp
 Component Describer
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Describer.DSItem(name=None, dstype=None, record=None, dsitem=None, parentobj=None)
+.B class  nxsrecconfig.Describer.DSItem(name=None, dstype=None, record=None, dsitem=None, parentobj=None)
 Bases: \fI\%object\fP
 .sp
 Basic DataSource item
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -778,15 +778,15 @@
 .TP
 .B record
 (\fI\%str\fP) datasource record
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Describer.Describer(nexusconfig_device, tree=False, pyevalfromscript=False)
+.B class  nxsrecconfig.Describer.Describer(nexusconfig_device, tree=False, pyevalfromscript=False)
 Bases: \fI\%object\fP
 .sp
 Lists datasources, strategy, dstype and record name
 of given component
 .sp
 constructor
 .INDENT 7.0
@@ -861,15 +861,15 @@
 .B Return type
 [\fI\%dict\fP <\fI\%str\fP, \fI\%ExDSDict\fP > ] or                 [{“dsname”: \fI\%str\fP, “dstype”: \fI\%str\fP,                   “record”: \fI\%str\fP}, …]
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Describer.ExDSDict(*args, **kw)
+.B class  nxsrecconfig.Describer.ExDSDict(*args, **kw)
 Bases: \fI\%dict\fP
 .sp
 Extended DataSource Dictionary
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -906,16 +906,16 @@
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Describer.ExDSItem(dsitem=None, mode=None, nxtype=None, shape=None)
-Bases: \fI\%nxsrecconfig.Describer.DSItem\fP
+.B class  nxsrecconfig.Describer.ExDSItem(dsitem=None, mode=None, nxtype=None, shape=None)
+Bases: \fI\%DSItem\fP
 .sp
 Extended DataSource item
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
@@ -947,15 +947,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.DynamicComponent module
 .sp
 Dynamic Component
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.DynamicComponent.DynamicComponent(nexusconfig_device, defaultpath="/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection", defaulttype=\(aqNX_CHAR\(aq, defaultuserpath="/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/user_data:NXparameters")
+.B class  nxsrecconfig.DynamicComponent.DynamicComponent(nexusconfig_device, defaultpath=\(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection\(dq, defaulttype=\(aqNX_CHAR\(aq, defaultuserpath=\(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/user_data:NXparameters\(dq)
 Bases: \fI\%object\fP
 .sp
 Creates dynamic component
 of given component
 .sp
 constructor
 .INDENT 7.0
@@ -1065,15 +1065,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.MacroServerPools module
 .sp
 Selection state
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.MacroServerPools.MacroServerPools(numberOfThreads)
+.B class  nxsrecconfig.MacroServerPools.MacroServerPools(numberOfThreads)
 Bases: \fI\%object\fP
 .sp
 sardanamacro server and pools
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -1253,16 +1253,16 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.NXSConfig module
 .sp
 Selector Server for NeXus Sardana Recorder
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.NXSConfig.NXSRecSelector(cl, name)
-Bases: \fI\%tango.device_server.LatestDeviceImpl\fP
+.B class  nxsrecconfig.NXSConfig.NXSRecSelector(cl, name)
+Bases: \fI\%LatestDeviceImpl\fP
 .sp
 NXSRecSelector server interface
 .INDENT 7.0
 .TP
 .B Brief
 Tango Server for Nexus Sardana Recorder Settings.
 Device States Description:
@@ -2965,55 +2965,55 @@
 .B Parameters
 \fBattr\fP (\fI\%tango.Attribute\fP) – written attribute
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.NXSConfig.NXSRecSelectorClass(name)
-Bases: \fBtango._tango.DeviceClass\fP
+.B class  nxsrecconfig.NXSConfig.NXSRecSelectorClass(name)
+Bases: \fBDeviceClass\fP
 .sp
 NXSRecSelectorclass Constructor
 .INDENT 7.0
 .TP
-.B attr_list = {\(aqAppendEntry\(aq: [[tango._tango.CmdArgType.DevBoolean, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqAppend Entry\(aq, \(aqdescription\(aq: \(aqflag for entry appending\(aq}], \(aqCanFailDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to be switch into canfail mode\(aq, \(aqdescription\(aq: \(aqlist of datasources to be switched into canfail mode\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqComponents\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqSelected Components\(aq, \(aqdescription\(aq: \(aqlist of Selected Components\(aq}], \(aqConfigDevice\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqConfiguration Device\(aq, \(aqdescription\(aq: \(aqConfiguration device name\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqConfigVariables\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqConfiguration Variables\(aq, \(aqdescription\(aq: \(aqJSON dictionary with configuration variablesfor templated components\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqSelected Datasources\(aq, \(aqdescription\(aq: \(aqlist of Selected Datasources\(aq}], \(aqDescriptionErrors\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqDescriptive Component Errors\(aq, \(aqdescription\(aq: \(aqlist of Descriptive Component Errors\(aq}], \(aqDeviceGroups\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqDevice groups\(aq, \(aqdescription\(aq: \(aqJSON dictionary with device groups\(aq, \(aqMemorized\(aq: \(aqtrue\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqDoor\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqDoor\(aq, \(aqdescription\(aq: \(aqDoor device name\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqLinkDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to which a link will be added\(aq, \(aqdescription\(aq: \(aqlist of datasources to which a link will be added\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqMacroServer\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ], {\(aqlabel\(aq: \(aqMacroServer\(aq, \(aqdescription\(aq: \(aqMacro Server device name\(aq}], \(aqMntGrp\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aq Measurement Group\(aq, \(aqdescription\(aq: \(aq Measurement Group name\(aq}], \(aqProfileConfiguration\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqProfile Configuration\(aq, \(aqdescription\(aq: \(aqJSON dict of server configuration\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqProfileFile\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqProfile File with its Path\(aq, \(aqdescription\(aq: \(aqconfig file with its full path\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqScanDir\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan Directory\(aq, \(aqdescription\(aq: \(aqScan Directory\(aq}], \(aqScanFile\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan File(s)\(aq, \(aqdescription\(aq: \(aqScan File(s)\(aq}], \(aqScanID\(aq: [[tango._tango.CmdArgType.DevLong, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan ID\(aq, \(aqdescription\(aq: \(aqScan ID\(aq}], \(aqStepDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to be switch into step mode\(aq, \(aqdescription\(aq: \(aqlist of datasources to be switched into step mode\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqUserData\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqClient Data\(aq, \(aqdescription\(aq: \(aqJSON dictionary with User Data\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqVersion\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ], {\(aqlabel\(aq: \(aqVersion\(aq, \(aqdescription\(aq: \(aqserver version\(aq}], \(aqWriterDevice\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqWriter Device\(aq, \(aqdescription\(aq: \(aqWriter device device name\(aq}]}
+.B attr_list  =  {\(aqAppendEntry\(aq: [[tango._tango.CmdArgType.DevBoolean, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqAppend Entry\(aq, \(aqdescription\(aq: \(aqflag for entry appending\(aq}], \(aqCanFailDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to be switch into canfail mode\(aq, \(aqdescription\(aq: \(aqlist of datasources to be switched into canfail mode\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqComponents\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqSelected Components\(aq, \(aqdescription\(aq: \(aqlist of Selected Components\(aq}], \(aqConfigDevice\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqConfiguration Device\(aq, \(aqdescription\(aq: \(aqConfiguration device name\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqConfigVariables\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqConfiguration Variables\(aq, \(aqdescription\(aq: \(aqJSON dictionary with configuration variablesfor templated components\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqSelected Datasources\(aq, \(aqdescription\(aq: \(aqlist of Selected Datasources\(aq}], \(aqDescriptionErrors\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SPECTRUM, tango._tango.AttrWriteType.READ, 10000], {\(aqlabel\(aq: \(aqDescriptive Component Errors\(aq, \(aqdescription\(aq: \(aqlist of Descriptive Component Errors\(aq}], \(aqDeviceGroups\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqDevice groups\(aq, \(aqdescription\(aq: \(aqJSON dictionary with device groups\(aq, \(aqMemorized\(aq: \(aqtrue\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqDoor\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqDoor\(aq, \(aqdescription\(aq: \(aqDoor device name\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqLinkDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to which a link will be added\(aq, \(aqdescription\(aq: \(aqlist of datasources to which a link will be added\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqMacroServer\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ], {\(aqlabel\(aq: \(aqMacroServer\(aq, \(aqdescription\(aq: \(aqMacro Server device name\(aq}], \(aqMntGrp\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aq Measurement Group\(aq, \(aqdescription\(aq: \(aq Measurement Group name\(aq}], \(aqProfileConfiguration\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqProfile Configuration\(aq, \(aqdescription\(aq: \(aqJSON dict of server configuration\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqProfileFile\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqProfile File with its Path\(aq, \(aqdescription\(aq: \(aqconfig file with its full path\(aq, \(aqMemorized\(aq: \(aqtrue\(aq}], \(aqScanDir\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan Directory\(aq, \(aqdescription\(aq: \(aqScan Directory\(aq}], \(aqScanFile\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan File(s)\(aq, \(aqdescription\(aq: \(aqScan File(s)\(aq}], \(aqScanID\(aq: [[tango._tango.CmdArgType.DevLong, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqScan ID\(aq, \(aqdescription\(aq: \(aqScan ID\(aq}], \(aqStepDataSources\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqlist of datasources to be switch into step mode\(aq, \(aqdescription\(aq: \(aqlist of datasources to be switched into step mode\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqUserData\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqClient Data\(aq, \(aqdescription\(aq: \(aqJSON dictionary with User Data\(aq, \(aqDisplay level\(aq: tango._tango.DispLevel.EXPERT}], \(aqVersion\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ], {\(aqlabel\(aq: \(aqVersion\(aq, \(aqdescription\(aq: \(aqserver version\(aq}], \(aqWriterDevice\(aq: [[tango._tango.CmdArgType.DevString, tango._tango.AttrDataFormat.SCALAR, tango._tango.AttrWriteType.READ_WRITE], {\(aqlabel\(aq: \(aqWriter Device\(aq, \(aqdescription\(aq: \(aqWriter device device name\(aq}]}
 .UNINDENT
 .INDENT 7.0
 .TP
-.B class_property_list = {}
+.B class_property_list  =  {}
 (\fI\%dict\fP <\fI\%str\fP, [ \fI\%str\fP, \fI\%tango.CmdArgType\fP, [ \fI\%list\fP <\fI\%int\fP> ] ] > ) Class Properties
 .UNINDENT
 .INDENT 7.0
 .TP
-.B cmd_list = {\(aqAddStepDataSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required datasources\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of datasources not found in components\(aq]], \(aqAdministratorDataNames\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqadministrator data names\(aq]], \(aqAvailableComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available component names\(aq]], \(aqAvailableDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available DataSource names\(aq]], \(aqAvailableMntGrps\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available mntgrp names\(aq]], \(aqAvailableProfiles\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available selection names\(aq]], \(aqAvailableTimers\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available timers\(aq]], \(aqChannelProperties\(aq: [[tango._tango.CmdArgType.DevString, \(aqproperty type\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON dictionary with channel properties {channel:property}\(aq]], \(aqComponentClientSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of component client datasources\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON with description of component CLIENT Datasources\(aq]], \(aqComponentDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqprofile component datasources\(aq]], \(aqComponentDescription\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON component description\(aq]], \(aqComponentSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of components\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON with description of component Datasources\(aq]], \(aqCreateDataSources\(aq: [[tango._tango.CmdArgType.DevString, \(aqJSON dictionary with {\(ga\(gadsname\(ga\(ga: \(ga\(gatangosource\(ga\(ga, ...}\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqCreateDynamicComponent\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of JSON strings with datasource parameters\(aq], [tango._tango.CmdArgType.DevString, \(aqname of dynamic Component\(aq]], \(aqCreateWriterConfiguration\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required components\(aq], [tango._tango.CmdArgType.DevString, \(aqXML Settinges\(aq]], \(aqDataSourceDescription\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required datasources\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of JSON with description of CLIENT Datasources\(aq]], \(aqDeleteAllProfiles\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqDeleteProfile\(aq: [[tango._tango.CmdArgType.DevString, \(aqmntgrp name\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqExportEnvProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqFetchProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqFullDeviceNames\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON Dictionary with full device names for  all aliases \(aq]], \(aqImportEnvProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqImportMntGrp\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqIsMntGrpUpdated\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevBoolean, \(aqtrue if mntgrp changed\(aq]], \(aqLoadProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqMandatoryComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqMntGrpConfiguration\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqmntgrp configuration string\(aq]], \(aqMutedChannels\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted channels\(aq]], \(aqPoolElementNames\(aq: [[tango._tango.CmdArgType.DevString, \(aqpool list attribute name\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available pool elements\(aq]], \(aqPreselectComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqPreselectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqPreselectedDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqdatasources names\(aq]], \(aqRemoveDynamicComponent\(aq: [[tango._tango.CmdArgType.DevString, \(aqname of dynamic Component\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqResetPreselectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSaveProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqScanEnvVariables\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqenvironment data\(aq]], \(aqSelectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqSelectedDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqprofile datasources\(aq]], \(aqSetChannelProperties\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqa two element list with a property type and JSON value dictionary {channel:property}\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSetScanEnvVariables\(aq: [[tango._tango.CmdArgType.DevString, \(aqenvironment data\(aq], [tango._tango.CmdArgType.DevLong, \(aqscanID\(aq]], \(aqStoreProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSwitchProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqUpdateConfigVariables\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqUpdateMntGrp\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqconfiguration\(aq]], \(aqUpdateProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqmntgrp configuration string\(aq]], \(aqVariableComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON Dictionary with all Components for   configuration variable\(aq]]}
+.B cmd_list  =  {\(aqAddStepDataSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required datasources\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of datasources not found in components\(aq]], \(aqAdministratorDataNames\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqadministrator data names\(aq]], \(aqAvailableComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available component names\(aq]], \(aqAvailableDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available DataSource names\(aq]], \(aqAvailableMntGrps\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available mntgrp names\(aq]], \(aqAvailableProfiles\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available selection names\(aq]], \(aqAvailableTimers\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available timers\(aq]], \(aqChannelProperties\(aq: [[tango._tango.CmdArgType.DevString, \(aqproperty type\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON dictionary with channel properties {channel:property}\(aq]], \(aqComponentClientSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of component client datasources\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON with description of component CLIENT Datasources\(aq]], \(aqComponentDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqprofile component datasources\(aq]], \(aqComponentDescription\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON component description\(aq]], \(aqComponentSources\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of components\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON with description of component Datasources\(aq]], \(aqCreateDataSources\(aq: [[tango._tango.CmdArgType.DevString, \(aqJSON dictionary with {\(ga\(gadsname\(ga\(ga: \(ga\(gatangosource\(ga\(ga, ...}\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqCreateDynamicComponent\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of JSON strings with datasource parameters\(aq], [tango._tango.CmdArgType.DevString, \(aqname of dynamic Component\(aq]], \(aqCreateWriterConfiguration\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required components\(aq], [tango._tango.CmdArgType.DevString, \(aqXML Settinges\(aq]], \(aqDataSourceDescription\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqlist of required datasources\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of JSON with description of CLIENT Datasources\(aq]], \(aqDeleteAllProfiles\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqDeleteProfile\(aq: [[tango._tango.CmdArgType.DevString, \(aqmntgrp name\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqExportEnvProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqFetchProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqFullDeviceNames\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON Dictionary with full device names for  all aliases \(aq]], \(aqImportEnvProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqImportMntGrp\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqIsMntGrpUpdated\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevBoolean, \(aqtrue if mntgrp changed\(aq]], \(aqLoadProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqMandatoryComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqMntGrpConfiguration\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqmntgrp configuration string\(aq]], \(aqMutedChannels\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted channels\(aq]], \(aqPoolElementNames\(aq: [[tango._tango.CmdArgType.DevString, \(aqpool list attribute name\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of available pool elements\(aq]], \(aqPreselectComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqPreselectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqPreselectedDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqdatasources names\(aq]], \(aqRemoveDynamicComponent\(aq: [[tango._tango.CmdArgType.DevString, \(aqname of dynamic Component\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqResetPreselectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSaveProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqScanEnvVariables\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqenvironment data\(aq]], \(aqSelectedComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqcomponent names\(aq]], \(aqSelectedDataSources\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVarStringArray, \(aqprofile datasources\(aq]], \(aqSetChannelProperties\(aq: [[tango._tango.CmdArgType.DevVarStringArray, \(aqa two element list with a property type and JSON value dictionary {channel:property}\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSetScanEnvVariables\(aq: [[tango._tango.CmdArgType.DevString, \(aqenvironment data\(aq], [tango._tango.CmdArgType.DevLong, \(aqscanID\(aq]], \(aqStoreProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqSwitchProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqUpdateConfigVariables\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevVoid, \(aq\(aq]], \(aqUpdateMntGrp\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqconfiguration\(aq]], \(aqUpdateProfile\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqmntgrp configuration string\(aq]], \(aqVariableComponents\(aq: [[tango._tango.CmdArgType.DevVoid, \(aq\(aq], [tango._tango.CmdArgType.DevString, \(aqJSON Dictionary with all Components for   configuration variable\(aq]]}
 (\fI\%dict\fP <\fI\%str\fP, [[ \fI\%tango.CmdArgType\fP, \fI\%str\fP]] >)
 Command definitions
 .UNINDENT
 .INDENT 7.0
 .TP
-.B device_property_list = {\(aqAdminDataNames\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of administrator data names\(aq, []], \(aqClientRecordKeys\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of record keys for CLIENT datasources\(aq, []], \(aqDefaultCanFailDataSources\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of default datasources in the CanFail mode\(aq, []], \(aqDefaultMntGrp\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault measurement group name\(aq, [\(aqnxsmntgrp\(aq]], \(aqDefaultNeXusPath\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault NeXus path\(aq, ["/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection"]], \(aqDefaultNeXusType\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault dynamic component NeXus data type\(aq, [\(aqNX_CHAR\(aq]], \(aqDefaultPreselectedComponents\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of default preselected components\(aq, []], \(aqDefaultTimeZone\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault Time Zone\(aq, [\(aqEurope/Berlin\(aq]], \(aqDefaultUserDataPath\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault NeXus User Data path\(aq, ["/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/user_data:NXparameters"]], \(aqMasterTimer\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqset the master timer/monitor channel for older MG\(aq, [False]], \(aqMasterTimerFirst\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqthe master timer channel of MG with the index: 0\(aq, [True]], \(aqMergeProfilesToMntGrps\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqmerge profiles to available measurement groups\(aq, [False]], \(aqMutedChannelFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted channel filters\(aq, []], \(aqMutedPreScanAttrFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted attribute channel filters for PreScanSnapshot\(aq, []], \(aqNumberOfThreads\(aq: [tango._tango.CmdArgType.DevLong, \(aqmaximal number of threads\(aq, [20]], \(aqPoolBlacklist\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqblacklist of pools\(aq, []], \(aqResetInvalidDoor\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqreset Door when it is invalid\(aq, [True]], \(aqSyncSnapshot\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqpreselection merges the current ScanSnapshot\(aq, [False]], \(aqTangoSourceErrorStates\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of tango error states for tango datasources\(aq, [\(aqOFF\(aq, \(aqINIT\(aq, \(aqINSERT\(aq, \(aqCLOSE\(aq, \(aqUNKNOWN\(aq, \(aqFAULT\(aq]], \(aqTangoSourceWarningStates\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of tango warning states for tango datasources\(aq, [\(aqALARM\(aq, \(aqDISABLE\(aq]], \(aqTimerFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of timer device name filters\(aq, []], \(aqWritePoolMotorPositions\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqadd dynamic components for all pool motor positions\(aq, [False]]}
+.B device_property_list  =  {\(aqAdminDataNames\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of administrator data names\(aq, []], \(aqClientRecordKeys\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of record keys for CLIENT datasources\(aq, []], \(aqDefaultCanFailDataSources\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of default datasources in the CanFail mode\(aq, []], \(aqDefaultMntGrp\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault measurement group name\(aq, [\(aqnxsmntgrp\(aq]], \(aqDefaultNeXusPath\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault NeXus path\(aq, [\(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection\(dq]], \(aqDefaultNeXusType\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault dynamic component NeXus data type\(aq, [\(aqNX_CHAR\(aq]], \(aqDefaultPreselectedComponents\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of default preselected components\(aq, []], \(aqDefaultTimeZone\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault Time Zone\(aq, [\(aqEurope/Berlin\(aq]], \(aqDefaultUserDataPath\(aq: [tango._tango.CmdArgType.DevString, \(aqdefault NeXus User Data path\(aq, [\(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/user_data:NXparameters\(dq]], \(aqMasterTimer\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqset the master timer/monitor channel for older MG\(aq, [False]], \(aqMasterTimerFirst\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqthe master timer channel of MG with the index: 0\(aq, [True]], \(aqMergeProfilesToMntGrps\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqmerge profiles to available measurement groups\(aq, [False]], \(aqMutedChannelFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted channel filters\(aq, []], \(aqMutedPreScanAttrFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of muted attribute channel filters for PreScanSnapshot\(aq, []], \(aqNumberOfThreads\(aq: [tango._tango.CmdArgType.DevLong, \(aqmaximal number of threads\(aq, [20]], \(aqPoolBlacklist\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqblacklist of pools\(aq, []], \(aqResetInvalidDoor\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqreset Door when it is invalid\(aq, [True]], \(aqSyncSnapshot\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqpreselection merges the current ScanSnapshot\(aq, [False]], \(aqTangoSourceErrorStates\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of tango error states for tango datasources\(aq, [\(aqOFF\(aq, \(aqINIT\(aq, \(aqINSERT\(aq, \(aqCLOSE\(aq, \(aqUNKNOWN\(aq, \(aqFAULT\(aq]], \(aqTangoSourceWarningStates\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of tango warning states for tango datasources\(aq, [\(aqALARM\(aq, \(aqDISABLE\(aq]], \(aqTimerFilters\(aq: [tango._tango.CmdArgType.DevVarStringArray, \(aqlist of timer device name filters\(aq, []], \(aqWritePoolMotorPositions\(aq: [tango._tango.CmdArgType.DevBoolean, \(aqadd dynamic components for all pool motor positions\(aq, [False]]}
 (\fI\%dict\fP <\fI\%str\fP, [ \fI\%str\fP, \fI\%tango.CmdArgType\fP, [ \fI\%list\fP <\fI\%int\fP> ] ] > ) Device Properties
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.ProfileManager module
 .sp
 ProfileManager
 .INDENT 0.0
 .TP
-.B nxsrecconfig.ProfileManager.DEFAULT_RECORD_KEYS = [\(aqserialno\(aq, \(aqend_time\(aq, \(aqstart_time\(aq, \(aqpoint_nb\(aq, \(aqtimestamps\(aq, \(aqscan_title\(aq, \(aqfilename\(aq]
+.B nxsrecconfig.ProfileManager.DEFAULT_RECORD_KEYS  =  [\(aqserialno\(aq, \(aqend_time\(aq, \(aqstart_time\(aq, \(aqpoint_nb\(aq, \(aqtimestamps\(aq, \(aqscan_title\(aq, \(aqfilename\(aq]
 (\fI\%list\fP <\fI\%str\fP>) default data names
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxsrecconfig.ProfileManager.NXSTOOLS = True
+.B nxsrecconfig.ProfileManager.NXSTOOLS  =  True
 (\fI\%bool\fP) flag for nxstools installed
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.ProfileManager.ProfileManager(selector, syncsnapshot=False, writepoolmotorpositions=False)
+.B class  nxsrecconfig.ProfileManager.ProfileManager(selector, syncsnapshot=False, writepoolmotorpositions=False)
 Bases: \fI\%object\fP
 .sp
 Manages Measurement Group and Profile from Selector
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -3271,15 +3271,15 @@
 .sp
 NeXus Sardana Recorder Settings \- Release
 .SS nxsrecconfig.Selection module
 .sp
 Selection state
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Selection.Selection(*args, **kw)
+.B class  nxsrecconfig.Selection.Selection(*args, **kw)
 Bases: \fI\%dict\fP
 .sp
 Selection Dictionary which contains the following records:
 {
 “Timer”:  ‘[]’,
 “OrderedChannels”:  ‘[]’,
 “ComponentSelection”:  ‘{}’,
@@ -3431,15 +3431,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.Selector module
 .sp
 Selection state
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Selector.Selector(macroserverpools, version, defaultpath="/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection", defaulttimezone=\(aqEurope/Berlin\(aq, defaultmntgrp=\(aqnxsmntgrp\(aq)
+.B class  nxsrecconfig.Selector.Selector(macroserverpools, version, defaultpath=\(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/NXinstrument/collection\(dq, defaulttimezone=\(aqEurope/Berlin\(aq, defaultmntgrp=\(aqnxsmntgrp\(aq)
 Bases: \fI\%object\fP
 .sp
 access class to Selection dictionary and Config Device
 .sp
 constructor
 .INDENT 7.0
 .TP
@@ -3697,15 +3697,15 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.Settings module
 .sp
 NeXus Sardana Recorder Settings implementation
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Settings.Settings(server=None, numberofthreads=None, defaultnexuspath=None, defaulttimezone=None, defaultmntgrp=None, syncsnapshot=False, writepoolmotorpositions=False, defaultnexustype=None, defaultudatapath=None)
+.B class  nxsrecconfig.Settings.Settings(server=None, numberofthreads=None, defaultnexuspath=None, defaulttimezone=None, defaultmntgrp=None, syncsnapshot=False, writepoolmotorpositions=False, defaultnexustype=None, defaultudatapath=None)
 Bases: \fI\%object\fP
 .sp
 NeXus Sardana Recorder settings
 .sp
 contructor
 .INDENT 7.0
 .TP
@@ -3760,15 +3760,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property appendEntry
+.B property  appendEntry
 (\fI\%bool\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B availableComponents()
 available components
 .INDENT 7.0
@@ -3830,15 +3830,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property canfaildatasources
+.B property  canfaildatasources
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B channelProperties(ptype)
 provides channel properties of the given type
 .INDENT 7.0
@@ -3851,15 +3851,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property clientRecordKeys
+.B property  clientRecordKeys
 (\fI\%list\fP <\fI\%str\fP>) client record keys
 .UNINDENT
 .INDENT 7.0
 .TP
 .B componentClientSources(cps)
 provides description of client datasources
 .INDENT 7.0
@@ -3914,25 +3914,25 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property components
+.B property  components
 (\fI\%list\fP <\fI\%str\fP>) provides selected components
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property configDevice
+.B property  configDevice
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property configVariables
+.B property  configVariables
 (\fI\%str\fP) the json variables string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B createDataSources(datasources)
 describe datasources
 .INDENT 7.0
@@ -3988,15 +3988,15 @@
 .TP
 .B Return type
 [{“dsname”: \fI\%str\fP, “dstype”: \fI\%str\fP,                   “record”: \fI\%str\fP}, …]
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property dataSources
+.B property  dataSources
 (\fI\%list\fP <\fI\%str\fP>) provides all selected data sources
 .UNINDENT
 .INDENT 7.0
 .TP
 .B defaultCanFailDataSources
 (\fI\%list\fP <\fI\%str\fP>) default CanFail DataSources
 .UNINDENT
@@ -4013,15 +4013,15 @@
 .INDENT 7.0
 .TP
 .B defaultNeXusType
 (\fI\%str\fP) default NeXus type
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property defaultPreselectedComponents
+.B property  defaultPreselectedComponents
 (\fI\%list\fP <\fI\%str\fP>) default PreselectedComponents
 .UNINDENT
 .INDENT 7.0
 .TP
 .B defaultTimeZone
 (\fI\%str\fP) default time zone
 .UNINDENT
@@ -4043,25 +4043,25 @@
 .TP
 .B Parameters
 \fBname\fP (\fI\%str\fP) – mntgrp name
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property descriptionErrors
+.B property  descriptionErrors
 (\fI\%list\fP <\fI\%str\fP>) provides preselected components
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property deviceGroups
+.B property  deviceGroups
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property door
+.B property  door
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B exportEnvProfile()
 exports all Enviroutment Data
 .UNINDENT
@@ -4104,25 +4104,25 @@
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property linkdatasources
+.B property  linkdatasources
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B loadProfile()
 loads configuration
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property macroServer
+.B property  macroServer
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B mandatoryComponents()
 mandatory components
 .INDENT 7.0
@@ -4132,30 +4132,30 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property masterTimer
+.B property  masterTimer
 (\fI\%bool\fP) set master channels
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property masterTimerFirst
+.B property  masterTimerFirst
 (\fI\%bool\fP) master channels with the 0 index
 .UNINDENT
 .INDENT 7.0
 .TP
 .B mergeProfilesToMntGrps
 (\fI\%bool\fP) merge profiles to available measurement groups
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property mntGrp
+.B property  mntGrp
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B mntGrpConfiguration()
 provides configuration of mntgrp
 .INDENT 7.0
@@ -4183,15 +4183,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property mutedPreScanAttrFilters
+.B property  mutedPreScanAttrFilters
 (\fI\%list\fP <\fI\%str\fP>) muted prescan attribute filters
 .UNINDENT
 .INDENT 7.0
 .TP
 .B names()
 provides names of variables
 .INDENT 7.0
@@ -4206,15 +4206,15 @@
 .INDENT 7.0
 .TP
 .B numberOfThreads
 (\fI\%int\fP) number of threads
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property poolBlacklist
+.B property  poolBlacklist
 (\fI\%list\fP <\fI\%str\fP>) black list of pools
 .UNINDENT
 .INDENT 7.0
 .TP
 .B poolElementNames(listattr)
 provides names from given pool listattr
 .INDENT 7.0
@@ -4258,15 +4258,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property profileConfiguration
+.B property  profileConfiguration
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B profileFile
 (\fI\%str\fP) configuration file
 .UNINDENT
@@ -4293,15 +4293,15 @@
 .INDENT 7.0
 .TP
 .B saveProfile()
 saves configuration
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property scanDir
+.B property  scanDir
 the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B scanEnvVariables()
 gets Scan Environment Data
 .INDENT 7.0
@@ -4311,20 +4311,20 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property scanFile
+.B property  scanFile
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property scanID
+.B property  scanID
 (\fI\%int\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B selectedComponents()
 provides user selected components
 .INDENT 7.0
@@ -4364,15 +4364,15 @@
 .TP
 .B Parameters
 \fBjdata\fP (\fI\%str\fP) – JSON String with important variables
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property stepdatasources
+.B property  stepdatasources
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B storeProfile()
 saves configuration
 .UNINDENT
@@ -4389,25 +4389,25 @@
 .INDENT 7.0
 .TP
 .B syncSnapshot
 (\fI\%bool\fP) preselection merges current ScanSnapshot
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property tangoSourceErrorStates
+.B property  tangoSourceErrorStates
 (\fI\%list\fP <\fI\%str\fP>) tango source fault state
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property tangoSourceWarningStates
+.B property  tangoSourceWarningStates
 (\fI\%list\fP <\fI\%str\fP>) tango source alarm state
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property timerFilters
+.B property  timerFilters
 (\fI\%list\fP <\fI\%str\fP>) timer filters
 .UNINDENT
 .INDENT 7.0
 .TP
 .B updateConfigVariables()
 sends ConfigVariables into ConfigServer
 and updates serialno if appendEntry selected
@@ -4436,15 +4436,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property userData
+.B property  userData
 (\fI\%str\fP) the json data string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B value(name)
 provides values of the required variable
 .INDENT 7.0
@@ -4470,34 +4470,34 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property version
+.B property  version
 (\fI\%str\fP) server version
 .UNINDENT
 .INDENT 7.0
 .TP
 .B writepoolmotorpositions
 (\fI\%bool\fP) add dynamic components for all pool motor positions
 .UNINDENT
 .INDENT 7.0
 .TP
-.B property writerDevice
+.B property  writerDevice
 (\fI\%str\fP) the json data string
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.StreamSet module
 .sp
 labels to Tango Streams
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.StreamSet.StreamSet(streams)
+.B class  nxsrecconfig.StreamSet.StreamSet(streams)
 Bases: \fI\%object\fP
 .sp
 streamset constractor
 .INDENT 7.0
 .TP
 .B Parameters
 \fBstreams\fP (\fI\%StreamSet\fP or \fI\%tango.LatestDeviceImpl\fP) – tango\-like steamset class
@@ -4609,21 +4609,21 @@
 .UNINDENT
 .UNINDENT
 .SS nxsrecconfig.Utils module
 .sp
 Tango Utilities
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Utils.MSUtils
+.B class  nxsrecconfig.Utils.MSUtils
 Bases: \fI\%object\fP
 .sp
 MacroServer Utilities
 .INDENT 7.0
 .TP
-.B classmethod getEnv(var, ms)
+.B classmethod  getEnv(var, ms)
 provides environment variable value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBvar\fP (\fI\%str\fP) – variable name
@@ -4636,15 +4636,15 @@
 .TP
 .B Return type
 \fIany\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getMacroServer(db, door, find=True)
+.B classmethod  getMacroServer(db, door, find=True)
 provides macro server of given door
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBdb\fP (\fI\%tango.Database\fP) – tango database
@@ -4659,15 +4659,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod setEnv(var, value, ms)
+.B classmethod  setEnv(var, value, ms)
 sets environment variable value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBvar\fP (\fI\%str\fP) – variable name
@@ -4676,45 +4676,45 @@
 .IP \(bu 2
 \fBms\fP (\fI\%str\fP) – macroserver
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod setEnvs(varvalues, ms)
+.B classmethod  setEnvs(varvalues, ms)
 sets environment variable value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBvarvalues\fP (\fI\%dict\fP <\fI\%str\fP , \fIany\fP>) – variable value dictionary
 .IP \(bu 2
 \fBms\fP (\fI\%str\fP) – macroserver
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod usetEnv(var, ms)
+.B classmethod  usetEnv(var, ms)
 unsets environment variable
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBvar\fP (\fI\%str\fP) – variable name
 .IP \(bu 2
 \fBms\fP (\fI\%str\fP) – macroserver
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod writeEnvAttr(value, dp)
+.B classmethod  writeEnvAttr(value, dp)
 sets environment variable value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBvalue\fP (\fI\%dict\fP <\fI\%str\fP , \fIany\fP> or \fIany\fP) – variable value dictionary
@@ -4722,33 +4722,33 @@
 \fBdp\fP (\fI\%str\fP) – macroserver
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B exception nxsrecconfig.Utils.OldTangoError
+.B exception  nxsrecconfig.Utils.OldTangoError
 Bases: \fI\%Exception\fP
 .sp
 Old Tango version Exception class
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxsrecconfig.Utils.PYTG_BUG_213 = False
+.B nxsrecconfig.Utils.PYTG_BUG_213  =  False
 (\fI\%bool\fP) tango bug #213 flag related to EncodedAttributes in python3
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Utils.PoolUtils
+.B class  nxsrecconfig.Utils.PoolUtils
 Bases: \fI\%object\fP
 .sp
 Pool Utilities
 .INDENT 7.0
 .TP
-.B classmethod filterNames(pools, filters=None, lst=None)
+.B classmethod  filterNames(pools, filters=None, lst=None)
 provides channels of given pools
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4761,15 +4761,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod filterOutTango(lst, filters=None)
+.B classmethod  filterOutTango(lst, filters=None)
 provides channels of given pools
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBlst\fP (\fI\%list\fP <\fI\%str\fP or (\fI\%str\fP, \fI\%str\fP)>) – list of strings to filter out
@@ -4782,15 +4782,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getAliases(pools, names=None)
+.B classmethod  getAliases(pools, names=None)
 find aliases from fullnames
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4803,15 +4803,15 @@
 .TP
 .B Return type
 \fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getChannelSources(pools, devices)
+.B classmethod  getChannelSources(pools, devices)
 provides channel sources
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4824,15 +4824,15 @@
 .TP
 .B Return type
 \fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getDeviceControllers(pools, devices=None)
+.B classmethod  getDeviceControllers(pools, devices=None)
 provides device controller full names
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4845,15 +4845,15 @@
 .TP
 .B Return type
 \fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getElementNames(pools, listattr, typefilter=None)
+.B classmethod  getElementNames(pools, listattr, typefilter=None)
 provides experimental Channels
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4868,15 +4868,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getFullDeviceNames(pools, names=None)
+.B classmethod  getFullDeviceNames(pools, names=None)
 find device names from aliases
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4889,15 +4889,15 @@
 .TP
 .B Return type
 \fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getMntGrpName(pools, alias)
+.B classmethod  getMntGrpName(pools, alias)
 find measurement group name from alias
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4910,15 +4910,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getMotorPositionAttributes(pools)
+.B classmethod  getMotorPositionAttributes(pools)
 find motor names
 .INDENT 7.0
 .TP
 .B Parameters
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
 .TP
 .B Returns
@@ -4932,15 +4932,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP,:obj:\fIstr\fP, \fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getSource(name)
+.B classmethod  getSource(name)
 provides datasource from pool device
 .INDENT 7.0
 .TP
 .B Parameters
 \fBname\fP (\fI\%str\fP) – pool device name
 .TP
 .B Returns
@@ -4948,15 +4948,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getTimers(pools, filters=None)
+.B classmethod  getTimers(pools, filters=None)
 provides tiemrs of given pools
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpools\fP (\fI\%list\fP <\fI\%tango.DeviceProxy\fP>) – list of pool devices
@@ -4970,21 +4970,21 @@
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Utils.TangoUtils
+.B class  nxsrecconfig.Utils.TangoUtils
 Bases: \fI\%object\fP
 .sp
 Tango Utilities
 .INDENT 7.0
 .TP
-.B classmethod command(server, command, *var)
+.B classmethod  command(server, command, *var)
 executes command on server on python package
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBserver\fP (\fI\%tango.DeviceProxy\fP              or \fI\%nxsconfigserver.XMLConfigurator.XMLConfigurator\fP) – tango server name or package name
@@ -4999,15 +4999,15 @@
 .TP
 .B Return type
 \fIany\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getDeviceName(db, cname)
+.B classmethod  getDeviceName(db, cname)
 finds device of give class
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBdb\fP (\fI\%tango.DeviceProxy\fP) – tango database
@@ -5020,15 +5020,15 @@
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getFullAttrName(source, fqdn=False)
+.B classmethod  getFullAttrName(source, fqdn=False)
 provides tango device full name with host and port
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBsource\fP (\fI\%str\fP) – string with device name and its attribute
@@ -5041,15 +5041,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getProxies(names)
+.B classmethod  getProxies(names)
 provides proxies of given device names
 .INDENT 7.0
 .TP
 .B Parameters
 \fBnames\fP (\fI\%list\fP <\fI\%str\fP>) – given device names
 .TP
 .B Returns
@@ -5057,15 +5057,15 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%tango.DeviceProxy\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getShapeTypeUnit(source)
+.B classmethod  getShapeTypeUnit(source)
 retrives shape type units for attribure
 .INDENT 7.0
 .TP
 .B Parameters
 \fBsource\fP (\fI\%str\fP) – string with device name and its attribute
 .TP
 .B Returns
@@ -5073,15 +5073,15 @@
 .TP
 .B Return type
 (\fI\%list\fP <\fI\%int\fP>, \fI\%str\fP, \fI\%str\fP)
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod openProxy(device, counter=1000)
+.B classmethod  openProxy(device, counter=1000)
 opens device proxy of the given device
 .INDENT 7.0
 .TP
 .B Parameters
 \fBdevice\fP (\fI\%str\fP) – device name
 .TP
 .B Returns
@@ -5089,21 +5089,21 @@
 .TP
 .B Return type
 \fI\%tango.DeviceProxy\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B tTnp = {tango._tango.CmdArgType.DevBoolean: \(aqbool\(aq, tango._tango.CmdArgType.DevShort: \(aqint16\(aq, tango._tango.CmdArgType.DevLong: \(aqint32\(aq, tango._tango.CmdArgType.DevFloat: \(aqfloat32\(aq, tango._tango.CmdArgType.DevDouble: \(aqfloat64\(aq, tango._tango.CmdArgType.DevUShort: \(aquint16\(aq, tango._tango.CmdArgType.DevULong: \(aquint32\(aq, tango._tango.CmdArgType.DevString: \(aqstring\(aq, tango._tango.CmdArgType.DevUChar: \(aquint8\(aq, tango._tango.CmdArgType.DevLong64: \(aqint64\(aq, tango._tango.CmdArgType.DevULong64: \(aquint64\(aq, tango._tango.CmdArgType.DevEncoded: \(aqencoded\(aq}
+.B tTnp  =  {tango._tango.CmdArgType.DevBoolean: \(aqbool\(aq, tango._tango.CmdArgType.DevShort: \(aqint16\(aq, tango._tango.CmdArgType.DevLong: \(aqint32\(aq, tango._tango.CmdArgType.DevFloat: \(aqfloat32\(aq, tango._tango.CmdArgType.DevDouble: \(aqfloat64\(aq, tango._tango.CmdArgType.DevUShort: \(aquint16\(aq, tango._tango.CmdArgType.DevULong: \(aquint32\(aq, tango._tango.CmdArgType.DevString: \(aqstring\(aq, tango._tango.CmdArgType.DevUChar: \(aquint8\(aq, tango._tango.CmdArgType.DevLong64: \(aqint64\(aq, tango._tango.CmdArgType.DevULong64: \(aquint64\(aq, tango._tango.CmdArgType.DevEncoded: \(aqencoded\(aq}
 (\fI\%dict\fP <\fI\%tango.CmdArgType\fP, \fI\%str\fP>)
 map of Tango:Numpy types
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod wait(proxy, counter=100, state=\(aqRUNNING\(aq)
+.B classmethod  wait(proxy, counter=100, state=\(aqRUNNING\(aq)
 waits for device proxy not running
 .INDENT 7.0
 .TP
 .B Parameters
 \fBproxy\fP (\fI\%tango.DeviceProxy\fP) – device proxy
 .TP
 .B Returns
@@ -5112,21 +5112,21 @@
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxsrecconfig.Utils.Utils
+.B class  nxsrecconfig.Utils.Utils
 Bases: \fI\%object\fP
 .sp
 Miscellaneous Utilities
 .INDENT 7.0
 .TP
-.B classmethod compareDict(dct, dct2)
+.B classmethod  compareDict(dct, dct2)
 copares two dictionaries
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBdct\fP (\fI\%dict\fP) – first dictinary
@@ -5139,15 +5139,15 @@
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getRecord(node)
+.B classmethod  getRecord(node)
 provides datasource record from xml dom node
 .INDENT 7.0
 .TP
 .B Parameters
 \fBnode\fP (\fBlxml.etree.Element\fP) – xml DOM node
 .TP
 .B Returns
@@ -5155,34 +5155,34 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getText(node)
+.B classmethod  getText(node)
 collects text from text child nodes
 .INDENT 7.0
 .TP
 .B Parameters
 \fBnode\fP (\fI\%xml.etree.ElementTree.Element\fP) – parent node
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod pickleloads(bytestr)
+.B classmethod  pickleloads(bytestr)
 loads pickle byte string
 :param bytestr: byte string to convert
 :type bytesstr: \fI\%bytes\fP
 :returns: loaded bytestring
 :rtype: \fI\%any\fP
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod stringToDictJson(string, toBool=False)
+.B classmethod  stringToDictJson(string, toBool=False)
 converts string to json dictionary
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBstring\fP (\fI\%str\fP) – string with list of item or json dictionary
@@ -5195,15 +5195,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod stringToListJson(string)
+.B classmethod  stringToListJson(string)
 converts string to json list
 .INDENT 7.0
 .TP
 .B Parameters
 \fBstring\fP (\fI\%str\fP) – with list of item or json list
 .TP
 .B Returns
@@ -5211,15 +5211,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod toString(obj)
+.B classmethod  toString(obj)
 converts list/dict/object of unicode/string to string object
 .INDENT 7.0
 .TP
 .B Parameters
 \fBobj\fP (\fIany\fP) – given unicode/string object
 .TP
 .B Returns
@@ -5227,15 +5227,15 @@
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod tostr(text)
+.B classmethod  tostr(text)
 convert bytestr or unicode to python str
 :param text: text to convert
 :type text: \fI\%bytes\fP or \fBunicode\fP or \fI\%str\fP
 :returns: converted text
 :rtype: \fI\%str\fP
 .UNINDENT
 .UNINDENT
@@ -5250,19 +5250,19 @@
 .TP
 .B Parameters
 \fBargv\fP (\fI\%list\fP <\fI\%str\fP>) – command\-line arguments
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-genindex
+\fI\%Index\fP
 .IP \(bu 2
-modindex
+\fI\%Module Index\fP
 .IP \(bu 2
-search
+\fI\%Search Page\fP
 .UNINDENT
 .SH AUTHOR
 Author
 .SH COPYRIGHT
 2012-2017 DESY, Jan Kotanski <jkotan@mail.desy.de>
 
 GNU GENERAL PUBLIC LICENSE, version 3
```

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.40.0/nxsrecconfig/CheckerThread.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Converter.py` & `nxsrecselector-3.40.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Describer.py` & `nxsrecselector-3.40.0/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.40.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.40.0/nxsrecconfig/MacroServerPools.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.40.0/nxsrecconfig/NXSConfig.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.40.0/nxsrecconfig/ProfileManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,16 @@
                                         fdss.add(ds)
 
                 if fdss:
                     if not (cpdss - fdss):
                         if cp in jpcps.keys() and jpcps[cp] is False:
                             jpcps[cp] = None
                         for ds in fdss:
-                            snpds[ds] = True
+                            if ds not in poolds:
+                                snpds[ds] = True
         for ds, val in snpds.items():
             if val is not True:
                 jpdss[ds] = None
         pcps = json.dumps(jpcps)
         pdss = json.dumps(jpdss)
         if pcps != self.__selector["ComponentPreselection"]:
             self.__selector["ComponentPreselection"] = pcps
```

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Release.py` & `nxsrecselector-3.40.0/nxsrecconfig/Release.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.39.0"
+__version__ = "3.40.0"
```

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Selection.py` & `nxsrecselector-3.40.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Selector.py` & `nxsrecselector-3.40.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Settings.py` & `nxsrecselector-3.40.0/nxsrecconfig/Settings.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.40.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/Utils.py` & `nxsrecselector-3.40.0/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecconfig/__init__.py` & `nxsrecselector-3.40.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.40.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.39.0/setup.py` & `nxsrecselector-3.40.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,22 +104,22 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     install_requires=install_requires,
     scripts=['NXSRecSelector'],
     cmdclass={
         # 'test': TestCommand,
         'build_sphinx': BuildDoc
     },
```

