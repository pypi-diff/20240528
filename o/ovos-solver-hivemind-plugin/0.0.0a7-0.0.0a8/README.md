# Comparing `tmp/ovos_solver_hivemind_plugin-0.0.0a7-py3-none-any.whl.zip` & `tmp/ovos_solver_hivemind_plugin-0.0.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4586 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3292 b- defN 24-May-21 18:00 ovos_hivemind_solver/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-May-21 18:00 ovos_hivemind_solver/version.py
--rw-r--r--  2.0 unx     2539 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/zip-safe
--rw-rw-r--  2.0 unx      787 b- defN 24-May-21 18:01 ovos_solver_hivemind_plugin-0.0.0a7.dist-info/RECORD
-8 files, 6995 bytes uncompressed, 3166 bytes compressed:  54.7%
+Zip file size: 4292 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2351 b- defN 24-May-28 06:12 ovos_hivemind_solver/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-28 06:13 ovos_hivemind_solver/version.py
+-rw-r--r--  2.0 unx     2539 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      787 b- defN 24-May-28 06:13 ovos_solver_hivemind_plugin-0.0.0a8.dist-info/RECORD
+8 files, 6054 bytes uncompressed, 2872 bytes compressed:  52.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_hivemind_solver/__init__.py
 Comment: 
 
 Filename: ovos_hivemind_solver/version.py
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/METADATA
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/METADATA
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/WHEEL
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/entry_points.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/top_level.txt
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/zip-safe
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_solver_hivemind_plugin-0.0.0a7.dist-info/RECORD
+Filename: ovos_solver_hivemind_plugin-0.0.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_hivemind_solver/__init__.py

```diff
@@ -24,36 +24,17 @@
 
     def connect(self):
         """assume identity set beforehand, eg via `hivemind-client set-identity`
         """
         self.hm = HiveMessageBusClient(useragent="ovos-hivemind-solver")
         self.hm.run_in_thread()
         self.hm.on_mycroft("speak", self._receive_answer)
-        # NOTE: this message not yet introduced in ovos-core
         self.hm.on_mycroft("ovos.utterance.handled", self._end_of_response)
 
-        ##############
-        # HACK - waiting for https://github.com/OpenVoiceOS/ovos-core/pull/478
-        # TODO - new bus message in ovos-core
-        #  to unambiguosly identify end of utterance parsing
-        #  currently these are 4 possible outcomes for any request
-        #  does not account for OCP pipeline requests
-        self.hm.on_mycroft("ovos.utterance.cancelled",
-                           self._end_of_response)
-        self.hm.on_mycroft("complete_intent_failure",
-                           self._end_of_response)
-        self.hm.on_mycroft("mycroft.skill.handler.complete",
-                           self._end_of_response)
-        self.hm.on_mycroft( "skill.converse.response",
-                           self._end_of_response)
-
     def _end_of_response(self, message):
-        if message.type == "skill.converse.response":
-            if not message.data.get("result"):
-                return
         self._response.set()
 
     def _receive_answer(self, message):
         utt = message.data["utterance"]
         self._responses.append(utt)
 
     # abstract Solver methods
```

## ovos_hivemind_solver/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 7
+VERSION_ALPHA = 8
 # END_VERSION_BLOCK
```

## Comparing `ovos_solver_hivemind_plugin-0.0.0a7.dist-info/METADATA` & `ovos_solver_hivemind_plugin-0.0.0a8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-hivemind-plugin
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: A question solver plugin for OVOS
 Home-page: https://github.com/JarbasHiveMind/ovos-solver-hivemind-plugin
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Keywords: OVOS openvoiceos plugin utterance fallback query
 Platform: UNKNOWN
```

