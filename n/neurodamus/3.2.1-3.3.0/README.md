# Comparing `tmp/neurodamus-3.2.1.tar.gz` & `tmp/neurodamus-3.3.0.tar.gz`

## Comparing `neurodamus-3.2.1.tar` & `neurodamus-3.3.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/__init__.py
--rw-r--r--   0        0        0    38362 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/cell_distributor.py
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/commands.py
--rw-r--r--   0        0        0    32924 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/connection.py
--rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/connection_manager.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/gap_junction.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/hocify.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/lfp_manager.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/metype.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/modification_manager.py
--rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/morphio_wrapper.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/neuromodulation_manager.py
--rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/ngv.py
--rw-r--r--   0        0        0    81050 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/node.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/replay.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/report.py
--rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/stimulus_manager.py
--rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/target_manager.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_engine.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_mpi.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_neurodamus.py
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_neuron.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_shmutils.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_utils.py
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/cell.py
--rw-r--r--   0        0        0    44943 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/configuration.py
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/coreneuron_configuration.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/mechanisms.py
--rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/nodeset.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/random.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/stimuli.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/synapses.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/init.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/Cell.hoc
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/ConnectionUtils.hoc
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/Map.hoc
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/MorphIO.hoc
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/RNGSettings.hoc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/defvar.hoc
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/fileUtils.hoc
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/neurodamus.hoc
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/ALU.mod
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/CoreNEURONArtificialCell.mod
--rw-r--r--   0        0        0    45115 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/HDF5reader.mod
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/SonataReportHelper.mod
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/SonataReports.mod
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/VecStim.mod
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/coreneuron_modlist.txt
--rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/netstim_inhpoisson.mod
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/__init__.py
--rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/cell_readers.py
--rw-r--r--   0        0        0    19452 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/sonata_config.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/synapse_reader.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/cli.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/compat.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/logging.py
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/memory.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/multimap.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/progressbar.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/pyutils.py
--rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/timeit.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 neurodamus-3.2.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 neurodamus-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 neurodamus-3.2.1/README.rst
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neurodamus-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    18296 2020-02-02 00:00:00.000000 neurodamus-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/__init__.py
+-rw-r--r--   0        0        0    38438 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/cell_distributor.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/commands.py
+-rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/connection.py
+-rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/connection_manager.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/gap_junction.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/hocify.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/lfp_manager.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/metype.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/modification_manager.py
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/morphio_wrapper.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/neuromodulation_manager.py
+-rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/ngv.py
+-rw-r--r--   0        0        0    80490 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/node.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/replay.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/report.py
+-rw-r--r--   0        0        0    29071 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/stimulus_manager.py
+-rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/target_manager.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_engine.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_mpi.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_neurodamus.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_neuron.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_shmutils.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/_utils.py
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/cell.py
+-rw-r--r--   0        0        0    44848 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/configuration.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/coreneuron_configuration.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/mechanisms.py
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/nodeset.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/random.py
+-rw-r--r--   0        0        0    20680 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/stimuli.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/core/synapses.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/init.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/Cell.hoc
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/ConnectionUtils.hoc
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/Map.hoc
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/MorphIO.hoc
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/RNGSettings.hoc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/defvar.hoc
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/fileUtils.hoc
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/hoc/neurodamus.hoc
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/ALU.mod
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/CoreNEURONArtificialCell.mod
+-rw-r--r--   0        0        0    45115 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/HDF5reader.mod
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/SonataReportHelper.mod
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/SonataReports.mod
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/VecStim.mod
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/coreneuron_modlist.txt
+-rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/data/mod/netstim_inhpoisson.mod
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/io/__init__.py
+-rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/io/cell_readers.py
+-rw-r--r--   0        0        0    19452 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/io/sonata_config.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/io/synapse_reader.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/__init__.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/cli.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/compat.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/logging.py
+-rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/memory.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/multimap.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/progressbar.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/pyutils.py
+-rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 neurodamus-3.3.0/neurodamus/utils/timeit.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 neurodamus-3.3.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 neurodamus-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 neurodamus-3.3.0/README.rst
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neurodamus-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18296 2020-02-02 00:00:00.000000 neurodamus-3.3.0/PKG-INFO
```

### Comparing `neurodamus-3.2.1/neurodamus/__init__.py` & `neurodamus-3.3.0/neurodamus/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/cell_distributor.py` & `neurodamus-3.3.0/neurodamus/cell_distributor.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,18 +414,19 @@
         """Setup recording of spike events (crossing of threshold) for cells on this node
         """
         if not self._local_nodes:
             return
         spikevec, idvec = append_spike_vecs or (Nd.Vector(), Nd.Vector())
         if gids is None:
             gids = self._local_nodes.final_gids()
+            gid_offset = self._local_nodes.offset
 
         for gid in gids:
             # only want to collect spikes of cell pieces with the soma (i.e. the real gid)
