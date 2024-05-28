# Comparing `tmp/anemone_daisy_maker-1.58.tar.gz` & `tmp/anemone_daisy_maker-1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.58.tar", last modified: Thu May 16 06:08:52 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.59.tar", last modified: Tue May 28 05:17:44 2024, max compression
```

## Comparing `anemone_daisy_maker-1.58.tar` & `anemone_daisy_maker-1.59.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-16 06:08:52.610046 anemone_daisy_maker-1.58/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-16 06:08:45.000000 anemone_daisy_maker-1.58/LICENSE
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6926 2024-05-16 06:08:52.606046 anemone_daisy_maker-1.58/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-16 06:08:52.606046 anemone_daisy_maker-1.58/anemone/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    76621 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone/__main__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-16 06:08:52.606046 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6926 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       23 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-16 06:08:52.610046 anemone_daisy_maker-1.58/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7093 2024-05-16 06:08:52.000000 anemone_daisy_maker-1.58/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-28 05:17:37.000000 anemone_daisy_maker-1.59/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7050 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    77301 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7050 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       23 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7217 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/setup.py
```

### Comparing `anemone_daisy_maker-1.58/LICENSE` & `anemone_daisy_maker-1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.58/PKG-INFO` & `anemone_daisy_maker-1.59/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.58
+Version: 1.59
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
+3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