-            if not self._binfo or self._binfo.thishost_gid(gid) == gid:
+            if not self._binfo or self._binfo.thishost_gid(gid - gid_offset) + gid_offset == gid:
                 self._pc.spike_record(gid, spikevec, idvec)
         return spikevec, idvec
 
     def register_connection_manager(self, conn_manager: ConnectionManagerBase):
         src_population = conn_manager.src_cell_manager.population_name
         if src_population in self._conn_managers_per_src_pop:
             logging.warning("Skip registering %s as a second pop source", conn_manager)
```

### Comparing `neurodamus-3.2.1/neurodamus/commands.py` & `neurodamus-3.3.0/neurodamus/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os
 import sys
 import time
 from docopt import docopt
 from os.path import abspath
 from pathlib import Path
 
+from neurodamus.utils.timeit import TimerManager
+
 from . import Neurodamus
 from .core import MPI, OtherRankError
 from .core.configuration import ConfigurationError, LogLevel, EXCEPTION_NODE_FILENAME
 from .hocify import Hocify, process_file as hocify_process_file
 from .utils.pyutils import docopt_sanitize
 
 
@@ -77,14 +79,15 @@
     # Some previous executions may have left a bad exception node file
     # This is done now so it's a very early stage and we know the mpi rank
     if MPI.rank == 0 and os.path.exists(EXCEPTION_NODE_FILENAME):
         os.remove(EXCEPTION_NODE_FILENAME)
 
     try:
         Neurodamus(config_file, True, logging_level=log_level, **options).run()
+        TimerManager.timeit_show_stats()
     except ConfigurationError as e:  # Common, only show error in Rank 0
         if MPI._rank == 0:           # Use _rank so that we avoid init
             logging.error(str(e))
         return 1
     except OtherRankError:
         return 1  # no need for _mpi_abort, error is being handled by all ranks
     except Exception:
```

### Comparing `neurodamus-3.2.1/neurodamus/connection.py` & `neurodamus-3.3.0/neurodamus/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -710,44 +710,20 @@
         netcon = Nd.NetCon(ips, syn_obj, sec=sec)
         netcon.delay = 0.1
         netcon.weight[0] = syn_params.weight * conn.weight_factor
         conn.netcon_set_type(netcon, syn_obj, NetConType.NC_SPONTMINI)
         self._store(ips, netcon)
 
         src_pop_id, dst_pop_id = conn.population_id
-        rng_mode = self._rng_info.getRNGMode()
         rng_seed = self._rng_info.getMinisSeed()
         tgid_seed = conn.tgid + 250
 
-        if rng_mode == self._rng_info.RANDOM123:
-            seed2 = (src_pop_id * 65536 + dst_pop_id + rng_seed)
-            ips.setRNGs(syn_obj.synapseID + 200, tgid_seed, seed2 + 300,
-                        syn_obj.synapseID + 200, tgid_seed, seed2 + 350)
-        else:
-            seed2 = src_pop_id * 16777216
-            exprng = Nd.Random()
-            if rng_mode == self._rng_info.COMPATIBILITY:
-                exprng.MCellRan4(syn_obj.synapseID * 100000 + 200,
-                                 tgid_seed + base_seed + rng_seed)
-            else:  # if ( rngIndo.getRNGMode()== rng_info.UPMCELLRAN4 ):
-                exprng.MCellRan4(syn_obj.synapseID * 1000 + 200,
-                                 seed2 + tgid_seed + base_seed + rng_seed)
-
-            exprng.negexp(1)
-            uniformrng = Nd.Random()
-            if rng_mode == self._rng_info.COMPATIBILITY:
-                uniformrng.MCellRan4(syn_obj.synapseID * 100000 + 300,
-                                     tgid_seed + base_seed + rng_seed)
-            else:  # if ( rngIndo.getRNGMode()== rng_info.UPMCELLRAN4 ):
-                uniformrng.MCellRan4(syn_obj.synapseID * 1000 + 300,
-                                     seed2 + tgid_seed + base_seed + rng_seed)
-
-            uniformrng.uniform(0.0, 1.0)
-            ips.setRNGs(exprng, uniformrng)
-            self._keep_alive += (exprng, uniformrng)
+        seed2 = (src_pop_id * 65536 + dst_pop_id + rng_seed)
+        ips.setRNGs(syn_obj.synapseID + 200, tgid_seed, seed2 + 300,
+                    syn_obj.synapseID + 200, tgid_seed, seed2 + 350)
 
     def __bool__(self):
         """object is considered False in case rate is not positive"""
         return bool(self.get_rate())
 
     def __del__(self):
         for ips in self.netstims:
```

### Comparing `neurodamus-3.2.1/neurodamus/connection_manager.py` & `neurodamus-3.3.0/neurodamus/connection_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/gap_junction.py` & `neurodamus-3.3.0/neurodamus/gap_junction.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/hocify.py` & `neurodamus-3.3.0/neurodamus/hocify.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/lfp_manager.py` & `neurodamus-3.3.0/neurodamus/lfp_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/metype.py` & `neurodamus-3.3.0/neurodamus/metype.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/modification_manager.py` & `neurodamus-3.3.0/neurodamus/modification_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/morphio_wrapper.py` & `neurodamus-3.3.0/neurodamus/morphio_wrapper.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/neuromodulation_manager.py` & `neurodamus-3.3.0/neurodamus/neuromodulation_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/ngv.py` & `neurodamus-3.3.0/neurodamus/ngv.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/node.py` & `neurodamus-3.3.0/neurodamus/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1519,64 +1519,59 @@
             if len(gids):
                 log_all(logging.INFO, "Rank %d: Debugging %d gids from debug_gids.txt",
                         MPI.rank, len(gids))
 
         for gid in gids:
             self._pc.prcellstate(gid, suffix)
 
-    # ---------------------------------------------------------------------------
-    # Note: This method may be called automatically from Neurodamus.__del__
-    #     and therefore it must stay as simple as possible as exceptions are ignored
     def cleanup(self):
         """Have the compute nodes wrap up tasks before exiting.
         """
         # MemUsage constructor will do MPI communications
         print_mem_usage()
 
         # Coreneuron runs clear the model before starting
         if not SimConfig.use_coreneuron or SimConfig.simulate_model is False:
             self.clear_model(avoid_creating_objs=True)
 
         if SimConfig.delete_corenrn_data and not SimConfig.dry_run:
-            data_folder = SimConfig.coreneuron_datadir
-            logging.info("Deleting intermediate data in %s", data_folder)
-
             with timeit(name="Delete corenrn data"):
-                if MPI.rank == 0:
-                    if ospath.islink(data_folder):
-                        # in restore, coreneuron data is a symbolic link
-                        os.unlink(data_folder)
-                    else:
-                        subprocess.call(['/bin/rm', '-rf', data_folder])
-                    os.remove(ospath.join(SimConfig.output_root, "sim.conf"))
-                    if self._run_conf["EnableReports"]:
-                        os.remove(ospath.join(SimConfig.output_root, "report.conf"))
-
-                # Delete the SHM folder if it was used
-                if self._shm_enabled:
-                    data_folder_shm = SHMUtil.get_datadir_shm(data_folder)
-                    logging.info("Deleting intermediate SHM data in %s", data_folder_shm)
-                    subprocess.call(['/bin/rm', '-rf', data_folder_shm])
+                self._delete_corenrn_data()
+                MPI.barrier()
 
-            MPI.barrier()
+    @run_only_rank0
+    def _delete_corenrn_data(self):
+        data_folder = SimConfig.coreneuron_datadir
+        logging.info("Deleting intermediate data in %s", data_folder)
+
+        if ospath.islink(data_folder):
+            # in restore, coreneuron data is a symbolic link
+            os.unlink(data_folder)
+        else:
+            subprocess.call(['/bin/rm', '-rf', data_folder])
+        os.remove(ospath.join(SimConfig.output_root, "sim.conf"))
+        if self._run_conf["EnableReports"]:
+            os.remove(ospath.join(SimConfig.output_root, "report.conf"))
 
-        logging.info("Finished")
-        TimerManager.timeit_show_stats()
+        # Delete the SHM folder if it was used
+        if self._shm_enabled:
+            data_folder_shm = SHMUtil.get_datadir_shm(data_folder)
+            logging.info("Deleting intermediate SHM data in %s", data_folder_shm)
+            subprocess.call(['/bin/rm', '-rf', data_folder_shm])
 
 
 # Helper class
 # ------------
 class Neurodamus(Node):
     """A high level interface to Neurodamus
     """
 
     def __init__(
         self, config_file,
         auto_init=True,
-        cleanup_atexit=True,
         logging_level=None,
         **user_opts
     ):
         """Creates and initializes a neurodamus run node
 
         As part of Initiazation it calls:
          * load_targets
@@ -1588,45 +1583,37 @@
         Args:
             config_file: The simulation config recipe file
             logging_level: (int) Redefine the global logging level.
                 0 - Only warnings / errors
                 1 - Info messages (default)
                 2 - Verbose
                 3 - Debug messages
-            cleanup_atexit: (bool) Call cleanup in the destructor
-                [for more see: https://bbpteam.epfl.ch/project/issues/browse/BBPBGLIB-976]
             user_opts: Options to Neurodamus overriding the simulation config file
         """
-        self._init_ok = False
-        self.cleanup_atexit = cleanup_atexit
         enable_reports = not user_opts.pop("disable_reports", False)
 
         if logging_level is not None:
             GlobalConfig.verbosity = logging_level
 
         Node.__init__(self, config_file, user_opts)
         # Use the run_conf dict to avoid passing it around
         self._run_conf["EnableReports"] = enable_reports
         self._run_conf["AutoInit"] = auto_init
 
         if SimConfig.dry_run:
             self.load_targets()
             self.create_cells()
             self.create_synapses()
-            self._init_ok = True
             return
 
         if SimConfig.restore_coreneuron:
             self._coreneuron_restore()
         elif SimConfig.build_model:
             self._instantiate_simulation()
 
-        # In case an exception occurs we must prevent the destructor from cleaning
-        self._init_ok = True
-
         # Remove .SUCCESS file if exists
         self._success_file = SimConfig.config_file + ".SUCCESS"
         self._remove_file(self._success_file)
 
     # -
     def _build_model(self):
         log_stage("================ CALCULATING LOAD BALANCE ================")