### Comparing `anemone_daisy_maker-1.58/anemone/__init__.py` & `anemone_daisy_maker-1.59/anemone/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Anemone 1.58 (http://ssb22.user.srcf.net/anemone)
+Anemone 1.59 (http://ssb22.user.srcf.net/anemone)
 (c) 2023-24 Silas S. Brown.  License: Apache 2
 
 To use this module, either run it from the command
 line, or import it and use the anemone() function.
 """
 
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -298,21 +298,20 @@
         else: error(f"Format of '{fOrig}' has not been recognised")
   def check(self) -> None:
     "Checks we've got everything"
     # You may omit calling this if you're creating
     # a temporary Run just to call something like
     # check_for_JSON_transcript and get its HTML
     R = self
-    if not R.audioData: error("Creating DAISY files without audio is not yet implemented")
-    if R.htmlData and not R.jsonData: error("Full text without time markers is not yet implemented")
+    if R.htmlData and R.audioData and not R.jsonData: error("Full text and audio without time markers is not yet implemented")
     if R.jsonData and not R.htmlData: error("Time markers without full text is not implemented")
     if R.htmlData and R.textData: error("Combining full text with title-only text files is not yet implemented.  Please specify full text for everything or just titles for everything, not both.")
     if R.jsonData and not len(R.audioData)==len(R.jsonData): error(f"If JSON marker files are specified, there must be exactly one JSON file for each recording file.  We got f{len(R.jsonData)} JSON files and f{len(R.audioData)} recording files.")
     if R.textData and not len(R.audioData)==len(R.textData): error(f"If text files are specified, there must be exactly one text file for each recording file.  We got f{len(R.textData)} text files and f{len(R.audioData)} recording files.")
-    if R.htmlData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
+    if R.htmlData and R.audioData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents with audio are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
     if not R.outputFile:
         R.outputFile=f"output_daisy{os.extsep}zip"
     if not R.title: R.title=R.outputFile.replace(f"{os.extsep}zip","").replace("_daisy","")
   def warning(self,warningText) -> None:
     if self.warnings_are_errors:error(warningText)
     self.warnings.append(warningText)
     sys.stderr.write(f"WARNING: {warningText}\n")
@@ -337,21 +336,34 @@
         R.htmlData.append(' '.join(
             f'<span {R.marker_attribute}="{i}">{c}</span>' for i,c in enumerate(bodyList) if c))
         R.jsonData[-1]={"markers":[
             {"id":f"{i}","time":t}
             for i,t in enumerate(
                     s["startTime"] for s in R.jsonData[-1]["segments"])
             if bodyList[i]]}
+  def make_null_jsonData(self) -> None:
+    """Generate no-audio JSON for internal use
+    when making text-only DAISY files from HTML.
+    In this case we assume any element with any
+    marker-attribute should be extracted."""
+    self.jsonData = [
+        {'markers':
+         [{'id':i[self.marker_attribute], 'time':0}
+          for i in BeautifulSoup(h,'html.parser')
+          .find_all(**{self.marker_attribute:
+                       True})]}
+        for h in self.htmlData]
   def get_texts(self) -> list:
     """Gets the text markup required for the run,
     extracting it from HTML (guided by JSON IDs)
     if we need to do that."""
     R = self
     if R.textData: return R.textData # section titles only, from text files
     elif not R.htmlData: return R.filenameTitles # section titles only, from sound filenames
+    elif not R.jsonData: self.make_null_jsonData()
     recordingTexts = []
     for h,j in zip(R.htmlData,R.jsonData):
         markers = j['markers']
         want_pids = [jsonAttr(m,"id") for m in markers]
         extractor = PidsExtractor(R,want_pids)
         extractor.handle_soup(
             BeautifulSoup(h, 'html.parser'))
@@ -371,19 +383,19 @@
   def write_all(self,recordingTexts) -> None:
     """Writes the DAISY zip and everything in it.
     Each item of recordingTexts is either 1 text
     for section title of whole recording, or a
     TextsAndTimesWithPages i.e. ([TagAndText,time,
     TagAndText,time,TagAndText],[PageInfo,...])"""
     R = self
-    assert len(R.audioData) == len(recordingTexts)
+    assert len(R.audioData) == len(recordingTexts) or not R.audioData
     headings = R.getHeadings(recordingTexts)
     if R.dry_run: return sys.stderr.write(f"Dry run: {len(R.warnings) if R.warnings else 'no'} warning{'' if len(R.warnings)==1 else 's'} for {R.outputFile}\n")
-    merge0lenSpans(recordingTexts,headings)
-    if R.mp3_recode or any(
+    if R.audioData: merge0lenSpans(recordingTexts,headings)
+    if R.mp3_recode and R.audioData or any(
             'audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData): # parallelise lame if possible
         if not __name__=="__main__":
             sys.stderr.write(f"Making {R.outputFile}...\n"),sys.stderr.flush() # especially if repeatedly called, print which outputFile we're working on BEFORE the mp3s also
         executor = ThreadPoolExecutor(
             max_workers=cpu_count())
         recordingTasks=[executor.submit(
             (recodeMP3 if
@@ -440,20 +452,21 @@
     # (it's iOS users that need the above, apparently.  Can't DAISY have a non-ZIP extension so Apple systems don't automatically unpack it?  but we do need to manually unpack if writing to a CD-ROM for old devices.  Can't Apple look at some kind of embedded "don't auto-unpack this zip" request?)
     secsSoFar = 0
     durations = [] ; curP = 1
     for recNo in range(1,len(recordingTexts)+1):
         rTxt = recordingTexts[recNo-1]
         secsThisRecording = mutagen.File(
             BytesIO(R.audioData[recNo-1])
-        ).info.length
+        ).info.length if R.audioData else 0
         if secsThisRecording > 3600: R.warning(f"Recording {recNo} is long enough to cause ~{secsThisRecording*.0001:.1f}sec synchronisation error on some readers") # seems lame v3.100 can result in timestamps being effectively multiplied by ~1.0001 on some players but not all, causing slight de-sync on 1h+ recordings (bladeenc may avoid this but be lower quality overall; better to keep the recordings shorter if possible)
         durations.append(secsThisRecording)
         if recordingTasks is not None:
             sys.stderr.write(f"Adding {recNo:04d}.mp3..."),sys.stderr.flush()
-        writestr(f"{recNo:04d}.mp3",
+        if R.audioData:
+            writestr(f"{recNo:04d}.mp3",
                  R.audioData[recNo-1]
                  if recordingTasks is None
                  else recordingTasks[recNo-1].result())
         if recordingTasks is not None:
             sys.stderr.write(" done\n")
         writestr(f'{recNo:04d}.smil',D(
             R.section_smil(recNo,secsSoFar,
@@ -658,17 +671,24 @@
     <meta name="ncc:charset" content="utf-8" />
     <meta name="ncc:pageFront" content="0" />
     <meta name="ncc:maxPageNormal" content="{maxPageNo}" />
     <meta name="ncc:pageNormal" content="{numPages}" />
     <meta name="ncc:pageSpecial" content="0" />
     <meta name="ncc:tocItems" content="{len(headingsR)+sum(len(PNs) for PNs in pageNos)}" />
     <meta name="ncc:totalTime" content="{hmsTime(totalSecs)}" />
-    <meta name="ncc:multimediaType" content="{"audioFullText" if hasFullText else "audioNcc"}" />
-    <meta name="{'dtb' if R.daisy3 else 'ncc'}:depth" content="{max(int(h.hTag[1:]) for h in headingsR if h.hTag.startswith('h'))+(1 if any(h.hTag=='div' for h in headingsR) else 0)}" />
-    <meta name="ncc:files" content="{2+len(headings)*(3 if hasFullText else 2)+len(R.imageFiles)}" />
+    <meta name="ncc:multimediaType" content="{
+    "textNcc" if not R.audioData else
+    "audioFullText" if hasFullText else "audioNcc" }" />
+    <meta name="{'dtb' if R.daisy3 else 'ncc'
+    }:depth" content="{max(int(h.hTag[1:])
+    for h in headingsR if h.hTag.startswith('h'))
+    +(1 if any(h.hTag=='div' for h in headingsR)
+    else 0)}" />
+    <meta name="ncc:files" content="{2+
+    len(headings)*(3 if hasFullText and R.audioData else 2)+len(R.imageFiles)}" />
   </head>
   {f'<docTitle><text>{R.title}</text></docTitle>'
     if R.daisy3 else ''}
   {f'<docAuthor><text>{R.creator}</text></docAuthor>'
     if R.daisy3 else ''}
   <{'navMap id="navMap"' if R.daisy3 else 'body'}>"""+''.join((f"""
     <navPoint id="s{s+1}" class="{t.hTag}" playOrder="{s+1}">
```

### Comparing `anemone_daisy_maker-1.58/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: anemone-daisy-maker
-Version: 1.58
+Version: 1.59
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
+3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

### Comparing `anemone_daisy_maker-1.58/setup.py` & `anemone_daisy_maker-1.59/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.58',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.59',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
+3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