@@ -1778,17 +1765,22 @@
             TimerManager.archive(archive_name="Cycle Run {:d}".format(cycle_i + 1))
 
         if MPI.rank == 0:
             self._merge_filesdat(n_cycles)
 
     # -
     @timeit(name="finished Run")
-    def run(self):
+    def run(self, cleanup=True):
         """Prepares and launches the simulation according to the loaded config.
         If '--only-build-model' option is set, simulation is skipped.
+
+        Args:
+            cleanup (bool): Free up the model and intermediate files [default: true]
+                Rationale is: the high-level run() method it's typically for a
+                one shot simulation so we should cleanup. If not it can be set to False
         """
         if SimConfig.dry_run:
             log_stage("============= DRY RUN (SKIP SIMULATION) =============")
             self._dry_run_stats.display_total()
             self._dry_run_stats.display_node_suggestions()
             ranks = self._dry_run_stats.get_num_target_ranks(SimConfig.num_target_ranks)
             self._dry_run_stats.collect_all_mpi()
@@ -1799,20 +1791,20 @@
             log_stage("======== [SKIPPED] SIMULATION (MODEL BUILD ONLY) ========")
         elif not SimConfig.build_model:
             log_stage("============= SIMULATION (SKIP MODEL BUILD) =============")
             self._run_coreneuron()
         else:
             log_stage("======================= SIMULATION =======================")
             self.run_all()
+
         # Create SUCCESS file if the simulation finishes successfully
         self._touch_file(self._success_file)
-        logging.info("Creating .SUCCESS file: '%s'", self._success_file)
+        logging.info("Finished! Creating .SUCCESS file: '%s'", self._success_file)
 
-    def __del__(self):
-        if self._init_ok and self.cleanup_atexit:
+        if cleanup:
             self.cleanup()
 
     @run_only_rank0
     def _remove_file(self, file_name):
         import contextlib
         with contextlib.suppress(FileNotFoundError):
             os.remove(file_name)
```

### Comparing `neurodamus-3.2.1/neurodamus/replay.py` & `neurodamus-3.3.0/neurodamus/replay.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/report.py` & `neurodamus-3.3.0/neurodamus/report.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/stimulus_manager.py` & `neurodamus-3.3.0/neurodamus/stimulus_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     """
 
     IsNoise = False
 
     def __init__(self, _target, stim_info: dict, _cell_manager):
         self.duration = float(stim_info["Duration"])  # duration [ms]
         self.delay = float(stim_info["Delay"])        # start time [ms]
+        self.represents_physical_electrode = stim_info.get('RepresentsPhysicalElectrode', False)
 
 
 @StimulusManager.register_type
 class OrnsteinUhlenbeck(BaseStim):
     """
     Ornstein-Uhlenbeck process, injected as current or conductance
     """
@@ -119,15 +120,18 @@
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 rng = random.Random123(seed1, seed2, seed3(gid))  # setup RNG
                 ou_args = (self.tau, self.sigma, self.mean, self.duration)
-                ou_kwargs = {'dt': self.dt, 'delay': self.delay, 'rng': rng}
+                ou_kwargs = {
+                    'dt': self.dt, 'delay': self.delay, 'rng': rng,
+                    'physical_electrode': self.represents_physical_electrode
+                }
                 # inject Ornstein-Uhlenbeck signal
                 if stim_info["Mode"] == "Conductance":
                     cs = ConductanceSource.ornstein_uhlenbeck(*ou_args, **ou_kwargs,
                                                               base_amp=self.reversal)
                 else:
                     cs = CurrentSource.ornstein_uhlenbeck(*ou_args, **ou_kwargs)
                 # attach source to section
@@ -248,15 +252,18 @@
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 rng = random.Random123(seed1, seed2, seed3(gid))  # setup RNG
                 shotnoise_args = (self.tau_D, self.tau_R, self.rate,
                                   self.amp_mean, self.amp_var, self.duration)
-                shotnoise_kwargs = {'dt': self.dt, 'delay': self.delay, 'rng': rng}
+                shotnoise_kwargs = {
+                    'dt': self.dt, 'delay': self.delay, 'rng': rng,
+                    'physical_electrode': self.represents_physical_electrode
+                }
                 # generate shot noise current source
                 if stim_info["Mode"] == "Conductance":
                     cs = ConductanceSource.shot_noise(*shotnoise_args, **shotnoise_kwargs,
                                                       base_amp=self.reversal)
                 else:
                     cs = CurrentSource.shot_noise(*shotnoise_args, **shotnoise_kwargs)
                 # attach current source to section
@@ -450,16 +457,19 @@
 
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 # generate ramp current source
-                cs = CurrentSource.ramp(self.amp_start, self.amp_end, self.duration,
-                                        delay=self.delay)
+                cs = CurrentSource.ramp(
+                    self.amp_start, self.amp_end, self.duration,
+                    delay=self.delay,
+                    physical_electrode=self.represents_physical_electrode
+                )
                 # attach current source to section
                 cs.attach_to(sc.sec, tpoint_list.x[sec_id])
                 self.stimList.append(cs)  # save CurrentSource
 
     def parse_check_all_parameters(self, stim_info: dict):
         # Amplitude at start
         self.amp_start = float(stim_info["AmpStart"])
@@ -547,23 +557,19 @@
         super().__init__(target, stim_info, cell_manager)
 
         self.stimList = []  # CurrentSource's go here
 
         self.parse_check_all_parameters(stim_info)
 
         sim_dt = float(SimConfig.run_conf["Dt"])  # simulation time-step [ms]
-        rng_mode = SimConfig.rng_info.getRNGMode()  # simulation RNGMode
 
         # setup RNG
-        if rng_mode == SimConfig.rng_info.RANDOM123:
-            rand = lambda gid: random.Random123(Noise.stimCount + 100,
-                                                SimConfig.rng_info.getStimulusSeed() + 500,
-                                                gid + 300)
-        else:
-            raise Exception("rng_mod is not RANDOM123")
+        rand = lambda gid: random.Random123(Noise.stimCount + 100,
+                                            SimConfig.rng_info.getStimulusSeed() + 500,
+                                            gid + 300)
 
         # apply stim to each point in target
         tpoints = target.getPointList(cell_manager)
         for tpoint_list in tpoints:
             gid = tpoint_list.gid
             cell = cell_manager.get_cell(gid)
 
@@ -576,16 +582,18 @@
 
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 # generate noise current source
-                cs = CurrentSource.noise(self.mean, self.var, self.duration,
-                                         dt=self.dt, delay=self.delay, rng=rng)
+                cs = CurrentSource.noise(
+                    self.mean, self.var, self.duration, dt=self.dt, delay=self.delay, rng=rng,
+                    physical_electrode=self.represents_physical_electrode
+                )
                 # attach current source to section
                 cs.attach_to(sc.sec, tpoint_list.x[sec_id])
                 self.stimList.append(cs)  # save CurrentSource
 
         Noise.stimCount += 1  # increment global count
 
     def parse_check_all_parameters(self, stim_info: dict):
@@ -656,16 +664,19 @@
         for tpoint_list in tpoints:
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 # generate pulse train current source
-                cs = CurrentSource.train(self.amp, self.freq, self.width,
-                                         self.duration, delay=self.delay)
+                cs = CurrentSource.train(
+                    self.amp, self.freq, self.width, self.duration,
+                    delay=self.delay,
+                    physical_electrode=self.represents_physical_electrode
+                )
                 # attach current source to section
                 cs.attach_to(sc.sec, tpoint_list.x[sec_id])
                 self.stimList.append(cs)  # save CurrentSource
 
     def parse_check_all_parameters(self, stim_info: dict):
         self.amp = float(stim_info["AmpStart"])  # amplitude [nA]
         self.freq = float(stim_info["Frequency"])  # frequency [Hz]
@@ -692,16 +703,18 @@
         for tpoint_list in tpoints:
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 # generate sinusoidal current source
-                cs = CurrentSource.sin(self.amp, self.duration, self.freq,
-                                       step=self.dt, delay=self.delay)
+                cs = CurrentSource.sin(
+                    self.amp, self.duration, self.freq, step=self.dt, delay=self.delay,
+                    physical_electrode=self.represents_physical_electrode
+                )
                 # attach current source to section
                 cs.attach_to(sc.sec, tpoint_list.x[sec_id])
                 self.stimList.append(cs)  # save CurrentSource
 
     def parse_check_all_parameters(self, stim_info: dict):
         self.dt = float(stim_info.get("Dt", 0.025))  # stimulus timestep [ms]
         if self.dt <= 0:
@@ -731,14 +744,15 @@
             for sec_id, sc in enumerate(tpoint_list.sclst):
                 # skip sections not in this split
                 if not sc.exists():
                     continue
 
                 # create single electrode voltage clamp at location
                 seclamp = Nd.h.SEClamp(tpoint_list.x[sec_id], sec=sc.sec)
+
                 seclamp.rs = self.rs
                 seclamp.dur1 = self.duration
                 seclamp.amp1 = self.vhold
                 self.stimList.append(seclamp)  # save SEClamp
 
     def parse_check_all_parameters(self, stim_info: dict):
         self.vhold = float(stim_info["Voltage"])  # holding voltage [mV]
```

### Comparing `neurodamus-3.2.1/neurodamus/target_manager.py` & `neurodamus-3.3.0/neurodamus/target_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/__init__.py` & `neurodamus-3.3.0/neurodamus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_engine.py` & `neurodamus-3.3.0/neurodamus/core/_engine.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_mpi.py` & `neurodamus-3.3.0/neurodamus/core/_mpi.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_neurodamus.py` & `neurodamus-3.3.0/neurodamus/core/_neurodamus.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_neuron.py` & `neurodamus-3.3.0/neurodamus/core/_neuron.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_shmutils.py` & `neurodamus-3.3.0/neurodamus/core/_shmutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/_utils.py` & `neurodamus-3.3.0/neurodamus/core/_utils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/cell.py` & `neurodamus-3.3.0/neurodamus/core/cell.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/configuration.py` & `neurodamus-3.3.0/neurodamus/core/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,14 @@
     MorphologyPath = None
     CircuitTarget = None
     PopulationID = 0
     DetailedAxon = False
 
 
 class RNGConfig(ConfigT):
-    Modes = Enum("Mode", "COMPATIBILITY RANDOM123 UPMCELLRAN4")
-    mode = Modes.COMPATIBILITY
     global_seed = None
     IonChannelSeed = None
     StimulusSeed = None
     MinisSeed = None
     SynapseSeed = None
```

### Comparing `neurodamus-3.2.1/neurodamus/core/coreneuron_configuration.py` & `neurodamus-3.3.0/neurodamus/core/coreneuron_configuration.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/mechanisms.py` & `neurodamus-3.3.0/neurodamus/core/mechanisms.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/nodeset.py` & `neurodamus-3.3.0/neurodamus/core/nodeset.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/core/stimuli.py` & `neurodamus-3.3.0/neurodamus/core/stimuli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from . import Neuron
 from .random import RNG, gamma
 import logging
 
 
 class SignalSource:
 
-    def __init__(self, base_amp=0.0, *, delay=0, rng=None):
+    def __init__(self, base_amp=0.0, *, delay=0, rng=None, represents_physical_electrode=False):
         """
         Creates a new signal source, which can create composed signals
         Args:
             base_amp: The base (resting) amplitude of the signal (Default: 0)
             rng: The Random Number Generator. Used in the Noise functions
+            represents_physical_electrode: Whether the source represents a phsyical
+            electrode or missing synaptic input
         """
         h = Neuron.h
         self.stim_vec = h.Vector()
         self.time_vec = h.Vector()
         self._cur_t = 0
         self._base_amp = base_amp
         self._rng = rng
+        self._represents_physical_electrode = represents_physical_electrode
         if delay > .0:
             self._add_point(base_amp)
             self._cur_t = delay
 
     def reset(self):
         self.stim_vec.resize(0)
         self.time_vec.resize(0)
@@ -352,38 +355,46 @@
 
     @classmethod
     def shot_noise(cls, tau_D, tau_R, rate, amp_mean, var, duration, dt=0.25, base_amp=.0, **kw):
         return cls(base_amp, **kw).add_shot_noise(tau_D, tau_R, rate, amp_mean, var, duration, dt)
 
     @classmethod
     def ornstein_uhlenbeck(cls, tau, sigma, mean, duration, dt=0.25, base_amp=.0, **kw):
-        return cls(base_amp, **kw).add_ornstein_uhlenbeck(tau, sigma, mean,duration, dt)
+        return cls(base_amp, **kw).add_ornstein_uhlenbeck(tau, sigma, mean, duration, dt)
 
     # Operations
     def __add__(self, other):
         """# Adds signals. Two added signals sum amplitudes"""
         raise NotImplementedError("Adding signals is not available yet")
 
 
 class CurrentSource(SignalSource):
     _all_sources = []
 
-    def __init__(self, base_amp=0.0, *, delay=0, rng=None):
+    def __init__(self, base_amp=0.0, *, delay=0, rng=None, physical_electrode=False):
         """
         Creates a new current source that injects a signal under IClamp
         """
-        super().__init__(base_amp, delay=delay, rng=rng)
+        super().__init__(base_amp, delay=delay, rng=rng,
+                         represents_physical_electrode=physical_electrode)
         self._clamps = set()
         self._all_sources.append(self)
 
     class _Clamp:
         def __init__(self, cell_section, position=0.5, clamp_container=None,
                      stim_vec_mode=True, time_vec=None, stim_vec=None,
                      **clamp_params):
-            self.clamp = Neuron.h.IClamp(position, sec=cell_section)
+            represents_physical_electrode = clamp_params.get('represents_physical_electrode', False)
+            # Checks if new MembraneCurrentSource mechanism is available and if source does not
+            # represent physical electrode, otherwise fall back to IClamp.
+            if not represents_physical_electrode and hasattr(Neuron.h, "MembraneCurrentSource"):
+                self.clamp = Neuron.h.MembraneCurrentSource(position, sec=cell_section)
+            else:
+                self.clamp = Neuron.h.IClamp(position, sec=cell_section)
+
             if stim_vec_mode:
                 assert time_vec is not None and stim_vec is not None
                 self.clamp.dur = time_vec[-1]
                 stim_vec.play(self.clamp._ref_amp, time_vec, 1)
             else:
                 for param, val in clamp_params.items():
                     setattr(self.clamp, param, val)
@@ -393,16 +404,17 @@
 
         def detach(self):
             """Detaches a clamp from a cell, destroying it"""
             self._all_clamps.discard(self)
             del self.clamp  # Force del on the clamp (there might be references to self)
 
     def attach_to(self, section, position=0.5):
-        return CurrentSource._Clamp(section, position, self._clamps, True,
-                                    self.time_vec, self.stim_vec)
+        return CurrentSource._Clamp(
+            section, position, self._clamps, True, self.time_vec, self.stim_vec,
+            represents_physical_electrode=self._represents_physical_electrode)
 
     # Constant has a special attach_to and doesnt share any composing method
     class Constant:
         """Class implementing a minimal IClamp for a Constant current."""
         _clamps = set()
 
         def __init__(self, amp, duration, delay=0):
@@ -414,31 +426,40 @@
             return CurrentSource._Clamp(section, position, self._clamps, False,
                                         amp=self._amp, delay=self._delay, dur=self._dur)
 
 
 class ConductanceSource(SignalSource):
     _all_sources = []
 
-    def __init__(self, reversal=0.0, *, delay=.0, rng=None):
+    def __init__(self, reversal=0.0, *, delay=.0, rng=None, physical_electrode=False):
         """
         Creates a new conductance source that injects a conductance by driving
         the rs of an SEClamp at a given reversal potential.
 
         reversal: reversal potential of conductance (mV)
         """
-        super().__init__(0.0, delay=delay, rng=rng)  # set SignalSource's base_amp to zero
+        # set SignalSource's base_amp to zero
+        super().__init__(reversal, delay=delay, rng=rng,
+                         represents_physical_electrode=physical_electrode)
         self._reversal = reversal   # set reversal from base_amp parameter in classmethods
         self._clamps = set()
         self._all_sources.append(self)
 
     class _DynamicClamp:
         def __init__(self, cell_section, position=0.5, clamp_container=None,
                      stim_vec_mode=True, time_vec=None, stim_vec=None,
                      reversal=0.0, **clamp_params):
-            self.clamp = Neuron.h.SEClamp(position, sec=cell_section)
+            represents_physical_electrode = clamp_params.get('represents_physical_electrode', False)
+            # Checks if new conductanceSource mechanism is available and if source does not
+            # represent physical electrode, otherwise fall back to SEClamp.
+            if not represents_physical_electrode and hasattr(Neuron.h, "ConductanceSource"):
+                self.clamp = Neuron.h.ConductanceSource(position, sec=cell_section)
+            else:
+                self.clamp = Neuron.h.SEClamp(position, sec=cell_section)
+
             if stim_vec_mode:
                 assert time_vec is not None and stim_vec is not None
                 self.clamp.dur1 = time_vec[-1]
                 self.clamp.amp1 = reversal
                 # support delay with initial zero
                 self.time_vec = Neuron.h.Vector(1, 0).append(time_vec)
                 self.stim_vec = Neuron.h.Vector(1, 0).append(stim_vec)
@@ -456,16 +477,17 @@
 
         def detach(self):
             """Detaches a clamp from a cell, destroying it"""
             self._all_clamps.discard(self)
             del self.clamp  # Force del on the clamp (there might be references to self)
 
     def attach_to(self, section, position=0.5):
-        return ConductanceSource._DynamicClamp(section, position, self._clamps, True,
-                                               self.time_vec, self.stim_vec, self._reversal)
+        return ConductanceSource._DynamicClamp(
+            section, position, self._clamps, True, self.time_vec, self.stim_vec,
+            self._reversal, represents_physical_electrode=self._represents_physical_electrode)
 
 
 # EStim class is a derivative of TStim for stimuli with an extracelular electrode. The main
 # difference is that it collects all elementary stimuli pulses and converts them using a
 # VirtualElectrode object before it injects anything
 #
 # The stimulus is defined on the hoc level by using the addpoint function for every (step) change
```

### Comparing `neurodamus-3.2.1/neurodamus/core/synapses.py` & `neurodamus-3.3.0/neurodamus/core/synapses.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/init.py` & `neurodamus-3.3.0/neurodamus/data/init.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/Cell.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/Cell.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/ConnectionUtils.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/ConnectionUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/Map.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/Map.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/MorphIO.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/MorphIO.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/defvar.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/defvar.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/hoc/fileUtils.hoc` & `neurodamus-3.3.0/neurodamus/data/hoc/fileUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/ALU.mod` & `neurodamus-3.3.0/neurodamus/data/mod/ALU.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/HDF5reader.mod` & `neurodamus-3.3.0/neurodamus/data/mod/HDF5reader.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/SonataReportHelper.mod` & `neurodamus-3.3.0/neurodamus/data/mod/SonataReportHelper.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/SonataReports.mod` & `neurodamus-3.3.0/neurodamus/data/mod/SonataReports.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/VecStim.mod` & `neurodamus-3.3.0/neurodamus/data/mod/VecStim.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/data/mod/netstim_inhpoisson.mod` & `neurodamus-3.3.0/neurodamus/data/mod/netstim_inhpoisson.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/io/cell_readers.py` & `neurodamus-3.3.0/neurodamus/io/cell_readers.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/io/sonata_config.py` & `neurodamus-3.3.0/neurodamus/io/sonata_config.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/io/synapse_reader.py` & `neurodamus-3.3.0/neurodamus/io/synapse_reader.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/cli.py` & `neurodamus-3.3.0/neurodamus/utils/cli.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/compat.py` & `neurodamus-3.3.0/neurodamus/utils/compat.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/logging.py` & `neurodamus-3.3.0/neurodamus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/memory.py` & `neurodamus-3.3.0/neurodamus/utils/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 from .compat import Vector
 from collections import defaultdict
 from enum import Enum
 from ..io.sonata_config import ConnectionTypes
 
 import numpy as np
 
+# The factor to multiply the cell + synapses memory usage by to get the simulation memory estimate.
+# This is an heuristic estimate based on tests on multiple circuits.
+# More info in docs/architecture.rst.
+SIM_ESTIMATE_FACTOR = 2.5
+
 
 def trim_memory():
     """
     malloc_trim - release free memory from the heap (back to the OS)
 
     * We should only run malloc_trim if we are using the default glibc memory allocator.
     When using a custom allocator such as jemalloc, this could cause unexpected behavior
@@ -357,16 +362,22 @@
         logging.info("+{:=^57}+".format(" Total Memory Estimates "))
         logging.info("| {:^40s} | {:^12s} |".format("Item", "Memory (MiB)"))
         logging.info("+{:-^57}+".format(""))
         full_overhead = self.base_memory * MPI.size
         logging.info("| {:<40s} | {:12.1f} |".format(f"Overhead (ranks={MPI.size})", full_overhead))
         logging.info("| {:<40s} | {:12.1f} |".format("Cells", self.cell_memory_total))
         logging.info("| {:<40s} | {:12.1f} |".format("Synapses", self.synapse_memory_total))
+        self.simulation_estimate = (self.cell_memory_total
+                                    + self.synapse_memory_total) * SIM_ESTIMATE_FACTOR
+        logging.info("| {:<40s} | {:12.1f} |".format("Simulation", self.simulation_estimate))
         logging.info("+{:-^57}+".format(""))
-        grand_total = full_overhead + self.cell_memory_total + self.synapse_memory_total
+        grand_total = (full_overhead
+                       + self.cell_memory_total
+                       + self.synapse_memory_total
+                       + self.simulation_estimate)
         grand_total = pretty_printing_memory_mb(grand_total)
         logging.info("| {:<40s} | {:>12s} |".format("GRAND TOTAL", grand_total))
         logging.info("+{:-^57}+".format(""))
 
     def total_memory_available():
         """
         Returns the total memory available in the system in MB
@@ -398,15 +409,20 @@
         est_nodes = 0
         prev_est_nodes = None
         max_iter = 5
         iter_count = 0
 
         while (prev_est_nodes is None or est_nodes != prev_est_nodes) and iter_count < max_iter:
             prev_est_nodes = est_nodes
-            mem_usage_per_node = full_overhead + self.cell_memory_total + self.synapse_memory_total
+            simulation_estimate = (self.cell_memory_total +
+                                   self.synapse_memory_total) * SIM_ESTIMATE_FACTOR
+            mem_usage_per_node = (full_overhead
+                                  + self.cell_memory_total
+                                  + self.synapse_memory_total
+                                  + simulation_estimate)
             mem_usage_with_margin = mem_usage_per_node * (1 + margin)
             est_nodes = math.ceil(mem_usage_with_margin / DryRunStats.total_memory_available())
             full_overhead = self.base_memory * ranks_per_node * est_nodes
             iter_count += 1
 
         return est_nodes
```

### Comparing `neurodamus-3.2.1/neurodamus/utils/multimap.py` & `neurodamus-3.3.0/neurodamus/utils/multimap.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/progressbar.py` & `neurodamus-3.3.0/neurodamus/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/pyutils.py` & `neurodamus-3.3.0/neurodamus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/neurodamus/utils/timeit.py` & `neurodamus-3.3.0/neurodamus/utils/timeit.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
     units = ['', 'K', 'M', 'B', 'T', 'P']
     power = int(floor(log(num, 1000.)))
     return '{:.2f}{:s}'.format(num / 1000. ** power, units[power]) if power >= 1 \
         else str(int(num))
 
 
-delim = u'\u255a'
+delim = '+'
 
 
 class _Timer(object):
     total_time = property(lambda self: self._total_time)
     accumulated = property(lambda self: self._accumulated)
     name = property(lambda self: self._name)
     hits = property(lambda self: self._hits)
```

### Comparing `neurodamus-3.2.1/LICENSE.txt` & `neurodamus-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/README.rst` & `neurodamus-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/pyproject.toml` & `neurodamus-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.1/PKG-INFO` & `neurodamus-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: neurodamus
-Version: 3.2.1
+Version: 3.3.0
 Summary: A BBP Simulation Control application for NEURON
 Project-URL: Homepage, https://github.com/BlueBrain/neurodamus
 Project-URL: Repository, https://github.com/BlueBrain/neurodamus.git
 Project-URL: Tracker, https://github.com/BlueBrain/neurodamus/issues
 Author: Blue Brain Project, EPFL
 License:                                  Apache License
                                    Version 2.0, January 2004
```

