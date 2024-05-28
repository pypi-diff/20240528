# Comparing `tmp/gemmi-0.6.5.tar.gz` & `tmp/gemmi-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi-0.6.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "gemmi-0.6.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `gemmi-0.6.5.tar` & `gemmi-0.6.6.tar`

### file list

```diff
@@ -1,465 +1,491 @@
--rw-r--r--   0        0        0    23125 2022-11-09 12:37:21.000000 gemmi-0.6.5/CMakeLists.txt
--rw-r--r--   0        0        0    16726 2022-11-09 12:37:21.000000 gemmi-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 gemmi-0.6.5/README.md
--rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/elem.cpp
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/mod.cpp
--rw-r--r--   0        0        0     1926 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/niggli.cpp
--rw-r--r--   0        0        0     5643 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/pdb.cpp
--rw-r--r--   0        0        0     3563 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/resinfo.cpp
--rw-r--r--   0        0        0     2434 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/round.cpp
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/smat33.cpp
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/stoi.cpp
--rw-r--r--   0        0        0     2382 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/sym.cpp
--rw-r--r--   0        0        0     1237 2022-11-09 12:37:21.000000 gemmi-0.6.5/benchmarks/writecif.cpp
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/cell.cpp
--rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/cif_cc.cpp
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/elem.cpp
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/maybegz.cpp
--rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/mutate.cpp
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/newmtz.cpp
--rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/resinfo.cpp
--rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/smcif.cpp
--rw-r--r--   0        0        0     1237 2022-11-09 12:37:21.000000 gemmi-0.6.5/docs/code/sym.cpp
--rwxr-xr-x   0        0        0     1175 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/aafreq.py
--rw-r--r--   0        0        0     1233 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/auth_label.cpp
--rwxr-xr-x   0        0        0     2378 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/ccd_gi.py
--rwxr-xr-x   0        0        0     1266 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/ccd_subgraph.py
--rw-r--r--   0        0        0     3161 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/check_conn.cpp
--rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/check_symmetry.cpp
--rw-r--r--   0        0        0      529 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/cif_i_sigi.py
--rwxr-xr-x   0        0        0     1300 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/col_order.py
--rwxr-xr-x   0        0        0      725 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/from_json.py
--rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/hello.cpp
--rwxr-xr-x   0        0        0      503 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/hello.py
--rwxr-xr-x   0        0        0     1442 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/long_geom.py
--rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/map2mtz.py
--rw-r--r--   0        0        0     3822 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/maskcheck.py
--rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/maskdiff.py
--rwxr-xr-x   0        0        0     6844 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/matthews.py
--rwxr-xr-x   0        0        0     1446 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/merge_mtz_mmcif.py
--rwxr-xr-x   0        0        0     5359 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/monomers.py
--rwxr-xr-x   0        0        0     1052 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/mtrix_iso.py
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/mtz_i_sigi.py
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/multiproc.py
--rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/patterson_slice.py
--rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/rama_gather.py
--rwxr-xr-x   0        0        0     1182 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/rama_plot.py
--rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/refln-stats.py
--rwxr-xr-x   0        0        0      323 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/simple_search.py
--rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/sub_ccd.py
--rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/torsion_in_ring.cpp
--rwxr-xr-x   0        0        0     4952 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/weight.py
--rw-r--r--   0        0        0     7656 2022-11-09 12:37:21.000000 gemmi-0.6.5/examples/with_bgl.cpp
--rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/addends.hpp
--rw-r--r--   0        0        0    11686 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/align.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/assembly.hpp
--rw-r--r--   0        0        0     7455 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/asudata.hpp
--rw-r--r--   0        0        0    11452 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/asumask.hpp
--rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/atof.hpp
--rw-r--r--   0        0        0     3810 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/atox.hpp
--rw-r--r--   0        0        0     3983 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/bessel.hpp
--rw-r--r--   0        0        0     7728 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/binner.hpp
--rw-r--r--   0        0        0     4864 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/blob.hpp
--rw-r--r--   0        0        0     3045 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/bond_idx.hpp
--rw-r--r--   0        0        0    10347 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/c4322.hpp
--rw-r--r--   0        0        0     5574 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/calculate.hpp
--rw-r--r--   0        0        0    17346 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/ccp4.hpp
--rw-r--r--   0        0        0    13372 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/cellred.hpp
--rw-r--r--   0        0        0    24868 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/chemcomp.hpp
--rw-r--r--   0        0        0     4707 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/chemcomp_xyz.hpp
--rw-r--r--   0        0        0    14157 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/cif.hpp
--rw-r--r--   0        0        0    21583 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/cif2mtz.hpp
--rw-r--r--   0        0        0    37584 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/cifdoc.hpp
--rw-r--r--   0        0        0     5036 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/contact.hpp
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/crd.hpp
--rw-r--r--   0        0        0     2570 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/ddl.hpp
--rw-r--r--   0        0        0     7505 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/dencalc.hpp
--rw-r--r--   0        0        0     7379 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/dirwalk.hpp
--rw-r--r--   0        0        0     3246 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/ecalc.hpp
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/eig3.hpp
--rw-r--r--   0        0        0    14569 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/elem.hpp
--rw-r--r--   0        0        0     4526 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/enumstr.hpp
--rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/fail.hpp
--rw-r--r--   0        0        0     3810 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/fileutil.hpp
--rw-r--r--   0        0        0     5176 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/floodfill.hpp
--rw-r--r--   0        0        0     6424 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/formfact.hpp
--rw-r--r--   0        0        0    13533 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/fourier.hpp
--rw-r--r--   0        0        0   271931 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/fprime.hpp
--rw-r--r--   0        0        0     2222 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/fstream.hpp
--rw-r--r--   0        0        0    27376 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/grid.hpp
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/gz.hpp
--rw-r--r--   0        0        0     4508 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/input.hpp
--rw-r--r--   0        0        0     5206 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/intensit.hpp
--rw-r--r--   0        0        0     1864 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/interop.hpp
--rw-r--r--   0        0        0    23738 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/it92.hpp
--rw-r--r--   0        0        0    10089 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/iterator.hpp
--rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/json.hpp
--rw-r--r--   0        0        0     9023 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/levmar.hpp
--rw-r--r--   0        0        0     6763 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/linkhunt.hpp
--rw-r--r--   0        0        0    15230 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/math.hpp
--rw-r--r--   0        0        0    13886 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/metadata.hpp
--rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mmcif.hpp
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mmcif_impl.hpp
--rw-r--r--   0        0        0    11289 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mmdb.hpp
--rw-r--r--   0        0        0     3894 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mmread.hpp
--rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mmread_gz.hpp
--rw-r--r--   0        0        0    39656 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/model.hpp
--rw-r--r--   0        0        0     8826 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/modify.hpp
--rw-r--r--   0        0        0    11660 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/monlib.hpp
--rw-r--r--   0        0        0    37353 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mtz.hpp
--rw-r--r--   0        0        0     5019 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/mtz2cif.hpp
--rw-r--r--   0        0        0    13443 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/neighbor.hpp
--rw-r--r--   0        0        0     2759 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/neutron92.hpp
--rw-r--r--   0        0        0     1479 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/numb.hpp
--rw-r--r--   0        0        0    28186 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/pdb.hpp
--rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/pdb_id.hpp
--rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/pirfasta.hpp
--rw-r--r--   0        0        0     7765 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/polyheur.hpp
--rw-r--r--   0        0        0    12909 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/qcp.hpp
--rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/read_cif.hpp
--rw-r--r--   0        0        0     1117 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/read_map.hpp
--rw-r--r--   0        0        0     6457 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/recgrid.hpp
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/reciproc.hpp
--rw-r--r--   0        0        0     8868 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/refln.hpp
--rw-r--r--   0        0        0    25493 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/remarks.hpp
--rw-r--r--   0        0        0     3682 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/resinfo.hpp
--rw-r--r--   0        0        0     1016 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/riding_h.hpp
--rw-r--r--   0        0        0    10197 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/scaling.hpp
--rw-r--r--   0        0        0    16677 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/select.hpp
--rw-r--r--   0        0        0    11291 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/seqalign.hpp
--rw-r--r--   0        0        0     5125 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/seqid.hpp
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/seqtools.hpp
--rw-r--r--   0        0        0     5714 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/serialize.hpp
--rw-r--r--   0        0        0     5631 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/sfcalc.hpp
--rw-r--r--   0        0        0     4034 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/small.hpp
--rw-r--r--   0        0        0     6800 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/smcif.hpp
--rw-r--r--   0        0        0    18223 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/solmask.hpp
--rw-r--r--   0        0        0     4668 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/span.hpp
--rw-r--r--   0        0        0     2368 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/sprintf.hpp
--rw-r--r--   0        0        0     2761 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/stats.hpp
--rw-r--r--   0        0        0    93858 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/symmetry.hpp
--rw-r--r--   0        0        0   130949 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/fast_float.h
--rw-r--r--   0        0        0   107015 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/pocketfft_hdronly.h
--rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/LICENSE
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/NOTES
--rw-r--r--   0        0        0     4544 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
--rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
--rw-r--r--   0        0        0     1705 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
--rw-r--r--   0        0        0     1099 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
--rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
--rw-r--r--   0        0        0      990 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
--rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analyze.hpp
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
--rw-r--r--   0        0        0     1339 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/argv_input.hpp
--rw-r--r--   0        0        0     3463 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/ascii.hpp
--rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
--rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/config.hpp
--rw-r--r--   0        0        0      872 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
--rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/eol.hpp
--rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
--rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/file_input.hpp
--rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/input_error.hpp
--rw-r--r--   0        0        0     1439 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/action.hpp
--rw-r--r--   0        0        0     2869 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
--rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
--rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/any.hpp
--rw-r--r--   0        0        0     2750 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
--rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
--rw-r--r--   0        0        0     1229 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
--rw-r--r--   0        0        0     1626 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/at.hpp
--rw-r--r--   0        0        0      862 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
--rw-r--r--   0        0        0      870 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
--rw-r--r--   0        0        0     1573 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
--rw-r--r--   0        0        0     1373 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
--rw-r--r--   0        0        0     1076 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
--rw-r--r--   0        0        0     1445 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/control.hpp
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
--rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
--rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
--rw-r--r--   0        0        0     1178 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
--rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
--rw-r--r--   0        0        0     1003 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
--rw-r--r--   0        0        0     7228 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
--rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
--rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
--rw-r--r--   0        0        0     5410 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
--rw-r--r--   0        0        0     2938 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
--rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
--rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
--rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
--rw-r--r--   0        0        0     2011 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
--rw-r--r--   0        0        0     3297 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
--rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
--rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
--rw-r--r--   0        0        0     1862 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
--rw-r--r--   0        0        0     3323 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
--rw-r--r--   0        0        0     1159 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
--rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
--rw-r--r--   0        0        0     1229 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
--rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list.hpp
--rw-r--r--   0        0        0      610 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
--rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
--rw-r--r--   0        0        0     2409 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
--rw-r--r--   0        0        0     2092 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
--rw-r--r--   0        0        0     2484 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/must.hpp
--rw-r--r--   0        0        0     1652 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
--rw-r--r--   0        0        0     2429 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/one.hpp
--rw-r--r--   0        0        0     1648 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
--rw-r--r--   0        0        0     2245 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
--rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
--rw-r--r--   0        0        0     2931 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
--rw-r--r--   0        0        0     4180 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
--rw-r--r--   0        0        0     1786 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
--rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/range.hpp
--rw-r--r--   0        0        0     2994 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
--rw-r--r--   0        0        0     2020 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
--rw-r--r--   0        0        0     2880 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
--rw-r--r--   0        0        0     1500 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
--rw-r--r--   0        0        0     1172 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/require.hpp
--rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
--rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
--rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
--rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
--rw-r--r--   0        0        0     2150 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/star.hpp
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
--rw-r--r--   0        0        0     2769 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/state.hpp
--rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/string.hpp
--rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/until.hpp
--rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/istream_input.hpp
--rw-r--r--   0        0        0     9778 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/memory_input.hpp
--rw-r--r--   0        0        0     1913 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
--rw-r--r--   0        0        0     3897 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/normal.hpp
--rw-r--r--   0        0        0      586 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/nothing.hpp
--rw-r--r--   0        0        0     1616 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/parse.hpp
--rw-r--r--   0        0        0     1106 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/parse_error.hpp
--rw-r--r--   0        0        0     1351 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/position.hpp
--rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/read_input.hpp
--rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
--rw-r--r--   0        0        0     4942 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/rules.hpp
--rw-r--r--   0        0        0     1936 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/string_input.hpp
--rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
--rw-r--r--   0        0        0     2832 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf16.hpp
--rw-r--r--   0        0        0     2832 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf32.hpp
--rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf8.hpp
--rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/version.hpp
--rw-r--r--   0        0        0      793 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tao/pegtl.hpp
--rw-r--r--   0        0        0    19231 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/third_party/tinydir.h
--rw-r--r--   0        0        0     3373 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/to_chemcomp.hpp
--rw-r--r--   0        0        0     7774 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/to_cif.hpp
--rw-r--r--   0        0        0     8862 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/to_json.hpp
--rw-r--r--   0        0        0     2361 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/to_mmcif.hpp
--rw-r--r--   0        0        0     2173 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/to_pdb.hpp
--rw-r--r--   0        0        0    10545 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/topo.hpp
--rw-r--r--   0        0        0    10321 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/twin.hpp
--rw-r--r--   0        0        0    21702 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/unitcell.hpp
--rw-r--r--   0        0        0     2433 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/utf.hpp
--rw-r--r--   0        0        0     9845 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/util.hpp
--rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/version.hpp
--rw-r--r--   0        0        0    14985 2022-11-09 12:37:21.000000 gemmi-0.6.5/include/gemmi/xds_ascii.hpp
--rw-r--r--   0        0        0    14912 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/align.cpp
--rw-r--r--   0        0        0     7789 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/blobs.cpp
--rw-r--r--   0        0        0     3586 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/cif2json.cpp
--rw-r--r--   0        0        0    13306 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/cif2mtz.cpp
--rw-r--r--   0        0        0     3546 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/cifdiff.cpp
--rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/cifmod.h
--rw-r--r--   0        0        0     8280 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/contact.cpp
--rw-r--r--   0        0        0    10512 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/contents.cpp
--rw-r--r--   0        0        0    17708 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/convert.cpp
--rw-r--r--   0        0        0     5609 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/crd.cpp
--rw-r--r--   0        0        0     5579 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/ecalc.cpp
--rw-r--r--   0        0        0     2257 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/fprime.cpp
--rw-r--r--   0        0        0    19996 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/grep.cpp
--rw-r--r--   0        0        0     6305 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/h.cpp
--rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/histogram.h
--rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/json2cif.cpp
--rw-r--r--   0        0        0     6541 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/main.cpp
--rw-r--r--   0        0        0    10826 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/map.cpp
--rw-r--r--   0        0        0     5467 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/map2sf.cpp
--rw-r--r--   0        0        0     8999 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mapcoef.cpp
--rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mapcoef.h
--rw-r--r--   0        0        0     6315 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mask.cpp
--rw-r--r--   0        0        0    12277 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/merge.cpp
--rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mixmtz.cpp
--rw-r--r--   0        0        0     9067 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mondiff.cpp
--rw-r--r--   0        0        0     3369 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/monlib_opt.cpp
--rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/monlib_opt.h
--rw-r--r--   0        0        0    23570 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mtz.cpp
--rw-r--r--   0        0        0    14506 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/mtz2cif.cpp
--rw-r--r--   0        0        0    10811 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/options.cpp
--rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/options.h
--rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/reindex.cpp
--rw-r--r--   0        0        0    13421 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/residues.cpp
--rw-r--r--   0        0        0    11471 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/rmsz.cpp
--rw-r--r--   0        0        0     3857 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/sf2map.cpp
--rw-r--r--   0        0        0    33441 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/sfcalc.cpp
--rw-r--r--   0        0        0     4872 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/sg.cpp
--rw-r--r--   0        0        0    11892 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/tags.cpp
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/timer.h
--rw-r--r--   0        0        0    10932 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/validate.cpp
--rw-r--r--   0        0        0    11777 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/validate_mon.cpp
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/validate_mon.h
--rw-r--r--   0        0        0    14342 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/wcn.cpp
--rw-r--r--   0        0        0    11556 2022-11-09 12:37:21.000000 gemmi-0.6.5/prog/xds2mtz.cpp
--rw-r--r--   0        0        0     3467 2022-11-09 12:37:21.000000 gemmi-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4500 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/align.cpp
--rw-r--r--   0        0        0      327 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/arrvec.h
--rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/ccp4.cpp
--rw-r--r--   0        0        0     8464 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/chemcomp.cpp
--rw-r--r--   0        0        0    20409 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/cif.cpp
--rw-r--r--   0        0        0     3157 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/common.h
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/custom.cpp
--rw-r--r--   0        0        0     5949 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/elem.cpp
--rw-r--r--   0        0        0     6912 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/gemmi.cpp
--rw-r--r--   0        0        0    12801 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/grid.cpp
--rw-r--r--   0        0        0    18024 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/hkl.cpp
--rw-r--r--   0        0        0    17287 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/meta.cpp
--rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/meta.h
--rw-r--r--   0        0        0      571 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/miller_a.h
--rw-r--r--   0        0        0    27662 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/mol.cpp
--rw-r--r--   0        0        0     5685 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/monlib.cpp
--rw-r--r--   0        0        0    17059 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/mtz.cpp
--rw-r--r--   0        0        0     7676 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/read.cpp
--rw-r--r--   0        0        0     9555 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/recgrid.cpp
--rw-r--r--   0        0        0     2055 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/scaling.cpp
--rw-r--r--   0        0        0     6733 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/search.cpp
--rw-r--r--   0        0        0     3693 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/sf.cpp
--rw-r--r--   0        0        0    11581 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/sym.cpp
--rw-r--r--   0        0        0     7584 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/topo.cpp
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/tostr.hpp
--rw-r--r--   0        0        0    17574 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/unitcell.cpp
--rw-r--r--   0        0        0     4725 2022-11-09 12:37:21.000000 gemmi-0.6.5/python/write.cpp
--rw-r--r--   0        0        0     2279 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/align.cpp
--rw-r--r--   0        0        0    17883 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/assembly.cpp
--rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/calculate.cpp
--rw-r--r--   0        0        0    25037 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/crd.cpp
--rw-r--r--   0        0        0    23898 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/ddl.cpp
--rw-r--r--   0        0        0     5904 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/eig3.cpp
--rw-r--r--   0        0        0     4948 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/gz.cpp
--rw-r--r--   0        0        0    15562 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/intensit.cpp
--rw-r--r--   0        0        0     4700 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/json.cpp
--rw-r--r--   0        0        0    38545 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/mmcif.cpp
--rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/mmread_gz.cpp
--rw-r--r--   0        0        0    22129 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/monlib.cpp
--rw-r--r--   0        0        0    16192 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/mtz.cpp
--rw-r--r--   0        0        0    37691 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/mtz2cif.cpp
--rw-r--r--   0        0        0    14015 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/polyheur.cpp
--rw-r--r--   0        0        0      899 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/read_cif.cpp
--rw-r--r--   0        0        0    25715 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/resinfo.cpp
--rw-r--r--   0        0        0    18044 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/riding_h.cpp
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/sprintf.cpp
--rw-r--r--   0        0        0    55330 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/to_mmcif.cpp
--rw-r--r--   0        0        0    27080 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/to_pdb.cpp
--rw-r--r--   0        0        0    44087 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/topo.cpp
--rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 gemmi-0.6.5/src/xds_ascii.cpp
--rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1011031.cif
--rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1lzh.pdb.gz
--rw-r--r--   0        0        0    71037 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1orc.pdb
--rw-r--r--   0        0        0    26819 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1pfe.cif.gz
--rw-r--r--   0        0        0   112575 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1pfe.json
--rw-r--r--   0        0        0     2812 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/1pfe_asu.msk.gz
--rw-r--r--   0        0        0     7328 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/2013551.cif
--rw-r--r--   0        0        0    13833 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/2242624.cif
--rw-r--r--   0        0        0     3328 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/2242624.hkl
--rw-r--r--   0        0        0    19473 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/3dg1_final.cif
--rw-r--r--   0        0        0    12742 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/3wup.json.gz
--rw-r--r--   0        0        0    36221 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/4003024.cif
--rw-r--r--   0        0        0     4319 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/4aap-sf-subset.cif
--rw-r--r--   0        0        0     8100 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/4hhh_frag.pdb
--rw-r--r--   0        0        0    54837 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/4oz7.pdb
--rw-r--r--   0        0        0   107503 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5cvz_final.pdb
--rw-r--r--   0        0        0    17472 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5e5z.mtz
--rw-r--r--   0        0        0    63576 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5i55.cif
--rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5i55_tiny.ccp4
--rw-r--r--   0        0        0    42363 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5moo_header.pdb
--rw-r--r--   0        0        0    26568 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5wkd.pdb
--rw-r--r--   0        0        0    17562 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/5wkd_phases.mtz.gz
--rw-r--r--   0        0        0    12689 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/HEM.cif
--rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/HEM.pdb
--rw-r--r--   0        0        0     8953 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/HEN.cif
--rw-r--r--   0        0        0     2539 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/SO3.cif
--rw-r--r--   0        0        0     2900 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/cif.cpp
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/common.py
--rw-r--r--   0        0        0     5695 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/disulf.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/ener_lib.cif
--rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/eol-test.cif
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/iota_yzx.ccp4.gz
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/list/mon_lib_list.cif
--rw-r--r--   0        0        0     6250 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/main.cpp
--rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/misc.cif
--rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/misc.json
--rw-r--r--   0        0        0    59158 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/mmcif_pdbx_v50_frag.dic
--rw-r--r--   0        0        0    17415 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/pdb1gdr.ent
--rw-r--r--   0        0        0    33045 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/r5wkdsf.ent
--rw-r--r--   0        0        0    30928 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/rnase_frag.pdb
--rw-r--r--   0        0        0     3828 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_align.py
--rwxr-xr-x   0        0        0    15957 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_cif.py
--rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_cif_json.py
--rwxr-xr-x   0        0        0     3696 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_elem.py
--rw-r--r--   0        0        0     3010 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_examples.py
--rw-r--r--   0        0        0     8050 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_grid.py
--rwxr-xr-x   0        0        0    13535 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_hkl.py
--rwxr-xr-x   0        0        0     2733 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_misc.py
--rw-r--r--   0        0        0    40179 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_mol.py
--rwxr-xr-x   0        0        0     5645 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_monlib.py
--rw-r--r--   0        0        0     5066 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_neighbor.py
--rwxr-xr-x   0        0        0     5626 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_prog.py
--rw-r--r--   0        0        0     6485 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_seq.py
--rwxr-xr-x   0        0        0     4063 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_sf.py
--rwxr-xr-x   0        0        0     1535 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_smallmol.py
--rw-r--r--   0        0        0    16490 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_symmetry.py
--rw-r--r--   0        0        0     5897 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_twin.py
--rw-r--r--   0        0        0    11311 2022-11-09 12:37:21.000000 gemmi-0.6.5/tests/test_unitcell.py
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/README
--rw-r--r--   0        0        0   268970 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/doctest.h
--rw-r--r--   0        0        0    47289 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/linalg.h
--rw-r--r--   0        0        0   102124 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/optionparser.h
--rw-r--r--   0        0        0    95912 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/sajson.h
--rw-r--r--   0        0        0    58248 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/stb_sprintf.h
--rw-r--r--   0        0        0     1002 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/LICENSE
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/NOTE
--rw-r--r--   0        0        0     4964 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/adler32.c
--rw-r--r--   0        0        0    31605 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/crc32.c
--rw-r--r--   0        0        0     6676 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/gzguts.h
--rw-r--r--   0        0        0    16270 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/gzlib.c
--rw-r--r--   0        0        0    19918 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/gzread.c
--rw-r--r--   0        0        0    12924 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inffast.c
--rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inffast.h
--rw-r--r--   0        0        0     6332 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inffixed.h
--rw-r--r--   0        0        0    55519 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inflate.c
--rw-r--r--   0        0        0     6683 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inflate.h
--rw-r--r--   0        0        0    13024 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inftrees.c
--rw-r--r--   0        0        0     2920 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/inftrees.h
--rw-r--r--   0        0        0    16500 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/zconf.h
--rw-r--r--   0        0        0    96829 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/zlib.h
--rw-r--r--   0        0        0     7179 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/zutil.c
--rw-r--r--   0        0        0     6677 2022-11-09 12:37:21.000000 gemmi-0.6.5/third_party/zlib/zutil.h
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 gemmi-0.6.5/tools/gemmi-config.cmake.in
--rw-r--r--   0        0        0     2254 2022-11-09 12:37:21.000000 gemmi-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    23336 2022-11-09 12:37:21.000000 gemmi-0.6.6/CMakeLists.txt
+-rw-r--r--   0        0        0    16726 2022-11-09 12:37:21.000000 gemmi-0.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 gemmi-0.6.6/README.md
+-rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/elem.cpp
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/mod.cpp
+-rw-r--r--   0        0        0     1926 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/niggli.cpp
+-rw-r--r--   0        0        0     5643 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/pdb.cpp
+-rw-r--r--   0        0        0     3563 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/resinfo.cpp
+-rw-r--r--   0        0        0     2434 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/round.cpp
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/smat33.cpp
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/stoi.cpp
+-rw-r--r--   0        0        0     2382 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/sym.cpp
+-rw-r--r--   0        0        0     1237 2022-11-09 12:37:21.000000 gemmi-0.6.6/benchmarks/writecif.cpp
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/cell.cpp
+-rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/cif_cc.cpp
+-rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/elem.cpp
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/maybegz.cpp
+-rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/mutate.cpp
+-rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/newmtz.cpp
+-rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/resinfo.cpp
+-rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/smcif.cpp
+-rw-r--r--   0        0        0     1237 2022-11-09 12:37:21.000000 gemmi-0.6.6/docs/code/sym.cpp
+-rwxr-xr-x   0        0        0     1175 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/aafreq.py
+-rw-r--r--   0        0        0     1233 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/auth_label.cpp
+-rwxr-xr-x   0        0        0     2378 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/ccd_gi.py
+-rwxr-xr-x   0        0        0     1266 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/ccd_subgraph.py
+-rw-r--r--   0        0        0     3161 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/check_conn.cpp
+-rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/check_symmetry.cpp
+-rw-r--r--   0        0        0      529 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/cif_i_sigi.py
+-rwxr-xr-x   0        0        0     1300 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/col_order.py
+-rwxr-xr-x   0        0        0      725 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/from_json.py
+-rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/hello.cpp
+-rwxr-xr-x   0        0        0      503 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/hello.py
+-rwxr-xr-x   0        0        0     1442 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/long_geom.py
+-rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/map2mtz.py
+-rw-r--r--   0        0        0     3822 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/maskcheck.py
+-rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/maskdiff.py
+-rwxr-xr-x   0        0        0     6844 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/matthews.py
+-rwxr-xr-x   0        0        0     1446 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/merge_mtz_mmcif.py
+-rwxr-xr-x   0        0        0     5359 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/monomers.py
+-rwxr-xr-x   0        0        0     1052 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/mtrix_iso.py
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/mtz_i_sigi.py
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/multiproc.py
+-rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/patterson_slice.py
+-rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/rama_gather.py
+-rwxr-xr-x   0        0        0     1182 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/rama_plot.py
+-rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/refln-stats.py
+-rwxr-xr-x   0        0        0      323 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/simple_search.py
+-rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/sub_ccd.py
+-rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/to_rdkit.py
+-rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/torsion_in_ring.cpp
+-rwxr-xr-x   0        0        0     4952 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/weight.py
+-rw-r--r--   0        0        0     7656 2022-11-09 12:37:21.000000 gemmi-0.6.6/examples/with_bgl.cpp
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/addends.hpp
+-rw-r--r--   0        0        0    11686 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/align.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/assembly.hpp
+-rw-r--r--   0        0        0     7455 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/asudata.hpp
+-rw-r--r--   0        0        0    11452 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/asumask.hpp
+-rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/atof.hpp
+-rw-r--r--   0        0        0     3810 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/atox.hpp
+-rw-r--r--   0        0        0     3983 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/bessel.hpp
+-rw-r--r--   0        0        0     7728 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/binner.hpp
+-rw-r--r--   0        0        0     4864 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/blob.hpp
+-rw-r--r--   0        0        0     3045 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/bond_idx.hpp
+-rw-r--r--   0        0        0    10347 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/c4322.hpp
+-rw-r--r--   0        0        0     7102 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/calculate.hpp
+-rw-r--r--   0        0        0    17346 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/ccp4.hpp
+-rw-r--r--   0        0        0    13372 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/cellred.hpp
+-rw-r--r--   0        0        0    24868 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/chemcomp.hpp
+-rw-r--r--   0        0        0     4707 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/chemcomp_xyz.hpp
+-rw-r--r--   0        0        0    14157 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/cif.hpp
+-rw-r--r--   0        0        0    21583 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/cif2mtz.hpp
+-rw-r--r--   0        0        0    37686 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/cifdoc.hpp
+-rw-r--r--   0        0        0     5036 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/contact.hpp
+-rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/crd.hpp
+-rw-r--r--   0        0        0     2570 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/ddl.hpp
+-rw-r--r--   0        0        0     7092 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/dencalc.hpp
+-rw-r--r--   0        0        0     7379 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/dirwalk.hpp
+-rw-r--r--   0        0        0     3246 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/ecalc.hpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/eig3.hpp
+-rw-r--r--   0        0        0    14917 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/elem.hpp
+-rw-r--r--   0        0        0     4526 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/enumstr.hpp
+-rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/fail.hpp
+-rw-r--r--   0        0        0     3964 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/fileutil.hpp
+-rw-r--r--   0        0        0     5176 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/floodfill.hpp
+-rw-r--r--   0        0        0     6424 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/formfact.hpp
+-rw-r--r--   0        0        0    13533 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/fourier.hpp
+-rw-r--r--   0        0        0   271931 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/fprime.hpp
+-rw-r--r--   0        0        0     2222 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/fstream.hpp
+-rw-r--r--   0        0        0    27792 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/grid.hpp
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/gz.hpp
+-rw-r--r--   0        0        0     4508 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/input.hpp
+-rw-r--r--   0        0        0     5206 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/intensit.hpp
+-rw-r--r--   0        0        0     1864 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/interop.hpp
+-rw-r--r--   0        0        0    23737 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/it92.hpp
+-rw-r--r--   0        0        0    10089 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/iterator.hpp
+-rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/json.hpp
+-rw-r--r--   0        0        0     9107 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/levmar.hpp
+-rw-r--r--   0        0        0     6763 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/linkhunt.hpp
+-rw-r--r--   0        0        0    15478 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/math.hpp
+-rw-r--r--   0        0        0    14030 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/metadata.hpp
+-rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mmcif.hpp
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mmcif_impl.hpp
+-rw-r--r--   0        0        0    11248 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mmdb.hpp
+-rw-r--r--   0        0        0     4432 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mmread.hpp
+-rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mmread_gz.hpp
+-rw-r--r--   0        0        0    39708 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/model.hpp
+-rw-r--r--   0        0        0    10806 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/modify.hpp
+-rw-r--r--   0        0        0    11631 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/monlib.hpp
+-rw-r--r--   0        0        0    37353 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mtz.hpp
+-rw-r--r--   0        0        0     5019 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/mtz2cif.hpp
+-rw-r--r--   0        0        0    13443 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/neighbor.hpp
+-rw-r--r--   0        0        0     2759 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/neutron92.hpp
+-rw-r--r--   0        0        0     1479 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/numb.hpp
+-rw-r--r--   0        0        0    28186 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/pdb.hpp
+-rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/pdb_id.hpp
+-rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/pirfasta.hpp
+-rw-r--r--   0        0        0     7921 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/polyheur.hpp
+-rw-r--r--   0        0        0    12909 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/qcp.hpp
+-rw-r--r--   0        0        0     1131 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/read_cif.hpp
+-rw-r--r--   0        0        0     1117 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/read_map.hpp
+-rw-r--r--   0        0        0     6753 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/recgrid.hpp
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/reciproc.hpp
+-rw-r--r--   0        0        0     8868 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/refln.hpp
+-rw-r--r--   0        0        0    25493 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/remarks.hpp
+-rw-r--r--   0        0        0     3682 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/resinfo.hpp
+-rw-r--r--   0        0        0     1016 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/riding_h.hpp
+-rw-r--r--   0        0        0    12086 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/scaling.hpp
+-rw-r--r--   0        0        0    16677 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/select.hpp
+-rw-r--r--   0        0        0    11324 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/seqalign.hpp
+-rw-r--r--   0        0        0     5125 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/seqid.hpp
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/seqtools.hpp
+-rw-r--r--   0        0        0     5753 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/serialize.hpp
+-rw-r--r--   0        0        0     5631 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/sfcalc.hpp
+-rw-r--r--   0        0        0     8126 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/small.hpp
+-rw-r--r--   0        0        0     7534 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/smcif.hpp
+-rw-r--r--   0        0        0    18280 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/solmask.hpp
+-rw-r--r--   0        0        0     4668 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/span.hpp
+-rw-r--r--   0        0        0     2368 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/sprintf.hpp
+-rw-r--r--   0        0        0     2761 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/stats.hpp
+-rw-r--r--   0        0        0    96467 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/symmetry.hpp
+-rw-r--r--   0        0        0   130919 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/fast_float.h
+-rw-r--r--   0        0        0   107015 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/pocketfft_hdronly.h
+-rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/LICENSE
+-rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/NOTES
+-rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
+-rw-r--r--   0        0        0      669 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
+-rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
+-rw-r--r--   0        0        0     1705 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
+-rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
+-rw-r--r--   0        0        0     1130 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
+-rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analyze.hpp
+-rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
+-rw-r--r--   0        0        0     1449 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/argv_input.hpp
+-rw-r--r--   0        0        0     3821 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/ascii.hpp
+-rw-r--r--   0        0        0     6426 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
+-rw-r--r--   0        0        0     1223 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_action.hpp
+-rw-r--r--   0        0        0     2647 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_action_and_state.hpp
+-rw-r--r--   0        0        0     3055 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_action_and_states.hpp
+-rw-r--r--   0        0        0     1085 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_control.hpp
+-rw-r--r--   0        0        0     2310 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_state.hpp
+-rw-r--r--   0        0        0     2695 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_states.hpp
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/config.hpp
+-rw-r--r--   0        0        0     1056 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
+-rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/disable_action.hpp
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/discard_input.hpp
+-rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/discard_input_on_failure.hpp
+-rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/discard_input_on_success.hpp
+-rw-r--r--   0        0        0     1037 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/enable_action.hpp
+-rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/eol.hpp
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/file_input.hpp
+-rw-r--r--   0        0        0     2073 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/input_error.hpp
+-rw-r--r--   0        0        0     1632 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/action.hpp
+-rw-r--r--   0        0        0     3120 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
+-rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
+-rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/always_false.hpp
+-rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/any.hpp
+-rw-r--r--   0        0        0     2794 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
+-rw-r--r--   0        0        0     2565 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
+-rw-r--r--   0        0        0     1229 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
+-rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/at.hpp
+-rw-r--r--   0        0        0      862 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
+-rw-r--r--   0        0        0      870 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bump.hpp
+-rw-r--r--   0        0        0     1573 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
+-rw-r--r--   0        0        0     1076 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
+-rw-r--r--   0        0        0     1643 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/control.hpp
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
+-rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
+-rw-r--r--   0        0        0     1395 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
+-rw-r--r--   0        0        0     1178 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
+-rw-r--r--   0        0        0     2078 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
+-rw-r--r--   0        0        0     1523 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
+-rw-r--r--   0        0        0     1003 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
+-rw-r--r--   0        0        0     7494 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
+-rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
+-rw-r--r--   0        0        0     1583 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
+-rw-r--r--   0        0        0     5796 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
+-rw-r--r--   0        0        0     2944 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
+-rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
+-rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
+-rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_mapper_posix.hpp
+-rw-r--r--   0        0        0     2012 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
+-rw-r--r--   0        0        0     3331 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
+-rw-r--r--   0        0        0      851 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
+-rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/has_match.hpp
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
+-rw-r--r--   0        0        0     3978 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
+-rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_missing.hpp
+-rw-r--r--   0        0        0     1687 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
+-rw-r--r--   0        0        0     1906 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
+-rw-r--r--   0        0        0     3323 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
+-rw-r--r--   0        0        0     1159 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
+-rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
+-rw-r--r--   0        0        0     1229 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
+-rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list.hpp
+-rw-r--r--   0        0        0      610 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
+-rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
+-rw-r--r--   0        0        0     2409 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/must.hpp
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
+-rw-r--r--   0        0        0     2301 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/one.hpp
+-rw-r--r--   0        0        0     1665 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
+-rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
+-rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_mask_uint.hpp
+-rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_mask_uint8.hpp
+-rw-r--r--   0        0        0     1500 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_uint.hpp
+-rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_uint8.hpp
+-rw-r--r--   0        0        0     1885 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
+-rw-r--r--   0        0        0     1366 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
+-rw-r--r--   0        0        0     3286 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
+-rw-r--r--   0        0        0     4224 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
+-rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
+-rw-r--r--   0        0        0     1642 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
+-rw-r--r--   0        0        0     1721 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/range.hpp
+-rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
+-rw-r--r--   0        0        0     1922 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/read_uint.hpp
+-rw-r--r--   0        0        0     3124 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rematch.hpp
+-rw-r--r--   0        0        0     2078 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
+-rw-r--r--   0        0        0     2899 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
+-rw-r--r--   0        0        0     1665 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
+-rw-r--r--   0        0        0     1172 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/require.hpp
+-rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
+-rw-r--r--   0        0        0     1395 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
+-rw-r--r--   0        0        0     2617 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
+-rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
+-rw-r--r--   0        0        0     1617 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/star.hpp
+-rw-r--r--   0        0        0      601 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
+-rw-r--r--   0        0        0     3024 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/state.hpp
+-rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/string.hpp
+-rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
+-rw-r--r--   0        0        0     2077 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
+-rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/until.hpp
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/istream_input.hpp
+-rw-r--r--   0        0        0     3388 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/match.hpp
+-rw-r--r--   0        0        0    12206 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/memory_input.hpp
+-rw-r--r--   0        0        0     2292 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
+-rw-r--r--   0        0        0     3358 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/normal.hpp
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/nothing.hpp
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/parse.hpp
+-rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/parse_error.hpp
+-rw-r--r--   0        0        0     1272 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/position.hpp
+-rw-r--r--   0        0        0     2317 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/read_input.hpp
+-rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/require_apply.hpp
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/require_apply0.hpp
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
+-rw-r--r--   0        0        0     5243 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/rules.hpp
+-rw-r--r--   0        0        0     2059 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/string_input.hpp
+-rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
+-rw-r--r--   0        0        0     4843 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/uint16.hpp
+-rw-r--r--   0        0        0     4843 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/uint32.hpp
+-rw-r--r--   0        0        0     4844 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/uint64.hpp
+-rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/uint8.hpp
+-rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf16.hpp
+-rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf32.hpp
+-rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf8.hpp
+-rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/version.hpp
+-rw-r--r--   0        0        0     1442 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tao/pegtl.hpp
+-rw-r--r--   0        0        0    19231 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/third_party/tinydir.h
+-rw-r--r--   0        0        0     3338 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/to_chemcomp.hpp
+-rw-r--r--   0        0        0     7774 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/to_cif.hpp
+-rw-r--r--   0        0        0     8862 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/to_json.hpp
+-rw-r--r--   0        0        0     2432 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/to_mmcif.hpp
+-rw-r--r--   0        0        0     2173 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/to_pdb.hpp
+-rw-r--r--   0        0        0    10545 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/topo.hpp
+-rw-r--r--   0        0        0    10321 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/twin.hpp
+-rw-r--r--   0        0        0    21785 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/unitcell.hpp
+-rw-r--r--   0        0        0     2433 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/utf.hpp
+-rw-r--r--   0        0        0     9845 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/util.hpp
+-rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/version.hpp
+-rw-r--r--   0        0        0    14985 2022-11-09 12:37:21.000000 gemmi-0.6.6/include/gemmi/xds_ascii.hpp
+-rw-r--r--   0        0        0    14912 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/align.cpp
+-rw-r--r--   0        0        0     7789 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/blobs.cpp
+-rw-r--r--   0        0        0     3586 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/cif2json.cpp
+-rw-r--r--   0        0        0    13306 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/cif2mtz.cpp
+-rw-r--r--   0        0        0     5070 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/cifdiff.cpp
+-rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/cifmod.h
+-rw-r--r--   0        0        0     8280 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/contact.cpp
+-rw-r--r--   0        0        0    10512 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/contents.cpp
+-rw-r--r--   0        0        0    21241 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/convert.cpp
+-rw-r--r--   0        0        0     5609 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/crd.cpp
+-rw-r--r--   0        0        0     5579 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/ecalc.cpp
+-rw-r--r--   0        0        0     2257 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/fprime.cpp
+-rw-r--r--   0        0        0    19996 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/grep.cpp
+-rw-r--r--   0        0        0     6305 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/h.cpp
+-rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/histogram.h
+-rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/json2cif.cpp
+-rw-r--r--   0        0        0     6541 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/main.cpp
+-rw-r--r--   0        0        0    10826 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/map.cpp
+-rw-r--r--   0        0        0     5467 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/map2sf.cpp
+-rw-r--r--   0        0        0     8999 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mapcoef.cpp
+-rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mapcoef.h
+-rw-r--r--   0        0        0     6315 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mask.cpp
+-rw-r--r--   0        0        0    12277 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/merge.cpp
+-rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mixmtz.cpp
+-rw-r--r--   0        0        0     9067 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mondiff.cpp
+-rw-r--r--   0        0        0     3369 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/monlib_opt.cpp
+-rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/monlib_opt.h
+-rw-r--r--   0        0        0    23653 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mtz.cpp
+-rw-r--r--   0        0        0    14549 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/mtz2cif.cpp
+-rw-r--r--   0        0        0    10921 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/options.cpp
+-rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/options.h
+-rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/reindex.cpp
+-rw-r--r--   0        0        0    13552 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/residues.cpp
+-rw-r--r--   0        0        0    11471 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/rmsz.cpp
+-rw-r--r--   0        0        0     3857 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/sf2map.cpp
+-rw-r--r--   0        0        0    35977 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/sfcalc.cpp
+-rw-r--r--   0        0        0     4962 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/sg.cpp
+-rw-r--r--   0        0        0    11892 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/tags.cpp
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/timer.h
+-rw-r--r--   0        0        0    10932 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/validate.cpp
+-rw-r--r--   0        0        0    11777 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/validate_mon.cpp
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/validate_mon.h
+-rw-r--r--   0        0        0    14342 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/wcn.cpp
+-rw-r--r--   0        0        0    11556 2022-11-09 12:37:21.000000 gemmi-0.6.6/prog/xds2mtz.cpp
+-rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 gemmi-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     4500 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/align.cpp
+-rw-r--r--   0        0        0      327 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/arrvec.h
+-rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/ccp4.cpp
+-rw-r--r--   0        0        0     8517 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/chemcomp.cpp
+-rw-r--r--   0        0        0    20454 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/cif.cpp
+-rw-r--r--   0        0        0     3157 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/common.h
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/custom.cpp
+-rw-r--r--   0        0        0     5949 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/elem.cpp
+-rw-r--r--   0        0        0     6741 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/gemmi.cpp
+-rw-r--r--   0        0        0    12804 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/grid.cpp
+-rw-r--r--   0        0        0    18024 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/hkl.cpp
+-rw-r--r--   0        0        0    17514 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/meta.cpp
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/meta.h
+-rw-r--r--   0        0        0      571 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/miller_a.h
+-rw-r--r--   0        0        0    27924 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/mol.cpp
+-rw-r--r--   0        0        0     5756 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/monlib.cpp
+-rw-r--r--   0        0        0    17059 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/mtz.cpp
+-rw-r--r--   0        0        0     8016 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/read.cpp
+-rw-r--r--   0        0        0     9555 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/recgrid.cpp
+-rw-r--r--   0        0        0     2128 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/scaling.cpp
+-rw-r--r--   0        0        0     6733 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/search.cpp
+-rw-r--r--   0        0        0     3771 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/sf.cpp
+-rw-r--r--   0        0        0    11680 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/sym.cpp
+-rw-r--r--   0        0        0     7642 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/topo.cpp
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/tostr.hpp
+-rw-r--r--   0        0        0    17574 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/unitcell.cpp
+-rw-r--r--   0        0        0     4725 2022-11-09 12:37:21.000000 gemmi-0.6.6/python/write.cpp
+-rw-r--r--   0        0        0     2279 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/align.cpp
+-rw-r--r--   0        0        0    17883 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/assembly.cpp
+-rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/calculate.cpp
+-rw-r--r--   0        0        0    25390 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/crd.cpp
+-rw-r--r--   0        0        0    23898 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/ddl.cpp
+-rw-r--r--   0        0        0     5904 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/eig3.cpp
+-rw-r--r--   0        0        0     5068 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/gz.cpp
+-rw-r--r--   0        0        0    15562 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/intensit.cpp
+-rw-r--r--   0        0        0     4700 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/json.cpp
+-rw-r--r--   0        0        0    38768 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/mmcif.cpp
+-rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/mmread_gz.cpp
+-rw-r--r--   0        0        0    22129 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/monlib.cpp
+-rw-r--r--   0        0        0    16192 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/mtz.cpp
+-rw-r--r--   0        0        0    37691 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/mtz2cif.cpp
+-rw-r--r--   0        0        0    15225 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/polyheur.cpp
+-rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/read_cif.cpp
+-rw-r--r--   0        0        0    25715 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/resinfo.cpp
+-rw-r--r--   0        0        0    17805 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/riding_h.cpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/sprintf.cpp
+-rw-r--r--   0        0        0    55441 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/to_mmcif.cpp
+-rw-r--r--   0        0        0    27806 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/to_pdb.cpp
+-rw-r--r--   0        0        0    44087 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/topo.cpp
+-rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 gemmi-0.6.6/src/xds_ascii.cpp
+-rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1011031.cif
+-rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1lzh.pdb.gz
+-rw-r--r--   0        0        0    71037 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1orc.pdb
+-rw-r--r--   0        0        0    26819 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1pfe.cif.gz
+-rw-r--r--   0        0        0   112575 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1pfe.json
+-rw-r--r--   0        0        0     2812 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/1pfe_asu.msk.gz
+-rw-r--r--   0        0        0     7328 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/2013551.cif
+-rw-r--r--   0        0        0    13833 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/2242624.cif
+-rw-r--r--   0        0        0     3328 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/2242624.hkl
+-rw-r--r--   0        0        0    19473 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/3dg1_final.cif
+-rw-r--r--   0        0        0    12742 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/3wup.json.gz
+-rw-r--r--   0        0        0    36221 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/4003024.cif
+-rw-r--r--   0        0        0     4319 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/4aap-sf-subset.cif
+-rw-r--r--   0        0        0     8100 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/4hhh_frag.pdb
+-rw-r--r--   0        0        0    54837 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/4oz7.pdb
+-rw-r--r--   0        0        0   107503 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5cvz_final.pdb
+-rw-r--r--   0        0        0    17472 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5e5z.mtz
+-rw-r--r--   0        0        0    63576 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5i55.cif
+-rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5i55_tiny.ccp4
+-rw-r--r--   0        0        0    42363 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5moo_header.pdb
+-rw-r--r--   0        0        0    26568 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5wkd.pdb
+-rw-r--r--   0        0        0    17562 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/5wkd_phases.mtz.gz
+-rw-r--r--   0        0        0    12689 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/HEM.cif
+-rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/HEM.pdb
+-rw-r--r--   0        0        0     8953 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/HEN.cif
+-rw-r--r--   0        0        0     2539 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/SO3.cif
+-rw-r--r--   0        0        0     2900 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/cif.cpp
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/common.py
+-rw-r--r--   0        0        0     5695 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/disulf.cpp
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/ener_lib.cif
+-rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/eol-test.cif
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/iota_yzx.ccp4.gz
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/list/mon_lib_list.cif
+-rw-r--r--   0        0        0     6250 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/main.cpp
+-rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/misc.cif
+-rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/misc.json
+-rw-r--r--   0        0        0    59158 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/mmcif_pdbx_v50_frag.dic
+-rw-r--r--   0        0        0    17415 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/pdb1gdr.ent
+-rw-r--r--   0        0        0    33045 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/r5wkdsf.ent
+-rw-r--r--   0        0        0    30928 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/rnase_frag.pdb
+-rw-r--r--   0        0        0     3828 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_align.py
+-rwxr-xr-x   0        0        0    15957 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_cif.py
+-rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_cif_json.py
+-rwxr-xr-x   0        0        0     3758 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_elem.py
+-rw-r--r--   0        0        0     3010 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_examples.py
+-rw-r--r--   0        0        0     9224 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_grid.py
+-rwxr-xr-x   0        0        0    13535 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_hkl.py
+-rwxr-xr-x   0        0        0     2733 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_misc.py
+-rw-r--r--   0        0        0    40215 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_mol.py
+-rwxr-xr-x   0        0        0     5645 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_monlib.py
+-rw-r--r--   0        0        0     5066 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_neighbor.py
+-rwxr-xr-x   0        0        0     5626 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_prog.py
+-rw-r--r--   0        0        0     6485 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_seq.py
+-rwxr-xr-x   0        0        0     4050 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_sf.py
+-rwxr-xr-x   0        0        0     1535 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_smallmol.py
+-rw-r--r--   0        0        0    19872 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_symmetry.py
+-rw-r--r--   0        0        0     5897 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_twin.py
+-rw-r--r--   0        0        0    11311 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/test_unitcell.py
+-rw-r--r--   0        0        0     3352 2022-11-09 12:37:21.000000 gemmi-0.6.6/tests/windowsh.cpp
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/README
+-rw-r--r--   0        0        0   321728 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/doctest.h
+-rw-r--r--   0        0        0    47289 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/linalg.h
+-rw-r--r--   0        0        0   102124 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/optionparser.h
+-rw-r--r--   0        0        0    95912 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/sajson.h
+-rw-r--r--   0        0        0    58248 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/stb_sprintf.h
+-rw-r--r--   0        0        0     1002 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/LICENSE
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/NOTE
+-rw-r--r--   0        0        0     4964 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/adler32.c
+-rw-r--r--   0        0        0    31605 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/crc32.c
+-rw-r--r--   0        0        0     6676 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/gzguts.h
+-rw-r--r--   0        0        0    16270 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/gzlib.c
+-rw-r--r--   0        0        0    19918 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/gzread.c
+-rw-r--r--   0        0        0    12924 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inffast.c
+-rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inffast.h
+-rw-r--r--   0        0        0     6332 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inffixed.h
+-rw-r--r--   0        0        0    55519 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inflate.c
+-rw-r--r--   0        0        0     6683 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inflate.h
+-rw-r--r--   0        0        0    13024 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inftrees.c
+-rw-r--r--   0        0        0     2920 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/inftrees.h
+-rw-r--r--   0        0        0    16500 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/zconf.h
+-rw-r--r--   0        0        0    96829 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/zlib.h
+-rw-r--r--   0        0        0     7179 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/zutil.c
+-rw-r--r--   0        0        0     6677 2022-11-09 12:37:21.000000 gemmi-0.6.6/third_party/zlib/zutil.h
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 gemmi-0.6.6/tools/gemmi-config.cmake.in
+-rw-r--r--   0        0        0     2254 2022-11-09 12:37:21.000000 gemmi-0.6.6/PKG-INFO
```

### Comparing `gemmi-0.6.5/CMakeLists.txt` & `gemmi-0.6.6/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
       "Install path for gemmi CMake files")
 endif()
 option(STRIP_BINARY "Strip symbols from program" OFF)
 
 # uncomment to show compilation times for each compilation unit
 #set_property(GLOBAL PROPERTY RULE_LAUNCH_COMPILE "\"${CMAKE_COMMAND}\" -E time")
 
-if (DEFINED ENV{FC} OR CMAKE_Fortran_COMPILER)
+if ((DEFINED ENV{FC} AND NOT "$ENV{FC}" STREQUAL "") OR CMAKE_Fortran_COMPILER)
   set(USE_FORTRAN ON CACHE BOOL "Build Fortran bindings" FORCE)
 endif()
 
 if (DEFINED Python_EXECUTABLE)
   set(USE_PYTHON ON CACHE BOOL "Build Python bindings" FORCE)
 endif()
 
@@ -79,17 +79,17 @@
 endif()
 
 if (INFO)
   set(GEMMI_VERSION_INFO ${INFO} CACHE STRING "Extra text for gemmi -V" FORCE)
 endif()
 
 if (USE_FORTRAN)
-   message(STATUS "Currently, Fortran bindings are not built by cmake.")
-   message(STATUS "They can be built by running make in fortran directory.")
-  enable_language(Fortran)
+  message(STATUS "Currently, Fortran bindings are not built by cmake.")
+  message(STATUS "They can be built by running make in fortran/.")
+  #enable_language(Fortran)
 else()
   #message(STATUS "Skipping Fortran bindings. Add -D USE_FORTRAN=1 to build them.")
 endif()
 
 if (DEFINED ENV{EXTRA_WFLAGS})
   set(EXTRA_WARNINGS ON CACHE BOOL "Set extra warning flags" FORCE)
 endif()
@@ -356,15 +356,15 @@
 endif()
 
 ### tests and examples ###
 
 #add_executable(c_test EXCLUDE_FROM_ALL fortran/c_test.c)
 #target_link_libraries(c_test PRIVATE cgemmi)
 
-add_executable(cpptest EXCLUDE_FROM_ALL tests/main.cpp tests/cif.cpp)
+add_executable(cpptest EXCLUDE_FROM_ALL tests/main.cpp tests/cif.cpp tests/windowsh.cpp)
 target_compile_definitions(cpptest PRIVATE USE_STD_SNPRINTF=1)
 target_link_libraries(cpptest PRIVATE gemmi_headers)
 target_include_directories(cpptest PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/third_party")
 
 add_executable(hello EXCLUDE_FROM_ALL examples/hello.cpp)
 target_link_libraries(hello PRIVATE gemmi_headers)
 add_executable(doc_example EXCLUDE_FROM_ALL
@@ -442,14 +442,18 @@
   message(STATUS "The python module will be built.")
   # CMake >=3.18 has subcomponent Development.Module, scikit-build-core also has it
   if (${CMAKE_VERSION} VERSION_LESS 3.18 AND NOT SKBUILD)
     find_package(Python ${PYTHON_VERSION} REQUIRED COMPONENTS Interpreter Development)
   else()
     find_package(Python ${PYTHON_VERSION} REQUIRED COMPONENTS Interpreter Development.Module)
   endif()
+  # pybind11 macros use PYTHON_EXECUTABLE
+  if (DEFINED Python_EXECUTABLE AND NOT DEFINED PYTHON_EXECUTABLE)
+    set(PYTHON_EXECUTABLE "${Python_EXECUTABLE}")
+  endif()
   if (EXISTS "${CMAKE_HOME_DIRECTORY}/pybind11")
     message(STATUS "Using ${CMAKE_HOME_DIRECTORY}/pybind11 (internal copy).")
     add_subdirectory(pybind11)
   else()
     # use pybind11-config (if available) to determine pybind11_DIR
     execute_process(COMMAND pybind11-config --cmakedir OUTPUT_VARIABLE pybind11_DIR)
     string(STRIP "${pybind11_DIR}" pybind11_DIR)
```

### Comparing `gemmi-0.6.5/LICENSE.txt` & `gemmi-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/README.md` & `gemmi-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/elem.cpp` & `gemmi-0.6.6/benchmarks/elem.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/mod.cpp` & `gemmi-0.6.6/benchmarks/mod.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/niggli.cpp` & `gemmi-0.6.6/benchmarks/niggli.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/pdb.cpp` & `gemmi-0.6.6/benchmarks/pdb.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/resinfo.cpp` & `gemmi-0.6.6/benchmarks/resinfo.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/round.cpp` & `gemmi-0.6.6/benchmarks/round.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/smat33.cpp` & `gemmi-0.6.6/benchmarks/smat33.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/stoi.cpp` & `gemmi-0.6.6/benchmarks/stoi.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/sym.cpp` & `gemmi-0.6.6/benchmarks/sym.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/benchmarks/writecif.cpp` & `gemmi-0.6.6/benchmarks/writecif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/docs/code/cif_cc.cpp` & `gemmi-0.6.6/docs/code/cif_cc.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/docs/code/newmtz.cpp` & `gemmi-0.6.6/docs/code/newmtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/docs/code/sym.cpp` & `gemmi-0.6.6/docs/code/sym.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/aafreq.py` & `gemmi-0.6.6/examples/aafreq.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/auth_label.cpp` & `gemmi-0.6.6/examples/auth_label.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/ccd_gi.py` & `gemmi-0.6.6/examples/ccd_gi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/ccd_subgraph.py` & `gemmi-0.6.6/examples/ccd_subgraph.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/check_conn.cpp` & `gemmi-0.6.6/examples/check_conn.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/check_symmetry.cpp` & `gemmi-0.6.6/examples/check_symmetry.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/cif_i_sigi.py` & `gemmi-0.6.6/examples/cif_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/col_order.py` & `gemmi-0.6.6/examples/col_order.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/from_json.py` & `gemmi-0.6.6/examples/from_json.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/hello.cpp` & `gemmi-0.6.6/examples/hello.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/long_geom.py` & `gemmi-0.6.6/examples/long_geom.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/map2mtz.py` & `gemmi-0.6.6/examples/map2mtz.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/maskcheck.py` & `gemmi-0.6.6/examples/maskcheck.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/maskdiff.py` & `gemmi-0.6.6/examples/maskdiff.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/matthews.py` & `gemmi-0.6.6/examples/matthews.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/merge_mtz_mmcif.py` & `gemmi-0.6.6/examples/merge_mtz_mmcif.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/monomers.py` & `gemmi-0.6.6/examples/monomers.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/mtrix_iso.py` & `gemmi-0.6.6/examples/mtrix_iso.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/mtz_i_sigi.py` & `gemmi-0.6.6/examples/mtz_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/multiproc.py` & `gemmi-0.6.6/examples/multiproc.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/patterson_slice.py` & `gemmi-0.6.6/examples/patterson_slice.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/rama_gather.py` & `gemmi-0.6.6/examples/rama_gather.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/rama_plot.py` & `gemmi-0.6.6/examples/rama_plot.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/refln-stats.py` & `gemmi-0.6.6/examples/refln-stats.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/sub_ccd.py` & `gemmi-0.6.6/examples/sub_ccd.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/torsion_in_ring.cpp` & `gemmi-0.6.6/examples/torsion_in_ring.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/weight.py` & `gemmi-0.6.6/examples/weight.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/examples/with_bgl.cpp` & `gemmi-0.6.6/examples/with_bgl.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/addends.hpp` & `gemmi-0.6.6/include/gemmi/addends.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/align.hpp` & `gemmi-0.6.6/include/gemmi/align.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/assembly.hpp` & `gemmi-0.6.6/include/gemmi/assembly.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/asudata.hpp` & `gemmi-0.6.6/include/gemmi/asudata.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/asumask.hpp` & `gemmi-0.6.6/include/gemmi/asumask.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/atof.hpp` & `gemmi-0.6.6/include/gemmi/atof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/atox.hpp` & `gemmi-0.6.6/include/gemmi/atox.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/bessel.hpp` & `gemmi-0.6.6/include/gemmi/bessel.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/binner.hpp` & `gemmi-0.6.6/include/gemmi/binner.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/blob.hpp` & `gemmi-0.6.6/include/gemmi/blob.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/bond_idx.hpp` & `gemmi-0.6.6/include/gemmi/bond_idx.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/c4322.hpp` & `gemmi-0.6.6/include/gemmi/c4322.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/calculate.hpp` & `gemmi-0.6.6/include/gemmi/calculate.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 //
 // Calculate various properties of the model.
 
 #ifndef GEMMI_CALCULATE_HPP_
 #define GEMMI_CALCULATE_HPP_
 
 #include <array>
+#include <algorithm>  // for std::min, std::minmax
 #include "model.hpp"
 
 namespace gemmi {
 
 template<class T> bool has_hydrogen(const T& obj) {
   for (const auto& child : obj.children())
     if (has_hydrogen(child))
@@ -56,14 +57,49 @@
   return total;
 }
 template<> inline CenterOfMass calculate_center_of_mass(const Atom& atom) {
   double w_mass = atom.element.weight() * atom.occ;
   return CenterOfMass{Position(atom.pos * w_mass), w_mass};
 }
 
+template<class T> std::pair<float,float> calculate_b_iso_range(const T& obj) {
+  std::pair<float, float> range{INFINITY, -INFINITY};
+  for (const auto& child : obj.children()) {
+    auto r = calculate_b_iso_range(child);
+    range.first = std::min(range.first, r.first);
+    range.second = std::max(range.second, r.second);
+  }
+  return range;
+}
+template<> inline std::pair<float,float> calculate_b_iso_range(const Atom& atom) {
+  return {atom.b_iso, atom.b_iso};
+}
+
+/// uses min/max eigenvalues of Baniso, or Biso if B-factor is isotropic
+inline std::pair<double, double> calculate_b_aniso_range(const Model& model) {
+  std::pair<double, double> range{INFINITY, -INFINITY};
+  for (const Chain& chain : model.chains)
+    for (const Residue& residue : chain.residues)
+      for (const Atom& atom : residue.atoms) {
+        if (atom.occ == 0)
+          continue;
+        if (atom.aniso.nonzero()) {
+          std::array<double,3> eig = atom.aniso.calculate_eigenvalues();
+          auto u = std::minmax({eig[0], eig[1], eig[2]});
+          range.first = std::min(range.first, u.first * u_to_b());
+          range.second = std::max(range.second, u.second * u_to_b());
+        } else {
+          range.first = std::min(range.first, (double) atom.b_iso);
+          range.second = std::max(range.second, (double) atom.b_iso);
+        }
+      }
+  return range;
+}
+
+
 template<class T> void expand_box(const T& obj, Box<Position>& box) {
   for (const auto& child : obj.children())
     expand_box(child, box);
 }
 template<> inline void expand_box(const Atom& atom, Box<Position>& box) {
   box.extend(atom.pos);
 }
@@ -74,14 +110,16 @@
   expand_box(st, box);
   if (margin != 0.)
     box.add_margin(margin);
   return box;
 }
 
 inline Box<Fractional> calculate_fractional_box(const Structure& st, double margin=0.) {
+  if (!st.cell.is_crystal())
+    fail("calculate_fractional_box(): Structure has no unit cell for fractionalization");
   Box<Fractional> box;
   for (const Model& model : st.models)
     for (const Chain& chain : model.chains)
       for (const Residue& res : chain.residues)
         for (const Atom& atom : res.atoms)
           box.extend(st.cell.fractionalize(atom.pos));
   if (margin != 0.)
```

### Comparing `gemmi-0.6.5/include/gemmi/ccp4.hpp` & `gemmi-0.6.6/include/gemmi/ccp4.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/cellred.hpp` & `gemmi-0.6.6/include/gemmi/cellred.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/chemcomp.hpp` & `gemmi-0.6.6/include/gemmi/chemcomp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/chemcomp_xyz.hpp` & `gemmi-0.6.6/include/gemmi/chemcomp_xyz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/cif.hpp` & `gemmi-0.6.6/include/gemmi/cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/cif2mtz.hpp` & `gemmi-0.6.6/include/gemmi/cif2mtz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/cifdoc.hpp` & `gemmi-0.6.6/include/gemmi/cifdoc.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,16 @@
 
   Column find_column(const std::string& tag) {
     return column_at_pos(find_column_position(tag));
   }
 
   void erase();
 
-  void convert_pair_to_loop();
+  /// if it's pairs, convert it to loop
+  void ensure_loop();
 
   // It is not a proper input iterator, but just enough for using range-for.
   struct iterator {
     Table& parent;
     int index;
     void operator++() { index++; }
     bool operator==(const iterator& o) const { return index == o.index; }
@@ -743,29 +744,28 @@
 
 template <typename T> void Table::append_row(T new_values) {
   if (!ok())
     fail("append_row(): table not found");
   if (new_values.size() != width())
     fail("append_row(): wrong row length");
   if (!loop_item)
-    convert_pair_to_loop();
+    fail("append_row(): data is not in loop, call ensure_loop() first");
   Loop& loop = loop_item->loop;
   size_t cur_size = loop.values.size();
   loop.values.resize(cur_size + loop.width(), ".");
   int n = 0;
   for (const auto& value : new_values)
     loop.values[cur_size + positions[n++]] = value;
 }
 
 inline void Table::remove_rows(int start, int end) {
   if (!ok())
     // this function is used mostly through remove_row()
     fail("remove_row(): table not found");
-  if (!loop_item)
-    convert_pair_to_loop();
+  ensure_loop();  // should we fail instead if we have pairs?
   Loop& loop = loop_item->loop;
   size_t start_pos = start * loop.width();
   size_t end_pos = end * loop.width();
   if (start_pos >= end_pos || end_pos > loop.values.size())
     throw std::out_of_range("remove_row(): invalid index");
   loop.values.erase(loop.values.begin() + start_pos,
                     loop.values.begin() + end_pos);
@@ -785,26 +785,28 @@
     for (int pos : positions)
       if (pos >= 0)
         bloc.items[pos].erase();
   }
   positions.clear();
 }
 
-inline void Table::convert_pair_to_loop() {
-  assert(loop_item == nullptr);
+inline void Table::ensure_loop() {
+  if (loop_item)
+    return;
   Item new_item(LoopArg{});
   new_item.loop.tags.resize(positions.size());
   new_item.loop.values.resize(positions.size());
+  loop_item = &bloc.items.at(positions[0]);
   for (size_t i = 0; i != positions.size(); ++i) {
     Item& item = bloc.items[positions[i]];
     new_item.loop.tags[i].swap(item.pair[0]);
     new_item.loop.values[i].swap(item.pair[1]);
     item.erase();
+    positions[i] = i;
   }
-  loop_item = &bloc.items.at(positions[0]);
   loop_item->set_value(std::move(new_item));
 }
 
 inline Block::Block(const std::string& name_) : name(name_) {}
 inline Block::Block() {}
 
 inline const Item* Block::find_pair_item(const std::string& tag) const {
```

### Comparing `gemmi-0.6.5/include/gemmi/contact.hpp` & `gemmi-0.6.6/include/gemmi/contact.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/ddl.hpp` & `gemmi-0.6.6/include/gemmi/ddl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/dencalc.hpp` & `gemmi-0.6.6/include/gemmi/dencalc.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #define GEMMI_DENCALC_HPP_
 
 #include <cassert>
 #include "addends.hpp"  // for Addends
 #include "formfact.hpp" // for ExpSum
 #include "grid.hpp"     // for Grid
 #include "model.hpp"    // for Structure, ...
+#include "calculate.hpp" // for calculate_b_aniso_range
 
 namespace gemmi {
 
 template<int N, typename Real>
 Real determine_cutoff_radius(Real x1, const ExpSum<N, Real>& precal, Real cutoff_level) {
   Real y1, dy;
   std::tie(y1, dy) = precal.calculate_with_derivative(x1);
@@ -62,35 +63,18 @@
 
 // approximated radius of electron density (IT92) above cutoff=1e-5 for C
 template <typename Real>
 Real it92_radius_approx(Real b) {
   return (8.5f + 0.075f * b) / (2.4f + 0.0045f * b);
 }
 
-inline double get_minimum_b(const Model& model) {
-  double b_min = 1000.;
-  for (const Chain& chain : model.chains)
-    for (const Residue& residue : chain.residues)
-      for (const Atom& atom : residue.atoms) {
-        if (atom.occ == 0) continue;
-        double b = atom.b_iso;
-        if (atom.aniso.nonzero()) {
-          std::array<double,3> eig = atom.aniso.calculate_eigenvalues();
-          b = std::min(std::min(eig[0], eig[1]), eig[2]) * u_to_b();
-        }
-        if (b < b_min)
-          b_min = b;
-      }
-  return b_min;
-}
-
 // Usual usage:
 // - set d_min and optionally also other parameters,
 // - set addends to f' values for your wavelength (see fprime.hpp)
-// - use set_grid_cell_and_spacegroup() to set grid's unit cell and space group
+// - use grid.setup_from() to set grid's unit cell and space group
 // - check that Table has SF coefficients for all elements that are to be used
 // - call put_model_density_on_grid()
 // - do FFT using transform_map_to_f_phi()
 // - if blur is used, multiply the SF by reciprocal_space_multiplier()
 template <typename Table, typename GReal>
 struct DensityCalculator {
   // GReal = type of grid; CReal = type of coefficients in Table
@@ -104,20 +88,22 @@
   size_t atoms_added = 0;
   size_t density_computations = 0;
 #endif
   Addends addends;
 
   double requested_grid_spacing() const { return d_min / (2 * rate); }
 
-  void set_refmac_compatible_blur(const Model& model) {
+  void set_refmac_compatible_blur(const Model& model, bool allow_negative=false) {
     double spacing = requested_grid_spacing();
     if (spacing <= 0)
       spacing = std::min(std::min(grid.spacing[0], grid.spacing[1]), grid.spacing[2]);
-    double b_min = get_minimum_b(model);
-    blur = std::max(u_to_b() / 1.1 * sq(spacing) - b_min, 0.);
+    double b_min = calculate_b_aniso_range(model).first;
+    blur = u_to_b() / 1.1 * sq(spacing) - b_min;
+    if (!allow_negative && blur < 0)
+      blur = 0.;
   }
 
   // pre: check if Table::has(atom.element)
   void add_atom_density_to_grid(const Atom& atom) {
     Element el = atom.element;
     do_add_atom_density_to_grid(atom, Table::get(el, atom.charge), addends.get(el));
   }
@@ -198,17 +184,17 @@
 
   void put_model_density_on_grid(const Model& model) {
     initialize_grid();
     add_model_density_to_grid(model);
     grid.symmetrize_sum();
   }
 
+  // deprecated, use directly grid.setup_from(st)
   void set_grid_cell_and_spacegroup(const Structure& st) {
-    grid.unit_cell = st.cell;
-    grid.spacegroup = st.find_spacegroup();
+    grid.setup_from(st);
   }
 
   // The argument is 1/d^2 - as outputted by unit_cell.calculate_1_d2(hkl).
   double reciprocal_space_multiplier(double inv_d2) const {
     return std::exp(blur * 0.25 * inv_d2);
   }
```

### Comparing `gemmi-0.6.5/include/gemmi/dirwalk.hpp` & `gemmi-0.6.6/include/gemmi/dirwalk.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/ecalc.hpp` & `gemmi-0.6.6/include/gemmi/ecalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/elem.hpp` & `gemmi-0.6.6/include/gemmi/elem.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,20 @@
   };
   static_assert(table[static_cast<int>(El::D)] == false, "Hmm");
   static_assert(sizeof(table) / sizeof(table[0]) ==
                 static_cast<int>(El::END) + 1, "Hmm");
   return table[static_cast<int>(el)];
 }
 
+// Helper function, not public. Replaces =='s in static_assert comparisons
+// that were reported to fail on i386 / GCC 13: the numbers were compared
+// as 80-bit, the tabulated value was double-rounded, the literal was not.
+constexpr bool ce_almost_eq(double x, double y) {
+  return -1e-6 < x-y && x-y < 1e-6;
+}
 
 inline double molecular_weight(El el) {
   static constexpr double weights[] = {
     /*X*/ 1.0,
     /*H*/ 1.00794, /*He*/ 4.0026,
     /*Li*/ 6.941, /*Be*/ 9.012182, /*B*/ 10.811, /*C*/ 12.0107,
     /*N*/ 14.0067, /*O*/ 15.9994, /*F*/ 18.998403, /*Ne*/ 20.1797,
@@ -93,15 +99,15 @@
     /*U*/ 238.029, /*Np*/ 237, /*Pu*/ 244, /*Am*/ 243, /*Cm*/ 247,
     /*Bk*/ 247, /*Cf*/ 251, /*Es*/ 252, /*Fm*/ 257, /*Md*/ 258,
     /*No*/ 259, /*Lr*/ 262, /*Rf*/ 267, /*Db*/ 268, /*Sg*/ 271,
     /*Bh*/ 272, /*Hs*/ 270, /*Mt*/ 276, /*Ds*/ 281, /*Rg*/ 280, /*Cn*/ 285,
     /*Nh*/ 284, /*Fl*/ 289, /*Mc*/ 288, /*Lv*/ 293, /*Ts*/ 294, /*Og*/ 294,
     /*D*/ 2.0141, /*END*/ 0.0
   };
-  static_assert(weights[static_cast<int>(El::D)] == 2.0141, "Hmm");
+  static_assert(ce_almost_eq(weights[static_cast<int>(El::D)], 2.0141), "Hmm");
   static_assert(sizeof(weights) / sizeof(weights[0]) ==
                 static_cast<int>(El::END) + 1, "Hmm");
   return weights[static_cast<int>(el)];
 }
 
 // Covalent radius data from https://en.wikipedia.org/wiki/Covalent_radius
 // which in turn comes from
@@ -134,15 +140,15 @@
     /*Bk*/ 1.68f, /*Cf*/ 1.68f, /*Es*/ 1.65f, /*Fm*/ 1.67f, /*Md*/ 1.73f,
     /*No*/ 1.76f, /*Lr*/ 1.61f, /*Rf*/ 1.57f, /*Db*/ 1.49f, /*Sg*/ 1.43f,
     /*Bh*/ 1.41f, /*Hs*/ 1.34f, /*Mt*/ 1.29f, /*Ds*/ 1.28f, /*Rg*/ 1.21f,
     /*Cn*/ 1.22f, /*Nh*/ 1.50f, /*Fl*/ 1.50f, /*Mc*/ 1.50f, /*Lv*/ 1.50f,
     /*Ts*/ 1.50f, /*Og*/ 1.50f,
     /*D*/ 0.31f, /*END*/ 0.0f
   };
-  static_assert(radii[static_cast<int>(El::D)] == 0.31f, "Hmm");
+  static_assert(ce_almost_eq(radii[static_cast<int>(El::D)], 0.31f), "Hmm");
   static_assert(sizeof(radii) / sizeof(radii[0]) ==
                 static_cast<int>(El::END) + 1, "Hmm");
   return radii[static_cast<int>(el)];
 }
 
 // Van der Waals radii. Taken from:
 // https://en.wikipedia.org/wiki/Atomic_radii_of_the_elements_(data_page)
@@ -179,15 +185,15 @@
     /*Bk*/ 1.64f, /*Cf*/ 1.63f, /*Es*/ 1.62f, /*Fm*/ 1.61f, /*Md*/ 1.60f,
     /*No*/ 1.59f, /*Lr*/ 1.58f, /*Rf*/ 1.00f, /*Db*/ 1.00f, /*Sg*/ 1.00f,
     /*Bh*/ 1.00f, /*Hs*/ 1.00f, /*Mt*/ 1.00f, /*Ds*/ 1.00f, /*Rg*/ 1.00f,
     /*Cn*/ 1.00f, /*Nh*/ 1.00f, /*Fl*/ 1.00f, /*Mc*/ 1.00f, /*Lv*/ 1.00f,
     /*Ts*/ 1.00f, /*Og*/ 1.00f,
     /*D*/  1.20f, /*END*/0.f
   };
-  static_assert(radii[static_cast<int>(El::D)] == 1.2f, "Hmm");
+  static_assert(ce_almost_eq(radii[static_cast<int>(El::D)], 1.2f), "Hmm");
   static_assert(sizeof(radii) / sizeof(radii[0]) ==
                 static_cast<int>(El::END) + 1, "Hmm");
   return radii[static_cast<int>(el)];
 }
 
 
 typedef const char elname_t[3];
```

### Comparing `gemmi-0.6.5/include/gemmi/enumstr.hpp` & `gemmi-0.6.6/include/gemmi/enumstr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/fail.hpp` & `gemmi-0.6.6/include/gemmi/fail.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/fileutil.hpp` & `gemmi-0.6.6/include/gemmi/fileutil.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -30,35 +30,45 @@
         basename.compare(basename.length() - len, len, ext, len) == 0)
       basename.resize(basename.length() - len);
   }
   return basename;
 }
 
 // file operations
-typedef std::unique_ptr<std::FILE, decltype(&std::fclose)> fileptr_t;
+
+/// deleter for fileptr_t
+struct needs_fclose {
+  bool use_fclose;
+  void operator()(std::FILE* f) const noexcept {
+    if (use_fclose)
+      std::fclose(f);
+  }
+};
+
+typedef std::unique_ptr<std::FILE, needs_fclose> fileptr_t;
 
 inline fileptr_t file_open(const char* path, const char* mode) {
   std::FILE* file;
 #if defined(_WIN32) && !defined(GEMMI_USE_FOPEN)
   std::wstring wpath = UTF8_to_wchar(path);
   std::wstring wmode = UTF8_to_wchar(mode);
   if ((file = ::_wfopen(wpath.c_str(), wmode.c_str())) == nullptr)
 #else
   if ((file = std::fopen(path, mode)) == nullptr)
 #endif
     sys_fail(std::string("Failed to open ") + path +
              (*mode == 'w' ? " for writing" : ""));
-  return fileptr_t(file, &std::fclose);
+  return fileptr_t(file, needs_fclose{true});
 }
 
 // helper function for treating "-" as stdin or stdout
 inline fileptr_t file_open_or(const char* path, const char* mode,
                               std::FILE* dash_stream) {
   if (path[0] == '-' && path[1] == '\0')
-    return fileptr_t(dash_stream, [](std::FILE*) { return 0; });
+    return fileptr_t(dash_stream, needs_fclose{false});
   return file_open(path, mode);
 }
 
 inline std::size_t file_size(std::FILE* f, const std::string& path) {
   if (std::fseek(f, 0, SEEK_END) != 0)
     sys_fail(path + ": fseek failed");
   long length = std::ftell(f);
```

### Comparing `gemmi-0.6.5/include/gemmi/floodfill.hpp` & `gemmi-0.6.6/include/gemmi/floodfill.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/formfact.hpp` & `gemmi-0.6.6/include/gemmi/formfact.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/fourier.hpp` & `gemmi-0.6.6/include/gemmi/fourier.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/fprime.hpp` & `gemmi-0.6.6/include/gemmi/fprime.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/fstream.hpp` & `gemmi-0.6.6/include/gemmi/fstream.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/grid.hpp` & `gemmi-0.6.6/include/gemmi/grid.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -72,41 +72,49 @@
       sign = -sign;
       ++k;
     }
   }
   return n;
 }
 
-inline std::array<int, 3> good_grid_size(const std::array<double, 3>& limit,
+inline std::array<int, 3> good_grid_size(std::array<double, 3> limit,
                                          GridSizeRounding rounding,
                                          const SpaceGroup* sg) {
   std::array<int, 3> m = {{0, 0, 0}};
   GroupOps gops;
   if (sg)
     gops = sg->operations();
   std::array<int, 3> sg_fac = gops.find_grid_factors();
-  for (int i = 0; i != 3; ++i) {
+
+  // If two dimensions are symmetry-related, they must have the same size.
+  // Otherwise, if two dimensions are almost equal, the same grid size
+  // looks better and is preferred.
+  for (int i = 1; i < 3; ++i)
     for (int j = 0; j < i; ++j)
-      if (std::fabs(limit[i] - limit[j]) < 0.5 && sg_fac[i] == sg_fac[j]) {
-        m[i] = m[j];
-        break;
+      if (gops.are_directions_symmetry_related(i, j) ||
+          (std::fabs(limit[i] - limit[j]) < 0.5 && sg_fac[i] == sg_fac[j])) {
+        if (rounding == GridSizeRounding::Up)
+          limit[j] = std::max(limit[i], limit[j]);
+        else if (rounding == GridSizeRounding::Down)
+          limit[j] = std::min(limit[i], limit[j]);
+        else // GridSizeRounding::Nearest
+          limit[j] = 0.5 * (limit[i] + limit[j]);
+        sg_fac[i] = -j;  // mark the dimension with higher index
       }
-    if (m[i] == 0) {
-      // having sizes always even simplifies things
-      int f = sg_fac[i] % 2 == 0 ? sg_fac[i] : 2 * sg_fac[i];
-      int n = round_with_small_factorization(limit[i] / f, rounding);
-      m[i] = n * f;
+
+  for (int i = 0; i < 3; ++i) {
+    int f = sg_fac[i];
+    if (f > 0) {  // need to calculate the size
+      if (f % 2 != 0)
+        f *= 2; // always use even sizes - it simplifies things
+      m[i] = f * round_with_small_factorization(limit[i] / f, rounding);
+    } else { // the same size was already calculated
+      m[i] = m[-f];
     }
   }
-  for (int i = 1; i != 3; ++i)
-    for (int j = 0; j != i; ++j)
-      if (gops.are_directions_symmetry_related(i, j) && m[i] != m[j]) {
-        bool denser = rounding != GridSizeRounding::Down;
-        m[i] = m[j] = (denser ? std::max(m[i], m[j]) : std::min(m[i], m[j]));
-      }
   return m;
 }
 
 struct GridOp {
   Op scaled_op;
 
   std::array<int, 3> apply(int u, int v, int w) const {
@@ -362,18 +370,19 @@
 
   void set_unit_cell(const UnitCell& cell) {
     unit_cell = cell;
     calculate_spacing();
   }
 
   template<typename S>
-  void setup_from(const S& st, double approx_spacing) {
+  void setup_from(const S& st, double approx_spacing=0) {
     spacegroup = st.find_spacegroup();
     unit_cell = st.cell;
-    set_size_from_spacing(approx_spacing, GridSizeRounding::Up);
+    if (approx_spacing > 0)
+      set_size_from_spacing(approx_spacing, GridSizeRounding::Up);
   }
 
   /// Returns index in data array for (u,v,w). Safe but slower than index_q().
   size_t index_s(int u, int v, int w) const {
     this->check_not_empty();
     return this->index_q(modulo(u, nu), modulo(v, nv), modulo(w, nw));
   }
```

### Comparing `gemmi-0.6.5/include/gemmi/gz.hpp` & `gemmi-0.6.6/include/gemmi/gz.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #include <string>
 #include "fail.hpp"     // GEMMI_DLL
 #include "input.hpp"    // BasicInput
 #include "util.hpp"     // iends_with
 
 namespace gemmi {
 
+GEMMI_DLL extern const char* const zlib_description;
+
 GEMMI_DLL size_t estimate_uncompressed_size(const std::string& path);
 
 // the same interface as FileStream and MemoryStream
 struct GEMMI_DLL GzStream {
   void* f;  // implementation detail
   char* gets(char* line, int size);
   int getc();
```

### Comparing `gemmi-0.6.5/include/gemmi/input.hpp` & `gemmi-0.6.6/include/gemmi/input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/intensit.hpp` & `gemmi-0.6.6/include/gemmi/intensit.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/interop.hpp` & `gemmi-0.6.6/include/gemmi/interop.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/it92.hpp` & `gemmi-0.6.6/include/gemmi/it92.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
   {El::Np, +6},
   {El::Pu, +3},
   {El::Pu, +4},
   {El::Pu, +6},
 };
 
 template<class Real>
-bool IT92<Real>::ignore_charge = false;
+bool IT92<Real>::ignore_charge = true;
 
 #if defined(__GNUC__) && __GNUC__-0 > 4
 #pragma GCC diagnostic pop
 #endif
 
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/iterator.hpp` & `gemmi-0.6.6/include/gemmi/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/json.hpp` & `gemmi-0.6.6/include/gemmi/json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/levmar.hpp` & `gemmi-0.6.6/include/gemmi/levmar.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 /// Gauss-Jordan elimination with partial pivoting.
 ///
 /// A * x = b
 ///
 /// a is n x n matrix (in vector)
 /// b is vector of length n,
 /// This function returns vector x[] in b[], and 1-matrix in a[].
-inline void jordan_solve(std::vector<double>& a, std::vector<double>& b) {
-  assert(a.size() == b.size() * b.size());
-  int n = (int) b.size();
+inline void jordan_solve(double* a, double* b, int n) {
   for (int i = 0; i < n; i++) {
     // looking for a pivot element
     int maxnr = -1;
     double amax = 0;
     for (int j = i; j < n; j++) {
       double aji = std::fabs(a[n * j + i]);
       if (aji > amax) {
@@ -66,14 +64,19 @@
         for (int j = i; j < n; j++)
           a[k * n + j] -= a[i * n + j] * d;
         b[k] -= b[i] * d;
       }
   }
 }
 
+inline void jordan_solve(std::vector<double>& a, std::vector<double>& b) {
+  assert(a.size() == b.size() * b.size());
+  jordan_solve(a.data(), b.data(), (int)b.size());
+}
+
 
 #ifdef GEMMI_DEBUG_LEVMAR
 inline void debug_print(const std::string& name, std::vector<double> &a) {
   fprintf(stderr, " %s:", name.c_str());
   for (double& x : a)
     fprintf(stderr, " %g", x);
   fprintf(stderr, "\n");
```

### Comparing `gemmi-0.6.5/include/gemmi/linkhunt.hpp` & `gemmi-0.6.6/include/gemmi/linkhunt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/math.hpp` & `gemmi-0.6.6/include/gemmi/math.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 
 constexpr double deg(double angle) { return 180.0 / pi() * angle; }
 constexpr double rad(double angle) { return pi() / 180.0 * angle; }
 
 constexpr float sq(float x) { return x * x; }
 constexpr double sq(double x) { return x * x; }
 
+inline double log_cosh(double x) {
+  // cosh(x) would overflow for x > 710.5, so we calculate:
+  // ln(cosh(x)) = ln(e^x + e^-x) - ln(2) = ln(e^x * (1 + e^-2x)) - ln(2)
+  x = std::abs(x);
+  return x - std::log(2) + std::log1p(std::exp(-2 * x));
+}
+
 inline int iround(double d) { return static_cast<int>(std::round(d)); }
 
 inline double angle_abs_diff(double a, double b, double full=360.0) {
   double d = std::fabs(a - b);
   if (d > full)
     d -= std::floor(d / full) * full;
   return std::min(d, full - d);
```

### Comparing `gemmi-0.6.5/include/gemmi/metadata.hpp` & `gemmi-0.6.6/include/gemmi/metadata.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   enum Classification {
     DataCollection, DataExtraction, DataProcessing, DataReduction,
     DataScaling, ModelBuilding, Phasing, Refinement, Unspecified
   };
   std::string name;
   std::string version;
   std::string date;
+  std::string description;
   Classification classification = Unspecified;
 };
 
 // Information from REMARK 200/230 is significantly expanded in PDBx/mmCIF.
 // These remarks corresponds to data across 12 mmCIF categories
 // including categories _exptl, _reflns, _exptl_crystal, _diffrn and others.
 // _exptl and _reflns seem to be 1:1. Usually we have one experiment (_exptl),
@@ -229,14 +230,16 @@
     SeqId db_begin, db_end;
     SeqId::OptionalNum label_seq_begin, label_seq_end;
   };
   std::string name;
   std::vector<std::string> subchains;
   EntityType entity_type = EntityType::Unknown;
   PolymerType polymer_type = PolymerType::Unknown;
+  // In case of microheterogeneity, PDB SEQRES has only the first residue name.
+  bool reflects_microhetero = false;
   std::vector<DbRef> dbrefs;
   /// List of SIFTS Uniprot ACs referenced by SiftsUnpResidue::acc_index
   std::vector<std::string> sifts_unp_acc;
   /// SEQRES or entity_poly_seq with microheterogeneity as comma-separated names
   std::vector<std::string> full_sequence;
 
   Entity() = default;
```

### Comparing `gemmi-0.6.5/include/gemmi/mmcif.hpp` & `gemmi-0.6.6/include/gemmi/mmcif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/mmcif_impl.hpp` & `gemmi-0.6.6/include/gemmi/mmcif_impl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/mmdb.hpp` & `gemmi-0.6.6/include/gemmi/mmdb.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       mat[i][j] = tr.mat[i][j];
     vec[i] = tr.vec.at(i);
   }
 }
 
 template<int N>
 void strcpy_to_mmdb(char (&dest)[N], const std::string& src) {
-  if (src.size() >= N)
+  if (src.size() + 1 >= N)
     fail("This string is too long: " + src);
   std::memcpy(dest, src.c_str(), src.size() + 1);
 }
 
 inline void set_seqid_in_mmdb(int* seqnum, mmdb::InsCode& icode, SeqId seqid) {
   *seqnum = *seqid.num;
   icode[0] = seqid.icode;
@@ -71,15 +71,15 @@
     std::string line = rtrim_str(s);
     manager->PutPDBString(line.c_str());
   }
 
   for (int imodel = 0; imodel < (int) st.models.size(); ++imodel) {
     const Model& model = st.models[imodel];
     mmdb::Model* model2 = mmdb::newModel();
-    model2->SetMMDBManager(manager, imodel);
+    manager->AddModel(model2);
 
     for (const Chain& chain : model.chains) {
       mmdb::Chain* chain2 = model2->CreateChain(chain.name.c_str());
       for (const Residue& res : chain.residues) {
         const char icode[2] = {res.seqid.icode, '\0'};
         mmdb::Residue* res2 = chain2->GetResidueCreate(res.name.c_str(),
                                                        *res.seqid.num,
@@ -116,15 +116,14 @@
           mmdb::Atom* atom2 = mmdb::newAtom();
           atom2->MakeTer();
           atom2->serNum = res.atoms.back().serial + 1;
           res2->AddAtom(atom2);
         }
       }
     }
-    manager->AddModel(model2);
     manager->PutCell(st.cell.a, st.cell.b, st.cell.c,
                      st.cell.alpha, st.cell.beta, st.cell.gamma, 1);
     manager->SetSpaceGroup(st.spacegroup_hm.c_str());
     mmdb::Cryst* cryst = manager->GetCrystData();
     auto z = st.info.find("_cell.Z_PDB");
     if (z != st.info.end() && !z->second.empty()) {
       cryst->Z = std::atoi(z->second.c_str());
```

### Comparing `gemmi-0.6.5/include/gemmi/mmread.hpp` & `gemmi-0.6.6/include/gemmi/mmread.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -53,36 +53,46 @@
     int n = check_chemcomp_block_number(doc);
     if (n != -1)
       return make_structure_from_chemcomp_block(doc.blocks[n]);
   }
   return make_structure(std::move(doc), save_doc);
 }
 
-inline Structure read_structure_from_char_array(char* data, size_t size,
-                                                const std::string& path,
-                                                cif::Document* save_doc=nullptr) {
+// when reading JSON, the input buffer is changed (as an optimization)
+inline Structure read_structure_from_memory(char* data, size_t size,
+                                            const std::string& path,
+                                            CoorFormat format=CoorFormat::Unknown,
+                                            cif::Document* save_doc=nullptr) {
   if (save_doc)
     save_doc->clear();
-  CoorFormat format = coor_format_from_content(data, data + size);
+  if (format == CoorFormat::Unknown || format == CoorFormat::Detect)
+    format = coor_format_from_content(data, data + size);
   if (format == CoorFormat::Pdb)
     return read_pdb_from_memory(data, size, path);
   if (format == CoorFormat::Mmcif)
     return make_structure_from_doc(cif::read_memory(data, size, path.c_str()),
                                    true, save_doc);
   if (format == CoorFormat::Mmjson)
     return make_structure(cif::read_mmjson_insitu(data, size, path), save_doc);
   fail("wrong format of coordinate file " + path);
 }
 
+// deprecated
+inline Structure read_structure_from_char_array(char* data, size_t size,
+                                                const std::string& path,
+                                                cif::Document* save_doc=nullptr) {
+  return read_structure_from_memory(data, size, path, CoorFormat::Unknown, save_doc);
+}
+
 template<typename T>
 Structure read_structure(T&& input, CoorFormat format=CoorFormat::Unknown,
                          cif::Document* save_doc=nullptr) {
   if (format == CoorFormat::Detect) {
     CharArray mem = read_into_buffer(input);
-    return read_structure_from_char_array(mem.data(), mem.size(), input.path(), save_doc);
+    return read_structure_from_memory(mem.data(), mem.size(), input.path(), format, save_doc);
   }
   if (save_doc)
     save_doc->clear();
   if (format == CoorFormat::Unknown)
     format = coor_format_from_ext(input.basepath());
   switch (format) {
     case CoorFormat::Pdb:
```

### Comparing `gemmi-0.6.5/include/gemmi/mmread_gz.hpp` & `gemmi-0.6.6/include/gemmi/mmread_gz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/model.hpp` & `gemmi-0.6.6/include/gemmi/model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -921,14 +921,15 @@
 }
 inline const Entity* find_entity_of_subchain(const std::string& subchain_id,
                                              const std::vector<Entity>& entities) {
   return find_entity_of_subchain(subchain_id, const_cast<std::vector<Entity>&>(entities));
 }
 
 struct Structure {
+  static const char* what() { return "Structure"; }
   std::string name;
   UnitCell cell;
   std::string spacegroup_hm;  // usually pdb symbol, cf. SpaceGroup::pdb_name()
   std::vector<Model> models;
   std::vector<NcsOp> ncs;
   std::vector<Entity> entities;
   std::vector<Connection> connections;
```

### Comparing `gemmi-0.6.5/include/gemmi/modify.hpp` & `gemmi-0.6.6/include/gemmi/modify.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,19 @@
 }
 inline void assign_serial_numbers(Structure& st, bool numbered_ter=false) {
   for (Model& model : st.models)
     assign_serial_numbers(model, numbered_ter);
 }
 
 
+/// Helper function for processing (usually: changing) names and numbers
+/// in AtomAddress instances in metadata:
+/// Connection, CisPep, Helix, Sheet::Strand.
+/// Other fields are not updated here, in particular: ModRes, Entity::DbRef,
+/// Entity::full_sequence, TlsGroup::Selection.
 template<typename Func>
 void process_addresses(Structure& st, Func func) {
   for (Connection& con : st.connections) {
     func(con.partner1);
     func(con.partner2);
   }
   for (CisPep& cispep : st.cispeps) {
@@ -130,32 +135,77 @@
       func(strand.start);
       func(strand.end);
       func(strand.hbond_atom2);
       func(strand.hbond_atom1);
     }
 }
 
+/// Takes func(const std::string& chain_name, gemmi::SeqId& seqid).
+/// It doesn't process Entity::DbRef::seq_begin/seq_end (b/c there is no
+/// single corresponding chain name).
+template<typename Func>
+void process_sequence_ids(Structure& st, Func func) {
+  process_addresses(st, [&](AtomAddress& aa) { func(aa.chain_name, aa.res_id.seqid); });
+  for (ModRes& modres : st.mod_residues)
+    func(modres.chain_name, modres.res_id.seqid);
+  for (RefinementInfo& ri : st.meta.refinement)
+    for (TlsGroup& tls : ri.tls_groups)
+      for (TlsGroup::Selection& sel : tls.selections) {
+        func(sel.chain, sel.res_begin);
+        func(sel.chain, sel.res_end);
+      }
+}
 
 inline void rename_chain(Structure& st, const std::string& old_name,
                                         const std::string& new_name) {
-  process_addresses(st, [&](AtomAddress& aa) {
-      if (aa.chain_name == old_name)
-        aa.chain_name = new_name;
-  });
+  auto update = [&](std::string& name) {
+    if (name == old_name)
+      name = new_name;
+  };
+  process_addresses(st, [&](AtomAddress& aa) { update(aa.chain_name); });
+  for (ModRes& modres : st.mod_residues)
+    update(modres.chain_name);
   for (RefinementInfo& ri : st.meta.refinement)
     for (TlsGroup& tls : ri.tls_groups)
       for (TlsGroup::Selection& sel : tls.selections)
-        if (sel.chain == old_name)
-          sel.chain = new_name;
+        update(sel.chain);
   for (Model& model : st.models)
     for (Chain& chain : model.chains)
-      if (chain.name == old_name)
-        chain.name = new_name;
+      update(chain.name);
 }
 
+inline void rename_residues(Structure& st, const std::string& old_name,
+                                           const std::string& new_name) {
+  auto update = [&](ResidueId& rid) {
+    if (rid.name == old_name)
+      rid.name = new_name;
+  };
+  process_addresses(st, [&](AtomAddress& aa) { update(aa.res_id); });
+  for (ModRes& modres : st.mod_residues)
+    update(modres.res_id);
+  for (Entity& ent : st.entities)
+    for (std::string& mon_ids : ent.full_sequence)
+      for (size_t start = 0;;) {
+        size_t end = mon_ids.find(',', start);
+        if (mon_ids.compare(start, end-start, old_name) == 0) {
+          mon_ids.replace(start, end-start, new_name);
+          if (end != std::string::npos)
+            end = start + new_name.size();
+        }
+        if (end == std::string::npos)
+          break;
+        start = end + 1;
+      }
+  for (Model& model : st.models)
+    for (Chain& chain : model.chains)
+      for (Residue& res : chain.residues)
+        update(res);
+}
+
+
 inline void rename_atom_names(Structure& st, const std::string& res_name,
                               const std::map<std::string, std::string>& old_new) {
   auto update = [&old_new](std::string& name) {
     auto it = old_new.find(name);
     if (it != old_new.end())
       name = it->second;
   };
```

### Comparing `gemmi-0.6.5/include/gemmi/monlib.hpp` & `gemmi-0.6.6/include/gemmi/monlib.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,14 @@
   }
   std::map<std::string, Atom> atoms; // type->Atom
   std::multimap<std::string, Bond> bonds; // atom_type_1->Bond
 };
 
 struct GEMMI_DLL MonLib {
   std::string monomer_dir;
-  std::string lib_version;
   EnerLib ener_lib;
   std::map<std::string, ChemComp> monomers;
   std::map<std::string, ChemLink> links;
   std::map<std::string, ChemMod> modifications;
   std::map<std::string, ChemComp::Group> cc_groups;
 
   const ChemLink* get_link(const std::string& link_id) const {
@@ -253,19 +252,15 @@
     }
     return path;
   }
 
   void read_monomer_doc(const cif::Document& doc);
 
   void read_monomer_cif(const std::string& path_, read_cif_func read_cif) {
-    const cif::Document& doc = (*read_cif)(path_);
-    if (!doc.blocks.empty() && doc.blocks[0].name == "lib")
-      if (const std::string* ver = doc.blocks[0].find_value("_lib.version"))
-        lib_version = *ver;
-    read_monomer_doc(doc);
+    read_monomer_doc((*read_cif)(path_));
   }
 
   void set_monomer_dir(const std::string& monomer_dir_) {
     monomer_dir = monomer_dir_;
     if (!monomer_dir.empty() && monomer_dir.back() != '/' && monomer_dir.back() != '\\')
       monomer_dir += '/';
   }
@@ -276,15 +271,20 @@
                         const std::vector<std::string>& resnames,
                         read_cif_func read_cif,
                         std::string* error=nullptr) {
     if (monomer_dir_.empty())
       fail("read_monomer_lib: monomer_dir not specified.");
     set_monomer_dir(monomer_dir_);
 
-    read_monomer_cif(monomer_dir + "list/mon_lib_list.cif", read_cif);
+    // Only recent versions of CCP4 Monomer Library have links_and_mods.cif
+    try {
+      read_monomer_cif(monomer_dir + "links_and_mods.cif", read_cif);
+    } catch (std::system_error&) {
+      read_monomer_cif(monomer_dir + "list/mon_lib_list.cif", read_cif);
+    }
     ener_lib.read((*read_cif)(monomer_dir + "ener_lib.cif"));
 
     bool ok = true;
     for (const std::string& name : resnames) {
       if (monomers.find(name) != monomers.end())
         continue;
       try {
```

### Comparing `gemmi-0.6.5/include/gemmi/mtz.hpp` & `gemmi-0.6.6/include/gemmi/mtz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/mtz2cif.hpp` & `gemmi-0.6.6/include/gemmi/mtz2cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/neighbor.hpp` & `gemmi-0.6.6/include/gemmi/neighbor.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/neutron92.hpp` & `gemmi-0.6.6/include/gemmi/neutron92.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/numb.hpp` & `gemmi-0.6.6/include/gemmi/numb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/pdb.hpp` & `gemmi-0.6.6/include/gemmi/pdb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/pdb_id.hpp` & `gemmi-0.6.6/include/gemmi/pdb_id.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,25 @@
 #include <cstdlib>   // getenv
 #include <string>
 #include "fail.hpp"  // for fail
 #include "util.hpp"  // for to_lower
 
 namespace gemmi {
 
+inline bool all_alnums(const char* p) {
+  for (;;++p)
+    if (!std::isalnum(*p))
+      return *p == '\0';
+  unreachable();
+}
+
 inline bool is_pdb_code(const std::string& str) {
-  return (str.length() == 4 && std::isdigit(str[0]) && std::isalnum(str[1])
-                            && std::isalnum(str[2]) && std::isalnum(str[3]))
+  return (str.length() == 4 && std::isdigit(str[0]) && all_alnums(&str[1]))
       || (str.length() == 12 && str.compare(0, 4, "pdb_") == 0
-                             && std::isdigit(str[4]));
+                             && std::isdigit(str[4]) && all_alnums(&str[5]));
 }
 
 /// Call it after checking the code with gemmi::is_pdb_code(code).
 /// The convention for $PDB_DIR is the same as in BioJava, see the docs.
 /// \par type is the requested file type: 'M' for mmCIF or 'P' for PDB, 'S' for SF-mmCIF.
 inline std::string expand_pdb_code_to_path(const std::string& code, char type,
                                            bool throw_if_unset=false) {
```

### Comparing `gemmi-0.6.5/include/gemmi/pirfasta.hpp` & `gemmi-0.6.6/include/gemmi/pirfasta.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/polyheur.hpp` & `gemmi-0.6.6/include/gemmi/polyheur.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,28 @@
 inline void setup_entities(Structure& st) {
   add_entity_types(st, /*overwrite=*/false);
   assign_subchains(st, /*force=*/false);
   ensure_entities(st);
   deduplicate_entities(st);
 }
 
+/// Determine ATOM/HETATM record type, based on Residue::entity_type
+GEMMI_DLL char recommended_het_flag(const Residue& res);
+/// R = recommended_het_flag(), other valid values are A, H and '\0'
+template<class T> void assign_het_flags(T& obj, char flag='R') {
+  for (auto& child : obj.children())
+    assign_het_flags(child, flag);
+}
+template<> inline void assign_het_flags(Residue& res, char flag) {
+  flag &= ~0x20; // uppercase letters, ' ' -> \0
+  if (flag != 'R' && flag != '\0' && flag != 'A' && flag != 'H')
+    fail("assign_het_flags(): the only allowed values are A, H, ' ' and R");
+  res.het_flag = flag == '?' ? recommended_het_flag(res) : flag;
+}
+
 // Remove waters. It may leave empty chains.
 template<class T> void remove_waters(T& obj) {
   for (auto& child : obj.children())
     remove_waters(child);
 }
 template<> inline void remove_waters(Chain& ch) {
   vector_remove_if(ch.residues,
@@ -164,43 +178,24 @@
       if (res.entity_type == EntityType::Unknown)
         fail("remove_ligands_and_waters(): missing entity_type in chain ", ch.name);
       return res.entity_type != EntityType::Polymer;
   });
 }
 
 // Trim to alanine. Returns true if trimmed, false if it's (likely) not AA.
-inline bool trim_to_alanine(Residue& res) {
-  static const std::pair<std::string, El> ala_atoms[6] = {
-    {"N", El::N}, {"CA", El::C}, {"C", El::C}, {"O", El::O}, {"CB", El::C},
-    {"OXT", El::O}
-  };
-  if (res.get_ca() == nullptr)
-    return false;
-  vector_remove_if(res.atoms, [](const Atom& a) {
-      for (const auto& name_el : ala_atoms)
-        if (a.name == name_el.first && a.element == name_el.second)
-          return false;
-      return true;
-  });
-  return true;
-}
+GEMMI_DLL bool trim_to_alanine(Residue& res);
 
 inline void trim_to_alanine(Chain& chain) {
   for (Residue& res : chain.residues)
     trim_to_alanine(res);
 }
 
 // Functions for switching between long (>3 chars) residue names (CCD codes)
 // and shortened ones that are compatible with the PDB format.
-GEMMI_DLL
-void change_ccd_code(Structure& st, const std::string& old, const std::string& new_);
-
 GEMMI_DLL void shorten_ccd_codes(Structure& st);
+GEMMI_DLL void restore_full_ccd_codes(Structure& st);
 
-inline void restore_full_ccd_codes(Structure& st) {
-  for (const auto& item : st.shortened_ccd_codes)
-    change_ccd_code(st, item.second, item.first);
-  st.shortened_ccd_codes.clear();
-}
+/// Modifies Entity::full_sequence. Uses only the first chain for each Entity.
+GEMMI_DLL void add_microhetero_to_sequences(Structure& st, bool overwrite=false);
 
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/qcp.hpp` & `gemmi-0.6.6/include/gemmi/qcp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/read_cif.hpp` & `gemmi-0.6.6/include/gemmi/read_cif.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 #include "input.hpp"  // for CharArray
 
 namespace gemmi {
 
 GEMMI_DLL cif::Document read_cif_gz(const std::string& path);
 GEMMI_DLL cif::Document read_mmjson_gz(const std::string& path);
 GEMMI_DLL CharArray read_into_buffer_gz(const std::string& path);
-GEMMI_DLL cif::Document read_cif_from_buffer(const CharArray& buffer, const char* name);
+GEMMI_DLL cif::Document read_cif_from_memory(const char* data, size_t size, const char* name);
 GEMMI_DLL cif::Document read_first_block_gz(const std::string& path, size_t limit);
 
 inline cif::Document read_cif_or_mmjson_gz(const std::string& path) {
   if (giends_with(path, "json") || giends_with(path, "js"))
     return read_mmjson_gz(path);
   return read_cif_gz(path);
 }
 
+// deprecated
+inline cif::Document read_cif_from_buffer(const CharArray& buffer, const char* name) {
+  return read_cif_from_memory(buffer.data(), buffer.size(), name);
+}
+
 } // namespace gemmi
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/read_map.hpp` & `gemmi-0.6.6/include/gemmi/read_map.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/recgrid.hpp` & `gemmi-0.6.6/include/gemmi/recgrid.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,18 @@
   template <typename R=T>
   AsuData<R> prepare_asu_data(double dmin=0, double unblur=0,
                               bool with_000=false, bool with_sys_abs=false,
                               bool mott_bethe=false) {
     AsuData<R> asu_data;
     if (this->axis_order == AxisOrder::ZYX)
       fail("get_asu_values(): ZYX order is not supported yet");
+    // Why "- 1" below? To skip the value at Nyquist frequency (±n/2).
+    // For even lengths of DFT (real -> reciprocal space) the resulting
+    // h=+nu/2 and h=-nu/2 are both represented by one (strictly real) value.
+    // The grid should be big enough so that these values are not needed.
     int max_h = (this->nu - 1) / 2;
     int max_k = (this->nv - 1) / 2;
     int max_l = half_l ? this->nw - 1 : (this->nw - 1) / 2;
     double max_1_d2 = 0.;
     if (dmin != 0.) {
       max_1_d2 = 1. / (dmin * dmin);
       Miller lim = this->unit_cell.get_hkl_limits(dmin);
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gemmi-0.6.5/include/gemmi/reciproc.hpp` & `gemmi-0.6.6/include/gemmi/reciproc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/refln.hpp` & `gemmi-0.6.6/include/gemmi/refln.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/remarks.hpp` & `gemmi-0.6.6/include/gemmi/remarks.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/resinfo.hpp` & `gemmi-0.6.6/include/gemmi/resinfo.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/riding_h.hpp` & `gemmi-0.6.6/include/gemmi/riding_h.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/scaling.hpp` & `gemmi-0.6.6/include/gemmi/scaling.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -207,24 +207,29 @@
     return k_sol * std::exp(-b_sol * stol2);
   }
 
   double get_overall_scale_factor(const Miller& hkl) const {
     return k_overall * std::exp(-0.25 * b_star.r_u_r(hkl));
   }
 
-  // quick linear fit (ignoring sigma) to get initial parameters
+  std::complex<Real> get_fcalc(const Point& p) const {
+    if (!use_solvent)
+      return p.fcmol;
+    return p.fcmol + (Real)get_solvent_scale(p.stol2) * p.fmask;
+  }
+
+  // quick linear fit (ignoring sigma) to get initial k_overall and isotropic B
   void fit_isotropic_b_approximately() {
     double sx = 0, sy = 0, sxx = 0, sxy = 0;
     int n = 0;
     for (const Point& p : points) {
       if (p.fobs < 1 || p.fobs < p.sigma)  // skip weak reflections
         continue;
+      double fcalc = std::abs(get_fcalc(p));
       double x = p.stol2;
-      double fcalc = std::abs(use_solvent ? p.fcmol + (Real)get_solvent_scale(x) * p.fmask
-                                          : p.fcmol);
       double y = std::log(static_cast<float>(p.fobs / fcalc));
       sx += x;
       sy += y;
       sxx += x * x;
       sxy += x * y;
       n += 1;
     }
@@ -233,26 +238,74 @@
     double slope = (n * sxy - sx * sy) / (n * sxx - sx * sx);
     double intercept = (sy - slope * sx) / n;
     double b_iso = -slope;
     k_overall = std::exp(intercept);
     set_b_overall({b_iso, b_iso, b_iso, 0, 0, 0});
   }
 
-  void fit_parameters() {
+  // least-squares fitting of k_overall only
+  double lsq_k_overall() const {
+    double sxx = 0, sxy = 0;
+    for (const Point& p : points) {
+      if (p.fobs < 1 || p.fobs < p.sigma)  // skip weak reflections
+        continue;
+      double x = std::abs(get_fcalc(p));
+      double y = p.fobs;
+      sxx += x * x;
+      sxy += x * y;
+    }
+    return sxx != 0. ? sxy / sxx : 1.;
+  }
+
+  // For testing only, don't use it.
+  // Estimates anisotropic b_star using other parameters (incl. isotropic B),
+  // following P. Afonine et al, doi:10.1107/S0907444913000462 sec. 2.1.
+  // The symmetry constraints are not implemented - don't use it!
+  void fit_b_star_approximately() {
+    double b_iso = 1/3. * get_b_overall().trace();
+    //size_t nc = constraint_matrix.size();
+    double M[36] = {};
+    double b[6] = {};
+    //std::vector<double> Vc(nc);
+    for (const Point& p : points) {
+      double fcalc = std::abs(get_fcalc(p));
+      // the factor 1 / 2 pi^2 will be taken into account later
+      double Z = std::log(p.fobs / (k_overall * fcalc)) + b_iso * p.stol2;
+      Vec3 h(p.hkl);
+      double V[6] = {h.x * h.x, h.y * h.y, h.z * h.z,
+                     2 * h.x * h.y, 2 * h.x * h.z, 2 * h.y * h.z};
+      //for (size_t i = 0; i < nc; ++i)
+      //  Vc[i] = vec6_dot(constraint_matrix[i], V);
+      for (size_t i = 0; i < 6; ++i) {
+        for (size_t j = 0; j < 6; ++j)
+          M[6*i+j] += V[i] * V[j];
+        b[i] -= Z * V[i];
+      }
+    }
+    jordan_solve(M, b, 6);
+    double b_star_iso = 1/3. * b_star.trace();
+    SMat33<double> u_star{b[0], b[1], b[2], b[3], b[4], b[5]};
+    // u_to_b() / (2 pi^2) = 8 pi^2 / 2 pi^2 = 4
+    b_star = u_star.scaled(4.0).added_kI(b_star_iso);
+    //auto e = get_b_overall().elements_pdb();
+    //printf("fitted B = {%g %g %g  %g %g %g}\n", e[0], e[1], e[2], e[3], e[4], e[5]);
+  }
+
+  double fit_parameters() {
     LevMar levmar;
-    levmar.fit(*this);
+    return levmar.fit(*this);
   }
 
 
   // interface for fitting
   std::vector<double> compute_values() const {
     std::vector<double> values;
     values.reserve(points.size());
     for (const Point& p : points) {
-      double fcalc = std::abs(p.fcmol + (Real)get_solvent_scale(p.stol2) * p.fmask);
+      double fcalc = std::abs(get_fcalc(p));
       values.push_back(fcalc * (Real) get_overall_scale_factor(p.hkl));
     }
     return values;
   }
 
   // the tile_* parameters allow tiling: computing derivatives from a span
   // of points at one time, which limits memory usage.
```

### Comparing `gemmi-0.6.5/include/gemmi/select.hpp` & `gemmi-0.6.6/include/gemmi/select.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/seqalign.hpp` & `gemmi-0.6.6/include/gemmi/seqalign.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #define GEMMI_SEQALIGN_HPP_
 
 #include <cstdint>
 #include <algorithm> // for reverse
 #include <map>
 #include <string>
 #include <vector>
+#include "fail.hpp"  // for fail
 
 namespace gemmi {
 
 struct AlignmentScoring {
   int match;
   int mismatch;
   int gapo;  // gap opening penalty
```

### Comparing `gemmi-0.6.5/include/gemmi/seqid.hpp` & `gemmi-0.6.6/include/gemmi/seqid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/seqtools.hpp` & `gemmi-0.6.6/include/gemmi/seqtools.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/serialize.hpp` & `gemmi-0.6.6/include/gemmi/serialize.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 SERIALIZE(SeqId, o.num, o.icode)
 
 SERIALIZE(AtomAddress, o.chain_name, o.res_id, o.atom_name, o.altloc)
 
 SERIALIZE(Metadata, o.authors, o.experiments, o.crystals, o.refinement,
           o.software, o.solved_by, o.starting_model, o.remark_300_detail)
 
-SERIALIZE(SoftwareItem, o.name, o.version, o.date, o.classification)
+SERIALIZE(SoftwareItem, o.name, o.version, o.date, o.description, o.classification)
 
 SERIALIZE(ReflectionsInfo, o.resolution_high, o.resolution_low, o.completeness,
           o.redundancy, o.r_merge, o.r_sym, o.mean_I_over_sigma)
 
 SERIALIZE(ExperimentInfo, o.method, o.number_of_crystals, o.unique_reflections,
           o.reflections, o.b_wilson, o.shells, o.diffraction_ids)
 
@@ -90,15 +90,15 @@
             o.luzzati_error, o.dpi_blow_r, o.dpi_blow_rfree,
             o.dpi_cruickshank_r, o.dpi_cruickshank_rfree,
             o.cc_fo_fc, o.cc_fo_fc_free, o.restr_stats, o.tls_groups, o.remarks)
 
 SERIALIZE(RefinementInfo::Restr, o.name, o.count, o.weight, o.function, o.dev_ideal)
 
 SERIALIZE(Entity, o.name, o.subchains, o.entity_type, o.polymer_type,
-          o.dbrefs, o.sifts_unp_acc, o.full_sequence)
+          o.reflects_microhetero, o.dbrefs, o.sifts_unp_acc, o.full_sequence)
 
 SERIALIZE(Entity::DbRef, o.db_name, o.accession_code, o.id_code,
           o.isoform, o.seq_begin, o.seq_end, o.db_begin, o.db_end,
           o.label_seq_begin, o.label_seq_end)
 
 SERIALIZE(SiftsUnpResidue, o.res, o.acc_index, o.num)
```

### Comparing `gemmi-0.6.5/include/gemmi/sfcalc.hpp` & `gemmi-0.6.6/include/gemmi/sfcalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/smcif.hpp` & `gemmi-0.6.6/include/gemmi/smcif.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #include "sprintf.hpp"   // for to_str
 
 namespace gemmi {
 
 inline
 SmallStructure make_small_structure_from_block(const cif::Block& block_) {
   using cif::as_number;
-  using cif::as_string;
   cif::Block& block = const_cast<cif::Block&>(block_);
   SmallStructure st;
   st.name = block.name;
 
   // unit cell and symmetry
   cif::Table cell = block.find("_cell_",
                                {"length_a", "length_b", "length_c",
@@ -29,34 +28,52 @@
     if (!cif::is_null(c[0]) && !cif::is_null(c[1]) && !cif::is_null(c[2]))
       st.cell.set(as_number(c[0]), as_number(c[1]), as_number(c[2]),
                   as_number(c[3]), as_number(c[4]), as_number(c[5]));
   }
   for (const char* tag : {"_space_group_name_H-M_alt",
                           "_symmetry_space_group_name_H-M"})
     if (const std::string* val = block.find_value(tag)) {
-      st.spacegroup_hm = as_string(*val);
+      st.spacegroup_hm = cif::as_string(*val);
       break;
     }
+  for (const char* tag : {"_space_group_symop_operation_xyz",
+                          "_symmetry_equiv_pos_as_xyz"}) {
+    if (const cif::Column col = block.find_values(tag)) {
+      st.symops.reserve(col.length());
+      for (const std::string& value : col)
+        st.symops.push_back(cif::as_string(value));
+      break;
+    }
+  }
+  for (const char* tag : {"_space_group_name_Hall", "_symmetry_space_group_name_Hall"})
+    if (const std::string* val = block.find_value(tag))
+      st.spacegroup_hall = cif::as_string(*val);
+  for (const char* tag : {"_space_group_IT_number", "_symmetry_Int_Tables_number"})
+    if (const std::string* val = block.find_value(tag)) {
+      st.spacegroup_number = cif::as_int(*val, 0);
+      break;
+    }
+  st.set_spacegroup("S.H2");
 
   enum { kLabel, kSymbol, kX, kY, kZ, kUiso, kBiso, kOcc, kDisorderGroup };
   cif::Table atom_table = block.find("_atom_site_",
                                      {"label",
                                       "?type_symbol",
                                       "?fract_x",
                                       "?fract_y",
                                       "?fract_z",
                                       "?U_iso_or_equiv",
                                       "?B_iso_or_equiv",
                                       "?occupancy",
                                       "?disorder_group"});
   for (auto row : atom_table) {
     SmallStructure::Site site;
-    site.label = as_string(row[kLabel]);
+    site.label = cif::as_string(row[kLabel]);
     if (row.has(kSymbol))
-      site.type_symbol = as_string(row[kSymbol]);
+      site.type_symbol = cif::as_string(row[kSymbol]);
     else
       site.type_symbol = site.label;
     if (row.has(kX))
       site.fract.x = as_number(row[kX]);
     if (row.has(kY))
       site.fract.y = as_number(row[kY]);
     if (row.has(kZ))
@@ -103,16 +120,14 @@
     atom_type.dispersion_real = cif::as_number(row[1]);
     atom_type.dispersion_imag = cif::as_number(row[2]);
     split_element_and_charge(atom_type.symbol, &atom_type);
     st.atom_types.push_back(atom_type);
   }
   if (cif::Column w_col = block.find_values("_diffrn_radiation_wavelength"))
     st.wavelength = cif::as_number(w_col.at(0));
-  st.setup_cell_images();
-
   return st;
 }
 
 inline cif::Block make_cif_block_from_small_structure(const SmallStructure& st) {
   cif::Block block;
   block.name = st.name;
   if (st.cell.is_crystal()) {
```

### Comparing `gemmi-0.6.5/include/gemmi/solmask.hpp` & `gemmi-0.6.6/include/gemmi/solmask.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     /*Bk*/ 1.64f, /*Cf*/ 1.63f, /*Es*/ 1.62f, /*Fm*/ 1.61f, /*Md*/ 1.60f,
     /*No*/ 1.59f, /*Lr*/ 1.58f, /*Rf*/ 1.00f, /*Db*/ 1.00f, /*Sg*/ 1.00f,
     /*Bh*/ 1.00f, /*Hs*/ 1.00f, /*Mt*/ 1.00f, /*Ds*/ 1.00f, /*Rg*/ 1.00f,
     /*Cn*/ 1.00f, /*Nh*/ 1.00f, /*Fl*/ 1.00f, /*Mc*/ 1.00f, /*Lv*/ 1.00f,
     /*Ts*/ 1.00f, /*Og*/ 1.00f,
     /*D*/  1.20f, /*END*/0.f
   };
-  static_assert(radii[static_cast<int>(El::D)] == 1.2f, "Hmm");
+  static_assert(ce_almost_eq(radii[static_cast<int>(El::D)], 1.2f), "Hmm");
   static_assert(sizeof(radii) / sizeof(radii[0]) ==
                 static_cast<int>(El::END) + 1, "Hmm");
   return radii[static_cast<int>(el)];
 }
 
 // Data from Refmac's ener_lib.cif: ionic radius - 0.2A or vdW radius + 0.2A.
 // For full compatibility use r_probe=1.0A and r_shrink=0.8A.
@@ -83,15 +83,15 @@
     /*Bk*/ 0.77f, /*Cf*/ 0.76f, /*Es*/ 1.00f, /*Fm*/ 1.00f, /*Md*/ 1.00f,
     /*No*/ 1.00f, /*Lr*/ 1.00f, /*Rf*/ 1.00f, /*Db*/ 1.00f, /*Sg*/ 1.00f,
     /*Bh*/ 1.00f, /*Hs*/ 1.00f, /*Mt*/ 1.00f, /*Ds*/ 1.00f, /*Rg*/ 1.00f,
     /*Cn*/ 1.00f, /*Nh*/ 1.00f, /*Fl*/ 1.00f, /*Mc*/ 1.00f, /*Lv*/ 1.00f,
     /*Ts*/ 1.00f, /*Og*/ 1.00f,
     /*D*/  1.40f, /*END*/0.f
   };
-  static_assert(radii[static_cast<int>(El::D)] == 1.40f, "Hmm");
+  static_assert(ce_almost_eq(radii[static_cast<int>(El::D)], 1.40f), "Hmm");
   return radii[static_cast<int>(el)];
 #else
   // temporary solution used in Refmac
   switch (el) {
     case El::H: return 1.4f;
     case El::D: return 1.4f;
     case El::O: return 1.08f;
@@ -209,14 +209,15 @@
   AtomicRadiiSet atomic_radii_set;
   bool ignore_hydrogen;
   bool ignore_zero_occupancy_atoms;
   double rprobe;
   double rshrink;
   double island_min_volume;
   double constant_r;
+  double requested_spacing = 0.;
 
   SolventMasker(AtomicRadiiSet choice, double constant_r_=0.) {
     set_radii(choice, constant_r_);
   }
 
   // currently this function sets also parameters other than radii
   void set_radii(AtomicRadiiSet choice, double constant_r_=0.) {
```

### Comparing `gemmi-0.6.5/include/gemmi/span.hpp` & `gemmi-0.6.6/include/gemmi/span.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/sprintf.hpp` & `gemmi-0.6.6/include/gemmi/sprintf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/stats.hpp` & `gemmi-0.6.6/include/gemmi/stats.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/symmetry.hpp` & `gemmi-0.6.6/include/gemmi/symmetry.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -58,22 +58,28 @@
   Rot rot;
   Tran tran;
 
   std::string triplet(char style='x') const;
 
   Op inverse() const;
 
-  // If the translation points outside of the unit cell, wrap it.
-  Op& wrap() {
+  Op::Tran wrapped_tran() const {
+    Op::Tran t = tran;
     for (int i = 0; i != 3; ++i) {
-      if (tran[i] >= DEN) // elements need to be in [0,DEN)
-        tran[i] %= DEN;
-      else if (tran[i] < 0)
-        tran[i] = ((tran[i] + 1) % DEN) + DEN - 1;
+      if (t[i] >= DEN) // elements need to be in [0,DEN)
+        t[i] %= DEN;
+      else if (t[i] < 0)
+        t[i] = ((t[i] + 1) % DEN) + DEN - 1;
     }
+    return t;
+  }
+
+  // If the translation points outside of the unit cell, wrap it.
+  Op& wrap() {
+    tran = wrapped_tran();
     return *this;
   }
 
   Op& translate(const Tran& a) {
     for (int i = 0; i != 3; ++i)
       tran[i] += a[i];
     return *this;
@@ -258,18 +264,31 @@
       num = (*c == '+' ? Op::DEN : -Op::DEN);
       c = impl::skip_blank(++c);
     }
     if (num == 0)
       fail("wrong or unsupported triplet format: " + s);
     int r_idx;
     int den = 1;
-    if (*c >= '0' && *c <= '9') {
+    if ((*c >= '0' && *c <= '9') || *c == '.') {
       // syntax examples in this branch: "1", "-1/2", "+2*x", "1/2 * b"
       char* endptr;
-      num *= std::strtol(c, &endptr, 10);
+      int n = std::strtol(c, &endptr, 10);
+      // some COD CIFs have decimal fractions ("-x+0.25", ".5+Y", "1.25000-y")
+      if (*endptr == '.') {
+        // avoiding strtod() etc which is locale-dependent
+        double fract = n;
+        for (double denom = 0.1; *++endptr >= '0' && *endptr <= '9'; denom *= 0.1)
+          fract += int(*endptr - '0') * denom;
+        double rounded = std::round(fract * num);
+        if (std::fabs(rounded - fract * num) > 0.05)
+          fail("unexpected number in a symmetry triplet part: " + s);
+        num = int(rounded);
+      } else {
+        num *= n;
+      }
       if (*endptr == '/')
         den = std::strtol(endptr + 1, &endptr, 10);
       if (*endptr == '*') {
         c = impl::skip_blank(endptr + 1);
         r_idx = interpret_miller_character(*c, s);
         ++c;
       } else {
@@ -727,17 +746,18 @@
 // Create GroupOps from Ops by separating centering vectors
 inline GroupOps split_centering_vectors(const std::vector<Op>& ops) {
   const Op identity = Op::identity();
   GroupOps go;
   go.sym_ops.push_back(identity);
   for (const Op& op : ops)
     if (Op* old_op = go.find_by_rotation(op.rot)) {
+      Op::Tran tran = op.wrapped_tran();
       if (op.rot == identity.rot)  // pure shift
-        go.cen_ops.push_back(op.tran);
-      if (op.tran == identity.tran)  // or rather |op.tran| < |old_op->tran| ?
+        go.cen_ops.push_back(tran);
+      if (tran == identity.tran)  // or rather |tran| < |old_op->tran| ?
         old_op->tran = op.tran;
     } else {
       go.sym_ops.push_back(op);
     }
   return go;
 }
 
@@ -1050,69 +1070,15 @@
     case 110: return {D/4, 0, 0};
     case 122: return {D/4, 0, D/8};
     case 210: return {D/8, D/8, D/8};
     default: return {0, 0, 0};
   }
 }
 
-// Generated by tools/gen_sg_table.py.
-inline const char* get_basisop(int basisop_idx) {
-  static const char* basisops[49] = {
-    "x,y,z",  // 0
-    "z,x,y",  // 1
-    "y,z,x",  // 2
-    "z,y,-x",  // 3
-    "x,y,-x+z",  // 4
-    "-x,z,y",  // 5
-    "-x+z,x,y",  // 6
-    "y,-x,z",  // 7
-    "y,-x+z,x",  // 8
-    "x-z,y,z",  // 9
-    "z,x-z,y",  // 10
-    "y,z,x-z",  // 11
-    "z,y,-x+z",  // 12
-    "x+z,y,-x",  // 13
-    "x+1/4,y+1/4,z",  // 14
-    "-x+z,z,y",  // 15
-    "-x,x+z,y",  // 16
-    "y,-x+z,z",  // 17
-    "y,-x,x+z",  // 18
-    "x+1/4,y-1/4,z",  // 19
-    "x-1/4,y-1/4,z-1/4",  // 20
-    "x-1/4,y-1/4,z",  // 21
-    "z,x-1/4,y-1/4",  // 22
-    "y-1/4,z,x-1/4",  // 23
-    "x-1/2,y-1/4,z+1/4",  // 24
-    "z+1/4,x-1/2,y-1/4",  // 25
-    "y-1/4,z+1/4,x-1/2",  // 26
-    "x+1/8,y+1/8,z+1/8",  // 27
-    "x+1/4,y-1/4,z+1/4",  // 28
-    "x-1/4,y+1/4,z",  // 29
-    "x+1/4,y+1/4,z+1/4",  // 30
-    "x,y+1/4,z+1/8",  // 31
-    "x-1/4,y+1/4,z+1/4",  // 32
-    "x-1/4,y+1/4,z-1/4",  // 33
-    "x-1/2,y+1/4,z+1/8",  // 34
-    "x-1/2,y+1/4,z-3/8",  // 35
-    "-y+z,x+z,-x+y+z",  // 36
-    "x-1/8,y-1/8,z-1/8",  // 37
-    "x+1/4,y+1/4,-x+z-1/4",  // 38
-    "x+1/4,y,z",  // 39
-    "x,y,z+1/4",  // 40
-    "-x,-y/2+z/2,y/2+z/2",  // 41
-    "-x/2+z/2,-y,x/2+z/2",  // 42
-    "x/2+y/2,x/2-y/2,-z",  // 43
-    "y/2+z/2,x/2+z/2,x/2+y/2",  // 44
-    "-x/2+y/2+z/2,x/2-y/2+z/2,x/2+y/2-z/2",  // 45
-    "-x/2+z,x/2,y",  // 46
-    "x-z/2,y,z/2",  // 47
-    "x/2+y/2,-x/2+y/2,z",  // 48
-  };
-  return basisops[basisop_idx];
-}
+const char* get_basisop(int basisop_idx);
 
 // Returns a change-of-basis operator for centred -> primitive transformation.
 // The same operator as inverse of z2p_op in sgtbx.
 inline Op::Rot centred_to_primitive(char centring_type) {
   constexpr int D = Op::DEN;
   constexpr int H = Op::DEN / 2;
   constexpr int T = Op::DEN / 3;
@@ -1235,21 +1201,21 @@
 // the template here is only to substitute C++17 inline variables
 // https://stackoverflow.com/questions/38043442/how-do-inline-variables-work
 namespace impl {
 
 template<class Dummy>
 struct Tables_
 {
-  static const SpaceGroup main[559];
+  static const SpaceGroup main[564];
   static const SpaceGroupAltName alt_names[28];
   static const unsigned char ccp4_hkl_asu[230];
 };
 
 template<class Dummy>
-const SpaceGroup Tables_<Dummy>::main[559] = {
+const SpaceGroup Tables_<Dummy>::main[564] = {
   // This table was generated by tools/gen_sg_table.py.
   // First 530 entries in the same order as in SgInfo, sgtbx and ITB.
   // Note: spacegroup 68 has three duplicates with different H-M names.
   {  1,    1, "P 1"       ,   0,     "", "P 1"           , 0 }, //   0
   {  2,    2, "P -1"      ,   0,     "", "-P 1"          , 0 }, //   1
   {  3,    3, "P 1 2 1"   ,   0,    "b", "P 2y"          , 0 }, //   2
   {  3, 1003, "P 1 1 2"   ,   0,    "c", "P 2"           , 1 }, //   3
@@ -1801,34 +1767,39 @@
   {  1,    0, "F 1"       ,   0,     "", "F 1"           , 44}, // 542
   {  1,    0, "I 1"       ,   0,     "", "I 1"           , 45}, // 543
   {  2,    0, "A -1"      ,   0,     "", "-A 1"          , 41}, // 544
   {  2,    0, "B -1"      ,   0,     "", "-B 1"          , 42}, // 545
   {  2,    0, "C -1"      ,   0,     "", "-C 1"          , 43}, // 546
   {  2,    0, "F -1"      ,   0,     "", "-F 1"          , 44}, // 547
   {  2,    0, "I -1"      ,   0,     "", "-I 1"          , 45}, // 548
-  // monoclinic
-  {  3,    0, "C 1 1 2"  ,    0,   "c1", "C 2"           , 46}, // 549
-  {  4,    0, "C 1 1 21"  ,   0,   "c1", "C 2c"          , 46}, // 550
-  { 12,    0, "F 1 2/m 1" ,   0,   "b4", "-F 2y"         , 47}, // 551
+  // monoclinic (qualifiers such as "b1" are assigned arbitrary unique numbers)
+  {  3,    0, "B 1 2 1"  ,    0,   "b1", "B 2y"          , 46}, // 549
+  {  3,    0, "C 1 1 2"  ,    0,   "c1", "C 2"           , 47}, // 550
+  {  4,    0, "B 1 21 1"  ,   0,   "b1", "B 2yb"         , 46}, // 551
+  {  4,    0, "C 1 1 21"  ,   0,   "c2", "C 2c"          , 47}, // 552
+  {  5,    0, "F 1 2 1"   ,   0,   "b6", "F 2y"          , 48}, // 553
+  {  8,    0, "F 1 m 1"   ,   0,   "b4", "F -2y"         , 48}, // 554
+  {  9,    0, "F 1 d 1"   ,   0,   "b4", "F -2yuw"       , 49}, // 555
+  { 12,    0, "F 1 2/m 1" ,   0,   "b4", "-F 2y"         , 48}, // 556
   // orthorhombic
-  { 64,    0, "A b a m"   ,   0,     "", "-A 2 2ab"      , 3 }, // 552 (==306)
+  { 64,    0, "A b a m"   ,   0,     "", "-A 2 2ab"      , 3 }, // 557 (==306)
   // tetragonal - enlarged C- and F-centred unit cells
-  { 89,    0, "C 4 2 2" ,     0,     "", "C 4 2"         , 48}, // 553
-  { 90,    0, "C 4 2 21" ,    0,     "", "C 4a 2"        , 48}, // 554
-  { 97,    0, "F 4 2 2" ,     0,     "", "F 4 2"         , 48}, // 555
-  {115,    0, "C -4 2 m"  ,   0,     "", "C -4 2"        , 48}, // 556
-  {117,    0, "C -4 2 b"  ,   0,     "", "C -4 2ya"      , 48}, // 557
-  {139,    0, "F 4/m m m" ,   0,     "", "-F 4 2"        , 48}, // 558
+  { 89,    0, "C 4 2 2" ,     0,     "", "C 4 2"         , 50}, // 558
+  { 90,    0, "C 4 2 21" ,    0,     "", "C 4a 2"        , 50}, // 559
+  { 97,    0, "F 4 2 2" ,     0,     "", "F 4 2"         , 50}, // 560
+  {115,    0, "C -4 2 m"  ,   0,     "", "C -4 2"        , 50}, // 561
+  {117,    0, "C -4 2 b"  ,   0,     "", "C -4 2ya"      , 50}, // 562
+  {139,    0, "F 4/m m m" ,   0,     "", "-F 4 2"        , 50}, // 563
 };
 
 template<class Dummy>
 const SpaceGroupAltName Tables_<Dummy>::alt_names[28] = {
   // In 1990's ITfC vol.A changed some of the standard names, introducing
-  // symbols 'e' and 'g'. sgtbx interprets these new symbols with
-  // option ad_hoc_1992. spglib uses only the new symbols.
+  // symbol 'e'. sgtbx interprets these new symbols with option ad_hoc_1992.
+  // spglib uses only the new symbols.
   {"A e m 2",   0, 190}, // A b m 2
   {"B m e 2",   0, 191}, // B m a 2
   {"B 2 e m",   0, 192}, // B 2 c m
   {"C 2 m e",   0, 193}, // C 2 m b
   {"C m 2 e",   0, 194}, // C m 2 a
   {"A e 2 m",   0, 195}, // A c 2 m
   {"A e a 2",   0, 202}, // A b a 2
@@ -1871,14 +1842,72 @@
   9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9, 9
 };
 
 } // namespace impl
 
 using spacegroup_tables = impl::Tables_<void>;
 
+// Generated by tools/gen_sg_table.py.
+inline const char* get_basisop(int basisop_idx) {
+  static const char* basisops[51] = {
+    "x,y,z",  // 0
+    "z,x,y",  // 1
+    "y,z,x",  // 2
+    "z,y,-x",  // 3
+    "x,y,-x+z",  // 4
+    "-x,z,y",  // 5
+    "-x+z,x,y",  // 6
+    "y,-x,z",  // 7
+    "y,-x+z,x",  // 8
+    "x-z,y,z",  // 9
+    "z,x-z,y",  // 10
+    "y,z,x-z",  // 11
+    "z,y,-x+z",  // 12
+    "x+z,y,-x",  // 13
+    "x+1/4,y+1/4,z",  // 14
+    "-x+z,z,y",  // 15
+    "-x,x+z,y",  // 16
+    "y,-x+z,z",  // 17
+    "y,-x,x+z",  // 18
+    "x+1/4,y-1/4,z",  // 19
+    "x-1/4,y-1/4,z-1/4",  // 20
+    "x-1/4,y-1/4,z",  // 21
+    "z,x-1/4,y-1/4",  // 22
+    "y-1/4,z,x-1/4",  // 23
+    "x-1/2,y-1/4,z+1/4",  // 24
+    "z+1/4,x-1/2,y-1/4",  // 25
+    "y-1/4,z+1/4,x-1/2",  // 26
+    "x+1/8,y+1/8,z+1/8",  // 27
+    "x+1/4,y-1/4,z+1/4",  // 28
+    "x-1/4,y+1/4,z",  // 29
+    "x+1/4,y+1/4,z+1/4",  // 30
+    "x,y+1/4,z+1/8",  // 31
+    "x-1/4,y+1/4,z+1/4",  // 32
+    "x-1/4,y+1/4,z-1/4",  // 33
+    "x-1/2,y+1/4,z+1/8",  // 34
+    "x-1/2,y+1/4,z-3/8",  // 35
+    "-y+z,x+z,-x+y+z",  // 36
+    "x-1/8,y-1/8,z-1/8",  // 37
+    "x+1/4,y+1/4,-x+z-1/4",  // 38
+    "x+1/4,y,z",  // 39
+    "x,y,z+1/4",  // 40
+    "-x,-y/2+z/2,y/2+z/2",  // 41
+    "-x/2+z/2,-y,x/2+z/2",  // 42
+    "x/2+y/2,x/2-y/2,-z",  // 43
+    "y/2+z/2,x/2+z/2,x/2+y/2",  // 44
+    "-x/2+y/2+z/2,x/2-y/2+z/2,x/2+y/2-z/2",  // 45
+    "x/2,y,-x/2+z",  // 46
+    "-x/2+z,x/2,y",  // 47
+    "x-z/2,y,z/2",  // 48
+    "x+z/2,y,z/2",  // 49
+    "x/2+y/2,-x/2+y/2,z",  // 50
+  };
+  return basisops[basisop_idx];
+}
+
 inline const SpaceGroup* find_spacegroup_by_number(int ccp4) noexcept {
   if (ccp4 == 0)
     return &spacegroup_tables::main[0];
   for (const SpaceGroup& sg : spacegroup_tables::main)
     if (sg.ccp4 == ccp4)
       return &sg;
   return nullptr;
@@ -1896,18 +1925,33 @@
   for (const SpaceGroup& sg : spacegroup_tables::main)
     if (sg.number == number && sg.is_reference_setting())
       return sg;
   throw std::invalid_argument("Invalid space-group number: "
                               + std::to_string(number));
 }
 
-// the angles alpha and gamma are optional. If provided they are only used
-// to distinguish hexagonal and rhombohedral settings (e.g. for "R 3").
+/// If angles alpha and gamma are provided, they are used to
+/// distinguish hexagonal and rhombohedral settings (e.g. for "R 3").
+/// \param prefer can specify preferred H/R settings and 1/2 origin choice.
+/// For example, prefer="2H" means the origin choice 2 and hexagonal
+/// settings. The default is "1H".
 inline const SpaceGroup* find_spacegroup_by_name(std::string name,
-                                  double alpha=0., double gamma=0.) noexcept {
+                                  double alpha=0., double gamma=0.,
+                                  const char* prefer=nullptr) {
+  bool prefer_2 = false;
+  bool prefer_R = false;
+  if (prefer)
+    for (const char* p = prefer; *p != '\0'; ++p) {
+      if (*p == '2')
+        prefer_2 = true;
+      else if (*p == 'R')
+        prefer_R = true;
+      else if (*p != '1' && *p != 'H')
+        throw std::invalid_argument("find_spacegroup_by_name(): invalid arg 'prefer'");
+    }
   const char* p = impl::skip_blank(name.c_str());
   if (*p >= '0' && *p <= '9') { // handle numbers
     char *endptr;
     long n = std::strtol(p, &endptr, 10);
     return *endptr == '\0' ? find_spacegroup_by_number(n) : nullptr;
   }
   char first = *p & ~0x20; // to uppercase
@@ -1922,40 +1966,55 @@
     if (name[i] >= 'A' && name[i] <= 'Z')
       name[i] |= 0x20;  // to lowercase
     else if (name[i] == ':')
       while (++i < name.size())
         if (name[i] >= 'a' && name[i] <= 'z')
           name[i] &= ~0x20;  // to uppercase
   }
+  // allow names ending with R or H, such as R3R instead of R3:R
+  if (name.back() == 'h' || name.back() == 'r') {
+    name.back() &= ~0x20;  // to uppercase
+    name.insert(name.end() - 1, ':');
+  }
   // The string that const char* p points to was just modified.
   // This confuses some compilers (GCC 4.8), so let's re-assign p.
   p = name.c_str() + start;
 
   for (const SpaceGroup& sg : spacegroup_tables::main)
     if (sg.hm[0] == first) {
       if (sg.hm[2] == *p) {
         const char* a = impl::skip_blank(p + 1);
         const char* b = impl::skip_blank(sg.hm + 3);
-        while (*a == *b && *b != '\0') {
+        // In IT 1935 and 1952, symbols of centrosymmetric, cubic space groups
+        // 200-206 and 221-230 had symbol 3 (not -3), e.g. Pm3 instead of Pm-3,
+        // as listed in Table 3.3.3.1 in ITfC (2016) vol. A, p.788.
+        while ((*a == *b && *b != '\0') ||
+               (*a == '3' && *b == '-' && b == sg.hm + 4 && *++b == '3')) {
           a = impl::skip_blank(a+1);
           b = impl::skip_blank(b+1);
         }
-        if (*b == '\0' &&
-            (*a == '\0' || (*a == ':' && *impl::skip_blank(a+1) == sg.ext))) {
-          // Change hexagonal settings to rhombohedral if the unit cell angles
-          // are more consistent with the latter.
-          // We have possible ambiguity in the hexagonal crystal family.
-          // For instance, "R 3" may mean "R 3:H" (hexagonal setting) or
-          // "R 3:R" (rhombohedral setting). The :H symbols come first
-          // in the table and are used by default. The ratio gamma:alpha
-          // is 120:90 in the hexagonal system and 1:1 in rhombohedral.
-          // We assume that the 'R' entry follows directly the 'H' entry.
-          if (*a == '\0' && sg.ext == 'H' && gamma < 1.125 * alpha)
-            return &sg + 1;
-          return &sg;
+        if (*b == '\0') {
+          if (*a == '\0') {
+            // Change hexagonal settings to rhombohedral if the unit cell
+            // angles are more consistent with the latter.
+            // We have possible ambiguity in the hexagonal crystal family.
+            // For instance, "R 3" may mean "R 3:H" (hexagonal setting) or
+            // "R 3:R" (rhombohedral setting). The :H symbols come first
+            // in the table and are used by default. The ratio gamma:alpha
+            // is 120:90 in the hexagonal system and 1:1 in rhombohedral.
+            // We assume that the 'R' entry follows directly the 'H' entry.
+            if (sg.ext == 'H' && (alpha == 0. ? prefer_R : gamma < 1.125 * alpha))
+              return &sg + 1;
+            // Similarly, the origin choice #2 follows directly #1.
+            if (sg.ext == '1' && prefer_2)
+              return &sg + 1;
+            return &sg;
+          } else if (*a == ':' && *impl::skip_blank(a+1) == sg.ext) {
+            return &sg;
+          }
         }
       } else if (sg.hm[2] == '1' && sg.hm[3] == ' ') {
         // check monoclinic short names, matching P2 to "P 1 2 1";
         // as an exception "B 2" == "B 1 1 2" (like in the PDB)
         const char* b = sg.hm + 4;
         if (*b != '1' || (first == 'B' && *++b == ' ' && *++b != '1')) {
           char end = (b == sg.hm + 4 ? ' ' : '\0');
@@ -2011,19 +2070,22 @@
   Op::Rot rot{};  // value-initialized only to avoid -Wmaybe-uninitialized
   bool is_ref;
 
   ReciprocalAsu(const SpaceGroup* sg, bool tnt=false) {
     if (sg == nullptr)
       fail("Missing space group");
     idx = spacegroup_tables::ccp4_hkl_asu[sg->number - 1];
-    if (tnt)
+    if (tnt) {
       idx += 10;
-    is_ref = sg->is_reference_setting();
-    if (!is_ref)
-      rot = sg->basisop().rot;
+      is_ref = true; // TNT ASU is given wrt current (not standard) settings
+    } else {
+      is_ref = sg->is_reference_setting();
+      if (!is_ref)
+        rot = sg->basisop().rot;
+    }
   }
 
   bool is_in(const Op::Miller& hkl) const {
     if (is_ref)
       return is_in_reference_setting(hkl[0], hkl[1], hkl[2]);
     Op::Miller r;
     for (int i = 0; i != 3; ++i)
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/fast_float.h` & `gemmi-0.6.6/include/gemmi/third_party/fast_float.h`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,14 @@
 #include <cfloat>
 #include <cstdint>
 #include <cassert>
 #include <cstring>
 #include <type_traits>
 #include <system_error>
 #ifdef __has_include
-  // line copied from a PR to fast_float, to avoid warnings
   #if __has_include(<stdfloat>) && (__cplusplus > 202002L || _MSVC_LANG > 202002L)
     #include <stdfloat>
   #endif
 #endif
 
 namespace fast_float {
 
@@ -459,15 +458,15 @@
 #if defined(_M_ARM64) && !defined(__MINGW32__)
   // ARM64 has native support for 64-bit multiplications, no need to emulate
   // But MinGW on ARM64 doesn't have native support for 64-bit multiplications
   answer.high = __umulh(a, b);
   answer.low = a * b;
 #elif defined(FASTFLOAT_32BIT) || (defined(_WIN64) && !defined(__clang__))
   answer.low = _umul128(a, b, &answer.high); // _umul128 not available on ARM64
-#elif defined(FASTFLOAT_64BIT)
+#elif defined(FASTFLOAT_64BIT) && defined(__SIZEOF_INT128__)
   __uint128_t r = ((__uint128_t)a) * b;
   answer.low = uint64_t(r);
   answer.high = uint64_t(r >> 64);
 #else
   answer.low = umul128_generic(a, b, &answer.high);
 #endif
   return answer;
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/pocketfft_hdronly.h` & `gemmi-0.6.6/include/gemmi/third_party/pocketfft_hdronly.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/LICENSE` & `gemmi-0.6.6/include/gemmi/third_party/tao/LICENSE`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_ANALYZE_CYCLES_HPP
 #define TAO_PEGTL_ANALYSIS_ANALYZE_CYCLES_HPP
 
 #include <cassert>
 
@@ -36,15 +36,15 @@
             const bool m_verbose;
             unsigned m_problems;
             grammar_info m_info;
             std::set< std::string > m_stack;
             std::map< std::string, bool > m_cache;
             std::map< std::string, bool > m_results;
 
-            const std::map< std::string, rule_info >::const_iterator find( const std::string& name ) const noexcept
+            std::map< std::string, rule_info >::const_iterator find( const std::string& name ) const noexcept
             {
                const auto iter = m_info.map.find( name );
                assert( iter != m_info.map.end() );
                return iter;
             }
 
             bool work( const std::map< std::string, rule_info >::const_iterator& start, const bool accum )
@@ -52,36 +52,36 @@
                const auto j = m_cache.find( start->first );
 
                if( j != m_cache.end() ) {
                   return j->second;
                }
                if( const auto g = make_insert_guard( m_stack, start->first ) ) {
                   switch( start->second.type ) {
-                     case rule_type::ANY: {
+                     case rule_type::any: {
                         bool a = false;
                         for( const auto& r : start->second.rules ) {
                            a = a || work( find( r ), accum || a );
                         }
                         return m_cache[ start->first ] = true;
                      }
-                     case rule_type::OPT: {
+                     case rule_type::opt: {
                         bool a = false;
                         for( const auto& r : start->second.rules ) {
                            a = a || work( find( r ), accum || a );
                         }
                         return m_cache[ start->first ] = false;
                      }
-                     case rule_type::SEQ: {
+                     case rule_type::seq: {
                         bool a = false;
                         for( const auto& r : start->second.rules ) {
                            a = a || work( find( r ), accum || a );
                         }
                         return m_cache[ start->first ] = a;
                      }
-                     case rule_type::SOR: {
+                     case rule_type::sor: {
                         bool a = true;
                         for( const auto& r : start->second.rules ) {
                            a = a && work( find( r ), accum );
                         }
                         return m_cache[ start->first ] = a;
                      }
                   }
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_ANALYSIS_COUNTED_HPP
-#define TAO_PEGTL_ANALYSIS_COUNTED_HPP
+#ifndef TAO_PEGTL_INTERNAL_REP_MIN_HPP
+#define TAO_PEGTL_INTERNAL_REP_MIN_HPP
 
 #include "../config.hpp"
 
-#include "generic.hpp"
+#include "rep.hpp"
+#include "seq.hpp"
+#include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace analysis
+      namespace internal
       {
-         template< rule_type Type, unsigned Count, typename... Rules >
-         struct counted
-            : generic< ( Count != 0 ) ? Type : rule_type::OPT, Rules... >
-         {
-         };
+         template< unsigned Min, typename Rule, typename... Rules >
+         using rep_min = seq< rep< Min, Rule, Rules... >, star< Rule, Rules... > >;
 
-      }  // namespace analysis
+      }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_GENERIC_HPP
 #define TAO_PEGTL_ANALYSIS_GENERIC_HPP
 
 #include "../config.hpp"
 
 #include "grammar_info.hpp"
-#include "insert_rules.hpp"
 #include "rule_type.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace analysis
@@ -20,15 +19,20 @@
          struct generic
          {
             template< typename Name >
             static std::string insert( grammar_info& g )
             {
                const auto r = g.insert< Name >( Type );
                if( r.second ) {
-                  insert_rules< Rules... >::insert( g, r.first->second );
+#ifdef __cpp_fold_expressions
+                  ( r.first->second.rules.push_back( Rules::analyze_t::template insert< Rules >( g ) ), ... );
+#else
+                  using swallow = bool[];
+                  (void)swallow{ ( r.first->second.rules.push_back( Rules::analyze_t::template insert< Rules >( g ) ), true )..., true };
+#endif
                }
                return r.first->first;
             }
          };
 
       }  // namespace analysis
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_GRAMMAR_INFO_HPP
 #define TAO_PEGTL_ANALYSIS_GRAMMAR_INFO_HPP
 
 #include <map>
 #include <string>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_INSERT_GUARD_HPP
 #define TAO_PEGTL_ANALYSIS_INSERT_GUARD_HPP
 
 #include <utility>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_ANALYSIS_INSERT_RULES_HPP
-#define TAO_PEGTL_ANALYSIS_INSERT_RULES_HPP
+#ifndef TAO_PEGTL_INTERNAL_BYTES_HPP
+#define TAO_PEGTL_INTERNAL_BYTES_HPP
 
 #include "../config.hpp"
 
-#include "grammar_info.hpp"
-#include "rule_info.hpp"
+#include "skip_control.hpp"
+
+#include "../analysis/counted.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace analysis
+      namespace internal
       {
-         template< typename... >
-         struct insert_rules;
-
-         template<>
-         struct insert_rules<>
+         template< unsigned Num >
+         struct bytes
          {
-            static void insert( grammar_info& /*unused*/, rule_info& /*unused*/ )
+            using analyze_t = analysis::counted< analysis::rule_type::any, Num >;
+
+            template< typename Input >
+            static bool match( Input& in ) noexcept( noexcept( in.size( 0 ) ) )
             {
+               if( in.size( Num ) >= Num ) {
+                  in.bump( Num );
+                  return true;
+               }
+               return false;
             }
          };
 
-         template< typename Rule, typename... Rules >
-         struct insert_rules< Rule, Rules... >
+         template< unsigned Num >
+         struct skip_control< bytes< Num > > : std::true_type
          {
-            static void insert( grammar_info& g, rule_info& r )
-            {
-               r.rules.push_back( Rule::analyze_t::template insert< Rule >( g ) );
-               insert_rules< Rules... >::insert( g, r );
-            }
          };
 
-      }  // namespace analysis
+      }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_RULE_INFO_HPP
 #define TAO_PEGTL_ANALYSIS_RULE_INFO_HPP
 
 #include <string>
 #include <vector>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ANALYSIS_RULE_TYPE_HPP
 #define TAO_PEGTL_ANALYSIS_RULE_TYPE_HPP
 
 #include "../config.hpp"
 
@@ -10,18 +10,24 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace analysis
       {
          enum class rule_type : char
          {
-            ANY,  // Consumption-on-success is always true; assumes bounded repetition of conjunction of sub-rules.
-            OPT,  // Consumption-on-success not necessarily true; assumes bounded repetition of conjunction of sub-rules.
-            SEQ,  // Consumption-on-success depends on consumption of (non-zero bounded repetition of) conjunction of sub-rules.
-            SOR   // Consumption-on-success depends on consumption of (non-zero bounded repetition of) disjunction of sub-rules.
+            any,  // Consumption-on-success is always true; assumes bounded repetition of conjunction of sub-rules.
+            opt,  // Consumption-on-success not necessarily true; assumes bounded repetition of conjunction of sub-rules.
+            seq,  // Consumption-on-success depends on consumption of (non-zero bounded repetition of) conjunction of sub-rules.
+            sor,  // Consumption-on-success depends on consumption of (non-zero bounded repetition of) disjunction of sub-rules.
+
+            // Compatibility, remove with 3.0.0
+            ANY = any,
+            OPT = opt,
+            SEQ = seq,
+            SOR = sor
          };
 
       }  // namespace analysis
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/analyze.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_ANALYZE_HPP
-#define TAO_PEGTL_ANALYZE_HPP
+#ifndef TAO_PEGTL_ANALYSIS_COUNTED_HPP
+#define TAO_PEGTL_ANALYSIS_COUNTED_HPP
 
-#include "config.hpp"
+#include "../config.hpp"
 
-#include "analysis/analyze_cycles.hpp"
+#include <cstddef>
+
+#include "generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      template< typename Rule >
-      std::size_t analyze( const bool verbose = true )
+      namespace analysis
       {
-         return analysis::analyze_cycles< Rule >( verbose ).problems();
-      }
+         template< rule_type Type, std::size_t Count, typename... Rules >
+         struct counted
+            : generic< ( Count != 0 ) ? Type : rule_type::opt, Rules... >
+         {
+         };
+
+      }  // namespace analysis
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/argv_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/argv_input.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ARGV_INPUT_HPP
 #define TAO_PEGTL_ARGV_INPUT_HPP
 
 #include <cstddef>
 #include <sstream>
@@ -25,15 +25,15 @@
             std::ostringstream os;
             os << "argv[" << argn << ']';
             return os.str();
          }
 
       }  // namespace internal
 
-      template< tracking_mode P = tracking_mode::IMMEDIATE, typename Eol = eol::lf_crlf >
+      template< tracking_mode P = tracking_mode::eager, typename Eol = eol::lf_crlf >
       struct argv_input
          : public memory_input< P, Eol >
       {
          template< typename T >
          argv_input( char** argv, const std::size_t argn, T&& in_source )
             : memory_input< P, Eol >( static_cast< const char* >( argv[ argn ] ), std::forward< T >( in_source ) )
          {
@@ -41,12 +41,17 @@
 
          argv_input( char** argv, const std::size_t argn )
             : argv_input( argv, argn, internal::make_argv_source( argn ) )
          {
          }
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      argv_input( Ts&&... )->argv_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/ascii.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/ascii.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,65 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_ASCII_HPP
 #define TAO_PEGTL_ASCII_HPP
 
 #include "config.hpp"
 #include "eol.hpp"
 
+#include "internal/always_false.hpp"
 #include "internal/result_on_found.hpp"
 #include "internal/rules.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       inline namespace ascii
       {
          // clang-format off
          struct alnum : internal::alnum {};
          struct alpha : internal::alpha {};
          struct any : internal::any< internal::peek_char > {};
-         struct blank : internal::one< internal::result_on_found::SUCCESS, internal::peek_char, ' ', '\t' > {};
-         struct digit : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, '0', '9' > {};
+         struct blank : internal::one< internal::result_on_found::success, internal::peek_char, ' ', '\t' > {};
+         struct digit : internal::range< internal::result_on_found::success, internal::peek_char, '0', '9' > {};
+         struct ellipsis : internal::string< '.', '.', '.' > {};
          struct eolf : internal::eolf {};
+         template< char... Cs > struct forty_two : internal::rep< 42, internal::one< internal::result_on_found::success, internal::peek_char, Cs... > > {};
          struct identifier_first : internal::identifier_first {};
          struct identifier_other : internal::identifier_other {};
          struct identifier : internal::identifier {};
          template< char... Cs > struct istring : internal::istring< Cs... > {};
          template< char... Cs > struct keyword : internal::seq< internal::string< Cs... >, internal::not_at< internal::identifier_other > > {};
-         struct lower : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, 'a', 'z' > {};
-         template< char... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_char, Cs... > {};
-         template< char Lo, char Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_char, Lo, Hi > {};
-         struct nul : internal::one< internal::result_on_found::SUCCESS, internal::peek_char, char( 0 ) > {};
-         template< char... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_char, Cs... > {};
-         struct print : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, char( 32 ), char( 126 ) > {};
-         template< char Lo, char Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, Lo, Hi > {};
+         struct lower : internal::range< internal::result_on_found::success, internal::peek_char, 'a', 'z' > {};
+         template< char... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_char, Cs... > {};
+         template< char Lo, char Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_char, Lo, Hi > {};
+         struct nul : internal::one< internal::result_on_found::success, internal::peek_char, char( 0 ) > {};
+         template< char... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_char, Cs... > {};
+         struct print : internal::range< internal::result_on_found::success, internal::peek_char, char( 32 ), char( 126 ) > {};
+         template< char Lo, char Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_char, Lo, Hi > {};
          template< char... Cs > struct ranges : internal::ranges< internal::peek_char, Cs... > {};
-         struct seven : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, char( 0 ), char( 127 ) > {};
-         struct shebang : internal::if_must< internal::string< '#', '!' >, internal::until< internal::eolf > > {};
-         struct space : internal::one< internal::result_on_found::SUCCESS, internal::peek_char, ' ', '\n', '\r', '\t', '\v', '\f' > {};
+         struct seven : internal::range< internal::result_on_found::success, internal::peek_char, char( 0 ), char( 127 ) > {};
+         struct shebang : internal::if_must< false, internal::string< '#', '!' >, internal::until< internal::eolf > > {};
+         struct space : internal::one< internal::result_on_found::success, internal::peek_char, ' ', '\n', '\r', '\t', '\v', '\f' > {};
          template< char... Cs > struct string : internal::string< Cs... > {};
+         template< char C > struct three : internal::string< C, C, C > {};
          template< char C > struct two : internal::string< C, C > {};
-         struct upper : internal::range< internal::result_on_found::SUCCESS, internal::peek_char, 'A', 'Z' > {};
+         struct upper : internal::range< internal::result_on_found::success, internal::peek_char, 'A', 'Z' > {};
          struct xdigit : internal::ranges< internal::peek_char, '0', '9', 'a', 'f', 'A', 'F' > {};
          // clang-format on
 
          template<>
          struct keyword<>
          {
             template< typename Input >
             static bool match( Input& /*unused*/ ) noexcept
             {
-               static_assert( sizeof( Input ) == 0, "empty keywords not allowed" );
+               static_assert( internal::always_false< Input >::value, "empty keywords not allowed" );
                return false;
             }
          };
 
       }  // namespace ascii
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/buffer_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/buffer_input.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_BUFFER_INPUT_HPP
 #define TAO_PEGTL_BUFFER_INPUT_HPP
 
+#include <algorithm>
+#include <cassert>
 #include <cstddef>
+#include <cstdint>
 #include <cstring>
 #include <memory>
+#include <stdexcept>
 #include <string>
 
 #include "config.hpp"
 #include "eol.hpp"
 #include "memory_input.hpp"
 #include "position.hpp"
 #include "tracking_mode.hpp"
 
 #include "internal/action_input.hpp"
-#include "internal/bump_impl.hpp"
+#include "internal/bump.hpp"
 #include "internal/iterator.hpp"
 #include "internal/marker.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      template< typename Reader, typename Eol = eol::lf_crlf, typename Source = std::string >
+      template< typename Reader, typename Eol = eol::lf_crlf, typename Source = std::string, std::size_t Chunk = 64 >
       class buffer_input
       {
       public:
-         static constexpr tracking_mode tracking_mode_v = tracking_mode::IMMEDIATE;
          using reader_t = Reader;
 
          using eol_t = Eol;
          using source_t = Source;
 
          using iterator_t = internal::iterator;
 
          using action_t = internal::action_input< buffer_input >;
 
+         static constexpr std::size_t chunk_size = Chunk;
+         static constexpr tracking_mode tracking_mode_v = tracking_mode::eager;
+
          template< typename T, typename... As >
          buffer_input( T&& in_source, const std::size_t maximum, As&&... as )
             : m_reader( std::forward< As >( as )... ),
-              m_maximum( maximum ),
-              m_buffer( new char[ maximum ] ),
+              m_maximum( maximum + Chunk ),
+              m_buffer( new char[ maximum + Chunk ] ),
               m_current( m_buffer.get() ),
               m_end( m_buffer.get() ),
               m_source( std::forward< T >( in_source ) )
          {
+            static_assert( Chunk != 0, "zero chunk size not implemented" );
+            assert( m_maximum > maximum );  // Catches overflow; change to >= when zero chunk size is implemented.
          }
 
          buffer_input( const buffer_input& ) = delete;
          buffer_input( buffer_input&& ) = delete;
 
          ~buffer_input() = default;
 
@@ -62,15 +70,15 @@
             require( 1 );
             return m_current.data == m_end;
          }
 
          std::size_t size( const std::size_t amount )
          {
             require( amount );
-            return std::size_t( m_end - m_current.data );
+            return buffer_occupied();
          }
 
          const char* current() const noexcept
          {
             return m_current.data;
          }
 
@@ -101,17 +109,23 @@
          }
 
          char peek_char( const std::size_t offset = 0 ) const noexcept
          {
             return m_current.data[ offset ];
          }
 
-         unsigned char peek_byte( const std::size_t offset = 0 ) const noexcept
+         std::uint8_t peek_uint8( const std::size_t offset = 0 ) const noexcept
+         {
+            return static_cast< std::uint8_t >( peek_char( offset ) );
+         }
+
+         // Compatibility, remove with 3.0.0
+         std::uint8_t peek_byte( const std::size_t offset = 0 ) const noexcept
          {
-            return static_cast< unsigned char >( peek_char( offset ) );
+            return static_cast< std::uint8_t >( peek_char( offset ) );
          }
 
          void bump( const std::size_t in_count = 1 ) noexcept
          {
             internal::bump( m_current, in_count, Eol::ch );
          }
 
@@ -123,31 +137,32 @@
          void bump_to_next_line( const std::size_t in_count = 1 ) noexcept
          {
             internal::bump_to_next_line( m_current, in_count );
          }
 
          void discard() noexcept
          {
-            const auto s = m_end - m_current.data;
-            std::memmove( m_buffer.get(), m_current.data, s );
-            m_current.data = m_buffer.get();
-            m_end = m_buffer.get() + s;
+            if( m_current.data > m_buffer.get() + Chunk ) {
+               const auto s = m_end - m_current.data;
+               std::memmove( m_buffer.get(), m_current.data, s );
+               m_current.data = m_buffer.get();
+               m_end = m_buffer.get() + s;
+            }
          }
 
          void require( const std::size_t amount )
          {
-            if( m_current.data + amount > m_end ) {
-               if( m_current.data + amount <= m_buffer.get() + m_maximum ) {
-                  if( const auto r = m_reader( m_end, amount - std::size_t( m_end - m_current.data ) ) ) {
-                     m_end += r;
-                  }
-                  else {
-                     m_maximum = 0;
-                  }
-               }
+            if( m_current.data + amount <= m_end ) {
+               return;
+            }
+            if( m_current.data + amount > m_buffer.get() + m_maximum ) {
+               throw std::overflow_error( "require beyond end of buffer" );
+            }
+            if( const auto r = m_reader( m_end, ( std::min )( buffer_free_after_end(), ( std::max )( amount - buffer_occupied(), Chunk ) ) ) ) {
+               m_end += r;
             }
          }
 
          template< rewind_mode M >
          internal::marker< iterator_t, M > mark() noexcept
          {
             return internal::marker< iterator_t, M >( m_current );
@@ -164,18 +179,41 @@
          }
 
          const iterator_t& iterator() const noexcept
          {
             return m_current;
          }
 
+         std::size_t buffer_capacity() const noexcept
+         {
+            return m_maximum;
+         }
+
+         std::size_t buffer_occupied() const noexcept
+         {
+            assert( m_end >= m_current.data );
+            return std::size_t( m_end - m_current.data );
+         }
+
+         std::size_t buffer_free_before_current() const noexcept
+         {
+            assert( m_current.data >= m_buffer.get() );
+            return std::size_t( m_current.data - m_buffer.get() );
+         }
+
+         std::size_t buffer_free_after_end() const noexcept
+         {
+            assert( m_buffer.get() + m_maximum >= m_end );
+            return std::size_t( m_buffer.get() + m_maximum - m_end );
+         }
+
       private:
          Reader m_reader;
          std::size_t m_maximum;
-         std::unique_ptr< char[] > m_buffer;
+         std::unique_ptr< char[] > m_buffer;  // NOLINT
          iterator_t m_current;
          char* m_end;
          const Source m_source;
       };
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/config.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/config.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_CONFIG_HPP
 #define TAO_PEGTL_CONFIG_HPP
 
-// Compatibility, remove with 3.0
+// Compatibility, remove with 3.0.0
 #ifdef TAOCPP_PEGTL_NAMESPACE
 #define TAO_PEGTL_NAMESPACE TAOCPP_PEGTL_NAMESPACE
 #endif
 
 #ifndef TAO_PEGTL_NAMESPACE
 #define TAO_PEGTL_NAMESPACE pegtl
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/cstream_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/istream_input.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_CSTREAM_INPUT_HPP
-#define TAO_PEGTL_CSTREAM_INPUT_HPP
+#ifndef TAO_PEGTL_ISTREAM_INPUT_HPP
+#define TAO_PEGTL_ISTREAM_INPUT_HPP
 
-#include <cstdio>
+#include <istream>
 
 #include "buffer_input.hpp"
 #include "config.hpp"
 #include "eol.hpp"
 
-#include "internal/cstream_reader.hpp"
+#include "internal/istream_reader.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      template< typename Eol = eol::lf_crlf >
-      struct cstream_input
-         : buffer_input< internal::cstream_reader, Eol >
+      template< typename Eol = eol::lf_crlf, std::size_t Chunk = 64 >
+      struct istream_input
+         : buffer_input< internal::istream_reader, Eol, std::string, Chunk >
       {
          template< typename T >
-         cstream_input( std::FILE* in_stream, const std::size_t in_maximum, T&& in_source )
-            : buffer_input< internal::cstream_reader, Eol >( std::forward< T >( in_source ), in_maximum, in_stream )
+         istream_input( std::istream& in_stream, const std::size_t in_maximum, T&& in_source )
+            : buffer_input< internal::istream_reader, Eol, std::string, Chunk >( std::forward< T >( in_source ), in_maximum, in_stream )
          {
          }
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      istream_input( Ts&&... )->istream_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/eol.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_EOL_HPP
 #define TAO_PEGTL_EOL_HPP
 
 #include "config.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/input_error.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/input_error.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INPUT_ERROR_HPP
 #define TAO_PEGTL_INPUT_ERROR_HPP
 
 #include <cerrno>
 #include <sstream>
@@ -42,8 +42,16 @@
    do {                                                                                 \
       const int errorno = errno;                                                        \
       std::ostringstream oss;                                                           \
       oss << TAO_PEGTL_INTERNAL_UNWRAP( MESSAGE ); \
       throw std::system_error( errorno, std::system_category(), oss.str() );            \
    } while( false )
 
+#define TAO_PEGTL_THROW_INPUT_WIN32_ERROR( MESSAGE )                                             \
+   do {                                                                                          \
+      const int errorno = GetLastError();                                                        \
+      std::ostringstream oss;                                                                    \
+      oss << TAO_PEGTL_INTERNAL_UNWRAP( MESSAGE ); \
+      throw std::system_error( errorno, std::system_category(), oss.str() );            \
+   } while( false )
+
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/action.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_control.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,40 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2019-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_ACTION_HPP
-#define TAO_PEGTL_INTERNAL_ACTION_HPP
+#ifndef TAO_PEGTL_CHANGE_CONTROL_HPP
+#define TAO_PEGTL_CHANGE_CONTROL_HPP
 
-#include "../config.hpp"
-
-#include "duseltronik.hpp"
-#include "seq.hpp"
-#include "skip_control.hpp"
-
-#include "../apply_mode.hpp"
-#include "../rewind_mode.hpp"
-
-#include "../analysis/generic.hpp"
+#include "apply_mode.hpp"
+#include "config.hpp"
+#include "match.hpp"
+#include "nothing.hpp"
+#include "rewind_mode.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace internal
+      template< template< typename... > class NewControl >
+      struct change_control
+         : maybe_nothing
       {
-         template< template< typename... > class Action, typename... Rules >
-         struct action
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   typename Input,
+                   typename... States >
+         static bool match( Input& in, States&&... st )
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
-
-            template< apply_mode A,
-                      rewind_mode M,
-                      template< typename... > class,
-                      template< typename... > class Control,
-                      typename Input,
-                      typename... States >
-            static bool match( Input& in, States&&... st )
-            {
-               return duseltronik< seq< Rules... >, A, M, Action, Control >::match( in, st... );
-            }
-         };
-
-         template< template< typename... > class Action, typename... Rules >
-         struct skip_control< action< Action, Rules... > > : std::true_type
-         {
-         };
-
-      }  // namespace internal
+            return TAO_PEGTL_NAMESPACE::match< Rule, A, M, Action, NewControl >( in, st... );
+         }
+      };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ACTION_INPUT_HPP
 #define TAO_PEGTL_INTERNAL_ACTION_INPUT_HPP
 
 #include <cstddef>
+#include <cstdint>
 #include <string>
 
 #include "iterator.hpp"
 
 #include "../config.hpp"
 #include "../position.hpp"
 
@@ -85,22 +86,28 @@
             }
 
             char peek_char( const std::size_t offset = 0 ) const noexcept
             {
                return begin()[ offset ];
             }
 
-            unsigned char peek_byte( const std::size_t offset = 0 ) const noexcept
+            std::uint8_t peek_uint8( const std::size_t offset = 0 ) const noexcept
             {
-               return static_cast< unsigned char >( peek_char( offset ) );
+               return static_cast< std::uint8_t >( peek_char( offset ) );
+            }
+
+            // Compatibility, remove with 3.0.0
+            std::uint8_t peek_byte( const std::size_t offset = 0 ) const noexcept
+            {
+               return static_cast< std::uint8_t >( peek_char( offset ) );
             }
 
             TAO_PEGTL_NAMESPACE::position position() const
             {
-               return input().position( iterator() );  // NOTE: Not efficient with LAZY inputs.
+               return input().position( iterator() );  // NOTE: Not efficient with lazy inputs.
             }
 
          protected:
             const iterator_t m_begin;
             const Input& m_input;
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_ALNUM_HPP
-#define TAO_PEGTL_INTERNAL_ALNUM_HPP
+#ifndef TAO_PEGTL_INTERNAL_ALPHA_HPP
+#define TAO_PEGTL_INTERNAL_ALPHA_HPP
 
 #include "../config.hpp"
 
 #include "peek_char.hpp"
 #include "ranges.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         using alnum = ranges< peek_char, 'a', 'z', 'A', 'Z', '0', '9' >;
+         using alpha = ranges< peek_char, 'a', 'z', 'A', 'Z' >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_ALPHA_HPP
-#define TAO_PEGTL_INTERNAL_ALPHA_HPP
+#ifndef TAO_PEGTL_INTERNAL_LIST_TAIL_PAD_HPP
+#define TAO_PEGTL_INTERNAL_LIST_TAIL_PAD_HPP
 
 #include "../config.hpp"
 
-#include "peek_char.hpp"
-#include "ranges.hpp"
+#include "list.hpp"
+#include "opt.hpp"
+#include "pad.hpp"
+#include "seq.hpp"
+#include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         using alpha = ranges< peek_char, 'a', 'z', 'A', 'Z' >;
+         template< typename Rule, typename Sep, typename Pad >
+         using list_tail_pad = seq< list< Rule, pad< Sep, Pad > >, opt< star< Pad >, Sep > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/any.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/any.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ANY_HPP
 #define TAO_PEGTL_INTERNAL_ANY_HPP
 
 #include "../config.hpp"
 
@@ -19,15 +19,15 @@
       {
          template< typename Peek >
          struct any;
 
          template<>
          struct any< peek_char >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
             {
                if( !in.empty() ) {
                   in.bump();
                   return true;
@@ -35,24 +35,22 @@
                return false;
             }
          };
 
          template< typename Peek >
          struct any
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
+            static bool match( Input& in ) noexcept( noexcept( Peek::peek( in ) ) )
             {
-               if( !in.empty() ) {
-                  if( const auto t = Peek::peek( in ) ) {
-                     in.bump( t.size );
-                     return true;
-                  }
+               if( const auto t = Peek::peek( in ) ) {
+                  in.bump( t.size );
+                  return true;
                }
                return false;
             }
          };
 
          template< typename Peek >
          struct skip_control< any< Peek > > : std::true_type
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_APPLY_HPP
 #define TAO_PEGTL_INTERNAL_APPLY_HPP
 
 #include "../config.hpp"
 
@@ -19,25 +19,25 @@
    {
       namespace internal
       {
          template< apply_mode A, typename... Actions >
          struct apply_impl;
 
          template<>
-         struct apply_impl< apply_mode::ACTION >
+         struct apply_impl< apply_mode::action >
          {
             template< typename Input, typename... States >
             static bool match( Input& /*unused*/, States&&... /*unused*/ )
             {
                return true;
             }
          };
 
          template< typename... Actions >
-         struct apply_impl< apply_mode::ACTION, Actions... >
+         struct apply_impl< apply_mode::action, Actions... >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
                using action_t = typename Input::action_t;
                const action_t i2( in.iterator(), in );  // No data -- range is from begin to begin.
 #ifdef __cpp_fold_expressions
@@ -48,32 +48,34 @@
                (void)swallow{ result = result && apply_single< Actions >::match( i2, st... )... };
                return result;
 #endif
             }
          };
 
          template< typename... Actions >
-         struct apply_impl< apply_mode::NOTHING, Actions... >
+         struct apply_impl< apply_mode::nothing, Actions... >
          {
             template< typename Input, typename... States >
             static bool match( Input& /*unused*/, States&&... /*unused*/ )
             {
                return true;
             }
          };
 
          template< typename... Actions >
          struct apply
          {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, 0 >;
+            using analyze_t = analysis::counted< analysis::rule_type::any, 0 >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                return apply_impl< A, Actions... >::match( in, st... );
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_APPLY0_HPP
 #define TAO_PEGTL_INTERNAL_APPLY0_HPP
 
 #include "../config.hpp"
 
@@ -19,25 +19,25 @@
    {
       namespace internal
       {
          template< apply_mode A, typename... Actions >
          struct apply0_impl;
 
          template<>
-         struct apply0_impl< apply_mode::ACTION >
+         struct apply0_impl< apply_mode::action >
          {
             template< typename... States >
             static bool match( States&&... /*unused*/ ) noexcept
             {
                return true;
             }
          };
 
          template< typename... Actions >
-         struct apply0_impl< apply_mode::ACTION, Actions... >
+         struct apply0_impl< apply_mode::action, Actions... >
          {
             template< typename... States >
             static bool match( States&&... st )
             {
 #ifdef __cpp_fold_expressions
                return ( apply0_single< Actions >::match( st... ) && ... );
 #else
@@ -46,32 +46,34 @@
                (void)swallow{ result = result && apply0_single< Actions >::match( st... )... };
                return result;
 #endif
             }
          };
 
          template< typename... Actions >
-         struct apply0_impl< apply_mode::NOTHING, Actions... >
+         struct apply0_impl< apply_mode::nothing, Actions... >
          {
             template< typename... States >
             static bool match( States&&... /*unused*/ ) noexcept
             {
                return true;
             }
          };
 
          template< typename... Actions >
          struct apply0
          {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, 0 >;
+            using analyze_t = analysis::counted< analysis::rule_type::any, 0 >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& /*unused*/, States&&... st )
             {
                return apply0_impl< A, Actions... >::match( st... );
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_APPLY0_SINGLE_HPP
 #define TAO_PEGTL_INTERNAL_APPLY0_SINGLE_HPP
 
 #include "../config.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_APPLY_SINGLE_HPP
 #define TAO_PEGTL_INTERNAL_APPLY_SINGLE_HPP
 
 #include "../config.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/at.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/at.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_AT_HPP
 #define TAO_PEGTL_INTERNAL_AT_HPP
 
 #include "../config.hpp"
 
-#include "rule_conjunction.hpp"
+#include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -18,37 +18,42 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename... Rules >
-         struct at;
+         struct at
+            : at< seq< Rules... > >
+         {
+         };
 
          template<>
          struct at<>
             : trivial< true >
          {
          };
 
-         template< typename... Rules >
-         struct at
+         template< typename Rule >
+         struct at< Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt, Rule >;
 
             template< apply_mode,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               const auto m = in.template mark< rewind_mode::REQUIRED >();
-               return rule_conjunction< Rules... >::template match< apply_mode::NOTHING, rewind_mode::ACTIVE, Action, Control >( in, st... );
+               const auto m = in.template mark< rewind_mode::required >();
+               return Control< Rule >::template match< apply_mode::nothing, rewind_mode::active, Action, Control >( in, st... );
             }
          };
 
          template< typename... Rules >
          struct skip_control< at< Rules... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bof.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bof.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_BOF_HPP
 #define TAO_PEGTL_INTERNAL_BOF_HPP
 
 #include "../config.hpp"
 
@@ -14,15 +14,15 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          struct bof
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept
             {
                return in.byte() == 0;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bol.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_BOL_HPP
 #define TAO_PEGTL_INTERNAL_BOL_HPP
 
 #include "../config.hpp"
 
@@ -14,15 +14,15 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          struct bol
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept
             {
                return in.byte_in_line() == 0;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2015-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2015-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_BUMP_HELP_HPP
 #define TAO_PEGTL_INTERNAL_BUMP_HELP_HPP
 
 #include <cstddef>
 #include <type_traits>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/bump.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_BUMP_IMPL_HPP
-#define TAO_PEGTL_INTERNAL_BUMP_IMPL_HPP
+#ifndef TAO_PEGTL_INTERNAL_BUMP_HPP
+#define TAO_PEGTL_INTERNAL_BUMP_HPP
 
 #include "../config.hpp"
 
 #include "iterator.hpp"
 
 namespace tao
 {
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/discard.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_BYTES_HPP
-#define TAO_PEGTL_INTERNAL_BYTES_HPP
+#ifndef TAO_PEGTL_INTERNAL_DISCARD_HPP
+#define TAO_PEGTL_INTERNAL_DISCARD_HPP
 
 #include "../config.hpp"
 
 #include "skip_control.hpp"
 
-#include "../analysis/counted.hpp"
+#include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< unsigned Num >
-         struct bytes
+         struct discard
          {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, Num >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( in.size( 0 ) ) )
+            static bool match( Input& in ) noexcept
             {
-               if( in.size( Num ) >= Num ) {
-                  in.bump( Num );
-                  return true;
-               }
-               return false;
+               static_assert( noexcept( in.discard() ), "an input's discard()-method must be noexcept" );
+               in.discard();
+               return true;
             }
          };
 
-         template< unsigned Num >
-         struct skip_control< bytes< Num > > : std::true_type
+         template<>
+         struct skip_control< discard > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/control.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/enable.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_CONTROL_HPP
-#define TAO_PEGTL_INTERNAL_CONTROL_HPP
+#ifndef TAO_PEGTL_INTERNAL_ENABLE_HPP
+#define TAO_PEGTL_INTERNAL_ENABLE_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< template< typename... > class Control, typename... Rules >
-         struct control
+         template< typename... Rules >
+         struct enable
+            : enable< seq< Rules... > >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+         };
+
+         template< typename Rule >
+         struct enable< Rule >
+         {
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rule >;
 
-            template< apply_mode A,
+            template< apply_mode,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return duseltronik< seq< Rules... >, A, M, Action, Control >::match( in, st... );
+               return Control< Rule >::template match< apply_mode::action, M, Action, Control >( in, st... );
             }
          };
 
-         template< template< typename... > class Control, typename... Rules >
-         struct skip_control< control< Control, Rules... > > : std::true_type
+         template< typename... Rules >
+         struct skip_control< enable< Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_CR_CRLF_EOL_HPP
 #define TAO_PEGTL_INTERNAL_CR_CRLF_EOL_HPP
 
 #include "../config.hpp"
 #include "../eol_pair.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_CR_EOL_HPP
 #define TAO_PEGTL_INTERNAL_CR_EOL_HPP
 
 #include "../config.hpp"
 #include "../eol_pair.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_CRLF_EOL_HPP
 #define TAO_PEGTL_INTERNAL_CRLF_EOL_HPP
 
 #include "../config.hpp"
 #include "../eol_pair.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_CSTREAM_READER_HPP
 #define TAO_PEGTL_INTERNAL_CSTREAM_READER_HPP
 
 #include <cassert>
 #include <cstddef>
@@ -21,15 +21,15 @@
          {
             explicit cstream_reader( std::FILE* s ) noexcept
                : m_cstream( s )
             {
                assert( m_cstream != nullptr );
             }
 
-            std::size_t operator()( char* buffer, const std::size_t length )
+            std::size_t operator()( char* buffer, const std::size_t length ) const
             {
                if( const auto r = std::fread( buffer, 1, length, m_cstream ) ) {
                   return r;
                }
                if( std::feof( m_cstream ) != 0 ) {
                   return 0;
                }
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_CSTRING_READER_HPP
 #define TAO_PEGTL_INTERNAL_CSTRING_READER_HPP
 
 #include <cassert>
 #include <cstddef>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,26 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_DEMANGLE_HPP
-#define TAO_PEGTL_INTERNAL_DEMANGLE_HPP
-
-#include <string>
-#include <typeinfo>
+#ifndef TAO_PEGTL_INTERNAL_LIST_HPP
+#define TAO_PEGTL_INTERNAL_LIST_HPP
 
 #include "../config.hpp"
 
-#if defined( __GLIBCXX__ )
-#include "demangle_cxxabi.hpp"
-#elif defined( __has_include )
-#if __has_include( <cxxabi.h> )
-#include "demangle_cxxabi.hpp"
-#else
-#include "demangle_nop.hpp"
-#endif
-#else
-#include "demangle_nop.hpp"
-#endif
+#include "seq.hpp"
+#include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename T >
-         std::string demangle()
-         {
-            return demangle( typeid( T ).name() );
-         }
+         template< typename Rule, typename Sep >
+         using list = seq< Rule, star< Sep, Rule > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_DEMANGLE_CXXABI_HPP
 #define TAO_PEGTL_INTERNAL_DEMANGLE_CXXABI_HPP
 
 #include <cstdlib>
 #include <cxxabi.h>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_DEMANGLE_NOP_HPP
 #define TAO_PEGTL_INTERNAL_DEMANGLE_NOP_HPP
 
 #include <string>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_DEMANGLE_SANITISE_HPP
 #define TAO_PEGTL_INTERNAL_DEMANGLE_SANITISE_HPP
 
 #include <string>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/disable.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/disable.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_DISABLE_HPP
 #define TAO_PEGTL_INTERNAL_DISABLE_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -19,26 +18,34 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename... Rules >
          struct disable
+            : disable< seq< Rules... > >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+         };
+
+         template< typename Rule >
+         struct disable< Rule >
+         {
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rule >;
 
             template< apply_mode,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return duseltronik< seq< Rules... >, apply_mode::NOTHING, M, Action, Control >::match( in, st... );
+               return Control< Rule >::template match< apply_mode::nothing, M, Action, Control >( in, st... );
             }
          };
 
          template< typename... Rules >
          struct skip_control< disable< Rules... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/discard.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eof.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_DISCARD_HPP
-#define TAO_PEGTL_INTERNAL_DISCARD_HPP
+#ifndef TAO_PEGTL_INTERNAL_EOF_HPP
+#define TAO_PEGTL_INTERNAL_EOF_HPP
 
 #include "../config.hpp"
 
 #include "skip_control.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         struct discard
+         struct eof
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept
+            static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
             {
-               static_assert( noexcept( in.discard() ), "an input's discard()-method must be noexcept" );
-               in.discard();
-               return true;
+               return in.empty();
             }
          };
 
          template<>
-         struct skip_control< discard > : std::true_type
+         struct skip_control< eof > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_DUSELTRONIK_HPP
 #define TAO_PEGTL_INTERNAL_DUSELTRONIK_HPP
 
 #include "../apply_mode.hpp"
 #include "../config.hpp"
@@ -15,25 +15,29 @@
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control,
-                   dusel_mode = dusel_mode::NOTHING >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   dusel_mode = dusel_mode::nothing >
          struct duseltronik;
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::NOTHING >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::nothing >
          {
             template< typename Input, typename... States >
             static auto match( Input& in, States&&... st )
                -> decltype( Rule::template match< A, M, Action, Control >( in, st... ), true )
             {
                return Rule::template match< A, M, Action, Control >( in, st... );
             }
@@ -47,118 +51,128 @@
                return Rule::match( in );
             }
          };
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::CONTROL >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::control >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
                Control< Rule >::start( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< Rule, A, M, Action, Control, dusel_mode::NOTHING >::match( in, st... ) ) {
+               if( duseltronik< Rule, A, M, Action, Control, dusel_mode::nothing >::match( in, st... ) ) {
                   Control< Rule >::success( static_cast< const Input& >( in ), st... );
                   return true;
                }
                Control< Rule >::failure( static_cast< const Input& >( in ), st... );
                return false;
             }
          };
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::CONTROL_AND_APPLY_VOID >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::control_and_apply_void >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
-               auto m = in.template mark< rewind_mode::REQUIRED >();
+               auto m = in.template mark< rewind_mode::required >();
 
                Control< Rule >::start( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< Rule, A, rewind_mode::ACTIVE, Action, Control, dusel_mode::NOTHING >::match( in, st... ) ) {
+               if( duseltronik< Rule, A, rewind_mode::active, Action, Control, dusel_mode::nothing >::match( in, st... ) ) {
                   Control< Rule >::template apply< Action >( m.iterator(), static_cast< const Input& >( in ), st... );
                   Control< Rule >::success( static_cast< const Input& >( in ), st... );
                   return m( true );
                }
                Control< Rule >::failure( static_cast< const Input& >( in ), st... );
                return false;
             }
          };
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::CONTROL_AND_APPLY_BOOL >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::control_and_apply_bool >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
-               auto m = in.template mark< rewind_mode::REQUIRED >();
+               auto m = in.template mark< rewind_mode::required >();
 
                Control< Rule >::start( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< Rule, A, rewind_mode::ACTIVE, Action, Control, dusel_mode::NOTHING >::match( in, st... ) ) {
+               if( duseltronik< Rule, A, rewind_mode::active, Action, Control, dusel_mode::nothing >::match( in, st... ) ) {
                   if( Control< Rule >::template apply< Action >( m.iterator(), static_cast< const Input& >( in ), st... ) ) {
                      Control< Rule >::success( static_cast< const Input& >( in ), st... );
                      return m( true );
                   }
                }
                Control< Rule >::failure( static_cast< const Input& >( in ), st... );
                return false;
             }
          };
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::CONTROL_AND_APPLY0_VOID >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::control_and_apply0_void >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
                Control< Rule >::start( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< Rule, A, M, Action, Control, dusel_mode::NOTHING >::match( in, st... ) ) {
+               if( duseltronik< Rule, A, M, Action, Control, dusel_mode::nothing >::match( in, st... ) ) {
                   Control< Rule >::template apply0< Action >( static_cast< const Input& >( in ), st... );
                   Control< Rule >::success( static_cast< const Input& >( in ), st... );
                   return true;
                }
                Control< Rule >::failure( static_cast< const Input& >( in ), st... );
                return false;
             }
          };
 
          template< typename Rule,
                    apply_mode A,
                    rewind_mode M,
-                   template< typename... > class Action,
-                   template< typename... > class Control >
-         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::CONTROL_AND_APPLY0_BOOL >
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control >
+         struct duseltronik< Rule, A, M, Action, Control, dusel_mode::control_and_apply0_bool >
          {
             template< typename Input, typename... States >
             static bool match( Input& in, States&&... st )
             {
-               auto m = in.template mark< rewind_mode::REQUIRED >();
+               auto m = in.template mark< rewind_mode::required >();
 
                Control< Rule >::start( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< Rule, A, rewind_mode::ACTIVE, Action, Control, dusel_mode::NOTHING >::match( in, st... ) ) {
+               if( duseltronik< Rule, A, rewind_mode::active, Action, Control, dusel_mode::nothing >::match( in, st... ) ) {
                   if( Control< Rule >::template apply0< Action >( static_cast< const Input& >( in ), st... ) ) {
                      Control< Rule >::success( static_cast< const Input& >( in ), st... );
                      return m( true );
                   }
                }
                Control< Rule >::failure( static_cast< const Input& >( in ), st... );
                return false;
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/enable.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/star.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,59 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_ENABLE_HPP
-#define TAO_PEGTL_INTERNAL_ENABLE_HPP
+#ifndef TAO_PEGTL_INTERNAL_STAR_HPP
+#define TAO_PEGTL_INTERNAL_STAR_HPP
+
+#include <type_traits>
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename... Rules >
-         struct enable
+         template< typename Rule, typename... Rules >
+         struct star
+            : star< seq< Rule, Rules... > >
+         {};
+
+         template< typename Rule >
+         struct star< Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt, Rule, star >;
 
-            template< apply_mode,
-                      rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+            template< apply_mode A,
+                      rewind_mode,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return duseltronik< seq< Rules... >, apply_mode::ACTION, M, Action, Control >::match( in, st... );
+               while( Control< Rule >::template match< A, rewind_mode::required, Action, Control >( in, st... ) ) {
+               }
+               return true;
             }
          };
 
-         template< typename... Rules >
-         struct skip_control< enable< Rules... > > : std::true_type
+         template< typename Rule, typename... Rules >
+         struct skip_control< star< Rule, Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ENDIAN_HPP
 #define TAO_PEGTL_INTERNAL_ENDIAN_HPP
 
 #include <cstdint>
 #include <cstring>
 
+#include "../config.hpp"
+
 #if defined( _WIN32 ) && !defined( __MINGW32__ )
 #include "endian_win.hpp"
 #else
 #include "endian_gcc.hpp"
 #endif
 
 namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ENDIAN_GCC_HPP
 #define TAO_PEGTL_INTERNAL_ENDIAN_GCC_HPP
 
 #include <cstdint>
 #include <cstring>
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-
-#if not defined( __BYTE_ORDER__ )
+#if !defined( __BYTE_ORDER__ )
 #error No byte order defined!
 #elif __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__
 
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_be
          {
             template< typename T >
             static T convert( const T n ) noexcept
             {
                return n;
             }
          };
 
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_le;
 
          template<>
          struct to_and_from_le< 1 >
          {
             static std::uint8_t convert( const std::uint8_t n ) noexcept
             {
@@ -46,15 +45,15 @@
          };
 
          template<>
          struct to_and_from_le< 2 >
          {
             static std::int16_t convert( const std::int16_t n ) noexcept
             {
-               return __builtin_bswap16( n );
+               return static_cast< std::int16_t >( __builtin_bswap16( static_cast< std::uint16_t >( n ) ) );
             }
 
             static std::uint16_t convert( const std::uint16_t n ) noexcept
             {
                return __builtin_bswap16( n );
             }
          };
@@ -69,15 +68,15 @@
                u = convert( u );
                std::memcpy( &n, &u, 4 );
                return n;
             }
 
             static std::int32_t convert( const std::int32_t n ) noexcept
             {
-               return __builtin_bswap32( n );
+               return static_cast< std::int32_t >( __builtin_bswap32( static_cast< std::uint32_t >( n ) ) );
             }
 
             static std::uint32_t convert( const std::uint32_t n ) noexcept
             {
                return __builtin_bswap32( n );
             }
          };
@@ -92,40 +91,40 @@
                u = convert( u );
                std::memcpy( &n, &u, 8 );
                return n;
             }
 
             static std::int64_t convert( const std::int64_t n ) noexcept
             {
-               return __builtin_bswap64( n );
+               return static_cast< std::int64_t >( __builtin_bswap64( static_cast< std::uint64_t >( n ) ) );
             }
 
             static std::uint64_t convert( const std::uint64_t n ) noexcept
             {
                return __builtin_bswap64( n );
             }
          };
 
 #define TAO_PEGTL_NATIVE_ORDER be
 #define TAO_PEGTL_NATIVE_UTF16 utf16_be
 #define TAO_PEGTL_NATIVE_UTF32 utf32_be
 
 #elif __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__
 
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_le
          {
             template< typename T >
             static T convert( const T n ) noexcept
             {
                return n;
             }
          };
 
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_be;
 
          template<>
          struct to_and_from_be< 1 >
          {
             static std::int8_t convert( const std::int8_t n ) noexcept
             {
@@ -139,15 +138,15 @@
          };
 
          template<>
          struct to_and_from_be< 2 >
          {
             static std::int16_t convert( const std::int16_t n ) noexcept
             {
-               return __builtin_bswap16( n );
+               return static_cast< std::int16_t >( __builtin_bswap16( static_cast< std::uint16_t >( n ) ) );
             }
 
             static std::uint16_t convert( const std::uint16_t n ) noexcept
             {
                return __builtin_bswap16( n );
             }
          };
@@ -162,15 +161,15 @@
                u = convert( u );
                std::memcpy( &n, &u, 4 );
                return n;
             }
 
             static std::int32_t convert( const std::int32_t n ) noexcept
             {
-               return __builtin_bswap32( n );
+               return static_cast< std::int32_t >( __builtin_bswap32( static_cast< std::uint32_t >( n ) ) );
             }
 
             static std::uint32_t convert( const std::uint32_t n ) noexcept
             {
                return __builtin_bswap32( n );
             }
          };
@@ -183,20 +182,20 @@
                std::uint64_t u;
                std::memcpy( &u, &n, 8 );
                u = convert( u );
                std::memcpy( &n, &u, 8 );
                return n;
             }
 
-            static std::uint64_t convert( const std::uint64_t n ) noexcept
+            static std::int64_t convert( const std::int64_t n ) noexcept
             {
-               return __builtin_bswap64( n );
+               return static_cast< std::int64_t >( __builtin_bswap64( static_cast< std::uint64_t >( n ) ) );
             }
 
-            static std::int64_t convert( const std::int64_t n ) noexcept
+            static std::uint64_t convert( const std::uint64_t n ) noexcept
             {
                return __builtin_bswap64( n );
             }
          };
 
 #define TAO_PEGTL_NATIVE_ORDER le
 #define TAO_PEGTL_NATIVE_UTF16 utf16_le
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ENDIAN_WIN_HPP
 #define TAO_PEGTL_INTERNAL_ENDIAN_WIN_HPP
 
 #include <cstdint>
 #include <cstring>
@@ -11,25 +11,25 @@
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_le
          {
             template< typename T >
             static T convert( const T t ) noexcept
             {
                return t;
             }
          };
 
-         template< unsigned S >
+         template< std::size_t S >
          struct to_and_from_be;
 
          template<>
          struct to_and_from_be< 1 >
          {
             static std::int8_t convert( const std::int8_t n ) noexcept
             {
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eof.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eol.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_EOF_HPP
-#define TAO_PEGTL_INTERNAL_EOF_HPP
+#ifndef TAO_PEGTL_INTERNAL_EOL_HPP
+#define TAO_PEGTL_INTERNAL_EOL_HPP
 
 #include "../config.hpp"
 
 #include "skip_control.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         struct eof
+         struct eol
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
+            static bool match( Input& in ) noexcept( noexcept( Input::eol_t::match( in ) ) )
             {
-               return in.empty();
+               return Input::eol_t::match( in ).first;
             }
          };
 
          template<>
-         struct skip_control< eof > : std::true_type
+         struct skip_control< eol > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_EOL_HPP
-#define TAO_PEGTL_INTERNAL_EOL_HPP
+#ifndef TAO_PEGTL_INTERNAL_EOLF_HPP
+#define TAO_PEGTL_INTERNAL_EOLF_HPP
 
 #include "../config.hpp"
 
 #include "skip_control.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         struct eol
+         struct eolf
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept( noexcept( Input::eol_t::match( in ) ) )
             {
-               return Input::eol_t::match( in ).first;
+               const auto p = Input::eol_t::match( in );
+               return p.first || ( !p.second );
             }
          };
 
          template<>
-         struct skip_control< eol > : std::true_type
+         struct skip_control< eolf > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_EOLF_HPP
-#define TAO_PEGTL_INTERNAL_EOLF_HPP
+#ifndef TAO_PEGTL_INTERNAL_TRIVIAL_HPP
+#define TAO_PEGTL_INTERNAL_TRIVIAL_HPP
 
 #include "../config.hpp"
 
 #include "skip_control.hpp"
 
-#include "../analysis/generic.hpp"
+#include "../analysis/counted.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         struct eolf
+         template< bool Result >
+         struct trivial
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::counted< analysis::rule_type::any, unsigned( !Result ) >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( Input::eol_t::match( in ) ) )
+            static bool match( Input& /*unused*/ ) noexcept
             {
-               const auto p = Input::eol_t::match( in );
-               return p.first || ( !p.second );
+               return Result;
             }
          };
 
-         template<>
-         struct skip_control< eolf > : std::true_type
+         template< bool Result >
+         struct skip_control< trivial< Result > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_mapper_posix.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_FILE_MAPPER_HPP
-#define TAO_PEGTL_INTERNAL_FILE_MAPPER_HPP
+#ifndef TAO_PEGTL_INTERNAL_FILE_MAPPER_POSIX_HPP
+#define TAO_PEGTL_INTERNAL_FILE_MAPPER_POSIX_HPP
 
 #include <sys/mman.h>
 #include <unistd.h>
 
 #include "../config.hpp"
 
 #include "file_opener.hpp"
@@ -25,15 +25,15 @@
             explicit file_mapper( const char* filename )
                : file_mapper( file_opener( filename ) )
             {
             }
 
             explicit file_mapper( const file_opener& reader )
                : m_size( reader.size() ),
-                 m_data( static_cast< const char* >(::mmap( nullptr, m_size, PROT_READ, MAP_PRIVATE, reader.m_fd, 0 ) ) )
+                 m_data( static_cast< const char* >( ::mmap( nullptr, m_size, PROT_READ, MAP_PRIVATE, reader.m_fd, 0 ) ) )
             {
                if( ( m_size != 0 ) && ( intptr_t( m_data ) == -1 ) ) {
                   TAO_PEGTL_THROW_INPUT_ERROR( "unable to mmap() file " << reader.m_source << " descriptor " << reader.m_fd );
                }
             }
 
             file_mapper( const file_mapper& ) = delete;
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_FILE_OPENER_HPP
 #define TAO_PEGTL_INTERNAL_FILE_OPENER_HPP
 
 #include <fcntl.h>
 #include <sys/stat.h>
@@ -39,15 +39,15 @@
             void operator=( const file_opener& ) = delete;
             void operator=( file_opener&& ) = delete;
 
             std::size_t size() const
             {
                struct stat st;  // NOLINT
                errno = 0;
-               if(::fstat( m_fd, &st ) < 0 ) {
+               if( ::fstat( m_fd, &st ) < 0 ) {
                   TAO_PEGTL_THROW_INPUT_ERROR( "unable to fstat() file " << m_source << " descriptor " << m_fd );
                }
                return std::size_t( st.st_size );
             }
 
             const char* const m_source;
             const int m_fd;
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_FILE_READER_HPP
 #define TAO_PEGTL_INTERNAL_FILE_READER_HPP
 
 #include <cstdio>
 #include <memory>
@@ -19,31 +19,31 @@
       namespace internal
       {
          inline std::FILE* file_open( const char* filename )
          {
             errno = 0;
 #if defined( _MSC_VER )
             std::FILE* file;
-            if(::fopen_s( &file, filename, "rb" ) == 0 )
+            if( ::fopen_s( &file, filename, "rb" ) == 0 )
 #elif defined( __MINGW32__ )
-            if( auto* file = std::fopen( filename, "rb" ) )
+            if( auto* file = std::fopen( filename, "rb" ) )  // NOLINT
 #else
-            if( auto* file = std::fopen( filename, "rbe" ) )
+            if( auto* file = std::fopen( filename, "rbe" ) )  // NOLINT
 #endif
             {
                return file;
             }
             TAO_PEGTL_THROW_INPUT_ERROR( "unable to fopen() file " << filename << " for reading" );
          }
 
          struct file_close
          {
             void operator()( FILE* f ) const noexcept
             {
-               std::fclose( f );
+               std::fclose( f );  // NOLINT
             }
          };
 
          class file_reader
          {
          public:
             explicit file_reader( const char* filename )
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_HAS_APPLY_HPP
-#define TAO_PEGTL_INTERNAL_HAS_APPLY_HPP
+#ifndef TAO_PEGTL_INTERNAL_HAS_APPLY0_HPP
+#define TAO_PEGTL_INTERNAL_HAS_APPLY0_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename, typename, typename... >
-         struct has_apply : std::false_type
-         {
-         };
-
-         template< typename A, typename... S >
-         struct has_apply< A, decltype( A::apply( std::declval< S >()... ) ), S... > : std::true_type
-         {
-         };
+         template< typename, typename, template< typename... > class, typename... >
+         struct has_apply0
+            : std::false_type
+         {};
+
+         template< typename C, template< typename... > class Action, typename... S >
+         struct has_apply0< C, decltype( C::template apply0< Action >( std::declval< S >()... ) ), Action, S... >
+            : std::true_type
+         {};
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_HAS_APPLY0_HPP
-#define TAO_PEGTL_INTERNAL_HAS_APPLY0_HPP
+#ifndef TAO_PEGTL_INTERNAL_HAS_APPLY_HPP
+#define TAO_PEGTL_INTERNAL_HAS_APPLY_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename, typename, typename... >
-         struct has_apply0 : std::false_type
-         {
-         };
-
-         template< typename A, typename... S >
-         struct has_apply0< A, decltype( A::apply0( std::declval< S >()... ) ), S... > : std::true_type
-         {
-         };
+         template< typename, typename, template< typename... > class, typename... >
+         struct has_apply
+            : std::false_type
+         {};
+
+         template< typename C, template< typename... > class Action, typename... S >
+         struct has_apply< C, decltype( C::template apply< Action >( std::declval< S >()... ) ), Action, S... >
+            : std::true_type
+         {};
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_IDENTIFIER_HPP
 #define TAO_PEGTL_INTERNAL_IDENTIFIER_HPP
 
 #include "../config.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_IF_APPLY_HPP
 #define TAO_PEGTL_INTERNAL_IF_APPLY_HPP
 
 #include "../config.hpp"
 
@@ -19,42 +19,46 @@
    {
       namespace internal
       {
          template< apply_mode A, typename Rule, typename... Actions >
          struct if_apply_impl;
 
          template< typename Rule >
-         struct if_apply_impl< apply_mode::ACTION, Rule >
+         struct if_apply_impl< apply_mode::action, Rule >
          {
             template< rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return Control< Rule >::template match< apply_mode::ACTION, M, Action, Control >( in, st... );
+               return Control< Rule >::template match< apply_mode::action, M, Action, Control >( in, st... );
             }
          };
 
          template< typename Rule, typename... Actions >
-         struct if_apply_impl< apply_mode::ACTION, Rule, Actions... >
+         struct if_apply_impl< apply_mode::action, Rule, Actions... >
          {
             template< rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                using action_t = typename Input::action_t;
 
-               auto m = in.template mark< rewind_mode::REQUIRED >();
+               auto m = in.template mark< rewind_mode::required >();
 
-               if( Control< Rule >::template match< apply_mode::ACTION, rewind_mode::ACTIVE, Action, Control >( in, st... ) ) {
+               if( Control< Rule >::template match< apply_mode::action, rewind_mode::active, Action, Control >( in, st... ) ) {
                   const action_t i2( m.iterator(), in );
 #ifdef __cpp_fold_expressions
                   return m( ( apply_single< Actions >::match( i2, st... ) && ... ) );
 #else
                   bool result = true;
                   using swallow = bool[];
                   (void)swallow{ result = result && apply_single< Actions >::match( i2, st... )... };
@@ -62,36 +66,40 @@
 #endif
                }
                return false;
             }
          };
 
          template< typename Rule, typename... Actions >
-         struct if_apply_impl< apply_mode::NOTHING, Rule, Actions... >
+         struct if_apply_impl< apply_mode::nothing, Rule, Actions... >
          {
             template< rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return Control< Rule >::template match< apply_mode::NOTHING, M, Action, Control >( in, st... );
+               return Control< Rule >::template match< apply_mode::nothing, M, Action, Control >( in, st... );
             }
          };
 
          template< typename Rule, typename... Actions >
          struct if_apply
          {
             using analyze_t = typename Rule::analyze_t;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                return if_apply_impl< A, Rule, Actions... >::template match< M, Action, Control >( in, st... );
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_IF_MUST_HPP
-#define TAO_PEGTL_INTERNAL_IF_MUST_HPP
+#ifndef TAO_PEGTL_INTERNAL_IF_MUST_ELSE_HPP
+#define TAO_PEGTL_INTERNAL_IF_MUST_ELSE_HPP
 
 #include "../config.hpp"
 
+#include "if_then_else.hpp"
 #include "must.hpp"
-#include "seq.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Cond, typename... Thens >
-         using if_must = seq< Cond, must< Thens... > >;
+         template< typename Cond, typename Then, typename Else >
+         using if_must_else = if_then_else< Cond, must< Then >, must< Else > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_IF_MUST_ELSE_HPP
-#define TAO_PEGTL_INTERNAL_IF_MUST_ELSE_HPP
+#ifndef TAO_PEGTL_INTERNAL_LIST_MUST_HPP
+#define TAO_PEGTL_INTERNAL_LIST_MUST_HPP
 
 #include "../config.hpp"
 
-#include "if_then_else.hpp"
 #include "must.hpp"
+#include "seq.hpp"
+#include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Cond, typename Then, typename Else >
-         using if_must_else = if_then_else< Cond, must< Then >, must< Else > >;
+         template< typename Rule, typename Sep >
+         using list_must = seq< Rule, star< Sep, must< Rule > > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_IF_THEN_ELSE_HPP
 #define TAO_PEGTL_INTERNAL_IF_THEN_ELSE_HPP
 
 #include "../config.hpp"
 
@@ -21,28 +21,30 @@
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename Cond, typename Then, typename Else >
          struct if_then_else
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SOR, seq< Cond, Then >, seq< not_at< Cond >, Else > >;
+            using analyze_t = analysis::generic< analysis::rule_type::sor, seq< Cond, Then >, seq< not_at< Cond >, Else > >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
                using m_t = decltype( m );
 
-               if( Control< Cond >::template match< A, rewind_mode::REQUIRED, Action, Control >( in, st... ) ) {
+               if( Control< Cond >::template match< A, rewind_mode::required, Action, Control >( in, st... ) ) {
                   return m( Control< Then >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) );
                }
                return m( Control< Else >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) );
             }
          };
 
          template< typename Cond, typename Then, typename Else >
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_INPUT_PAIR_HPP
 #define TAO_PEGTL_INTERNAL_INPUT_PAIR_HPP
 
+#include <cstdint>
+
 #include "../config.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename Data >
          struct input_pair
          {
             Data data;
-            unsigned char size;
+            std::uint8_t size;
 
             using data_t = Data;
 
             explicit operator bool() const noexcept
             {
                return size > 0;
             }
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_INTEGER_SEQUENCE_HPP
 #define TAO_PEGTL_INTERNAL_INTEGER_SEQUENCE_HPP
 
 #include <cstddef>
 #include <type_traits>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ISTREAM_READER_HPP
 #define TAO_PEGTL_INTERNAL_ISTREAM_READER_HPP
 
 #include <istream>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/istring.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/istring.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ISTRING_HPP
 #define TAO_PEGTL_INTERNAL_ISTRING_HPP
 
 #include <type_traits>
 
@@ -74,22 +74,22 @@
             : trivial< true >
          {
          };
 
          template< char... Cs >
          struct istring
          {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, sizeof...( Cs ) >;
+            using analyze_t = analysis::counted< analysis::rule_type::any, sizeof...( Cs ) >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept( noexcept( in.size( 0 ) ) )
             {
                if( in.size( sizeof...( Cs ) ) >= sizeof...( Cs ) ) {
                   if( istring_equal< Cs... >::match( in.current() ) ) {
-                     bump_help< result_on_found::SUCCESS, Input, char, Cs... >( in, sizeof...( Cs ) );
+                     bump_help< result_on_found::success, Input, char, Cs... >( in, sizeof...( Cs ) );
                      return true;
                   }
                }
                return false;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ITERATOR_HPP
 #define TAO_PEGTL_INTERNAL_ITERATOR_HPP
 
 #include <cstdlib>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_LF_CRLF_EOL_HPP
 #define TAO_PEGTL_INTERNAL_LF_CRLF_EOL_HPP
 
 #include "../config.hpp"
 #include "../eol_pair.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_LF_EOL_HPP
 #define TAO_PEGTL_INTERNAL_LF_EOL_HPP
 
 #include "../config.hpp"
 #include "../eol_pair.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pad.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_LIST_HPP
-#define TAO_PEGTL_INTERNAL_LIST_HPP
+#ifndef TAO_PEGTL_INTERNAL_PAD_HPP
+#define TAO_PEGTL_INTERNAL_PAD_HPP
 
 #include "../config.hpp"
 
 #include "seq.hpp"
 #include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename Sep >
-         using list = seq< Rule, star< Sep, Rule > >;
+         template< typename Rule, typename Pad1, typename Pad2 = Pad1 >
+         using pad = seq< star< Pad1 >, Rule, star< Pad2 > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_LIST_MUST_HPP
-#define TAO_PEGTL_INTERNAL_LIST_MUST_HPP
+#ifndef TAO_PEGTL_INTERNAL_PAD_OPT_HPP
+#define TAO_PEGTL_INTERNAL_PAD_OPT_HPP
 
 #include "../config.hpp"
 
-#include "must.hpp"
+#include "opt.hpp"
 #include "seq.hpp"
 #include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename Sep >
-         using list_must = seq< Rule, star< Sep, must< Rule > > >;
+         template< typename Rule, typename Pad >
+         using pad_opt = seq< star< Pad >, opt< Rule, star< Pad > > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_LIST_TAIL_HPP
 #define TAO_PEGTL_INTERNAL_LIST_TAIL_HPP
 
 #include "../config.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_uint8.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2018-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_LIST_TAIL_PAD_HPP
-#define TAO_PEGTL_INTERNAL_LIST_TAIL_PAD_HPP
+#ifndef TAO_PEGTL_INTERNAL_PEEK_UINT8_HPP
+#define TAO_PEGTL_INTERNAL_PEEK_UINT8_HPP
+
+#include <cstddef>
+#include <cstdint>
 
 #include "../config.hpp"
 
-#include "list.hpp"
-#include "opt.hpp"
-#include "pad.hpp"
-#include "seq.hpp"
-#include "star.hpp"
+#include "input_pair.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename Sep, typename Pad >
-         using list_tail_pad = seq< list< Rule, pad< Sep, Pad > >, opt< star< Pad >, Sep > >;
+         struct peek_uint8
+         {
+            using data_t = std::uint8_t;
+            using pair_t = input_pair< std::uint8_t >;
+
+            template< typename Input >
+            static pair_t peek( Input& in ) noexcept( noexcept( in.empty() ) )
+            {
+               if( in.empty() ) {
+                  return { 0, 0 };
+               }
+               return { in.peek_uint8(), 1 };
+            }
+         };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/marker.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/marker.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_MARKER_HPP
 #define TAO_PEGTL_INTERNAL_MARKER_HPP
 
 #include "../config.hpp"
 #include "../rewind_mode.hpp"
@@ -37,18 +37,18 @@
             bool operator()( const bool result ) const noexcept
             {
                return result;
             }
          };
 
          template< typename Iterator >
-         class marker< Iterator, rewind_mode::REQUIRED >
+         class marker< Iterator, rewind_mode::required >
          {
          public:
-            static constexpr rewind_mode next_rewind_mode = rewind_mode::ACTIVE;
+            static constexpr rewind_mode next_rewind_mode = rewind_mode::active;
 
             explicit marker( Iterator& i ) noexcept
                : m_saved( i ),
                  m_input( &i )
             {
             }
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/minus.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_missing.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,70 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2019-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_MINUS_HPP
-#define TAO_PEGTL_INTERNAL_MINUS_HPP
+#ifndef TAO_PEGTL_INTERNAL_IF_MISSING_HPP
+#define TAO_PEGTL_INTERNAL_IF_MISSING_HPP
 
 #include "../config.hpp"
-
-#include "skip_control.hpp"
-
-#include "../apply_mode.hpp"
-#include "../memory_input.hpp"
 #include "../rewind_mode.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         inline const char* source_pointer( const char* source ) noexcept
-         {
-            return source;
-         }
-
-         inline const char* source_pointer( const std::string& source ) noexcept
-         {
-            return source.c_str();
-         }
+         template< bool >
+         struct if_missing;
 
-         template< typename R, typename S >
-         struct minus
+         template<>
+         struct if_missing< true >
          {
-            using analyze_t = typename R::analyze_t;  // NOTE: S is currently ignored for analyze().
-
-            template< apply_mode A,
-                      rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+            template< typename Control,
+                      template< typename... >
+                      class Action,
                       typename Input,
                       typename... States >
-            static bool match( Input& in, States&&... st )
+            static void apply( Input& in, States&&... st )
             {
-               auto m = in.template mark< rewind_mode::REQUIRED >();
+               auto m = in.template mark< rewind_mode::required >();
+               Control::template apply< Action >( m.iterator(), in, st... );
+            }
 
-               if( !Control< R >::template match< A, rewind_mode::ACTIVE, Action, Control >( in, st... ) ) {
-                  return false;
-               }
-               memory_input< tracking_mode::LAZY, typename Input::eol_t, const char* > i2( m.iterator(), in.current(), source_pointer( in.source() ) );
-
-               if( !Control< S >::template match< apply_mode::NOTHING, rewind_mode::ACTIVE, Action, Control >( i2, st... ) ) {
-                  return m( true );
-               }
-               return m( !i2.empty() );
+            template< typename Control,
+                      template< typename... >
+                      class Action,
+                      typename Input,
+                      typename... States >
+            static void apply0( Input& in, States&&... st )
+            {
+               Control::template apply0< Action >( in, st... );
             }
          };
 
-         template< typename R, typename S >
-         struct skip_control< minus< R, S > > : std::true_type
+         template<>
+         struct if_missing< false >
          {
+            template< typename Control,
+                      template< typename... >
+                      class Action,
+                      typename Input,
+                      typename... States >
+            static void apply( Input& /*unused*/, States&&... /*unused*/ )
+            {
+            }
+
+            template< typename Control,
+                      template< typename... >
+                      class Action,
+                      typename Input,
+                      typename... States >
+            static void apply0( Input& /*unused*/, States&&... /*unused*/ )
+            {
+            }
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/must.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/seq.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,88 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_MUST_HPP
-#define TAO_PEGTL_INTERNAL_MUST_HPP
+#ifndef TAO_PEGTL_INTERNAL_SEQ_HPP
+#define TAO_PEGTL_INTERNAL_SEQ_HPP
 
 #include "../config.hpp"
 
-#include "raise.hpp"
-#include "rule_conjunction.hpp"
 #include "skip_control.hpp"
+#include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         // The general case applies must<> to each of the
-         // rules in the 'Rules' parameter pack individually.
-
          template< typename... Rules >
-         struct must
+         struct seq;
+
+         template<>
+         struct seq<>
+            : trivial< true >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+         };
+
+         template< typename Rule >
+         struct seq< Rule >
+         {
+            using analyze_t = typename Rule::analyze_t;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return rule_conjunction< must< Rules >... >::template match< A, M, Action, Control >( in, st... );
+               return Control< Rule >::template match< A, M, Action, Control >( in, st... );
             }
          };
 
-         // While in theory the implementation for a single rule could
-         // be simplified to must< Rule > = sor< Rule, raise< Rule > >, this
-         // would result in some unnecessary run-time overhead.
-
-         template< typename Rule >
-         struct must< Rule >
+         template< typename... Rules >
+         struct seq
          {
-            using analyze_t = typename Rule::analyze_t;
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rules... >;
 
             template< apply_mode A,
-                      rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      rewind_mode M,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               if( !Control< Rule >::template match< A, rewind_mode::DONTCARE, Action, Control >( in, st... ) ) {
-                  raise< Rule >::template match< A, rewind_mode::DONTCARE, Action, Control >( in, st... );
-               }
-               return true;
+               auto m = in.template mark< M >();
+               using m_t = decltype( m );
+#ifdef __cpp_fold_expressions
+               return m( ( Control< Rules >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) && ... ) );
+#else
+               bool result = true;
+               using swallow = bool[];
+               (void)swallow{ result = result && Control< Rules >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... )... };
+               return m( result );
+#endif
             }
-         };
+
+         };  // namespace internal
 
          template< typename... Rules >
-         struct skip_control< must< Rules... > > : std::true_type
+         struct skip_control< seq< Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_NOT_AT_HPP
 #define TAO_PEGTL_INTERNAL_NOT_AT_HPP
 
 #include "../config.hpp"
 
-#include "rule_conjunction.hpp"
+#include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -18,37 +18,42 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename... Rules >
-         struct not_at;
+         struct not_at
+            : not_at< seq< Rules... > >
+         {
+         };
 
          template<>
          struct not_at<>
             : trivial< false >
          {
          };
 
-         template< typename... Rules >
-         struct not_at
+         template< typename Rule >
+         struct not_at< Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt, Rule >;
 
             template< apply_mode,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               const auto m = in.template mark< rewind_mode::REQUIRED >();
-               return !rule_conjunction< Rules... >::template match< apply_mode::NOTHING, rewind_mode::ACTIVE, Action, Control >( in, st... );
+               const auto m = in.template mark< rewind_mode::required >();
+               return !Control< Rule >::template match< apply_mode::nothing, rewind_mode::active, Action, Control >( in, st... );
             }
          };
 
          template< typename... Rules >
          struct skip_control< not_at< Rules... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/one.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/one.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_ONE_HPP
 #define TAO_PEGTL_INTERNAL_ONE_HPP
 
 #include <algorithm>
 #include <utility>
@@ -26,45 +26,41 @@
          {
             return std::find( l.begin(), l.end(), c ) != l.end();
          }
 
          template< result_on_found R, typename Peek, typename Peek::data_t... Cs >
          struct one
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
+            static bool match( Input& in ) noexcept( noexcept( Peek::peek( in ) ) )
             {
-               if( !in.empty() ) {
-                  if( const auto t = Peek::peek( in ) ) {
-                     if( contains( t.data, { Cs... } ) == bool( R ) ) {
-                        bump_help< R, Input, typename Peek::data_t, Cs... >( in, t.size );
-                        return true;
-                     }
+               if( const auto t = Peek::peek( in ) ) {
+                  if( contains( t.data, { Cs... } ) == bool( R ) ) {
+                     bump_help< R, Input, typename Peek::data_t, Cs... >( in, t.size );
+                     return true;
                   }
                }
                return false;
             }
          };
 
          template< result_on_found R, typename Peek, typename Peek::data_t C >
          struct one< R, Peek, C >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< typename Input >
-            static bool match( Input& in ) noexcept( noexcept( in.empty() ) )
+            static bool match( Input& in ) noexcept( noexcept( Peek::peek( in ) ) )
             {
-               if( !in.empty() ) {
-                  if( const auto t = Peek::peek( in ) ) {
-                     if( ( t.data == C ) == bool( R ) ) {
-                        bump_help< R, Input, typename Peek::data_t, C >( in, t.size );
-                        return true;
-                     }
+               if( const auto t = Peek::peek( in ) ) {
+                  if( ( t.data == C ) == bool( R ) ) {
+                     bump_help< R, Input, typename Peek::data_t, C >( in, t.size );
+                     return true;
                   }
                }
                return false;
             }
          };
 
          template< result_on_found R, typename Peek, typename Peek::data_t... Cs >
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/opt.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/must.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_OPT_HPP
-#define TAO_PEGTL_INTERNAL_OPT_HPP
-
-#include <type_traits>
+#ifndef TAO_PEGTL_INTERNAL_MUST_HPP
+#define TAO_PEGTL_INTERNAL_MUST_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
+#include "raise.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
-#include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename... Rules >
-         struct opt;
+         // The general case applies must<> to each of the
+         // rules in the 'Rules' parameter pack individually.
 
-         template<>
-         struct opt<>
-            : trivial< true >
+         template< typename... Rules >
+         struct must
+            : seq< must< Rules >... >
          {
          };
 
-         template< typename... Rules >
-         struct opt
+         // While in theory the implementation for a single rule could
+         // be simplified to must< Rule > = sor< Rule, raise< Rule > >, this
+         // would result in some unnecessary run-time overhead.
+
+         template< typename Rule >
+         struct must< Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT, Rules... >;
+            using analyze_t = typename Rule::analyze_t;
 
             template< apply_mode A,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               if( !in.empty() ) {
-                  duseltronik< seq< Rules... >, A, rewind_mode::REQUIRED, Action, Control >::match( in, st... );
+               if( !Control< Rule >::template match< A, rewind_mode::dontcare, Action, Control >( in, st... ) ) {
+                  raise< Rule >::template match< A, rewind_mode::dontcare, Action, Control >( in, st... );
                }
                return true;
             }
          };
 
          template< typename... Rules >
-         struct skip_control< opt< Rules... > > : std::true_type
+         struct skip_control< must< Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pad.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_PAD_HPP
-#define TAO_PEGTL_INTERNAL_PAD_HPP
+#ifndef TAO_PEGTL_INTERNAL_RESULT_ON_FOUND_HPP
+#define TAO_PEGTL_INTERNAL_RESULT_ON_FOUND_HPP
 
 #include "../config.hpp"
 
-#include "seq.hpp"
-#include "star.hpp"
-
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename Pad1, typename Pad2 = Pad1 >
-         using pad = seq< star< Pad1 >, Rule, star< Pad2 > >;
+         enum class result_on_found : bool
+         {
+            success = true,
+            failure = false,
+         };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_PAD_OPT_HPP
-#define TAO_PEGTL_INTERNAL_PAD_OPT_HPP
+#ifndef TAO_PEGTL_INTERNAL_DUSEL_MODE_HPP
+#define TAO_PEGTL_INTERNAL_DUSEL_MODE_HPP
 
 #include "../config.hpp"
 
-#include "opt.hpp"
-#include "seq.hpp"
-#include "star.hpp"
-
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename Pad >
-         using pad_opt = seq< star< Pad >, opt< Rule, star< Pad > > >;
+         enum class dusel_mode : char
+         {
+            nothing = 0,
+            control = 1,
+            control_and_apply_void = 2,
+            control_and_apply_bool = 3,
+            control_and_apply0_void = 4,
+            control_and_apply0_bool = 5,
+         };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PEEK_CHAR_HPP
 #define TAO_PEGTL_INTERNAL_PEEK_CHAR_HPP
 
 #include <cstddef>
 
@@ -18,17 +18,20 @@
       {
          struct peek_char
          {
             using data_t = char;
             using pair_t = input_pair< char >;
 
             template< typename Input >
-            static pair_t peek( Input& in, const std::size_t o = 0 ) noexcept( noexcept( in.peek_char( 0 ) ) )
+            static pair_t peek( Input& in ) noexcept( noexcept( in.empty() ) )
             {
-               return { in.peek_char( o ), 1 };
+               if( in.empty() ) {
+                  return { 0, 0 };
+               }
+               return { in.peek_char(), 1 };
             }
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PEEK_UTF16_HPP
 #define TAO_PEGTL_INTERNAL_PEEK_UTF16_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
-#include "endian.hpp"
 #include "input_pair.hpp"
+#include "read_uint.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
@@ -27,50 +27,35 @@
 
             static_assert( sizeof( short_t ) == 2, "expected size 2 for 16bit value" );
             static_assert( sizeof( char16_t ) == 2, "expected size 2 for 16bit value" );
 
             template< typename Input >
             static pair_t peek( Input& in ) noexcept( noexcept( in.size( 4 ) ) )
             {
-               const std::size_t s = in.size( 4 );
-               if( s >= 2 ) {
-                  const char32_t t = R::read( in.current() );
-                  if( ( t < 0xd800 ) || ( t > 0xdbff ) || ( s < 4 ) ) {
-                     return { t, 2 };
-                  }
-                  const char32_t u = R::read( in.current() + 2 );
-                  if( ( u < 0xdc00 ) || ( u > 0xdfff ) ) {
-                     return { t, 2 };
-                  }
-                  return { ( ( ( t & 0x03ff ) << 10 ) | ( u & 0x03ff ) ) + 0x10000, 4 };
+               if( in.size( 2 ) < 2 ) {
+                  return { 0, 0 };
+               }
+               const char32_t t = R::read( in.current() );
+               if( ( t < 0xd800 ) || ( t > 0xdfff ) ) {
+                  return { t, 2 };
+               }
+               if( ( t >= 0xdc00 ) || ( in.size( 4 ) < 4 ) ) {
+                  return { 0, 0 };
+               }
+               const char32_t u = R::read( in.current() + 2 );
+               if( ( u >= 0xdc00 ) && ( u <= 0xdfff ) ) {
+                  const auto cp = ( ( ( t & 0x03ff ) << 10 ) | ( u & 0x03ff ) ) + 0x10000;
+                  return { cp, 4 };
                }
                return { 0, 0 };
             }
          };
 
-         struct read_utf16_be
-         {
-            static std::uint16_t read( const void* d ) noexcept
-            {
-               return be_to_h< std::uint16_t >( d );
-            }
-         };
-
-         struct read_utf16_le
-         {
-            static std::uint16_t read( const void* d ) noexcept
-            {
-               return le_to_h< std::uint16_t >( d );
-            }
-         };
-
-         using peek_utf16_be = peek_utf16_impl< read_utf16_be >;
-         using peek_utf16_le = peek_utf16_impl< read_utf16_le >;
-
-         using peek_utf16 = peek_utf16_le;
+         using peek_utf16_be = peek_utf16_impl< read_uint16_be >;
+         using peek_utf16_le = peek_utf16_impl< read_uint16_le >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PEEK_UTF32_HPP
 #define TAO_PEGTL_INTERNAL_PEEK_UTF32_HPP
 
 #include <cstddef>
 
 #include "../config.hpp"
 
-#include "endian.hpp"
 #include "input_pair.hpp"
+#include "read_uint.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
@@ -24,45 +24,27 @@
             using pair_t = input_pair< char32_t >;
 
             static_assert( sizeof( char32_t ) == 4, "expected size 4 for 32bit value" );
 
             template< typename Input >
             static pair_t peek( Input& in ) noexcept( noexcept( in.size( 4 ) ) )
             {
-               const std::size_t s = in.size( 4 );
-               if( s >= 4 ) {
-                  const char32_t t = R::read( in.current() );
-                  if( ( 0 <= t ) && ( t <= 0x10ffff ) ) {
-                     return { t, 4 };
-                  }
+               if( in.size( 4 ) < 4 ) {
+                  return { 0, 0 };
+               }
+               const char32_t t = R::read( in.current() );
+               if( ( t <= 0x10ffff ) && !( t >= 0xd800 && t <= 0xdfff ) ) {
+                  return { t, 4 };
                }
                return { 0, 0 };
             }
          };
 
-         struct read_utf32_be
-         {
-            static std::uint32_t read( const void* d ) noexcept
-            {
-               return be_to_h< std::uint32_t >( d );
-            }
-         };
-
-         struct read_utf32_le
-         {
-            static std::uint32_t read( const void* d ) noexcept
-            {
-               return le_to_h< std::uint32_t >( d );
-            }
-         };
-
-         using peek_utf32_be = peek_utf32_impl< read_utf32_be >;
-         using peek_utf32_le = peek_utf32_impl< read_utf32_le >;
-
-         using peek_utf32 = peek_utf32_le;
+         using peek_utf32_be = peek_utf32_impl< read_uint32_be >;
+         using peek_utf32_le = peek_utf32_impl< read_uint32_le >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PEEK_UTF8_HPP
 #define TAO_PEGTL_INTERNAL_PEEK_UTF8_HPP
 
 #include "../config.hpp"
 
@@ -16,55 +16,64 @@
       {
          struct peek_utf8
          {
             using data_t = char32_t;
             using pair_t = input_pair< char32_t >;
 
             template< typename Input >
-            static pair_t peek( Input& in ) noexcept( noexcept( in.size( 4 ) ) )
+            static pair_t peek( Input& in ) noexcept( noexcept( in.empty() ) )
             {
-               char32_t c0 = in.peek_byte();
-
+               if( in.empty() ) {
+                  return { 0, 0 };
+               }
+               char32_t c0 = in.peek_uint8();
                if( ( c0 & 0x80 ) == 0 ) {
                   return { c0, 1 };
                }
+               return peek_impl( in, c0 );
+            }
+
+         private:
+            template< typename Input >
+            static pair_t peek_impl( Input& in, char32_t c0 ) noexcept( noexcept( in.size( 4 ) ) )
+            {
                if( ( c0 & 0xE0 ) == 0xC0 ) {
                   if( in.size( 2 ) >= 2 ) {
-                     const char32_t c1 = in.peek_byte( 1 );
+                     const char32_t c1 = in.peek_uint8( 1 );
                      if( ( c1 & 0xC0 ) == 0x80 ) {
                         c0 &= 0x1F;
                         c0 <<= 6;
                         c0 |= ( c1 & 0x3F );
                         if( c0 >= 0x80 ) {
                            return { c0, 2 };
                         }
                      }
                   }
                }
                else if( ( c0 & 0xF0 ) == 0xE0 ) {
                   if( in.size( 3 ) >= 3 ) {
-                     const char32_t c1 = in.peek_byte( 1 );
-                     const char32_t c2 = in.peek_byte( 2 );
+                     const char32_t c1 = in.peek_uint8( 1 );
+                     const char32_t c2 = in.peek_uint8( 2 );
                      if( ( ( c1 & 0xC0 ) == 0x80 ) && ( ( c2 & 0xC0 ) == 0x80 ) ) {
                         c0 &= 0x0F;
                         c0 <<= 6;
                         c0 |= ( c1 & 0x3F );
                         c0 <<= 6;
                         c0 |= ( c2 & 0x3F );
-                        if( c0 >= 0x800 ) {
+                        if( c0 >= 0x800 && !( c0 >= 0xD800 && c0 <= 0xDFFF ) ) {
                            return { c0, 3 };
                         }
                      }
                   }
                }
                else if( ( c0 & 0xF8 ) == 0xF0 ) {
                   if( in.size( 4 ) >= 4 ) {
-                     const char32_t c1 = in.peek_byte( 1 );
-                     const char32_t c2 = in.peek_byte( 2 );
-                     const char32_t c3 = in.peek_byte( 3 );
+                     const char32_t c1 = in.peek_uint8( 1 );
+                     const char32_t c2 = in.peek_uint8( 2 );
+                     const char32_t c3 = in.peek_uint8( 3 );
                      if( ( ( c1 & 0xC0 ) == 0x80 ) && ( ( c2 & 0xC0 ) == 0x80 ) && ( ( c3 & 0xC0 ) == 0x80 ) ) {
                         c0 &= 0x07;
                         c0 <<= 6;
                         c0 |= ( c1 & 0x3F );
                         c0 <<= 6;
                         c0 |= ( c2 & 0x3F );
                         c0 <<= 6;
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2015-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2015-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PEGTL_STRING_HPP
 #define TAO_PEGTL_INTERNAL_PEGTL_STRING_HPP
 
 #include <cstddef>
 #include <type_traits>
@@ -55,15 +55,15 @@
 }  // namespace tao
 
 #define TAO_PEGTL_INTERNAL_EMPTY()
 #define TAO_PEGTL_INTERNAL_DEFER( X ) X TAO_PEGTL_INTERNAL_EMPTY()
 #define TAO_PEGTL_INTERNAL_EXPAND( ... ) __VA_ARGS__
 
 #define TAO_PEGTL_INTERNAL_STRING_AT( S, x, n ) \
-   tao::TAO_PEGTL_NAMESPACE::internal::string_at< S, ( 0##n < sizeof( x ) ) ? ( x )[ 0##n ] : 0, ( 0##n < sizeof( x ) - 1 ) >::type
+   tao::TAO_PEGTL_NAMESPACE::internal::string_at< S, ( 0##n < ( sizeof( x ) / sizeof( char ) ) ) ? ( x )[ 0##n ] : 0, ( 0##n < ( sizeof( x ) / sizeof( char ) ) - 1 ) >::type
 
 #define TAO_PEGTL_INTERNAL_JOIN_8( M, S, x, n )                                                  \
    tao::TAO_PEGTL_NAMESPACE::internal::string_join< TAO_PEGTL_INTERNAL_DEFER( M )( S, x, n##0 ), \
                                                     TAO_PEGTL_INTERNAL_DEFER( M )( S, x, n##1 ), \
                                                     TAO_PEGTL_INTERNAL_DEFER( M )( S, x, n##2 ), \
                                                     TAO_PEGTL_INTERNAL_DEFER( M )( S, x, n##3 ), \
                                                     TAO_PEGTL_INTERNAL_DEFER( M )( S, x, n##4 ), \
@@ -91,13 +91,13 @@
 
 #define TAO_PEGTL_ISTRING( x ) \
    TAO_PEGTL_INTERNAL_STRING( tao::TAO_PEGTL_NAMESPACE::ascii::istring, x )
 
 #define TAO_PEGTL_KEYWORD( x ) \
    TAO_PEGTL_INTERNAL_STRING( tao::TAO_PEGTL_NAMESPACE::ascii::keyword, x )
 
-// Compatibility, remove with 3.0
+// Compatibility, remove with 3.0.0
 #define TAOCPP_PEGTL_STRING( x ) TAO_PEGTL_STRING( x )
 #define TAOCPP_PEGTL_ISTRING( x ) TAO_PEGTL_ISTRING( x )
 #define TAOCPP_PEGTL_KEYWORD( x ) TAO_PEGTL_KEYWORD( x )
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/plus.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/plus.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_PLUS_HPP
 #define TAO_PEGTL_INTERNAL_PLUS_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "opt.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 #include "star.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
@@ -28,26 +27,34 @@
          // While plus<> could easily be implemented with
          // seq< Rule, Rules ..., star< Rule, Rules ... > > we
          // provide an explicit implementation to optimise away
          // the otherwise created input mark.
 
          template< typename Rule, typename... Rules >
          struct plus
+            : plus< seq< Rule, Rules... > >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rule, Rules..., opt< plus > >;
+         };
+
+         template< typename Rule >
+         struct plus< Rule >
+         {
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rule, opt< plus > >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               return seq< Rule, Rules... >::template match< A, M, Action, Control >( in, st... ) && star< Rule, Rules... >::template match< A, M, Action, Control >( in, st... );
+               return Control< Rule >::template match< A, M, Action, Control >( in, st... ) && Control< star< Rule > >::template match< A, M, Action, Control >( in, st... );
             }
          };
 
          template< typename Rule, typename... Rules >
          struct skip_control< plus< Rule, Rules... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/raise.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/raise.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_RAISE_HPP
 #define TAO_PEGTL_INTERNAL_RAISE_HPP
 
 #include <cstdlib>
 #include <stdexcept>
@@ -21,24 +21,26 @@
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename T >
          struct raise
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
 #ifdef _MSC_VER
 #pragma warning( push )
 #pragma warning( disable : 4702 )
 #endif
             template< apply_mode,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                Control< T >::raise( static_cast< const Input& >( in ), st... );
                throw std::logic_error( "code should be unreachable: Control< T >::raise() did not throw an exception" );  // NOLINT, LCOV_EXCL_LINE
 #ifdef _MSC_VER
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/range.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/range.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_RANGE_HPP
 #define TAO_PEGTL_INTERNAL_RANGE_HPP
 
 #include "../config.hpp"
 
@@ -17,31 +17,31 @@
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< result_on_found R, typename Peek, typename Peek::data_t Lo, typename Peek::data_t Hi >
          struct range
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            static_assert( Lo <= Hi, "invalid range detected" );
+
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< int Eol >
             struct can_match_eol
             {
                static constexpr bool value = ( ( ( Lo <= Eol ) && ( Eol <= Hi ) ) == bool( R ) );
             };
 
             template< typename Input >
-            static bool match( Input& in )
+            static bool match( Input& in ) noexcept( noexcept( Peek::peek( in ) ) )
             {
-               if( !in.empty() ) {
-                  if( const auto t = Peek::peek( in ) ) {
-                     if( ( ( Lo <= t.data ) && ( t.data <= Hi ) ) == bool( R ) ) {
-                        bump_impl< can_match_eol< Input::eol_t::ch >::value >::bump( in, t.size );
-                        return true;
-                     }
+               if( const auto t = Peek::peek( in ) ) {
+                  if( ( ( Lo <= t.data ) && ( t.data <= Hi ) ) == bool( R ) ) {
+                     bump_impl< can_match_eol< Input::eol_t::ch >::value >::bump( in, t.size );
+                     return true;
                   }
                }
                return false;
             }
          };
 
          template< result_on_found R, typename Peek, typename Peek::data_t Lo, typename Peek::data_t Hi >
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_RANGES_HPP
 #define TAO_PEGTL_INTERNAL_RANGES_HPP
 
 #include "../config.hpp"
 
@@ -42,51 +42,51 @@
                return c == Eq;
             }
          };
 
          template< int Eol, typename Char, Char Lo, Char Hi, Char... Cs >
          struct ranges_impl< Eol, Char, Lo, Hi, Cs... >
          {
+            static_assert( Lo <= Hi, "invalid range detected" );
+
             static constexpr bool can_match_eol = ( ( ( Lo <= Eol ) && ( Eol <= Hi ) ) || ranges_impl< Eol, Char, Cs... >::can_match_eol );
 
             static bool match( const Char c ) noexcept
             {
                return ( ( Lo <= c ) && ( c <= Hi ) ) || ranges_impl< Eol, Char, Cs... >::match( c );
             }
          };
 
          template< typename Peek, typename Peek::data_t... Cs >
          struct ranges
          {
-            using analyze_t = analysis::generic< analysis::rule_type::ANY >;
+            using analyze_t = analysis::generic< analysis::rule_type::any >;
 
             template< int Eol >
             struct can_match_eol
             {
                static constexpr bool value = ranges_impl< Eol, typename Peek::data_t, Cs... >::can_match_eol;
             };
 
             template< typename Input >
-            static bool match( Input& in )
+            static bool match( Input& in ) noexcept( noexcept( Peek::peek( in ) ) )
             {
-               if( !in.empty() ) {
-                  if( const auto t = Peek::peek( in ) ) {
-                     if( ranges_impl< Input::eol_t::ch, typename Peek::data_t, Cs... >::match( t.data ) ) {
-                        bump_impl< can_match_eol< Input::eol_t::ch >::value >::bump( in, t.size );
-                        return true;
-                     }
+               if( const auto t = Peek::peek( in ) ) {
+                  if( ranges_impl< Input::eol_t::ch, typename Peek::data_t, Cs... >::match( t.data ) ) {
+                     bump_impl< can_match_eol< Input::eol_t::ch >::value >::bump( in, t.size );
+                     return true;
                   }
                }
                return false;
             }
          };
 
          template< typename Peek, typename Peek::data_t Lo, typename Peek::data_t Hi >
          struct ranges< Peek, Lo, Hi >
-            : range< result_on_found::SUCCESS, Peek, Lo, Hi >
+            : range< result_on_found::success, Peek, Lo, Hi >
          {
          };
 
          template< typename Peek, typename Peek::data_t... Cs >
          struct skip_control< ranges< Peek, Cs... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_REP_HPP
 #define TAO_PEGTL_INTERNAL_REP_HPP
 
 #include "../config.hpp"
 
-#include "rule_conjunction.hpp"
+#include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/counted.hpp"
@@ -18,46 +18,51 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< unsigned Num, typename... Rules >
-         struct rep;
+         struct rep
+            : rep< Num, seq< Rules... > >
+         {
+         };
 
          template< unsigned Num >
          struct rep< Num >
             : trivial< true >
          {
          };
 
-         template< typename Rule, typename... Rules >
-         struct rep< 0, Rule, Rules... >
+         template< typename Rule >
+         struct rep< 0, Rule >
             : trivial< true >
          {
          };
 
-         template< unsigned Num, typename... Rules >
-         struct rep
+         template< unsigned Num, typename Rule >
+         struct rep< Num, Rule >
          {
-            using analyze_t = analysis::counted< analysis::rule_type::SEQ, Num, Rules... >;
+            using analyze_t = analysis::counted< analysis::rule_type::seq, Num, Rule >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
                using m_t = decltype( m );
 
                for( unsigned i = 0; i != Num; ++i ) {
-                  if( !rule_conjunction< Rules... >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) {
+                  if( !Control< Rule >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) {
                      return false;
                   }
                }
                return m( true );
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_REP_MIN_HPP
-#define TAO_PEGTL_INTERNAL_REP_MIN_HPP
+#ifndef TAO_PEGTL_INTERNAL_STAR_MUST_HPP
+#define TAO_PEGTL_INTERNAL_STAR_MUST_HPP
 
 #include "../config.hpp"
 
-#include "rep.hpp"
-#include "seq.hpp"
+#include "if_must.hpp"
 #include "star.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< unsigned Min, typename Rule, typename... Rules >
-         using rep_min = seq< rep< Min, Rule, Rules... >, star< Rule, Rules... > >;
+         template< typename Cond, typename... Rules >
+         using star_must = star< if_must< false, Cond, Rules... > >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_REP_MIN_MAX_HPP
 #define TAO_PEGTL_INTERNAL_REP_MIN_MAX_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "not_at.hpp"
-#include "rule_conjunction.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
@@ -23,58 +21,63 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< unsigned Min, unsigned Max, typename... Rules >
-         struct rep_min_max;
+         struct rep_min_max
+            : rep_min_max< Min, Max, seq< Rules... > >
+         {
+         };
 
          template< unsigned Min, unsigned Max >
          struct rep_min_max< Min, Max >
             : trivial< false >
          {
             static_assert( Min <= Max, "invalid rep_min_max rule (maximum number of repetitions smaller than minimum)" );
          };
 
-         template< typename Rule, typename... Rules >
-         struct rep_min_max< 0, 0, Rule, Rules... >
-            : not_at< Rule, Rules... >
+         template< typename Rule >
+         struct rep_min_max< 0, 0, Rule >
+            : not_at< Rule >
          {
          };
 
-         template< unsigned Min, unsigned Max, typename... Rules >
-         struct rep_min_max
+         template< unsigned Min, unsigned Max, typename Rule >
+         struct rep_min_max< Min, Max, Rule >
          {
-            using analyze_t = analysis::counted< analysis::rule_type::SEQ, Min, Rules... >;
+            using analyze_t = analysis::counted< analysis::rule_type::seq, Min, Rule >;
 
             static_assert( Min <= Max, "invalid rep_min_max rule (maximum number of repetitions smaller than minimum)" );
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
                using m_t = decltype( m );
 
                for( unsigned i = 0; i != Min; ++i ) {
-                  if( !rule_conjunction< Rules... >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) {
+                  if( !Control< Rule >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) {
                      return false;
                   }
                }
                for( unsigned i = Min; i != Max; ++i ) {
-                  if( !duseltronik< seq< Rules... >, A, rewind_mode::REQUIRED, Action, Control >::match( in, st... ) ) {
+                  if( !Control< Rule >::template match< A, rewind_mode::required, Action, Control >( in, st... ) ) {
                      return m( true );
                   }
                }
-               return m( duseltronik< not_at< Rules... >, A, m_t::next_rewind_mode, Action, Control >::match( in, st... ) );  // NOTE that not_at<> will always rewind.
+               return m( Control< not_at< Rule > >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) );  // NOTE that not_at<> will always rewind.
             }
          };
 
          template< unsigned Min, unsigned Max, typename... Rules >
          struct skip_control< rep_min_max< Min, Max, Rules... > > : std::true_type
          {
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_REP_OPT_HPP
 #define TAO_PEGTL_INTERNAL_REP_OPT_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -19,26 +18,34 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< unsigned Max, typename... Rules >
          struct rep_opt
+            : rep_opt< Max, seq< Rules... > >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT, Rules... >;
+         };
+
+         template< unsigned Max, typename Rule >
+         struct rep_opt< Max, Rule >
+         {
+            using analyze_t = analysis::generic< analysis::rule_type::opt, Rule >;
 
             template< apply_mode A,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               for( unsigned i = 0; ( i != Max ) && duseltronik< seq< Rules... >, A, rewind_mode::REQUIRED, Action, Control >::match( in, st... ); ++i ) {
+               for( unsigned i = 0; ( i != Max ) && Control< Rule >::template match< A, rewind_mode::required, Action, Control >( in, st... ); ++i ) {
                }
                return true;
             }
          };
 
          template< unsigned Max, typename... Rules >
          struct skip_control< rep_opt< Max, Rules... > > : std::true_type
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/require.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/require.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2016-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_REQUIRE_HPP
 #define TAO_PEGTL_INTERNAL_REQUIRE_HPP
 
 #include "../config.hpp"
 
@@ -25,15 +25,15 @@
             : trivial< true >
          {
          };
 
          template< unsigned Amount >
          struct require
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept( noexcept( in.size( 0 ) ) )
             {
                return in.size( Amount ) >= Amount;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/apply_mode.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_RESULT_ON_FOUND_HPP
-#define TAO_PEGTL_INTERNAL_RESULT_ON_FOUND_HPP
+#ifndef TAO_PEGTL_APPLY_MODE_HPP
+#define TAO_PEGTL_APPLY_MODE_HPP
 
-#include "../config.hpp"
+#include "config.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace internal
+      enum class apply_mode : bool
       {
-         enum class result_on_found : bool
-         {
-            SUCCESS = true,
-            FAILURE = false
-         };
+         action = true,
+         nothing = false,
 
-      }  // namespace internal
+         // Compatibility, remove with 3.0.0
+         ACTION = action,
+         NOTHING = nothing
+      };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/change_action_and_states.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,83 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2019-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_RULE_CONJUNCTION_HPP
-#define TAO_PEGTL_INTERNAL_RULE_CONJUNCTION_HPP
+#ifndef TAO_PEGTL_CHANGE_ACTION_AND_STATES_HPP
+#define TAO_PEGTL_CHANGE_ACTION_AND_STATES_HPP
 
-#include "../apply_mode.hpp"
-#include "../config.hpp"
-#include "../rewind_mode.hpp"
+#include <tuple>
+#include <type_traits>
+
+#include "apply_mode.hpp"
+#include "config.hpp"
+#include "nothing.hpp"
+#include "rewind_mode.hpp"
+
+#include "internal/integer_sequence.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace internal
+      template< template< typename... > class NewAction, typename... NewStates >
+      struct change_action_and_states
+         : maybe_nothing
       {
-         template< typename... Rules >
-         struct rule_conjunction;
-
-         template<>
-         struct rule_conjunction<>
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   std::size_t... Ns,
+                   typename Input,
+                   typename... States >
+         static bool match( TAO_PEGTL_NAMESPACE::internal::index_sequence< Ns... >, Input& in, States&&... st )
          {
-            template< apply_mode A,
-                      rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
-                      typename Input,
-                      typename... States >
-            static bool match( Input& /*unused*/, States&&... /*unused*/ ) noexcept
-            {
+            auto t = std::tie( st... );
+            if( Control< Rule >::template match< A, M, NewAction, Control >( in, std::get< Ns >( t )... ) ) {
+               Action< Rule >::success( static_cast< const Input& >( in ), st... );
                return true;
             }
-         };
+            return false;
+         }
 
-         template< typename... Rules >
-         struct rule_conjunction
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   typename Input,
+                   typename... States >
+         static auto match( Input& in, States&&... st )
+            -> typename std::enable_if< ( A == apply_mode::action ), bool >::type
          {
-            template< apply_mode A,
-                      rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
-                      typename Input,
-                      typename... States >
-            static bool match( Input& in, States&&... st )
-            {
-#ifdef __cpp_fold_expressions
-               return ( Control< Rules >::template match< A, M, Action, Control >( in, st... ) && ... );
-#else
-               bool result = true;
-               using swallow = bool[];
-               (void)swallow{ result = result && Control< Rules >::template match< A, M, Action, Control >( in, st... )... };
-               return result;
-#endif
-            }
-         };
-
-      }  // namespace internal
+            static_assert( !std::is_same< Action< void >, NewAction< void > >::value, "old and new action class templates are identical" );
+            return match< Rule, A, M, Action, Control >( TAO_PEGTL_NAMESPACE::internal::index_sequence_for< NewStates... >(), in, NewStates()..., st... );
+         }
+
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   typename Input,
+                   typename... States,
+                   int = 1 >
+         static auto match( Input& in, States&&... /*unused*/ )
+            -> typename std::enable_if< ( A == apply_mode::nothing ), bool >::type
+         {
+            static_assert( !std::is_same< Action< void >, NewAction< void > >::value, "old and new action class templates are identical" );
+            return Control< Rule >::template match< A, M, NewAction, Control >( in, NewStates()... );
+         }
+      };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/rules.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/rules.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_RULES_HPP
 #define TAO_PEGTL_INTERNAL_RULES_HPP
 
 #include "action.hpp"
 #include "alnum.hpp"
@@ -27,25 +27,25 @@
 #include "if_must_else.hpp"
 #include "if_then_else.hpp"
 #include "istring.hpp"
 #include "list.hpp"
 #include "list_must.hpp"
 #include "list_tail.hpp"
 #include "list_tail_pad.hpp"
-#include "minus.hpp"
 #include "must.hpp"
 #include "not_at.hpp"
 #include "one.hpp"
 #include "opt.hpp"
 #include "pad.hpp"
 #include "pad_opt.hpp"
 #include "plus.hpp"
 #include "raise.hpp"
 #include "range.hpp"
 #include "ranges.hpp"
+#include "rematch.hpp"
 #include "rep.hpp"
 #include "rep_min.hpp"
 #include "rep_min_max.hpp"
 #include "rep_opt.hpp"
 #include "require.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/seq.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/opt.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_SEQ_HPP
-#define TAO_PEGTL_INTERNAL_SEQ_HPP
+#ifndef TAO_PEGTL_INTERNAL_OPT_HPP
+#define TAO_PEGTL_INTERNAL_OPT_HPP
+
+#include <type_traits>
 
 #include "../config.hpp"
 
-#include "rule_conjunction.hpp"
+#include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -18,60 +20,47 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename... Rules >
-         struct seq;
+         struct opt
+            : opt< seq< Rules... > >
+         {
+         };
 
          template<>
-         struct seq<>
+         struct opt<>
             : trivial< true >
          {
          };
 
          template< typename Rule >
-         struct seq< Rule >
-         {
-            using analyze_t = typename Rule::analyze_t;
-
-            template< apply_mode A,
-                      rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
-                      typename Input,
-                      typename... States >
-            static bool match( Input& in, States&&... st )
-            {
-               return Control< Rule >::template match< A, M, Action, Control >( in, st... );
-            }
-         };
-
-         template< typename... Rules >
-         struct seq
+         struct opt< Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::opt, Rule >;
 
             template< apply_mode A,
-                      rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      rewind_mode,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               auto m = in.template mark< M >();
-               using m_t = decltype( m );
-               return m( rule_conjunction< Rules... >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) );
+               Control< Rule >::template match< A, rewind_mode::required, Action, Control >( in, st... );
+               return true;
             }
          };
 
          template< typename... Rules >
-         struct skip_control< seq< Rules... > > : std::true_type
+         struct skip_control< opt< Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_SKIP_CONTROL_HPP
 #define TAO_PEGTL_INTERNAL_SKIP_CONTROL_HPP
 
 #include <type_traits>
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/sor.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/sor.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_SOR_HPP
 #define TAO_PEGTL_INTERNAL_SOR_HPP
 
 #include "../config.hpp"
 
@@ -35,30 +35,32 @@
             : sor< index_sequence_for< Rules... >, Rules... >
          {
          };
 
          template< std::size_t... Indices, typename... Rules >
          struct sor< index_sequence< Indices... >, Rules... >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SOR, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::sor, Rules... >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
 #ifdef __cpp_fold_expressions
-               return ( Control< Rules >::template match < A, ( Indices == ( sizeof...( Rules ) - 1 ) ) ? M : rewind_mode::REQUIRED, Action, Control > ( in, st... ) || ... );
+               return ( Control< Rules >::template match < A, ( Indices == ( sizeof...( Rules ) - 1 ) ) ? M : rewind_mode::required, Action, Control > ( in, st... ) || ... );
 #else
                bool result = false;
                using swallow = bool[];
-               (void)swallow{ result = result || Control< Rules >::template match < A, ( Indices == ( sizeof...( Rules ) - 1 ) ) ? M : rewind_mode::REQUIRED, Action, Control > ( in, st... )... };
+               (void)swallow{ result = result || Control< Rules >::template match < A, ( Indices == ( sizeof...( Rules ) - 1 ) ) ? M : rewind_mode::required, Action, Control > ( in, st... )... };
                return result;
 #endif
             }
          };
 
          template< typename... Rules >
          struct skip_control< sor< Rules... > > : std::true_type
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/star.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_STAR_HPP
-#define TAO_PEGTL_INTERNAL_STAR_HPP
-
-#include <type_traits>
+#ifndef TAO_PEGTL_INTERNAL_IF_MUST_HPP
+#define TAO_PEGTL_INTERNAL_IF_MUST_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
-#include "seq.hpp"
+#include "must.hpp"
 #include "skip_control.hpp"
+#include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
-#include "../analysis/generic.hpp"
+#include "../analysis/counted.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Rule, typename... Rules >
-         struct star
+         template< bool Default, typename Cond, typename... Rules >
+         struct if_must
          {
-            using analyze_t = analysis::generic< analysis::rule_type::OPT, Rule, Rules..., star >;
+            using analyze_t = analysis::counted< analysis::rule_type::seq, Default ? 0 : 1, Cond, must< Rules... > >;
 
             template< apply_mode A,
-                      rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      rewind_mode M,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
-               while( seq< Rule, Rules... >::template match< A, rewind_mode::REQUIRED, Action, Control >( in, st... ) ) {
+               if( Control< Cond >::template match< A, M, Action, Control >( in, st... ) ) {
+                  Control< must< Rules... > >::template match< A, M, Action, Control >( in, st... );
+                  return true;
                }
-               return true;
+               return Default;
             }
          };
 
-         template< typename Rule, typename... Rules >
-         struct skip_control< star< Rule, Rules... > > : std::true_type
+         template< bool Default, typename Cond, typename... Rules >
+         struct skip_control< if_must< Default, Cond, Rules... > > : std::true_type
          {
          };
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_STAR_MUST_HPP
-#define TAO_PEGTL_INTERNAL_STAR_MUST_HPP
+#ifndef TAO_PEGTL_INTERNAL_ALNUM_HPP
+#define TAO_PEGTL_INTERNAL_ALNUM_HPP
 
 #include "../config.hpp"
 
-#include "if_must.hpp"
-#include "star.hpp"
+#include "peek_char.hpp"
+#include "ranges.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
-         template< typename Cond, typename... Rules >
-         using star_must = star< if_must< Cond, Rules... > >;
+         using alnum = ranges< peek_char, 'a', 'z', 'A', 'Z', '0', '9' >;
 
       }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/state.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/state.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_STATE_HPP
 #define TAO_PEGTL_INTERNAL_STATE_HPP
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -19,55 +18,67 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename State, typename... Rules >
          struct state
+            : state< State, seq< Rules... > >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+         };
+
+         template< typename State, typename Rule >
+         struct state< State, Rule >
+         {
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rule >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static auto success( State& s, const Input& in, States&&... st )
                -> decltype( s.template success< A, M, Action, Control >( in, st... ), void() )
             {
                s.template success< A, M, Action, Control >( in, st... );
             }
 
             // NOTE: The additional "int = 0" is a work-around for missing expression SFINAE in VS2015.
 
             template< apply_mode,
                       rewind_mode,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States,
                       int = 0 >
             static auto success( State& s, const Input& in, States&&... st )
                -> decltype( s.success( in, st... ), void() )
             {
                s.success( in, st... );
             }
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                State s( static_cast< const Input& >( in ), st... );
 
-               if( duseltronik< seq< Rules... >, A, M, Action, Control >::match( in, s ) ) {
+               if( Control< Rule >::template match< A, M, Action, Control >( in, s ) ) {
                   success< A, M, Action, Control >( s, in, st... );
                   return true;
                }
                return false;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/string.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/string.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_STRING_HPP
 #define TAO_PEGTL_INTERNAL_STRING_HPP
 
 #include <cstring>
 #include <utility>
@@ -35,22 +35,22 @@
             : trivial< true >
          {
          };
 
          template< char... Cs >
          struct string
          {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, sizeof...( Cs ) >;
+            using analyze_t = analysis::counted< analysis::rule_type::any, sizeof...( Cs ) >;
 
             template< typename Input >
             static bool match( Input& in ) noexcept( noexcept( in.size( 0 ) ) )
             {
                if( in.size( sizeof...( Cs ) ) >= sizeof...( Cs ) ) {
                   if( unsafe_equals( in.current(), { Cs... } ) ) {
-                     bump_help< result_on_found::SUCCESS, Input, char, Cs... >( in, sizeof...( Cs ) );
+                     bump_help< result_on_found::success, Input, char, Cs... >( in, sizeof...( Cs ) );
                      return true;
                   }
                }
                return false;
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/enable_action.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2019-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_INTERNAL_TRIVIAL_HPP
-#define TAO_PEGTL_INTERNAL_TRIVIAL_HPP
+#ifndef TAO_PEGTL_ENABLE_ACTION_HPP
+#define TAO_PEGTL_ENABLE_ACTION_HPP
 
-#include "../config.hpp"
-
-#include "skip_control.hpp"
-
-#include "../analysis/counted.hpp"
+#include "apply_mode.hpp"
+#include "config.hpp"
+#include "match.hpp"
+#include "nothing.hpp"
+#include "rewind_mode.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      namespace internal
+      struct enable_action
+         : maybe_nothing
       {
-         template< bool Result >
-         struct trivial
-         {
-            using analyze_t = analysis::counted< analysis::rule_type::ANY, unsigned( !Result ) >;
-
-            template< typename Input >
-            static bool match( Input& /*unused*/ ) noexcept
-            {
-               return Result;
-            }
-         };
-
-         template< bool Result >
-         struct skip_control< trivial< Result > > : std::true_type
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   typename Input,
+                   typename... States >
+         static bool match( Input& in, States&&... st )
          {
-         };
-
-      }  // namespace internal
+            return TAO_PEGTL_NAMESPACE::match< Rule, apply_mode::action, M, Action, Control >( in, st... );
+         }
+      };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_TRY_CATCH_TYPE_HPP
 #define TAO_PEGTL_INTERNAL_TRY_CATCH_TYPE_HPP
 
 #include <type_traits>
 
 #include "../config.hpp"
 
-#include "duseltronik.hpp"
 #include "seq.hpp"
 #include "skip_control.hpp"
 #include "trivial.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
@@ -21,40 +20,45 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename Exception, typename... Rules >
-         struct try_catch_type;
+         struct try_catch_type
+            : try_catch_type< Exception, seq< Rules... > >
+         {
+         };
 
          template< typename Exception >
          struct try_catch_type< Exception >
             : trivial< true >
          {
          };
 
-         template< typename Exception, typename... Rules >
-         struct try_catch_type
+         template< typename Exception, typename Rule >
+         struct try_catch_type< Exception, Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, Rules... >;
+            using analyze_t = analysis::generic< analysis::rule_type::seq, Rule >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
                using m_t = decltype( m );
 
                try {
-                  return m( duseltronik< seq< Rules... >, A, m_t::next_rewind_mode, Action, Control >::match( in, st... ) );
+                  return m( Control< Rule >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) );
                }
                catch( const Exception& ) {
                   return false;
                }
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/internal/until.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/until.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_INTERNAL_UNTIL_HPP
 #define TAO_PEGTL_INTERNAL_UNTIL_HPP
 
 #include "../config.hpp"
 
 #include "bytes.hpp"
 #include "eof.hpp"
 #include "not_at.hpp"
-#include "rule_conjunction.hpp"
+#include "seq.hpp"
 #include "skip_control.hpp"
 #include "star.hpp"
 
 #include "../apply_mode.hpp"
 #include "../rewind_mode.hpp"
 
 #include "../analysis/generic.hpp"
@@ -21,59 +21,66 @@
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< typename Cond, typename... Rules >
-         struct until;
+         struct until
+            : until< Cond, seq< Rules... > >
+         {
+         };
 
          template< typename Cond >
          struct until< Cond >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, star< not_at< Cond >, not_at< eof >, bytes< 1 > >, Cond >;
+            using analyze_t = analysis::generic< analysis::rule_type::seq, star< not_at< Cond >, not_at< eof >, bytes< 1 > >, Cond >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
 
-               while( !Control< Cond >::template match< A, rewind_mode::REQUIRED, Action, Control >( in, st... ) ) {
+               while( !Control< Cond >::template match< A, rewind_mode::required, Action, Control >( in, st... ) ) {
                   if( in.empty() ) {
                      return false;
                   }
                   in.bump();
                }
                return m( true );
             }
          };
 
-         template< typename Cond, typename... Rules >
-         struct until
+         template< typename Cond, typename Rule >
+         struct until< Cond, Rule >
          {
-            using analyze_t = analysis::generic< analysis::rule_type::SEQ, star< not_at< Cond >, not_at< eof >, Rules... >, Cond >;
+            using analyze_t = analysis::generic< analysis::rule_type::seq, star< not_at< Cond >, not_at< eof >, Rule >, Cond >;
 
             template< apply_mode A,
                       rewind_mode M,
-                      template< typename... > class Action,
-                      template< typename... > class Control,
+                      template< typename... >
+                      class Action,
+                      template< typename... >
+                      class Control,
                       typename Input,
                       typename... States >
             static bool match( Input& in, States&&... st )
             {
                auto m = in.template mark< M >();
                using m_t = decltype( m );
 
-               while( !Control< Cond >::template match< A, rewind_mode::REQUIRED, Action, Control >( in, st... ) ) {
-                  if( in.empty() || ( !rule_conjunction< Rules... >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) ) {
+               while( !Control< Cond >::template match< A, rewind_mode::required, Action, Control >( in, st... ) ) {
+                  if( !Control< Rule >::template match< A, m_t::next_rewind_mode, Action, Control >( in, st... ) ) {
                      return false;
                   }
                }
                return m( true );
             }
          };
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/istream_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/discard_input_on_success.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2019-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_ISTREAM_INPUT_HPP
-#define TAO_PEGTL_ISTREAM_INPUT_HPP
+#ifndef TAO_PEGTL_DISCARD_INPUT_ON_SUCCESS_HPP
+#define TAO_PEGTL_DISCARD_INPUT_ON_SUCCESS_HPP
 
-#include <istream>
-
-#include "buffer_input.hpp"
+#include "apply_mode.hpp"
 #include "config.hpp"
-#include "eol.hpp"
-
-#include "internal/istream_reader.hpp"
+#include "match.hpp"
+#include "nothing.hpp"
+#include "rewind_mode.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      template< typename Eol = eol::lf_crlf >
-      struct istream_input
-         : buffer_input< internal::istream_reader, Eol >
+      struct discard_input_on_success
+         : maybe_nothing
       {
-         template< typename T >
-         istream_input( std::istream& in_stream, const std::size_t in_maximum, T&& in_source )
-            : buffer_input< internal::istream_reader, Eol >( std::forward< T >( in_source ), in_maximum, in_stream )
+         template< typename Rule,
+                   apply_mode A,
+                   rewind_mode M,
+                   template< typename... >
+                   class Action,
+                   template< typename... >
+                   class Control,
+                   typename Input,
+                   typename... States >
+         static bool match( Input& in, States&&... st )
          {
+            const bool result = TAO_PEGTL_NAMESPACE::match< Rule, A, M, Action, Control >( in, st... );
+            if( result ) {
+               in.discard();
+            }
+            return result;
          }
       };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/memory_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/memory_input.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,63 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_MEMORY_INPUT_HPP
 #define TAO_PEGTL_MEMORY_INPUT_HPP
 
 #include <cstddef>
+#include <cstdint>
 #include <cstring>
 #include <string>
 #include <type_traits>
 #include <utility>
 
 #include "config.hpp"
 #include "eol.hpp"
+#include "normal.hpp"
+#include "nothing.hpp"
 #include "position.hpp"
 #include "tracking_mode.hpp"
 
 #include "internal/action_input.hpp"
-#include "internal/bump_impl.hpp"
+#include "internal/at.hpp"
+#include "internal/bump.hpp"
+#include "internal/eolf.hpp"
 #include "internal/iterator.hpp"
 #include "internal/marker.hpp"
+#include "internal/until.hpp"
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
          template< tracking_mode, typename Eol, typename Source >
          class memory_input_base;
 
          template< typename Eol, typename Source >
-         class memory_input_base< tracking_mode::IMMEDIATE, Eol, Source >
+         class memory_input_base< tracking_mode::eager, Eol, Source >
          {
          public:
             using iterator_t = internal::iterator;
 
             template< typename T >
             memory_input_base( const iterator_t& in_begin, const char* in_end, T&& in_source ) noexcept( std::is_nothrow_constructible< Source, T&& >::value )
-               : m_current( in_begin ),
+               : m_begin( in_begin.data ),
+                 m_current( in_begin ),
                  m_end( in_end ),
                  m_source( std::forward< T >( in_source ) )
             {
             }
 
             template< typename T >
             memory_input_base( const char* in_begin, const char* in_end, T&& in_source ) noexcept( std::is_nothrow_constructible< Source, T&& >::value )
-               : m_current( in_begin ),
+               : m_begin( in_begin ),
+                 m_current( in_begin ),
                  m_end( in_end ),
                  m_source( std::forward< T >( in_source ) )
             {
             }
 
             memory_input_base( const memory_input_base& ) = delete;
             memory_input_base( memory_input_base&& ) = delete;
@@ -60,14 +68,19 @@
             memory_input_base operator=( memory_input_base&& ) = delete;
 
             const char* current() const noexcept
             {
                return m_current.data;
             }
 
+            const char* begin() const noexcept
+            {
+               return m_begin;
+            }
+
             const char* end( const std::size_t /*unused*/ = 0 ) const noexcept
             {
                return m_end;
             }
 
             std::size_t byte() const noexcept
             {
@@ -100,22 +113,31 @@
             }
 
             TAO_PEGTL_NAMESPACE::position position( const iterator_t& it ) const
             {
                return TAO_PEGTL_NAMESPACE::position( it, m_source );
             }
 
+            void restart( const std::size_t in_byte = 0, const std::size_t in_line = 1, const std::size_t in_byte_in_line = 0 )
+            {
+               m_current.data = m_begin;
+               m_current.byte = in_byte;
+               m_current.line = in_line;
+               m_current.byte_in_line = in_byte_in_line;
+            }
+
          protected:
+            const char* const m_begin;
             iterator_t m_current;
             const char* const m_end;
             const Source m_source;
          };
 
          template< typename Eol, typename Source >
-         class memory_input_base< tracking_mode::LAZY, Eol, Source >
+         class memory_input_base< tracking_mode::lazy, Eol, Source >
          {
          public:
             using iterator_t = const char*;
 
             template< typename T >
             memory_input_base( const internal::iterator& in_begin, const char* in_end, T&& in_source ) noexcept( std::is_nothrow_constructible< Source, T&& >::value )
                : m_begin( in_begin ),
@@ -143,14 +165,19 @@
             memory_input_base operator=( memory_input_base&& ) = delete;
 
             const char* current() const noexcept
             {
                return m_current;
             }
 
+            const char* begin() const noexcept
+            {
+               return m_begin.data;
+            }
+
             const char* end( const std::size_t /*unused*/ = 0 ) const noexcept
             {
                return m_end;
             }
 
             std::size_t byte() const noexcept
             {
@@ -175,24 +202,29 @@
             TAO_PEGTL_NAMESPACE::position position( const iterator_t it ) const
             {
                internal::iterator c( m_begin );
                internal::bump( c, std::size_t( it - m_begin.data ), Eol::ch );
                return TAO_PEGTL_NAMESPACE::position( c, m_source );
             }
 
+            void restart()
+            {
+               m_current = m_begin.data;
+            }
+
          protected:
             const internal::iterator m_begin;
             iterator_t m_current;
             const char* const m_end;
             const Source m_source;
          };
 
       }  // namespace internal
 
-      template< tracking_mode P = tracking_mode::IMMEDIATE, typename Eol = eol::lf_crlf, typename Source = std::string >
+      template< tracking_mode P = tracking_mode::eager, typename Eol = eol::lf_crlf, typename Source = std::string >
       class memory_input
          : public internal::memory_input_base< P, Eol, Source >
       {
       public:
          static constexpr tracking_mode tracking_mode_v = P;
 
          using eol_t = Eol;
@@ -255,29 +287,43 @@
          }
 
          char peek_char( const std::size_t offset = 0 ) const noexcept
          {
             return this->current()[ offset ];
          }
 
-         unsigned char peek_byte( const std::size_t offset = 0 ) const noexcept
+         std::uint8_t peek_uint8( const std::size_t offset = 0 ) const noexcept
          {
-            return static_cast< unsigned char >( peek_char( offset ) );
+            return static_cast< std::uint8_t >( peek_char( offset ) );
+         }
+
+         // Compatibility, remove with 3.0.0
+         std::uint8_t peek_byte( const std::size_t offset = 0 ) const noexcept
+         {
+            return static_cast< std::uint8_t >( peek_char( offset ) );
          }
 
          iterator_t& iterator() noexcept
          {
             return this->m_current;
          }
 
          const iterator_t& iterator() const noexcept
          {
             return this->m_current;
          }
 
+         using internal::memory_input_base< P, Eol, Source >::restart;
+
+         template< rewind_mode M >
+         void restart( const internal::marker< iterator_t, M >& m )
+         {
+            iterator() = m.iterator();
+         }
+
          using internal::memory_input_base< P, Eol, Source >::position;
 
          TAO_PEGTL_NAMESPACE::position position() const
          {
             return position( iterator() );
          }
 
@@ -290,14 +336,43 @@
          }
 
          template< rewind_mode M >
          internal::marker< iterator_t, M > mark() noexcept
          {
             return internal::marker< iterator_t, M >( iterator() );
          }
+
+         const char* at( const TAO_PEGTL_NAMESPACE::position& p ) const noexcept
+         {
+            return this->begin() + p.byte;
+         }
+
+         const char* begin_of_line( const TAO_PEGTL_NAMESPACE::position& p ) const noexcept
+         {
+            return at( p ) - p.byte_in_line;
+         }
+
+         const char* end_of_line( const TAO_PEGTL_NAMESPACE::position& p ) const noexcept
+         {
+            using input_t = memory_input< tracking_mode::lazy, Eol, const char* >;
+            input_t in( at( p ), this->end(), "" );
+            using grammar = internal::until< internal::at< internal::eolf > >;
+            normal< grammar >::match< apply_mode::nothing, rewind_mode::dontcare, nothing, normal >( in );
+            return in.current();
+         }
+
+         std::string line_at( const TAO_PEGTL_NAMESPACE::position& p ) const
+         {
+            return std::string( begin_of_line( p ), end_of_line( p ) );
+         }
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      memory_input( Ts&&... )->memory_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/mmap_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/mmap_input.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_MMAP_INPUT_HPP
 #define TAO_PEGTL_MMAP_INPUT_HPP
 
 #include <string>
 #include <utility>
 
 #include "config.hpp"
 #include "eol.hpp"
 #include "memory_input.hpp"
 #include "tracking_mode.hpp"
 
-#include "internal/file_mapper.hpp"
+#if defined( __unix__ ) || ( defined( __APPLE__ ) && defined( __MACH__ ) )
+#include <unistd.h>  // Required for _POSIX_MAPPED_FILES
+#endif
+
+#if defined( _POSIX_MAPPED_FILES )
+#include "internal/file_mapper_posix.hpp"
+#elif defined( _WIN32 )
+#include "internal/file_mapper_win32.hpp"
+#else
+#endif
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace internal
       {
@@ -39,15 +48,15 @@
 
             void operator=( const mmap_holder& ) = delete;
             void operator=( mmap_holder&& ) = delete;
          };
 
       }  // namespace internal
 
-      template< tracking_mode P = tracking_mode::IMMEDIATE, typename Eol = eol::lf_crlf >
+      template< tracking_mode P = tracking_mode::eager, typename Eol = eol::lf_crlf >
       struct mmap_input
          : private internal::mmap_holder,
            public memory_input< P, Eol, const char* >
       {
          template< typename T >
          explicit mmap_input( T&& in_filename )
             : internal::mmap_holder( std::forward< T >( in_filename ) ),
@@ -60,12 +69,17 @@
 
          ~mmap_input() = default;
 
          void operator=( const mmap_input& ) = delete;
          void operator=( mmap_input&& ) = delete;
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      explicit mmap_input( Ts&&... )->mmap_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/nothing.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/internal/always_false.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2018-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
-#ifndef TAO_PEGTL_NOTHING_HPP
-#define TAO_PEGTL_NOTHING_HPP
+#ifndef TAO_PEGTL_INTERNAL_ALWAYS_FALSE_HPP
+#define TAO_PEGTL_INTERNAL_ALWAYS_FALSE_HPP
 
-#include <type_traits>
+#include "../config.hpp"
 
-#include "config.hpp"
+#include <type_traits>
 
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
-      template< typename Rule >
-      struct nothing
+      namespace internal
       {
-      };
+         template< typename... >
+         struct always_false
+            : std::false_type
+         {
+         };
 
-      template< template< typename... > class Action, typename Rule >
-      using is_nothing = std::is_base_of< nothing< Rule >, Action< Rule > >;
+      }  // namespace internal
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/parse.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/parse.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_PARSE_HPP
 #define TAO_PEGTL_PARSE_HPP
 
+#include <cassert>
+
 #include "apply_mode.hpp"
 #include "config.hpp"
 #include "normal.hpp"
 #include "nothing.hpp"
 #include "parse_error.hpp"
 #include "rewind_mode.hpp"
 
+#include "internal/action_input.hpp"
+
 namespace tao
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       template< typename Rule,
                 template< typename... > class Action = nothing,
                 template< typename... > class Control = normal,
-                apply_mode A = apply_mode::ACTION,
-                rewind_mode M = rewind_mode::REQUIRED,
+                apply_mode A = apply_mode::action,
+                rewind_mode M = rewind_mode::required,
                 typename Input,
                 typename... States >
       bool parse( Input&& in, States&&... st )
       {
          return Control< Rule >::template match< A, M, Action, Control >( in, st... );
       }
 
       template< typename Rule,
                 template< typename... > class Action = nothing,
                 template< typename... > class Control = normal,
-                apply_mode A = apply_mode::ACTION,
-                rewind_mode M = rewind_mode::REQUIRED,
+                apply_mode A = apply_mode::action,
+                rewind_mode M = rewind_mode::required,
                 typename Outer,
                 typename Input,
                 typename... States >
       bool parse_nested( const Outer& oi, Input&& in, States&&... st )
       {
          try {
             return parse< Rule, Action, Control, A, M >( in, st... );
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/parse_error.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/parse_error.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_PARSE_ERROR_HPP
 #define TAO_PEGTL_PARSE_ERROR_HPP
 
 #include <stdexcept>
 #include <vector>
@@ -31,14 +31,20 @@
 
          parse_error( const std::string& msg, const position& pos )
             : std::runtime_error( to_string( pos ) + ": " + msg ),
               positions( 1, pos )
          {
          }
 
+         parse_error( const std::string& msg, position&& pos )
+            : std::runtime_error( to_string( pos ) + ": " + msg )
+         {
+            positions.emplace_back( std::move( pos ) );
+         }
+
          std::vector< position > positions;
       };
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/position.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/position.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_POSITION_HPP
 #define TAO_PEGTL_POSITION_HPP
 
 #include <cstdlib>
 #include <ostream>
@@ -33,16 +33,15 @@
          std::size_t line;
          std::size_t byte_in_line;
          std::string source;
       };
 
       inline std::ostream& operator<<( std::ostream& o, const position& p )
       {
-         //return o << p.source << ':' << p.line << ':' << p.byte_in_line << '(' << p.byte << ')';
-         return o << p.source << ':' << p.line << ':' << p.byte_in_line + 1;
+         return o << p.source << ':' << p.line << ':' << p.byte_in_line << '(' << p.byte << ')';
       }
 
       inline std::string to_string( const position& p )
       {
          std::ostringstream o;
          o << p;
          return o.str();
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/read_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/read_input.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_READ_INPUT_HPP
 #define TAO_PEGTL_READ_INPUT_HPP
 
 #include <string>
 
@@ -36,15 +36,15 @@
 
             void operator=( const filename_holder& ) = delete;
             void operator=( filename_holder&& ) = delete;
          };
 
       }  // namespace internal
 
-      template< tracking_mode P = tracking_mode::IMMEDIATE, typename Eol = eol::lf_crlf >
+      template< tracking_mode P = tracking_mode::eager, typename Eol = eol::lf_crlf >
       struct read_input
          : private internal::filename_holder,
            public string_input< P, Eol, const char* >
       {
          template< typename T >
          explicit read_input( T&& in_filename )
             : internal::filename_holder( std::forward< T >( in_filename ) ),
@@ -64,12 +64,17 @@
 
          ~read_input() = default;
 
          void operator=( const read_input& ) = delete;
          void operator=( read_input&& ) = delete;
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      explicit read_input( Ts&&... )->read_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/rules.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/rules.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_RULES_HPP
 #define TAO_PEGTL_RULES_HPP
 
 #include "config.hpp"
 #include "parse_error.hpp"
@@ -24,45 +24,47 @@
       template< template< typename... > class Control, typename... Rules > struct control : internal::control< Control, Rules... > {};
       template< typename... Rules > struct disable : internal::disable< Rules... > {};
       struct discard : internal::discard {};
       template< typename... Rules > struct enable : internal::enable< Rules... > {};
       struct eof : internal::eof {};
       struct failure : internal::trivial< false > {};
       template< typename Rule, typename... Actions > struct if_apply : internal::if_apply< Rule, Actions... > {};
-      template< typename Cond, typename... Thens > struct if_must : internal::if_must< Cond, Thens... > {};
+      template< typename Cond, typename... Thens > struct if_must : internal::if_must< false, Cond, Thens... > {};
       template< typename Cond, typename Then, typename Else > struct if_must_else : internal::if_must_else< Cond, Then, Else > {};
       template< typename Cond, typename Then, typename Else > struct if_then_else : internal::if_then_else< Cond, Then, Else > {};
       template< typename Rule, typename Sep, typename Pad = void > struct list : internal::list< Rule, internal::pad< Sep, Pad > > {};
       template< typename Rule, typename Sep > struct list< Rule, Sep, void > : internal::list< Rule, Sep > {};
       template< typename Rule, typename Sep, typename Pad = void > struct list_must : internal::list_must< Rule, internal::pad< Sep, Pad > > {};
       template< typename Rule, typename Sep > struct list_must< Rule, Sep, void > : internal::list_must< Rule, Sep > {};
       template< typename Rule, typename Sep, typename Pad = void > struct list_tail : internal::list_tail_pad< Rule, Sep, Pad > {};
       template< typename Rule, typename Sep > struct list_tail< Rule, Sep, void > : internal::list_tail< Rule, Sep > {};
-      template< typename M, typename S > struct minus : internal::minus< M, S > {};
+      template< typename M, typename S > struct minus : internal::rematch< M, internal::not_at< S, internal::eof > > {};
       template< typename... Rules > struct must : internal::must< Rules... > {};
       template< typename... Rules > struct not_at : internal::not_at< Rules... > {};
       template< typename... Rules > struct opt : internal::opt< Rules... > {};
+      template< typename Cond, typename... Rules > struct opt_must : internal::if_must< true, Cond, Rules... > {};
       template< typename Rule, typename Pad1, typename Pad2 = Pad1 > struct pad : internal::pad< Rule, Pad1, Pad2 > {};
       template< typename Rule, typename Pad > struct pad_opt : internal::pad_opt< Rule, Pad > {};
       template< typename Rule, typename... Rules > struct plus : internal::plus< Rule, Rules... > {};
       template< typename Exception > struct raise : internal::raise< Exception > {};
+      template< typename Head, typename... Rules > struct rematch : internal::rematch< Head, Rules... > {};
       template< unsigned Num, typename... Rules > struct rep : internal::rep< Num, Rules... > {};
       template< unsigned Max, typename... Rules > struct rep_max : internal::rep_min_max< 0, Max, Rules... > {};
       template< unsigned Min, typename Rule, typename... Rules > struct rep_min : internal::rep_min< Min, Rule, Rules... > {};
       template< unsigned Min, unsigned Max, typename... Rules > struct rep_min_max : internal::rep_min_max< Min, Max, Rules... > {};
       template< unsigned Max, typename... Rules > struct rep_opt : internal::rep_opt< Max, Rules... > {};
       template< unsigned Amount > struct require : internal::require< Amount > {};
       template< typename... Rules > struct seq : internal::seq< Rules... > {};
       template< typename... Rules > struct sor : internal::sor< Rules... > {};
       template< typename Rule, typename... Rules > struct star : internal::star< Rule, Rules... > {};
       template< typename Cond, typename... Rules > struct star_must : internal::star_must< Cond, Rules... > {};
       template< typename State, typename... Rules > struct state : internal::state< State, Rules... > {};
       struct success : internal::trivial< true > {};
-      template< typename... Rules > struct try_catch : internal::try_catch_type< parse_error, Rules... > {};
-      template< typename Exception, typename... Rules > struct try_catch_type : internal::try_catch_type< Exception, Rules... > {};
+      template< typename... Rules > struct try_catch : internal::seq< internal::try_catch_type< parse_error, Rules... > > {};
+      template< typename Exception, typename... Rules > struct try_catch_type : internal::seq< internal::try_catch_type< Exception, Rules... > > {};
       template< typename Cond, typename... Rules > struct until : internal::until< Cond, Rules... > {};
       // clang-format on
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/string_input.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/string_input.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_STRING_INPUT_HPP
 #define TAO_PEGTL_STRING_INPUT_HPP
 
 #include <string>
 #include <utility>
@@ -35,15 +35,15 @@
 
             void operator=( const string_holder& ) = delete;
             void operator=( string_holder&& ) = delete;
          };
 
       }  // namespace internal
 
-      template< tracking_mode P = tracking_mode::IMMEDIATE, typename Eol = eol::lf_crlf, typename Source = std::string >
+      template< tracking_mode P = tracking_mode::eager, typename Eol = eol::lf_crlf, typename Source = std::string >
       struct string_input
          : private internal::string_holder,
            public memory_input< P, Eol, Source >
       {
          template< typename V, typename T, typename... Ts >
          explicit string_input( V&& in_data, T&& in_source, Ts&&... ts )
             : internal::string_holder( std::forward< V >( in_data ) ),
@@ -56,12 +56,17 @@
 
          ~string_input() = default;
 
          void operator=( const string_input& ) = delete;
          void operator=( string_input&& ) = delete;
       };
 
+#ifdef __cpp_deduction_guides
+      template< typename... Ts >
+      explicit string_input( Ts&&... )->string_input<>;
+#endif
+
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf16.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf16.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2015-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2015-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_UTF16_HPP
 #define TAO_PEGTL_UTF16_HPP
 
 #include "config.hpp"
 
@@ -14,40 +14,40 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace utf16_be
       {
          // clang-format off
          struct any : internal::any< internal::peek_utf16_be > {};
-         struct bom : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_be, 0xfeff > {};
-         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_utf16_be, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_utf16_be, Lo, Hi > {};
-         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_be, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_utf16_be, Lo, Hi > {};
+         struct bom : internal::one< internal::result_on_found::success, internal::peek_utf16_be, 0xfeff > {};
+         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_utf16_be, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_utf16_be, Lo, Hi > {};
+         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_utf16_be, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_utf16_be, Lo, Hi > {};
          template< char32_t... Cs > struct ranges : internal::ranges< internal::peek_utf16_be, Cs... > {};
-         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_be, Cs >... > {};
+         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::success, internal::peek_utf16_be, Cs >... > {};
          // clang-format on
 
       }  // namespace utf16_be
 
       namespace utf16_le
       {
          // clang-format off
          struct any : internal::any< internal::peek_utf16_le > {};
-         struct bom : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_le, 0xfeff > {};
-         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_utf16_le, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_utf16_le, Lo, Hi > {};
-         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_le, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_utf16_le, Lo, Hi > {};
+         struct bom : internal::one< internal::result_on_found::success, internal::peek_utf16_le, 0xfeff > {};
+         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_utf16_le, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_utf16_le, Lo, Hi > {};
+         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_utf16_le, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_utf16_le, Lo, Hi > {};
          template< char32_t... Cs > struct ranges : internal::ranges< internal::peek_utf16_le, Cs... > {};
-         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::SUCCESS, internal::peek_utf16_le, Cs >... > {};
+         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::success, internal::peek_utf16_le, Cs >... > {};
          // clang-format on
 
       }  // namespace utf16_le
 
-      namespace utf16 = TAO_PEGTL_NATIVE_UTF16;  // NOLINT(misc-unused-alias-decls)
+      namespace utf16 = TAO_PEGTL_NATIVE_UTF16;
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf32.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf32.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_UTF32_HPP
 #define TAO_PEGTL_UTF32_HPP
 
 #include "config.hpp"
 
@@ -14,40 +14,40 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace utf32_be
       {
          // clang-format off
          struct any : internal::any< internal::peek_utf32_be > {};
-         struct bom : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_be, 0xfeff > {};
-         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_utf32_be, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_utf32_be, Lo, Hi > {};
-         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_be, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_utf32_be, Lo, Hi > {};
+         struct bom : internal::one< internal::result_on_found::success, internal::peek_utf32_be, 0xfeff > {};
+         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_utf32_be, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_utf32_be, Lo, Hi > {};
+         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_utf32_be, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_utf32_be, Lo, Hi > {};
          template< char32_t... Cs > struct ranges : internal::ranges< internal::peek_utf32_be, Cs... > {};
-         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_be, Cs >... > {};
+         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::success, internal::peek_utf32_be, Cs >... > {};
          // clang-format on
 
       }  // namespace utf32_be
 
       namespace utf32_le
       {
          // clang-format off
          struct any : internal::any< internal::peek_utf32_le > {};
-         struct bom : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_le, 0xfeff > {};
-         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_utf32_le, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_utf32_le, Lo, Hi > {};
-         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_le, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_utf32_le, Lo, Hi > {};
+         struct bom : internal::one< internal::result_on_found::success, internal::peek_utf32_le, 0xfeff > {};
+         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_utf32_le, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_utf32_le, Lo, Hi > {};
+         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_utf32_le, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_utf32_le, Lo, Hi > {};
          template< char32_t... Cs > struct ranges : internal::ranges< internal::peek_utf32_le, Cs... > {};
-         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::SUCCESS, internal::peek_utf32_le, Cs >... > {};
+         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::success, internal::peek_utf32_le, Cs >... > {};
          // clang-format on
 
       }  // namespace utf32_le
 
-      namespace utf32 = TAO_PEGTL_NATIVE_UTF32;  // NOLINT(misc-unused-alias-decls)
+      namespace utf32 = TAO_PEGTL_NATIVE_UTF32;
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/utf8.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/utf8.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2014-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2014-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_UTF8_HPP
 #define TAO_PEGTL_UTF8_HPP
 
 #include "config.hpp"
 
@@ -14,21 +14,21 @@
 {
    namespace TAO_PEGTL_NAMESPACE
    {
       namespace utf8
       {
          // clang-format off
          struct any : internal::any< internal::peek_utf8 > {};
-         struct bom : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf8, 0xfeff > {};
-         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::FAILURE, internal::peek_utf8, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::FAILURE, internal::peek_utf8, Lo, Hi > {};
-         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::SUCCESS, internal::peek_utf8, Cs... > {};
-         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::SUCCESS, internal::peek_utf8, Lo, Hi > {};
+         struct bom : internal::one< internal::result_on_found::success, internal::peek_utf8, 0xfeff > {};
+         template< char32_t... Cs > struct not_one : internal::one< internal::result_on_found::failure, internal::peek_utf8, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct not_range : internal::range< internal::result_on_found::failure, internal::peek_utf8, Lo, Hi > {};
+         template< char32_t... Cs > struct one : internal::one< internal::result_on_found::success, internal::peek_utf8, Cs... > {};
+         template< char32_t Lo, char32_t Hi > struct range : internal::range< internal::result_on_found::success, internal::peek_utf8, Lo, Hi > {};
          template< char32_t... Cs > struct ranges : internal::ranges< internal::peek_utf8, Cs... > {};
-         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::SUCCESS, internal::peek_utf8, Cs >... > {};
+         template< char32_t... Cs > struct string : internal::seq< internal::one< internal::result_on_found::success, internal::peek_utf8, Cs >... > {};
          // clang-format on
 
       }  // namespace utf8
 
    }  // namespace TAO_PEGTL_NAMESPACE
 
 }  // namespace tao
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tao/pegtl/version.hpp` & `gemmi-0.6.6/include/gemmi/third_party/tao/pegtl/version.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-// Copyright (c) 2017-2018 Dr. Colin Hirsch and Daniel Frey
+// Copyright (c) 2017-2020 Dr. Colin Hirsch and Daniel Frey
 // Please see LICENSE for license or visit https://github.com/taocpp/PEGTL/
 
 #ifndef TAO_PEGTL_VERSION_HPP
 #define TAO_PEGTL_VERSION_HPP
 
-#define TAO_PEGTL_VERSION "2.4.0"
+#define TAO_PEGTL_VERSION "2.8.3"
 
 #define TAO_PEGTL_VERSION_MAJOR 2
-#define TAO_PEGTL_VERSION_MINOR 4
-#define TAO_PEGTL_VERSION_PATCH 0
+#define TAO_PEGTL_VERSION_MINOR 8
+#define TAO_PEGTL_VERSION_PATCH 3
 
-// Compatibility, remove with 3.0
+// Compatibility, remove with 3.0.0
 #define TAOCPP_PEGTL_VERSION TAO_PEGTL_VERSION
 #define TAOCPP_PEGTL_VERSION_MAJOR TAO_PEGTL_VERSION_MAJOR
 #define TAOCPP_PEGTL_VERSION_MINOR TAO_PEGTL_VERSION_MINOR
 #define TAOCPP_PEGTL_VERSION_PATCH TAO_PEGTL_VERSION_PATCH
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/third_party/tinydir.h` & `gemmi-0.6.6/include/gemmi/third_party/tinydir.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/to_chemcomp.hpp` & `gemmi-0.6.6/include/gemmi/to_chemcomp.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,15 @@
   {
     std::vector<std::string> tags =
         {"comp_id", "atom_id", "type_symbol", "type_energy", "charge"};
     if (cc.has_coordinates)
       for (char c = 'x'; c <= 'z'; ++c)
         tags.emplace_back(1, c);
     cif::Table tab = block.find_or_add("_chem_comp_atom.", tags);
-    if (!tab.loop_item)
-      tab.convert_pair_to_loop();
+    tab.ensure_loop();
     size_t pos = tab.length();
     cif::Loop& loop = tab.loop_item->loop;
     loop.values.resize(loop.values.size() + loop.width() * cc.atoms.size(), ".");
     for (const ChemComp::Atom& a : cc.atoms) {
       cif::Table::Row row = tab[pos++];
       row[0] = cc.name;
       row[1] = a.id;
```

### Comparing `gemmi-0.6.5/include/gemmi/to_cif.hpp` & `gemmi-0.6.6/include/gemmi/to_cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/to_json.hpp` & `gemmi-0.6.6/include/gemmi/to_json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/to_mmcif.hpp` & `gemmi-0.6.6/include/gemmi/to_mmcif.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -62,13 +62,14 @@
                                             MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Block make_mmcif_block(const Structure& st,
                                       MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Block make_mmcif_headers(const Structure& st);
 GEMMI_DLL void add_minimal_mmcif_data(const Structure& st, cif::Block& block);
 
 // temporarily we use it in crd.cpp
+GEMMI_DLL void write_ncs_oper(const Structure& st, cif::Block& block);
 GEMMI_DLL void write_struct_conn(const Structure& st, cif::Block& block);
 GEMMI_DLL void write_cispeps(const Structure& st, cif::Block& block);
 
 } // namespace gemmi
 
 #endif
```

### Comparing `gemmi-0.6.5/include/gemmi/to_pdb.hpp` & `gemmi-0.6.6/include/gemmi/to_pdb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/topo.hpp` & `gemmi-0.6.6/include/gemmi/topo.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/twin.hpp` & `gemmi-0.6.6/include/gemmi/twin.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/unitcell.hpp` & `gemmi-0.6.6/include/gemmi/unitcell.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -331,38 +331,41 @@
     return true;
   }
 
   bool is_compatible_with_spacegroup(const SpaceGroup* sg, double eps=1e-3) {
     return sg ? is_compatible_with_groupops(sg->operations(), eps) : false;
   }
 
-  void set_cell_images_from_spacegroup(const SpaceGroup* sg) {
+  void set_cell_images_from_groupops(const GroupOps& group_ops) {
     images.clear();
-    cs_count = 0;
-    if (!sg)
-      return;
-    GroupOps group_ops = sg->operations();
     cs_count = (short) group_ops.order() - 1;
     images.reserve(cs_count);
-    for (Op op : group_ops) {
-      if (op == Op::identity())
-        continue;
-      images.push_back(Transform{rot_as_mat33(op), tran_as_vec3(op)});
+    for (Op op : group_ops)
+      if (op != Op::identity())
+        images.push_back(Transform{rot_as_mat33(op), tran_as_vec3(op)});
+  }
+
+  void set_cell_images_from_spacegroup(const SpaceGroup* sg) {
+    if (sg) {
+      set_cell_images_from_groupops(sg->operations());
+    } else {
+      images.clear();
+      cs_count = 0;
     }
   }
 
   void add_ncs_images_to_cs_images(const std::vector<NcsOp>& ncs) {
     assert(cs_count == (short) images.size());
     for (const NcsOp& ncs_op : ncs)
       if (!ncs_op.given) {
         // We need it to operates on fractional, not orthogonal coordinates.
         FTransform f = frac.combine(ncs_op.tr.combine(orth));
-        images.emplace_back(f);
+        images.push_back(f);
         for (int i = 0; i < cs_count; ++i)
-          images.emplace_back(images[i].combine(f));
+          images.push_back(images[i].combine(f));
       }
   }
 
   std::vector<FTransform> get_ncs_transforms() const {
     std::vector<FTransform> ncs;
     for (size_t n = cs_count; n < images.size(); n += cs_count + 1)
       ncs.push_back(images[n]);
```

### Comparing `gemmi-0.6.5/include/gemmi/utf.hpp` & `gemmi-0.6.6/include/gemmi/utf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/util.hpp` & `gemmi-0.6.6/include/gemmi/util.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/include/gemmi/xds_ascii.hpp` & `gemmi-0.6.6/include/gemmi/xds_ascii.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/align.cpp` & `gemmi-0.6.6/prog/align.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/blobs.cpp` & `gemmi-0.6.6/prog/blobs.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/cif2json.cpp` & `gemmi-0.6.6/prog/cif2json.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/cif2mtz.cpp` & `gemmi-0.6.6/prog/cif2mtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/cifdiff.cpp` & `gemmi-0.6.6/prog/cifdiff.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 // Copyright 2023 Global Phasing Ltd.
 
 #include <cstdio>   // for printf, fprintf
 #include <algorithm>  // for find
 #include "gemmi/read_cif.hpp"  // for read_cif_gz
+#include "gemmi/pdb_id.hpp"  // for expand_if_pdb_code
 
 #define GEMMI_PROG cifdiff
 #include "options.h"
 
 namespace cif = gemmi::cif;
 
 namespace {
 
 enum OptionIndex {
-  OnlyCategories=4, NoComparison,
+  Tag=4, OnlyCategories, NoComparison,
 };
 
 const option::Descriptor Usage[] = {
   { NoOp, 0, "", "", Arg::None,
     "Usage:\n"
     " " EXE_NAME " [options] FILE1.cif FILE2.cif\n"
     " " EXE_NAME " [options] -n FILE.cif\n\n"
     "Compares (or just prints) categories and tags in CIF files.\n"
     "First block only." },
   CommonUsage[Help],
   CommonUsage[Version],
   CommonUsage[Verbose],
+  { Tag, 0, "t", "", Arg::Required,
+    "  -t TAG \tCompare values of TAG." },
   { OnlyCategories, 0, "q", "", Arg::None,
     "  -q  \tPrint only categories." },
   { NoComparison, 0, "n", "", Arg::None,
     "  -n  \tNo comparison, just list categories and tags." },
   { 0, 0, 0, 0, 0, 0 }
 };
 
@@ -56,44 +59,82 @@
       diff.insert(diff.begin() + idx, DiffItem{'-', s});
       idx++;
     }
   }
   return diff;
 }
 
+void compare_tag_values(cif::Block& b1, cif::Block& b2, const std::string& tag) {
+  printf("  checking %s ...\n", tag.c_str());
+  auto col1 = b1.find_values(tag);
+  auto col2 = b2.find_values(tag);
+  if (!col1 || !col2) {
+    if (!col1)
+      std::printf("    NOT FOUND in file 1 block %s\n", b1.name.c_str());
+    if (!col2)
+      std::printf("    NOT FOUND in file 2 block %s\n", b2.name.c_str());
+    return;
+  }
+  int n1 = col1.length();
+  int n2 = col2.length();
+  int n = std::min(n1, n2);
+  if (n1 != n2) {
+    std::printf("-   number of values: %d\n", n1);
+    std::printf("+   number of values: %d\n", n2);
+    printf("  comparing the first %d values...\n", n);
+  }
+  int diff_count = 0;
+  for (int i = 0; i < n; ++i)
+    if (col1[i] != col2[i] && col1.str(i) != col2.str(i) && diff_count++ < 4) {
+      std::printf("-   value %d: %s\n", i, col1[i].c_str());
+      std::printf("+   value %d: %s\n", i, col2[i].c_str());
+    }
+  if (diff_count >= 4)
+    printf("    ...\n"
+           "  %d of %d values differ\n", diff_count, n);
+  else if (diff_count == 0)
+    printf("  %d identical values\n", n);
+}
+
 } // anonymous namespace
 
 int GEMMI_MAIN(int argc, char **argv) {
   OptParser p(EXE_NAME);
   p.simple_parse(argc, argv, Usage);
+  p.check_exclusive_pair(Tag, NoComparison);
   bool one_file = p.options[NoComparison];
   p.require_positional_args(one_file ? 1 : 2);
   const char* path1 = p.nonOption(0);
   const char* path2 = one_file ? nullptr : p.nonOption(1);
   //int verbose = p.options[Verbose].count();
   try {
     // Starting like an unified diff (with "--- ") enables colordiff.
     printf("%sReading %s\n", one_file ? "" : "--- ", path1);
-    cif::Document doc1 = gemmi::read_cif_or_mmjson_gz(path1);
+    cif::Document doc1 = gemmi::read_cif_or_mmjson_gz(gemmi::expand_if_pdb_code(path1));
     cif::Block* b1 = &doc1.blocks.at(0);
     // NoComparison mode is implemented as comparing Block with itself
     // (inefficient, but simple).
     cif::Document doc2;
     cif::Block* b2 = b1;
     if (!one_file) {
       printf("+++ Reading %s\n", path2);
-      doc2 = gemmi::read_cif_or_mmjson_gz(path2);
+      doc2 = gemmi::read_cif_or_mmjson_gz(gemmi::expand_if_pdb_code(path2));
       b2 = &doc2.blocks.at(0);
     }
     if (b1->name == b2->name) {
       printf("  block name: %s\n", b1->name.c_str());
     } else {
       printf("- block name: %s\n", b1->name.c_str());
       printf("+ block name: %s\n", b2->name.c_str());
     }
+    if (p.options[Tag]) {
+      for (const option::Option* opt = p.options[Tag]; opt; opt = opt->next())
+        compare_tag_values(*b1, *b2, opt->arg);
+      return 0;
+    }
     Diff category_diff = make_diff(b1->get_mmcif_category_names(),
                                    b2->get_mmcif_category_names());
     for (DiffItem& cat : category_diff) {
       cif::Table t1 = b1->find_mmcif_category(cat.str);
       cif::Table t2 = b2->find_mmcif_category(cat.str);
       size_t len1 = t1.length();
       size_t len2 = t2.length();
```

### Comparing `gemmi-0.6.5/prog/cifmod.h` & `gemmi-0.6.6/prog/cifmod.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/contact.cpp` & `gemmi-0.6.6/prog/contact.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/contents.cpp` & `gemmi-0.6.6/prog/contents.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/convert.cpp` & `gemmi-0.6.6/prog/convert.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,34 @@
   static option::ArgStatus AnisouChoice(const option::Option& option, bool msg) {
     return Arg::Choice(option, msg, {"yes", "no", "heavy"});
   }
 
   static option::ArgStatus NcsChoice(const option::Option& option, bool msg) {
     return Arg::Choice(option, msg, {"dup", "num", "x"});
   }
+
+  static option::ArgStatus RecordChoice(const option::Option& option, bool msg) {
+    auto status = Arg::Optional(option, msg);
+    if (status == option::ARG_OK && option.arg[0] != 'A' && option.arg[0] != 'H') {
+      if (msg)
+        fprintf(stderr, "If option %.*s has argument, it must be ATOM or HETATM.\n",
+                option.namelen, option.name);
+      status = option::ARG_ILLEGAL;
+    }
+    return status;
+  }
 };
 
 enum OptionIndex {
   FormatIn=AfterCifModOptions, FormatOut, CifStyle, AllAuth, BlockName,
   ExpandNcs, AsAssembly,
   RemoveH, RemoveWaters, RemoveLigWat, TrimAla, Select, Remove, ApplySymop,
   Reframe, ShortTer, Linkr, CopyRemarks, Minimal, ShortenCN, RenameChain,
-  ShortenTLC, ChangeCcdCode, SetSeq,
-  SiftsNum, Biso, Anisou, SetCis, SegmentAsChain, OldPdb, ForceLabel
+  ShortenTLC, ChangeCcdCode, SetSeq, SiftsNum,
+  Biso, Anisou, AssignRecords, SetCis, SegmentAsChain, OldPdb, ForceLabel
 };
 
 const option::Descriptor Usage[] = {
   { NoOp, 0, "", "", Arg::None,
     "Usage:"
     "\n " EXE_NAME " [options] INPUT_FILE OUTPUT_FILE"
     "\n\nwith possible conversions between PDB, mmCIF and mmJSON."
@@ -106,21 +117,24 @@
   { ShortenTLC, 0, "", "shorten-tlc", Arg::None,
     "  --shorten-tlc  \tChange 5-character monomer names to 3-char. aliases." },
   { ChangeCcdCode, 0, "", "monomer", Arg::ColonPair,
     "  --monomer=OLD:NEW  \tChange monomer name (CCD code) OLD to NEW." },
   { SetSeq, 0, "s", "", Arg::Required,
     "  -s FILE  \tUse sequence(s) from FILE in PIR or FASTA format. Each chain"
     " is assigned the best matching sequence, if any." },
-  { SiftsNum, 0, "", "sifts-num", Arg::None,
-    "  --sifts-num  \tUse SIFTS-mapped position in UniProt sequence as sequence ID." },
+  { SiftsNum, 0, "", "sifts-num", Arg::Optional,
+    "  --sifts-num[=AC]  \tSet sequence ID to SIFTS-mapped UniProt positions."
+    " In chimeric chains use AC. Adds 5000 to other seqnums." },
   { Biso, 0, "B", "", Arg::Required,
     "  -B MIN[:MAX]  \tSet isotropic B-factors to a single value or change values "
       "out of given range to MIN/MAX." },
   { Anisou, 0, "", "anisou", ConvArg::AnisouChoice,
     "  --anisou=yes|no|heavy  \tAdd or remove ANISOU records." },
+  { AssignRecords, 0, "", "assign-records", ConvArg::RecordChoice,
+    "  --assign-records[=A|H]  \tRe-assign ATOM/HETATM (w/o argument: auto)." },
   // disabled: probably not used and implementing it would require either
   // using Topo::set_cispeps_in_structure() or duplicating the code.
   //{ SetCis, 0, "", "set-cispep", Arg::None,
   //  "  --set-cispep  \tReset CISPEP records from omega angles." },
 
   { NoOp, 0, "", "", Arg::None, "\nMacromolecular operations:" },
   { Select, 0, "", "select", Arg::Required,
@@ -170,14 +184,84 @@
   while (stream) {
     stream.read(buffer, buf_size);
     out.append(buffer, stream.gcount());
   }
   return out;
 }
 
+std::uint8_t select_acc_index(const std::vector<std::string>& acc, // Entity::sifts_unp_acc
+                              const gemmi::ConstResidueSpan& polymer,
+                              const std::vector<std::string>& preferred_acs) {
+  if (acc.size() < 2)
+    return 0;
+  for (const std::string& pa : preferred_acs) {
+    auto it = std::find(acc.begin(), acc.end(), pa);
+    if (it != acc.end())
+      return std::uint8_t(it - acc.begin());
+  }
+  // return SIFTS mapping with most residues
+  std::vector<int> counts(acc.size(), 0);
+  for (const gemmi::Residue& res : polymer)
+    if (res.sifts_unp.res && res.sifts_unp.acc_index < acc.size())
+      ++counts[res.sifts_unp.acc_index];
+  auto max_el = std::max_element(counts.begin(), counts.end());
+  return std::uint8_t(max_el - counts.begin());
+}
+
+// Set seqid corresponding to one UniProt sequence.
+// Other residues have seqid changed to avoid conflicts.
+void to_sifts_num(gemmi::Structure& st, const std::vector<std::string>& preferred_acs) {
+  using Key = std::pair<std::string, gemmi::SeqId>;
+  std::map<Key, gemmi::SeqId> seqid_map;
+  bool first_model = true;
+  for (gemmi::Model& model: st.models) {
+    for (gemmi::Chain& chain : model.chains) {
+      auto polymer = chain.get_polymer();
+      gemmi::Entity* ent = st.get_entity_of(polymer);
+      std::uint8_t acc_index = 0;
+      if (ent)
+        acc_index = select_acc_index(ent->sifts_unp_acc, polymer, preferred_acs);
+      std::uint16_t offset = 4950;
+      for (gemmi::Residue& res : chain.residues) {
+        if (res.sifts_unp.res && res.sifts_unp.acc_index == acc_index) {
+          // assert(ent && res.entity_id == ent->name);
+          gemmi::SeqId new_seqid(res.sifts_unp.num, ' ');
+          if (first_model)
+            seqid_map.emplace(std::make_pair(chain.name, res.seqid), new_seqid);
+          res.seqid = new_seqid;
+          offset = std::max(offset, res.sifts_unp.num);
+        }
+      }
+      offset = (offset + 50) / 1000 * 1000;  // always >= 5000
+      for (gemmi::Residue& res : chain.residues)
+        if (!res.sifts_unp.res || res.sifts_unp.acc_index != acc_index) {
+          gemmi::SeqId orig_seqid = res.seqid;
+          res.seqid.num += offset;
+          if (first_model)
+            seqid_map.emplace(std::make_pair(chain.name, orig_seqid), res.seqid);
+        }
+    }
+    first_model = false;
+  }
+
+  auto update_seqid = [&](const std::string& chain_name, gemmi::SeqId& seqid) {
+    auto it = seqid_map.find(std::make_pair(chain_name, seqid));
+    if (it != seqid_map.end())
+      seqid = it->second;
+    else
+      seqid.num = gemmi::SeqId::OptionalNum();
+  };
+  process_sequence_ids(st, update_seqid);
+  // Just remove outdated DbRef::seq_*; it is needed when writing a PDB file,
+  // but if it's absent, it's determined from DbRef::label_seq_*.
+  for (gemmi::Entity& ent : st.entities)
+    for (gemmi::Entity::DbRef& dbref : ent.dbrefs)
+      dbref.seq_begin = dbref.seq_end = gemmi::SeqId();
+}
+
 void convert(gemmi::Structure& st,
              const std::string& output, CoorFormat output_type,
              const std::vector<option::Option>& options) {
   if (st.models.empty())
     gemmi::fail("No atoms in the input file. Wrong file format?");
   if (st.ter_status == 'e')
     std::cerr << "WARNING: TER records in the input PDB are clearly where they shouldn't be."
@@ -185,21 +269,30 @@
 
   for (const option::Option* opt = options[ChangeCcdCode]; opt; opt = opt->next()) {
     const char* sep = std::strchr(opt->arg, ':');
     std::string old_name(opt->arg, sep);
     std::string new_name(sep+1);
     if (options[Verbose])
       std::cerr << "Renaming " << old_name << " to " << new_name << std::endl;
-    gemmi::change_ccd_code(st, old_name, new_name);
+    gemmi::rename_residues(st, old_name, new_name);
   }
 
-  gemmi::setup_entities(st);
+  if (options[AssignRecords])
+    // avoid using initial ATOM/HETATM in setup_entities()
+    gemmi::assign_het_flags(st, '\0');
+  // gemmi::setup_entities(st) with postponed deduplicate_entities()
+  gemmi::add_entity_types(st, /*overwrite=*/false);
+  assign_subchains(st, /*force=*/false);
+  ensure_entities(st);
+  // call deduplicate_entities() after add_microhetero_to_sequences()
   if (st.input_format == CoorFormat::Pdb) {
-    if (!options[SetSeq])
+    if (!options[SetSeq]) {
       gemmi::assign_label_seq_id(st, options[ForceLabel]);
+      gemmi::add_microhetero_to_sequences(st);
+    }
     if (!options[CopyRemarks])
       st.raw_remarks.clear();
   } else {
     // handles special tag from Refmac's mmCIF
     store_deuterium_as_fraction(st, false);
   }
 
@@ -243,14 +336,19 @@
           for (gemmi::Residue& res : chain.residues)
             for (gemmi::Atom& atom : res.atoms)
               if (!atom.is_hydrogen())
                 gemmi::ensure_anisou(atom);
     }
   }
 
+  if (const option::Option* opt = options[AssignRecords]) {
+    char flag = opt->arg ? opt->arg[0] : '?';
+    gemmi::assign_het_flags(st, flag);
+  }
+
   for (const option::Option* opt = options[RenameChain]; opt; opt = opt->next()) {
     const char* sep = std::strchr(opt->arg, ':');
     std::string old_name(opt->arg, sep);
     std::string new_name(sep+1);
     gemmi::rename_chain(st, old_name, new_name);
   }
   if (options[ShortenCN]) {
@@ -269,57 +367,39 @@
       for (gemmi::FastaSeq& fs : gemmi::read_pir_or_fasta(str))
         fasta_sequences.push_back(std::move(fs.seq));
     }
     if (options[Verbose])
       std::cerr << fasta_sequences.size() << " sequence(s) was read..." << std::endl;
     gemmi::clear_sequences(st);
     gemmi::assign_best_sequences(st, fasta_sequences);
-    gemmi::deduplicate_entities(st);
     gemmi::assign_label_seq_id(st, options[ForceLabel]);
+    gemmi::add_microhetero_to_sequences(st);
     for (gemmi::Entity& ent : st.entities) {
       if (ent.entity_type == gemmi::EntityType::Polymer && ent.full_sequence.empty())
         std::cerr << "No sequence found for "
                   << polymer_type_to_string(ent.polymer_type) << " entity " << ent.name
                   << " (" << gemmi::join_str(ent.subchains, ',') << ')' << std::endl;
     }
   }
+  // call it after add_microhetero_to_sequences()
+  gemmi::deduplicate_entities(st);
 
-  if (options[SiftsNum]) {
-    // Currently, we change seqid only for residues _pdbx_sifts_xref_db.unp_num
-    // set, and leave seqid for other residues.
-    // A more robust method would be to re-assign the whole polymer always when
-    // nup_num is set for any residue. This would mean:
-    // using insertion codes for insertions (up to 26 residues),
-    // renumbering ligands and waters if needed, and
-    // failing if we get duplicated seqid (multiple mappings for one chain).
-    bool changed = false;
-    for (gemmi::Model& model: st.models)
-      for (gemmi::Chain& chain : model.chains) {
-        const gemmi::Residue* prev_res = nullptr;
-        bool wrong_order = false;
-        for (gemmi::Residue& res : chain.residues) {
-          if (res.sifts_unp.res) {
-            res.seqid = gemmi::SeqId(res.sifts_unp.num, ' ');
-            if (prev_res && !(prev_res->seqid < res.seqid))
-              wrong_order = true;
-            changed = true;
-          }
-          prev_res = &res;
-        }
-        if (wrong_order) {
-          std::cerr << "WARNING: new sequence IDs are in wrong order in chain "
-                    << chain.name;
-          if (st.models.size() > 1)
-            std::cerr << " (model " << model.name << ')';
-          std::cerr << std::endl;
-        }
-      }
-    if (options[Verbose] && !changed)
-      std::cerr << "Option --sifts-num had no effect, "
-                   "it works only with _pdbx_sifts_xref_db.unp_num." << std::endl;
+  if (const option::Option* opt = options[SiftsNum]) {
+    if (std::all_of(st.entities.begin(), st.entities.end(),
+                    [](const gemmi::Entity& ent) { return ent.sifts_unp_acc.empty(); }))
+      gemmi::fail("--sifts-num failed: SIFTS annotation not found in the file.\n"
+                  "Check if tags such as _pdbx_sifts_xref_db.unp_num are present.");
+    std::vector<std::string> preferred_acs;
+    if (opt->arg) {
+      gemmi::split_str_into(opt->arg, ',', preferred_acs);
+      for (const std::string& ac : preferred_acs)
+        if (ac.size() < 6 || ac[0] < 'A' || ac[0] > 'Z' || ac[1] < '0' || ac[1] > '9')
+          gemmi::fail(ac + " is not in UniProtKB AC format, from: " + opt->name);
+    }
+    to_sifts_num(st, preferred_acs);
   }
 
   HowToNameCopiedChain how = HowToNameCopiedChain::AddNumber;
   if (output_type == CoorFormat::Pdb)
     how = HowToNameCopiedChain::Short;
   if (options[AsAssembly]) {
     std::ostream* out = options[Verbose] ? &std::cerr : nullptr;
```

### Comparing `gemmi-0.6.5/prog/crd.cpp` & `gemmi-0.6.6/prog/crd.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/ecalc.cpp` & `gemmi-0.6.6/prog/ecalc.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/fprime.cpp` & `gemmi-0.6.6/prog/fprime.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/grep.cpp` & `gemmi-0.6.6/prog/grep.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/h.cpp` & `gemmi-0.6.6/prog/h.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/histogram.h` & `gemmi-0.6.6/prog/histogram.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/json2cif.cpp` & `gemmi-0.6.6/prog/json2cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/main.cpp` & `gemmi-0.6.6/prog/main.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/map.cpp` & `gemmi-0.6.6/prog/map.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/map2sf.cpp` & `gemmi-0.6.6/prog/map2sf.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mapcoef.cpp` & `gemmi-0.6.6/prog/mapcoef.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mapcoef.h` & `gemmi-0.6.6/prog/mapcoef.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mask.cpp` & `gemmi-0.6.6/prog/mask.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/merge.cpp` & `gemmi-0.6.6/prog/merge.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mixmtz.cpp` & `gemmi-0.6.6/prog/mixmtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mondiff.cpp` & `gemmi-0.6.6/prog/mondiff.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/monlib_opt.cpp` & `gemmi-0.6.6/prog/monlib_opt.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/monlib_opt.h` & `gemmi-0.6.6/prog/monlib_opt.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/mtz.cpp` & `gemmi-0.6.6/prog/mtz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     return Arg::Choice(option, msg, {"ccp4", "tnt"});
   }
 };
 
 enum OptionIndex {
   Headers=4, Dump, PrintBatch, PrintBatches, ExpandedBatches, PrintAppendix,
   PrintTsv, PrintStats, PrintHistogram, PrintCells, CheckAsu,
-  Compare, ToggleEndian, NoIsym, UpdateReso
+  Compare, ToggleEndian, NoIsym
 };
 
 const option::Descriptor Usage[] = {
   { NoOp, 0, "", "", Arg::None,
     "Usage:\n " EXE_NAME " [options] MTZ_FILE[...]"
     "\nPrint information from an mtz file."},
   CommonUsage[Help],
@@ -63,16 +63,14 @@
     "  --check-asu=ccp4|tnt  \tCheck if reflections are in ASU." },
   { Compare, 0, "", "compare", Arg::Required,
     "  --compare=FILE  \tCompare two MTZ files." },
   { ToggleEndian, 0, "", "toggle-endian", Arg::None,
     "  --toggle-endian  \tToggle assumed endianness (little <-> big)." },
   { NoIsym, 0, "", "no-isym", Arg::None,
     "  --no-isym  \tDo not apply symmetry from M/ISYM column." },
-  { UpdateReso, 0, "", "update-reso", Arg::None,
-    "  --update-reso  \tRecalculate resolution limits before printing." },
   { 0, 0, 0, 0, 0, 0 }
 };
 
 void print_cell_parameters(const char* prefix, const gemmi::UnitCell& cell) {
   printf("%s %g %7g %7g  %6g %6g %6g\n", prefix,
          cell.a, cell.b, cell.c, cell.alpha, cell.beta, cell.gamma);
 }
@@ -354,14 +352,15 @@
       if (v < stat.min_value)
         stat.min_value = v;
       if (v > stat.max_value)
         stat.max_value = v;
       stat.var.add_point(v);
     }
   }
+  printf("Resolution: %.5f - %.5f A\n", mtz.resolution_high(), mtz.resolution_low());
   printf("column type @dataset  completeness        min       max"
          "       mean   stddev\n");
   for (size_t i = 0; i != column_stats.size(); ++i) {
     const Mtz::Column& col = mtz.columns[i];
     const ColumnStats& stat = column_stats[i];
     printf("%-14s %c @%d  %d (%6.2f%%) %9.5g %9.5g  %9.5g %8.4g\n",
            col.label.c_str(), col.type, col.dataset_id,
@@ -436,16 +435,19 @@
     int l = (int) mtz.data[i * ncol + 2];
     if (asu.is_in({{h, k, l}}))
       ++counter;
   }
   if (!mtz.is_merged())
     printf("NOTE: this is multirecord (unmerged) MTZ file\n");
   printf("spacegroup: %s\n", sg->xhm().c_str());
-  printf("%s ASU convention wrt. standard setting: %s\n",
-         tnt ? "TNT" : "CCP4", asu.condition_str());
+  std::string wrt;
+  if (!tnt && !sg->is_reference_setting())
+    wrt = " wrt. " + gemmi::get_spacegroup_reference_setting(sg->number).xhm();
+  printf("%s ASU convention%s: %s\n",
+         tnt ? "TNT" : "CCP4", wrt.c_str(), asu.condition_str());
   printf("inside / outside of ASU: %d / %d\n",
          counter, mtz.nreflections - counter);
   double dmin = mtz.resolution_high() - 1e-6;
   printf("All unique reflections up to d=%g: %d\n",
          dmin, gemmi::count_reflections(mtz.cell, mtz.spacegroup, dmin));
 }
 
@@ -543,18 +545,16 @@
   }
   if (options[Verbose])
     mtz.warnings = &std::cerr;
   mtz.read_main_headers(stream);
   mtz.read_history_and_batch_headers(stream);
   mtz.setup_spacegroup();
   if (options[PrintTsv] || options[PrintStats] || options[PrintHistogram] ||
-      options[CheckAsu] || options[Compare] || options[UpdateReso])
+      options[CheckAsu] || options[Compare])
     mtz.read_raw_data(stream);
-  if (options[UpdateReso])
-    mtz.update_reso();
   if (options[Dump] ||
       !(options[PrintBatch] || options[PrintBatches] || options[PrintTsv] ||
         options[PrintStats] || options[PrintHistogram] ||
         options[PrintAppendix] || options[PrintCells] ||
         options[CheckAsu] || options[Compare] || options[Headers]))
     dump(mtz);
   if (options[PrintBatch]) {
@@ -578,14 +578,16 @@
     mtz.switch_to_original_hkl();
   if (options[PrintCells])
     print_cells(mtz);
   for (const option::Option* opt = options[PrintHistogram]; opt; opt = opt->next())
     print_column_statistics(mtz, opt->arg);
   if (options[PrintTsv])
     print_tsv(mtz);
+  if (options[CheckAsu] || options[PrintStats])
+    mtz.update_reso();
   if (options[PrintStats])
     print_stats(mtz);
   if (options[CheckAsu])
     check_asu(mtz, options[CheckAsu].arg[0] == 't');
   if (options[Compare])
     // here mtz gets sorted, so this option must be at the end
     compare_mtz(mtz, options[Compare].arg, options[Verbose]);
```

### Comparing `gemmi-0.6.5/prog/mtz2cif.cpp` & `gemmi-0.6.6/prog/mtz2cif.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -110,22 +110,23 @@
 
 } // anonymous namespace
 
 int GEMMI_MAIN(int argc, char **argv) {
   OptParser p(EXE_NAME);
   p.simple_parse(argc, argv, Usage);
   if (p.options[PrintSpec]) {
-    std::printf("                                for merged mtz\n");
+    std::printf(" ========   for merged mtz   ========\n");
     const char** lines = gemmi::MtzToCif::default_spec(/*for_merged=*/true);
     for (; *lines != nullptr; ++lines)
       std::printf("%s\n", *lines);
-    std::printf("\n                             for unmerged mtz\n");
+    std::printf("\n ========   for unmerged mtz   ========\n");
     lines = gemmi::MtzToCif::default_spec(/*for_merged=*/false);
     for (; *lines != nullptr; ++lines)
       std::printf("%s\n", *lines);
+    std::printf("\n");
     return 0;
   }
 
   int nargs = p.nonOptionsCount();
   if (nargs != 2 && nargs != 3) {
     fprintf(stderr, "%s requires 2 or 3 arguments, got %d.", p.program_name, nargs);
     p.print_try_help_and_exit("");
@@ -278,15 +279,16 @@
             std::cerr << ". Taking into account anisotropic scaling.\n";
           else
             std::cerr << ". B tensor is unknown. Intensities won't be checked.\n";
         }
         mi.read_merged_intensities_from_mtz(*mtz[0]);
       } else {
         gemmi::ReflnBlock rblock = gemmi::get_refln_block(
-            gemmi::read_cif_from_buffer(cif_buf, cif_input).blocks, {});
+            gemmi::read_cif_from_memory(cif_buf.data(), cif_buf.size(), cif_input).blocks,
+            {});
         if (!rblock.entry_id.empty() && rblock.entry_id != mtz_to_cif.entry_id) {
           fprintf(stderr, "Note: using _entry.id from mmCIF (%s) instead of %s.\n",
                   rblock.entry_id.c_str(), mtz_to_cif.entry_id.c_str());
           mtz_to_cif.entry_id = rblock.entry_id;
         }
         mi.take_staraniso_b_from_mmcif(rblock.block);
         mi.read_merged_intensities_from_mmcif(rblock);
```

### Comparing `gemmi-0.6.5/prog/options.cpp` & `gemmi-0.6.6/prog/options.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 // Copyright 2018 Global Phasing Ltd.
 
 #define GEMMI_PROG na
 #include "options.h"
 #include <cstdio>   // for fprintf, fopen
 #include <cstdlib>  // for strtol, strtod, exit
 #include <cstring>  // for strcmp, strchr
+#include <gemmi/atox.hpp>      // for skip_blank
 #include <gemmi/fileutil.hpp>  // for file_open_or
+#include <gemmi/gz.hpp>        // for zlib_version
+#include <gemmi/model.hpp>     // for CoorFormat
 #include <gemmi/pdb_id.hpp>    // for expand_if_pdb_code
+#include <gemmi/to_cif.hpp>    // for cif::WriteOptions
+#include <gemmi/util.hpp>      // for trim_str
 #include <gemmi/version.hpp>   // for GEMMI_VERSION
-#include <gemmi/util.hpp>   // for trim_str
-#include <gemmi/model.hpp>  // for gemmi::CoorFormat
-#include <gemmi/to_cif.hpp>  // for gemmi::cif::WriteOptions
-#include <gemmi/atox.hpp>   // for skip_blank
 
 using std::fprintf;
 
 const option::Descriptor CommonUsage[] = {
   { 0, 0, 0, 0, 0, 0 }, // this makes CommonUsage[Help] return Help item, etc
   { Help, 0, "h", "help", Arg::None, "  -h, --help  \tPrint usage and exit." },
   { Version, 0, "V", "version", Arg::None,
@@ -308,14 +309,15 @@
 #  if defined(__clang__)
     std::printf("Compiler: Clang %d.%d.%d (C++ %ld)\n",
                 __clang_major__, __clang_minor__, __clang_patchlevel__, __cplusplus);
 #  elif defined(__GNUC__)
     std::printf("Compiler: GCC %d.%d.%d (C++ %ld)\n",
                 __GNUC__, __GNUC_MINOR__, __GNUC_PATCHLEVEL__, __cplusplus);
 #  endif
+    std::printf("Built with: %s\n", gemmi::zlib_description);
 #endif
   }
 }
 
 void read_spec_file(const char* path, std::vector<std::string>& output) {
   char buf[256];
   gemmi::fileptr_t f_spec = gemmi::file_open_or(path, "r", stdin);
```

### Comparing `gemmi-0.6.5/prog/options.h` & `gemmi-0.6.6/prog/options.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/reindex.cpp` & `gemmi-0.6.6/prog/reindex.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/residues.cpp` & `gemmi-0.6.6/prog/residues.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -188,21 +188,21 @@
             printf("...  (%d residues)", counter);
           putchar('\n');
         }
         const char* etype = entity_type_to_string(res.entity_type);
         if (p.options[Label])
           col = printf("%s (%s) %-11s", chain.name.c_str(), res.subchain.c_str(), etype);
         else
-          col = printf("%-3s %-11s ", chain.name.c_str(), etype);
+          col = printf("%-4s %-11s ", chain.name.c_str(), etype);
         counter = 0;
         prev = res.entity_type;
       }
       if (short_level == 1) {
         if (counter == kWrap) {
-          printf("\n                  ");
+          printf("\n                 ");
           counter = 0;
         }
         printf(" %5s%c %-3s",
                res.seqid.num.str().c_str(), res.seqid.icode, res.name.c_str());
       } else {
         if (col < kLimit) {
           if (short_level == 2) {
@@ -272,25 +272,27 @@
           prev = *res.label_seq;
           ++length;
         }
         printf("    - %s from strand %s, %d residues",
                sub.c_str(), strand->second.c_str(), length);
         if (!polymer.empty()) {
           printf(": %s-%s", polymer.front().label_seq.str().c_str(),
-                              polymer.back().label_seq.str().c_str());
+                            polymer.back().label_seq.str().c_str());
           if (!gaps.empty()) {
             printf(" except");
             for (std::pair<int, int> gap : gaps) {
               printf(" %d", gap.first);
               if (gap.second != gap.first)
                 printf("-%d", gap.second);
             }
           }
         }
         putchar('\n');
+        if (!ent.sifts_unp_acc.empty())
+          printf("    SIFTS mapping: %s\n", gemmi::join_str(ent.sifts_unp_acc, ' ').c_str());
       }
     }
   printf("Others\n");
   for (const gemmi::Entity& ent : st.entities)
     if (ent.entity_type != gemmi::EntityType::Polymer) {
       printf("  entity %s, %s",
              ent.name.c_str(), gemmi::entity_type_to_string(ent.entity_type));
```

### Comparing `gemmi-0.6.5/prog/rmsz.cpp` & `gemmi-0.6.6/prog/rmsz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/sf2map.cpp` & `gemmi-0.6.6/prog/sf2map.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/sfcalc.cpp` & `gemmi-0.6.6/prog/sfcalc.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 
 #define GEMMI_PROG sfcalc
 #include "options.h"
 
 namespace {
 
 enum OptionIndex {
-  Hkl=4, Dmin, For, NormalizeIt92, Rate, Blur, RCut, Test, ToMtz, Compare,
-  CifFp, Wavelength, Unknown, NoAniso, Margin, ScaleTo, SigmaCutoff, FLabel,
-  PhiLabel, Ksolv, Bsolv, Baniso, RadiiSet, Rprobe, Rshrink, WriteMap
+  Hkl=4, Dmin, For, NormalizeIt92, UseCharge, Rate, Blur, RCut,
+  Test, WriteMap, ToMtz, Compare, FLabel, PhiLabel,
+  CifFp, Wavelength, Unknown, NoAniso, Margin, ScaleTo, SigmaCutoff,
+  MaskSpacing, RadiiSet, Rprobe, Rshrink, MaskFile, Ksolv, Bsolv, Kov, Baniso
 };
 
 struct SfCalcArg: public Arg {
   static option::ArgStatus FormFactors(const option::Option& option, bool msg) {
     return Arg::Choice(option, msg, {"xray", "electron", "neutron", "mott-bethe"});
   }
   static option::ArgStatus Radii(const option::Option& option, bool msg) {
@@ -80,14 +81,16 @@
     "  --hkl=H,K,L  \tCalculate structure factor F_hkl." },
   { Dmin, 0, "", "dmin", Arg::Float,
     "  --dmin=NUM  \tCalculate structure factors up to given resolution." },
   { For, 0, "", "for", SfCalcArg::FormFactors,
     "  --for=TYPE  \tTYPE is xray (default), electron, neutron or mott-bethe." },
   { NormalizeIt92, 0, "", "normalize-it92", Arg::None,
     "  --normalize-it92  \tNormalize X-ray form factors (a tiny change)." },
+  { UseCharge, 0, "", "use-charge", Arg::None,
+    "  --use-charge  \tUse X-ray form factors with charges when available." },
   { CifFp, 0, "", "ciffp", Arg::None,
     "  --ciffp  \tRead f' from _atom_type_scat_dispersion_real in CIF." },
   { Wavelength, 0, "w", "wavelength", Arg::Float,
     "  --wavelength=NUM  \tWavelength [A] for calculation of f' "
     "(use --wavelength=0 or -w0 to ignore anomalous scattering)." },
   { Unknown, 0, "", "unknown", Arg::Required,
     "  --unknown=SYMBOL  \tUse form factor of SYMBOL for unknown atoms." },
@@ -115,25 +118,32 @@
   { ScaleTo, 0, "", "scale-to", Arg::Required,
     "  --scale-to=FILE:COL  \tAnisotropic scaling to F from MTZ file."
     "\n\tArgument: FILE[:FCOL[:SIGFCOL]] (defaults: F and SIGF)." },
   { SigmaCutoff, 0, "", "sigma-cutoff", Arg::Float,
     "  --sigma-cutoff=NUM  \tUse only data with F/SIGF > NUM (default: 0)." },
   // TODO: solvent option: mask, babinet, none
 
-  { NoOp, 0, "", "", Arg::None, "\nOptions for bulk solvent correction (only w/ FFT):" },
+  { NoOp, 0, "", "", Arg::None,
+    "\nOptions for bulk solvent correction and scaling (only w/ FFT):" },
+  { MaskSpacing, 0, "", "d-mask", Arg::Float,
+    "  --d-mask=NUM  \tSpacing of mask grid (default: same as for model)." },
   { RadiiSet, 0, "", "radii-set", SfCalcArg::Radii,
     "  --radii-set=SET  \tSet of per-element radii, one of: vdw, cctbx, refmac." },
   { Rprobe, 0, "", "r-probe", Arg::Float,
     "  --r-probe=NUM  \tValue added to VdW radius (default: 1.0A)." },
   { Rshrink, 0, "", "r-shrink", Arg::Float,
     "  --r-shrink=NUM  \tValue for shrinking the solvent area (default: 1.1A)." },
+  { MaskFile, 0, "", "solvent-mask", Arg::Required,
+    "  --solvent-mask=FILE  \tUse mask from file instead of calculating it." },
   { Ksolv, 0, "", "ksolv", Arg::Float,
     "  --ksolv=NUM  \tValue (if optimizing: initial value) of k_solv." },
   { Bsolv, 0, "", "bsolv", Arg::Float,
     "  --bsolv=NUM  \tValue (if optimizing: initial value) of B_solv." },
+  { Kov, 0, "", "kov", Arg::Float,
+    "  --kov=NUM  \tValue (if optimizing: initial value) of k_overall." },
   { Baniso, 0, "", "baniso", SfCalcArg::Float6,
     "  --baniso=B11:...:B23 \tAnisotropic scale matrix (6 colon-separated numbers: "
       "B11, B22, B33, B12, B13, B23)." },
 
   { NoOp, 0, "", "", Arg::None,
     "\nOptions for comparing calculated values with values from a file:" },
   { Compare, 0, "", "compare", Arg::Required,
@@ -223,27 +233,26 @@
   output_mtz->write_to_file(file.path);
 }
 
 template<typename Table, typename Real>
 void process_with_fft(const gemmi::Structure& st,
                       gemmi::DensityCalculator<Table, Real>& dencalc,
                       bool mott_bethe,
-                      const gemmi::SolventMasker& masker,
+                      const gemmi::AsuData<std::complex<Real>>* mask_data,
                       gemmi::Scaling<Real>& scaling,
                       bool verbose, const RefFile& file,
                       const gemmi::AsuData<gemmi::ValueSigma<Real>>& scale_to,
                       const char* map_file) {
   // prepare electron density map
   if (verbose) {
     fprintf(stderr, "Preparing electron density on a grid...\n");
     fflush(stderr);
   }
   Timer timer(verbose);
   timer.start();
-  dencalc.set_grid_cell_and_spacegroup(st);
   dencalc.put_model_density_on_grid(st.models[0]);
   timer.print("...took");
   if (map_file) {
     gemmi::Ccp4<Real> ccp4;
     ccp4.grid = dencalc.grid;
     ccp4.update_ccp4_header(2);
     ccp4.write_ccp4_map(map_file);
@@ -264,59 +273,58 @@
   if (verbose) {
     timer.print("...took");
     fprintf(stderr, "Preparing results...\n");
     fflush(stderr);
   }
   gemmi::StructureFactorCalculator<Table> calc(st.cell);
   calc.addends = dencalc.addends;
-  gemmi::fileptr_t cache(nullptr, nullptr);
+  gemmi::fileptr_t cache(nullptr, gemmi::needs_fclose{false});
   gemmi::AsuData<std::complex<double>> compared_data;
   if (file.path) {
     if (file.mode == RefFile::Mode::Test) {
       cache = gemmi::file_open(file.path, "r");
     } else if (file.mode == RefFile::Mode::Compare) {
       gemmi::Mtz mtz;
       mtz.read_input(gemmi::MaybeGzipped(file.path), true);
       compared_data.load_values<2>(gemmi::MtzDataProxy{mtz}, {file.f_label, file.phi_label});
     }
   }
   auto asu_data = sf.prepare_asu_data(dencalc.d_min, dencalc.blur, false, false, mott_bethe);
 
-  gemmi::AsuData<std::complex<Real>> mask_data;
-  if (scaling.use_solvent) {
-    // uses scaling.grid as a temporary array
-    masker.put_mask_on_grid(dencalc.grid, st.models[0]);
-    mask_data = transform_map_to_f_phi(dencalc.grid, /*half_l=*/true)
-                .prepare_asu_data(dencalc.d_min, 0);
-  }
-
   if (scale_to.size() != 0) {
-    scaling.prepare_points(asu_data, scale_to, &mask_data);
+    scaling.prepare_points(asu_data, scale_to, mask_data);
     printf("Calculating scale factors using %zu points...\n", scaling.points.size());
-    scaling.fit_isotropic_b_approximately();
-    //fprintf(stderr, "k_ov=%g B_ov=%g\n", scaling.k_overall, scaling.get_b_overall().u11);
+    if (scaling.b_star.all_zero()) {
+      scaling.fit_isotropic_b_approximately();
+      //fprintf(stderr, "initial k_ov=%g B_ov=%g\n",
+      //        scaling.k_overall, scaling.get_b_overall().u11);
+    } else if (scaling.k_overall == 1.) {
+      scaling.k_overall = scaling.lsq_k_overall();
+      //fprintf(stderr, "initial k_ov=%g\n", scaling.k_overall);
+    }
+    //scaling.fit_b_star_approximately();
     scaling.fit_parameters();
-    gemmi::SMat33<double> b_aniso = scaling.get_b_overall();
     if (scaling.use_solvent)
       fprintf(stderr, "Bulk solvent parameters: k_sol=%g B_sol=%g\n",
               scaling.k_sol, scaling.b_sol);
+    gemmi::SMat33<double> b_aniso = scaling.get_b_overall();
     fprintf(stderr, "k_ov=%g B11=%g B22=%g B33=%g B12=%g B13=%g B23=%g\n",
             scaling.k_overall, b_aniso.u11, b_aniso.u22, b_aniso.u33,
                                b_aniso.u12, b_aniso.u13, b_aniso.u23);
     if (verbose) {
       std::vector<double> computed = scaling.compute_values();
       Comparator comparator;
       for (size_t i = 0; i != scaling.points.size(); ++i)
         comparator.add(computed[i], (double)scaling.points[i].fobs);
       fprintf(stderr, "After scaling: ");
       print_to_stderr(comparator);
       fprintf(stderr, "\n");
     }
   }
-  scaling.scale_data(asu_data, &mask_data);
+  scaling.scale_data(asu_data, mask_data);
 
   if (file.mode == RefFile::Mode::WriteMtz) {
     write_asudata_to_mtz(asu_data, file);
   } else if (file.mode == RefFile::Mode::None) {
     for (gemmi::HklValue<std::complex<Real>>& hv : asu_data.v)
       print_sf(hv.value, hv.hkl);
   } else {
@@ -369,15 +377,15 @@
   timer.start();
   int counter = 0;
   // cf. prepare_asu_data()
   double max_1_d = 1. / d_min;
   int max_h = int(max_1_d / small.cell.ar);
   int max_k = int(max_1_d / small.cell.br);
   int max_l = int(max_1_d / small.cell.cr);
-  const gemmi::SpaceGroup* sg = small.find_spacegroup();
+  const gemmi::SpaceGroup* sg = small.spacegroup;
   if (!sg)
     sg = &gemmi::get_spacegroup_p1();
   gemmi::ReciprocalAsu asu(sg);
   gemmi::AsuData<std::complex<double>> asu_data;
   gemmi::GroupOps gops = sg->operations();
   for (int h = -max_h; h <= max_h; ++h)
     for (int k = -max_k; k <= max_k; ++k)
@@ -515,41 +523,47 @@
 
 template<typename Table>
 void process_with_table(bool use_st, gemmi::Structure& st, const gemmi::SmallStructure& small,
                         double wavelength, bool mott_bethe, const OptParser& p) {
   const gemmi::UnitCell& cell = use_st ? st.cell : small.cell;
   gemmi::StructureFactorCalculator<Table> calc(cell);
 
-  // assign f' given explicitly in a file
-  if (p.options[CifFp]) {
+
+  auto present_elems = use_st ? st.models[0].present_elements()
+                              : small.present_elements();
+  if (present_elems[(int)gemmi::El::X])
+    gemmi::fail("unknown element. Add --unknown=O to treat unknown atoms as oxygen.");
+  for (size_t i = 1; i != present_elems.size(); ++i)
+    if (present_elems[i] && !Table::has((gemmi::El)i))
+      gemmi::fail("Missing form factor for element ", element_name((gemmi::El)i));
+
+  if (p.options[CifFp]) { // assign f' given explicitly in a file
     if (use_st) {
       // _atom_type.scat_dispersion_real is almost never used,
       // so for now we ignore it.
+      fprintf(stderr, "WARNING: --ciffp ignored, f' is not read (yet) from mmCIF and PDB.\n");
     } else { // small molecule
       if (p.options[Verbose])
         fprintf(stderr, "Using f' read from cif file (%u atom types)\n",
                 (unsigned) small.atom_types.size());
       for (const gemmi::SmallStructure::AtomType& atom_type : small.atom_types)
         calc.addends.set(atom_type.element, (float)atom_type.dispersion_real);
     }
-  }
-
-  auto present_elems = use_st ? st.models[0].present_elements()
-                              : small.present_elements();
-  if (present_elems[(int)gemmi::El::X])
-    gemmi::fail("unknown element. Add --unknown=O to treat unknown atoms as oxygen.");
-  for (size_t i = 1; i != present_elems.size(); ++i)
-    if (present_elems[i] && !Table::has((gemmi::El)i))
-      gemmi::fail("Missing form factor for element ", element_name((gemmi::El)i));
-  if (wavelength > 0) {
+  } else if (wavelength > 0) {
+    if (p.options[Verbose])
+      fprintf(stderr, "Wavelength %g A. Using Cromer-Liberman approximation for f'.\n",
+              wavelength);
     double energy = gemmi::hc() / wavelength;
     for (int z = 1; z <= 92; ++z)
       if (present_elems[z] && calc.addends.values[z] == 0) {
         calc.addends.values[z] = (float) gemmi::cromer_liberman(z, energy, nullptr);
       }
+  } else {
+    if (p.options[Verbose])
+      fprintf(stderr, "Unknown wavelength, f' not used.\n");
   }
   if (mott_bethe)
     calc.addends.subtract_z();
 
   // handle option --hkl
   for (const option::Option* opt = p.options[Hkl]; opt; opt = opt->next()) {
     std::vector<int> hkl_ = parse_comma_separated_ints(opt->arg);
@@ -632,28 +646,30 @@
       gemmi::DensityCalculator<Table, Real> dencalc;
       dencalc.d_min = d_min;
       if (p.options[Rate])
         dencalc.rate = std::atof(p.options[Rate].arg);
       if (p.options[RCut])
         dencalc.cutoff = (float) std::atof(p.options[RCut].arg);
       dencalc.addends = calc.addends;
+      dencalc.grid.setup_from(st);
       if (p.options[Blur]) {
         dencalc.blur = std::atof(p.options[Blur].arg);
       } else if (dencalc.rate < 3) {
         // ITfC vol B section 1.3.4.4.5 has formula
         // B = log Q / (sigma * (sigma - 1) * d*_max ^2)
         // where Q is quality factor, sigma is the oversampling rate.
         // This value is not optimal.
         // The optimal value would depend on the distribution of B-factors
         // and on the atomic cutoff radius, and probably it would be too
         // hard to estimate. Here we use the same formula as in Refmac.
         dencalc.set_refmac_compatible_blur(st.models[0]);
-        if (p.options[Verbose])
-          fprintf(stderr, "B_min=%g, B_add=%g\n",
-                  gemmi::get_minimum_b(st.models[0]), dencalc.blur);
+        if (p.options[Verbose]) {
+          double b_min = gemmi::calculate_b_aniso_range(st.models[0]).first;
+          fprintf(stderr, "B_min=%g, B_add=%g\n", b_min, dencalc.blur);
+        }
       }
       gemmi::AtomicRadiiSet radii_choice = gemmi::AtomicRadiiSet::VanDerWaals;
       if (p.options[RadiiSet]) {
         char c = p.options[RadiiSet].arg[0];
         if (c == 'v')
           radii_choice = gemmi::AtomicRadiiSet::VanDerWaals;
         else if (c == 'c')
@@ -662,36 +678,69 @@
           radii_choice = gemmi::AtomicRadiiSet::Refmac;
       }
       gemmi::SolventMasker masker(radii_choice);
       if (p.options[Rprobe])
         masker.rprobe = std::atof(p.options[Rprobe].arg);
       if (p.options[Rshrink])
         masker.rshrink = std::atof(p.options[Rshrink].arg);
+      if (p.options[MaskSpacing])
+        masker.requested_spacing = std::atof(p.options[MaskSpacing].arg);
 
       gemmi::Scaling<Real> scaling(cell, st.find_spacegroup());
       if (p.options[Ksolv] || p.options[Bsolv] || scale_to.size() != 0) {
         scaling.use_solvent = true;
         if (p.options[Ksolv])
           scaling.k_sol = std::atof(p.options[Ksolv].arg);
         if (p.options[Bsolv])
           scaling.b_sol = std::atof(p.options[Bsolv].arg);
       }
+      if (p.options[Kov])
+        scaling.k_overall = std::atof(p.options[Kov].arg);
       if (p.options[Baniso]) {
         char* endptr = nullptr;
         gemmi::SMat33<double> b_aniso;
         b_aniso.u11 = std::strtod(p.options[Baniso].arg, &endptr);
         b_aniso.u22 = std::strtod(endptr + 1, &endptr);
         b_aniso.u33 = std::strtod(endptr + 1, &endptr);
         b_aniso.u12 = std::strtod(endptr + 1, &endptr);
         b_aniso.u13 = std::strtod(endptr + 1, &endptr);
         b_aniso.u23 = std::strtod(endptr + 1, &endptr);
         scaling.set_b_overall(b_aniso);
       }
       const char* map_file = p.options[WriteMap] ? p.options[WriteMap].arg : nullptr;
-      process_with_fft(st, dencalc, mott_bethe, masker, scaling,
+
+      // mask's coefficients
+      gemmi::AsuData<std::complex<Real>> mask_data;
+      auto mask_data_ptr = &mask_data;
+      if (scaling.use_solvent) {
+        gemmi::Grid<Real> gr;
+        if (p.options[MaskFile]) {
+          gemmi::Ccp4<Real> ccp4;
+          ccp4.read_ccp4(gemmi::MaybeGzipped(p.options[MaskFile].arg));
+          ccp4.setup(0, gemmi::MapSetup::Full);
+          gr = std::move(ccp4.grid);
+        } else {
+          gr.unit_cell = dencalc.grid.unit_cell;
+          gr.spacegroup = dencalc.grid.spacegroup;
+          double spacing = masker.requested_spacing;
+          if (spacing <= 0)
+            spacing = dencalc.requested_grid_spacing();
+          gr.set_size_from_spacing(spacing, gemmi::GridSizeRounding::Up);
+          masker.put_mask_on_grid(gr, st.models[0]);
+        }
+        if (p.options[Verbose])
+          fprintf(stderr, "Solvent mask: %.1f%% of %d x %d x %d grid.\n",
+                  100. * gr.sum() / gr.point_count(), gr.nu, gr.nv, gr.nw);
+        mask_data = transform_map_to_f_phi(gr, /*half_l=*/true)
+                    .prepare_asu_data(dencalc.d_min, 0);
+      } else {
+        mask_data_ptr = nullptr;
+      }
+
+      process_with_fft(st, dencalc, mott_bethe, mask_data_ptr, scaling,
                        p.options[Verbose], file, scale_to, map_file);
     } else {
       if (p.options[Rate] || p.options[RCut] || p.options[Blur] ||
           p.options[Test])
         gemmi::fail("Small molecule SFs are calculated directly. Do not use any\n"
                     "of the FFT-related options: --rate, --blur, --rcut, --test.");
       print_structure_factors_sm(small, calc, mott_bethe, d_min, p.options[Verbose], file);
@@ -801,18 +850,17 @@
     }
   }
 
   char table = p.options[For] ? p.options[For].arg[0] : 'x';
   if (p.options[CifFp] && table != 'x')
     gemmi::fail("Electron scattering has no dispersive part (--ciffp)");
   if (table == 'x' || table == 'm') {
+    gemmi::IT92<float>::ignore_charge = (table == 'm' || !p.options[UseCharge]);
     if (p.options[NormalizeIt92])
       gemmi::IT92<float>::normalize();
-    if (table == 'm')
-      gemmi::IT92<float>::ignore_charge = true;
     process_with_table<gemmi::IT92<float>>(use_st, st, small, wavelength,
                                            table == 'm', p);
   } else if (table == 'e') {
     process_with_table<gemmi::C4322<float>>(use_st, st, small, 0., false, p);
   } else if (table == 'n') {
     process_with_table<gemmi::Neutron92<double>>(use_st, st, small, 0., false, p);
   }
@@ -820,14 +868,20 @@
 
 } // anonymous namespace
 
 int GEMMI_MAIN(int argc, char **argv) {
   OptParser p(EXE_NAME);
   p.simple_parse(argc, argv, Usage);
   p.check_exclusive_group({ToMtz, Test, Compare});
+  if (p.options[MaskFile]) {
+    for (int opt2 : {MaskSpacing, RadiiSet, Rprobe, Rshrink})
+      if (p.options[opt2])
+        std::fprintf(stderr, "WARNING: -%s is ignored when --solvent-mask is given.\n",
+                     p.given_name(opt2));
+  }
   p.require_input_files_as_args();
   try {
     for (int i = 0; i < p.nonOptionsCount(); ++i) {
       std::string input = p.coordinate_input_file(i);
       if (p.options[Verbose]) {
         fprintf(stderr, "Reading file %s ...\n", input.c_str());
         fflush(stderr);
```

### Comparing `gemmi-0.6.5/prog/sg.cpp` & `gemmi-0.6.6/prog/sg.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -102,20 +102,22 @@
   printf("Laue class: %s\n", sg->laue_str());
   printf("Crystal system: %s\n", sg->crystal_system_str());
   gemmi::GroupOps ops = sg->operations();
   printf("Is centrosymmetric: %s\n", ops.is_centrosymmetric() ? "yes" : "no");
   printf("Is enantiomorphic: %s\n", sg->is_enantiomorphic() ? "yes" : "no");
   std::array<int, 3> gf = ops.find_grid_factors();
   printf("Grid restrictions: NX=%dn NY=%dn NZ=%dn\n", gf[0], gf[1], gf[2]);
-  for (bool tnt : {false, true})
-    printf("Reciprocal space ASU (%s)%s: %s%s\n",
-           tnt ? "TNT" : "CCP4",
-           is_reference ? "" : " wrt. standard setting",
-           tnt ? " " : "",
-           gemmi::ReciprocalAsu(sg, tnt).condition_str());
+  std::string wrt;
+  if (!is_reference)
+    wrt = " wrt. " + gemmi::get_spacegroup_reference_setting(sg->number).xhm();
+  printf("CCP4 reciprocal space ASU%s: %s\n",
+         wrt.c_str(),
+         gemmi::ReciprocalAsu(sg, false).condition_str());
+  printf("TNT reciprocal space ASU:  %s\n",
+         gemmi::ReciprocalAsu(sg, true).condition_str());
   gemmi::AsuBrick brick = gemmi::find_asu_brick(sg);
   printf("Direct space ASU brick: %s\n", brick.str().c_str());
   print_symmetry_operations(ops);
   if (verbose)
     print_verbose_info(sg->hall);
   printf("\n");
 }
```

### Comparing `gemmi-0.6.5/prog/tags.cpp` & `gemmi-0.6.6/prog/tags.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/timer.h` & `gemmi-0.6.6/prog/timer.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/validate.cpp` & `gemmi-0.6.6/prog/validate.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/validate_mon.cpp` & `gemmi-0.6.6/prog/validate_mon.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/wcn.cpp` & `gemmi-0.6.6/prog/wcn.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/prog/xds2mtz.cpp` & `gemmi-0.6.6/prog/xds2mtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/pyproject.toml` & `gemmi-0.6.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["scikit-build-core~=0.8.0", "pybind11>=2.6.2",
+requires = ["scikit-build-core~=0.9.0", "pybind11>=2.6.2",
             "pybind11-stubgen~=2.4.2", "numpy"]
 build-backend = "scikit_build_core.build"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "gemmi"
 dynamic = ["version"]
@@ -74,28 +74,28 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "-q"]
 testpaths = ["tests"]
 
 [tool.codespell]
-skip = 'third_party,*.pdb,*.crd,*.cif,*.mmcif,*.ent,*.log*,*.dic,*.idx,tags,*.bak,docs/_build,tests/mmcif_pdbx_v50_frag.dic,docs/*-help.txt'
+skip = 'third_party,*.pdb,*.crd,*.cif,*.mmcif,*.ent,*.log*,*.dic,*.idx,tags,*.bak,docs/_build,tests/mmcif_pdbx_v50_frag.dic,docs/*-help.txt,wasm/node_modules'
 ignore-words-list = 'inout,fo,fom,te,nd,ser,unx,ket,acn,readd,conect'
 
 [tool.cibuildwheel]
 # increase pip debugging output
 build-verbosity = 1
 test-command = "python -m unittest discover -v -s {project}/tests/"
 [tool.cibuildwheel.environment]
 SKBUILD_CMAKE_ARGS = '-DBUILD_GEMMI_PROGRAM=OFF;-DINSTALL_DEV_FILES=OFF;-DBUILD_SHARED_LIBS=OFF;-DFETCH_ZLIB_NG=ON'
 
 # https://cibuildwheel.readthedocs.io/en/stable/faq/#macos-building-cpython-38-wheels-on-arm64
 [[tool.cibuildwheel.overrides]]
 select = "cp38-macosx_arm64"
-environment.SKBUILD_CMAKE_DEFINE = 'GENERATE_STUBS=OFF'
+environment.SKBUILD_CMAKE_ARGS = '-DBUILD_GEMMI_PROGRAM=OFF;-DINSTALL_DEV_FILES=OFF;-DBUILD_SHARED_LIBS=OFF;-DFETCH_ZLIB_NG=ON;-DGENERATE_STUBS=OFF'
 
 [tool.pylint]
 basic.const-naming-style = "any"
 basic.variable-naming-style = "any"
 basic.module-naming-style = "any"
 refactoring.max-nested-blocks = 7
 design.max-locals = 16
```

### Comparing `gemmi-0.6.5/python/align.cpp` & `gemmi-0.6.6/python/align.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/ccp4.cpp` & `gemmi-0.6.6/python/ccp4.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/chemcomp.cpp` & `gemmi-0.6.6/python/chemcomp.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     .def("name_from_alias", &ChemComp::Aliasing::name_from_alias)
     ;
   chemcomp
     .def_readwrite("name", &ChemComp::name)
     .def_readwrite("group", &ChemComp::group)
     .def_readonly("atoms", &ChemComp::atoms)
     .def_readonly("rt", &ChemComp::rt)
+    .def_static("read_group", &ChemComp::read_group)
     .def_static("group_str", &ChemComp::group_str)
     .def("set_group", &ChemComp::set_group)
     .def("get_atom", &ChemComp::get_atom)
     .def("find_atom", [](ChemComp& self, const std::string& atom_id) {
         auto it = self.find_atom(atom_id);
         return it != self.atoms.end() ? &*it : nullptr;
     }, py::return_value_policy::reference_internal)
```

### Comparing `gemmi-0.6.5/python/cif.cpp` & `gemmi-0.6.6/python/cif.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -395,14 +395,15 @@
     .def("get_prefix", &Table::get_prefix)
     .def("has_column", &Table::has_column)
     .def("column", &Table::column, py::arg("n"), py::keep_alive<0, 1>())
     .def("find_row", &Table::find_row, py::keep_alive<0, 1>())
     .def("find_column", &Table::find_column, py::arg("tag"),
          py::keep_alive<0, 1>())
     .def("erase", &Table::erase)
+    .def("ensure_loop", &Table::ensure_loop)
     .def("append_row", &Table::append_row<std::vector<std::string>>,
          py::arg("new_values"))
     .def("remove_row", &Table::remove_row, py::arg("row_index"))
     .def("move_row", &Table::move_row, py::arg("old_pos"), py::arg("new_pos"))
     .def_property_readonly("tags",
             py::cpp_function(&Table::tags, py::keep_alive<0, 1>()))
     .def("__iter__", [](Table& self) {
```

### Comparing `gemmi-0.6.5/python/common.h` & `gemmi-0.6.6/python/common.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/elem.cpp` & `gemmi-0.6.6/python/elem.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/gemmi.cpp` & `gemmi-0.6.6/python/gemmi.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -45,19 +45,15 @@
   m.def("expand_pdb_code_to_path", &gemmi::expand_pdb_code_to_path,
         py::arg("code"), py::arg("filetype"), py::arg("throw_if_unset")=false);
   m.def("expand_if_pdb_code", &gemmi::expand_if_pdb_code,
         py::arg("code"), py::arg("filetype")='M');
   m.attr("hc") = py::float_(gemmi::hc());
   m.def("bessel_i1_over_i0", py::vectorize(gemmi::bessel_i1_over_i0));
   m.def("log_bessel_i0", py::vectorize(gemmi::log_bessel_i0));
-  m.def("log_cosh", py::vectorize([](double x) {
-        // ln(cosh(x)) = ln(e^x + e^-x) - ln(2) = ln(e^x * (1 + e^-2x)) - ln(2)
-        x = std::abs(x);
-        return x + std::log1p(std::exp(-2 * x)) - std::log(2);
-  }));
+  m.def("log_cosh", py::vectorize(gemmi::log_cosh));
 
   // pirfasta.hpp
   py::class_<gemmi::FastaSeq>(m, "FastaSeq")
     .def_readonly("header", &gemmi::FastaSeq::header)
     .def_readonly("seq", &gemmi::FastaSeq::seq)
     ;
   m.def("read_pir_or_fasta", &gemmi::read_pir_or_fasta);
```

### Comparing `gemmi-0.6.5/python/grid.cpp` & `gemmi-0.6.6/python/grid.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     .def("get_point", &Gr::get_point)
     .def("get_nearest_point", (GrPoint (Gr::*)(const Position&)) &Gr::get_nearest_point)
     .def("point_to_fractional", &Gr::point_to_fractional)
     .def("point_to_position", &Gr::point_to_position)
     .def("change_values", &Gr::change_values, py::arg("old_value"), py::arg("new_value"))
     .def("copy_metadata_from", &Gr::copy_metadata_from)
     .def("setup_from", &Gr::template setup_from<Structure>,
-         py::arg("st"), py::arg("spacing"))
+         py::arg("st"), py::arg("spacing")=0.)
     .def("set_unit_cell", (void (Gr::*)(const UnitCell&)) &Gr::set_unit_cell)
     .def("set_points_around", &Gr::set_points_around,
          py::arg("position"), py::arg("radius"), py::arg("value"), py::arg("use_pbc")=true)
     .def("symmetrize_min", &Gr::symmetrize_min)
     .def("symmetrize_max", &Gr::symmetrize_max)
     .def("symmetrize_abs_max", &Gr::symmetrize_abs_max)
     .def("symmetrize_sum", &Gr::symmetrize_sum)
```

### Comparing `gemmi-0.6.5/python/hkl.cpp` & `gemmi-0.6.6/python/hkl.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/meta.cpp` & `gemmi-0.6.6/python/meta.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,18 @@
             return py::make_tuple(self.num, self.icode);
         },
         [](py::tuple t) {
             if (t.size() != 2)
                 throw std::runtime_error("invalid tuple size");
             return SeqId(t[0].cast<int>(), t[1].cast<char>());
         }
-    ));
+    ))
+    .def("__hash__", [](const SeqId& self) {
+        return py::hash(py::make_tuple(self.num, self.icode));
+    });
 
   py::class_<ResidueId>(m, "ResidueId")
     .def(py::init<>())
     .def_readwrite("name", &ResidueId::name)
     .def_readwrite("seqid", &ResidueId::seqid)
     .def_readwrite("segment", &ResidueId::segment)
     .def("__str__", &ResidueId::str)
@@ -262,14 +265,17 @@
     .def(py::init<const std::string&>())
     .def_readwrite("name", &Assembly::name)
     .def_readwrite("author_determined", &Assembly::author_determined)
     .def_readwrite("software_determined", &Assembly::software_determined)
     .def_readwrite("oligomeric_details", &Assembly::oligomeric_details)
     .def_readonly("generators", &Assembly::generators)
     .def_readwrite("special_kind", &Assembly::special_kind)
+    .def("__repr__", [](const Assembly& self) {
+        return cat("<gemmi.Assembly ", self.name, ">");
+    });
     ;
   py::bind_vector<std::vector<Assembly>>(m, "AssemblyList");
 
   py::class_<SoftwareItem> softitem(m, "SoftwareItem");
   py::enum_<SoftwareItem::Classification>(softitem, "Classification")
     .value("DataCollection", SoftwareItem::Classification::DataCollection)
     .value("DataExtraction", SoftwareItem::Classification::DataExtraction)
```

### Comparing `gemmi-0.6.5/python/meta.h` & `gemmi-0.6.6/python/meta.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/miller_a.h` & `gemmi-0.6.6/python/miller_a.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/mol.cpp` & `gemmi-0.6.6/python/mol.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
          py::arg("serial1"), py::arg("serial2"), py::arg("order"))
     .def("clear_conect", [](Structure& self) { self.conect_map.clear(); })
     .def("assign_subchains", &assign_subchains,
          py::arg("force")=false, py::arg("fail_if_unknown")=true)
     .def("ensure_entities", &ensure_entities)
     .def("deduplicate_entities", &deduplicate_entities)
     .def("setup_entities", &setup_entities)
+    .def("assign_het_flags", assign_het_flags<Structure>, py::arg("flag")='R')
     .def("remove_waters", remove_waters<Structure>)
     .def("remove_ligands_and_waters", remove_ligands_and_waters<Structure>)
     .def("shorten_ccd_codes", &shorten_ccd_codes)
     .def("restore_full_ccd_codes", &restore_full_ccd_codes)
     .def_readwrite("shortened_ccd_codes", &Structure::shortened_ccd_codes)
 
     // modify.hpp
@@ -263,14 +264,16 @@
     // deprecated, use has_hydrogen() or count_atom_sites(Selection('[H,D]'))
     .def("count_hydrogen_sites", &count_hydrogen_sites<Model>)
     .def("count_occupancies", &count_occupancies<Model>, py::arg("sel")=nullptr)
     .def("calculate_mass", &calculate_mass<Model>)
     .def("calculate_center_of_mass", [](const Model& self) {
         return calculate_center_of_mass(self).get();
     })
+    .def("calculate_b_iso_range", &calculate_b_iso_range<Model>)
+    .def("calculate_b_aniso_range", &calculate_b_aniso_range)
     .def("transform_pos_and_adp", transform_pos_and_adp<Model>, py::arg("tr"))
     .def("split_chains_by_segments", &split_chains_by_segments)
     .def("clone", [](const Model& self) { return new Model(self); })
     .def("__repr__", [](const Model& self) {
         return cat("<gemmi.Model ", self.name, " with ", self.chains.size(), " chain(s)>");
     });
 
@@ -470,14 +473,15 @@
          py::keep_alive<0, 1>())
     .def("sole_atom", &Residue::sole_atom)
     .def("get_ca", &Residue::get_ca, py::return_value_policy::reference_internal)
     .def("get_p", &Residue::get_p, py::return_value_policy::reference_internal)
     .def("is_water", &Residue::is_water)
     .def("remove_hydrogens", &remove_hydrogens<Residue>)
     .def("trim_to_alanine", (bool (*)(Residue&)) &trim_to_alanine)
+    .def("recommended_het_flag", &recommended_het_flag)
     .def("clone", [](const Residue& self) { return new Residue(self); })
     .def("__repr__", [](const Residue& self) {
         return cat("<gemmi.Residue ", self.str(), " with ", self.atoms.size(), " atoms>");
     });
 
   py::enum_<CalcFlag>(m, "CalcFlag")
     .value("NotSet", CalcFlag::NotSet)
```

### Comparing `gemmi-0.6.5/python/monlib.cpp` & `gemmi-0.6.6/python/monlib.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,16 @@
     .def("update_old_atom_names", &MonLib::update_old_atom_names)
     .def("path", &MonLib::path, py::arg("code")=std::string())
     .def("__repr__", [](const MonLib& self) {
         return "<gemmi.MonLib with " +
                std::to_string(self.monomers.size()) + " monomers, " +
                std::to_string(self.links.size()) + " links, " +
                std::to_string(self.modifications.size()) + " modifications>";
-    });
+    })
+    .def("clone", [](const MonLib& self) { return new MonLib(self); });
 
   m.def("read_monomer_lib", [](const std::string& monomer_dir,
                                const std::vector<std::string>& resnames,
                                const std::string& libin,
                                bool ignore_missing) {
     return read_monomer_lib(monomer_dir, resnames, gemmi::read_cif_gz, libin, ignore_missing);
   }, py::arg("monomer_dir"), py::arg("resnames"), py::arg("libin")=std::string(),
```

### Comparing `gemmi-0.6.5/python/mtz.cpp` & `gemmi-0.6.6/python/mtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/read.cpp` & `gemmi-0.6.6/python/read.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -126,29 +126,34 @@
         return "<gemmi.SmallStructure.AtomType " + self.symbol + ">";
     });
 
   small_structure
     .def(py::init<>())
     .def_readwrite("name", &SmallStructure::name)
     .def_readwrite("cell", &SmallStructure::cell)
+    .def_readonly("spacegroup", &SmallStructure::spacegroup,
+                  py::return_value_policy::reference_internal)
     .def_readwrite("spacegroup_hm", &SmallStructure::spacegroup_hm)
+    .def_readwrite("spacegroup_hall", &SmallStructure::spacegroup_hall)
+    .def_readwrite("spacegroup_number", &SmallStructure::spacegroup_number)
+    .def_readwrite("symops", &SmallStructure::symops)
     .def_readonly("sites", &SmallStructure::sites)
     .def_readonly("atom_types", &SmallStructure::atom_types)
     .def_readwrite("wavelength", &SmallStructure::wavelength)
     .def("add_site", [](SmallStructure& self, const SmallStructure::Site& site) {
         self.sites.push_back(site);
     })
-    .def("find_spacegroup", &SmallStructure::find_spacegroup)
+    .def("set_spacegroup", &SmallStructure::set_spacegroup, py::arg("order"))
+    .def("check_spacegroup", &SmallStructure::check_spacegroup)
     .def("get_atom_type", &SmallStructure::get_atom_type)
     .def("get_all_unit_cell_sites", &SmallStructure::get_all_unit_cell_sites)
     .def("remove_hydrogens", &SmallStructure::remove_hydrogens)
     .def("change_occupancies_to_crystallographic",
          &SmallStructure::change_occupancies_to_crystallographic,
          py::arg("max_dist")=0.4)
-    .def("setup_cell_images", &SmallStructure::setup_cell_images)
     .def("make_cif_block", &make_cif_block_from_small_structure)
     .def("__repr__", [](const SmallStructure& self) {
         return "<gemmi.SmallStructure: " + std::string(self.name) + ">";
     });
   m.def("mx_to_sx_structure", &gemmi::mx_to_sx_structure,
         py::arg("st"), py::arg("n")=0);
 }
```

### Comparing `gemmi-0.6.5/python/recgrid.cpp` & `gemmi-0.6.6/python/recgrid.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/scaling.cpp` & `gemmi-0.6.6/python/scaling.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     .def_property("b_overall", &Scaling::get_b_overall, &Scaling::set_b_overall)
     .def_readwrite("use_solvent", &Scaling::use_solvent)
     .def_readwrite("k_sol", &Scaling::k_sol)
     .def_readwrite("b_sol", &Scaling::b_sol)
     .def("prepare_points", &Scaling::prepare_points,
          py::arg("calc"), py::arg("obs"), py::arg("mask")=static_cast<FPhiData*>(nullptr))
     .def("fit_isotropic_b_approximately", &Scaling::fit_isotropic_b_approximately)
+    .def("fit_b_star_approximately", &Scaling::fit_b_star_approximately)
     .def("fit_parameters", &Scaling::fit_parameters)
     .def("get_overall_scale_factor", &Scaling::get_overall_scale_factor, py::arg("hkl"))
     .def("get_overall_scale_factor", [](const Scaling& self, py::array_t<int> hkl) {
         auto h = hkl.unchecked<2>();
         if (h.shape(1) != 3)
           throw std::domain_error("the hkl array must have size N x 3");
         auto len = h.shape(0);
```

### Comparing `gemmi-0.6.5/python/search.cpp` & `gemmi-0.6.6/python/search.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/sf.cpp` & `gemmi-0.6.6/python/sf.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,22 @@
     .def(py::init<>())
     .def_readonly("grid", &DenCalc::grid)
     .def_readwrite("d_min", &DenCalc::d_min)
     .def_readwrite("rate", &DenCalc::rate)
     .def_readwrite("blur", &DenCalc::blur)
     .def_readwrite("cutoff", &DenCalc::cutoff)
     .def_readwrite("addends", &DenCalc::addends)
-    .def("set_refmac_compatible_blur", &DenCalc::set_refmac_compatible_blur)
+    .def("set_refmac_compatible_blur", &DenCalc::set_refmac_compatible_blur,
+         py::arg("model"), py::arg("allow_negative")=false)
     .def("put_model_density_on_grid", &DenCalc::put_model_density_on_grid)
     .def("initialize_grid", &DenCalc::initialize_grid)
     .def("add_model_density_to_grid", &DenCalc::add_model_density_to_grid)
     .def("add_atom_density_to_grid", &DenCalc::add_atom_density_to_grid)
     .def("add_c_contribution_to_grid", &DenCalc::add_c_contribution_to_grid)
+    // deprecated
     .def("set_grid_cell_and_spacegroup", &DenCalc::set_grid_cell_and_spacegroup)
     .def("reciprocal_space_multiplier", &DenCalc::reciprocal_space_multiplier)
     .def("mott_bethe_factor", &DenCalc::mott_bethe_factor)
     .def("estimate_radius", [](const DenCalc &self, const gemmi::Atom &atom) {
         double b = atom.b_iso;
         // rough estimate, so we don't calculate eigenvalues
         float max_b = std::max(std::max(atom.aniso.u11, atom.aniso.u22), atom.aniso.u33);
```

### Comparing `gemmi-0.6.5/python/sym.cpp` & `gemmi-0.6.6/python/sym.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     .def("laue_str", &SpaceGroup::laue_str,
          "Returns name of the Laue class (for centrosymmetric groups "
          "the same as point_group_hm).")
     .def("crystal_system", &SpaceGroup::crystal_system)
     .def("crystal_system_str", &SpaceGroup::crystal_system_str,
          "Returns lower-case name of the crystal system.")
     .def("is_centrosymmetric", &SpaceGroup::is_centrosymmetric)
+    .def("monoclinic_unique_axis", &SpaceGroup::monoclinic_unique_axis)
     .def("is_reference_setting", &SpaceGroup::is_reference_setting)
     .def("centred_to_primitive", &SpaceGroup::centred_to_primitive)
     .def("change_of_hand_op", &SpaceGroup::change_of_hand_op)
     .def("operations", &SpaceGroup::operations, "Group of operations")
     .def("switch_to_asu", [](const SpaceGroup& sg, py::array_t<int> hkl) {
         auto h = hkl.mutable_unchecked<2>();
         if (h.shape(1) < 3)
@@ -218,15 +219,15 @@
         "Parse Hall notation.");
   m.def("symops_from_hall", &symops_from_hall, py::arg("hall"),
         "Parse Hall notation.");
   m.def("find_spacegroup_by_number", &find_spacegroup_by_number,
         py::arg("ccp4"), py::return_value_policy::reference,
         "Returns space-group of given number.");
   m.def("find_spacegroup_by_name", &find_spacegroup_by_name,
-        py::arg("hm"), py::arg("alpha")=0., py::arg("gamma")=0.,
+        py::arg("hm"), py::arg("alpha")=0., py::arg("gamma")=0., py::arg("prefer")=nullptr,
         py::return_value_policy::reference,
         "Returns space-group with given name.");
   m.def("get_spacegroup_reference_setting", &get_spacegroup_reference_setting,
         py::arg("number"), py::return_value_policy::reference);
   m.def("find_spacegroup_by_ops", &find_spacegroup_by_ops,
         py::arg("group_ops"), py::return_value_policy::reference,
         "Returns space-group with identical operations.");
```

### Comparing `gemmi-0.6.5/python/topo.cpp` & `gemmi-0.6.6/python/topo.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -181,8 +181,9 @@
        py::arg("warnings")=py::none(), py::arg("ignore_unknown_links")=false,
        py::arg("use_cispeps")=false);
 
   // crd.hpp
   m.def("setup_for_crd", &setup_for_crd);
   m.def("prepare_refmac_crd", &prepare_refmac_crd);
   m.def("add_automatic_links", &add_automatic_links);
+  m.def("add_dictionary_blocks", &add_dictionary_blocks);
 }
```

### Comparing `gemmi-0.6.5/python/tostr.hpp` & `gemmi-0.6.6/python/tostr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/unitcell.cpp` & `gemmi-0.6.6/python/unitcell.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/python/write.cpp` & `gemmi-0.6.6/python/write.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/align.cpp` & `gemmi-0.6.6/src/align.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/assembly.cpp` & `gemmi-0.6.6/src/assembly.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/calculate.cpp` & `gemmi-0.6.6/src/calculate.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/crd.cpp` & `gemmi-0.6.6/src/crd.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,20 @@
                                      "##############"});
   items.emplace_back("_symmetry.entry_id", id);
   const std::string& hm = st.spacegroup_hm;
   items.emplace_back("_symmetry.space_group_name_H-M", cif::quote(hm));
   if (const SpaceGroup* sg = st.find_spacegroup())
     items.emplace_back("_symmetry.Int_Tables_number",
                        std::to_string(sg->number));
+  if (!st.ncs.empty()) {
+    items.emplace_back(cif::CommentArg{"#########\n"
+                                       "## NCS ##\n"
+                                       "#########"});
+    write_ncs_oper(st, block);
+  }
   const Model& model0 = st.first_model();
   items.emplace_back(cif::CommentArg{"#################\n"
                                      "## STRUCT_ASYM ##\n"
                                      "#################"});
   cif::Loop& asym_loop = block.init_mmcif_loop("_struct_asym.",
                                                {"id", "entity_id"});
   for (const Chain& chain : model0.chains)
@@ -522,22 +528,28 @@
 
   return block;
 }
 
 cif::Document prepare_refmac_crd(Structure& st, const Topo& topo,
                                  const MonLib& monlib, HydrogenChange h_change) {
   cif::Document doc;
-  std::string info_comment = "# Refmac CRD file generated with gemmi " GEMMI_VERSION
-                             "\n# Monomer library version: " + monlib.lib_version;
+  std::string info_comment = "# Refmac CRD file generated with gemmi " GEMMI_VERSION;
   std::vector<std::string> resnames = st.models.at(0).get_all_residue_names();
   shorten_ccd_codes(st);
   doc.blocks.push_back(prepare_crd(st, topo, h_change, info_comment));
   doc.blocks.push_back(prepare_rst(topo, monlib, st.cell));
 
   doc.blocks.emplace_back("for_refmac_mmcif");
+  add_dictionary_blocks(doc, resnames, topo, monlib);
+
+  return doc;
+}
+
+void add_dictionary_blocks(cif::Document& doc, const std::vector<std::string>& resnames,
+                           const Topo& topo, const MonLib& monlib) {
   for (const std::string& resname : resnames) {
     auto it = monlib.monomers.find(resname);
     if (it != monlib.monomers.end()) {
       const ChemComp& cc = it->second;
       doc.blocks.emplace_back(cc.name);
       cif::Block& block = doc.blocks.back();
       block.items.emplace_back("_chem_comp.id", cc.name);
@@ -581,12 +593,10 @@
   for (const std::string& mod_name : used_mods)
     if (const ChemMod* mod = monlib.get_mod(mod_name)) {
       doc.blocks.push_back(mod->block);
       cif::Block& block = doc.blocks.back();
       block.init_mmcif_loop("_chem_mod.", {"id", "name", "comp_id", "group_id"})
         .add_row({q(mod->id), q(mod->name), q(mod->comp_id), q(mod->group_id)});
     }
-
-  return doc;
 }
 
 }
```

### Comparing `gemmi-0.6.5/src/ddl.cpp` & `gemmi-0.6.6/src/ddl.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/eig3.cpp` & `gemmi-0.6.6/src/eig3.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/gz.cpp` & `gemmi-0.6.6/src/gz.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 # include <zlib.h>
 # define GG(name) name
 #endif
 #include <gemmi/fileutil.hpp> // file_open
 
 namespace gemmi {
 
+const char* const zlib_description =
+#if USE_ZLIB_NG
+  "zlib-ng " ZLIBNG_VERSION;
+#else
+  "zlib " ZLIB_VERSION;
+#endif
+
 // Throws if the size is not found or if it is suspicious.
 // Anything outside of the arbitrary limits from 1 to 10x of the compressed
 // size looks suspicious to us.
 // **This function should not be relied upon.**
 // In particular, if the return values is >= 4GiB - it's only a guess.
 size_t estimate_uncompressed_size(const std::string& path) {
   fileptr_t f = file_open(path.c_str(), "rb");
```

### Comparing `gemmi-0.6.5/src/intensit.cpp` & `gemmi-0.6.6/src/intensit.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/json.cpp` & `gemmi-0.6.6/src/json.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/mmcif.cpp` & `gemmi-0.6.6/src/mmcif.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -624,22 +624,24 @@
     copy_double(row, 7, exper.reflections.r_sym);
     copy_double(row, 8, exper.reflections.mean_I_over_sigma);
   }
 
   for (auto row : block.find("_software.", {"name",
                                             "?classification",
                                             "?version",
-                                            "?date"})) {
+                                            "?date",
+                                            "?description"})) {
     st.meta.software.emplace_back();
     SoftwareItem& item = st.meta.software.back();
     item.name = row.str(0);
     if (row.has2(1))
       item.classification = software_classification_from_string(row.str(1));
     copy_string(row, 2, item.version);
     copy_string(row, 3, item.date);
+    copy_string(row, 4, item.description);
   }
 
   std::vector<std::string> ncs_oper_tags = transform_tags("matrix", "vector");
   ncs_oper_tags.emplace_back("id");  // 12
   ncs_oper_tags.emplace_back("?code");  // 13
   cif::Table ncs_oper = block.find("_struct_ncs_oper.", ncs_oper_tags);
   for (auto op : ncs_oper) {
@@ -808,26 +810,28 @@
     ent.polymer_type = PolymerType::Unknown;
     if (polymer_types.ok()) {
       try {
         std::string poly_type = polymer_types.find_row(ent.name).str(1);
         ent.polymer_type = polymer_type_from_string(poly_type);
       } catch (std::runtime_error&) {}
     }
+    // _entity_poly_seq is supposed to reflect heterogeneities in _atom_site.
+    ent.reflects_microhetero = true;
     st.entities.push_back(ent);
   }
 
   for (auto row : block.find("_entity_poly_seq.",
                              {"entity_id", "num", "mon_id"}))
     if (Entity* ent = st.get_entity(row.str(0))) {
       // According to the spec, num must be >= 1.
       int pos = cif::as_int(row[1], 0) - 1;
       if (pos == (int) ent->full_sequence.size())
         ent->full_sequence.push_back(row.str(2));
       else if (pos >= 0 && pos < (int) ent->full_sequence.size())
-        ent->full_sequence[pos] += "," + row.str(2);
+        cat_to(ent->full_sequence[pos], ',', row.str(2));
     }
 
   cif::Table struct_ref = block.find("_struct_ref.",
       {"id", "entity_id", "db_name", "db_code",
        "?pdbx_db_accession", "?pdbx_db_isoform"});
   cif::Table struct_ref_seq = block.find("_struct_ref_seq.",
       {"ref_id", "seq_align_beg", "seq_align_end",                   // 0-2
```

### Comparing `gemmi-0.6.5/src/mmread_gz.cpp` & `gemmi-0.6.6/src/mmread_gz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/monlib.cpp` & `gemmi-0.6.6/src/monlib.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/mtz.cpp` & `gemmi-0.6.6/src/mtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/mtz2cif.cpp` & `gemmi-0.6.6/src/mtz2cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/polyheur.cpp` & `gemmi-0.6.6/src/polyheur.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 // Copyright 2017-2022 Global Phasing Ltd.
 
 #include <gemmi/polyheur.hpp>
 #include <gemmi/resinfo.hpp>   // for find_tabulated_residue
+#include <gemmi/modify.hpp>   // for rename_residues
 
 namespace gemmi {
 
 PolymerType check_polymer_type(const ConstResidueSpan& span, bool ignore_entity_type) {
   if (span.empty())
     return PolymerType::Unknown;
   size_t counts[(int)ResidueKind::ELS+1] = {0};
@@ -76,30 +77,39 @@
   }
   return seq;
 }
 
 static std::vector<Residue>::iterator infer_polymer_end(Chain& chain, PolymerType ptype) {
   auto b = chain.residues.begin();
   auto e = chain.residues.end();
+
+  // find the last residue w/ record type ATOM
+  auto last_a = e;
+  for (auto it = e; it-- != b;)
+    if (it->het_flag == 'A')
+      last_a = it;
+
   for (auto it = b; it != e; ++it) {
     ResidueInfo info = find_tabulated_residue(it->name);
     if (info.found()) {
       if (info.is_water()) {
         e = it;
         break;
       }
       bool maybe_linking = (is_polypeptide(ptype) && info.is_peptide_linking())
                         || (is_polynucleotide(ptype) && info.is_na_linking());
       // The first residue could be non-polymer.
       if (!maybe_linking && b != chain.residues.begin()) {
         e = it;
         break;
       }
-      // If a standard residue is HETATM we assume that it is in the buffer.
-      if (info.is_standard() && it->het_flag == 'H') {
+      // If a standard residue is HETATM, it should be in the buffer. Although
+      // it could happen that a non-standard residue was mutated to a standard
+      // one, but the record type was not updated, so it's not 100% reliable.
+      if (info.is_standard() && it->het_flag == 'H' && it > last_a) {
         e = it;
         break;
       }
       if (maybe_linking && info.is_standard())
         b = it;
     }
   }
@@ -287,57 +297,40 @@
             j->full_sequence == i->full_sequence &&
             j->dbrefs == i->dbrefs) {
           vector_move_extend(i->subchains, std::move(j->subchains));
           st.entities.erase(j--);
         }
 }
 
-void change_ccd_code(Structure& st, const std::string& old, const std::string& new_) {
-  auto process = [&](ResidueId& rid) {
-    if (rid.name == old)
-      rid.name = new_;
+char recommended_het_flag(const Residue& res) {
+    if (res.entity_type == EntityType::Unknown)
+      return '\0';
+    if (res.entity_type == EntityType::Polymer &&
+        find_tabulated_residue(res.name).is_standard())
+      return 'A';
+    return 'H';
+}
+
+bool trim_to_alanine(Residue& res) {
+  static const std::pair<std::string, El> ala_atoms[6] = {
+    {"N", El::N}, {"CA", El::C}, {"C", El::C}, {"O", El::O}, {"CB", El::C},
+    {"OXT", El::O}
   };
-  for (Model& model : st.models)
-    for (Chain& chain : model.chains)
-      for (Residue& res : chain.residues)
-        process(res);
-  for (Entity& ent : st.entities)
-    for (std::string& mon_ids : ent.full_sequence)
-      for (size_t start = 0;;) {
-        size_t end = mon_ids.find(',', start);
-        if (mon_ids.compare(start, end-start, old) == 0) {
-          mon_ids.replace(start, end-start, new_);
-          if (end != std::string::npos)
-            end = start + new_.size();
-        }
-        if (end == std::string::npos)
-          break;
-        start = end + 1;
-      }
-  for (Connection& conn : st.connections) {
-    process(conn.partner1.res_id);
-    process(conn.partner2.res_id);
-  }
-  for (CisPep& cispep : st.cispeps) {
-    process(cispep.partner_c.res_id);
-    process(cispep.partner_n.res_id);
-  }
-  for (ModRes& modres : st.mod_residues)
-    process(modres.res_id);
-  for (Helix& helix : st.helices) {
-    process(helix.start.res_id);
-    process(helix.end.res_id);
-  }
-  for (Sheet& sheet : st.sheets)
-    for (Sheet::Strand& strand : sheet.strands) {
-      process(strand.start.res_id);
-      process(strand.end.res_id);
-      process(strand.hbond_atom2.res_id);
-      process(strand.hbond_atom1.res_id);
-    }
+  if (res.get_ca() == nullptr)
+    return false;
+  vector_remove_if(res.atoms, [](const Atom& a) {
+      for (const auto& name_el : ala_atoms)
+        if (a.name == name_el.first && a.element == name_el.second)
+          return false;
+      return true;
+  });
+  // if non-standard polymer residue was mutated, update het_flag
+  if (res.entity_type == EntityType::Polymer && res.het_flag == 'H')
+    res.het_flag = 'A';
+  return true;
 }
 
 template <size_t I, typename T1, typename T2>
 bool in_vector_at(T1& x, std::vector<T2>& v) {
   for (const auto& el : v)
     if (std::get<I>(el) == x)
       return true;
@@ -369,23 +362,65 @@
   // the first try on renaming: ABCDE -> ~DE
   for (auto& old_new : st.shortened_ccd_codes) {
     const std::string& old = old_new.first;
     char short_code[4] = {'~', *(old.end()-2), *(old.end()-1), '\0'};
     if (!in_vector_at<1>(short_code, st.shortened_ccd_codes))
       old_new.second = short_code;
   }
-  // pick a new residue name and call change_ccd_code()
+  // pick a new residue name and call rename_residues()
   int i = -1;
   for (auto& old_new : st.shortened_ccd_codes) {
     // If ~DE was not unique, use ~00, ~01, ...
     // After ~99, the middle character will be punctuation or letter.
     // After ~Z9 (430+ names), we give up and the names will be empty.
     while (old_new.second.empty() && ++i < 'Z'*10) {
       char short_code[4] = {'~', char('0' + i/10), char('0' + i%10), '\0'};
       if (!in_vector_at<1>(short_code, st.shortened_ccd_codes))
         old_new.second = short_code;
     }
-    change_ccd_code(st, old_new.first, old_new.second);
+    rename_residues(st, old_new.first, old_new.second);
+  }
+}
+
+void restore_full_ccd_codes(Structure& st) {
+  for (const auto& item : st.shortened_ccd_codes)
+    rename_residues(st, item.second, item.first);
+  st.shortened_ccd_codes.clear();
+}
+
+// Unlike _entity_poly_seq, SEQRES doesn't contain alternative residue names.
+// This function adds the alternative names to full_sequence.
+void add_microhetero_to_sequence(Entity& ent, ConstResidueSpan polymer) {
+  ent.reflects_microhetero = false;
+  int max_n = -1;  // max label_seq seen so far
+  for (const Residue& res : polymer) {
+    int n = *res.label_seq;
+    if (size_t(n-1) > ent.full_sequence.size())
+      return;
+    std::string& seq_item = ent.full_sequence[n-1];
+    if (n > max_n) {
+      if (!is_in_list(res.name, seq_item))
+        return;
+      max_n = n;
+    } else {  // n < max_n shouldn't happen
+      if (!is_in_list(res.name, seq_item))
+        cat_to(seq_item, ',', res.name);
+    }
+  }
+  ent.reflects_microhetero = true;
+}
+
+void add_microhetero_to_sequences(Structure& st, bool overwrite) {
+  if (st.models.empty())
+    return;
+  for (Entity& ent : st.entities) {
+    if (ent.subchains.empty())
+      continue;
+    ConstResidueSpan polymer = st.models[0].get_subchain(ent.subchains[0]);
+    if (!polymer || !polymer.front().label_seq)
+      continue;
+    if (overwrite || !ent.reflects_microhetero)
+      add_microhetero_to_sequence(ent, polymer);
   }
 }
 
 } // namespace gemmi
```

### Comparing `gemmi-0.6.5/src/resinfo.cpp` & `gemmi-0.6.6/src/resinfo.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/riding_h.cpp` & `gemmi-0.6.6/src/riding_h.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -142,30 +142,25 @@
       double theta = pi();
       if (const Angle* ang = topo.take_angle(hs[1].ptr, &atom, hs[0].ptr))
         theta = ang->radians();
       hs[1].pos = atom.pos + Position(hs[1].dist * cos(theta),
                                       hs[1].dist * sin(theta), 0);
     }
     if (hs.size() > 2) {
-      if (hs.size() == 3) {
-        // for now only NH3 (NH2.cif and NH3.cif) has such configuration,
-        // so we are cheating here a little.
-        double y = 2 * atom.pos.y - hs[1].pos.y;
-        hs[2].pos = Position(hs[1].pos.x, y, hs[1].pos.z);
-      } else if (hs.size() == 4) {
-        // similarly, only CH4 (CH2.cif) and NH4 (NH4.cif) are handled here
-        const Angle* ang1 = topo.take_angle(hs[2].ptr, &atom, hs[0].ptr);
-        const Angle* ang2 = topo.take_angle(hs[2].ptr, &atom, hs[1].ptr);
-        double theta1 = rad(ang1 ? ang1->value : 109.47122);
-        double theta2 = rad(ang2 ? ang2->value : 109.47122);
-        auto pos = position_from_two_angles(atom.pos, hs[0].pos, hs[1].pos,
-                                            hs[2].dist, theta1, theta2);
-        hs[2].pos = pos.first;
+      const Angle* ang1 = topo.take_angle(hs[2].ptr, &atom, hs[0].ptr);
+      const Angle* ang2 = topo.take_angle(hs[2].ptr, &atom, hs[1].ptr);
+      double theta1 = rad(ang1 ? ang1->value : 109.47122);
+      double theta2 = rad(ang2 ? ang2->value : 109.47122);
+      auto pos = position_from_two_angles(atom.pos, hs[0].pos, hs[1].pos,
+                                          hs[2].dist, theta1, theta2);
+      hs[2].pos = pos.first;
+      // 3 hydrogens: for now happens only NH3 (NH2.cif and NH3.cif)
+      // 4 hydrogens: CH4 (CH2.cif) and NH4 (NH4.cif)
+      if (hs.size() == 4)
         hs[3].pos = pos.second;
-      }
     }
 
   // ==== one heavy atom and hydrogens ====
   } else if (known.size() == 1) {
     const BondedAtom& h = hs[0];
     const BondedAtom& heavy = known[0];
     const Restraints::Angle* angle = topo.take_angle(h.ptr, &atom, heavy.ptr);
```

### Comparing `gemmi-0.6.5/src/sprintf.cpp` & `gemmi-0.6.6/src/sprintf.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/to_mmcif.cpp` & `gemmi-0.6.6/src/to_mmcif.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,21 @@
   span.set_pair("_cell.length_b",    to_str(cell.b));
   span.set_pair("_cell.length_c",    to_str(cell.c));
   span.set_pair("_cell.angle_alpha", to_str(cell.alpha));
   span.set_pair("_cell.angle_beta",  to_str(cell.beta));
   span.set_pair("_cell.angle_gamma", to_str(cell.gamma));
 }
 
+bool is_valid_block_name(const std::string& name) {
+  return !name.empty() &&
+         std::all_of(name.begin(), name.end(), [](char c){ return c >= '!' && c <= '~'; });
+}
+
+} // anonymous namespace
+
 void write_ncs_oper(const Structure& st, cif::Block& block) {
   // _struct_ncs_oper (MTRIX)
   if (st.ncs.empty())
     return;
   cif::Loop& ncs_oper = block.init_mmcif_loop("_struct_ncs_oper.",
       {"id", "code",
        "matrix[1][1]", "matrix[1][2]", "matrix[1][3]", "vector[1]",
@@ -317,21 +324,14 @@
   if (identity != st.info.end() &&
       !in_vector_f([&](const NcsOp& op) { return op.id == identity->second; }, st.ncs))
     add_op(NcsOp{identity->second, true, {}});
   for (const NcsOp& op : st.ncs)
     add_op(op);
 }
 
-bool is_valid_block_name(const std::string& name) {
-  return !name.empty() &&
-         std::all_of(name.begin(), name.end(), [](char c){ return c >= '!' && c <= '~'; });
-}
-
-} // anonymous namespace
-
 void write_struct_conn(const Structure& st, cif::Block& block) {
   // example:
   // disulf1 disulf A CYS 3  SG ? 3 ? 1_555 A CYS 18 SG ? 18 ?  1_555 ? 2.045
   std::array<bool,(int)Connection::Type::Unknown+1> type_ids{};
   bool use_ccp4_link_id = false;
   for (const Connection& con : st.connections)
     if (!con.link_id.empty())
@@ -1102,31 +1102,33 @@
     cif::Loop& atom_type_loop = block.init_mmcif_loop("_atom_type.", {"symbol"});
     for (int i = 0; i < (int)El::END; ++i)
       if (types[i])
         atom_type_loop.add_row({Element((El)i).uname()});
   }
 
   if (groups.entity_poly_seq) {
-    // SEQRES from PDB doesn't record microheterogeneity, so if the resulting
-    // cif has unknown("?") _entity_poly_seq.num, it cannot be trusted.
     cif::Loop& poly_loop = block.init_mmcif_loop("_entity_poly_seq.",
-                                           {"entity_id", "num", "mon_id"});
+                                     {"entity_id", "num", "mon_id", "hetero"});
     for (const Entity& ent : st.entities)
-      if (ent.entity_type == EntityType::Polymer)
+      if (ent.entity_type == EntityType::Polymer) {
+        // SEQRES from PDB doesn't record microheterogeneity.
+        std::string hetero_no = ent.reflects_microhetero ? "n" : "?";
         for (size_t i = 0; i != ent.full_sequence.size(); ++i) {
           const std::string& mon_ids = ent.full_sequence[i];
           std::string num = std::to_string(i+1);
           size_t start = 0, end;
           while ((end = mon_ids.find(',', start)) != std::string::npos) {
             poly_loop.add_row({qchain(ent.name), num,
-                               mon_ids.substr(start, end-start)});
+                               mon_ids.substr(start, end-start), "y"});
             start = end + 1;
           }
-          poly_loop.add_row({qchain(ent.name), num, mon_ids.substr(start)});
+          poly_loop.add_row({qchain(ent.name), num, mon_ids.substr(start),
+                             start == 0 ? hetero_no : "y"});
         }
+      }
   }
 
   if (groups.atoms)
     add_cif_atoms(st, block, groups.group_pdb, groups.auth_all);
 
   if (groups.tls && st.meta.has_tls()) {
     cif::Loop& loop = block.init_mmcif_loop("_pdbx_refine_tls.", {
@@ -1167,23 +1169,24 @@
                               string_or_qmark(sel.chain),
                               sel.res_end.num ? sel.res_end.str() : "?",
                               string_or_qmark(sel.details)});
   }
 
   if (groups.software && !st.meta.software.empty()) {
     cif::Loop& loop = block.init_mmcif_loop("_software.",
-                 {"pdbx_ordinal", "classification", "name", "version", "date"});
+        {"pdbx_ordinal", "classification", "name", "version", "date", "description"});
     int ordinal = 0;
     for (const SoftwareItem& item : st.meta.software)
       loop.add_row({
           std::to_string(++ordinal),
           cif::quote(software_classification_to_string(item.classification)),
           cif::quote(item.name),
           string_or_dot(item.version),
-          string_or_qmark(item.date)});
+          string_or_qmark(item.date),
+          string_or_qmark(item.description)});
   }
 }
 
 cif::Document make_mmcif_document(const Structure& st, MmcifOutputGroups groups) {
   cif::Document doc;
   doc.blocks.resize(1);
   update_mmcif_block(st, doc.blocks[0], groups);
```

### Comparing `gemmi-0.6.5/src/to_pdb.cpp` & `gemmi-0.6.6/src/to_pdb.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -234,42 +234,56 @@
       // 47-54  8f  z
       // 55-60  6f  occupancy (6.2)
       // 61-66  6f  temperature factor (6.2)
       // 67-76  6   -
       // 73-76      segment identifier, left-justified (non-standard)
       // 77-78  2s  element symbol, right-justified
       // 79-80  2s  charge
-      WRITE("%-6s%5s %-4.4s%c%3.3s"
-            "%2s%5s   %8.3f%8.3f%8.3f"
-            "%6.2f%6.2f      %-4.4s%2s%c%c",
+      int written_bytes = snprintf_z(buf, 82,
+            "%-6s%5s %-4.4s%c%3.3s"
+            "%2s%5s   %8.3f%8.3f%8.3f",
             as_het ? "HETATM" : "ATOM",
             encode_serial_in_hybrid36(serial).data(),
             a.padded_name().c_str(),
             a.altloc ? std::toupper(a.altloc) : ' ',
             res.name.c_str(),
             chain.name.c_str(),
             write_seq_id(res.seqid).data(),
             // We want to avoid negative zero and round the numbers up
             // if they originally had one digit more and that digit was 5.
             a.pos.x > -5e-4 && a.pos.x < 0 ? 0 : a.pos.x + 1e-10,
             a.pos.y > -5e-4 && a.pos.y < 0 ? 0 : a.pos.y + 1e-10,
-            a.pos.z > -5e-4 && a.pos.z < 0 ? 0 : a.pos.z + 1e-10,
+            a.pos.z > -5e-4 && a.pos.z < 0 ? 0 : a.pos.z + 1e-10);
+      if GEMMI_UNLIKELY(written_bytes > 54) {
+        // The only items expected to overflow above are the coordinates,
+        // if the integer part of the number exceeds 5 characters.
+        // This happens when something goes wrong and the model is far from
+        // the origin. Such a model should be shifted; it can't be written it
+        // in a spec-conforming format: Real(8.3). Here we overwrite the last
+        // digits - trimming is better than overflowing the line.
+        snprintf_z(buf+38, 82-38, "%8.3f", a.pos.y);
+        snprintf_z(buf+46, 82-46, "%8.3f", a.pos.z);
+      }
+      snprintf_z(buf+54, 82-54,
+            "%6.2f%6.2f      %-4.4s%2s%c%c",
             // Occupancy is stored as single prec, but we know it's <= 1,
             // so no precision is lost even if it had 6 digits after dot.
             a.occ + 1e-6,
             // B is harder to get rounded right. It is stored as float,
             // and may be given with more than single precision in mmCIF
             // If it was originally %.5f (5TIS) we need to add 0.5 * 10^-5.
             std::min(a.b_iso + 0.5e-5, 999.99),
             res.segment.c_str(),
             a.element.uname(),
             // Charge is written as 1+ or 2-, etc, or just empty space.
             // Sometimes PDB files have explicit 0s (5M05); we ignore them.
             a.charge ? a.charge > 0 ? '0'+a.charge : '0'-a.charge : ' ',
             a.charge ? a.charge > 0 ? '+' : '-' : ' ');
+      buf[80] = '\n';
+      os.write(buf, 81);
       if (a.aniso.nonzero()) {
         // re-using part of the buffer
         std::memcpy(buf, "ANISOU", 6);
         const double eps = 1e-6;
         snprintf_z(buf+28, 43, "%7.0f%7.0f%7.0f%7.0f%7.0f%7.0f",
                    a.aniso.u11*1e4 + eps, a.aniso.u22*1e4 + eps,
                    a.aniso.u33*1e4 + eps, a.aniso.u12*1e4 + eps,
```

### Comparing `gemmi-0.6.5/src/topo.cpp` & `gemmi-0.6.6/src/topo.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/src/xds_ascii.cpp` & `gemmi-0.6.6/src/xds_ascii.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1011031.cif` & `gemmi-0.6.6/tests/1011031.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1lzh.pdb.gz` & `gemmi-0.6.6/tests/1lzh.pdb.gz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1orc.pdb` & `gemmi-0.6.6/tests/1orc.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1pfe.cif.gz` & `gemmi-0.6.6/tests/1pfe.cif.gz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1pfe.json` & `gemmi-0.6.6/tests/1pfe.json`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/1pfe_asu.msk.gz` & `gemmi-0.6.6/tests/1pfe_asu.msk.gz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/2013551.cif` & `gemmi-0.6.6/tests/2013551.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/2242624.cif` & `gemmi-0.6.6/tests/2242624.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/2242624.hkl` & `gemmi-0.6.6/tests/2242624.hkl`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/3dg1_final.cif` & `gemmi-0.6.6/tests/3dg1_final.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/3wup.json.gz` & `gemmi-0.6.6/tests/3wup.json.gz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/4003024.cif` & `gemmi-0.6.6/tests/4003024.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/4aap-sf-subset.cif` & `gemmi-0.6.6/tests/4aap-sf-subset.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/4hhh_frag.pdb` & `gemmi-0.6.6/tests/4hhh_frag.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/4oz7.pdb` & `gemmi-0.6.6/tests/4oz7.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5cvz_final.pdb` & `gemmi-0.6.6/tests/5cvz_final.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5e5z.mtz` & `gemmi-0.6.6/tests/5e5z.mtz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5i55.cif` & `gemmi-0.6.6/tests/5i55.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5i55_tiny.ccp4` & `gemmi-0.6.6/tests/5i55_tiny.ccp4`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5moo_header.pdb` & `gemmi-0.6.6/tests/5moo_header.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5wkd.pdb` & `gemmi-0.6.6/tests/5wkd.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/5wkd_phases.mtz.gz` & `gemmi-0.6.6/tests/5wkd_phases.mtz.gz`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/HEM.cif` & `gemmi-0.6.6/tests/HEM.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/HEM.pdb` & `gemmi-0.6.6/tests/HEM.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/HEN.cif` & `gemmi-0.6.6/tests/HEN.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/SO3.cif` & `gemmi-0.6.6/tests/SO3.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/cif.cpp` & `gemmi-0.6.6/tests/cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/common.py` & `gemmi-0.6.6/tests/common.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/disulf.cpp` & `gemmi-0.6.6/tests/disulf.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/eol-test.cif` & `gemmi-0.6.6/tests/eol-test.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/main.cpp` & `gemmi-0.6.6/tests/main.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/misc.cif` & `gemmi-0.6.6/tests/misc.cif`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/misc.json` & `gemmi-0.6.6/tests/misc.json`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/mmcif_pdbx_v50_frag.dic` & `gemmi-0.6.6/tests/mmcif_pdbx_v50_frag.dic`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/pdb1gdr.ent` & `gemmi-0.6.6/tests/pdb1gdr.ent`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/r5wkdsf.ent` & `gemmi-0.6.6/tests/r5wkdsf.ent`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/rnase_frag.pdb` & `gemmi-0.6.6/tests/rnase_frag.pdb`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_align.py` & `gemmi-0.6.6/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_cif.py` & `gemmi-0.6.6/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_cif_json.py` & `gemmi-0.6.6/tests/test_cif_json.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_elem.py` & `gemmi-0.6.6/tests/test_elem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 import unittest
-from gemmi import Element, IT92_get_exact
+from gemmi import Element, IT92_get_exact, IT92_set_ignore_charge
 
 
 class TestElem(unittest.TestCase):
     def test_name(self):
         for name in ELEMENT_MASS:
             el = Element(name)
             self.assertEqual(el.name, name)
@@ -44,14 +44,15 @@
         self.assertIsNone(es.c4322)
         self.assertEqual(h.it92.get_coefs(), d.it92.get_coefs())
         self.assertEqual(h.c4322.get_coefs(), d.c4322.get_coefs())
         self.assertEqual(Element('X').it92.get_coefs(),
                          Element('O').it92.get_coefs())
         fe_coefs = fe.it92.get_coefs()
         fe0_coefs = IT92_get_exact(fe, 0).get_coefs()
+        IT92_set_ignore_charge(False)
         fe2_coefs = IT92_get_exact(fe, 2).get_coefs()
         self.assertIsNone(IT92_get_exact(fe, 4))
         self.assertEqual(fe_coefs, fe0_coefs)
         self.assertNotEqual(fe_coefs, fe2_coefs)
 
 
 ELEMENT_MASS = {
```

### Comparing `gemmi-0.6.5/tests/test_examples.py` & `gemmi-0.6.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_grid.py` & `gemmi-0.6.6/tests/test_grid.py`

 * *Files 20% similar despite different names*

```diff
@@ -81,14 +81,36 @@
         m.fill(2.0)
         m.spacegroup = gemmi.find_spacegroup_by_name('P 62 2 2')
         self.assertEqual(len(m.spacegroup.operations()), 12)
         m.set_value(1, 2, 3, 0.0)
         m.symmetrize_min()
         self.assertEqual(m.sum(), 2 * N * N * N - 2 * 12)
 
+    def test_grid_size(self):
+        # original cell from 4a0g, and a cell with a <-> b
+        cell = gemmi.UnitCell(79.442, 80.066, 136.939, 99.96, 107.12, 97.25)
+        cell2 = gemmi.UnitCell(80.066, 79.442, 136.939, 99.96, 107.12, 97.25)
+        self.assertAlmostEqual(cell.calculate_d([4, -32, 9]), 2.501956204)
+        dmin = 2.5
+        self.assertEqual(cell.get_hkl_limits(dmin), [31, 32, 54])
+        self.assertEqual(cell2.get_hkl_limits(dmin), [32, 31, 54])
+        # In prepare_asu_data(), max_k == (grid.nv - 1) / 2,
+        # so for k=31 we need nv>=63, for k=32 we need nv>=65.
+        # But when choosing grid size, we take the same n for almost equal
+        # lengths (a and b here). So both nu and nv are 72 instead of 64.
+        grid = gemmi.FloatGrid()
+        grid.spacegroup = gemmi.SpaceGroup('P 1')
+        grid.unit_cell = cell
+        grid.set_size_from_spacing(dmin / 2, gemmi.GridSizeRounding.Up)
+        self.assertTrue([grid.nu, grid.nv, grid.nw] == [72, 72, 120])
+        grid.unit_cell = cell2
+        grid.set_size_from_spacing(dmin / 2, gemmi.GridSizeRounding.Up)
+        self.assertTrue([grid.nu, grid.nv, grid.nw] == [72, 72, 120])
+
+
 class TestCcp4Map(unittest.TestCase):
     @unittest.skipIf(numpy is None, "NumPy not installed.")
     def test_567_map(self):
         # make a small, contrived map
         data = numpy.arange(5*6*7, dtype=numpy.float32).reshape((5,6,7))
         cell = gemmi.UnitCell(150, 132, 140, 90, 90, 90)
         m = gemmi.Ccp4Map()
```

### Comparing `gemmi-0.6.5/tests/test_hkl.py` & `gemmi-0.6.6/tests/test_hkl.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_misc.py` & `gemmi-0.6.6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_mol.py` & `gemmi-0.6.6/tests/test_mol.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
     def test_software_category(self):
         doc = gemmi.cif.read_file(full_path('3dg1_final.cif'))
         input_block = doc.sole_block()
         st = gemmi.make_structure_from_block(input_block)
         output_block = st.make_mmcif_document().sole_block()
         software = output_block.get_mmcif_category('_software')
         del software['date']
+        del software['description']
         assert software['version'][0] is False
         software['version'][0] = None
         self.assertEqual(input_block.get_mmcif_category('_software'), software)
 
     def test_5moo_header(self):
         st = gemmi.read_structure(full_path('5moo_header.pdb'))
         block = st.make_mmcif_document().sole_block()
```

### Comparing `gemmi-0.6.5/tests/test_monlib.py` & `gemmi-0.6.6/tests/test_monlib.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_neighbor.py` & `gemmi-0.6.6/tests/test_neighbor.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_prog.py` & `gemmi-0.6.6/tests/test_prog.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 ''')  # noqa: E501
 #RMSE=5.7890e-05  8.194e-05%  max|dF|=0.0001430  R=0.000%  <dPhi>=1.158e-05
 
     @unittest.skipIf(sys.platform == 'win32', 'with MSVC it differs slightly')
     def test_sfcalc_1pfe(self):
         self.do('''\
 $ gemmi sfcalc --dmin=9 --rate=4 --blur=70 --rcut=1e-7 --test -v tests/1pfe.cif.gz
-[...] 40 50
+[...] 41 51
  (2 1 5)	 251.29	 251.287 	214.22	214.220	d=10.02
  (2 1 6)	 300.96	 300.961 	 41.99	 41.989	d= 9.25
  (2 2 0)	 349.07	 349.072 	180.00	180.000	d= 9.84
  (2 2 1)	 202.08	 202.077 	270.00	270.000	d= 9.77
  (2 2 2)	 471.47	 471.469 	  0.00	  0.000	d= 9.56
  (2 2 3)	 913.55	 913.547 	 90.00	 90.000	d= 9.23
  (3 0 0)	 591.82	 591.825 	180.00	180.000	d=11.37
```

### Comparing `gemmi-0.6.5/tests/test_seq.py` & `gemmi-0.6.6/tests/test_seq.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_sf.py` & `gemmi-0.6.6/tests/test_sf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def test_unk_does_not_cause_segfault(self):
         st = gemmi.read_pdb_string(FRAGMENT_WITH_UNK)
         for calculator in [gemmi.DensityCalculatorX,
                            gemmi.DensityCalculatorE,
                            gemmi.DensityCalculatorN]:
             dencalc = calculator()
             dencalc.d_min = 2.1
-            dencalc.set_grid_cell_and_spacegroup(st)
+            dencalc.grid.setup_from(st)
             # we only check here that it doesn't crash
             dencalc.put_model_density_on_grid(st[0])
 
 class TestExpandingToP1(unittest.TestCase):
     def test_1gdr(self):
         st = gemmi.read_pdb(full_path('pdb1gdr.ent'), max_line_length=72)
         sg = st.find_spacegroup()
```

### Comparing `gemmi-0.6.5/tests/test_smallmol.py` & `gemmi-0.6.6/tests/test_smallmol.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_symmetry.py` & `gemmi-0.6.6/tests/test_symmetry.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,16 +42,72 @@
     "-X"    : [-D, 0, 0,  0],
     "-1/2+Y": [ 0, D, 0, -D//2],
     # we want to handle non-crystallographic translations
     "x+3"   : [ D, 0, 0,  D*3],
     "1+Y"   : [ 0, D, 0,  D],
     "-2+Y"  : [ 0, D, 0, -D*2],
     "-z-5/6": [ 0, 0,-D, -D*5//6],
+    # some CIF files from COD have decimal fractions
+    "0.5-x":  [-D, 0, 0,  D//2],
+    ".5+Y":   [ 0, D, 0, D//2],
+    "-Z+0.25": [ 0, 0, -D, D//4],
+    "x+0.6666666667": [ D, 0, 0, D*2//3],
+    "1.25000-y": [ 0, -D, 0, D*5//4],
 }
 
+# From PLATON manual (WinGX v1.80, Chapter 9.3 PLATON),
+# Table 7.1 Space group names known to the program
+PLATON_SPACE_GROUP_NAMES = """\
+P1 P-1 P2 P112 P21 P1121 C2 A2
+B112 PM P11M PC PA PN P11B CM
+AM B11M CC IC IA AA B11B P2/M
+P112/M P21/M P1121/M C2/M A2/M B112/M P2/C P2/A
+P112/B P21/C P21/A P2/N P1121/B P21/N P21/N11 C2/C
+A2/A C2/N I2/C I2/N I2/M I2/A B112/B P222
+P2221 P2212 P2122 P21212 P212121 C2221 B2212 C222
+F222 I222 I212121 PMM2 PMC21 PCC2 PMA2 PCA21
+PNC2 PMN21 PBA2 PNA21 P21NB PC21N PN21A PBN21
+P21CN PNN2 CMM2 CMC21 CCC2 AMM2 ABM2 AMA2
+ABA2 FMM2 FDD2 IMM2 IBA2 IMA2 PMMM PNNN
+PCCM PBAN PMMA PNNA PMNA PCCA PBAM PCCN
+PBCM PNNM PMMN PBCN PBCA PCAB PNMA PBNM
+PMCN PNAM PMNB PCMN CMCM CMCA CMMM CCCM
+CMMA CCCA FMMM FDDD IMMM IBAM IBCA IMMA
+P4 P41 P42 P43 I4 I41 P-4 I-4
+P4/M P42/M P4/N P42/N I4/M I41/A P422 P4212
+P4122 P41212 P4222 P42212 P4322 P43212 I422 I4122
+P4MM P4BM P42CM P42NM P4CC P4NC P42MC P42BC
+I4MM I4CM I41MD I41CD P-42M P-42C P-421M P-421C
+P-4M2 P-4C2 P-4B2 P-4N2 I-4M2 I-4C2 I-42M I-42D
+P4/MMM P4/MCC P4/NBM P4/NNC P4/MBM P4/MNC P4/NMM P4/NCC
+P42/MMC P42/MCM P42/NBC P42/NNM P42/MBC P42/MNM P42/NMC P42/NCM
+I4/MMM I4/MCM I41/AMD I41/ACD P3 P31 P32 R3
+R3R P-3 R-3 R-3R P312 P321 P3112 P3121
+P3212 P3221 R32 R32R P3M1 P31M P3C1 P31C
+R3M R3MR R3C R3CR P-31M P-31C P-3M1 P-3C1
+R-3M R-3MR R-3C R-3CR P6 P61 P65 P62
+P64 P63 P-6 P6/M P63/M P622 P6122 P6522
+P6222 P6422 P6322 P6MM P6CC P63CM P63MC P-6M2
+P-6C2 P-62M P-62C P6/MMM P6/MCC P63/MCM P63/MMC P23
+F23 I23 P213 I213 PM3 PM-3 PN3 PN-3
+FM3 FM-3 FD3 FD-3 IM3 IM-3 PA3 PA-3
+IA3 IA-3 P432 P4232 F432 F4132 I432 P4332
+P4132 I4132 P-43M F-43M I43M P-43N F-43C I-43D
+PM3M PM-3M PN3N PN-3N PM3N PM-3N PN3M PN-3M
+FM3M FM-3M FM3C FM-3C FD3M FD-3M FD3C FD-3C
+IM3M IM-3M IA3D IA-3D
+"""
+
+def simple_monoclinic_unique_axis(hm):
+    hm_split = hm.split()
+    if len(hm_split) == 4 and hm_split.count('1') == 2:
+        for i in [1,2,3]:
+            if hm_split[i] != '1':
+                return chr(ord('a') + i - 1)
+    return '\0'
 
 class TestSymmetry(unittest.TestCase):
     def test_parse_triplet_part(self):
         for single, row in CANONICAL_SINGLES.items():
             calculated = gemmi.parse_triplet_part(single)
             self.assertEqual(calculated, row)
         for single, row in OTHER_SINGLES.items():
@@ -200,43 +256,46 @@
                 c2p_sg = gemmi.Op(cctbx_sg.z2p_op().c().inverse().as_xyz())
                 self.assertEqual(sg.centred_to_primitive(), c2p_sg)
                 hand_sgtbx = cctbx_info.change_of_basis_op_to_other_hand()
                 self.assertEqual(sg.change_of_hand_op().triplet(),
                                  hand_sgtbx.as_xyz())
             ops = gemmi.get_spacegroup_reference_setting(sg.number).operations()
             ops.change_basis_forward(sg.basisop)
-            self.assertEqual(ops, sg.operations())
+            self.assertEqual(ops, sg.operations(), msg=sg.xhm())
+            self.assertEqual(sg.monoclinic_unique_axis(),
+                             simple_monoclinic_unique_axis(sg.hm))
         itb = gemmi.spacegroup_table_itb()
         if sgtbx:
             for s in sgtbx.space_group_symbol_iterator():
                 self.assertEqual(s.hall().strip(), next(itb).hall)
             with self.assertRaises(StopIteration):
                 next(itb)
 
     def test_enantiomorphic_pairs(self):
         counter = 0
         for sg in gemmi.spacegroup_table():
             coh = sg.change_of_hand_op()
             ops = sg.operations()
             ops.change_basis_forward(coh)
             other_hand = gemmi.find_spacegroup_by_ops(ops)
+            self.assertIsNotNone(other_hand, msg=f'{sg} {coh}')
             if sg.hall != other_hand.hall:
                 counter += 1
             elif sg != other_hand:
                 # duplicates
                 self.assertTrue(sg.number == 68 or sg.xhm() == 'A b a m')
         self.assertEqual(counter, 2 * 11)
 
     def test_symmorphic(self):
         for sg in gemmi.spacegroup_table():
             ops = sg.operations()
             symmor_ops = ops.derive_symmorphic()
             self.assertEqual(len(ops), len(symmor_ops))
             symmor = gemmi.find_spacegroup_by_ops(symmor_ops)
-            self.assertTrue(symmor is not None)
+            self.assertTrue(symmor is not None, msg=sg.xhm())
             self.assertTrue(symmor.is_symmorphic())
             if sg.is_symmorphic():
                 self.assertEqual(sg.number, symmor.number)
 
     def test_find_spacegroup(self):
         self.assertEqual(gemmi.SpaceGroup('P21212').hm, 'P 21 21 2')
         self.assertEqual(gemmi.find_spacegroup_by_name('P21').hm, 'P 1 21 1')
@@ -343,14 +402,17 @@
             self.assertAlmostEqual((shift - expected) % 360, 0)
 
     def test_reciprocal_asu_checker(self):
         sg = gemmi.SpaceGroup('I 1 2 1')
         checker = gemmi.ReciprocalAsu(sg)
         self.assertTrue(checker.is_in([-5, 5, 1]))
         self.assertFalse(checker.is_in([5, 5, -1]))
+        checker = gemmi.ReciprocalAsu(sg, tnt=True)
+        self.assertTrue(checker.is_in([5, 5, -1]))
+        self.assertFalse(checker.is_in([-5, 5, 1]))
 
     def test_reflection_properties(self):
         sg = gemmi.SpaceGroup('I 1 2 1')
         gops = sg.operations()
         self.assertTrue(gops.is_reflection_centric([3,0,3]))
         self.assertFalse(gops.is_reflection_centric([3,3,3]))
         self.assertEqual(gops.epsilon_factor([3,0,3]), 2)
@@ -366,9 +428,25 @@
     def test_pickling(self):
         sg = gemmi.SpaceGroup("P 31 2 1")
         pkl_string = pickle.dumps(sg, protocol=pickle.HIGHEST_PROTOCOL)
         result = pickle.loads(pkl_string)
         self.assertTrue(isinstance(result, gemmi.SpaceGroup))
         self.assertEqual(sg.xhm(), result.xhm())
 
+    # test space group names listed in PLATON docs
+    def test_platon_spacegroup_names(self):
+        if sgtbx is None:
+            return
+        for s in PLATON_SPACE_GROUP_NAMES.split():
+            # these names are not recognized neither by sgtbx nor by gemmi
+            if s in ['I2/N', 'I43M']:
+                continue
+            # By default, for groups such as Pnnn, gemmi uses the first
+            # settings (ext==1) and sgtbx the ones with ext==2.
+            # But with table_id='A', sgtbx also uses extension 1.
+            sgtbx_group = sgtbx.space_group_type(s, table_id='A')
+            sgtbx_ops = gemmi.symops_from_hall(sgtbx_group.hall_symbol())
+            gemmi_ops = gemmi.SpaceGroup(s).operations()
+            self.assertEqual(sgtbx_ops, gemmi_ops)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gemmi-0.6.5/tests/test_twin.py` & `gemmi-0.6.6/tests/test_twin.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/tests/test_unitcell.py` & `gemmi-0.6.6/tests/test_unitcell.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/doctest.h` & `gemmi-0.6.6/third_party/doctest.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 // ====================================================================== lgtm [cpp/missing-header-guard]
 // == DO NOT MODIFY THIS FILE BY HAND - IT IS AUTO GENERATED BY CMAKE! ==
 // ======================================================================
 //
 // doctest.h - the lightest feature-rich C++ single-header testing framework for unit tests and TDD
 //
-// Copyright (c) 2016-2019 Viktor Kirilov
+// Copyright (c) 2016-2023 Viktor Kirilov
 //
 // Distributed under the MIT Software License
 // See accompanying file LICENSE.txt or copy at
 // https://opensource.org/licenses/MIT
 //
 // The documentation can be found at the library's page:
-// https://github.com/onqtam/doctest/blob/master/doc/markdown/readme.md
+// https://github.com/doctest/doctest/blob/master/doc/markdown/readme.md
 //
 // =================================================================================================
 // =================================================================================================
 // =================================================================================================
 //
 // The library is heavily influenced by Catch - https://github.com/catchorg/Catch2
 // which uses the Boost Software License - Version 1.0
@@ -43,60 +43,80 @@
 #define DOCTEST_LIBRARY_INCLUDED
 
 // =================================================================================================
 // == VERSION ======================================================================================
 // =================================================================================================
 
 #define DOCTEST_VERSION_MAJOR 2
-#define DOCTEST_VERSION_MINOR 3
-#define DOCTEST_VERSION_PATCH 8
-#define DOCTEST_VERSION_STR "2.3.8"
+#define DOCTEST_VERSION_MINOR 4
+#define DOCTEST_VERSION_PATCH 11
+
+// util we need here
+#define DOCTEST_TOSTR_IMPL(x) #x
+#define DOCTEST_TOSTR(x) DOCTEST_TOSTR_IMPL(x)
+
+#define DOCTEST_VERSION_STR                                                                        \
+    DOCTEST_TOSTR(DOCTEST_VERSION_MAJOR) "."                                                       \
+    DOCTEST_TOSTR(DOCTEST_VERSION_MINOR) "."                                                       \
+    DOCTEST_TOSTR(DOCTEST_VERSION_PATCH)
 
 #define DOCTEST_VERSION                                                                            \
     (DOCTEST_VERSION_MAJOR * 10000 + DOCTEST_VERSION_MINOR * 100 + DOCTEST_VERSION_PATCH)
 
 // =================================================================================================
 // == COMPILER VERSION =============================================================================
 // =================================================================================================
 
 // ideas for the version stuff are taken from here: https://github.com/cxxstuff/cxx_detect
 
+#ifdef _MSC_VER
+#define DOCTEST_CPLUSPLUS _MSVC_LANG
+#else
+#define DOCTEST_CPLUSPLUS __cplusplus
+#endif
+
 #define DOCTEST_COMPILER(MAJOR, MINOR, PATCH) ((MAJOR)*10000000 + (MINOR)*100000 + (PATCH))
 
 // GCC/Clang and GCC/MSVC are mutually exclusive, but Clang/MSVC are not because of clang-cl...
 #if defined(_MSC_VER) && defined(_MSC_FULL_VER)
 #if _MSC_VER == _MSC_FULL_VER / 10000
 #define DOCTEST_MSVC DOCTEST_COMPILER(_MSC_VER / 100, _MSC_VER % 100, _MSC_FULL_VER % 10000)
 #else // MSVC
 #define DOCTEST_MSVC                                                                               \
     DOCTEST_COMPILER(_MSC_VER / 100, (_MSC_FULL_VER / 100000) % 100, _MSC_FULL_VER % 100000)
 #endif // MSVC
 #endif // MSVC
-#if defined(__clang__) && defined(__clang_minor__)
+#if defined(__clang__) && defined(__clang_minor__) && defined(__clang_patchlevel__)
 #define DOCTEST_CLANG DOCTEST_COMPILER(__clang_major__, __clang_minor__, __clang_patchlevel__)
 #elif defined(__GNUC__) && defined(__GNUC_MINOR__) && defined(__GNUC_PATCHLEVEL__) &&              \
         !defined(__INTEL_COMPILER)
 #define DOCTEST_GCC DOCTEST_COMPILER(__GNUC__, __GNUC_MINOR__, __GNUC_PATCHLEVEL__)
 #endif // GCC
+#if defined(__INTEL_COMPILER)
+#define DOCTEST_ICC DOCTEST_COMPILER(__INTEL_COMPILER / 100, __INTEL_COMPILER % 100, 0)
+#endif // ICC
 
 #ifndef DOCTEST_MSVC
 #define DOCTEST_MSVC 0
 #endif // DOCTEST_MSVC
 #ifndef DOCTEST_CLANG
 #define DOCTEST_CLANG 0
 #endif // DOCTEST_CLANG
 #ifndef DOCTEST_GCC
 #define DOCTEST_GCC 0
 #endif // DOCTEST_GCC
+#ifndef DOCTEST_ICC
+#define DOCTEST_ICC 0
+#endif // DOCTEST_ICC
 
 // =================================================================================================
 // == COMPILER WARNINGS HELPERS ====================================================================
 // =================================================================================================
 
-#if DOCTEST_CLANG
+#if DOCTEST_CLANG && !DOCTEST_ICC
 #define DOCTEST_PRAGMA_TO_STR(x) _Pragma(#x)
 #define DOCTEST_CLANG_SUPPRESS_WARNING_PUSH _Pragma("clang diagnostic push")
 #define DOCTEST_CLANG_SUPPRESS_WARNING(w) DOCTEST_PRAGMA_TO_STR(clang diagnostic ignored w)
 #define DOCTEST_CLANG_SUPPRESS_WARNING_POP _Pragma("clang diagnostic pop")
 #define DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH(w)                                                \
     DOCTEST_CLANG_SUPPRESS_WARNING_PUSH DOCTEST_CLANG_SUPPRESS_WARNING(w)
 #else // DOCTEST_CLANG
@@ -133,145 +153,166 @@
 #define DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(w)
 #endif // DOCTEST_MSVC
 
 // =================================================================================================
 // == COMPILER WARNINGS ============================================================================
 // =================================================================================================
 
+// both the header and the implementation suppress all of these,
+// so it only makes sense to aggregate them like so
+#define DOCTEST_SUPPRESS_COMMON_WARNINGS_PUSH                                                      \
+    DOCTEST_CLANG_SUPPRESS_WARNING_PUSH                                                            \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wunknown-pragmas")                                            \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wweak-vtables")                                               \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wpadded")                                                     \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-prototypes")                                         \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat")                                               \
+    DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat-pedantic")                                      \
+                                                                                                   \
+    DOCTEST_GCC_SUPPRESS_WARNING_PUSH                                                              \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wunknown-pragmas")                                              \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wpragmas")                                                      \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Weffc++")                                                       \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-overflow")                                              \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-aliasing")                                              \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wmissing-declarations")                                         \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wuseless-cast")                                                 \
+    DOCTEST_GCC_SUPPRESS_WARNING("-Wnoexcept")                                                     \
+                                                                                                   \
+    DOCTEST_MSVC_SUPPRESS_WARNING_PUSH                                                             \
+    /* these 4 also disabled globally via cmake: */                                                \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4514) /* unreferenced inline function has been removed */        \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4571) /* SEH related */                                          \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4710) /* function not inlined */                                 \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4711) /* function selected for inline expansion*/                \
+    /* common ones */                                                                              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4616) /* invalid compiler warning */                             \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4619) /* invalid compiler warning */                             \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4996) /* The compiler encountered a deprecated declaration */    \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4706) /* assignment within conditional expression */             \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4512) /* 'class' : assignment operator could not be generated */ \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4127) /* conditional expression is constant */                   \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4820) /* padding */                                              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4625) /* copy constructor was implicitly deleted */              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4626) /* assignment operator was implicitly deleted */           \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5027) /* move assignment operator implicitly deleted */          \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5026) /* move constructor was implicitly deleted */              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4640) /* construction of local static object not thread-safe */  \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5045) /* Spectre mitigation for memory load */                   \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5264) /* 'variable-name': 'const' variable is not used */        \
+    /* static analysis */                                                                          \
+    DOCTEST_MSVC_SUPPRESS_WARNING(26439) /* Function may not throw. Declare it 'noexcept' */       \
+    DOCTEST_MSVC_SUPPRESS_WARNING(26495) /* Always initialize a member variable */                 \
+    DOCTEST_MSVC_SUPPRESS_WARNING(26451) /* Arithmetic overflow ... */                             \
+    DOCTEST_MSVC_SUPPRESS_WARNING(26444) /* Avoid unnamed objects with custom ctor and dtor... */  \
+    DOCTEST_MSVC_SUPPRESS_WARNING(26812) /* Prefer 'enum class' over 'enum' */
+
+#define DOCTEST_SUPPRESS_COMMON_WARNINGS_POP                                                       \
+    DOCTEST_CLANG_SUPPRESS_WARNING_POP                                                             \
+    DOCTEST_GCC_SUPPRESS_WARNING_POP                                                               \
+    DOCTEST_MSVC_SUPPRESS_WARNING_POP
+
+DOCTEST_SUPPRESS_COMMON_WARNINGS_PUSH
+
 DOCTEST_CLANG_SUPPRESS_WARNING_PUSH
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wunknown-pragmas")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wnon-virtual-dtor")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wweak-vtables")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wpadded")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wdeprecated")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-prototypes")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wunused-local-typedef")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat-pedantic")
 
 DOCTEST_GCC_SUPPRESS_WARNING_PUSH
-DOCTEST_GCC_SUPPRESS_WARNING("-Wunknown-pragmas")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wpragmas")
-DOCTEST_GCC_SUPPRESS_WARNING("-Weffc++")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-overflow")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-aliasing")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wctor-dtor-privacy")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wmissing-declarations")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wnon-virtual-dtor")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wunused-local-typedefs")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wuseless-cast")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wnoexcept")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wsign-promo")
 
 DOCTEST_MSVC_SUPPRESS_WARNING_PUSH
-DOCTEST_MSVC_SUPPRESS_WARNING(4616) // invalid compiler warning
-DOCTEST_MSVC_SUPPRESS_WARNING(4619) // invalid compiler warning
-DOCTEST_MSVC_SUPPRESS_WARNING(4996) // The compiler encountered a deprecated declaration
-DOCTEST_MSVC_SUPPRESS_WARNING(4706) // assignment within conditional expression
-DOCTEST_MSVC_SUPPRESS_WARNING(4512) // 'class' : assignment operator could not be generated
-DOCTEST_MSVC_SUPPRESS_WARNING(4127) // conditional expression is constant
-DOCTEST_MSVC_SUPPRESS_WARNING(4820) // padding
-DOCTEST_MSVC_SUPPRESS_WARNING(4625) // copy constructor was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(4626) // assignment operator was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(5027) // move assignment operator was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(5026) // move constructor was implicitly defined as deleted
 DOCTEST_MSVC_SUPPRESS_WARNING(4623) // default constructor was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(4640) // construction of local static object is not thread-safe
-// static analysis
-DOCTEST_MSVC_SUPPRESS_WARNING(26439) // This kind of function may not throw. Declare it 'noexcept'
-DOCTEST_MSVC_SUPPRESS_WARNING(26495) // Always initialize a member variable
-DOCTEST_MSVC_SUPPRESS_WARNING(26451) // Arithmetic overflow ...
-DOCTEST_MSVC_SUPPRESS_WARNING(26444) // Avoid unnamed objects with custom construction and dtr...
-DOCTEST_MSVC_SUPPRESS_WARNING(26812) // Prefer 'enum class' over 'enum'
-
-// 4548 - expression before comma has no effect; expected expression with side - effect
-// 4265 - class has virtual functions, but destructor is not virtual
-// 4986 - exception specification does not match previous declaration
-// 4350 - behavior change: 'member1' called instead of 'member2'
-// 4668 - 'x' is not defined as a preprocessor macro, replacing with '0' for '#if/#elif'
-// 4365 - conversion from 'int' to 'unsigned long', signed/unsigned mismatch
-// 4774 - format string expected in argument 'x' is not a string literal
-// 4820 - padding in structs
-
-// only 4 should be disabled globally:
-// - 4514 # unreferenced inline function has been removed
-// - 4571 # SEH related
-// - 4710 # function not inlined
-// - 4711 # function 'x' selected for automatic inline expansion
 
 #define DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_BEGIN                                 \
     DOCTEST_MSVC_SUPPRESS_WARNING_PUSH                                                             \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4548)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4265)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4986)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4350)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4668)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4365)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4774)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4820)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4625)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4626)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(5027)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(5026)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(4623)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(5039)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(5045)                                                            \
-    DOCTEST_MSVC_SUPPRESS_WARNING(5105)
+    DOCTEST_MSVC_SUPPRESS_WARNING(4548) /* before comma no effect; expected side - effect */       \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4265) /* virtual functions, but destructor is not virtual */     \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4986) /* exception specification does not match previous */      \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4350) /* 'member1' called instead of 'member2' */                \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4668) /* not defined as a preprocessor macro */                  \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4365) /* signed/unsigned mismatch */                             \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4774) /* format string not a string literal */                   \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4820) /* padding */                                              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4625) /* copy constructor was implicitly deleted */              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4626) /* assignment operator was implicitly deleted */           \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5027) /* move assignment operator implicitly deleted */          \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5026) /* move constructor was implicitly deleted */              \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4623) /* default constructor was implicitly deleted */           \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5039) /* pointer to pot. throwing function passed to extern C */ \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5045) /* Spectre mitigation for memory load */                   \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5105) /* macro producing 'defined' has undefined behavior */     \
+    DOCTEST_MSVC_SUPPRESS_WARNING(4738) /* storing float result in memory, loss of performance */  \
+    DOCTEST_MSVC_SUPPRESS_WARNING(5262) /* implicit fall-through */
 
 #define DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_END DOCTEST_MSVC_SUPPRESS_WARNING_POP
 
 // =================================================================================================
 // == FEATURE DETECTION ============================================================================
 // =================================================================================================
 
 // general compiler feature support table: https://en.cppreference.com/w/cpp/compiler_support
 // MSVC C++11 feature support table: https://msdn.microsoft.com/en-us/library/hh567368.aspx
 // GCC C++11 feature support table: https://gcc.gnu.org/projects/cxx-status.html
 // MSVC version table:
 // https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B#Internal_version_numbering
+// MSVC++ 14.3 (17) _MSC_VER == 1930 (Visual Studio 2022)
 // MSVC++ 14.2 (16) _MSC_VER == 1920 (Visual Studio 2019)
 // MSVC++ 14.1 (15) _MSC_VER == 1910 (Visual Studio 2017)
 // MSVC++ 14.0      _MSC_VER == 1900 (Visual Studio 2015)
 // MSVC++ 12.0      _MSC_VER == 1800 (Visual Studio 2013)
 // MSVC++ 11.0      _MSC_VER == 1700 (Visual Studio 2012)
 // MSVC++ 10.0      _MSC_VER == 1600 (Visual Studio 2010)
 // MSVC++ 9.0       _MSC_VER == 1500 (Visual Studio 2008)
 // MSVC++ 8.0       _MSC_VER == 1400 (Visual Studio 2005)
 
+// Universal Windows Platform support
+#if defined(WINAPI_FAMILY) && (WINAPI_FAMILY == WINAPI_FAMILY_APP)
+#define DOCTEST_CONFIG_NO_WINDOWS_SEH
+#endif // WINAPI_FAMILY
 #if DOCTEST_MSVC && !defined(DOCTEST_CONFIG_WINDOWS_SEH)
 #define DOCTEST_CONFIG_WINDOWS_SEH
 #endif // MSVC
 #if defined(DOCTEST_CONFIG_NO_WINDOWS_SEH) && defined(DOCTEST_CONFIG_WINDOWS_SEH)
 #undef DOCTEST_CONFIG_WINDOWS_SEH
 #endif // DOCTEST_CONFIG_NO_WINDOWS_SEH
 
 #if !defined(_WIN32) && !defined(__QNX__) && !defined(DOCTEST_CONFIG_POSIX_SIGNALS) &&             \
-        !defined(__EMSCRIPTEN__)
+        !defined(__EMSCRIPTEN__) && !defined(__wasi__)
 #define DOCTEST_CONFIG_POSIX_SIGNALS
 #endif // _WIN32
 #if defined(DOCTEST_CONFIG_NO_POSIX_SIGNALS) && defined(DOCTEST_CONFIG_POSIX_SIGNALS)
 #undef DOCTEST_CONFIG_POSIX_SIGNALS
 #endif // DOCTEST_CONFIG_NO_POSIX_SIGNALS
 
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
-#if !defined(__cpp_exceptions) && !defined(__EXCEPTIONS) && !defined(_CPPUNWIND)
+#if !defined(__cpp_exceptions) && !defined(__EXCEPTIONS) && !defined(_CPPUNWIND)                   \
+        || defined(__wasi__)
 #define DOCTEST_CONFIG_NO_EXCEPTIONS
 #endif // no exceptions
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS
 
 #ifdef DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
 #define DOCTEST_CONFIG_NO_EXCEPTIONS
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
 
 #if defined(DOCTEST_CONFIG_NO_EXCEPTIONS) && !defined(DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS)
 #define DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS && !DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS
 
+// (local change) disable multi-threading, otherwise MinGW can't compile it
+#if 1
+//#ifdef __wasi__
+#define DOCTEST_CONFIG_NO_MULTITHREADING
+#endif
+
 #if defined(DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN) && !defined(DOCTEST_CONFIG_IMPLEMENT)
 #define DOCTEST_CONFIG_IMPLEMENT
 #endif // DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN
 
 #if defined(_WIN32) || defined(__CYGWIN__)
 #if DOCTEST_MSVC
 #define DOCTEST_SYMBOL_EXPORT __declspec(dllexport)
@@ -291,235 +332,366 @@
 #else // DOCTEST_CONFIG_IMPLEMENT
 #define DOCTEST_INTERFACE DOCTEST_SYMBOL_IMPORT
 #endif // DOCTEST_CONFIG_IMPLEMENT
 #else  // DOCTEST_CONFIG_IMPLEMENTATION_IN_DLL
 #define DOCTEST_INTERFACE
 #endif // DOCTEST_CONFIG_IMPLEMENTATION_IN_DLL
 
+// needed for extern template instantiations
+// see https://github.com/fmtlib/fmt/issues/2228
+#if DOCTEST_MSVC
+#define DOCTEST_INTERFACE_DECL
+#define DOCTEST_INTERFACE_DEF DOCTEST_INTERFACE
+#else // DOCTEST_MSVC
+#define DOCTEST_INTERFACE_DECL DOCTEST_INTERFACE
+#define DOCTEST_INTERFACE_DEF
+#endif // DOCTEST_MSVC
+
 #define DOCTEST_EMPTY
 
 #if DOCTEST_MSVC
 #define DOCTEST_NOINLINE __declspec(noinline)
 #define DOCTEST_UNUSED
 #define DOCTEST_ALIGNMENT(x)
-#else // MSVC
+#elif DOCTEST_CLANG && DOCTEST_CLANG < DOCTEST_COMPILER(3, 5, 0)
+#define DOCTEST_NOINLINE
+#define DOCTEST_UNUSED
+#define DOCTEST_ALIGNMENT(x)
+#else
 #define DOCTEST_NOINLINE __attribute__((noinline))
 #define DOCTEST_UNUSED __attribute__((unused))
 #define DOCTEST_ALIGNMENT(x) __attribute__((aligned(x)))
-#endif // MSVC
+#endif
+
+#ifdef DOCTEST_CONFIG_NO_CONTRADICTING_INLINE
+#define DOCTEST_INLINE_NOINLINE inline
+#else
+#define DOCTEST_INLINE_NOINLINE inline DOCTEST_NOINLINE
+#endif
 
 #ifndef DOCTEST_NORETURN
+#if DOCTEST_MSVC && (DOCTEST_MSVC < DOCTEST_COMPILER(19, 0, 0))
+#define DOCTEST_NORETURN
+#else // DOCTEST_MSVC
 #define DOCTEST_NORETURN [[noreturn]]
+#endif // DOCTEST_MSVC
 #endif // DOCTEST_NORETURN
 
 #ifndef DOCTEST_NOEXCEPT
+#if DOCTEST_MSVC && (DOCTEST_MSVC < DOCTEST_COMPILER(19, 0, 0))
+#define DOCTEST_NOEXCEPT
+#else // DOCTEST_MSVC
 #define DOCTEST_NOEXCEPT noexcept
+#endif // DOCTEST_MSVC
 #endif // DOCTEST_NOEXCEPT
 
+#ifndef DOCTEST_CONSTEXPR
+#if DOCTEST_MSVC && (DOCTEST_MSVC < DOCTEST_COMPILER(19, 0, 0))
+#define DOCTEST_CONSTEXPR const
+#define DOCTEST_CONSTEXPR_FUNC inline
+#else // DOCTEST_MSVC
+#define DOCTEST_CONSTEXPR constexpr
+#define DOCTEST_CONSTEXPR_FUNC constexpr
+#endif // DOCTEST_MSVC
+#endif // DOCTEST_CONSTEXPR
+
+#ifndef DOCTEST_NO_SANITIZE_INTEGER
+#if DOCTEST_CLANG >= DOCTEST_COMPILER(3, 7, 0)
+#define DOCTEST_NO_SANITIZE_INTEGER __attribute__((no_sanitize("integer")))
+#else
+#define DOCTEST_NO_SANITIZE_INTEGER
+#endif
+#endif // DOCTEST_NO_SANITIZE_INTEGER
+
 // =================================================================================================
 // == FEATURE DETECTION END ========================================================================
 // =================================================================================================
 
+#define DOCTEST_DECLARE_INTERFACE(name)                                                            \
+    virtual ~name();                                                                               \
+    name() = default;                                                                              \
+    name(const name&) = delete;                                                                    \
+    name(name&&) = delete;                                                                         \
+    name& operator=(const name&) = delete;                                                         \
+    name& operator=(name&&) = delete;
+
+#define DOCTEST_DEFINE_INTERFACE(name)                                                             \
+    name::~name() = default;
+
 // internal macros for string concatenation and anonymous variable name generation
 #define DOCTEST_CAT_IMPL(s1, s2) s1##s2
 #define DOCTEST_CAT(s1, s2) DOCTEST_CAT_IMPL(s1, s2)
 #ifdef __COUNTER__ // not standard and may be missing for some compilers
 #define DOCTEST_ANONYMOUS(x) DOCTEST_CAT(x, __COUNTER__)
 #else // __COUNTER__
 #define DOCTEST_ANONYMOUS(x) DOCTEST_CAT(x, __LINE__)
 #endif // __COUNTER__
 
-#define DOCTEST_TOSTR(x) #x
-
 #ifndef DOCTEST_CONFIG_ASSERTION_PARAMETERS_BY_VALUE
 #define DOCTEST_REF_WRAP(x) x&
 #else // DOCTEST_CONFIG_ASSERTION_PARAMETERS_BY_VALUE
 #define DOCTEST_REF_WRAP(x) x
 #endif // DOCTEST_CONFIG_ASSERTION_PARAMETERS_BY_VALUE
 
 // not using __APPLE__ because... this is how Catch does it
 #ifdef __MAC_OS_X_VERSION_MIN_REQUIRED
 #define DOCTEST_PLATFORM_MAC
 #elif defined(__IPHONE_OS_VERSION_MIN_REQUIRED)
 #define DOCTEST_PLATFORM_IPHONE
 #elif defined(_WIN32)
 #define DOCTEST_PLATFORM_WINDOWS
+#elif defined(__wasi__)
+#define DOCTEST_PLATFORM_WASI
 #else // DOCTEST_PLATFORM
 #define DOCTEST_PLATFORM_LINUX
 #endif // DOCTEST_PLATFORM
 
-#define DOCTEST_GLOBAL_NO_WARNINGS(var)                                                            \
-    DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wglobal-constructors")                              \
-    DOCTEST_CLANG_SUPPRESS_WARNING("-Wunused-variable")                                            \
-    static int var DOCTEST_UNUSED // NOLINT(fuchsia-statically-constructed-objects,cert-err58-cpp)
-#define DOCTEST_GLOBAL_NO_WARNINGS_END() DOCTEST_CLANG_SUPPRESS_WARNING_POP
+namespace doctest { namespace detail {
+    static DOCTEST_CONSTEXPR int consume(const int*, int) noexcept { return 0; }
+}}
+
+#define DOCTEST_GLOBAL_NO_WARNINGS(var, ...)                                                         \
+    DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wglobal-constructors")                                \
+    static const int var = doctest::detail::consume(&var, __VA_ARGS__);                              \
+    DOCTEST_CLANG_SUPPRESS_WARNING_POP
 
 #ifndef DOCTEST_BREAK_INTO_DEBUGGER
 // should probably take a look at https://github.com/scottt/debugbreak
-#ifdef DOCTEST_PLATFORM_MAC
-#define DOCTEST_BREAK_INTO_DEBUGGER() __asm__("int $3\n" : :)
+#ifdef DOCTEST_PLATFORM_LINUX
+#if defined(__GNUC__) && (defined(__i386) || defined(__x86_64))
+// Break at the location of the failing check if possible
+#define DOCTEST_BREAK_INTO_DEBUGGER() __asm__("int $3\n" : :) // NOLINT(hicpp-no-assembler)
+#else
+#include <signal.h>
+#define DOCTEST_BREAK_INTO_DEBUGGER() raise(SIGTRAP)
+#endif
+#elif defined(DOCTEST_PLATFORM_MAC)
+#if defined(__x86_64) || defined(__x86_64__) || defined(__amd64__) || defined(__i386)
+#define DOCTEST_BREAK_INTO_DEBUGGER() __asm__("int $3\n" : :) // NOLINT(hicpp-no-assembler)
+#elif defined(__ppc__) || defined(__ppc64__)
+// https://www.cocoawithlove.com/2008/03/break-into-debugger.html
+#define DOCTEST_BREAK_INTO_DEBUGGER() __asm__("li r0, 20\nsc\nnop\nli r0, 37\nli r4, 2\nsc\nnop\n": : : "memory","r0","r3","r4") // NOLINT(hicpp-no-assembler)
+#else
+#define DOCTEST_BREAK_INTO_DEBUGGER() __asm__("brk #0"); // NOLINT(hicpp-no-assembler)
+#endif
 #elif DOCTEST_MSVC
 #define DOCTEST_BREAK_INTO_DEBUGGER() __debugbreak()
 #elif defined(__MINGW32__)
 DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wredundant-decls")
 extern "C" __declspec(dllimport) void __stdcall DebugBreak();
 DOCTEST_GCC_SUPPRESS_WARNING_POP
 #define DOCTEST_BREAK_INTO_DEBUGGER() ::DebugBreak()
 #else // linux
-#define DOCTEST_BREAK_INTO_DEBUGGER() ((void)0)
+#define DOCTEST_BREAK_INTO_DEBUGGER() (static_cast<void>(0))
 #endif // linux
 #endif // DOCTEST_BREAK_INTO_DEBUGGER
 
 // this is kept here for backwards compatibility since the config option was changed
 #ifdef DOCTEST_CONFIG_USE_IOSFWD
+#ifndef DOCTEST_CONFIG_USE_STD_HEADERS
 #define DOCTEST_CONFIG_USE_STD_HEADERS
+#endif
 #endif // DOCTEST_CONFIG_USE_IOSFWD
 
-#ifdef DOCTEST_CONFIG_USE_STD_HEADERS
-#include <iosfwd>
-#include <cstddef>
-#include <ostream>
-#else // DOCTEST_CONFIG_USE_STD_HEADERS
-
+// for clang - always include ciso646 (which drags some std stuff) because
+// we want to check if we are using libc++ with the _LIBCPP_VERSION macro in
+// which case we don't want to forward declare stuff from std - for reference:
+// https://github.com/doctest/doctest/issues/126
+// https://github.com/doctest/doctest/issues/356
 #if DOCTEST_CLANG
-// to detect if libc++ is being used with clang (the _LIBCPP_VERSION identifier)
 #include <ciso646>
 #endif // clang
 
 #ifdef _LIBCPP_VERSION
-#define DOCTEST_STD_NAMESPACE_BEGIN _LIBCPP_BEGIN_NAMESPACE_STD
-#define DOCTEST_STD_NAMESPACE_END _LIBCPP_END_NAMESPACE_STD
-#else // _LIBCPP_VERSION
-#define DOCTEST_STD_NAMESPACE_BEGIN namespace std {
-#define DOCTEST_STD_NAMESPACE_END }
+#ifndef DOCTEST_CONFIG_USE_STD_HEADERS
+#define DOCTEST_CONFIG_USE_STD_HEADERS
+#endif
 #endif // _LIBCPP_VERSION
 
+#ifdef DOCTEST_CONFIG_USE_STD_HEADERS
+#ifndef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
+#define DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
+#endif // DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
+DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_BEGIN
+#include <cstddef>
+#include <ostream>
+#include <istream>
+DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_END
+#else // DOCTEST_CONFIG_USE_STD_HEADERS
+
 // Forward declaring 'X' in namespace std is not permitted by the C++ Standard.
 DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4643)
 
-DOCTEST_STD_NAMESPACE_BEGIN // NOLINT (cert-dcl58-cpp)
-typedef decltype(nullptr) nullptr_t;
+namespace std { // NOLINT(cert-dcl58-cpp)
+typedef decltype(nullptr) nullptr_t; // NOLINT(modernize-use-using)
+typedef decltype(sizeof(void*)) size_t; // NOLINT(modernize-use-using)
 template <class charT>
 struct char_traits;
 template <>
 struct char_traits<char>;
 template <class charT, class traits>
-class basic_ostream;
-typedef basic_ostream<char, char_traits<char>> ostream;
+class basic_ostream; // NOLINT(fuchsia-virtual-inheritance)
+typedef basic_ostream<char, char_traits<char>> ostream; // NOLINT(modernize-use-using)
+template<class traits>
+// NOLINTNEXTLINE
+basic_ostream<char, traits>& operator<<(basic_ostream<char, traits>&, const char*);
+template <class charT, class traits>
+class basic_istream;
+typedef basic_istream<char, char_traits<char>> istream; // NOLINT(modernize-use-using)
 template <class... Types>
 class tuple;
 #if DOCTEST_MSVC >= DOCTEST_COMPILER(19, 20, 0)
-// see this issue on why this is needed: https://github.com/onqtam/doctest/issues/183
-template <class _Ty>
+// see this issue on why this is needed: https://github.com/doctest/doctest/issues/183
+template <class Ty>
 class allocator;
-template <class _Elem, class _Traits, class _Alloc>
+template <class Elem, class Traits, class Alloc>
 class basic_string;
 using string = basic_string<char, char_traits<char>, allocator<char>>;
 #endif // VS 2019
-DOCTEST_STD_NAMESPACE_END
+} // namespace std
 
 DOCTEST_MSVC_SUPPRESS_WARNING_POP
 
 #endif // DOCTEST_CONFIG_USE_STD_HEADERS
 
 #ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 #include <type_traits>
 #endif // DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 
 namespace doctest {
 
+using std::size_t;
+
 DOCTEST_INTERFACE extern bool is_running_in_test;
 
+#ifndef DOCTEST_CONFIG_STRING_SIZE_TYPE
+#define DOCTEST_CONFIG_STRING_SIZE_TYPE unsigned
+#endif
+
 // A 24 byte string class (can be as small as 17 for x64 and 13 for x86) that can hold strings with length
 // of up to 23 chars on the stack before going on the heap - the last byte of the buffer is used for:
 // - "is small" bit - the highest bit - if "0" then it is small - otherwise its "1" (128)
 // - if small - capacity left before going on the heap - using the lowest 5 bits
 // - if small - 2 bits are left unused - the second and third highest ones
 // - if small - acts as a null terminator if strlen() is 23 (24 including the null terminator)
 //              and the "is small" bit remains "0" ("as well as the capacity left") so its OK
 // Idea taken from this lecture about the string implementation of facebook/folly - fbstring
 // https://www.youtube.com/watch?v=kPR8h4-qZdk
 // TODO:
 // - optimizations - like not deleting memory unnecessarily in operator= and etc.
 // - resize/reserve/clear
-// - substr
 // - replace
 // - back/front
 // - iterator stuff
 // - find & friends
 // - push_back/pop_back
 // - assign/insert/erase
 // - relational operators as free functions - taking const char* as one of the params
 class DOCTEST_INTERFACE String
 {
-    static const unsigned len  = 24;      //!OCLINT avoid private static members
-    static const unsigned last = len - 1; //!OCLINT avoid private static members
+public:
+    using size_type = DOCTEST_CONFIG_STRING_SIZE_TYPE;
+
+private:
+    static DOCTEST_CONSTEXPR size_type len  = 24;      //!OCLINT avoid private static members
+    static DOCTEST_CONSTEXPR size_type last = len - 1; //!OCLINT avoid private static members
 
     struct view // len should be more than sizeof(view) - because of the final byte for flags
     {
         char*    ptr;
-        unsigned size;
-        unsigned capacity;
+        size_type size;
+        size_type capacity;
     };
 
     union
     {
-        char buf[len];
+        char buf[len]; // NOLINT(*-avoid-c-arrays)
         view data;
     };
 
-    bool isOnStack() const { return (buf[last] & 128) == 0; }
-    void setOnHeap();
-    void setLast(unsigned in = last);
+    char* allocate(size_type sz);
+
+    bool isOnStack() const noexcept { return (buf[last] & 128) == 0; }
+    void setOnHeap() noexcept;
+    void setLast(size_type in = last) noexcept;
+    void setSize(size_type sz) noexcept;
 
     void copy(const String& other);
 
 public:
-    String();
+    static DOCTEST_CONSTEXPR size_type npos = static_cast<size_type>(-1);
+
+    String() noexcept;
     ~String();
 
     // cppcheck-suppress noExplicitConstructor
     String(const char* in);
-    String(const char* in, unsigned in_size);
+    String(const char* in, size_type in_size);
+
+    String(std::istream& in, size_type in_size);
 
     String(const String& other);
     String& operator=(const String& other);
 
     String& operator+=(const String& other);
-    String  operator+(const String& other) const;
 
-    String(String&& other);
-    String& operator=(String&& other);
+    String(String&& other) noexcept;
+    String& operator=(String&& other) noexcept;
 
-    char  operator[](unsigned i) const;
-    char& operator[](unsigned i);
+    char  operator[](size_type i) const;
+    char& operator[](size_type i);
 
     // the only functions I'm willing to leave in the interface - available for inlining
     const char* c_str() const { return const_cast<String*>(this)->c_str(); } // NOLINT
     char*       c_str() {
-        if(isOnStack())
+        if (isOnStack()) {
             return reinterpret_cast<char*>(buf);
+        }
         return data.ptr;
     }
 
-    unsigned size() const;
-    unsigned capacity() const;
+    size_type size() const;
+    size_type capacity() const;
+
+    String substr(size_type pos, size_type cnt = npos) &&;
+    String substr(size_type pos, size_type cnt = npos) const &;
+
+    size_type find(char ch, size_type pos = 0) const;
+    size_type rfind(char ch, size_type pos = npos) const;
 
     int compare(const char* other, bool no_case = false) const;
     int compare(const String& other, bool no_case = false) const;
+
+friend DOCTEST_INTERFACE std::ostream& operator<<(std::ostream& s, const String& in);
 };
 
+DOCTEST_INTERFACE String operator+(const String& lhs, const String& rhs);
+
 DOCTEST_INTERFACE bool operator==(const String& lhs, const String& rhs);
 DOCTEST_INTERFACE bool operator!=(const String& lhs, const String& rhs);
 DOCTEST_INTERFACE bool operator<(const String& lhs, const String& rhs);
 DOCTEST_INTERFACE bool operator>(const String& lhs, const String& rhs);
 DOCTEST_INTERFACE bool operator<=(const String& lhs, const String& rhs);
 DOCTEST_INTERFACE bool operator>=(const String& lhs, const String& rhs);
 
-DOCTEST_INTERFACE std::ostream& operator<<(std::ostream& s, const String& in);
+class DOCTEST_INTERFACE Contains {
+public:
+    explicit Contains(const String& string);
+
+    bool checkWith(const String& other) const;
+
+    String string;
+};
+
+DOCTEST_INTERFACE String toString(const Contains& in);
+
+DOCTEST_INTERFACE bool operator==(const String& lhs, const Contains& rhs);
+DOCTEST_INTERFACE bool operator==(const Contains& lhs, const String& rhs);
+DOCTEST_INTERFACE bool operator!=(const String& lhs, const Contains& rhs);
+DOCTEST_INTERFACE bool operator!=(const Contains& lhs, const String& rhs);
 
 namespace Color {
     enum Enum
     {
         None = 0,
         White,
         Red,
@@ -584,15 +756,15 @@
         DT_WARN_THROWS_AS    = is_throws_as | is_warn,
         DT_CHECK_THROWS_AS   = is_throws_as | is_check,
         DT_REQUIRE_THROWS_AS = is_throws_as | is_require,
 
         DT_WARN_THROWS_WITH    = is_throws_with | is_warn,
         DT_CHECK_THROWS_WITH   = is_throws_with | is_check,
         DT_REQUIRE_THROWS_WITH = is_throws_with | is_require,
-        
+
         DT_WARN_THROWS_WITH_AS    = is_throws_with | is_throws_as | is_warn,
         DT_CHECK_THROWS_WITH_AS   = is_throws_with | is_throws_as | is_check,
         DT_REQUIRE_THROWS_WITH_AS = is_throws_with | is_throws_as | is_require,
 
         DT_WARN_NOTHROW    = is_nothrow | is_warn,
         DT_CHECK_NOTHROW   = is_nothrow | is_check,
         DT_REQUIRE_NOTHROW = is_nothrow | is_require,
@@ -633,20 +805,22 @@
 
 DOCTEST_INTERFACE const char* assertString(assertType::Enum at);
 DOCTEST_INTERFACE const char* failureString(assertType::Enum at);
 DOCTEST_INTERFACE const char* skipPathFromFilename(const char* file);
 
 struct DOCTEST_INTERFACE TestCaseData
 {
-    String      m_file;       // the file in which the test was registered
+    String      m_file;       // the file in which the test was registered (using String - see #350)
     unsigned    m_line;       // the line where the test was registered
     const char* m_name;       // name of the test case
     const char* m_test_suite; // the test suite in which the test was added
     const char* m_description;
     bool        m_skip;
+    bool        m_no_breaks;
+    bool        m_no_output;
     bool        m_may_fail;
     bool        m_should_fail;
     int         m_expected_failures;
     double      m_timeout;
 };
 
 struct DOCTEST_INTERFACE AssertData
@@ -663,17 +837,35 @@
     bool   m_threw;
     String m_exception;
 
     // for normal asserts
     String m_decomp;
 
     // for specific exception-related asserts
-    bool        m_threw_as;
-    const char* m_exception_type;
-    const char* m_exception_string;
+    bool           m_threw_as;
+    const char*    m_exception_type;
+
+    class DOCTEST_INTERFACE StringContains {
+        private:
+            Contains content;
+            bool isContains;
+
+        public:
+            StringContains(const String& str) : content(str), isContains(false) { }
+            StringContains(Contains cntn) : content(static_cast<Contains&&>(cntn)), isContains(true) { }
+
+            bool check(const String& str) { return isContains ? (content == str) : (content.string == str); }
+
+            operator const String&() const { return content.string; }
+
+            const char* c_str() const { return content.string.c_str(); }
+    } m_exception_string;
+
+    AssertData(assertType::Enum at, const char* file, int line, const char* expr,
+        const char* exception_type, const StringContains& exception_string);
 };
 
 struct DOCTEST_INTERFACE MessageData
 {
     String           m_string;
     const char*      m_file;
     int              m_line;
@@ -682,29 +874,34 @@
 
 struct DOCTEST_INTERFACE SubcaseSignature
 {
     String      m_name;
     const char* m_file;
     int         m_line;
 
+    bool operator==(const SubcaseSignature& other) const;
     bool operator<(const SubcaseSignature& other) const;
 };
 
 struct DOCTEST_INTERFACE IContextScope
 {
-    IContextScope();
-    virtual ~IContextScope();
+    DOCTEST_DECLARE_INTERFACE(IContextScope)
     virtual void stringify(std::ostream*) const = 0;
 };
 
+namespace detail {
+    struct DOCTEST_INTERFACE TestCase;
+} // namespace detail
+
 struct ContextOptions //!OCLINT too many fields
 {
-    std::ostream* cout;        // stdout stream - std::cout by default
-    std::ostream* cerr;        // stderr stream - std::cerr by default
-    String        binary_name; // the test binary name
+    std::ostream* cout = nullptr; // stdout stream
+    String        binary_name;    // the test binary name
+
+    const detail::TestCase* currentTest = nullptr;
 
     // == parameters from the command line
     String   out;       // output filename
     String   order_by;  // how tests should be ordered
     unsigned rand_seed; // the seed for rand ordering
 
     unsigned first; // the first (matching) test to be executed
@@ -713,215 +910,339 @@
     int abort_after;           // stop tests after this many failed assertions
     int subcase_filter_levels; // apply the subcase filters for the first N levels
 
     bool success;              // include successful assertions in output
     bool case_sensitive;       // if filtering should be case sensitive
     bool exit;                 // if the program should be exited after the tests are ran/whatever
     bool duration;             // print the time duration of each test case
+    bool minimal;              // minimal console output (only test failures)
+    bool quiet;                // no console output
     bool no_throw;             // to skip exceptions-related assertion macros
     bool no_exitcode;          // if the framework should return 0 as the exitcode
     bool no_run;               // to not run the tests at all (can be done with an "*" exclude)
+    bool no_intro;             // to not print the intro of the framework
     bool no_version;           // to not print the version of the framework
     bool no_colors;            // if output to the console should be colorized
     bool force_colors;         // forces the use of colors even when a tty cannot be detected
     bool no_breaks;            // to not break into the debugger
     bool no_skip;              // don't skip test cases which are marked to be skipped
     bool gnu_file_line;        // if line numbers should be surrounded with :x: and not (x):
     bool no_path_in_filenames; // if the path to files should be removed from the output
     bool no_line_numbers;      // if source code line numbers should be omitted from the output
+    bool no_debug_output;      // no output in the debug console when a debugger is attached
     bool no_skipped_summary;   // don't print "skipped" in the summary !!! UNDOCUMENTED !!!
+    bool no_time_in_output;    // omit any time/timestamps from output !!! UNDOCUMENTED !!!
 
     bool help;             // to print the help
     bool version;          // to print the version
     bool count;            // if only the count of matching tests is to be retrieved
     bool list_test_cases;  // to list all tests matching the filters
     bool list_test_suites; // to list all suites matching the filters
     bool list_reporters;   // lists all registered reporters
 };
 
 namespace detail {
-#if defined(DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING) || defined(DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS)
-    template <bool CONDITION, typename TYPE = void>
-    struct enable_if
-    {};
-
-    template <typename TYPE>
-    struct enable_if<true, TYPE>
-    { typedef TYPE type; };
-#endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING) || DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
+    namespace types {
+#ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
+        using namespace std;
+#else
+        template <bool COND, typename T = void>
+        struct enable_if { };
 
-    // clang-format off
-    template<class T> struct remove_reference      { typedef T type; };
-    template<class T> struct remove_reference<T&>  { typedef T type; };
-    template<class T> struct remove_reference<T&&> { typedef T type; };
+        template <typename T>
+        struct enable_if<true, T> { using type = T; };
 
-    template<class T> struct remove_const          { typedef T type; };
-    template<class T> struct remove_const<const T> { typedef T type; };
-    // clang-format on
+        struct true_type { static DOCTEST_CONSTEXPR bool value = true; };
+        struct false_type { static DOCTEST_CONSTEXPR bool value = false; };
+
+        template <typename T> struct remove_reference { using type = T; };
+        template <typename T> struct remove_reference<T&> { using type = T; };
+        template <typename T> struct remove_reference<T&&> { using type = T; };
+
+        template <typename T> struct is_rvalue_reference : false_type { };
+        template <typename T> struct is_rvalue_reference<T&&> : true_type { };
+
+        template<typename T> struct remove_const { using type = T; };
+        template <typename T> struct remove_const<const T> { using type = T; };
+
+        // Compiler intrinsics
+        template <typename T> struct is_enum { static DOCTEST_CONSTEXPR bool value = __is_enum(T); };
+        template <typename T> struct underlying_type { using type = __underlying_type(T); };
 
+        template <typename T> struct is_pointer : false_type { };
+        template <typename T> struct is_pointer<T*> : true_type { };
+
+        template <typename T> struct is_array : false_type { };
+        // NOLINTNEXTLINE(*-avoid-c-arrays)
+        template <typename T, size_t SIZE> struct is_array<T[SIZE]> : true_type { };
+#endif
+    }
+
+    // <utility>
     template <typename T>
-    struct deferred_false
-    // cppcheck-suppress unusedStructMember
-    { static const bool value = false; };
-
-    namespace has_insertion_operator_impl {
-        typedef char no;
-        typedef char yes[2];
+    T&& declval();
 
-        struct any_t
-        {
-            template <typename T>
-            // cppcheck-suppress noExplicitConstructor
-            any_t(const DOCTEST_REF_WRAP(T));
-        };
+    template <class T>
+    DOCTEST_CONSTEXPR_FUNC T&& forward(typename types::remove_reference<T>::type& t) DOCTEST_NOEXCEPT {
+        return static_cast<T&&>(t);
+    }
 
-        yes& testStreamable(std::ostream&);
-        no   testStreamable(no);
+    template <class T>
+    DOCTEST_CONSTEXPR_FUNC T&& forward(typename types::remove_reference<T>::type&& t) DOCTEST_NOEXCEPT {
+        return static_cast<T&&>(t);
+    }
 
-        no operator<<(const std::ostream&, const any_t&);
+    template <typename T>
+    struct deferred_false : types::false_type { };
 
-        template <typename T>
-        struct has_insertion_operator
-        {
-            static std::ostream& s;
-            static const DOCTEST_REF_WRAP(T) t;
-            static const bool value = sizeof(decltype(testStreamable(s << t))) == sizeof(yes);
-        };
-    } // namespace has_insertion_operator_impl
+// MSVS 2015 :(
+#if !DOCTEST_CLANG && defined(_MSC_VER) && _MSC_VER <= 1900
+    template <typename T, typename = void>
+    struct has_global_insertion_operator : types::false_type { };
+
+    template <typename T>
+    struct has_global_insertion_operator<T, decltype(::operator<<(declval<std::ostream&>(), declval<const T&>()), void())> : types::true_type { };
+
+    template <typename T, typename = void>
+    struct has_insertion_operator { static DOCTEST_CONSTEXPR bool value = has_global_insertion_operator<T>::value; };
+
+    template <typename T, bool global>
+    struct insert_hack;
 
     template <typename T>
-    struct has_insertion_operator : has_insertion_operator_impl::has_insertion_operator<T>
-    {};
+    struct insert_hack<T, true> {
+        static void insert(std::ostream& os, const T& t) { ::operator<<(os, t); }
+    };
 
-    DOCTEST_INTERFACE void my_memcpy(void* dest, const void* src, unsigned num);
+    template <typename T>
+    struct insert_hack<T, false> {
+        static void insert(std::ostream& os, const T& t) { operator<<(os, t); }
+    };
 
-    DOCTEST_INTERFACE std::ostream* getTlsOss(); // returns a thread-local ostringstream
-    DOCTEST_INTERFACE String getTlsOssResult();
+    template <typename T>
+    using insert_hack_t = insert_hack<T, has_global_insertion_operator<T>::value>;
+#else
+    template <typename T, typename = void>
+    struct has_insertion_operator : types::false_type { };
+#endif
+
+    template <typename T>
+    struct has_insertion_operator<T, decltype(operator<<(declval<std::ostream&>(), declval<const T&>()), void())> : types::true_type { };
+
+    template <typename T>
+    struct should_stringify_as_underlying_type {
+        static DOCTEST_CONSTEXPR bool value = detail::types::is_enum<T>::value && !doctest::detail::has_insertion_operator<T>::value;
+    };
+
+    DOCTEST_INTERFACE std::ostream* tlssPush();
+    DOCTEST_INTERFACE String tlssPop();
 
     template <bool C>
-    struct StringMakerBase
-    {
+    struct StringMakerBase {
         template <typename T>
         static String convert(const DOCTEST_REF_WRAP(T)) {
+#ifdef DOCTEST_CONFIG_REQUIRE_STRINGIFICATION_FOR_ALL_USED_TYPES
+            static_assert(deferred_false<T>::value, "No stringification detected for type T. See string conversion manual");
+#endif
             return "{?}";
         }
     };
 
-    template <>
-    struct StringMakerBase<true>
-    {
-        template <typename T>
-        static String convert(const DOCTEST_REF_WRAP(T) in) {
-            *getTlsOss() << in;
-            return getTlsOssResult();
-        }
-    };
-
-    DOCTEST_INTERFACE String rawMemoryToString(const void* object, unsigned size);
+    template <typename T>
+    struct filldata;
 
     template <typename T>
-    String rawMemoryToString(const DOCTEST_REF_WRAP(T) object) {
-        return rawMemoryToString(&object, sizeof(object));
+    void filloss(std::ostream* stream, const T& in) {
+        filldata<T>::fill(stream, in);
+    }
+
+    template <typename T, size_t N>
+    void filloss(std::ostream* stream, const T (&in)[N]) { // NOLINT(*-avoid-c-arrays)
+        // T[N], T(&)[N], T(&&)[N] have same behaviour.
+        // Hence remove reference.
+        filloss<typename types::remove_reference<decltype(in)>::type>(stream, in);
     }
 
     template <typename T>
-    const char* type_to_string() {
-        return "<>";
+    String toStream(const T& in) {
+        std::ostream* stream = tlssPush();
+        filloss(stream, in);
+        return tlssPop();
     }
+
+    template <>
+    struct StringMakerBase<true> {
+        template <typename T>
+        static String convert(const DOCTEST_REF_WRAP(T) in) {
+            return toStream(in);
+        }
+    };
 } // namespace detail
 
 template <typename T>
-struct StringMaker : public detail::StringMakerBase<detail::has_insertion_operator<T>::value>
+struct StringMaker : public detail::StringMakerBase<
+    detail::has_insertion_operator<T>::value || detail::types::is_pointer<T>::value || detail::types::is_array<T>::value>
 {};
 
-template <typename T>
-struct StringMaker<T*>
-{
-    template <typename U>
-    static String convert(U* p) {
-        if(p)
-            return detail::rawMemoryToString(p);
-        return "NULL";
-    }
-};
-
-template <typename R, typename C>
-struct StringMaker<R C::*>
-{
-    static String convert(R C::*p) {
-        if(p)
-            return detail::rawMemoryToString(p);
-        return "NULL";
-    }
-};
+#ifndef DOCTEST_STRINGIFY
+#ifdef DOCTEST_CONFIG_DOUBLE_STRINGIFY
+#define DOCTEST_STRINGIFY(...) toString(toString(__VA_ARGS__))
+#else
+#define DOCTEST_STRINGIFY(...) toString(__VA_ARGS__)
+#endif
+#endif
 
 template <typename T>
+String toString() {
+#if DOCTEST_CLANG == 0 && DOCTEST_GCC == 0 && DOCTEST_ICC == 0
+    String ret = __FUNCSIG__; // class doctest::String __cdecl doctest::toString<TYPE>(void)
+    String::size_type beginPos = ret.find('<');
+    return ret.substr(beginPos + 1, ret.size() - beginPos - static_cast<String::size_type>(sizeof(">(void)")));
+#else
+    String ret = __PRETTY_FUNCTION__; // doctest::String toString() [with T = TYPE]
+    String::size_type begin = ret.find('=') + 2;
+    return ret.substr(begin, ret.size() - begin - 1);
+#endif
+}
+
+template <typename T, typename detail::types::enable_if<!detail::should_stringify_as_underlying_type<T>::value, bool>::type = true>
 String toString(const DOCTEST_REF_WRAP(T) value) {
     return StringMaker<T>::convert(value);
 }
 
 #ifdef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-DOCTEST_INTERFACE String toString(char* in);
 DOCTEST_INTERFACE String toString(const char* in);
 #endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
+
+#if DOCTEST_MSVC >= DOCTEST_COMPILER(19, 20, 0)
+// see this issue on why this is needed: https://github.com/doctest/doctest/issues/183
+DOCTEST_INTERFACE String toString(const std::string& in);
+#endif // VS 2019
+
+DOCTEST_INTERFACE String toString(String in);
+
+DOCTEST_INTERFACE String toString(std::nullptr_t);
+
 DOCTEST_INTERFACE String toString(bool in);
+
 DOCTEST_INTERFACE String toString(float in);
 DOCTEST_INTERFACE String toString(double in);
 DOCTEST_INTERFACE String toString(double long in);
 
 DOCTEST_INTERFACE String toString(char in);
 DOCTEST_INTERFACE String toString(char signed in);
 DOCTEST_INTERFACE String toString(char unsigned in);
-DOCTEST_INTERFACE String toString(int short in);
-DOCTEST_INTERFACE String toString(int short unsigned in);
-DOCTEST_INTERFACE String toString(int in);
-DOCTEST_INTERFACE String toString(int unsigned in);
-DOCTEST_INTERFACE String toString(int long in);
-DOCTEST_INTERFACE String toString(int long unsigned in);
-DOCTEST_INTERFACE String toString(int long long in);
-DOCTEST_INTERFACE String toString(int long long unsigned in);
-DOCTEST_INTERFACE String toString(std::nullptr_t in);
+DOCTEST_INTERFACE String toString(short in);
+DOCTEST_INTERFACE String toString(short unsigned in);
+DOCTEST_INTERFACE String toString(signed in);
+DOCTEST_INTERFACE String toString(unsigned in);
+DOCTEST_INTERFACE String toString(long in);
+DOCTEST_INTERFACE String toString(long unsigned in);
+DOCTEST_INTERFACE String toString(long long in);
+DOCTEST_INTERFACE String toString(long long unsigned in);
 
-#if DOCTEST_MSVC >= DOCTEST_COMPILER(19, 20, 0)
-// see this issue on why this is needed: https://github.com/onqtam/doctest/issues/183
-DOCTEST_INTERFACE String toString(const std::string& in);
-#endif // VS 2019
+template <typename T, typename detail::types::enable_if<detail::should_stringify_as_underlying_type<T>::value, bool>::type = true>
+String toString(const DOCTEST_REF_WRAP(T) value) {
+    using UT = typename detail::types::underlying_type<T>::type;
+    return (DOCTEST_STRINGIFY(static_cast<UT>(value)));
+}
+
+namespace detail {
+    template <typename T>
+    struct filldata
+    {
+        static void fill(std::ostream* stream, const T& in) {
+#if defined(_MSC_VER) && _MSC_VER <= 1900
+        insert_hack_t<T>::insert(*stream, in);
+#else
+        operator<<(*stream, in);
+#endif
+        }
+    };
+
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4866)
+// NOLINTBEGIN(*-avoid-c-arrays)
+    template <typename T, size_t N>
+    struct filldata<T[N]> {
+        static void fill(std::ostream* stream, const T(&in)[N]) {
+            *stream << "[";
+            for (size_t i = 0; i < N; i++) {
+                if (i != 0) { *stream << ", "; }
+                *stream << (DOCTEST_STRINGIFY(in[i]));
+            }
+            *stream << "]";
+        }
+    };
+// NOLINTEND(*-avoid-c-arrays)
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
+
+    // Specialized since we don't want the terminating null byte!
+// NOLINTBEGIN(*-avoid-c-arrays)
+    template <size_t N>
+    struct filldata<const char[N]> {
+        static void fill(std::ostream* stream, const char (&in)[N]) {
+            *stream << String(in, in[N - 1] ? N : N - 1);
+        } // NOLINT(clang-analyzer-cplusplus.NewDeleteLeaks)
+    };
+// NOLINTEND(*-avoid-c-arrays)
+
+    template <>
+    struct filldata<const void*> {
+        static void fill(std::ostream* stream, const void* in);
+    };
 
-class DOCTEST_INTERFACE Approx
+    template <typename T>
+    struct filldata<T*> {
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4180)
+        static void fill(std::ostream* stream, const T* in) {
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
+DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wmicrosoft-cast")
+            filldata<const void*>::fill(stream,
+#if DOCTEST_GCC == 0 || DOCTEST_GCC >= DOCTEST_COMPILER(4, 9, 0)
+                reinterpret_cast<const void*>(in)
+#else
+                *reinterpret_cast<const void* const*>(&in)
+#endif
+            );
+DOCTEST_CLANG_SUPPRESS_WARNING_POP
+        }
+    };
+}
+
+struct DOCTEST_INTERFACE Approx
 {
-public:
-    explicit Approx(double value);
+    Approx(double value);
 
     Approx operator()(double value) const;
 
 #ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
     template <typename T>
     explicit Approx(const T& value,
-                    typename detail::enable_if<std::is_constructible<double, T>::value>::type* =
+                    typename detail::types::enable_if<std::is_constructible<double, T>::value>::type* =
                             static_cast<T*>(nullptr)) {
-        *this = Approx(static_cast<double>(value));
+        *this = static_cast<double>(value);
     }
 #endif // DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 
     Approx& epsilon(double newEpsilon);
 
 #ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
     template <typename T>
-    typename detail::enable_if<std::is_constructible<double, T>::value, Approx&>::type epsilon(
+    typename std::enable_if<std::is_constructible<double, T>::value, Approx&>::type epsilon(
             const T& newEpsilon) {
         m_epsilon = static_cast<double>(newEpsilon);
         return *this;
     }
 #endif //  DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 
     Approx& scale(double newScale);
 
 #ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
     template <typename T>
-    typename detail::enable_if<std::is_constructible<double, T>::value, Approx&>::type scale(
+    typename std::enable_if<std::is_constructible<double, T>::value, Approx&>::type scale(
             const T& newScale) {
         m_scale = static_cast<double>(newScale);
         return *this;
     }
 #endif // DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 
     // clang-format off
@@ -934,59 +1255,73 @@
     DOCTEST_INTERFACE friend bool operator>=(double lhs, const Approx & rhs);
     DOCTEST_INTERFACE friend bool operator>=(const Approx & lhs, double rhs);
     DOCTEST_INTERFACE friend bool operator< (double lhs, const Approx & rhs);
     DOCTEST_INTERFACE friend bool operator< (const Approx & lhs, double rhs);
     DOCTEST_INTERFACE friend bool operator> (double lhs, const Approx & rhs);
     DOCTEST_INTERFACE friend bool operator> (const Approx & lhs, double rhs);
 
-    DOCTEST_INTERFACE friend String toString(const Approx& in);
-
 #ifdef DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 #define DOCTEST_APPROX_PREFIX \
-    template <typename T> friend typename detail::enable_if<std::is_constructible<double, T>::value, bool>::type
+    template <typename T> friend typename std::enable_if<std::is_constructible<double, T>::value, bool>::type
 
-    DOCTEST_APPROX_PREFIX operator==(const T& lhs, const Approx& rhs) { return operator==(double(lhs), rhs); }
+    DOCTEST_APPROX_PREFIX operator==(const T& lhs, const Approx& rhs) { return operator==(static_cast<double>(lhs), rhs); }
     DOCTEST_APPROX_PREFIX operator==(const Approx& lhs, const T& rhs) { return operator==(rhs, lhs); }
     DOCTEST_APPROX_PREFIX operator!=(const T& lhs, const Approx& rhs) { return !operator==(lhs, rhs); }
     DOCTEST_APPROX_PREFIX operator!=(const Approx& lhs, const T& rhs) { return !operator==(rhs, lhs); }
-    DOCTEST_APPROX_PREFIX operator<=(const T& lhs, const Approx& rhs) { return double(lhs) < rhs.m_value || lhs == rhs; }
-    DOCTEST_APPROX_PREFIX operator<=(const Approx& lhs, const T& rhs) { return lhs.m_value < double(rhs) || lhs == rhs; }
-    DOCTEST_APPROX_PREFIX operator>=(const T& lhs, const Approx& rhs) { return double(lhs) > rhs.m_value || lhs == rhs; }
-    DOCTEST_APPROX_PREFIX operator>=(const Approx& lhs, const T& rhs) { return lhs.m_value > double(rhs) || lhs == rhs; }
-    DOCTEST_APPROX_PREFIX operator< (const T& lhs, const Approx& rhs) { return double(lhs) < rhs.m_value && lhs != rhs; }
-    DOCTEST_APPROX_PREFIX operator< (const Approx& lhs, const T& rhs) { return lhs.m_value < double(rhs) && lhs != rhs; }
-    DOCTEST_APPROX_PREFIX operator> (const T& lhs, const Approx& rhs) { return double(lhs) > rhs.m_value && lhs != rhs; }
-    DOCTEST_APPROX_PREFIX operator> (const Approx& lhs, const T& rhs) { return lhs.m_value > double(rhs) && lhs != rhs; }
+    DOCTEST_APPROX_PREFIX operator<=(const T& lhs, const Approx& rhs) { return static_cast<double>(lhs) < rhs.m_value || lhs == rhs; }
+    DOCTEST_APPROX_PREFIX operator<=(const Approx& lhs, const T& rhs) { return lhs.m_value < static_cast<double>(rhs) || lhs == rhs; }
+    DOCTEST_APPROX_PREFIX operator>=(const T& lhs, const Approx& rhs) { return static_cast<double>(lhs) > rhs.m_value || lhs == rhs; }
+    DOCTEST_APPROX_PREFIX operator>=(const Approx& lhs, const T& rhs) { return lhs.m_value > static_cast<double>(rhs) || lhs == rhs; }
+    DOCTEST_APPROX_PREFIX operator< (const T& lhs, const Approx& rhs) { return static_cast<double>(lhs) < rhs.m_value && lhs != rhs; }
+    DOCTEST_APPROX_PREFIX operator< (const Approx& lhs, const T& rhs) { return lhs.m_value < static_cast<double>(rhs) && lhs != rhs; }
+    DOCTEST_APPROX_PREFIX operator> (const T& lhs, const Approx& rhs) { return static_cast<double>(lhs) > rhs.m_value && lhs != rhs; }
+    DOCTEST_APPROX_PREFIX operator> (const Approx& lhs, const T& rhs) { return lhs.m_value > static_cast<double>(rhs) && lhs != rhs; }
 #undef DOCTEST_APPROX_PREFIX
 #endif // DOCTEST_CONFIG_INCLUDE_TYPE_TRAITS
 
     // clang-format on
 
-private:
     double m_epsilon;
     double m_scale;
     double m_value;
 };
 
 DOCTEST_INTERFACE String toString(const Approx& in);
 
 DOCTEST_INTERFACE const ContextOptions* getContextOptions();
 
-#if !defined(DOCTEST_CONFIG_DISABLE)
+template <typename F>
+struct DOCTEST_INTERFACE_DECL IsNaN
+{
+    F value; bool flipped;
+    IsNaN(F f, bool flip = false) : value(f), flipped(flip) { }
+    IsNaN<F> operator!() const { return { value, !flipped }; }
+    operator bool() const;
+};
+#ifndef __MINGW32__
+extern template struct DOCTEST_INTERFACE_DECL IsNaN<float>;
+extern template struct DOCTEST_INTERFACE_DECL IsNaN<double>;
+extern template struct DOCTEST_INTERFACE_DECL IsNaN<long double>;
+#endif
+DOCTEST_INTERFACE String toString(IsNaN<float> in);
+DOCTEST_INTERFACE String toString(IsNaN<double> in);
+DOCTEST_INTERFACE String toString(IsNaN<double long> in);
+
+#ifndef DOCTEST_CONFIG_DISABLE
 
 namespace detail {
     // clang-format off
 #ifdef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-    template<class T>               struct decay_array       { typedef T type; };
-    template<class T, unsigned N>   struct decay_array<T[N]> { typedef T* type; };
-    template<class T>               struct decay_array<T[]>  { typedef T* type; };
-
-    template<class T>   struct not_char_pointer              { enum { value = 1 }; };
-    template<>          struct not_char_pointer<char*>       { enum { value = 0 }; };
-    template<>          struct not_char_pointer<const char*> { enum { value = 0 }; };
+    template<class T>               struct decay_array       { using type = T; };
+    template<class T, unsigned N>   struct decay_array<T[N]> { using type = T*; };
+    template<class T>               struct decay_array<T[]>  { using type = T*; };
+
+    template<class T>   struct not_char_pointer              { static DOCTEST_CONSTEXPR int value = 1; };
+    template<>          struct not_char_pointer<char*>       { static DOCTEST_CONSTEXPR int value = 0; };
+    template<>          struct not_char_pointer<const char*> { static DOCTEST_CONSTEXPR int value = 0; };
 
     template<class T> struct can_use_op : public not_char_pointer<typename decay_array<T>::type> {};
 #endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
     // clang-format on
 
     struct DOCTEST_INTERFACE TestFailureException
     {
@@ -1001,29 +1336,50 @@
 
     struct DOCTEST_INTERFACE Subcase
     {
         SubcaseSignature m_signature;
         bool             m_entered = false;
 
         Subcase(const String& name, const char* file, int line);
+        Subcase(const Subcase&) = delete;
+        Subcase(Subcase&&) = delete;
+        Subcase& operator=(const Subcase&) = delete;
+        Subcase& operator=(Subcase&&) = delete;
         ~Subcase();
 
         operator bool() const;
+
+        private:
+            bool checkFilters();
     };
 
     template <typename L, typename R>
     String stringifyBinaryExpr(const DOCTEST_REF_WRAP(L) lhs, const char* op,
                                const DOCTEST_REF_WRAP(R) rhs) {
-        return toString(lhs) + op + toString(rhs);
+        return (DOCTEST_STRINGIFY(lhs)) + op + (DOCTEST_STRINGIFY(rhs));
     }
 
+#if DOCTEST_CLANG && DOCTEST_CLANG < DOCTEST_COMPILER(3, 6, 0)
+DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wunused-comparison")
+#endif
+
+// This will check if there is any way it could find a operator like member or friend and uses it.
+// If not it doesn't find the operator or if the operator at global scope is defined after
+// this template, the template won't be instantiated due to SFINAE. Once the template is not
+// instantiated it can look for global operator using normal conversions.
+#ifdef __NVCC__
+#define SFINAE_OP(ret,op) ret
+#else
+#define SFINAE_OP(ret,op) decltype((void)(doctest::detail::declval<L>() op doctest::detail::declval<R>()),ret{})
+#endif
+
 #define DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(op, op_str, op_macro)                              \
     template <typename R>                                                                          \
-    DOCTEST_NOINLINE Result operator op(const DOCTEST_REF_WRAP(R) rhs) {                           \
-        bool res = op_macro(lhs, rhs);                                                             \
+    DOCTEST_NOINLINE SFINAE_OP(Result,op) operator op(R&& rhs) {                                   \
+    bool res = op_macro(doctest::detail::forward<const L>(lhs), doctest::detail::forward<R>(rhs)); \
         if(m_at & assertType::is_false)                                                            \
             res = !res;                                                                            \
         if(!res || doctest::getContextOptions()->success)                                          \
             return Result(res, stringifyBinaryExpr(lhs, op_str, rhs));                             \
         return Result(res);                                                                        \
     }
 
@@ -1034,19 +1390,20 @@
     template <typename R>                                                                          \
     rt& operator op(const R&) {                                                                    \
         static_assert(deferred_false<R>::value,                                                    \
                       "Expression Too Complex Please Rewrite As Binary Comparison!");              \
         return *this;                                                                              \
     }
 
-    struct DOCTEST_INTERFACE Result
+    struct DOCTEST_INTERFACE Result // NOLINT(*-member-init)
     {
         bool   m_passed;
         String m_decomp;
 
+        Result() = default; // TODO: Why do we need this? (To remove NOLINT)
         Result(bool passed, const String& decomposition = String());
 
         // forbidding some expressions based on this table: https://en.cppreference.com/w/cpp/language/operator_precedence
         DOCTEST_FORBIT_EXPRESSION(Result, &)
         DOCTEST_FORBIT_EXPRESSION(Result, ^)
         DOCTEST_FORBIT_EXPRESSION(Result, |)
         DOCTEST_FORBIT_EXPRESSION(Result, &&)
@@ -1095,15 +1452,15 @@
 
 #endif // DOCTEST_CONFIG_NO_COMPARISON_WARNING_SUPPRESSION
 
     // clang-format off
 #ifndef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
 #define DOCTEST_COMPARISON_RETURN_TYPE bool
 #else // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-#define DOCTEST_COMPARISON_RETURN_TYPE typename enable_if<can_use_op<L>::value || can_use_op<R>::value, bool>::type
+#define DOCTEST_COMPARISON_RETURN_TYPE typename types::enable_if<can_use_op<L>::value || can_use_op<R>::value, bool>::type
     inline bool eq(const char* lhs, const char* rhs) { return String(lhs) == String(rhs); }
     inline bool ne(const char* lhs, const char* rhs) { return String(lhs) != String(rhs); }
     inline bool lt(const char* lhs, const char* rhs) { return String(lhs) <  String(rhs); }
     inline bool gt(const char* lhs, const char* rhs) { return String(lhs) >  String(rhs); }
     inline bool le(const char* lhs, const char* rhs) { return String(lhs) <= String(rhs); }
     inline bool ge(const char* lhs, const char* rhs) { return String(lhs) >= String(rhs); }
 #endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
@@ -1142,28 +1499,36 @@
     template <typename L>
     // cppcheck-suppress copyCtorAndEqOperator
     struct Expression_lhs
     {
         L                lhs;
         assertType::Enum m_at;
 
-        explicit Expression_lhs(L in, assertType::Enum at)
-                : lhs(in)
+        explicit Expression_lhs(L&& in, assertType::Enum at)
+                : lhs(static_cast<L&&>(in))
                 , m_at(at) {}
 
         DOCTEST_NOINLINE operator Result() {
-            bool res = !!lhs;
-            if(m_at & assertType::is_false) //!OCLINT bitwise operator in conditional
+// this is needed only for MSVC 2015
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4800) // 'int': forcing value to bool
+            bool res = static_cast<bool>(lhs);
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
+            if(m_at & assertType::is_false) { //!OCLINT bitwise operator in conditional
                 res = !res;
+            }
 
-            if(!res || getContextOptions()->success)
-                return Result(res, toString(lhs));
-            return Result(res);
+            if(!res || getContextOptions()->success) {
+                return { res, (DOCTEST_STRINGIFY(lhs)) };
+            }
+            return { res };
         }
 
+        /* This is required for user-defined conversions from Expression_lhs to L */
+        operator L() const { return lhs; }
+
         // clang-format off
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(==, " == ", DOCTEST_CMP_EQ) //!OCLINT bitwise operator in conditional
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(!=, " != ", DOCTEST_CMP_NE) //!OCLINT bitwise operator in conditional
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(>,  " >  ", DOCTEST_CMP_GT) //!OCLINT bitwise operator in conditional
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(<,  " <  ", DOCTEST_CMP_LT) //!OCLINT bitwise operator in conditional
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(>=, " >= ", DOCTEST_CMP_GE) //!OCLINT bitwise operator in conditional
         DOCTEST_DO_BINARY_EXPRESSION_COMPARISON(<=, " <= ", DOCTEST_CMP_LE) //!OCLINT bitwise operator in conditional
@@ -1196,77 +1561,93 @@
 
     DOCTEST_CLANG_SUPPRESS_WARNING_POP
     DOCTEST_MSVC_SUPPRESS_WARNING_POP
     DOCTEST_GCC_SUPPRESS_WARNING_POP
 
 #endif // DOCTEST_CONFIG_NO_COMPARISON_WARNING_SUPPRESSION
 
+#if DOCTEST_CLANG && DOCTEST_CLANG < DOCTEST_COMPILER(3, 6, 0)
+DOCTEST_CLANG_SUPPRESS_WARNING_POP
+#endif
+
     struct DOCTEST_INTERFACE ExpressionDecomposer
     {
         assertType::Enum m_at;
 
         ExpressionDecomposer(assertType::Enum at);
 
         // The right operator for capturing expressions is "<=" instead of "<<" (based on the operator precedence table)
         // but then there will be warnings from GCC about "-Wparentheses" and since "_Pragma()" is problematic this will stay for now...
         // https://github.com/catchorg/Catch2/issues/870
         // https://github.com/catchorg/Catch2/issues/565
         template <typename L>
-        Expression_lhs<const DOCTEST_REF_WRAP(L)> operator<<(const DOCTEST_REF_WRAP(L) operand) {
-            return Expression_lhs<const DOCTEST_REF_WRAP(L)>(operand, m_at);
+        Expression_lhs<L> operator<<(L&& operand) {
+            return Expression_lhs<L>(static_cast<L&&>(operand), m_at);
+        }
+
+        template <typename L,typename types::enable_if<!doctest::detail::types::is_rvalue_reference<L>::value,void >::type* = nullptr>
+        Expression_lhs<const L&> operator<<(const L &operand) {
+            return Expression_lhs<const L&>(operand, m_at);
         }
     };
 
     struct DOCTEST_INTERFACE TestSuite
     {
-        const char* m_test_suite;
-        const char* m_description;
-        bool        m_skip;
-        bool        m_may_fail;
-        bool        m_should_fail;
-        int         m_expected_failures;
-        double      m_timeout;
+        const char* m_test_suite = nullptr;
+        const char* m_description = nullptr;
+        bool        m_skip = false;
+        bool        m_no_breaks = false;
+        bool        m_no_output = false;
+        bool        m_may_fail = false;
+        bool        m_should_fail = false;
+        int         m_expected_failures = 0;
+        double      m_timeout = 0;
 
         TestSuite& operator*(const char* in);
 
         template <typename T>
         TestSuite& operator*(const T& in) {
             in.fill(*this);
             return *this;
         }
     };
 
-    typedef void (*funcType)();
+    using funcType = void (*)();
 
     struct DOCTEST_INTERFACE TestCase : public TestCaseData
     {
         funcType m_test; // a function pointer to the test case
 
-        const char* m_type; // for templated test cases - gets appended to the real name
+        String m_type; // for templated test cases - gets appended to the real name
         int m_template_id; // an ID used to distinguish between the different versions of a templated test case
         String m_full_name; // contains the name (only for templated test cases!) + the template type
 
         TestCase(funcType test, const char* file, unsigned line, const TestSuite& test_suite,
-                 const char* type = "", int template_id = -1);
+                 const String& type = String(), int template_id = -1);
 
         TestCase(const TestCase& other);
+        TestCase(TestCase&&) = delete;
 
         DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(26434) // hides a non-virtual function
         TestCase& operator=(const TestCase& other);
         DOCTEST_MSVC_SUPPRESS_WARNING_POP
 
+        TestCase& operator=(TestCase&&) = delete;
+
         TestCase& operator*(const char* in);
 
         template <typename T>
         TestCase& operator*(const T& in) {
             in.fill(*this);
             return *this;
         }
 
         bool operator<(const TestCase& other) const;
+
+        ~TestCase() = default;
     };
 
     // forward declarations of functions used by the macros
     DOCTEST_INTERFACE int  regTest(const TestCase& tc);
     DOCTEST_INTERFACE int  setTestSuite(const TestSuite& ts);
     DOCTEST_INTERFACE bool isDebuggerActive();
 
@@ -1288,45 +1669,54 @@
     // clang-format off
     template <int, class L, class R> struct RelationalComparator     { bool operator()(const DOCTEST_REF_WRAP(L),     const DOCTEST_REF_WRAP(R)    ) const { return false;        } };
 
 #define DOCTEST_BINARY_RELATIONAL_OP(n, op) \
     template <class L, class R> struct RelationalComparator<n, L, R> { bool operator()(const DOCTEST_REF_WRAP(L) lhs, const DOCTEST_REF_WRAP(R) rhs) const { return op(lhs, rhs); } };
     // clang-format on
 
-    DOCTEST_BINARY_RELATIONAL_OP(0, eq)
-    DOCTEST_BINARY_RELATIONAL_OP(1, ne)
-    DOCTEST_BINARY_RELATIONAL_OP(2, gt)
-    DOCTEST_BINARY_RELATIONAL_OP(3, lt)
-    DOCTEST_BINARY_RELATIONAL_OP(4, ge)
-    DOCTEST_BINARY_RELATIONAL_OP(5, le)
+    DOCTEST_BINARY_RELATIONAL_OP(0, doctest::detail::eq)
+    DOCTEST_BINARY_RELATIONAL_OP(1, doctest::detail::ne)
+    DOCTEST_BINARY_RELATIONAL_OP(2, doctest::detail::gt)
+    DOCTEST_BINARY_RELATIONAL_OP(3, doctest::detail::lt)
+    DOCTEST_BINARY_RELATIONAL_OP(4, doctest::detail::ge)
+    DOCTEST_BINARY_RELATIONAL_OP(5, doctest::detail::le)
 
     struct DOCTEST_INTERFACE ResultBuilder : public AssertData
     {
         ResultBuilder(assertType::Enum at, const char* file, int line, const char* expr,
-                      const char* exception_type = "", const char* exception_string = "");
+                      const char* exception_type = "", const String& exception_string = "");
+
+        ResultBuilder(assertType::Enum at, const char* file, int line, const char* expr,
+                      const char* exception_type, const Contains& exception_string);
 
         void setResult(const Result& res);
 
         template <int comparison, typename L, typename R>
-        DOCTEST_NOINLINE void binary_assert(const DOCTEST_REF_WRAP(L) lhs,
+        DOCTEST_NOINLINE bool binary_assert(const DOCTEST_REF_WRAP(L) lhs,
                                             const DOCTEST_REF_WRAP(R) rhs) {
             m_failed = !RelationalComparator<comparison, L, R>()(lhs, rhs);
-            if(m_failed || getContextOptions()->success)
+            if (m_failed || getContextOptions()->success) {
                 m_decomp = stringifyBinaryExpr(lhs, ", ", rhs);
+            }
+            return !m_failed;
         }
 
         template <typename L>
-        DOCTEST_NOINLINE void unary_assert(const DOCTEST_REF_WRAP(L) val) {
+        DOCTEST_NOINLINE bool unary_assert(const DOCTEST_REF_WRAP(L) val) {
             m_failed = !val;
 
-            if(m_at & assertType::is_false) //!OCLINT bitwise operator in conditional
+            if (m_at & assertType::is_false) { //!OCLINT bitwise operator in conditional
                 m_failed = !m_failed;
+            }
 
-            if(m_failed || getContextOptions()->success)
-                m_decomp = toString(val);
+            if (m_failed || getContextOptions()->success) {
+                m_decomp = (DOCTEST_STRINGIFY(val));
+            }
+
+            return !m_failed;
         }
 
         void translateException();
 
         bool log();
         void react() const;
     };
@@ -1338,78 +1728,79 @@
             dbgbreak    = 1,
             shouldthrow = 2
         };
     } // namespace assertAction
 
     DOCTEST_INTERFACE void failed_out_of_a_testing_context(const AssertData& ad);
 
-    DOCTEST_INTERFACE void decomp_assert(assertType::Enum at, const char* file, int line,
-                                         const char* expr, Result result);
+    DOCTEST_INTERFACE bool decomp_assert(assertType::Enum at, const char* file, int line,
+                                         const char* expr, const Result& result);
 
 #define DOCTEST_ASSERT_OUT_OF_TESTS(decomp)                                                        \
     do {                                                                                           \
         if(!is_running_in_test) {                                                                  \
             if(failed) {                                                                           \
                 ResultBuilder rb(at, file, line, expr);                                            \
                 rb.m_failed = failed;                                                              \
                 rb.m_decomp = decomp;                                                              \
                 failed_out_of_a_testing_context(rb);                                               \
                 if(isDebuggerActive() && !getContextOptions()->no_breaks)                          \
                     DOCTEST_BREAK_INTO_DEBUGGER();                                                 \
                 if(checkIfShouldThrow(at))                                                         \
                     throwException();                                                              \
             }                                                                                      \
-            return;                                                                                \
+            return !failed;                                                                        \
         }                                                                                          \
     } while(false)
 
 #define DOCTEST_ASSERT_IN_TESTS(decomp)                                                            \
     ResultBuilder rb(at, file, line, expr);                                                        \
     rb.m_failed = failed;                                                                          \
     if(rb.m_failed || getContextOptions()->success)                                                \
         rb.m_decomp = decomp;                                                                      \
     if(rb.log())                                                                                   \
         DOCTEST_BREAK_INTO_DEBUGGER();                                                             \
     if(rb.m_failed && checkIfShouldThrow(at))                                                      \
     throwException()
 
     template <int comparison, typename L, typename R>
-    DOCTEST_NOINLINE void binary_assert(assertType::Enum at, const char* file, int line,
+    DOCTEST_NOINLINE bool binary_assert(assertType::Enum at, const char* file, int line,
                                         const char* expr, const DOCTEST_REF_WRAP(L) lhs,
                                         const DOCTEST_REF_WRAP(R) rhs) {
         bool failed = !RelationalComparator<comparison, L, R>()(lhs, rhs);
 
         // ###################################################################################
         // IF THE DEBUGGER BREAKS HERE - GO 1 LEVEL UP IN THE CALLSTACK FOR THE FAILING ASSERT
         // THIS IS THE EFFECT OF HAVING 'DOCTEST_CONFIG_SUPER_FAST_ASSERTS' DEFINED
         // ###################################################################################
         DOCTEST_ASSERT_OUT_OF_TESTS(stringifyBinaryExpr(lhs, ", ", rhs));
         DOCTEST_ASSERT_IN_TESTS(stringifyBinaryExpr(lhs, ", ", rhs));
+        return !failed;
     }
 
     template <typename L>
-    DOCTEST_NOINLINE void unary_assert(assertType::Enum at, const char* file, int line,
+    DOCTEST_NOINLINE bool unary_assert(assertType::Enum at, const char* file, int line,
                                        const char* expr, const DOCTEST_REF_WRAP(L) val) {
         bool failed = !val;
 
         if(at & assertType::is_false) //!OCLINT bitwise operator in conditional
             failed = !failed;
 
         // ###################################################################################
         // IF THE DEBUGGER BREAKS HERE - GO 1 LEVEL UP IN THE CALLSTACK FOR THE FAILING ASSERT
         // THIS IS THE EFFECT OF HAVING 'DOCTEST_CONFIG_SUPER_FAST_ASSERTS' DEFINED
         // ###################################################################################
-        DOCTEST_ASSERT_OUT_OF_TESTS(toString(val));
-        DOCTEST_ASSERT_IN_TESTS(toString(val));
+        DOCTEST_ASSERT_OUT_OF_TESTS((DOCTEST_STRINGIFY(val)));
+        DOCTEST_ASSERT_IN_TESTS((DOCTEST_STRINGIFY(val)));
+        return !failed;
     }
 
     struct DOCTEST_INTERFACE IExceptionTranslator
     {
-        IExceptionTranslator();
-        virtual ~IExceptionTranslator();
+        DOCTEST_DECLARE_INTERFACE(IExceptionTranslator)
         virtual bool translate(String&) const = 0;
     };
 
     template <typename T>
     class ExceptionTranslator : public IExceptionTranslator //!OCLINT destructor of virtual class
     {
     public:
@@ -1417,122 +1808,109 @@
                 : m_translateFunction(translateFunction) {}
 
         bool translate(String& res) const override {
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
             try {
                 throw; // lgtm [cpp/rethrow-no-exception]
                 // cppcheck-suppress catchExceptionByValue
-            } catch(T ex) {                    // NOLINT
+            } catch(const T& ex) {
                 res = m_translateFunction(ex); //!OCLINT parameter reassignment
                 return true;
-            } catch(...) {} //!OCLINT -  empty catch statement
-#endif                      // DOCTEST_CONFIG_NO_EXCEPTIONS
-            ((void)res);    // to silence -Wunused-parameter
+            } catch(...) {}         //!OCLINT -  empty catch statement
+#endif                              // DOCTEST_CONFIG_NO_EXCEPTIONS
+            static_cast<void>(res); // to silence -Wunused-parameter
             return false;
         }
 
     private:
         String (*m_translateFunction)(T);
     };
 
     DOCTEST_INTERFACE void registerExceptionTranslatorImpl(const IExceptionTranslator* et);
 
-    template <bool C>
-    struct StringStreamBase
-    {
-        template <typename T>
-        static void convert(std::ostream* s, const T& in) {
-            *s << toString(in);
-        }
-
-        // always treat char* as a string in this context - no matter
-        // if DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING is defined
-        static void convert(std::ostream* s, const char* in) { *s << String(in); }
-    };
-
-    template <>
-    struct StringStreamBase<true>
-    {
-        template <typename T>
-        static void convert(std::ostream* s, const T& in) {
-            *s << in;
-        }
-    };
-
-    template <typename T>
-    struct StringStream : public StringStreamBase<has_insertion_operator<T>::value>
-    {};
+    // ContextScope base class used to allow implementing methods of ContextScope
+    // that don't depend on the template parameter in doctest.cpp.
+    struct DOCTEST_INTERFACE ContextScopeBase : public IContextScope {
+        ContextScopeBase(const ContextScopeBase&) = delete;
 
-    template <typename T>
-    void toStream(std::ostream* s, const T& value) {
-        StringStream<T>::convert(s, value);
-    }
+        ContextScopeBase& operator=(const ContextScopeBase&) = delete;
+        ContextScopeBase& operator=(ContextScopeBase&&) = delete;
 
-#ifdef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-    DOCTEST_INTERFACE void toStream(std::ostream* s, char* in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, const char* in);
-#endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-    DOCTEST_INTERFACE void toStream(std::ostream* s, bool in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, float in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, double in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, double long in);
-
-    DOCTEST_INTERFACE void toStream(std::ostream* s, char in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, char signed in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, char unsigned in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int short in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int short unsigned in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int unsigned in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int long in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int long unsigned in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int long long in);
-    DOCTEST_INTERFACE void toStream(std::ostream* s, int long long unsigned in);
+        ~ContextScopeBase() override = default;
 
-    // ContextScope base class used to allow implementing methods of ContextScope 
-    // that don't depend on the template parameter in doctest.cpp.
-    class DOCTEST_INTERFACE ContextScopeBase : public IContextScope {
     protected:
         ContextScopeBase();
+        ContextScopeBase(ContextScopeBase&& other) noexcept;
 
         void destroy();
+        bool need_to_destroy{true};
     };
 
     template <typename L> class ContextScope : public ContextScopeBase
     {
-        const L &lambda_;
+        L lambda_;
 
     public:
         explicit ContextScope(const L &lambda) : lambda_(lambda) {}
+        explicit ContextScope(L&& lambda) : lambda_(static_cast<L&&>(lambda)) { }
 
-        ContextScope(ContextScope &&other) : lambda_(other.lambda_) {}
+        ContextScope(const ContextScope&) = delete;
+        ContextScope(ContextScope&&) noexcept = default;
+
+        ContextScope& operator=(const ContextScope&) = delete;
+        ContextScope& operator=(ContextScope&&) = delete;
 
         void stringify(std::ostream* s) const override { lambda_(s); }
 
-        ~ContextScope() override { destroy(); }
+        ~ContextScope() override {
+            if (need_to_destroy) {
+                destroy();
+            }
+        }
     };
 
     struct DOCTEST_INTERFACE MessageBuilder : public MessageData
     {
         std::ostream* m_stream;
+        bool          logged = false;
 
         MessageBuilder(const char* file, int line, assertType::Enum severity);
-        MessageBuilder() = delete;
+
+        MessageBuilder(const MessageBuilder&) = delete;
+        MessageBuilder(MessageBuilder&&) = delete;
+
+        MessageBuilder& operator=(const MessageBuilder&) = delete;
+        MessageBuilder& operator=(MessageBuilder&&) = delete;
+
         ~MessageBuilder();
 
+        // the preferred way of chaining parameters for stringification
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4866)
         template <typename T>
-        MessageBuilder& operator<<(const T& in) {
-            toStream(m_stream, in);
+        MessageBuilder& operator,(const T& in) {
+            *m_stream << (DOCTEST_STRINGIFY(in));
             return *this;
         }
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
+
+        // kept here just for backwards-compatibility - the comma operator should be preferred now
+        template <typename T>
+        MessageBuilder& operator<<(const T& in) { return this->operator,(in); }
+
+        // the `,` operator has the lowest operator precedence - if `<<` is used by the user then
+        // the `,` operator will be called last which is not what we want and thus the `*` operator
+        // is used first (has higher operator precedence compared to `<<`) so that we guarantee that
+        // an operator of the MessageBuilder class is called first before the rest of the parameters
+        template <typename T>
+        MessageBuilder& operator*(const T& in) { return this->operator,(in); }
 
         bool log();
         void react();
     };
-    
+
     template <typename L>
     ContextScope<L> MakeContextScope(const L &lambda) {
         return ContextScope<L>(lambda);
     }
 } // namespace detail
 
 #define DOCTEST_DEFINE_DECORATOR(name, type, def)                                                  \
@@ -1544,14 +1922,16 @@
         void fill(detail::TestCase& state) const { state.DOCTEST_CAT(m_, name) = data; }           \
         void fill(detail::TestSuite& state) const { state.DOCTEST_CAT(m_, name) = data; }          \
     }
 
 DOCTEST_DEFINE_DECORATOR(test_suite, const char*, "");
 DOCTEST_DEFINE_DECORATOR(description, const char*, "");
 DOCTEST_DEFINE_DECORATOR(skip, bool, true);
+DOCTEST_DEFINE_DECORATOR(no_breaks, bool, true);
+DOCTEST_DEFINE_DECORATOR(no_output, bool, true);
 DOCTEST_DEFINE_DECORATOR(timeout, double, 0);
 DOCTEST_DEFINE_DECORATOR(may_fail, bool, true);
 DOCTEST_DEFINE_DECORATOR(should_fail, bool, true);
 DOCTEST_DEFINE_DECORATOR(expected_failures, int, 0);
 
 template <typename T>
 int registerExceptionTranslator(String (*translateFunction)(T)) {
@@ -1575,42 +1955,51 @@
 template <typename T>
 int registerExceptionTranslator(String (*)(T)) {
     return 0;
 }
 #endif // DOCTEST_CONFIG_DISABLE
 
 namespace detail {
-    typedef void (*assert_handler)(const AssertData&);
+    using assert_handler = void (*)(const AssertData&);
     struct ContextState;
 } // namespace detail
 
 class DOCTEST_INTERFACE Context
 {
     detail::ContextState* p;
 
     void parseArgs(int argc, const char* const* argv, bool withDefaults = false);
 
 public:
     explicit Context(int argc = 0, const char* const* argv = nullptr);
 
-    ~Context();
+    Context(const Context&) = delete;
+    Context(Context&&) = delete;
+
+    Context& operator=(const Context&) = delete;
+    Context& operator=(Context&&) = delete;
+
+    ~Context(); // NOLINT(performance-trivially-destructible)
 
     void applyCommandLine(int argc, const char* const* argv);
 
     void addFilter(const char* filter, const char* value);
     void clearFilters();
+    void setOption(const char* option, bool value);
     void setOption(const char* option, int value);
     void setOption(const char* option, const char* value);
 
     bool shouldExit();
 
     void setAsDefaultForAssertsOutOfTestCases();
 
     void setAssertHandler(detail::assert_handler ah);
 
+    void setCout(std::ostream* out);
+
     int run();
 };
 
 namespace TestCaseFailureReason {
     enum Enum
     {
         None                     = 0,
@@ -1629,14 +2018,15 @@
 
 struct DOCTEST_INTERFACE CurrentTestCaseStats
 {
     int    numAssertsCurrentTest;
     int    numAssertsFailedCurrentTest;
     double seconds;
     int    failure_flags; // use TestCaseFailureReason::Enum
+    bool   testCaseSuccess;
 };
 
 struct DOCTEST_INTERFACE TestCaseException
 {
     String error_string;
     bool   is_crash;
 };
@@ -1692,28 +2082,27 @@
     // called for each message (don't cache pointers to the input)
     virtual void log_message(const MessageData&) = 0;
 
     // called when a test case is skipped either because it doesn't pass the filters, has a skip decorator
     // or isn't in the execution range (between first and last) (safe to cache a pointer to the input)
     virtual void test_case_skipped(const TestCaseData&) = 0;
 
-    // doctest will not be managing the lifetimes of reporters given to it but this would still be nice to have
-    virtual ~IReporter();
+    DOCTEST_DECLARE_INTERFACE(IReporter)
 
     // can obtain all currently active contexts and stringify them if one wishes to do so
     static int                         get_num_active_contexts();
     static const IContextScope* const* get_active_contexts();
 
     // can iterate through contexts which have been stringified automatically in their destructors when an exception has been thrown
     static int           get_num_stringified_contexts();
     static const String* get_stringified_contexts();
 };
 
 namespace detail {
-    typedef IReporter* (*reporterCreatorFunc)(const ContextOptions&);
+    using reporterCreatorFunc =  IReporter* (*)(const ContextOptions&);
 
     DOCTEST_INTERFACE void registerReporterImpl(const char* name, int prio, reporterCreatorFunc c, bool isReporter);
 
     template <typename Reporter>
     IReporter* reporterCreator(const ContextOptions& o) {
         return new Reporter(o);
     }
@@ -1722,121 +2111,135 @@
 template <typename Reporter>
 int registerReporter(const char* name, int priority, bool isReporter) {
     detail::registerReporterImpl(name, priority, detail::reporterCreator<Reporter>, isReporter);
     return 0;
 }
 } // namespace doctest
 
+#ifdef DOCTEST_CONFIG_ASSERTS_RETURN_VALUES
+#define DOCTEST_FUNC_EMPTY [] { return false; }()
+#else
+#define DOCTEST_FUNC_EMPTY (void)0
+#endif
+
 // if registering is not disabled
-#if !defined(DOCTEST_CONFIG_DISABLE)
+#ifndef DOCTEST_CONFIG_DISABLE
+
+#ifdef DOCTEST_CONFIG_ASSERTS_RETURN_VALUES
+#define DOCTEST_FUNC_SCOPE_BEGIN [&]
+#define DOCTEST_FUNC_SCOPE_END ()
+#define DOCTEST_FUNC_SCOPE_RET(v) return v
+#else
+#define DOCTEST_FUNC_SCOPE_BEGIN do
+#define DOCTEST_FUNC_SCOPE_END while(false)
+#define DOCTEST_FUNC_SCOPE_RET(v) (void)0
+#endif
 
 // common code in asserts - for convenience
-#define DOCTEST_ASSERT_LOG_AND_REACT(b)                                                            \
-    if(b.log())                                                                                    \
-        DOCTEST_BREAK_INTO_DEBUGGER();                                                             \
-    b.react()
+#define DOCTEST_ASSERT_LOG_REACT_RETURN(b)                                                         \
+    if(b.log()) DOCTEST_BREAK_INTO_DEBUGGER();                                                     \
+    b.react();                                                                                     \
+    DOCTEST_FUNC_SCOPE_RET(!b.m_failed)
 
 #ifdef DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS
 #define DOCTEST_WRAP_IN_TRY(x) x;
 #else // DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS
 #define DOCTEST_WRAP_IN_TRY(x)                                                                     \
     try {                                                                                          \
         x;                                                                                         \
-    } catch(...) { _DOCTEST_RB.translateException(); }
+    } catch(...) { DOCTEST_RB.translateException(); }
 #endif // DOCTEST_CONFIG_NO_TRY_CATCH_IN_ASSERTS
 
 #ifdef DOCTEST_CONFIG_VOID_CAST_EXPRESSIONS
 #define DOCTEST_CAST_TO_VOID(...)                                                                  \
     DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wuseless-cast")                                       \
     static_cast<void>(__VA_ARGS__);                                                                \
     DOCTEST_GCC_SUPPRESS_WARNING_POP
 #else // DOCTEST_CONFIG_VOID_CAST_EXPRESSIONS
 #define DOCTEST_CAST_TO_VOID(...) __VA_ARGS__;
 #endif // DOCTEST_CONFIG_VOID_CAST_EXPRESSIONS
 
 // registers the test by initializing a dummy var with a function
 #define DOCTEST_REGISTER_FUNCTION(global_prefix, f, decorators)                                    \
-    global_prefix DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_VAR_)) =              \
+    global_prefix DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_VAR_), /* NOLINT */    \
             doctest::detail::regTest(                                                              \
                     doctest::detail::TestCase(                                                     \
                             f, __FILE__, __LINE__,                                                 \
                             doctest_detail_test_suite_ns::getCurrentTestSuite()) *                 \
-                    decorators);                                                                   \
-    DOCTEST_GLOBAL_NO_WARNINGS_END()
+                    decorators))
 
 #define DOCTEST_IMPLEMENT_FIXTURE(der, base, func, decorators)                                     \
-    namespace {                                                                                    \
+    namespace { /* NOLINT */                                                                       \
         struct der : public base                                                                   \
         {                                                                                          \
             void f();                                                                              \
         };                                                                                         \
-        static void func() {                                                                       \
+        static DOCTEST_INLINE_NOINLINE void func() {                                               \
             der v;                                                                                 \
             v.f();                                                                                 \
         }                                                                                          \
         DOCTEST_REGISTER_FUNCTION(DOCTEST_EMPTY, func, decorators)                                 \
     }                                                                                              \
-    inline DOCTEST_NOINLINE void der::f()
+    DOCTEST_INLINE_NOINLINE void der::f() // NOLINT(misc-definitions-in-headers)
 
 #define DOCTEST_CREATE_AND_REGISTER_FUNCTION(f, decorators)                                        \
     static void f();                                                                               \
     DOCTEST_REGISTER_FUNCTION(DOCTEST_EMPTY, f, decorators)                                        \
     static void f()
 
 #define DOCTEST_CREATE_AND_REGISTER_FUNCTION_IN_CLASS(f, proxy, decorators)                        \
     static doctest::detail::funcType proxy() { return f; }                                         \
-    DOCTEST_REGISTER_FUNCTION(inline const, proxy(), decorators)                                   \
+    DOCTEST_REGISTER_FUNCTION(inline, proxy(), decorators)                                         \
     static void f()
 
 // for registering tests
 #define DOCTEST_TEST_CASE(decorators)                                                              \
-    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_), decorators)
+    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_), decorators)
 
 // for registering tests in classes - requires C++17 for inline variables!
-#if __cplusplus >= 201703L || (DOCTEST_MSVC >= DOCTEST_COMPILER(19, 12, 0) && _MSVC_LANG >= 201703L)
+#if DOCTEST_CPLUSPLUS >= 201703L
 #define DOCTEST_TEST_CASE_CLASS(decorators)                                                        \
-    DOCTEST_CREATE_AND_REGISTER_FUNCTION_IN_CLASS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_),          \
-                                                  DOCTEST_ANONYMOUS(_DOCTEST_ANON_PROXY_),         \
+    DOCTEST_CREATE_AND_REGISTER_FUNCTION_IN_CLASS(DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_),           \
+                                                  DOCTEST_ANONYMOUS(DOCTEST_ANON_PROXY_),          \
                                                   decorators)
 #else // DOCTEST_TEST_CASE_CLASS
 #define DOCTEST_TEST_CASE_CLASS(...)                                                               \
     TEST_CASES_CAN_BE_REGISTERED_IN_CLASSES_ONLY_IN_CPP17_MODE_OR_WITH_VS_2017_OR_NEWER
 #endif // DOCTEST_TEST_CASE_CLASS
 
 // for registering tests with a fixture
 #define DOCTEST_TEST_CASE_FIXTURE(c, decorators)                                                   \
-    DOCTEST_IMPLEMENT_FIXTURE(DOCTEST_ANONYMOUS(_DOCTEST_ANON_CLASS_), c,                          \
-                              DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_), decorators)
+    DOCTEST_IMPLEMENT_FIXTURE(DOCTEST_ANONYMOUS(DOCTEST_ANON_CLASS_), c,                           \
+                              DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_), decorators)
 
 // for converting types to strings without the <typeinfo> header and demangling
-#define DOCTEST_TYPE_TO_STRING_IMPL(...)                                                           \
-    template <>                                                                                    \
-    inline const char* type_to_string<__VA_ARGS__>() {                                             \
-        return "<" #__VA_ARGS__ ">";                                                               \
-    }
-#define DOCTEST_TYPE_TO_STRING(...)                                                                \
-    namespace doctest { namespace detail {                                                         \
-            DOCTEST_TYPE_TO_STRING_IMPL(__VA_ARGS__)                                               \
+#define DOCTEST_TYPE_TO_STRING_AS(str, ...)                                                        \
+    namespace doctest {                                                                            \
+        template <>                                                                                \
+        inline String toString<__VA_ARGS__>() {                                                    \
+            return str;                                                                            \
         }                                                                                          \
     }                                                                                              \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    static_assert(true, "")
+
+#define DOCTEST_TYPE_TO_STRING(...) DOCTEST_TYPE_TO_STRING_AS(#__VA_ARGS__, __VA_ARGS__)
 
 #define DOCTEST_TEST_CASE_TEMPLATE_DEFINE_IMPL(dec, T, iter, func)                                 \
     template <typename T>                                                                          \
     static void func();                                                                            \
-    namespace {                                                                                    \
+    namespace { /* NOLINT */                                                                       \
         template <typename Tuple>                                                                  \
         struct iter;                                                                               \
         template <typename Type, typename... Rest>                                                 \
         struct iter<std::tuple<Type, Rest...>>                                                     \
         {                                                                                          \
             iter(const char* file, unsigned line, int index) {                                     \
                 doctest::detail::regTest(doctest::detail::TestCase(func<Type>, file, line,         \
                                             doctest_detail_test_suite_ns::getCurrentTestSuite(),   \
-                                            doctest::detail::type_to_string<Type>(),               \
+                                            doctest::toString<Type>(),                             \
                                             int(line) * 1000 + index)                              \
                                          * dec);                                                   \
                 iter<std::tuple<Rest...>>(file, line, index + 1);                                  \
             }                                                                                      \
         };                                                                                         \
         template <>                                                                                \
         struct iter<std::tuple<>>                                                                  \
@@ -1845,224 +2248,285 @@
         };                                                                                         \
     }                                                                                              \
     template <typename T>                                                                          \
     static void func()
 
 #define DOCTEST_TEST_CASE_TEMPLATE_DEFINE(dec, T, id)                                              \
     DOCTEST_TEST_CASE_TEMPLATE_DEFINE_IMPL(dec, T, DOCTEST_CAT(id, ITERATOR),                      \
-                                           DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_))
+                                           DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_))
 
 #define DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(id, anon, ...)                                 \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_CAT(anon, DUMMY)) =                                         \
-        doctest::detail::instantiationHelper(DOCTEST_CAT(id, ITERATOR)<__VA_ARGS__>(__FILE__, __LINE__, 0));\
-    DOCTEST_GLOBAL_NO_WARNINGS_END()
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_CAT(anon, DUMMY), /* NOLINT(cert-err58-cpp, fuchsia-statically-constructed-objects) */ \
+        doctest::detail::instantiationHelper(                                                      \
+            DOCTEST_CAT(id, ITERATOR)<__VA_ARGS__>(__FILE__, __LINE__, 0)))
 
 #define DOCTEST_TEST_CASE_TEMPLATE_INVOKE(id, ...)                                                 \
-    DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(id, DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_), std::tuple<__VA_ARGS__>) \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(id, DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_), std::tuple<__VA_ARGS__>) \
+    static_assert(true, "")
 
 #define DOCTEST_TEST_CASE_TEMPLATE_APPLY(id, ...)                                                  \
-    DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(id, DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_), __VA_ARGS__) \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(id, DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_), __VA_ARGS__) \
+    static_assert(true, "")
 
 #define DOCTEST_TEST_CASE_TEMPLATE_IMPL(dec, T, anon, ...)                                         \
     DOCTEST_TEST_CASE_TEMPLATE_DEFINE_IMPL(dec, T, DOCTEST_CAT(anon, ITERATOR), anon);             \
     DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE_IMPL(anon, anon, std::tuple<__VA_ARGS__>)               \
     template <typename T>                                                                          \
     static void anon()
 
 #define DOCTEST_TEST_CASE_TEMPLATE(dec, T, ...)                                                    \
-    DOCTEST_TEST_CASE_TEMPLATE_IMPL(dec, T, DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_), __VA_ARGS__)
+    DOCTEST_TEST_CASE_TEMPLATE_IMPL(dec, T, DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_), __VA_ARGS__)
 
 // for subcases
 #define DOCTEST_SUBCASE(name)                                                                      \
-    if(const doctest::detail::Subcase & DOCTEST_ANONYMOUS(_DOCTEST_ANON_SUBCASE_) DOCTEST_UNUSED = \
+    if(const doctest::detail::Subcase & DOCTEST_ANONYMOUS(DOCTEST_ANON_SUBCASE_) DOCTEST_UNUSED =  \
                doctest::detail::Subcase(name, __FILE__, __LINE__))
 
 // for grouping tests in test suites by using code blocks
 #define DOCTEST_TEST_SUITE_IMPL(decorators, ns_name)                                               \
     namespace ns_name { namespace doctest_detail_test_suite_ns {                                   \
-            static DOCTEST_NOINLINE doctest::detail::TestSuite& getCurrentTestSuite() {            \
+            static DOCTEST_NOINLINE doctest::detail::TestSuite& getCurrentTestSuite() noexcept {   \
                 DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4640)                                      \
                 DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wexit-time-destructors")                \
-                static doctest::detail::TestSuite data;                                            \
+                DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wmissing-field-initializers")             \
+                static doctest::detail::TestSuite data{};                                          \
                 static bool                       inited = false;                                  \
                 DOCTEST_MSVC_SUPPRESS_WARNING_POP                                                  \
                 DOCTEST_CLANG_SUPPRESS_WARNING_POP                                                 \
+                DOCTEST_GCC_SUPPRESS_WARNING_POP                                                   \
                 if(!inited) {                                                                      \
                     data* decorators;                                                              \
                     inited = true;                                                                 \
                 }                                                                                  \
                 return data;                                                                       \
             }                                                                                      \
         }                                                                                          \
     }                                                                                              \
     namespace ns_name
 
 #define DOCTEST_TEST_SUITE(decorators)                                                             \
-    DOCTEST_TEST_SUITE_IMPL(decorators, DOCTEST_ANONYMOUS(_DOCTEST_ANON_SUITE_))
+    DOCTEST_TEST_SUITE_IMPL(decorators, DOCTEST_ANONYMOUS(DOCTEST_ANON_SUITE_))
 
 // for starting a testsuite block
 #define DOCTEST_TEST_SUITE_BEGIN(decorators)                                                       \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_VAR_)) =                            \
-            doctest::detail::setTestSuite(doctest::detail::TestSuite() * decorators);              \
-    DOCTEST_GLOBAL_NO_WARNINGS_END()                                                               \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_VAR_), /* NOLINT(cert-err58-cpp) */  \
+            doctest::detail::setTestSuite(doctest::detail::TestSuite() * decorators))              \
+    static_assert(true, "")
 
 // for ending a testsuite block
 #define DOCTEST_TEST_SUITE_END                                                                     \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_VAR_)) =                            \
-            doctest::detail::setTestSuite(doctest::detail::TestSuite() * "");                      \
-    DOCTEST_GLOBAL_NO_WARNINGS_END()                                                               \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_VAR_), /* NOLINT(cert-err58-cpp) */  \
+            doctest::detail::setTestSuite(doctest::detail::TestSuite() * ""))                      \
+    using DOCTEST_ANONYMOUS(DOCTEST_ANON_FOR_SEMICOLON_) = int
 
 // for registering exception translators
 #define DOCTEST_REGISTER_EXCEPTION_TRANSLATOR_IMPL(translatorName, signature)                      \
     inline doctest::String translatorName(signature);                                              \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_TRANSLATOR_)) =                     \
-            doctest::registerExceptionTranslator(translatorName);                                  \
-    DOCTEST_GLOBAL_NO_WARNINGS_END()                                                               \
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_TRANSLATOR_), /* NOLINT(cert-err58-cpp) */ \
+            doctest::registerExceptionTranslator(translatorName))                                  \
     doctest::String translatorName(signature)
 
 #define DOCTEST_REGISTER_EXCEPTION_TRANSLATOR(signature)                                           \
-    DOCTEST_REGISTER_EXCEPTION_TRANSLATOR_IMPL(DOCTEST_ANONYMOUS(_DOCTEST_ANON_TRANSLATOR_),       \
+    DOCTEST_REGISTER_EXCEPTION_TRANSLATOR_IMPL(DOCTEST_ANONYMOUS(DOCTEST_ANON_TRANSLATOR_),        \
                                                signature)
 
 // for registering reporters
 #define DOCTEST_REGISTER_REPORTER(name, priority, reporter)                                        \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_REPORTER_)) =                       \
-            doctest::registerReporter<reporter>(name, priority, true);                             \
-    DOCTEST_GLOBAL_NO_WARNINGS_END() typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_REPORTER_), /* NOLINT(cert-err58-cpp) */ \
+            doctest::registerReporter<reporter>(name, priority, true))                             \
+    static_assert(true, "")
 
 // for registering listeners
 #define DOCTEST_REGISTER_LISTENER(name, priority, reporter)                                        \
-    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(_DOCTEST_ANON_REPORTER_)) =                       \
-            doctest::registerReporter<reporter>(name, priority, false);                            \
-    DOCTEST_GLOBAL_NO_WARNINGS_END() typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
-
-// for logging
-#define DOCTEST_INFO(expression)                                                                   \
-    DOCTEST_INFO_IMPL(DOCTEST_ANONYMOUS(_DOCTEST_CAPTURE_), DOCTEST_ANONYMOUS(_DOCTEST_CAPTURE_),  \
-                      DOCTEST_ANONYMOUS(_DOCTEST_CAPTURE_), expression)
-
-#define DOCTEST_INFO_IMPL(lambda_name, mb_name, s_name, expression)                                \
-    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4626)                                                  \
-    auto lambda_name = [&](std::ostream* s_name) {                                                 \
+    DOCTEST_GLOBAL_NO_WARNINGS(DOCTEST_ANONYMOUS(DOCTEST_ANON_REPORTER_), /* NOLINT(cert-err58-cpp) */ \
+            doctest::registerReporter<reporter>(name, priority, false))                            \
+    static_assert(true, "")
+
+// clang-format off
+// for logging - disabling formatting because it's important to have these on 2 separate lines - see PR #557
+#define DOCTEST_INFO(...)                                                                          \
+    DOCTEST_INFO_IMPL(DOCTEST_ANONYMOUS(DOCTEST_CAPTURE_),                                         \
+                      DOCTEST_ANONYMOUS(DOCTEST_CAPTURE_OTHER_),                                   \
+                      __VA_ARGS__)
+// clang-format on
+
+#define DOCTEST_INFO_IMPL(mb_name, s_name, ...)                                       \
+    auto DOCTEST_ANONYMOUS(DOCTEST_CAPTURE_) = doctest::detail::MakeContextScope(                  \
+        [&](std::ostream* s_name) {                                                                \
         doctest::detail::MessageBuilder mb_name(__FILE__, __LINE__, doctest::assertType::is_warn); \
         mb_name.m_stream = s_name;                                                                 \
-        mb_name << expression;                                                                     \
-    };                                                                                             \
-    DOCTEST_MSVC_SUPPRESS_WARNING_POP                                                              \
-    auto DOCTEST_ANONYMOUS(_DOCTEST_CAPTURE_) = doctest::detail::MakeContextScope(lambda_name)
+        mb_name * __VA_ARGS__;                                                                     \
+    })
 
-#define DOCTEST_CAPTURE(x) DOCTEST_INFO(#x " := " << x)
+#define DOCTEST_CAPTURE(x) DOCTEST_INFO(#x " := ", x)
 
-#define DOCTEST_ADD_AT_IMPL(type, file, line, mb, x)                                               \
-    do {                                                                                           \
+#define DOCTEST_ADD_AT_IMPL(type, file, line, mb, ...)                                             \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
         doctest::detail::MessageBuilder mb(file, line, doctest::assertType::type);                 \
-        mb << x;                                                                                   \
-        DOCTEST_ASSERT_LOG_AND_REACT(mb);                                                          \
-    } while(false)
+        mb * __VA_ARGS__;                                                                          \
+        if(mb.log())                                                                               \
+            DOCTEST_BREAK_INTO_DEBUGGER();                                                         \
+        mb.react();                                                                                \
+    } DOCTEST_FUNC_SCOPE_END
 
 // clang-format off
-#define DOCTEST_ADD_MESSAGE_AT(file, line, x) DOCTEST_ADD_AT_IMPL(is_warn, file, line, DOCTEST_ANONYMOUS(_DOCTEST_MESSAGE_), x)
-#define DOCTEST_ADD_FAIL_CHECK_AT(file, line, x) DOCTEST_ADD_AT_IMPL(is_check, file, line, DOCTEST_ANONYMOUS(_DOCTEST_MESSAGE_), x)
-#define DOCTEST_ADD_FAIL_AT(file, line, x) DOCTEST_ADD_AT_IMPL(is_require, file, line, DOCTEST_ANONYMOUS(_DOCTEST_MESSAGE_), x)
+#define DOCTEST_ADD_MESSAGE_AT(file, line, ...) DOCTEST_ADD_AT_IMPL(is_warn, file, line, DOCTEST_ANONYMOUS(DOCTEST_MESSAGE_), __VA_ARGS__)
+#define DOCTEST_ADD_FAIL_CHECK_AT(file, line, ...) DOCTEST_ADD_AT_IMPL(is_check, file, line, DOCTEST_ANONYMOUS(DOCTEST_MESSAGE_), __VA_ARGS__)
+#define DOCTEST_ADD_FAIL_AT(file, line, ...) DOCTEST_ADD_AT_IMPL(is_require, file, line, DOCTEST_ANONYMOUS(DOCTEST_MESSAGE_), __VA_ARGS__)
 // clang-format on
 
-#define DOCTEST_MESSAGE(x) DOCTEST_ADD_MESSAGE_AT(__FILE__, __LINE__, x)
-#define DOCTEST_FAIL_CHECK(x) DOCTEST_ADD_FAIL_CHECK_AT(__FILE__, __LINE__, x)
-#define DOCTEST_FAIL(x) DOCTEST_ADD_FAIL_AT(__FILE__, __LINE__, x)
+#define DOCTEST_MESSAGE(...) DOCTEST_ADD_MESSAGE_AT(__FILE__, __LINE__, __VA_ARGS__)
+#define DOCTEST_FAIL_CHECK(...) DOCTEST_ADD_FAIL_CHECK_AT(__FILE__, __LINE__, __VA_ARGS__)
+#define DOCTEST_FAIL(...) DOCTEST_ADD_FAIL_AT(__FILE__, __LINE__, __VA_ARGS__)
 
 #define DOCTEST_TO_LVALUE(...) __VA_ARGS__ // Not removed to keep backwards compatibility.
 
 #ifndef DOCTEST_CONFIG_SUPER_FAST_ASSERTS
 
 #define DOCTEST_ASSERT_IMPLEMENT_2(assert_type, ...)                                               \
     DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Woverloaded-shift-op-parentheses")                  \
-    doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__,         \
+    /* NOLINTNEXTLINE(clang-analyzer-cplusplus.NewDeleteLeaks) */                                  \
+    doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,          \
                                                __LINE__, #__VA_ARGS__);                            \
-    DOCTEST_WRAP_IN_TRY(_DOCTEST_RB.setResult(                                                     \
+    DOCTEST_WRAP_IN_TRY(DOCTEST_RB.setResult(                                                      \
             doctest::detail::ExpressionDecomposer(doctest::assertType::assert_type)                \
-            << __VA_ARGS__))                                                                       \
-    DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB)                                                      \
+            << __VA_ARGS__)) /* NOLINTNEXTLINE(clang-analyzer-cplusplus.NewDeleteLeaks) */         \
+    DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB)                                                    \
     DOCTEST_CLANG_SUPPRESS_WARNING_POP
 
 #define DOCTEST_ASSERT_IMPLEMENT_1(assert_type, ...)                                               \
-    do {                                                                                           \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
         DOCTEST_ASSERT_IMPLEMENT_2(assert_type, __VA_ARGS__);                                      \
-    } while(false)
+    } DOCTEST_FUNC_SCOPE_END // NOLINT(clang-analyzer-cplusplus.NewDeleteLeaks)
+
+#define DOCTEST_BINARY_ASSERT(assert_type, comp, ...)                                              \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
+        doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,      \
+                                                   __LINE__, #__VA_ARGS__);                        \
+        DOCTEST_WRAP_IN_TRY(                                                                       \
+                DOCTEST_RB.binary_assert<doctest::detail::binaryAssertComparison::comp>(           \
+                        __VA_ARGS__))                                                              \
+        DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB);                                               \
+    } DOCTEST_FUNC_SCOPE_END
+
+#define DOCTEST_UNARY_ASSERT(assert_type, ...)                                                     \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
+        doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,      \
+                                                   __LINE__, #__VA_ARGS__);                        \
+        DOCTEST_WRAP_IN_TRY(DOCTEST_RB.unary_assert(__VA_ARGS__))                                  \
+        DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB);                                               \
+    } DOCTEST_FUNC_SCOPE_END
 
 #else // DOCTEST_CONFIG_SUPER_FAST_ASSERTS
 
 // necessary for <ASSERT>_MESSAGE
 #define DOCTEST_ASSERT_IMPLEMENT_2 DOCTEST_ASSERT_IMPLEMENT_1
 
 #define DOCTEST_ASSERT_IMPLEMENT_1(assert_type, ...)                                               \
     DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Woverloaded-shift-op-parentheses")                  \
     doctest::detail::decomp_assert(                                                                \
             doctest::assertType::assert_type, __FILE__, __LINE__, #__VA_ARGS__,                    \
             doctest::detail::ExpressionDecomposer(doctest::assertType::assert_type)                \
                     << __VA_ARGS__) DOCTEST_CLANG_SUPPRESS_WARNING_POP
 
+#define DOCTEST_BINARY_ASSERT(assert_type, comparison, ...)                                        \
+    doctest::detail::binary_assert<doctest::detail::binaryAssertComparison::comparison>(           \
+            doctest::assertType::assert_type, __FILE__, __LINE__, #__VA_ARGS__, __VA_ARGS__)
+
+#define DOCTEST_UNARY_ASSERT(assert_type, ...)                                                     \
+    doctest::detail::unary_assert(doctest::assertType::assert_type, __FILE__, __LINE__,            \
+                                  #__VA_ARGS__, __VA_ARGS__)
+
 #endif // DOCTEST_CONFIG_SUPER_FAST_ASSERTS
 
 #define DOCTEST_WARN(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_WARN, __VA_ARGS__)
 #define DOCTEST_CHECK(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_CHECK, __VA_ARGS__)
 #define DOCTEST_REQUIRE(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_REQUIRE, __VA_ARGS__)
 #define DOCTEST_WARN_FALSE(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_WARN_FALSE, __VA_ARGS__)
 #define DOCTEST_CHECK_FALSE(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_CHECK_FALSE, __VA_ARGS__)
 #define DOCTEST_REQUIRE_FALSE(...) DOCTEST_ASSERT_IMPLEMENT_1(DT_REQUIRE_FALSE, __VA_ARGS__)
 
 // clang-format off
-#define DOCTEST_WARN_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_WARN, cond); } while(false)
-#define DOCTEST_CHECK_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_CHECK, cond); } while(false)
-#define DOCTEST_REQUIRE_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_REQUIRE, cond); } while(false)
-#define DOCTEST_WARN_FALSE_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_WARN_FALSE, cond); } while(false)
-#define DOCTEST_CHECK_FALSE_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_CHECK_FALSE, cond); } while(false)
-#define DOCTEST_REQUIRE_FALSE_MESSAGE(cond, msg) do { DOCTEST_INFO(msg); DOCTEST_ASSERT_IMPLEMENT_2(DT_REQUIRE_FALSE, cond); } while(false)
+#define DOCTEST_WARN_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_WARN, cond); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_CHECK, cond); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_REQUIRE, cond); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_WARN_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_WARN_FALSE, cond); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_CHECK_FALSE, cond); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_ASSERT_IMPLEMENT_2(DT_REQUIRE_FALSE, cond); } DOCTEST_FUNC_SCOPE_END
 // clang-format on
 
+#define DOCTEST_WARN_EQ(...) DOCTEST_BINARY_ASSERT(DT_WARN_EQ, eq, __VA_ARGS__)
+#define DOCTEST_CHECK_EQ(...) DOCTEST_BINARY_ASSERT(DT_CHECK_EQ, eq, __VA_ARGS__)
+#define DOCTEST_REQUIRE_EQ(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_EQ, eq, __VA_ARGS__)
+#define DOCTEST_WARN_NE(...) DOCTEST_BINARY_ASSERT(DT_WARN_NE, ne, __VA_ARGS__)
+#define DOCTEST_CHECK_NE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_NE, ne, __VA_ARGS__)
+#define DOCTEST_REQUIRE_NE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_NE, ne, __VA_ARGS__)
+#define DOCTEST_WARN_GT(...) DOCTEST_BINARY_ASSERT(DT_WARN_GT, gt, __VA_ARGS__)
+#define DOCTEST_CHECK_GT(...) DOCTEST_BINARY_ASSERT(DT_CHECK_GT, gt, __VA_ARGS__)
+#define DOCTEST_REQUIRE_GT(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_GT, gt, __VA_ARGS__)
+#define DOCTEST_WARN_LT(...) DOCTEST_BINARY_ASSERT(DT_WARN_LT, lt, __VA_ARGS__)
+#define DOCTEST_CHECK_LT(...) DOCTEST_BINARY_ASSERT(DT_CHECK_LT, lt, __VA_ARGS__)
+#define DOCTEST_REQUIRE_LT(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_LT, lt, __VA_ARGS__)
+#define DOCTEST_WARN_GE(...) DOCTEST_BINARY_ASSERT(DT_WARN_GE, ge, __VA_ARGS__)
+#define DOCTEST_CHECK_GE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_GE, ge, __VA_ARGS__)
+#define DOCTEST_REQUIRE_GE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_GE, ge, __VA_ARGS__)
+#define DOCTEST_WARN_LE(...) DOCTEST_BINARY_ASSERT(DT_WARN_LE, le, __VA_ARGS__)
+#define DOCTEST_CHECK_LE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_LE, le, __VA_ARGS__)
+#define DOCTEST_REQUIRE_LE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_LE, le, __VA_ARGS__)
+
+#define DOCTEST_WARN_UNARY(...) DOCTEST_UNARY_ASSERT(DT_WARN_UNARY, __VA_ARGS__)
+#define DOCTEST_CHECK_UNARY(...) DOCTEST_UNARY_ASSERT(DT_CHECK_UNARY, __VA_ARGS__)
+#define DOCTEST_REQUIRE_UNARY(...) DOCTEST_UNARY_ASSERT(DT_REQUIRE_UNARY, __VA_ARGS__)
+#define DOCTEST_WARN_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_WARN_UNARY_FALSE, __VA_ARGS__)
+#define DOCTEST_CHECK_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_CHECK_UNARY_FALSE, __VA_ARGS__)
+#define DOCTEST_REQUIRE_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_REQUIRE_UNARY_FALSE, __VA_ARGS__)
+
+#ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
+
 #define DOCTEST_ASSERT_THROWS_AS(expr, assert_type, message, ...)                                  \
-    do {                                                                                           \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
         if(!doctest::getContextOptions()->no_throw) {                                              \
-            doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__, \
+            doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,  \
                                                        __LINE__, #expr, #__VA_ARGS__, message);    \
             try {                                                                                  \
                 DOCTEST_CAST_TO_VOID(expr)                                                         \
-            } catch(const doctest::detail::remove_const<                                           \
-                    doctest::detail::remove_reference<__VA_ARGS__>::type>::type&) {                \
-                _DOCTEST_RB.translateException();                                                  \
-                _DOCTEST_RB.m_threw_as = true;                                                     \
-            } catch(...) { _DOCTEST_RB.translateException(); }                                     \
-            DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB);                                             \
+            } catch(const typename doctest::detail::types::remove_const<                           \
+                    typename doctest::detail::types::remove_reference<__VA_ARGS__>::type>::type&) {\
+                DOCTEST_RB.translateException();                                                   \
+                DOCTEST_RB.m_threw_as = true;                                                      \
+            } catch(...) { DOCTEST_RB.translateException(); }                                      \
+            DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB);                                           \
+        } else { /* NOLINT(*-else-after-return) */                                                 \
+            DOCTEST_FUNC_SCOPE_RET(false);                                                         \
         }                                                                                          \
-    } while(false)
+    } DOCTEST_FUNC_SCOPE_END
 
 #define DOCTEST_ASSERT_THROWS_WITH(expr, expr_str, assert_type, ...)                               \
-    do {                                                                                           \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
         if(!doctest::getContextOptions()->no_throw) {                                              \
-            doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__, \
+            doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,  \
                                                        __LINE__, expr_str, "", __VA_ARGS__);       \
             try {                                                                                  \
                 DOCTEST_CAST_TO_VOID(expr)                                                         \
-            } catch(...) { _DOCTEST_RB.translateException(); }                                     \
-            DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB);                                             \
+            } catch(...) { DOCTEST_RB.translateException(); }                                      \
+            DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB);                                           \
+        } else { /* NOLINT(*-else-after-return) */                                                 \
+           DOCTEST_FUNC_SCOPE_RET(false);                                                          \
         }                                                                                          \
-    } while(false)
+    } DOCTEST_FUNC_SCOPE_END
 
 #define DOCTEST_ASSERT_NOTHROW(assert_type, ...)                                                   \
-    do {                                                                                           \
-        doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__,     \
+    DOCTEST_FUNC_SCOPE_BEGIN {                                                                     \
+        doctest::detail::ResultBuilder DOCTEST_RB(doctest::assertType::assert_type, __FILE__,      \
                                                    __LINE__, #__VA_ARGS__);                        \
         try {                                                                                      \
             DOCTEST_CAST_TO_VOID(__VA_ARGS__)                                                      \
-        } catch(...) { _DOCTEST_RB.translateException(); }                                         \
-        DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB);                                                 \
-    } while(false)
+        } catch(...) { DOCTEST_RB.translateException(); }                                          \
+        DOCTEST_ASSERT_LOG_REACT_RETURN(DOCTEST_RB);                                               \
+    } DOCTEST_FUNC_SCOPE_END
 
 // clang-format off
 #define DOCTEST_WARN_THROWS(...) DOCTEST_ASSERT_THROWS_WITH((__VA_ARGS__), #__VA_ARGS__, DT_WARN_THROWS, "")
 #define DOCTEST_CHECK_THROWS(...) DOCTEST_ASSERT_THROWS_WITH((__VA_ARGS__), #__VA_ARGS__, DT_CHECK_THROWS, "")
 #define DOCTEST_REQUIRE_THROWS(...) DOCTEST_ASSERT_THROWS_WITH((__VA_ARGS__), #__VA_ARGS__, DT_REQUIRE_THROWS, "")
 
 #define DOCTEST_WARN_THROWS_AS(expr, ...) DOCTEST_ASSERT_THROWS_AS(expr, DT_WARN_THROWS_AS, "", __VA_ARGS__)
@@ -2077,329 +2541,356 @@
 #define DOCTEST_CHECK_THROWS_WITH_AS(expr, message, ...) DOCTEST_ASSERT_THROWS_AS(expr, DT_CHECK_THROWS_WITH_AS, message, __VA_ARGS__)
 #define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, message, ...) DOCTEST_ASSERT_THROWS_AS(expr, DT_REQUIRE_THROWS_WITH_AS, message, __VA_ARGS__)
 
 #define DOCTEST_WARN_NOTHROW(...) DOCTEST_ASSERT_NOTHROW(DT_WARN_NOTHROW, __VA_ARGS__)
 #define DOCTEST_CHECK_NOTHROW(...) DOCTEST_ASSERT_NOTHROW(DT_CHECK_NOTHROW, __VA_ARGS__)
 #define DOCTEST_REQUIRE_NOTHROW(...) DOCTEST_ASSERT_NOTHROW(DT_REQUIRE_NOTHROW, __VA_ARGS__)
 
-#define DOCTEST_WARN_THROWS_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_WARN_THROWS(expr); } while(false)
-#define DOCTEST_CHECK_THROWS_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_CHECK_THROWS(expr); } while(false)
-#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_REQUIRE_THROWS(expr); } while(false)
-#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_WARN_THROWS_AS(expr, ex); } while(false)
-#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_CHECK_THROWS_AS(expr, ex); } while(false)
-#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_REQUIRE_THROWS_AS(expr, ex); } while(false)
-#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, msg) do { DOCTEST_INFO(msg); DOCTEST_WARN_THROWS_WITH(expr, with); } while(false)
-#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, msg) do { DOCTEST_INFO(msg); DOCTEST_CHECK_THROWS_WITH(expr, with); } while(false)
-#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, msg) do { DOCTEST_INFO(msg); DOCTEST_REQUIRE_THROWS_WITH(expr, with); } while(false)
-#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_WARN_THROWS_WITH_AS(expr, with, ex); } while(false)
-#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ex); } while(false)
-#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) do { DOCTEST_INFO(msg); DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ex); } while(false)
-#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_WARN_NOTHROW(expr); } while(false)
-#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_CHECK_NOTHROW(expr); } while(false)
-#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, msg) do { DOCTEST_INFO(msg); DOCTEST_REQUIRE_NOTHROW(expr); } while(false)
+#define DOCTEST_WARN_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_WARN_THROWS(expr); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_CHECK_THROWS(expr); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_REQUIRE_THROWS(expr); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_WARN_THROWS_AS(expr, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_CHECK_THROWS_AS(expr, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_REQUIRE_THROWS_AS(expr, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_WARN_THROWS_WITH(expr, with); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_CHECK_THROWS_WITH(expr, with); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_REQUIRE_THROWS_WITH(expr, with); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_WARN_THROWS_WITH_AS(expr, with, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ex); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_WARN_NOTHROW(expr); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_CHECK_NOTHROW(expr); } DOCTEST_FUNC_SCOPE_END
+#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_SCOPE_BEGIN { DOCTEST_INFO(__VA_ARGS__); DOCTEST_REQUIRE_NOTHROW(expr); } DOCTEST_FUNC_SCOPE_END
 // clang-format on
 
-#ifndef DOCTEST_CONFIG_SUPER_FAST_ASSERTS
-
-#define DOCTEST_BINARY_ASSERT(assert_type, comp, ...)                                              \
-    do {                                                                                           \
-        doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__,     \
-                                                   __LINE__, #__VA_ARGS__);                        \
-        DOCTEST_WRAP_IN_TRY(                                                                       \
-                _DOCTEST_RB.binary_assert<doctest::detail::binaryAssertComparison::comp>(          \
-                        __VA_ARGS__))                                                              \
-        DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB);                                                 \
-    } while(false)
-
-#define DOCTEST_UNARY_ASSERT(assert_type, ...)                                                     \
-    do {                                                                                           \
-        doctest::detail::ResultBuilder _DOCTEST_RB(doctest::assertType::assert_type, __FILE__,     \
-                                                   __LINE__, #__VA_ARGS__);                        \
-        DOCTEST_WRAP_IN_TRY(_DOCTEST_RB.unary_assert(__VA_ARGS__))                                 \
-        DOCTEST_ASSERT_LOG_AND_REACT(_DOCTEST_RB);                                                 \
-    } while(false)
-
-#else // DOCTEST_CONFIG_SUPER_FAST_ASSERTS
-
-#define DOCTEST_BINARY_ASSERT(assert_type, comparison, ...)                                        \
-    doctest::detail::binary_assert<doctest::detail::binaryAssertComparison::comparison>(           \
-            doctest::assertType::assert_type, __FILE__, __LINE__, #__VA_ARGS__, __VA_ARGS__)
-
-#define DOCTEST_UNARY_ASSERT(assert_type, ...)                                                     \
-    doctest::detail::unary_assert(doctest::assertType::assert_type, __FILE__, __LINE__,            \
-                                  #__VA_ARGS__, __VA_ARGS__)
-
-#endif // DOCTEST_CONFIG_SUPER_FAST_ASSERTS
-
-#define DOCTEST_WARN_EQ(...) DOCTEST_BINARY_ASSERT(DT_WARN_EQ, eq, __VA_ARGS__)
-#define DOCTEST_CHECK_EQ(...) DOCTEST_BINARY_ASSERT(DT_CHECK_EQ, eq, __VA_ARGS__)
-#define DOCTEST_REQUIRE_EQ(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_EQ, eq, __VA_ARGS__)
-#define DOCTEST_WARN_NE(...) DOCTEST_BINARY_ASSERT(DT_WARN_NE, ne, __VA_ARGS__)
-#define DOCTEST_CHECK_NE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_NE, ne, __VA_ARGS__)
-#define DOCTEST_REQUIRE_NE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_NE, ne, __VA_ARGS__)
-#define DOCTEST_WARN_GT(...) DOCTEST_BINARY_ASSERT(DT_WARN_GT, gt, __VA_ARGS__)
-#define DOCTEST_CHECK_GT(...) DOCTEST_BINARY_ASSERT(DT_CHECK_GT, gt, __VA_ARGS__)
-#define DOCTEST_REQUIRE_GT(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_GT, gt, __VA_ARGS__)
-#define DOCTEST_WARN_LT(...) DOCTEST_BINARY_ASSERT(DT_WARN_LT, lt, __VA_ARGS__)
-#define DOCTEST_CHECK_LT(...) DOCTEST_BINARY_ASSERT(DT_CHECK_LT, lt, __VA_ARGS__)
-#define DOCTEST_REQUIRE_LT(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_LT, lt, __VA_ARGS__)
-#define DOCTEST_WARN_GE(...) DOCTEST_BINARY_ASSERT(DT_WARN_GE, ge, __VA_ARGS__)
-#define DOCTEST_CHECK_GE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_GE, ge, __VA_ARGS__)
-#define DOCTEST_REQUIRE_GE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_GE, ge, __VA_ARGS__)
-#define DOCTEST_WARN_LE(...) DOCTEST_BINARY_ASSERT(DT_WARN_LE, le, __VA_ARGS__)
-#define DOCTEST_CHECK_LE(...) DOCTEST_BINARY_ASSERT(DT_CHECK_LE, le, __VA_ARGS__)
-#define DOCTEST_REQUIRE_LE(...) DOCTEST_BINARY_ASSERT(DT_REQUIRE_LE, le, __VA_ARGS__)
-
-#define DOCTEST_WARN_UNARY(...) DOCTEST_UNARY_ASSERT(DT_WARN_UNARY, __VA_ARGS__)
-#define DOCTEST_CHECK_UNARY(...) DOCTEST_UNARY_ASSERT(DT_CHECK_UNARY, __VA_ARGS__)
-#define DOCTEST_REQUIRE_UNARY(...) DOCTEST_UNARY_ASSERT(DT_REQUIRE_UNARY, __VA_ARGS__)
-#define DOCTEST_WARN_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_WARN_UNARY_FALSE, __VA_ARGS__)
-#define DOCTEST_CHECK_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_CHECK_UNARY_FALSE, __VA_ARGS__)
-#define DOCTEST_REQUIRE_UNARY_FALSE(...) DOCTEST_UNARY_ASSERT(DT_REQUIRE_UNARY_FALSE, __VA_ARGS__)
-
-#ifdef DOCTEST_CONFIG_NO_EXCEPTIONS
-
-#undef DOCTEST_WARN_THROWS
-#undef DOCTEST_CHECK_THROWS
-#undef DOCTEST_REQUIRE_THROWS
-#undef DOCTEST_WARN_THROWS_AS
-#undef DOCTEST_CHECK_THROWS_AS
-#undef DOCTEST_REQUIRE_THROWS_AS
-#undef DOCTEST_WARN_THROWS_WITH
-#undef DOCTEST_CHECK_THROWS_WITH
-#undef DOCTEST_REQUIRE_THROWS_WITH
-#undef DOCTEST_WARN_THROWS_WITH_AS
-#undef DOCTEST_CHECK_THROWS_WITH_AS
-#undef DOCTEST_REQUIRE_THROWS_WITH_AS
-#undef DOCTEST_WARN_NOTHROW
-#undef DOCTEST_CHECK_NOTHROW
-#undef DOCTEST_REQUIRE_NOTHROW
-
-#undef DOCTEST_WARN_THROWS_MESSAGE
-#undef DOCTEST_CHECK_THROWS_MESSAGE
-#undef DOCTEST_REQUIRE_THROWS_MESSAGE
-#undef DOCTEST_WARN_THROWS_AS_MESSAGE
-#undef DOCTEST_CHECK_THROWS_AS_MESSAGE
-#undef DOCTEST_REQUIRE_THROWS_AS_MESSAGE
-#undef DOCTEST_WARN_THROWS_WITH_MESSAGE
-#undef DOCTEST_CHECK_THROWS_WITH_MESSAGE
-#undef DOCTEST_REQUIRE_THROWS_WITH_MESSAGE
-#undef DOCTEST_WARN_THROWS_WITH_AS_MESSAGE
-#undef DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE
-#undef DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE
-#undef DOCTEST_WARN_NOTHROW_MESSAGE
-#undef DOCTEST_CHECK_NOTHROW_MESSAGE
-#undef DOCTEST_REQUIRE_NOTHROW_MESSAGE
-
-#ifdef DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
-
-#define DOCTEST_WARN_THROWS(...) ((void)0)
-#define DOCTEST_CHECK_THROWS(...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS(...) ((void)0)
-#define DOCTEST_WARN_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_WARN_NOTHROW(...) ((void)0)
-#define DOCTEST_CHECK_NOTHROW(...) ((void)0)
-#define DOCTEST_REQUIRE_NOTHROW(...) ((void)0)
-
-#define DOCTEST_WARN_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, msg) ((void)0)
-
-#else // DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
-
-#undef DOCTEST_REQUIRE
-#undef DOCTEST_REQUIRE_FALSE
-#undef DOCTEST_REQUIRE_MESSAGE
-#undef DOCTEST_REQUIRE_FALSE_MESSAGE
-#undef DOCTEST_REQUIRE_EQ
-#undef DOCTEST_REQUIRE_NE
-#undef DOCTEST_REQUIRE_GT
-#undef DOCTEST_REQUIRE_LT
-#undef DOCTEST_REQUIRE_GE
-#undef DOCTEST_REQUIRE_LE
-#undef DOCTEST_REQUIRE_UNARY
-#undef DOCTEST_REQUIRE_UNARY_FALSE
-
-#endif // DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
-
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS
 
 // =================================================================================================
 // == WHAT FOLLOWS IS VERSIONS OF THE MACROS THAT DO NOT DO ANY REGISTERING!                      ==
 // == THIS CAN BE ENABLED BY DEFINING DOCTEST_CONFIG_DISABLE GLOBALLY!                            ==
 // =================================================================================================
 #else // DOCTEST_CONFIG_DISABLE
 
 #define DOCTEST_IMPLEMENT_FIXTURE(der, base, func, name)                                           \
-    namespace {                                                                                    \
+    namespace /* NOLINT */ {                                                                       \
         template <typename DOCTEST_UNUSED_TEMPLATE_TYPE>                                           \
         struct der : public base                                                                   \
         { void f(); };                                                                             \
     }                                                                                              \
     template <typename DOCTEST_UNUSED_TEMPLATE_TYPE>                                               \
     inline void der<DOCTEST_UNUSED_TEMPLATE_TYPE>::f()
 
 #define DOCTEST_CREATE_AND_REGISTER_FUNCTION(f, name)                                              \
     template <typename DOCTEST_UNUSED_TEMPLATE_TYPE>                                               \
     static inline void f()
 
 // for registering tests
 #define DOCTEST_TEST_CASE(name)                                                                    \
-    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_), name)
+    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_), name)
 
 // for registering tests in classes
 #define DOCTEST_TEST_CASE_CLASS(name)                                                              \
-    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_), name)
+    DOCTEST_CREATE_AND_REGISTER_FUNCTION(DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_), name)
 
 // for registering tests with a fixture
 #define DOCTEST_TEST_CASE_FIXTURE(x, name)                                                         \
-    DOCTEST_IMPLEMENT_FIXTURE(DOCTEST_ANONYMOUS(_DOCTEST_ANON_CLASS_), x,                          \
-                              DOCTEST_ANONYMOUS(_DOCTEST_ANON_FUNC_), name)
+    DOCTEST_IMPLEMENT_FIXTURE(DOCTEST_ANONYMOUS(DOCTEST_ANON_CLASS_), x,                           \
+                              DOCTEST_ANONYMOUS(DOCTEST_ANON_FUNC_), name)
 
 // for converting types to strings without the <typeinfo> header and demangling
-#define DOCTEST_TYPE_TO_STRING(...) typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
-#define DOCTEST_TYPE_TO_STRING_IMPL(...)
+#define DOCTEST_TYPE_TO_STRING_AS(str, ...) static_assert(true, "")
+#define DOCTEST_TYPE_TO_STRING(...) static_assert(true, "")
 
 // for typed tests
 #define DOCTEST_TEST_CASE_TEMPLATE(name, type, ...)                                                \
     template <typename type>                                                                       \
-    inline void DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_)()
+    inline void DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_)()
 
 #define DOCTEST_TEST_CASE_TEMPLATE_DEFINE(name, type, id)                                          \
     template <typename type>                                                                       \
-    inline void DOCTEST_ANONYMOUS(_DOCTEST_ANON_TMP_)()
-
-#define DOCTEST_TEST_CASE_TEMPLATE_INVOKE(id, ...)                                                 \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+    inline void DOCTEST_ANONYMOUS(DOCTEST_ANON_TMP_)()
 
-#define DOCTEST_TEST_CASE_TEMPLATE_APPLY(id, ...)                                                  \
-    typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+#define DOCTEST_TEST_CASE_TEMPLATE_INVOKE(id, ...) static_assert(true, "")
+#define DOCTEST_TEST_CASE_TEMPLATE_APPLY(id, ...) static_assert(true, "")
 
 // for subcases
 #define DOCTEST_SUBCASE(name)
 
 // for a testsuite block
-#define DOCTEST_TEST_SUITE(name) namespace
+#define DOCTEST_TEST_SUITE(name) namespace // NOLINT
 
 // for starting a testsuite block
-#define DOCTEST_TEST_SUITE_BEGIN(name) typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+#define DOCTEST_TEST_SUITE_BEGIN(name) static_assert(true, "")
 
 // for ending a testsuite block
-#define DOCTEST_TEST_SUITE_END typedef int DOCTEST_ANONYMOUS(_DOCTEST_ANON_FOR_SEMICOLON_)
+#define DOCTEST_TEST_SUITE_END using DOCTEST_ANONYMOUS(DOCTEST_ANON_FOR_SEMICOLON_) = int
 
 #define DOCTEST_REGISTER_EXCEPTION_TRANSLATOR(signature)                                           \
     template <typename DOCTEST_UNUSED_TEMPLATE_TYPE>                                               \
-    static inline doctest::String DOCTEST_ANONYMOUS(_DOCTEST_ANON_TRANSLATOR_)(signature)
+    static inline doctest::String DOCTEST_ANONYMOUS(DOCTEST_ANON_TRANSLATOR_)(signature)
 
 #define DOCTEST_REGISTER_REPORTER(name, priority, reporter)
 #define DOCTEST_REGISTER_LISTENER(name, priority, reporter)
 
-#define DOCTEST_INFO(x) ((void)0)
-#define DOCTEST_CAPTURE(x) ((void)0)
-#define DOCTEST_ADD_MESSAGE_AT(file, line, x) ((void)0)
-#define DOCTEST_ADD_FAIL_CHECK_AT(file, line, x) ((void)0)
-#define DOCTEST_ADD_FAIL_AT(file, line, x) ((void)0)
-#define DOCTEST_MESSAGE(x) ((void)0)
-#define DOCTEST_FAIL_CHECK(x) ((void)0)
-#define DOCTEST_FAIL(x) ((void)0)
-
-#define DOCTEST_WARN(...) ((void)0)
-#define DOCTEST_CHECK(...) ((void)0)
-#define DOCTEST_REQUIRE(...) ((void)0)
-#define DOCTEST_WARN_FALSE(...) ((void)0)
-#define DOCTEST_CHECK_FALSE(...) ((void)0)
-#define DOCTEST_REQUIRE_FALSE(...) ((void)0)
-
-#define DOCTEST_WARN_MESSAGE(cond, msg) ((void)0)
-#define DOCTEST_CHECK_MESSAGE(cond, msg) ((void)0)
-#define DOCTEST_REQUIRE_MESSAGE(cond, msg) ((void)0)
-#define DOCTEST_WARN_FALSE_MESSAGE(cond, msg) ((void)0)
-#define DOCTEST_CHECK_FALSE_MESSAGE(cond, msg) ((void)0)
-#define DOCTEST_REQUIRE_FALSE_MESSAGE(cond, msg) ((void)0)
-
-#define DOCTEST_WARN_THROWS(...) ((void)0)
-#define DOCTEST_CHECK_THROWS(...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS(...) ((void)0)
-#define DOCTEST_WARN_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_AS(expr, ...) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH(expr, ...) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ...) ((void)0)
-#define DOCTEST_WARN_NOTHROW(...) ((void)0)
-#define DOCTEST_CHECK_NOTHROW(...) ((void)0)
-#define DOCTEST_REQUIRE_NOTHROW(...) ((void)0)
-
-#define DOCTEST_WARN_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, msg) ((void)0)
-#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, msg) ((void)0)
-#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, msg) ((void)0)
-#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, msg) ((void)0)
-
-#define DOCTEST_WARN_EQ(...) ((void)0)
-#define DOCTEST_CHECK_EQ(...) ((void)0)
-#define DOCTEST_REQUIRE_EQ(...) ((void)0)
-#define DOCTEST_WARN_NE(...) ((void)0)
-#define DOCTEST_CHECK_NE(...) ((void)0)
-#define DOCTEST_REQUIRE_NE(...) ((void)0)
-#define DOCTEST_WARN_GT(...) ((void)0)
-#define DOCTEST_CHECK_GT(...) ((void)0)
-#define DOCTEST_REQUIRE_GT(...) ((void)0)
-#define DOCTEST_WARN_LT(...) ((void)0)
-#define DOCTEST_CHECK_LT(...) ((void)0)
-#define DOCTEST_REQUIRE_LT(...) ((void)0)
-#define DOCTEST_WARN_GE(...) ((void)0)
-#define DOCTEST_CHECK_GE(...) ((void)0)
-#define DOCTEST_REQUIRE_GE(...) ((void)0)
-#define DOCTEST_WARN_LE(...) ((void)0)
-#define DOCTEST_CHECK_LE(...) ((void)0)
-#define DOCTEST_REQUIRE_LE(...) ((void)0)
-
-#define DOCTEST_WARN_UNARY(...) ((void)0)
-#define DOCTEST_CHECK_UNARY(...) ((void)0)
-#define DOCTEST_REQUIRE_UNARY(...) ((void)0)
-#define DOCTEST_WARN_UNARY_FALSE(...) ((void)0)
-#define DOCTEST_CHECK_UNARY_FALSE(...) ((void)0)
-#define DOCTEST_REQUIRE_UNARY_FALSE(...) ((void)0)
+#define DOCTEST_INFO(...) (static_cast<void>(0))
+#define DOCTEST_CAPTURE(x) (static_cast<void>(0))
+#define DOCTEST_ADD_MESSAGE_AT(file, line, ...) (static_cast<void>(0))
+#define DOCTEST_ADD_FAIL_CHECK_AT(file, line, ...) (static_cast<void>(0))
+#define DOCTEST_ADD_FAIL_AT(file, line, ...) (static_cast<void>(0))
+#define DOCTEST_MESSAGE(...) (static_cast<void>(0))
+#define DOCTEST_FAIL_CHECK(...) (static_cast<void>(0))
+#define DOCTEST_FAIL(...) (static_cast<void>(0))
+
+#if defined(DOCTEST_CONFIG_EVALUATE_ASSERTS_EVEN_WHEN_DISABLED)                                    \
+ && defined(DOCTEST_CONFIG_ASSERTS_RETURN_VALUES)
+
+#define DOCTEST_WARN(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_CHECK(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_REQUIRE(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_WARN_FALSE(...) [&] { return !(__VA_ARGS__); }()
+#define DOCTEST_CHECK_FALSE(...) [&] { return !(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_FALSE(...) [&] { return !(__VA_ARGS__); }()
+
+#define DOCTEST_WARN_MESSAGE(cond, ...) [&] { return cond; }()
+#define DOCTEST_CHECK_MESSAGE(cond, ...) [&] { return cond; }()
+#define DOCTEST_REQUIRE_MESSAGE(cond, ...) [&] { return cond; }()
+#define DOCTEST_WARN_FALSE_MESSAGE(cond, ...) [&] { return !(cond); }()
+#define DOCTEST_CHECK_FALSE_MESSAGE(cond, ...) [&] { return !(cond); }()
+#define DOCTEST_REQUIRE_FALSE_MESSAGE(cond, ...) [&] { return !(cond); }()
+
+namespace doctest {
+namespace detail {
+#define DOCTEST_RELATIONAL_OP(name, op)                                                            \
+    template <typename L, typename R>                                                              \
+    bool name(const DOCTEST_REF_WRAP(L) lhs, const DOCTEST_REF_WRAP(R) rhs) { return lhs op rhs; }
+
+    DOCTEST_RELATIONAL_OP(eq, ==)
+    DOCTEST_RELATIONAL_OP(ne, !=)
+    DOCTEST_RELATIONAL_OP(lt, <)
+    DOCTEST_RELATIONAL_OP(gt, >)
+    DOCTEST_RELATIONAL_OP(le, <=)
+    DOCTEST_RELATIONAL_OP(ge, >=)
+} // namespace detail
+} // namespace doctest
+
+#define DOCTEST_WARN_EQ(...) [&] { return doctest::detail::eq(__VA_ARGS__); }()
+#define DOCTEST_CHECK_EQ(...) [&] { return doctest::detail::eq(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_EQ(...) [&] { return doctest::detail::eq(__VA_ARGS__); }()
+#define DOCTEST_WARN_NE(...) [&] { return doctest::detail::ne(__VA_ARGS__); }()
+#define DOCTEST_CHECK_NE(...) [&] { return doctest::detail::ne(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_NE(...) [&] { return doctest::detail::ne(__VA_ARGS__); }()
+#define DOCTEST_WARN_LT(...) [&] { return doctest::detail::lt(__VA_ARGS__); }()
+#define DOCTEST_CHECK_LT(...) [&] { return doctest::detail::lt(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_LT(...) [&] { return doctest::detail::lt(__VA_ARGS__); }()
+#define DOCTEST_WARN_GT(...) [&] { return doctest::detail::gt(__VA_ARGS__); }()
+#define DOCTEST_CHECK_GT(...) [&] { return doctest::detail::gt(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_GT(...) [&] { return doctest::detail::gt(__VA_ARGS__); }()
+#define DOCTEST_WARN_LE(...) [&] { return doctest::detail::le(__VA_ARGS__); }()
+#define DOCTEST_CHECK_LE(...) [&] { return doctest::detail::le(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_LE(...) [&] { return doctest::detail::le(__VA_ARGS__); }()
+#define DOCTEST_WARN_GE(...) [&] { return doctest::detail::ge(__VA_ARGS__); }()
+#define DOCTEST_CHECK_GE(...) [&] { return doctest::detail::ge(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_GE(...) [&] { return doctest::detail::ge(__VA_ARGS__); }()
+#define DOCTEST_WARN_UNARY(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_CHECK_UNARY(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_REQUIRE_UNARY(...) [&] { return __VA_ARGS__; }()
+#define DOCTEST_WARN_UNARY_FALSE(...) [&] { return !(__VA_ARGS__); }()
+#define DOCTEST_CHECK_UNARY_FALSE(...) [&] { return !(__VA_ARGS__); }()
+#define DOCTEST_REQUIRE_UNARY_FALSE(...) [&] { return !(__VA_ARGS__); }()
+
+#ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
+
+#define DOCTEST_WARN_THROWS_WITH(expr, with, ...) [] { static_assert(false, "Exception translation is not available when doctest is disabled."); return false; }()
+#define DOCTEST_CHECK_THROWS_WITH(expr, with, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_REQUIRE_THROWS_WITH(expr, with, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_WARN_THROWS_WITH_AS(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+
+#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH(,,)
+
+#define DOCTEST_WARN_THROWS(...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_CHECK_THROWS(...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_REQUIRE_THROWS(...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_WARN_THROWS_AS(expr, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_CHECK_THROWS_AS(expr, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_REQUIRE_THROWS_AS(expr, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_WARN_NOTHROW(...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+#define DOCTEST_CHECK_NOTHROW(...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+#define DOCTEST_REQUIRE_NOTHROW(...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+
+#define DOCTEST_WARN_THROWS_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_CHECK_THROWS_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return false; } catch (...) { return true; } }()
+#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, ...) [&] { try { expr; } catch (__VA_ARGS__) { return true; } catch (...) { } return false; }()
+#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, ...) [&] { try { __VA_ARGS__; return true; } catch (...) { return false; } }()
+
+#endif // DOCTEST_CONFIG_NO_EXCEPTIONS
+
+#else // DOCTEST_CONFIG_EVALUATE_ASSERTS_EVEN_WHEN_DISABLED
+
+#define DOCTEST_WARN(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_FALSE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_FALSE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_FALSE(...) DOCTEST_FUNC_EMPTY
+
+#define DOCTEST_WARN_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_FALSE_MESSAGE(cond, ...) DOCTEST_FUNC_EMPTY
+
+#define DOCTEST_WARN_EQ(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_EQ(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_EQ(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_NE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_NE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_NE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_GT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_GT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_GT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_LT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_LT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_LT(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_GE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_GE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_GE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_LE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_LE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_LE(...) DOCTEST_FUNC_EMPTY
+
+#define DOCTEST_WARN_UNARY(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_UNARY(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_UNARY(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_UNARY_FALSE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_UNARY_FALSE(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_UNARY_FALSE(...) DOCTEST_FUNC_EMPTY
+
+#ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
+
+#define DOCTEST_WARN_THROWS(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_AS(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_AS(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_AS(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_WITH(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_WITH(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_WITH(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_WITH_AS(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_NOTHROW(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_NOTHROW(...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_NOTHROW(...) DOCTEST_FUNC_EMPTY
+
+#define DOCTEST_WARN_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, ...) DOCTEST_FUNC_EMPTY
+
+#endif // DOCTEST_CONFIG_NO_EXCEPTIONS
+
+#endif // DOCTEST_CONFIG_EVALUATE_ASSERTS_EVEN_WHEN_DISABLED
 
 #endif // DOCTEST_CONFIG_DISABLE
 
+#ifdef DOCTEST_CONFIG_NO_EXCEPTIONS
+
+#ifdef DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
+#define DOCTEST_EXCEPTION_EMPTY_FUNC DOCTEST_FUNC_EMPTY
+#else // DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
+#define DOCTEST_EXCEPTION_EMPTY_FUNC [] { static_assert(false, "Exceptions are disabled! " \
+    "Use DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS if you want to compile with exceptions disabled."); return false; }()
+
+#undef DOCTEST_REQUIRE
+#undef DOCTEST_REQUIRE_FALSE
+#undef DOCTEST_REQUIRE_MESSAGE
+#undef DOCTEST_REQUIRE_FALSE_MESSAGE
+#undef DOCTEST_REQUIRE_EQ
+#undef DOCTEST_REQUIRE_NE
+#undef DOCTEST_REQUIRE_GT
+#undef DOCTEST_REQUIRE_LT
+#undef DOCTEST_REQUIRE_GE
+#undef DOCTEST_REQUIRE_LE
+#undef DOCTEST_REQUIRE_UNARY
+#undef DOCTEST_REQUIRE_UNARY_FALSE
+
+#define DOCTEST_REQUIRE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_FALSE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_MESSAGE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_FALSE_MESSAGE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_EQ DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_NE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_GT DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_LT DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_GE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_LE DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_UNARY DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_UNARY_FALSE DOCTEST_EXCEPTION_EMPTY_FUNC
+
+#endif // DOCTEST_CONFIG_NO_EXCEPTIONS_BUT_WITH_ALL_ASSERTS
+
+#define DOCTEST_WARN_THROWS(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_AS(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_AS(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_AS(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_WITH(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_WITH(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_WITH(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_WITH_AS(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_WITH_AS(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_NOTHROW(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_NOTHROW(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_NOTHROW(...) DOCTEST_EXCEPTION_EMPTY_FUNC
+
+#define DOCTEST_WARN_THROWS_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_WARN_NOTHROW_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_CHECK_NOTHROW_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+#define DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, ...) DOCTEST_EXCEPTION_EMPTY_FUNC
+
+#endif // DOCTEST_CONFIG_NO_EXCEPTIONS
+
 // clang-format off
 // KEPT FOR BACKWARDS COMPATIBILITY - FORWARDING TO THE RIGHT MACROS
 #define DOCTEST_FAST_WARN_EQ             DOCTEST_WARN_EQ
 #define DOCTEST_FAST_CHECK_EQ            DOCTEST_CHECK_EQ
 #define DOCTEST_FAST_REQUIRE_EQ          DOCTEST_REQUIRE_EQ
 #define DOCTEST_FAST_WARN_NE             DOCTEST_WARN_NE
 #define DOCTEST_FAST_CHECK_NE            DOCTEST_CHECK_NE
@@ -2420,15 +2911,15 @@
 #define DOCTEST_FAST_WARN_UNARY          DOCTEST_WARN_UNARY
 #define DOCTEST_FAST_CHECK_UNARY         DOCTEST_CHECK_UNARY
 #define DOCTEST_FAST_REQUIRE_UNARY       DOCTEST_REQUIRE_UNARY
 #define DOCTEST_FAST_WARN_UNARY_FALSE    DOCTEST_WARN_UNARY_FALSE
 #define DOCTEST_FAST_CHECK_UNARY_FALSE   DOCTEST_CHECK_UNARY_FALSE
 #define DOCTEST_FAST_REQUIRE_UNARY_FALSE DOCTEST_REQUIRE_UNARY_FALSE
 
-#define DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE DOCTEST_TEST_CASE_TEMPLATE_INVOKE
+#define DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE(id, ...) DOCTEST_TEST_CASE_TEMPLATE_INVOKE(id,__VA_ARGS__)
 // clang-format on
 
 // BDD style macros
 // clang-format off
 #define DOCTEST_SCENARIO(name) DOCTEST_TEST_CASE("  Scenario: " name)
 #define DOCTEST_SCENARIO_CLASS(name) DOCTEST_TEST_CASE_CLASS("  Scenario: " name)
 #define DOCTEST_SCENARIO_TEMPLATE(name, T, ...)  DOCTEST_TEST_CASE_TEMPLATE("  Scenario: " name, T, __VA_ARGS__)
@@ -2438,184 +2929,165 @@
 #define DOCTEST_WHEN(name)      DOCTEST_SUBCASE("    When: " name)
 #define DOCTEST_AND_WHEN(name)  DOCTEST_SUBCASE("And when: " name)
 #define DOCTEST_THEN(name)      DOCTEST_SUBCASE("    Then: " name)
 #define DOCTEST_AND_THEN(name)  DOCTEST_SUBCASE("     And: " name)
 // clang-format on
 
 // == SHORT VERSIONS OF THE MACROS
-#if !defined(DOCTEST_CONFIG_NO_SHORT_MACRO_NAMES)
+#ifndef DOCTEST_CONFIG_NO_SHORT_MACRO_NAMES
 
-#define TEST_CASE DOCTEST_TEST_CASE
-#define TEST_CASE_CLASS DOCTEST_TEST_CASE_CLASS
-#define TEST_CASE_FIXTURE DOCTEST_TEST_CASE_FIXTURE
-#define TYPE_TO_STRING DOCTEST_TYPE_TO_STRING
-#define TEST_CASE_TEMPLATE DOCTEST_TEST_CASE_TEMPLATE
-#define TEST_CASE_TEMPLATE_DEFINE DOCTEST_TEST_CASE_TEMPLATE_DEFINE
-#define TEST_CASE_TEMPLATE_INVOKE DOCTEST_TEST_CASE_TEMPLATE_INVOKE
-#define TEST_CASE_TEMPLATE_APPLY DOCTEST_TEST_CASE_TEMPLATE_APPLY
-#define SUBCASE DOCTEST_SUBCASE
-#define TEST_SUITE DOCTEST_TEST_SUITE
-#define TEST_SUITE_BEGIN DOCTEST_TEST_SUITE_BEGIN
+#define TEST_CASE(name) DOCTEST_TEST_CASE(name)
+#define TEST_CASE_CLASS(name) DOCTEST_TEST_CASE_CLASS(name)
+#define TEST_CASE_FIXTURE(x, name) DOCTEST_TEST_CASE_FIXTURE(x, name)
+#define TYPE_TO_STRING_AS(str, ...) DOCTEST_TYPE_TO_STRING_AS(str, __VA_ARGS__)
+#define TYPE_TO_STRING(...) DOCTEST_TYPE_TO_STRING(__VA_ARGS__)
+#define TEST_CASE_TEMPLATE(name, T, ...) DOCTEST_TEST_CASE_TEMPLATE(name, T, __VA_ARGS__)
+#define TEST_CASE_TEMPLATE_DEFINE(name, T, id) DOCTEST_TEST_CASE_TEMPLATE_DEFINE(name, T, id)
+#define TEST_CASE_TEMPLATE_INVOKE(id, ...) DOCTEST_TEST_CASE_TEMPLATE_INVOKE(id, __VA_ARGS__)
+#define TEST_CASE_TEMPLATE_APPLY(id, ...) DOCTEST_TEST_CASE_TEMPLATE_APPLY(id, __VA_ARGS__)
+#define SUBCASE(name) DOCTEST_SUBCASE(name)
+#define TEST_SUITE(decorators) DOCTEST_TEST_SUITE(decorators)
+#define TEST_SUITE_BEGIN(name) DOCTEST_TEST_SUITE_BEGIN(name)
 #define TEST_SUITE_END DOCTEST_TEST_SUITE_END
-#define REGISTER_EXCEPTION_TRANSLATOR DOCTEST_REGISTER_EXCEPTION_TRANSLATOR
-#define REGISTER_REPORTER DOCTEST_REGISTER_REPORTER
-#define REGISTER_LISTENER DOCTEST_REGISTER_LISTENER
-#define INFO DOCTEST_INFO
-#define CAPTURE DOCTEST_CAPTURE
-#define ADD_MESSAGE_AT DOCTEST_ADD_MESSAGE_AT
-#define ADD_FAIL_CHECK_AT DOCTEST_ADD_FAIL_CHECK_AT
-#define ADD_FAIL_AT DOCTEST_ADD_FAIL_AT
-#define MESSAGE DOCTEST_MESSAGE
-#define FAIL_CHECK DOCTEST_FAIL_CHECK
-#define FAIL DOCTEST_FAIL
-#define TO_LVALUE DOCTEST_TO_LVALUE
-
-#define WARN DOCTEST_WARN
-#define WARN_FALSE DOCTEST_WARN_FALSE
-#define WARN_THROWS DOCTEST_WARN_THROWS
-#define WARN_THROWS_AS DOCTEST_WARN_THROWS_AS
-#define WARN_THROWS_WITH DOCTEST_WARN_THROWS_WITH
-#define WARN_THROWS_WITH_AS DOCTEST_WARN_THROWS_WITH_AS
-#define WARN_NOTHROW DOCTEST_WARN_NOTHROW
-#define CHECK DOCTEST_CHECK
-#define CHECK_FALSE DOCTEST_CHECK_FALSE
-#define CHECK_THROWS DOCTEST_CHECK_THROWS
-#define CHECK_THROWS_AS DOCTEST_CHECK_THROWS_AS
-#define CHECK_THROWS_WITH DOCTEST_CHECK_THROWS_WITH
-#define CHECK_THROWS_WITH_AS DOCTEST_CHECK_THROWS_WITH_AS
-#define CHECK_NOTHROW DOCTEST_CHECK_NOTHROW
-#define REQUIRE DOCTEST_REQUIRE
-#define REQUIRE_FALSE DOCTEST_REQUIRE_FALSE
-#define REQUIRE_THROWS DOCTEST_REQUIRE_THROWS
-#define REQUIRE_THROWS_AS DOCTEST_REQUIRE_THROWS_AS
-#define REQUIRE_THROWS_WITH DOCTEST_REQUIRE_THROWS_WITH
-#define REQUIRE_THROWS_WITH_AS DOCTEST_REQUIRE_THROWS_WITH_AS
-#define REQUIRE_NOTHROW DOCTEST_REQUIRE_NOTHROW
-
-#define WARN_MESSAGE DOCTEST_WARN_MESSAGE
-#define WARN_FALSE_MESSAGE DOCTEST_WARN_FALSE_MESSAGE
-#define WARN_THROWS_MESSAGE DOCTEST_WARN_THROWS_MESSAGE
-#define WARN_THROWS_AS_MESSAGE DOCTEST_WARN_THROWS_AS_MESSAGE
-#define WARN_THROWS_WITH_MESSAGE DOCTEST_WARN_THROWS_WITH_MESSAGE
-#define WARN_THROWS_WITH_AS_MESSAGE DOCTEST_WARN_THROWS_WITH_AS_MESSAGE
-#define WARN_NOTHROW_MESSAGE DOCTEST_WARN_NOTHROW_MESSAGE
-#define CHECK_MESSAGE DOCTEST_CHECK_MESSAGE
-#define CHECK_FALSE_MESSAGE DOCTEST_CHECK_FALSE_MESSAGE
-#define CHECK_THROWS_MESSAGE DOCTEST_CHECK_THROWS_MESSAGE
-#define CHECK_THROWS_AS_MESSAGE DOCTEST_CHECK_THROWS_AS_MESSAGE
-#define CHECK_THROWS_WITH_MESSAGE DOCTEST_CHECK_THROWS_WITH_MESSAGE
-#define CHECK_THROWS_WITH_AS_MESSAGE DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE
-#define CHECK_NOTHROW_MESSAGE DOCTEST_CHECK_NOTHROW_MESSAGE
-#define REQUIRE_MESSAGE DOCTEST_REQUIRE_MESSAGE
-#define REQUIRE_FALSE_MESSAGE DOCTEST_REQUIRE_FALSE_MESSAGE
-#define REQUIRE_THROWS_MESSAGE DOCTEST_REQUIRE_THROWS_MESSAGE
-#define REQUIRE_THROWS_AS_MESSAGE DOCTEST_REQUIRE_THROWS_AS_MESSAGE
-#define REQUIRE_THROWS_WITH_MESSAGE DOCTEST_REQUIRE_THROWS_WITH_MESSAGE
-#define REQUIRE_THROWS_WITH_AS_MESSAGE DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE
-#define REQUIRE_NOTHROW_MESSAGE DOCTEST_REQUIRE_NOTHROW_MESSAGE
-
-#define SCENARIO DOCTEST_SCENARIO
-#define SCENARIO_CLASS DOCTEST_SCENARIO_CLASS
-#define SCENARIO_TEMPLATE DOCTEST_SCENARIO_TEMPLATE
-#define SCENARIO_TEMPLATE_DEFINE DOCTEST_SCENARIO_TEMPLATE_DEFINE
-#define GIVEN DOCTEST_GIVEN
-#define WHEN DOCTEST_WHEN
-#define AND_WHEN DOCTEST_AND_WHEN
-#define THEN DOCTEST_THEN
-#define AND_THEN DOCTEST_AND_THEN
-
-#define WARN_EQ DOCTEST_WARN_EQ
-#define CHECK_EQ DOCTEST_CHECK_EQ
-#define REQUIRE_EQ DOCTEST_REQUIRE_EQ
-#define WARN_NE DOCTEST_WARN_NE
-#define CHECK_NE DOCTEST_CHECK_NE
-#define REQUIRE_NE DOCTEST_REQUIRE_NE
-#define WARN_GT DOCTEST_WARN_GT
-#define CHECK_GT DOCTEST_CHECK_GT
-#define REQUIRE_GT DOCTEST_REQUIRE_GT
-#define WARN_LT DOCTEST_WARN_LT
-#define CHECK_LT DOCTEST_CHECK_LT
-#define REQUIRE_LT DOCTEST_REQUIRE_LT
-#define WARN_GE DOCTEST_WARN_GE
-#define CHECK_GE DOCTEST_CHECK_GE
-#define REQUIRE_GE DOCTEST_REQUIRE_GE
-#define WARN_LE DOCTEST_WARN_LE
-#define CHECK_LE DOCTEST_CHECK_LE
-#define REQUIRE_LE DOCTEST_REQUIRE_LE
-#define WARN_UNARY DOCTEST_WARN_UNARY
-#define CHECK_UNARY DOCTEST_CHECK_UNARY
-#define REQUIRE_UNARY DOCTEST_REQUIRE_UNARY
-#define WARN_UNARY_FALSE DOCTEST_WARN_UNARY_FALSE
-#define CHECK_UNARY_FALSE DOCTEST_CHECK_UNARY_FALSE
-#define REQUIRE_UNARY_FALSE DOCTEST_REQUIRE_UNARY_FALSE
+#define REGISTER_EXCEPTION_TRANSLATOR(signature) DOCTEST_REGISTER_EXCEPTION_TRANSLATOR(signature)
+#define REGISTER_REPORTER(name, priority, reporter) DOCTEST_REGISTER_REPORTER(name, priority, reporter)
+#define REGISTER_LISTENER(name, priority, reporter) DOCTEST_REGISTER_LISTENER(name, priority, reporter)
+#define INFO(...) DOCTEST_INFO(__VA_ARGS__)
+#define CAPTURE(x) DOCTEST_CAPTURE(x)
+#define ADD_MESSAGE_AT(file, line, ...) DOCTEST_ADD_MESSAGE_AT(file, line, __VA_ARGS__)
+#define ADD_FAIL_CHECK_AT(file, line, ...) DOCTEST_ADD_FAIL_CHECK_AT(file, line, __VA_ARGS__)
+#define ADD_FAIL_AT(file, line, ...) DOCTEST_ADD_FAIL_AT(file, line, __VA_ARGS__)
+#define MESSAGE(...) DOCTEST_MESSAGE(__VA_ARGS__)
+#define FAIL_CHECK(...) DOCTEST_FAIL_CHECK(__VA_ARGS__)
+#define FAIL(...) DOCTEST_FAIL(__VA_ARGS__)
+#define TO_LVALUE(...) DOCTEST_TO_LVALUE(__VA_ARGS__)
+
+#define WARN(...) DOCTEST_WARN(__VA_ARGS__)
+#define WARN_FALSE(...) DOCTEST_WARN_FALSE(__VA_ARGS__)
+#define WARN_THROWS(...) DOCTEST_WARN_THROWS(__VA_ARGS__)
+#define WARN_THROWS_AS(expr, ...) DOCTEST_WARN_THROWS_AS(expr, __VA_ARGS__)
+#define WARN_THROWS_WITH(expr, ...) DOCTEST_WARN_THROWS_WITH(expr, __VA_ARGS__)
+#define WARN_THROWS_WITH_AS(expr, with, ...) DOCTEST_WARN_THROWS_WITH_AS(expr, with, __VA_ARGS__)
+#define WARN_NOTHROW(...) DOCTEST_WARN_NOTHROW(__VA_ARGS__)
+#define CHECK(...) DOCTEST_CHECK(__VA_ARGS__)
+#define CHECK_FALSE(...) DOCTEST_CHECK_FALSE(__VA_ARGS__)
+#define CHECK_THROWS(...) DOCTEST_CHECK_THROWS(__VA_ARGS__)
+#define CHECK_THROWS_AS(expr, ...) DOCTEST_CHECK_THROWS_AS(expr, __VA_ARGS__)
+#define CHECK_THROWS_WITH(expr, ...) DOCTEST_CHECK_THROWS_WITH(expr, __VA_ARGS__)
+#define CHECK_THROWS_WITH_AS(expr, with, ...) DOCTEST_CHECK_THROWS_WITH_AS(expr, with, __VA_ARGS__)
+#define CHECK_NOTHROW(...) DOCTEST_CHECK_NOTHROW(__VA_ARGS__)
+#define REQUIRE(...) DOCTEST_REQUIRE(__VA_ARGS__)
+#define REQUIRE_FALSE(...) DOCTEST_REQUIRE_FALSE(__VA_ARGS__)
+#define REQUIRE_THROWS(...) DOCTEST_REQUIRE_THROWS(__VA_ARGS__)
+#define REQUIRE_THROWS_AS(expr, ...) DOCTEST_REQUIRE_THROWS_AS(expr, __VA_ARGS__)
+#define REQUIRE_THROWS_WITH(expr, ...) DOCTEST_REQUIRE_THROWS_WITH(expr, __VA_ARGS__)
+#define REQUIRE_THROWS_WITH_AS(expr, with, ...) DOCTEST_REQUIRE_THROWS_WITH_AS(expr, with, __VA_ARGS__)
+#define REQUIRE_NOTHROW(...) DOCTEST_REQUIRE_NOTHROW(__VA_ARGS__)
+
+#define WARN_MESSAGE(cond, ...) DOCTEST_WARN_MESSAGE(cond, __VA_ARGS__)
+#define WARN_FALSE_MESSAGE(cond, ...) DOCTEST_WARN_FALSE_MESSAGE(cond, __VA_ARGS__)
+#define WARN_THROWS_MESSAGE(expr, ...) DOCTEST_WARN_THROWS_MESSAGE(expr, __VA_ARGS__)
+#define WARN_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_WARN_THROWS_AS_MESSAGE(expr, ex, __VA_ARGS__)
+#define WARN_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_WARN_THROWS_WITH_MESSAGE(expr, with, __VA_ARGS__)
+#define WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_WARN_THROWS_WITH_AS_MESSAGE(expr, with, ex, __VA_ARGS__)
+#define WARN_NOTHROW_MESSAGE(expr, ...) DOCTEST_WARN_NOTHROW_MESSAGE(expr, __VA_ARGS__)
+#define CHECK_MESSAGE(cond, ...) DOCTEST_CHECK_MESSAGE(cond, __VA_ARGS__)
+#define CHECK_FALSE_MESSAGE(cond, ...) DOCTEST_CHECK_FALSE_MESSAGE(cond, __VA_ARGS__)
+#define CHECK_THROWS_MESSAGE(expr, ...) DOCTEST_CHECK_THROWS_MESSAGE(expr, __VA_ARGS__)
+#define CHECK_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_CHECK_THROWS_AS_MESSAGE(expr, ex, __VA_ARGS__)
+#define CHECK_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_CHECK_THROWS_WITH_MESSAGE(expr, with, __VA_ARGS__)
+#define CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_CHECK_THROWS_WITH_AS_MESSAGE(expr, with, ex, __VA_ARGS__)
+#define CHECK_NOTHROW_MESSAGE(expr, ...) DOCTEST_CHECK_NOTHROW_MESSAGE(expr, __VA_ARGS__)
+#define REQUIRE_MESSAGE(cond, ...) DOCTEST_REQUIRE_MESSAGE(cond, __VA_ARGS__)
+#define REQUIRE_FALSE_MESSAGE(cond, ...) DOCTEST_REQUIRE_FALSE_MESSAGE(cond, __VA_ARGS__)
+#define REQUIRE_THROWS_MESSAGE(expr, ...) DOCTEST_REQUIRE_THROWS_MESSAGE(expr, __VA_ARGS__)
+#define REQUIRE_THROWS_AS_MESSAGE(expr, ex, ...) DOCTEST_REQUIRE_THROWS_AS_MESSAGE(expr, ex, __VA_ARGS__)
+#define REQUIRE_THROWS_WITH_MESSAGE(expr, with, ...) DOCTEST_REQUIRE_THROWS_WITH_MESSAGE(expr, with, __VA_ARGS__)
+#define REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, ...) DOCTEST_REQUIRE_THROWS_WITH_AS_MESSAGE(expr, with, ex, __VA_ARGS__)
+#define REQUIRE_NOTHROW_MESSAGE(expr, ...) DOCTEST_REQUIRE_NOTHROW_MESSAGE(expr, __VA_ARGS__)
+
+#define SCENARIO(name) DOCTEST_SCENARIO(name)
+#define SCENARIO_CLASS(name) DOCTEST_SCENARIO_CLASS(name)
+#define SCENARIO_TEMPLATE(name, T, ...) DOCTEST_SCENARIO_TEMPLATE(name, T, __VA_ARGS__)
+#define SCENARIO_TEMPLATE_DEFINE(name, T, id) DOCTEST_SCENARIO_TEMPLATE_DEFINE(name, T, id)
+#define GIVEN(name) DOCTEST_GIVEN(name)
+#define WHEN(name) DOCTEST_WHEN(name)
+#define AND_WHEN(name) DOCTEST_AND_WHEN(name)
+#define THEN(name) DOCTEST_THEN(name)
+#define AND_THEN(name) DOCTEST_AND_THEN(name)
+
+#define WARN_EQ(...) DOCTEST_WARN_EQ(__VA_ARGS__)
+#define CHECK_EQ(...) DOCTEST_CHECK_EQ(__VA_ARGS__)
+#define REQUIRE_EQ(...) DOCTEST_REQUIRE_EQ(__VA_ARGS__)
+#define WARN_NE(...) DOCTEST_WARN_NE(__VA_ARGS__)
+#define CHECK_NE(...) DOCTEST_CHECK_NE(__VA_ARGS__)
+#define REQUIRE_NE(...) DOCTEST_REQUIRE_NE(__VA_ARGS__)
+#define WARN_GT(...) DOCTEST_WARN_GT(__VA_ARGS__)
+#define CHECK_GT(...) DOCTEST_CHECK_GT(__VA_ARGS__)
+#define REQUIRE_GT(...) DOCTEST_REQUIRE_GT(__VA_ARGS__)
+#define WARN_LT(...) DOCTEST_WARN_LT(__VA_ARGS__)
+#define CHECK_LT(...) DOCTEST_CHECK_LT(__VA_ARGS__)
+#define REQUIRE_LT(...) DOCTEST_REQUIRE_LT(__VA_ARGS__)
+#define WARN_GE(...) DOCTEST_WARN_GE(__VA_ARGS__)
+#define CHECK_GE(...) DOCTEST_CHECK_GE(__VA_ARGS__)
+#define REQUIRE_GE(...) DOCTEST_REQUIRE_GE(__VA_ARGS__)
+#define WARN_LE(...) DOCTEST_WARN_LE(__VA_ARGS__)
+#define CHECK_LE(...) DOCTEST_CHECK_LE(__VA_ARGS__)
+#define REQUIRE_LE(...) DOCTEST_REQUIRE_LE(__VA_ARGS__)
+#define WARN_UNARY(...) DOCTEST_WARN_UNARY(__VA_ARGS__)
+#define CHECK_UNARY(...) DOCTEST_CHECK_UNARY(__VA_ARGS__)
+#define REQUIRE_UNARY(...) DOCTEST_REQUIRE_UNARY(__VA_ARGS__)
+#define WARN_UNARY_FALSE(...) DOCTEST_WARN_UNARY_FALSE(__VA_ARGS__)
+#define CHECK_UNARY_FALSE(...) DOCTEST_CHECK_UNARY_FALSE(__VA_ARGS__)
+#define REQUIRE_UNARY_FALSE(...) DOCTEST_REQUIRE_UNARY_FALSE(__VA_ARGS__)
 
 // KEPT FOR BACKWARDS COMPATIBILITY
-#define FAST_WARN_EQ DOCTEST_FAST_WARN_EQ
-#define FAST_CHECK_EQ DOCTEST_FAST_CHECK_EQ
-#define FAST_REQUIRE_EQ DOCTEST_FAST_REQUIRE_EQ
-#define FAST_WARN_NE DOCTEST_FAST_WARN_NE
-#define FAST_CHECK_NE DOCTEST_FAST_CHECK_NE
-#define FAST_REQUIRE_NE DOCTEST_FAST_REQUIRE_NE
-#define FAST_WARN_GT DOCTEST_FAST_WARN_GT
-#define FAST_CHECK_GT DOCTEST_FAST_CHECK_GT
-#define FAST_REQUIRE_GT DOCTEST_FAST_REQUIRE_GT
-#define FAST_WARN_LT DOCTEST_FAST_WARN_LT
-#define FAST_CHECK_LT DOCTEST_FAST_CHECK_LT
-#define FAST_REQUIRE_LT DOCTEST_FAST_REQUIRE_LT
-#define FAST_WARN_GE DOCTEST_FAST_WARN_GE
-#define FAST_CHECK_GE DOCTEST_FAST_CHECK_GE
-#define FAST_REQUIRE_GE DOCTEST_FAST_REQUIRE_GE
-#define FAST_WARN_LE DOCTEST_FAST_WARN_LE
-#define FAST_CHECK_LE DOCTEST_FAST_CHECK_LE
-#define FAST_REQUIRE_LE DOCTEST_FAST_REQUIRE_LE
-
-#define FAST_WARN_UNARY DOCTEST_FAST_WARN_UNARY
-#define FAST_CHECK_UNARY DOCTEST_FAST_CHECK_UNARY
-#define FAST_REQUIRE_UNARY DOCTEST_FAST_REQUIRE_UNARY
-#define FAST_WARN_UNARY_FALSE DOCTEST_FAST_WARN_UNARY_FALSE
-#define FAST_CHECK_UNARY_FALSE DOCTEST_FAST_CHECK_UNARY_FALSE
-#define FAST_REQUIRE_UNARY_FALSE DOCTEST_FAST_REQUIRE_UNARY_FALSE
+#define FAST_WARN_EQ(...) DOCTEST_FAST_WARN_EQ(__VA_ARGS__)
+#define FAST_CHECK_EQ(...) DOCTEST_FAST_CHECK_EQ(__VA_ARGS__)
+#define FAST_REQUIRE_EQ(...) DOCTEST_FAST_REQUIRE_EQ(__VA_ARGS__)
+#define FAST_WARN_NE(...) DOCTEST_FAST_WARN_NE(__VA_ARGS__)
+#define FAST_CHECK_NE(...) DOCTEST_FAST_CHECK_NE(__VA_ARGS__)
+#define FAST_REQUIRE_NE(...) DOCTEST_FAST_REQUIRE_NE(__VA_ARGS__)
+#define FAST_WARN_GT(...) DOCTEST_FAST_WARN_GT(__VA_ARGS__)
+#define FAST_CHECK_GT(...) DOCTEST_FAST_CHECK_GT(__VA_ARGS__)
+#define FAST_REQUIRE_GT(...) DOCTEST_FAST_REQUIRE_GT(__VA_ARGS__)
+#define FAST_WARN_LT(...) DOCTEST_FAST_WARN_LT(__VA_ARGS__)
+#define FAST_CHECK_LT(...) DOCTEST_FAST_CHECK_LT(__VA_ARGS__)
+#define FAST_REQUIRE_LT(...) DOCTEST_FAST_REQUIRE_LT(__VA_ARGS__)
+#define FAST_WARN_GE(...) DOCTEST_FAST_WARN_GE(__VA_ARGS__)
+#define FAST_CHECK_GE(...) DOCTEST_FAST_CHECK_GE(__VA_ARGS__)
+#define FAST_REQUIRE_GE(...) DOCTEST_FAST_REQUIRE_GE(__VA_ARGS__)
+#define FAST_WARN_LE(...) DOCTEST_FAST_WARN_LE(__VA_ARGS__)
+#define FAST_CHECK_LE(...) DOCTEST_FAST_CHECK_LE(__VA_ARGS__)
+#define FAST_REQUIRE_LE(...) DOCTEST_FAST_REQUIRE_LE(__VA_ARGS__)
+
+#define FAST_WARN_UNARY(...) DOCTEST_FAST_WARN_UNARY(__VA_ARGS__)
+#define FAST_CHECK_UNARY(...) DOCTEST_FAST_CHECK_UNARY(__VA_ARGS__)
+#define FAST_REQUIRE_UNARY(...) DOCTEST_FAST_REQUIRE_UNARY(__VA_ARGS__)
+#define FAST_WARN_UNARY_FALSE(...) DOCTEST_FAST_WARN_UNARY_FALSE(__VA_ARGS__)
+#define FAST_CHECK_UNARY_FALSE(...) DOCTEST_FAST_CHECK_UNARY_FALSE(__VA_ARGS__)
+#define FAST_REQUIRE_UNARY_FALSE(...) DOCTEST_FAST_REQUIRE_UNARY_FALSE(__VA_ARGS__)
 
-#define TEST_CASE_TEMPLATE_INSTANTIATE DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE
+#define TEST_CASE_TEMPLATE_INSTANTIATE(id, ...) DOCTEST_TEST_CASE_TEMPLATE_INSTANTIATE(id, __VA_ARGS__)
 
 #endif // DOCTEST_CONFIG_NO_SHORT_MACRO_NAMES
 
-#if !defined(DOCTEST_CONFIG_DISABLE)
+#ifndef DOCTEST_CONFIG_DISABLE
 
 // this is here to clear the 'current test suite' for the current translation unit - at the top
 DOCTEST_TEST_SUITE_END();
 
-// add stringification for primitive/fundamental types
-namespace doctest { namespace detail {
-    DOCTEST_TYPE_TO_STRING_IMPL(bool)
-    DOCTEST_TYPE_TO_STRING_IMPL(float)
-    DOCTEST_TYPE_TO_STRING_IMPL(double)
-    DOCTEST_TYPE_TO_STRING_IMPL(long double)
-    DOCTEST_TYPE_TO_STRING_IMPL(char)
-    DOCTEST_TYPE_TO_STRING_IMPL(signed char)
-    DOCTEST_TYPE_TO_STRING_IMPL(unsigned char)
-#if !DOCTEST_MSVC || defined(_NATIVE_WCHAR_T_DEFINED)
-    DOCTEST_TYPE_TO_STRING_IMPL(wchar_t)
-#endif // not MSVC or wchar_t support enabled
-    DOCTEST_TYPE_TO_STRING_IMPL(short int)
-    DOCTEST_TYPE_TO_STRING_IMPL(unsigned short int)
-    DOCTEST_TYPE_TO_STRING_IMPL(int)
-    DOCTEST_TYPE_TO_STRING_IMPL(unsigned int)
-    DOCTEST_TYPE_TO_STRING_IMPL(long int)
-    DOCTEST_TYPE_TO_STRING_IMPL(unsigned long int)
-    DOCTEST_TYPE_TO_STRING_IMPL(long long int)
-    DOCTEST_TYPE_TO_STRING_IMPL(unsigned long long int)
-}} // namespace doctest::detail
-
 #endif // DOCTEST_CONFIG_DISABLE
 
 DOCTEST_CLANG_SUPPRESS_WARNING_POP
 DOCTEST_MSVC_SUPPRESS_WARNING_POP
 DOCTEST_GCC_SUPPRESS_WARNING_POP
 
+DOCTEST_SUPPRESS_COMMON_WARNINGS_POP
+
 #endif // DOCTEST_LIBRARY_INCLUDED
 
 #ifndef DOCTEST_SINGLE_HEADER
 #define DOCTEST_SINGLE_HEADER
 #endif // DOCTEST_SINGLE_HEADER
 
 #if defined(DOCTEST_CONFIG_IMPLEMENT) || !defined(DOCTEST_SINGLE_HEADER)
@@ -2627,158 +3099,136 @@
 DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wunused-macros")
 
 #ifndef DOCTEST_LIBRARY_IMPLEMENTATION
 #define DOCTEST_LIBRARY_IMPLEMENTATION
 
 DOCTEST_CLANG_SUPPRESS_WARNING_POP
 
+DOCTEST_SUPPRESS_COMMON_WARNINGS_PUSH
+
 DOCTEST_CLANG_SUPPRESS_WARNING_PUSH
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wunknown-pragmas")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wpadded")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wweak-vtables")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wglobal-constructors")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wexit-time-destructors")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-prototypes")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wsign-conversion")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wshorten-64-to-32")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-variable-declarations")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wswitch")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wswitch-enum")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wcovered-switch-default")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-noreturn")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wunused-local-typedef")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wdisabled-macro-expansion")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-braces")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wmissing-field-initializers")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat")
-DOCTEST_CLANG_SUPPRESS_WARNING("-Wc++98-compat-pedantic")
 DOCTEST_CLANG_SUPPRESS_WARNING("-Wunused-member-function")
+DOCTEST_CLANG_SUPPRESS_WARNING("-Wnonportable-system-include-path")
 
 DOCTEST_GCC_SUPPRESS_WARNING_PUSH
-DOCTEST_GCC_SUPPRESS_WARNING("-Wunknown-pragmas")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wpragmas")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wconversion")
-DOCTEST_GCC_SUPPRESS_WARNING("-Weffc++")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wsign-conversion")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-overflow")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wstrict-aliasing")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wmissing-field-initializers")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wmissing-braces")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wmissing-declarations")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wswitch")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wswitch-enum")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wswitch-default")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wunsafe-loop-optimizations")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wold-style-cast")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wunused-local-typedefs")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wuseless-cast")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wunused-function")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wmultiple-inheritance")
-DOCTEST_GCC_SUPPRESS_WARNING("-Wnoexcept")
 DOCTEST_GCC_SUPPRESS_WARNING("-Wsuggest-attribute")
 
 DOCTEST_MSVC_SUPPRESS_WARNING_PUSH
-DOCTEST_MSVC_SUPPRESS_WARNING(4616) // invalid compiler warning
-DOCTEST_MSVC_SUPPRESS_WARNING(4619) // invalid compiler warning
-DOCTEST_MSVC_SUPPRESS_WARNING(4996) // The compiler encountered a deprecated declaration
 DOCTEST_MSVC_SUPPRESS_WARNING(4267) // 'var' : conversion from 'x' to 'y', possible loss of data
-DOCTEST_MSVC_SUPPRESS_WARNING(4706) // assignment within conditional expression
-DOCTEST_MSVC_SUPPRESS_WARNING(4512) // 'class' : assignment operator could not be generated
-DOCTEST_MSVC_SUPPRESS_WARNING(4127) // conditional expression is constant
 DOCTEST_MSVC_SUPPRESS_WARNING(4530) // C++ exception handler used, but unwind semantics not enabled
 DOCTEST_MSVC_SUPPRESS_WARNING(4577) // 'noexcept' used with no exception handling mode specified
 DOCTEST_MSVC_SUPPRESS_WARNING(4774) // format string expected in argument is not a string literal
 DOCTEST_MSVC_SUPPRESS_WARNING(4365) // conversion from 'int' to 'unsigned', signed/unsigned mismatch
-DOCTEST_MSVC_SUPPRESS_WARNING(4820) // padding in structs
-DOCTEST_MSVC_SUPPRESS_WARNING(4640) // construction of local static object is not thread-safe
 DOCTEST_MSVC_SUPPRESS_WARNING(5039) // pointer to potentially throwing function passed to extern C
-DOCTEST_MSVC_SUPPRESS_WARNING(5045) // Spectre mitigation stuff
-DOCTEST_MSVC_SUPPRESS_WARNING(4626) // assignment operator was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(5027) // move assignment operator was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(5026) // move constructor was implicitly defined as deleted
-DOCTEST_MSVC_SUPPRESS_WARNING(4625) // copy constructor was implicitly defined as deleted
 DOCTEST_MSVC_SUPPRESS_WARNING(4800) // forcing value to bool 'true' or 'false' (performance warning)
-// static analysis
-DOCTEST_MSVC_SUPPRESS_WARNING(26439) // This kind of function may not throw. Declare it 'noexcept'
-DOCTEST_MSVC_SUPPRESS_WARNING(26495) // Always initialize a member variable
-DOCTEST_MSVC_SUPPRESS_WARNING(26451) // Arithmetic overflow ...
-DOCTEST_MSVC_SUPPRESS_WARNING(26444) // Avoid unnamed objects with custom construction and dtor...
-DOCTEST_MSVC_SUPPRESS_WARNING(26812) // Prefer 'enum class' over 'enum'
+DOCTEST_MSVC_SUPPRESS_WARNING(5245) // unreferenced function with internal linkage has been removed
 
 DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_BEGIN
 
 // required includes - will go only in one translation unit!
 #include <ctime>
 #include <cmath>
 #include <climits>
-// borland (Embarcadero) compiler requires math.h and not cmath - https://github.com/onqtam/doctest/pull/37
+// borland (Embarcadero) compiler requires math.h and not cmath - https://github.com/doctest/doctest/pull/37
 #ifdef __BORLANDC__
 #include <math.h>
 #endif // __BORLANDC__
 #include <new>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
 #include <limits>
 #include <utility>
 #include <fstream>
 #include <sstream>
+#ifndef DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
 #include <iostream>
+#endif // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
 #include <algorithm>
 #include <iomanip>
 #include <vector>
+#ifndef DOCTEST_CONFIG_NO_MULTITHREADING
 #include <atomic>
 #include <mutex>
+#define DOCTEST_DECLARE_MUTEX(name) std::mutex name;
+#define DOCTEST_DECLARE_STATIC_MUTEX(name) static DOCTEST_DECLARE_MUTEX(name)
+#define DOCTEST_LOCK_MUTEX(name) std::lock_guard<std::mutex> DOCTEST_ANONYMOUS(DOCTEST_ANON_LOCK_)(name);
+#else // DOCTEST_CONFIG_NO_MULTITHREADING
+#define DOCTEST_DECLARE_MUTEX(name)
+#define DOCTEST_DECLARE_STATIC_MUTEX(name)
+#define DOCTEST_LOCK_MUTEX(name)
+#endif // DOCTEST_CONFIG_NO_MULTITHREADING
 #include <set>
 #include <map>
+#include <unordered_set>
 #include <exception>
 #include <stdexcept>
-#ifdef DOCTEST_CONFIG_POSIX_SIGNALS
 #include <csignal>
-#endif // DOCTEST_CONFIG_POSIX_SIGNALS
 #include <cfloat>
 #include <cctype>
 #include <cstdint>
+#include <string>
 
 #ifdef DOCTEST_PLATFORM_MAC
 #include <sys/types.h>
 #include <unistd.h>
 #include <sys/sysctl.h>
 #endif // DOCTEST_PLATFORM_MAC
 
 #ifdef DOCTEST_PLATFORM_WINDOWS
 
 // defines for a leaner windows.h
 #ifndef WIN32_LEAN_AND_MEAN
 #define WIN32_LEAN_AND_MEAN
+#define DOCTEST_UNDEF_WIN32_LEAN_AND_MEAN
 #endif // WIN32_LEAN_AND_MEAN
 #ifndef NOMINMAX
 #define NOMINMAX
+#define DOCTEST_UNDEF_NOMINMAX
 #endif // NOMINMAX
 
 // not sure what AfxWin.h is for - here I do what Catch does
 #ifdef __AFXDLL
 #include <AfxWin.h>
 #else
-#if defined(__MINGW32__) || defined(__MINGW64__)
 #include <windows.h>
-#else // MINGW
-#include <Windows.h>
-#endif // MINGW
 #endif
 #include <io.h>
 
 #else // DOCTEST_PLATFORM_WINDOWS
 
 #include <sys/time.h>
 #include <unistd.h>
 
 #endif // DOCTEST_PLATFORM_WINDOWS
 
-// this is a fix for https://github.com/onqtam/doctest/issues/348
+// this is a fix for https://github.com/doctest/doctest/issues/348
 // https://mail.gnome.org/archives/xml/2012-January/msg00000.html
 #if !defined(HAVE_UNISTD_H) && !defined(STDOUT_FILENO)
 #define STDOUT_FILENO fileno(stdout)
 #endif // HAVE_UNISTD_H
 
 DOCTEST_MAKE_STD_HEADERS_CLEAN_FROM_WARNINGS_ON_WALL_END
 
@@ -2792,52 +3242,82 @@
 #endif // DOCTEST_CONFIG_DISABLE
 
 #ifndef DOCTEST_CONFIG_OPTIONS_PREFIX
 #define DOCTEST_CONFIG_OPTIONS_PREFIX "dt-"
 #endif
 
 #ifndef DOCTEST_THREAD_LOCAL
+#if defined(DOCTEST_CONFIG_NO_MULTITHREADING) || DOCTEST_MSVC && (DOCTEST_MSVC < DOCTEST_COMPILER(19, 0, 0))
+#define DOCTEST_THREAD_LOCAL
+#else // DOCTEST_MSVC
 #define DOCTEST_THREAD_LOCAL thread_local
+#endif // DOCTEST_MSVC
+#endif // DOCTEST_THREAD_LOCAL
+
+#ifndef DOCTEST_MULTI_LANE_ATOMICS_THREAD_LANES
+#define DOCTEST_MULTI_LANE_ATOMICS_THREAD_LANES 32
+#endif
+
+#ifndef DOCTEST_MULTI_LANE_ATOMICS_CACHE_LINE_SIZE
+#define DOCTEST_MULTI_LANE_ATOMICS_CACHE_LINE_SIZE 64
 #endif
 
 #ifdef DOCTEST_CONFIG_NO_UNPREFIXED_OPTIONS
 #define DOCTEST_OPTIONS_PREFIX_DISPLAY DOCTEST_CONFIG_OPTIONS_PREFIX
 #else
 #define DOCTEST_OPTIONS_PREFIX_DISPLAY ""
 #endif
 
+#if defined(WINAPI_FAMILY) && (WINAPI_FAMILY == WINAPI_FAMILY_APP)
+#define DOCTEST_CONFIG_NO_MULTI_LANE_ATOMICS
+#endif
+
+#ifndef DOCTEST_CDECL
+#define DOCTEST_CDECL __cdecl
+#endif
+
 namespace doctest {
 
 bool is_running_in_test = false;
 
 namespace {
     using namespace detail;
+
+    template <typename Ex>
+    DOCTEST_NORETURN void throw_exception(Ex const& e) {
+#ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
+        throw e;
+#else  // DOCTEST_CONFIG_NO_EXCEPTIONS
+#ifdef DOCTEST_CONFIG_HANDLE_EXCEPTION
+        DOCTEST_CONFIG_HANDLE_EXCEPTION(e);
+#else // DOCTEST_CONFIG_HANDLE_EXCEPTION
+#ifndef DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+        std::cerr << "doctest will terminate because it needed to throw an exception.\n"
+                  << "The message was: " << e.what() << '\n';
+#endif // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+#endif // DOCTEST_CONFIG_HANDLE_EXCEPTION
+        std::terminate();
+#endif // DOCTEST_CONFIG_NO_EXCEPTIONS
+    }
+
+#ifndef DOCTEST_INTERNAL_ERROR
+#define DOCTEST_INTERNAL_ERROR(msg)                                                                \
+    throw_exception(std::logic_error(                                                              \
+            __FILE__ ":" DOCTEST_TOSTR(__LINE__) ": Internal doctest error: " msg))
+#endif // DOCTEST_INTERNAL_ERROR
+
     // case insensitive strcmp
     int stricmp(const char* a, const char* b) {
         for(;; a++, b++) {
             const int d = tolower(*a) - tolower(*b);
             if(d != 0 || !*a)
                 return d;
         }
     }
 
-    template <typename T>
-    String fpToString(T value, int precision) {
-        std::ostringstream oss;
-        oss << std::setprecision(precision) << std::fixed << value;
-        std::string d = oss.str();
-        size_t      i = d.find_last_not_of('0');
-        if(i != std::string::npos && i != d.size() - 1) {
-            if(d[i] == '.')
-                i++;
-            d = d.substr(0, i + 1);
-        }
-        return d.c_str();
-    }
-
     struct Endianness
     {
         enum Arch
         {
             Big,
             Little
         };
@@ -2850,66 +3330,64 @@
                 return Little;
             return Big;
         }
     };
 } // namespace
 
 namespace detail {
-    void my_memcpy(void* dest, const void* src, unsigned num) { memcpy(dest, src, num); }
+    DOCTEST_THREAD_LOCAL class
+    {
+        std::vector<std::streampos> stack;
+        std::stringstream           ss;
 
-    String rawMemoryToString(const void* object, unsigned size) {
-        // Reverse order for little endian architectures
-        int i = 0, end = static_cast<int>(size), inc = 1;
-        if(Endianness::which() == Endianness::Little) {
-            i   = end - 1;
-            end = inc = -1;
+    public:
+        std::ostream* push() {
+            stack.push_back(ss.tellp());
+            return &ss;
         }
 
-        unsigned const char* bytes = static_cast<unsigned const char*>(object);
-        std::ostringstream   oss;
-        oss << "0x" << std::setfill('0') << std::hex;
-        for(; i != end; i += inc)
-            oss << std::setw(2) << static_cast<unsigned>(bytes[i]);
-        return oss.str().c_str();
-    }
+        String pop() {
+            if (stack.empty())
+                DOCTEST_INTERNAL_ERROR("TLSS was empty when trying to pop!");
 
-    DOCTEST_THREAD_LOCAL std::ostringstream g_oss; // NOLINT(cert-err58-cpp)
+            std::streampos pos = stack.back();
+            stack.pop_back();
+            unsigned sz = static_cast<unsigned>(ss.tellp() - pos);
+            ss.rdbuf()->pubseekpos(pos, std::ios::in | std::ios::out);
+            return String(ss, sz);
+        }
+    } g_oss;
 
-    std::ostream* getTlsOss() {
-        g_oss.clear(); // there shouldn't be anything worth clearing in the flags
-        g_oss.str(""); // the slow way of resetting a string stream
-        //g_oss.seekp(0); // optimal reset - as seen here: https://stackoverflow.com/a/624291/3162383
-        return &g_oss;
+    std::ostream* tlssPush() {
+        return g_oss.push();
     }
 
-    String getTlsOssResult() {
-        //g_oss << std::ends; // needed - as shown here: https://stackoverflow.com/a/624291/3162383
-        return g_oss.str().c_str();
+    String tlssPop() {
+        return g_oss.pop();
     }
 
 #ifndef DOCTEST_CONFIG_DISABLE
 
 namespace timer_large_integer
 {
-    
+
 #if defined(DOCTEST_PLATFORM_WINDOWS)
-    typedef ULONGLONG type;
+    using type = ULONGLONG;
 #else // DOCTEST_PLATFORM_WINDOWS
-    using namespace std;
-    typedef uint64_t type;
+    using type = std::uint64_t;
 #endif // DOCTEST_PLATFORM_WINDOWS
 }
 
-typedef timer_large_integer::type ticks_t;
+using ticks_t = timer_large_integer::type;
 
 #ifdef DOCTEST_CONFIG_GETCURRENTTICKS
     ticks_t getCurrentTicks() { return DOCTEST_CONFIG_GETCURRENTTICKS(); }
 #elif defined(DOCTEST_PLATFORM_WINDOWS)
     ticks_t getCurrentTicks() {
-        static LARGE_INTEGER hz = {0}, hzo = {0};
+        static LARGE_INTEGER hz = { {0} }, hzo = { {0} };
         if(!hz.QuadPart) {
             QueryPerformanceFrequency(&hz);
             QueryPerformanceCounter(&hzo);
         }
         LARGE_INTEGER t;
         QueryPerformanceCounter(&t);
         return ((t.QuadPart - hzo.QuadPart) * LONGLONG(1000000)) / hz.QuadPart;
@@ -2933,38 +3411,131 @@
         //}
         double getElapsedSeconds() const { return static_cast<double>(getCurrentTicks() - m_ticks) / 1000000.0; }
 
     private:
         ticks_t m_ticks = 0;
     };
 
+#ifdef DOCTEST_CONFIG_NO_MULTITHREADING
+    template <typename T>
+    using Atomic = T;
+#else // DOCTEST_CONFIG_NO_MULTITHREADING
+    template <typename T>
+    using Atomic = std::atomic<T>;
+#endif // DOCTEST_CONFIG_NO_MULTITHREADING
+
+#if defined(DOCTEST_CONFIG_NO_MULTI_LANE_ATOMICS) || defined(DOCTEST_CONFIG_NO_MULTITHREADING)
+    template <typename T>
+    using MultiLaneAtomic = Atomic<T>;
+#else // DOCTEST_CONFIG_NO_MULTI_LANE_ATOMICS
+    // Provides a multilane implementation of an atomic variable that supports add, sub, load,
+    // store. Instead of using a single atomic variable, this splits up into multiple ones,
+    // each sitting on a separate cache line. The goal is to provide a speedup when most
+    // operations are modifying. It achieves this with two properties:
+    //
+    // * Multiple atomics are used, so chance of congestion from the same atomic is reduced.
+    // * Each atomic sits on a separate cache line, so false sharing is reduced.
+    //
+    // The disadvantage is that there is a small overhead due to the use of TLS, and load/store
+    // is slower because all atomics have to be accessed.
+    template <typename T>
+    class MultiLaneAtomic
+    {
+        struct CacheLineAlignedAtomic
+        {
+            Atomic<T> atomic{};
+            char padding[DOCTEST_MULTI_LANE_ATOMICS_CACHE_LINE_SIZE - sizeof(Atomic<T>)];
+        };
+        CacheLineAlignedAtomic m_atomics[DOCTEST_MULTI_LANE_ATOMICS_THREAD_LANES];
+
+        static_assert(sizeof(CacheLineAlignedAtomic) == DOCTEST_MULTI_LANE_ATOMICS_CACHE_LINE_SIZE,
+                      "guarantee one atomic takes exactly one cache line");
+
+    public:
+        T operator++() DOCTEST_NOEXCEPT { return fetch_add(1) + 1; }
+
+        T operator++(int) DOCTEST_NOEXCEPT { return fetch_add(1); }
+
+        T fetch_add(T arg, std::memory_order order = std::memory_order_seq_cst) DOCTEST_NOEXCEPT {
+            return myAtomic().fetch_add(arg, order);
+        }
+
+        T fetch_sub(T arg, std::memory_order order = std::memory_order_seq_cst) DOCTEST_NOEXCEPT {
+            return myAtomic().fetch_sub(arg, order);
+        }
+
+        operator T() const DOCTEST_NOEXCEPT { return load(); }
+
+        T load(std::memory_order order = std::memory_order_seq_cst) const DOCTEST_NOEXCEPT {
+            auto result = T();
+            for(auto const& c : m_atomics) {
+                result += c.atomic.load(order);
+            }
+            return result;
+        }
+
+        T operator=(T desired) DOCTEST_NOEXCEPT { // lgtm [cpp/assignment-does-not-return-this]
+            store(desired);
+            return desired;
+        }
+
+        void store(T desired, std::memory_order order = std::memory_order_seq_cst) DOCTEST_NOEXCEPT {
+            // first value becomes desired", all others become 0.
+            for(auto& c : m_atomics) {
+                c.atomic.store(desired, order);
+                desired = {};
+            }
+        }
+
+    private:
+        // Each thread has a different atomic that it operates on. If more than NumLanes threads
+        // use this, some will use the same atomic. So performance will degrade a bit, but still
+        // everything will work.
+        //
+        // The logic here is a bit tricky. The call should be as fast as possible, so that there
+        // is minimal to no overhead in determining the correct atomic for the current thread.
+        //
+        // 1. A global static counter laneCounter counts continuously up.
+        // 2. Each successive thread will use modulo operation of that counter so it gets an atomic
+        //    assigned in a round-robin fashion.
+        // 3. This tlsLaneIdx is stored in the thread local data, so it is directly available with
+        //    little overhead.
+        Atomic<T>& myAtomic() DOCTEST_NOEXCEPT {
+            static Atomic<size_t> laneCounter;
+            DOCTEST_THREAD_LOCAL size_t tlsLaneIdx =
+                    laneCounter++ % DOCTEST_MULTI_LANE_ATOMICS_THREAD_LANES;
+
+            return m_atomics[tlsLaneIdx].atomic;
+        }
+    };
+#endif // DOCTEST_CONFIG_NO_MULTI_LANE_ATOMICS
+
     // this holds both parameters from the command line and runtime data for tests
     struct ContextState : ContextOptions, TestRunStats, CurrentTestCaseStats
     {
-        std::atomic<int> numAssertsCurrentTest_atomic;
-        std::atomic<int> numAssertsFailedCurrentTest_atomic;
+        MultiLaneAtomic<int> numAssertsCurrentTest_atomic;
+        MultiLaneAtomic<int> numAssertsFailedCurrentTest_atomic;
 
         std::vector<std::vector<String>> filters = decltype(filters)(9); // 9 different filters
 
         std::vector<IReporter*> reporters_currently_used;
 
-        const TestCase* currentTest = nullptr;
-
         assert_handler ah = nullptr;
 
         Timer timer;
 
         std::vector<String> stringifiedContexts; // logging from INFO() due to an exception
 
         // stuff for subcases
-        std::vector<SubcaseSignature>     subcasesStack;
-        std::set<decltype(subcasesStack)> subcasesPassed;
-        int                               subcasesCurrentMaxLevel;
-        bool                              should_reenter;
-        std::atomic<bool>                 shouldLogCurrentException;
+        bool reachedLeaf;
+        std::vector<SubcaseSignature> subcaseStack;
+        std::vector<SubcaseSignature> nextSubcaseStack;
+        std::unordered_set<unsigned long long> fullyTraversedSubcases;
+        size_t currentSubcaseDepth;
+        Atomic<bool> shouldLogCurrentException;
 
         void resetRunData() {
             numTestCases                = 0;
             numTestCasesPassingFilters  = 0;
             numTestSuitesPassingFilters = 0;
             numTestCasesFailed          = 0;
             numAsserts                  = 0;
@@ -3006,70 +3577,79 @@
             }
 
             bool ok_to_fail = (TestCaseFailureReason::ShouldHaveFailedAndDid & failure_flags) ||
                               (TestCaseFailureReason::CouldHaveFailedAndDid & failure_flags) ||
                               (TestCaseFailureReason::FailedExactlyNumTimes & failure_flags);
 
             // if any subcase has failed - the whole test case has failed
-            if(failure_flags && !ok_to_fail)
+            testCaseSuccess = !(failure_flags && !ok_to_fail);
+            if(!testCaseSuccess)
                 numTestCasesFailed++;
         }
     };
 
     ContextState* g_cs = nullptr;
 
     // used to avoid locks for the debug output
     // TODO: figure out if this is indeed necessary/correct - seems like either there still
     // could be a race or that there wouldn't be a race even if using the context directly
     DOCTEST_THREAD_LOCAL bool g_no_colors;
 
 #endif // DOCTEST_CONFIG_DISABLE
 } // namespace detail
 
-void String::setOnHeap() { *reinterpret_cast<unsigned char*>(&buf[last]) = 128; }
-void String::setLast(unsigned in) { buf[last] = char(in); }
+char* String::allocate(size_type sz) {
+    if (sz <= last) {
+        buf[sz] = '\0';
+        setLast(last - sz);
+        return buf;
+    } else {
+        setOnHeap();
+        data.size = sz;
+        data.capacity = data.size + 1;
+        data.ptr = new char[data.capacity];
+        data.ptr[sz] = '\0';
+        return data.ptr;
+    }
+}
+
+void String::setOnHeap() noexcept { *reinterpret_cast<unsigned char*>(&buf[last]) = 128; }
+void String::setLast(size_type in) noexcept { buf[last] = char(in); }
+void String::setSize(size_type sz) noexcept {
+    if (isOnStack()) { buf[sz] = '\0'; setLast(last - sz); }
+    else { data.ptr[sz] = '\0'; data.size = sz; }
+}
 
 void String::copy(const String& other) {
-    using namespace std;
     if(other.isOnStack()) {
         memcpy(buf, other.buf, len);
     } else {
-        setOnHeap();
-        data.size     = other.data.size;
-        data.capacity = data.size + 1;
-        data.ptr      = new char[data.capacity];
-        memcpy(data.ptr, other.data.ptr, data.size + 1);
+        memcpy(allocate(other.data.size), other.data.ptr, other.data.size);
     }
 }
 
-String::String() {
+String::String() noexcept {
     buf[0] = '\0';
     setLast();
 }
 
 String::~String() {
     if(!isOnStack())
         delete[] data.ptr;
-}
+} // NOLINT(clang-analyzer-cplusplus.NewDeleteLeaks)
 
 String::String(const char* in)
         : String(in, strlen(in)) {}
 
-String::String(const char* in, unsigned in_size) {
-    using namespace std;
-    if(in_size <= last) {
-        memcpy(buf, in, in_size + 1);
-        setLast(last - in_size);
-    } else {
-        setOnHeap();
-        data.size     = in_size;
-        data.capacity = data.size + 1;
-        data.ptr      = new char[data.capacity];
-        memcpy(data.ptr, in, in_size + 1);
-    }
+String::String(const char* in, size_type in_size) {
+    memcpy(allocate(in_size), in, in_size);
+}
+
+String::String(std::istream& in, size_type in_size) {
+    in.read(allocate(in_size), in_size);
 }
 
 String::String(const String& other) { copy(other); }
 
 String& String::operator=(const String& other) {
     if(this != &other) {
         if(!isOnStack())
@@ -3078,22 +3658,22 @@
         copy(other);
     }
 
     return *this;
 }
 
 String& String::operator+=(const String& other) {
-    const unsigned my_old_size = size();
-    const unsigned other_size  = other.size();
-    const unsigned total_size  = my_old_size + other_size;
-    using namespace std;
+    const size_type my_old_size = size();
+    const size_type other_size  = other.size();
+    const size_type total_size  = my_old_size + other_size;
     if(isOnStack()) {
         if(total_size < len) {
             // append to the current stack space
             memcpy(buf + my_old_size, other.c_str(), other_size + 1);
+            // NOLINTNEXTLINE(clang-analyzer-cplusplus.NewDeleteLeaks)
             setLast(last - total_size);
         } else {
             // alloc new chunk
             char* temp = new char[total_size + 1];
             // copy current data to new location before writing in the union
             memcpy(temp, buf, my_old_size); // skip the +1 ('\0') for speed
             // update data in union
@@ -3127,151 +3707,170 @@
             memcpy(data.ptr + my_old_size, other.c_str(), other_size + 1);
         }
     }
 
     return *this;
 }
 
-String String::operator+(const String& other) const { return String(*this) += other; }
-
-String::String(String&& other) {
-    using namespace std;
+String::String(String&& other) noexcept {
     memcpy(buf, other.buf, len);
     other.buf[0] = '\0';
     other.setLast();
 }
 
-String& String::operator=(String&& other) {
-    using namespace std;
+String& String::operator=(String&& other) noexcept {
     if(this != &other) {
         if(!isOnStack())
             delete[] data.ptr;
         memcpy(buf, other.buf, len);
         other.buf[0] = '\0';
         other.setLast();
     }
     return *this;
 }
 
-char String::operator[](unsigned i) const {
-    return const_cast<String*>(this)->operator[](i); // NOLINT
+char String::operator[](size_type i) const {
+    return const_cast<String*>(this)->operator[](i);
 }
 
-char& String::operator[](unsigned i) {
+char& String::operator[](size_type i) {
     if(isOnStack())
         return reinterpret_cast<char*>(buf)[i];
     return data.ptr[i];
 }
 
 DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wmaybe-uninitialized")
-unsigned String::size() const {
+String::size_type String::size() const {
     if(isOnStack())
-        return last - (unsigned(buf[last]) & 31); // using "last" would work only if "len" is 32
+        return last - (size_type(buf[last]) & 31); // using "last" would work only if "len" is 32
     return data.size;
 }
 DOCTEST_GCC_SUPPRESS_WARNING_POP
 
-unsigned String::capacity() const {
+String::size_type String::capacity() const {
     if(isOnStack())
         return len;
     return data.capacity;
 }
 
+String String::substr(size_type pos, size_type cnt) && {
+    cnt = std::min(cnt, size() - 1 - pos);
+    char* cptr = c_str();
+    memmove(cptr, cptr + pos, cnt);
+    setSize(cnt);
+    return std::move(*this);
+}
+
+String String::substr(size_type pos, size_type cnt) const & {
+    cnt = std::min(cnt, size() - 1 - pos);
+    return String{ c_str() + pos, cnt };
+}
+
+String::size_type String::find(char ch, size_type pos) const {
+    const char* begin = c_str();
+    const char* end = begin + size();
+    const char* it = begin + pos;
+    for (; it < end && *it != ch; it++);
+    if (it < end) { return static_cast<size_type>(it - begin); }
+    else { return npos; }
+}
+
+String::size_type String::rfind(char ch, size_type pos) const {
+    const char* begin = c_str();
+    const char* it = begin + std::min(pos, size() - 1);
+    for (; it >= begin && *it != ch; it--);
+    if (it >= begin) { return static_cast<size_type>(it - begin); }
+    else { return npos; }
+}
+
 int String::compare(const char* other, bool no_case) const {
     if(no_case)
         return doctest::stricmp(c_str(), other);
     return std::strcmp(c_str(), other);
 }
 
 int String::compare(const String& other, bool no_case) const {
     return compare(other.c_str(), no_case);
 }
 
-// clang-format off
+String operator+(const String& lhs, const String& rhs) { return  String(lhs) += rhs; }
+
 bool operator==(const String& lhs, const String& rhs) { return lhs.compare(rhs) == 0; }
 bool operator!=(const String& lhs, const String& rhs) { return lhs.compare(rhs) != 0; }
 bool operator< (const String& lhs, const String& rhs) { return lhs.compare(rhs) < 0; }
 bool operator> (const String& lhs, const String& rhs) { return lhs.compare(rhs) > 0; }
 bool operator<=(const String& lhs, const String& rhs) { return (lhs != rhs) ? lhs.compare(rhs) < 0 : true; }
 bool operator>=(const String& lhs, const String& rhs) { return (lhs != rhs) ? lhs.compare(rhs) > 0 : true; }
-// clang-format on
 
 std::ostream& operator<<(std::ostream& s, const String& in) { return s << in.c_str(); }
 
+Contains::Contains(const String& str) : string(str) { }
+
+bool Contains::checkWith(const String& other) const {
+    return strstr(other.c_str(), string.c_str()) != nullptr;
+}
+
+String toString(const Contains& in) {
+    return "Contains( " + in.string + " )";
+}
+
+bool operator==(const String& lhs, const Contains& rhs) { return rhs.checkWith(lhs); }
+bool operator==(const Contains& lhs, const String& rhs) { return lhs.checkWith(rhs); }
+bool operator!=(const String& lhs, const Contains& rhs) { return !rhs.checkWith(lhs); }
+bool operator!=(const Contains& lhs, const String& rhs) { return !lhs.checkWith(rhs); }
+
 namespace {
     void color_to_stream(std::ostream&, Color::Enum) DOCTEST_BRANCH_ON_DISABLED({}, ;)
 } // namespace
 
 namespace Color {
     std::ostream& operator<<(std::ostream& s, Color::Enum code) {
         color_to_stream(s, code);
         return s;
     }
 } // namespace Color
 
 // clang-format off
 const char* assertString(assertType::Enum at) {
-    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4062) // enum 'x' in switch of enum 'y' is not handled
-    switch(at) {  //!OCLINT missing default in switch statements
-        case assertType::DT_WARN                    : return "WARN";
-        case assertType::DT_CHECK                   : return "CHECK";
-        case assertType::DT_REQUIRE                 : return "REQUIRE";
-
-        case assertType::DT_WARN_FALSE              : return "WARN_FALSE";
-        case assertType::DT_CHECK_FALSE             : return "CHECK_FALSE";
-        case assertType::DT_REQUIRE_FALSE           : return "REQUIRE_FALSE";
-
-        case assertType::DT_WARN_THROWS             : return "WARN_THROWS";
-        case assertType::DT_CHECK_THROWS            : return "CHECK_THROWS";
-        case assertType::DT_REQUIRE_THROWS          : return "REQUIRE_THROWS";
-
-        case assertType::DT_WARN_THROWS_AS          : return "WARN_THROWS_AS";
-        case assertType::DT_CHECK_THROWS_AS         : return "CHECK_THROWS_AS";
-        case assertType::DT_REQUIRE_THROWS_AS       : return "REQUIRE_THROWS_AS";
-
-        case assertType::DT_WARN_THROWS_WITH        : return "WARN_THROWS_WITH";
-        case assertType::DT_CHECK_THROWS_WITH       : return "CHECK_THROWS_WITH";
-        case assertType::DT_REQUIRE_THROWS_WITH     : return "REQUIRE_THROWS_WITH";
-
-        case assertType::DT_WARN_THROWS_WITH_AS     : return "WARN_THROWS_WITH_AS";
-        case assertType::DT_CHECK_THROWS_WITH_AS    : return "CHECK_THROWS_WITH_AS";
-        case assertType::DT_REQUIRE_THROWS_WITH_AS  : return "REQUIRE_THROWS_WITH_AS";
-
-        case assertType::DT_WARN_NOTHROW            : return "WARN_NOTHROW";
-        case assertType::DT_CHECK_NOTHROW           : return "CHECK_NOTHROW";
-        case assertType::DT_REQUIRE_NOTHROW         : return "REQUIRE_NOTHROW";
-
-        case assertType::DT_WARN_EQ                 : return "WARN_EQ";
-        case assertType::DT_CHECK_EQ                : return "CHECK_EQ";
-        case assertType::DT_REQUIRE_EQ              : return "REQUIRE_EQ";
-        case assertType::DT_WARN_NE                 : return "WARN_NE";
-        case assertType::DT_CHECK_NE                : return "CHECK_NE";
-        case assertType::DT_REQUIRE_NE              : return "REQUIRE_NE";
-        case assertType::DT_WARN_GT                 : return "WARN_GT";
-        case assertType::DT_CHECK_GT                : return "CHECK_GT";
-        case assertType::DT_REQUIRE_GT              : return "REQUIRE_GT";
-        case assertType::DT_WARN_LT                 : return "WARN_LT";
-        case assertType::DT_CHECK_LT                : return "CHECK_LT";
-        case assertType::DT_REQUIRE_LT              : return "REQUIRE_LT";
-        case assertType::DT_WARN_GE                 : return "WARN_GE";
-        case assertType::DT_CHECK_GE                : return "CHECK_GE";
-        case assertType::DT_REQUIRE_GE              : return "REQUIRE_GE";
-        case assertType::DT_WARN_LE                 : return "WARN_LE";
-        case assertType::DT_CHECK_LE                : return "CHECK_LE";
-        case assertType::DT_REQUIRE_LE              : return "REQUIRE_LE";
-
-        case assertType::DT_WARN_UNARY              : return "WARN_UNARY";
-        case assertType::DT_CHECK_UNARY             : return "CHECK_UNARY";
-        case assertType::DT_REQUIRE_UNARY           : return "REQUIRE_UNARY";
-        case assertType::DT_WARN_UNARY_FALSE        : return "WARN_UNARY_FALSE";
-        case assertType::DT_CHECK_UNARY_FALSE       : return "CHECK_UNARY_FALSE";
-        case assertType::DT_REQUIRE_UNARY_FALSE     : return "REQUIRE_UNARY_FALSE";
+    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4061) // enum 'x' in switch of enum 'y' is not explicitly handled
+    #define DOCTEST_GENERATE_ASSERT_TYPE_CASE(assert_type) case assertType::DT_ ## assert_type: return #assert_type
+    #define DOCTEST_GENERATE_ASSERT_TYPE_CASES(assert_type) \
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(WARN_ ## assert_type); \
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(CHECK_ ## assert_type); \
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(REQUIRE_ ## assert_type)
+    switch(at) {
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(WARN);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(CHECK);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASE(REQUIRE);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(FALSE);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(THROWS);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(THROWS_AS);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(THROWS_WITH);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(THROWS_WITH_AS);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(NOTHROW);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(EQ);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(NE);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(GT);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(LT);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(GE);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(LE);
+
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(UNARY);
+        DOCTEST_GENERATE_ASSERT_TYPE_CASES(UNARY_FALSE);
+
+        default: DOCTEST_INTERNAL_ERROR("Tried stringifying invalid assert type!");
     }
     DOCTEST_MSVC_SUPPRESS_WARNING_POP
-    return "";
 }
 // clang-format on
 
 const char* failureString(assertType::Enum at) {
     if(at & assertType::is_warn) //!OCLINT bitwise operator in conditional
         return "WARNING";
     if(at & assertType::is_check) //!OCLINT bitwise operator in conditional
@@ -3281,74 +3880,91 @@
     return "";
 }
 
 DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wnull-dereference")
 DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wnull-dereference")
 // depending on the current options this will remove the path of filenames
 const char* skipPathFromFilename(const char* file) {
+#ifndef DOCTEST_CONFIG_DISABLE
     if(getContextOptions()->no_path_in_filenames) {
         auto back    = std::strrchr(file, '\\');
         auto forward = std::strrchr(file, '/');
         if(back || forward) {
             if(back > forward)
                 forward = back;
             return forward + 1;
         }
     }
+#endif // DOCTEST_CONFIG_DISABLE
     return file;
 }
 DOCTEST_CLANG_SUPPRESS_WARNING_POP
 DOCTEST_GCC_SUPPRESS_WARNING_POP
 
+bool SubcaseSignature::operator==(const SubcaseSignature& other) const {
+    return m_line == other.m_line
+        && std::strcmp(m_file, other.m_file) == 0
+        && m_name == other.m_name;
+}
+
 bool SubcaseSignature::operator<(const SubcaseSignature& other) const {
     if(m_line != other.m_line)
         return m_line < other.m_line;
     if(std::strcmp(m_file, other.m_file) != 0)
         return std::strcmp(m_file, other.m_file) < 0;
     return m_name.compare(other.m_name) < 0;
 }
 
-IContextScope::IContextScope()  = default;
-IContextScope::~IContextScope() = default;
+DOCTEST_DEFINE_INTERFACE(IContextScope)
+
+namespace detail {
+    void filldata<const void*>::fill(std::ostream* stream, const void* in) {
+        if (in) { *stream << in; }
+        else { *stream << "nullptr"; }
+    }
+
+    template <typename T>
+    String toStreamLit(T t) {
+        std::ostream* os = tlssPush();
+        os->operator<<(t);
+        return tlssPop();
+    }
+}
 
 #ifdef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-String toString(char* in) { return toString(static_cast<const char*>(in)); }
 String toString(const char* in) { return String("\"") + (in ? in : "{null string}") + "\""; }
 #endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-String toString(bool in) { return in ? "true" : "false"; }
-String toString(float in) { return fpToString(in, 5) + "f"; }
-String toString(double in) { return fpToString(in, 10); }
-String toString(double long in) { return fpToString(in, 15); }
-
-#define DOCTEST_TO_STRING_OVERLOAD(type, fmt)                                                      \
-    String toString(type in) {                                                                     \
-        char buf[64];                                                                              \
-        std::sprintf(buf, fmt, in);                                                                \
-        return buf;                                                                                \
-    }
-
-DOCTEST_TO_STRING_OVERLOAD(char, "%d")
-DOCTEST_TO_STRING_OVERLOAD(char signed, "%d")
-DOCTEST_TO_STRING_OVERLOAD(char unsigned, "%u")
-DOCTEST_TO_STRING_OVERLOAD(int short, "%d")
-DOCTEST_TO_STRING_OVERLOAD(int short unsigned, "%u")
-DOCTEST_TO_STRING_OVERLOAD(int, "%d")
-DOCTEST_TO_STRING_OVERLOAD(unsigned, "%u")
-DOCTEST_TO_STRING_OVERLOAD(int long, "%ld")
-DOCTEST_TO_STRING_OVERLOAD(int long unsigned, "%lu")
-DOCTEST_TO_STRING_OVERLOAD(int long long, "%lld")
-DOCTEST_TO_STRING_OVERLOAD(int long long unsigned, "%llu")
-
-String toString(std::nullptr_t) { return "NULL"; }
 
 #if DOCTEST_MSVC >= DOCTEST_COMPILER(19, 20, 0)
-// see this issue on why this is needed: https://github.com/onqtam/doctest/issues/183
+// see this issue on why this is needed: https://github.com/doctest/doctest/issues/183
 String toString(const std::string& in) { return in.c_str(); }
 #endif // VS 2019
 
+String toString(String in) { return in; }
+
+String toString(std::nullptr_t) { return "nullptr"; }
+
+String toString(bool in) { return in ? "true" : "false"; }
+
+String toString(float in) { return toStreamLit(in); }
+String toString(double in) { return toStreamLit(in); }
+String toString(double long in) { return toStreamLit(in); }
+
+String toString(char in) { return toStreamLit(static_cast<signed>(in)); }
+String toString(char signed in) { return toStreamLit(static_cast<signed>(in)); }
+String toString(char unsigned in) { return toStreamLit(static_cast<unsigned>(in)); }
+String toString(short in) { return toStreamLit(in); }
+String toString(short unsigned in) { return toStreamLit(in); }
+String toString(signed in) { return toStreamLit(in); }
+String toString(unsigned in) { return toStreamLit(in); }
+String toString(long in) { return toStreamLit(in); }
+String toString(long unsigned in) { return toStreamLit(in); }
+String toString(long long in) { return toStreamLit(in); }
+String toString(long long unsigned in) { return toStreamLit(in); }
+
 Approx::Approx(double value)
         : m_epsilon(static_cast<double>(std::numeric_limits<float>::epsilon()) * 100)
         , m_scale(1.0)
         , m_value(value) {}
 
 Approx Approx::operator()(double value) const {
     Approx approx(value);
@@ -3380,36 +3996,51 @@
 bool operator>=(const Approx& lhs, double rhs) { return lhs.m_value > rhs || lhs == rhs; }
 bool operator<(double lhs, const Approx& rhs) { return lhs < rhs.m_value && lhs != rhs; }
 bool operator<(const Approx& lhs, double rhs) { return lhs.m_value < rhs && lhs != rhs; }
 bool operator>(double lhs, const Approx& rhs) { return lhs > rhs.m_value && lhs != rhs; }
 bool operator>(const Approx& lhs, double rhs) { return lhs.m_value > rhs && lhs != rhs; }
 
 String toString(const Approx& in) {
-    return String("Approx( ") + doctest::toString(in.m_value) + " )";
+    return "Approx( " + doctest::toString(in.m_value) + " )";
 }
 const ContextOptions* getContextOptions() { return DOCTEST_BRANCH_ON_DISABLED(nullptr, g_cs); }
 
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4738)
+template <typename F>
+IsNaN<F>::operator bool() const {
+    return std::isnan(value) ^ flipped;
+}
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
+template struct DOCTEST_INTERFACE_DEF IsNaN<float>;
+template struct DOCTEST_INTERFACE_DEF IsNaN<double>;
+template struct DOCTEST_INTERFACE_DEF IsNaN<long double>;
+template <typename F>
+String toString(IsNaN<F> in) { return String(in.flipped ? "! " : "") + "IsNaN( " + doctest::toString(in.value) + " )"; }
+String toString(IsNaN<float> in) { return toString<float>(in); }
+String toString(IsNaN<double> in) { return toString<double>(in); }
+String toString(IsNaN<double long> in) { return toString<double long>(in); }
+
 } // namespace doctest
 
 #ifdef DOCTEST_CONFIG_DISABLE
 namespace doctest {
 Context::Context(int, const char* const*) {}
 Context::~Context() = default;
 void Context::applyCommandLine(int, const char* const*) {}
 void Context::addFilter(const char*, const char*) {}
 void Context::clearFilters() {}
+void Context::setOption(const char*, bool) {}
 void Context::setOption(const char*, int) {}
 void Context::setOption(const char*, const char*) {}
 bool Context::shouldExit() { return false; }
 void Context::setAsDefaultForAssertsOutOfTestCases() {}
 void Context::setAssertHandler(detail::assert_handler) {}
+void Context::setCout(std::ostream*) {}
 int  Context::run() { return 0; }
 
-IReporter::~IReporter() = default;
-
 int                         IReporter::get_num_active_contexts() { return 0; }
 const IContextScope* const* IReporter::get_active_contexts() { return nullptr; }
 int                         IReporter::get_num_stringified_contexts() { return 0; }
 const String*               IReporter::get_stringified_contexts() { return nullptr; }
 
 int registerReporter(const char*, int, IReporter*) { return 0; }
 
@@ -3425,24 +4056,24 @@
 #endif // platform
 #endif // DOCTEST_CONFIG_COLORS_WINDOWS && DOCTEST_CONFIG_COLORS_ANSI
 #endif // DOCTEST_CONFIG_COLORS_NONE
 
 namespace doctest_detail_test_suite_ns {
 // holds the current test suite
 doctest::detail::TestSuite& getCurrentTestSuite() {
-    static doctest::detail::TestSuite data;
+    static doctest::detail::TestSuite data{};
     return data;
 }
 } // namespace doctest_detail_test_suite_ns
 
 namespace doctest {
 namespace {
     // the int (priority) is part of the key for automatic sorting - sadly one can register a
     // reporter with a duplicate name and a different priority but hopefully that won't happen often :|
-    typedef std::map<std::pair<int, String>, reporterCreatorFunc> reporterMap;
+    using reporterMap = std::map<std::pair<int, String>, reporterCreatorFunc>;
 
     reporterMap& getReporters() {
         static reporterMap data;
         return data;
     }
     reporterMap& getListeners() {
         static reporterMap data;
@@ -3466,16 +4097,16 @@
 
         return false;
     }
 
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
     DOCTEST_NORETURN void throwException() {
         g_cs->shouldLogCurrentException = false;
-        throw TestFailureException();
-    } // NOLINT(cert-err60-cpp)
+        throw TestFailureException(); // NOLINT(hicpp-exception-baseclass)
+    }
 #else // DOCTEST_CONFIG_NO_EXCEPTIONS
     void throwException() {}
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS
 } // namespace detail
 
 namespace {
     using namespace detail;
@@ -3513,130 +4144,168 @@
 
         while(*wild == '*') {
             wild++;
         }
         return !*wild;
     }
 
-    //// C string hash function (djb2) - taken from http://www.cse.yorku.ca/~oz/hash.html
-    //unsigned hashStr(unsigned const char* str) {
-    //    unsigned long hash = 5381;
-    //    char          c;
-    //    while((c = *str++))
-    //        hash = ((hash << 5) + hash) + c; // hash * 33 + c
-    //    return hash;
-    //}
-
     // checks if the name matches any of the filters (and can be configured what to do when empty)
     bool matchesAny(const char* name, const std::vector<String>& filters, bool matchEmpty,
-                    bool caseSensitive) {
-        if(filters.empty() && matchEmpty)
+        bool caseSensitive) {
+        if (filters.empty() && matchEmpty)
             return true;
-        for(auto& curr : filters)
-            if(wildcmp(name, curr.c_str(), caseSensitive))
+        for (auto& curr : filters)
+            if (wildcmp(name, curr.c_str(), caseSensitive))
                 return true;
         return false;
     }
-} // namespace
-namespace detail {
 
-    Subcase::Subcase(const String& name, const char* file, int line)
-            : m_signature({name, file, line}) {
-        ContextState* s = g_cs;
+    DOCTEST_NO_SANITIZE_INTEGER
+    unsigned long long hash(unsigned long long a, unsigned long long b) {
+        return (a << 5) + b;
+    }
 
-        // check subcase filters
-        if(s->subcasesStack.size() < size_t(s->subcase_filter_levels)) {
-            if(!matchesAny(m_signature.m_name.c_str(), s->filters[6], true, s->case_sensitive))
-                return;
-            if(matchesAny(m_signature.m_name.c_str(), s->filters[7], false, s->case_sensitive))
-                return;
-        }
-        
-        // if a Subcase on the same level has already been entered
-        if(s->subcasesStack.size() < size_t(s->subcasesCurrentMaxLevel)) {
-            s->should_reenter = true;
-            return;
-        }
+    // C string hash function (djb2) - taken from http://www.cse.yorku.ca/~oz/hash.html
+    DOCTEST_NO_SANITIZE_INTEGER
+    unsigned long long hash(const char* str) {
+        unsigned long long hash = 5381;
+        char c;
+        while ((c = *str++))
+            hash = ((hash << 5) + hash) + c; // hash * 33 + c
+        return hash;
+    }
 
-        // push the current signature to the stack so we can check if the
-        // current stack + the current new subcase have been traversed
-        s->subcasesStack.push_back(m_signature);
-        if(s->subcasesPassed.count(s->subcasesStack) != 0) {
-            // pop - revert to previous stack since we've already passed this
-            s->subcasesStack.pop_back();
-            return;
+    unsigned long long hash(const SubcaseSignature& sig) {
+        return hash(hash(hash(sig.m_file), hash(sig.m_name.c_str())), sig.m_line);
+    }
+
+    unsigned long long hash(const std::vector<SubcaseSignature>& sigs, size_t count) {
+        unsigned long long running = 0;
+        auto end = sigs.begin() + count;
+        for (auto it = sigs.begin(); it != end; it++) {
+            running = hash(running, hash(*it));
         }
+        return running;
+    }
 
-        s->subcasesCurrentMaxLevel = s->subcasesStack.size();
-        m_entered = true;
+    unsigned long long hash(const std::vector<SubcaseSignature>& sigs) {
+        unsigned long long running = 0;
+        for (const SubcaseSignature& sig : sigs) {
+            running = hash(running, hash(sig));
+        }
+        return running;
+    }
+} // namespace
+namespace detail {
+    bool Subcase::checkFilters() {
+        if (g_cs->subcaseStack.size() < size_t(g_cs->subcase_filter_levels)) {
+            if (!matchesAny(m_signature.m_name.c_str(), g_cs->filters[6], true, g_cs->case_sensitive))
+                return true;
+            if (matchesAny(m_signature.m_name.c_str(), g_cs->filters[7], false, g_cs->case_sensitive))
+                return true;
+        }
+        return false;
+    }
 
-        DOCTEST_ITERATE_THROUGH_REPORTERS(subcase_start, m_signature);
+    Subcase::Subcase(const String& name, const char* file, int line)
+            : m_signature({name, file, line}) {
+        if (!g_cs->reachedLeaf) {
+            if (g_cs->nextSubcaseStack.size() <= g_cs->subcaseStack.size()
+                || g_cs->nextSubcaseStack[g_cs->subcaseStack.size()] == m_signature) {
+                // Going down.
+                if (checkFilters()) { return; }
+
+                g_cs->subcaseStack.push_back(m_signature);
+                g_cs->currentSubcaseDepth++;
+                m_entered = true;
+                DOCTEST_ITERATE_THROUGH_REPORTERS(subcase_start, m_signature);
+            }
+        } else {
+            if (g_cs->subcaseStack[g_cs->currentSubcaseDepth] == m_signature) {
+                // This subcase is reentered via control flow.
+                g_cs->currentSubcaseDepth++;
+                m_entered = true;
+                DOCTEST_ITERATE_THROUGH_REPORTERS(subcase_start, m_signature);
+            } else if (g_cs->nextSubcaseStack.size() <= g_cs->currentSubcaseDepth
+                    && g_cs->fullyTraversedSubcases.find(hash(hash(g_cs->subcaseStack, g_cs->currentSubcaseDepth), hash(m_signature)))
+                    == g_cs->fullyTraversedSubcases.end()) {
+                if (checkFilters()) { return; }
+                // This subcase is part of the one to be executed next.
+                g_cs->nextSubcaseStack.clear();
+                g_cs->nextSubcaseStack.insert(g_cs->nextSubcaseStack.end(),
+                    g_cs->subcaseStack.begin(), g_cs->subcaseStack.begin() + g_cs->currentSubcaseDepth);
+                g_cs->nextSubcaseStack.push_back(m_signature);
+            }
+        }
     }
 
-    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4996) // std::uncaught_exception is deprecated in C++17	
-    DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")	
+    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4996) // std::uncaught_exception is deprecated in C++17
+    DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
     DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
 
     Subcase::~Subcase() {
-        if(m_entered) {
-            // only mark the subcase stack as passed if no subcases have been skipped
-            if(g_cs->should_reenter == false)
-                g_cs->subcasesPassed.insert(g_cs->subcasesStack);
-            g_cs->subcasesStack.pop_back();
+        if (m_entered) {
+            g_cs->currentSubcaseDepth--;
+
+            if (!g_cs->reachedLeaf) {
+                // Leaf.
+                g_cs->fullyTraversedSubcases.insert(hash(g_cs->subcaseStack));
+                g_cs->nextSubcaseStack.clear();
+                g_cs->reachedLeaf = true;
+            } else if (g_cs->nextSubcaseStack.empty()) {
+                // All children are finished.
+                g_cs->fullyTraversedSubcases.insert(hash(g_cs->subcaseStack));
+            }
 
-#if defined(__cpp_lib_uncaught_exceptions) && __cpp_lib_uncaught_exceptions >= 201411L
+#if defined(__cpp_lib_uncaught_exceptions) && __cpp_lib_uncaught_exceptions >= 201411L && (!defined(__MAC_OS_X_VERSION_MIN_REQUIRED) || __MAC_OS_X_VERSION_MIN_REQUIRED >= 101200)
             if(std::uncaught_exceptions() > 0
 #else
             if(std::uncaught_exception()
 #endif
-            && g_cs->shouldLogCurrentException) {
+                && g_cs->shouldLogCurrentException) {
                 DOCTEST_ITERATE_THROUGH_REPORTERS(
                         test_case_exception, {"exception thrown in subcase - will translate later "
-                                              "when the whole test case has been exited (cannot "
-                                              "translate while there is an active exception)",
-                                              false});
+                                                "when the whole test case has been exited (cannot "
+                                                "translate while there is an active exception)",
+                                                false});
                 g_cs->shouldLogCurrentException = false;
             }
+
             DOCTEST_ITERATE_THROUGH_REPORTERS(subcase_end, DOCTEST_EMPTY);
         }
     }
 
-    DOCTEST_CLANG_SUPPRESS_WARNING_POP	
-    DOCTEST_GCC_SUPPRESS_WARNING_POP	
+    DOCTEST_CLANG_SUPPRESS_WARNING_POP
+    DOCTEST_GCC_SUPPRESS_WARNING_POP
     DOCTEST_MSVC_SUPPRESS_WARNING_POP
 
     Subcase::operator bool() const { return m_entered; }
 
     Result::Result(bool passed, const String& decomposition)
             : m_passed(passed)
             , m_decomp(decomposition) {}
 
     ExpressionDecomposer::ExpressionDecomposer(assertType::Enum at)
             : m_at(at) {}
 
     TestSuite& TestSuite::operator*(const char* in) {
         m_test_suite = in;
-        // clear state
-        m_description       = nullptr;
-        m_skip              = false;
-        m_may_fail          = false;
-        m_should_fail       = false;
-        m_expected_failures = 0;
-        m_timeout           = 0;
         return *this;
     }
 
     TestCase::TestCase(funcType test, const char* file, unsigned line, const TestSuite& test_suite,
-                       const char* type, int template_id) {
+                       const String& type, int template_id) {
         m_file              = file;
         m_line              = line;
         m_name              = nullptr; // will be later overridden in operator*
         m_test_suite        = test_suite.m_test_suite;
         m_description       = test_suite.m_description;
         m_skip              = test_suite.m_skip;
+        m_no_breaks         = test_suite.m_no_breaks;
+        m_no_output         = test_suite.m_no_output;
         m_may_fail          = test_suite.m_may_fail;
         m_should_fail       = test_suite.m_should_fail;
         m_expected_failures = test_suite.m_expected_failures;
         m_timeout           = test_suite.m_timeout;
 
         m_test        = test;
         m_type        = type;
@@ -3645,18 +4314,16 @@
 
     TestCase::TestCase(const TestCase& other)
             : TestCaseData() {
         *this = other;
     }
 
     DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(26434) // hides a non-virtual function
-    DOCTEST_MSVC_SUPPRESS_WARNING(26437)           // Do not slice
     TestCase& TestCase::operator=(const TestCase& other) {
-        static_cast<TestCaseData&>(*this) = static_cast<const TestCaseData&>(other);
-
+        TestCaseData::operator=(other);
         m_test        = other.m_test;
         m_type        = other.m_type;
         m_template_id = other.m_template_id;
         m_full_name   = other.m_full_name;
 
         if(m_template_id != -1)
             m_name = m_full_name.c_str();
@@ -3664,29 +4331,39 @@
     }
     DOCTEST_MSVC_SUPPRESS_WARNING_POP
 
     TestCase& TestCase::operator*(const char* in) {
         m_name = in;
         // make a new name with an appended type for templated test case
         if(m_template_id != -1) {
-            m_full_name = String(m_name) + m_type;
+            m_full_name = String(m_name) + "<" + m_type + ">";
             // redirect the name to point to the newly constructed full name
             m_name = m_full_name.c_str();
         }
         return *this;
     }
 
     bool TestCase::operator<(const TestCase& other) const {
+        // this will be used only to differentiate between test cases - not relevant for sorting
         if(m_line != other.m_line)
             return m_line < other.m_line;
+        const int name_cmp = strcmp(m_name, other.m_name);
+        if(name_cmp != 0)
+            return name_cmp < 0;
         const int file_cmp = m_file.compare(other.m_file);
         if(file_cmp != 0)
             return file_cmp < 0;
         return m_template_id < other.m_template_id;
     }
+
+    // all the registered tests
+    std::set<TestCase>& getRegisteredTests() {
+        static std::set<TestCase> data;
+        return data;
+    }
 } // namespace detail
 namespace {
     using namespace detail;
     // for sorting tests by file/line
     bool fileOrderComparator(const TestCase* lhs, const TestCase* rhs) {
         // this is needed because MSVC gives different case for drive letters
         // for __FILE__ when evaluated in a header and a source file
@@ -3710,47 +4387,18 @@
     bool nameOrderComparator(const TestCase* lhs, const TestCase* rhs) {
         const int res = std::strcmp(lhs->m_name, rhs->m_name);
         if(res != 0)
             return res < 0;
         return suiteOrderComparator(lhs, rhs);
     }
 
-    // all the registered tests
-    std::set<TestCase>& getRegisteredTests() {
-        static std::set<TestCase> data;
-        return data;
-    }
-
-#ifdef DOCTEST_CONFIG_COLORS_WINDOWS
-    HANDLE g_stdoutHandle;
-    WORD   g_origFgAttrs;
-    WORD   g_origBgAttrs;
-    bool   g_attrsInitted = false;
-
-    int colors_init() {
-        if(!g_attrsInitted) {
-            g_stdoutHandle = GetStdHandle(STD_OUTPUT_HANDLE);
-            g_attrsInitted = true;
-            CONSOLE_SCREEN_BUFFER_INFO csbiInfo;
-            GetConsoleScreenBufferInfo(g_stdoutHandle, &csbiInfo);
-            g_origFgAttrs = csbiInfo.wAttributes & ~(BACKGROUND_GREEN | BACKGROUND_RED |
-                                                     BACKGROUND_BLUE | BACKGROUND_INTENSITY);
-            g_origBgAttrs = csbiInfo.wAttributes & ~(FOREGROUND_GREEN | FOREGROUND_RED |
-                                                     FOREGROUND_BLUE | FOREGROUND_INTENSITY);
-        }
-        return 0;
-    }
-
-    int dumy_init_console_colors = colors_init();
-#endif // DOCTEST_CONFIG_COLORS_WINDOWS
-
     DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
     void color_to_stream(std::ostream& s, Color::Enum code) {
-        ((void)s);    // for DOCTEST_CONFIG_COLORS_NONE or DOCTEST_CONFIG_COLORS_WINDOWS
-        ((void)code); // for DOCTEST_CONFIG_COLORS_NONE
+        static_cast<void>(s);    // for DOCTEST_CONFIG_COLORS_NONE or DOCTEST_CONFIG_COLORS_WINDOWS
+        static_cast<void>(code); // for DOCTEST_CONFIG_COLORS_NONE
 #ifdef DOCTEST_CONFIG_COLORS_ANSI
         if(g_no_colors ||
            (isatty(STDOUT_FILENO) == false && getContextOptions()->force_colors == false))
             return;
 
         auto col = "";
         // clang-format off
@@ -3772,18 +4420,34 @@
             }
         // clang-format on
         s << "\033" << col;
 #endif // DOCTEST_CONFIG_COLORS_ANSI
 
 #ifdef DOCTEST_CONFIG_COLORS_WINDOWS
         if(g_no_colors ||
-           (isatty(fileno(stdout)) == false && getContextOptions()->force_colors == false))
+           (_isatty(_fileno(stdout)) == false && getContextOptions()->force_colors == false))
             return;
 
-#define DOCTEST_SET_ATTR(x) SetConsoleTextAttribute(g_stdoutHandle, x | g_origBgAttrs)
+        static struct ConsoleHelper {
+            HANDLE stdoutHandle;
+            WORD   origFgAttrs;
+            WORD   origBgAttrs;
+
+            ConsoleHelper() {
+                stdoutHandle = GetStdHandle(STD_OUTPUT_HANDLE);
+                CONSOLE_SCREEN_BUFFER_INFO csbiInfo;
+                GetConsoleScreenBufferInfo(stdoutHandle, &csbiInfo);
+                origFgAttrs = csbiInfo.wAttributes & ~(BACKGROUND_GREEN | BACKGROUND_RED |
+                    BACKGROUND_BLUE | BACKGROUND_INTENSITY);
+                origBgAttrs = csbiInfo.wAttributes & ~(FOREGROUND_GREEN | FOREGROUND_RED |
+                    FOREGROUND_BLUE | FOREGROUND_INTENSITY);
+            }
+        } ch;
+
+#define DOCTEST_SET_ATTR(x) SetConsoleTextAttribute(ch.stdoutHandle, x | ch.origBgAttrs)
 
         // clang-format off
         switch (code) {
             case Color::White:       DOCTEST_SET_ATTR(FOREGROUND_GREEN | FOREGROUND_RED | FOREGROUND_BLUE); break;
             case Color::Red:         DOCTEST_SET_ATTR(FOREGROUND_RED);                                      break;
             case Color::Green:       DOCTEST_SET_ATTR(FOREGROUND_GREEN);                                    break;
             case Color::Blue:        DOCTEST_SET_ATTR(FOREGROUND_BLUE);                                     break;
@@ -3792,15 +4456,15 @@
             case Color::Grey:        DOCTEST_SET_ATTR(0);                                                   break;
             case Color::LightGrey:   DOCTEST_SET_ATTR(FOREGROUND_INTENSITY);                                break;
             case Color::BrightRed:   DOCTEST_SET_ATTR(FOREGROUND_INTENSITY | FOREGROUND_RED);               break;
             case Color::BrightGreen: DOCTEST_SET_ATTR(FOREGROUND_INTENSITY | FOREGROUND_GREEN);             break;
             case Color::BrightWhite: DOCTEST_SET_ATTR(FOREGROUND_INTENSITY | FOREGROUND_GREEN | FOREGROUND_RED | FOREGROUND_BLUE); break;
             case Color::None:
             case Color::Bright: // invalid
-            default:                 DOCTEST_SET_ATTR(g_origFgAttrs);
+            default:                 DOCTEST_SET_ATTR(ch.origFgAttrs);
         }
             // clang-format on
 #endif // DOCTEST_CONFIG_COLORS_WINDOWS
     }
     DOCTEST_CLANG_SUPPRESS_WARNING_POP
 
     std::vector<const IExceptionTranslator*>& getExceptionTranslators() {
@@ -3848,15 +4512,36 @@
         doctest_detail_test_suite_ns::getCurrentTestSuite() = ts;
         return 0;
     }
 
 #ifdef DOCTEST_IS_DEBUGGER_ACTIVE
     bool isDebuggerActive() { return DOCTEST_IS_DEBUGGER_ACTIVE(); }
 #else // DOCTEST_IS_DEBUGGER_ACTIVE
-#ifdef DOCTEST_PLATFORM_MAC
+#ifdef DOCTEST_PLATFORM_LINUX
+    class ErrnoGuard {
+    public:
+        ErrnoGuard() : m_oldErrno(errno) {}
+        ~ErrnoGuard() { errno = m_oldErrno; }
+    private:
+        int m_oldErrno;
+    };
+    // See the comments in Catch2 for the reasoning behind this implementation:
+    // https://github.com/catchorg/Catch2/blob/v2.13.1/include/internal/catch_debugger.cpp#L79-L102
+    bool isDebuggerActive() {
+        ErrnoGuard guard;
+        std::ifstream in("/proc/self/status");
+        for(std::string line; std::getline(in, line);) {
+            static const int PREFIX_LEN = 11;
+            if(line.compare(0, PREFIX_LEN, "TracerPid:\t") == 0) {
+                return line.length() > PREFIX_LEN && line[PREFIX_LEN] != '0';
+            }
+        }
+        return false;
+    }
+#elif defined(DOCTEST_PLATFORM_MAC)
     // The following function is taken directly from the following technical note:
     // https://developer.apple.com/library/archive/qa/qa1361/_index.html
     // Returns true if the current process is being debugged (either
     // running under the debugger or has a debugger attached post facto).
     bool isDebuggerActive() {
         int        mib[4];
         kinfo_proc info;
@@ -3888,63 +4573,50 @@
 
     void registerExceptionTranslatorImpl(const IExceptionTranslator* et) {
         if(std::find(getExceptionTranslators().begin(), getExceptionTranslators().end(), et) ==
            getExceptionTranslators().end())
             getExceptionTranslators().push_back(et);
     }
 
-#ifdef DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-    void toStream(std::ostream* s, char* in) { *s << in; }
-    void toStream(std::ostream* s, const char* in) { *s << in; }
-#endif // DOCTEST_CONFIG_TREAT_CHAR_STAR_AS_STRING
-    void toStream(std::ostream* s, bool in) { *s << std::boolalpha << in << std::noboolalpha; }
-    void toStream(std::ostream* s, float in) { *s << in; }
-    void toStream(std::ostream* s, double in) { *s << in; }
-    void toStream(std::ostream* s, double long in) { *s << in; }
-
-    void toStream(std::ostream* s, char in) { *s << in; }
-    void toStream(std::ostream* s, char signed in) { *s << in; }
-    void toStream(std::ostream* s, char unsigned in) { *s << in; }
-    void toStream(std::ostream* s, int short in) { *s << in; }
-    void toStream(std::ostream* s, int short unsigned in) { *s << in; }
-    void toStream(std::ostream* s, int in) { *s << in; }
-    void toStream(std::ostream* s, int unsigned in) { *s << in; }
-    void toStream(std::ostream* s, int long in) { *s << in; }
-    void toStream(std::ostream* s, int long unsigned in) { *s << in; }
-    void toStream(std::ostream* s, int long long in) { *s << in; }
-    void toStream(std::ostream* s, int long long unsigned in) { *s << in; }
-
     DOCTEST_THREAD_LOCAL std::vector<IContextScope*> g_infoContexts; // for logging with INFO()
 
     ContextScopeBase::ContextScopeBase() {
         g_infoContexts.push_back(this);
     }
 
-    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4996) // std::uncaught_exception is deprecated in C++17	
-    DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")	
+    ContextScopeBase::ContextScopeBase(ContextScopeBase&& other) noexcept {
+        if (other.need_to_destroy) {
+            other.destroy();
+        }
+        other.need_to_destroy = false;
+        g_infoContexts.push_back(this);
+    }
+
+    DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4996) // std::uncaught_exception is deprecated in C++17
+    DOCTEST_GCC_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
     DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
 
     // destroy cannot be inlined into the destructor because that would mean calling stringify after
     // ContextScope has been destroyed (base class destructors run after derived class destructors).
     // Instead, ContextScope calls this method directly from its destructor.
     void ContextScopeBase::destroy() {
-#if defined(__cpp_lib_uncaught_exceptions) && __cpp_lib_uncaught_exceptions >= 201411L
+#if defined(__cpp_lib_uncaught_exceptions) && __cpp_lib_uncaught_exceptions >= 201411L && (!defined(__MAC_OS_X_VERSION_MIN_REQUIRED) || __MAC_OS_X_VERSION_MIN_REQUIRED >= 101200)
         if(std::uncaught_exceptions() > 0) {
 #else
         if(std::uncaught_exception()) {
 #endif
             std::ostringstream s;
             this->stringify(&s);
             g_cs->stringifiedContexts.push_back(s.str().c_str());
         }
         g_infoContexts.pop_back();
     }
 
-    DOCTEST_CLANG_SUPPRESS_WARNING_POP	
-    DOCTEST_GCC_SUPPRESS_WARNING_POP	
+    DOCTEST_CLANG_SUPPRESS_WARNING_POP
+    DOCTEST_GCC_SUPPRESS_WARNING_POP
     DOCTEST_MSVC_SUPPRESS_WARNING_POP
 } // namespace detail
 namespace {
     using namespace detail;
 
 #if !defined(DOCTEST_CONFIG_POSIX_SIGNALS) && !defined(DOCTEST_CONFIG_WINDOWS_SEH)
     struct FatalConditionHandler
@@ -3964,66 +4636,147 @@
         DWORD id;
         const char* name;
     };
     // There is no 1-1 mapping between signals and windows exceptions.
     // Windows can easily distinguish between SO and SigSegV,
     // but SigInt, SigTerm, etc are handled differently.
     SignalDefs signalDefs[] = {
-            {EXCEPTION_ILLEGAL_INSTRUCTION, "SIGILL - Illegal instruction signal"},
-            {EXCEPTION_STACK_OVERFLOW, "SIGSEGV - Stack overflow"},
-            {EXCEPTION_ACCESS_VIOLATION, "SIGSEGV - Segmentation violation signal"},
-            {EXCEPTION_INT_DIVIDE_BY_ZERO, "Divide by zero error"},
+            {static_cast<DWORD>(EXCEPTION_ILLEGAL_INSTRUCTION),
+             "SIGILL - Illegal instruction signal"},
+            {static_cast<DWORD>(EXCEPTION_STACK_OVERFLOW), "SIGSEGV - Stack overflow"},
+            {static_cast<DWORD>(EXCEPTION_ACCESS_VIOLATION),
+             "SIGSEGV - Segmentation violation signal"},
+            {static_cast<DWORD>(EXCEPTION_INT_DIVIDE_BY_ZERO), "Divide by zero error"},
     };
 
     struct FatalConditionHandler
     {
         static LONG CALLBACK handleException(PEXCEPTION_POINTERS ExceptionInfo) {
-            for(size_t i = 0; i < DOCTEST_COUNTOF(signalDefs); ++i) {
-                if(ExceptionInfo->ExceptionRecord->ExceptionCode == signalDefs[i].id) {
-                    reportFatal(signalDefs[i].name);
-                    break;
+            // Multiple threads may enter this filter/handler at once. We want the error message to be printed on the
+            // console just once no matter how many threads have crashed.
+            DOCTEST_DECLARE_STATIC_MUTEX(mutex)
+            static bool execute = true;
+            {
+                DOCTEST_LOCK_MUTEX(mutex)
+                if(execute) {
+                    bool reported = false;
+                    for(size_t i = 0; i < DOCTEST_COUNTOF(signalDefs); ++i) {
+                        if(ExceptionInfo->ExceptionRecord->ExceptionCode == signalDefs[i].id) {
+                            reportFatal(signalDefs[i].name);
+                            reported = true;
+                            break;
+                        }
+                    }
+                    if(reported == false)
+                        reportFatal("Unhandled SEH exception caught");
+                    if(isDebuggerActive() && !g_cs->no_breaks)
+                        DOCTEST_BREAK_INTO_DEBUGGER();
                 }
+                execute = false;
             }
-            // If its not an exception we care about, pass it along.
-            // This stops us from eating debugger breaks etc.
-            return EXCEPTION_CONTINUE_SEARCH;
+            std::exit(EXIT_FAILURE);
         }
 
         static void allocateAltStackMem() {}
         static void freeAltStackMem() {}
 
         FatalConditionHandler() {
             isSet = true;
             // 32k seems enough for doctest to handle stack overflow,
             // but the value was found experimentally, so there is no strong guarantee
             guaranteeSize = 32 * 1024;
             // Register an unhandled exception filter
             previousTop = SetUnhandledExceptionFilter(handleException);
             // Pass in guarantee size to be filled
             SetThreadStackGuarantee(&guaranteeSize);
+
+            // On Windows uncaught exceptions from another thread, exceptions from
+            // destructors, or calls to std::terminate are not a SEH exception
+
+            // The terminal handler gets called when:
+            // - std::terminate is called FROM THE TEST RUNNER THREAD
+            // - an exception is thrown from a destructor FROM THE TEST RUNNER THREAD
+            original_terminate_handler = std::get_terminate();
+            std::set_terminate([]() DOCTEST_NOEXCEPT {
+                reportFatal("Terminate handler called");
+                if(isDebuggerActive() && !g_cs->no_breaks)
+                    DOCTEST_BREAK_INTO_DEBUGGER();
+                std::exit(EXIT_FAILURE); // explicitly exit - otherwise the SIGABRT handler may be called as well
+            });
+
+            // SIGABRT is raised when:
+            // - std::terminate is called FROM A DIFFERENT THREAD
+            // - an exception is thrown from a destructor FROM A DIFFERENT THREAD
+            // - an uncaught exception is thrown FROM A DIFFERENT THREAD
+            prev_sigabrt_handler = std::signal(SIGABRT, [](int signal) DOCTEST_NOEXCEPT {
+                if(signal == SIGABRT) {
+                    reportFatal("SIGABRT - Abort (abnormal termination) signal");
+                    if(isDebuggerActive() && !g_cs->no_breaks)
+                        DOCTEST_BREAK_INTO_DEBUGGER();
+                    std::exit(EXIT_FAILURE);
+                }
+            });
+
+            // The following settings are taken from google test, and more
+            // specifically from UnitTest::Run() inside of gtest.cc
+
+            // the user does not want to see pop-up dialogs about crashes
+            prev_error_mode_1 = SetErrorMode(SEM_FAILCRITICALERRORS | SEM_NOALIGNMENTFAULTEXCEPT |
+                                             SEM_NOGPFAULTERRORBOX | SEM_NOOPENFILEERRORBOX);
+            // This forces the abort message to go to stderr in all circumstances.
+            prev_error_mode_2 = _set_error_mode(_OUT_TO_STDERR);
+            // In the debug version, Visual Studio pops up a separate dialog
+            // offering a choice to debug the aborted program - we want to disable that.
+            prev_abort_behavior = _set_abort_behavior(0x0, _WRITE_ABORT_MSG | _CALL_REPORTFAULT);
+            // In debug mode, the Windows CRT can crash with an assertion over invalid
+            // input (e.g. passing an invalid file descriptor). The default handling
+            // for these assertions is to pop up a dialog and wait for user input.
+            // Instead ask the CRT to dump such assertions to stderr non-interactively.
+            prev_report_mode = _CrtSetReportMode(_CRT_ASSERT, _CRTDBG_MODE_FILE | _CRTDBG_MODE_DEBUG);
+            prev_report_file = _CrtSetReportFile(_CRT_ASSERT, _CRTDBG_FILE_STDERR);
         }
 
         static void reset() {
             if(isSet) {
                 // Unregister handler and restore the old guarantee
                 SetUnhandledExceptionFilter(previousTop);
                 SetThreadStackGuarantee(&guaranteeSize);
-                previousTop = nullptr;
+                std::set_terminate(original_terminate_handler);
+                std::signal(SIGABRT, prev_sigabrt_handler);
+                SetErrorMode(prev_error_mode_1);
+                _set_error_mode(prev_error_mode_2);
+                _set_abort_behavior(prev_abort_behavior, _WRITE_ABORT_MSG | _CALL_REPORTFAULT);
+                static_cast<void>(_CrtSetReportMode(_CRT_ASSERT, prev_report_mode));
+                static_cast<void>(_CrtSetReportFile(_CRT_ASSERT, prev_report_file));
                 isSet = false;
             }
         }
 
         ~FatalConditionHandler() { reset(); }
 
     private:
+        static UINT         prev_error_mode_1;
+        static int          prev_error_mode_2;
+        static unsigned int prev_abort_behavior;
+        static int          prev_report_mode;
+        static _HFILE       prev_report_file;
+        static void (DOCTEST_CDECL *prev_sigabrt_handler)(int);
+        static std::terminate_handler original_terminate_handler;
         static bool isSet;
         static ULONG guaranteeSize;
         static LPTOP_LEVEL_EXCEPTION_FILTER previousTop;
     };
 
+    UINT         FatalConditionHandler::prev_error_mode_1;
+    int          FatalConditionHandler::prev_error_mode_2;
+    unsigned int FatalConditionHandler::prev_abort_behavior;
+    int          FatalConditionHandler::prev_report_mode;
+    _HFILE       FatalConditionHandler::prev_report_file;
+    void (DOCTEST_CDECL *FatalConditionHandler::prev_sigabrt_handler)(int);
+    std::terminate_handler FatalConditionHandler::original_terminate_handler;
     bool FatalConditionHandler::isSet = false;
     ULONG FatalConditionHandler::guaranteeSize = 0;
     LPTOP_LEVEL_EXCEPTION_FILTER FatalConditionHandler::previousTop = nullptr;
 
 #else // DOCTEST_PLATFORM_WINDOWS
 
     struct SignalDefs
@@ -4072,15 +4825,15 @@
             isSet = true;
             stack_t sigStack;
             sigStack.ss_sp    = altStackMem;
             sigStack.ss_size  = altStackSize;
             sigStack.ss_flags = 0;
             sigaltstack(&sigStack, &oldSigStack);
             struct sigaction sa = {};
-            sa.sa_handler       = handleSignal; // NOLINT
+            sa.sa_handler       = handleSignal;
             sa.sa_flags         = SA_ONSTACK;
             for(std::size_t i = 0; i < DOCTEST_COUNTOF(signalDefs); ++i) {
                 sigaction(signalDefs[i].id, &sa, &oldSigActions[i]);
             }
         }
 
         ~FatalConditionHandler() { reset(); }
@@ -4111,15 +4864,15 @@
 namespace {
     using namespace detail;
 
 #ifdef DOCTEST_PLATFORM_WINDOWS
 #define DOCTEST_OUTPUT_DEBUG_STRING(text) ::OutputDebugStringA(text)
 #else
     // TODO: integration with XCode and other IDEs
-#define DOCTEST_OUTPUT_DEBUG_STRING(text) // NOLINT(clang-diagnostic-unused-macros)
+#define DOCTEST_OUTPUT_DEBUG_STRING(text)
 #endif // Platform
 
     void addAssert(assertType::Enum at) {
         if((at & assertType::is_warn) == 0) //!OCLINT bitwise operator in conditional
             g_cs->numAssertsCurrentTest_atomic++;
     }
 
@@ -4130,46 +4883,47 @@
 
 #if defined(DOCTEST_CONFIG_POSIX_SIGNALS) || defined(DOCTEST_CONFIG_WINDOWS_SEH)
     void reportFatal(const std::string& message) {
         g_cs->failure_flags |= TestCaseFailureReason::Crash;
 
         DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_exception, {message.c_str(), true});
 
-        while(g_cs->subcasesStack.size()) {
-            g_cs->subcasesStack.pop_back();
+        while (g_cs->subcaseStack.size()) {
+            g_cs->subcaseStack.pop_back();
             DOCTEST_ITERATE_THROUGH_REPORTERS(subcase_end, DOCTEST_EMPTY);
         }
 
         g_cs->finalizeTestCaseData();
 
         DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_end, *g_cs);
 
         DOCTEST_ITERATE_THROUGH_REPORTERS(test_run_end, *g_cs);
     }
 #endif // DOCTEST_CONFIG_POSIX_SIGNALS || DOCTEST_CONFIG_WINDOWS_SEH
 } // namespace
-namespace detail {
 
-    ResultBuilder::ResultBuilder(assertType::Enum at, const char* file, int line, const char* expr,
-                                 const char* exception_type, const char* exception_string) {
-        m_test_case        = g_cs->currentTest;
-        m_at               = at;
-        m_file             = file;
-        m_line             = line;
-        m_expr             = expr;
-        m_failed           = true;
-        m_threw            = false;
-        m_threw_as         = false;
-        m_exception_type   = exception_type;
-        m_exception_string = exception_string;
+AssertData::AssertData(assertType::Enum at, const char* file, int line, const char* expr,
+    const char* exception_type, const StringContains& exception_string)
+    : m_test_case(g_cs->currentTest), m_at(at), m_file(file), m_line(line), m_expr(expr),
+    m_failed(true), m_threw(false), m_threw_as(false), m_exception_type(exception_type),
+    m_exception_string(exception_string) {
 #if DOCTEST_MSVC
-        if(m_expr[0] == ' ') // this happens when variadic macros are disabled under MSVC
-            ++m_expr;
+    if (m_expr[0] == ' ') // this happens when variadic macros are disabled under MSVC
+        ++m_expr;
 #endif // MSVC
-    }
+}
+
+namespace detail {
+    ResultBuilder::ResultBuilder(assertType::Enum at, const char* file, int line, const char* expr,
+                                 const char* exception_type, const String& exception_string)
+        : AssertData(at, file, line, expr, exception_type, exception_string) { }
+
+    ResultBuilder::ResultBuilder(assertType::Enum at, const char* file, int line, const char* expr,
+        const char* exception_type, const Contains& exception_string)
+        : AssertData(at, file, line, expr, exception_type, exception_string) { }
 
     void ResultBuilder::setResult(const Result& res) {
         m_decomp = res.m_decomp;
         m_failed = !res.m_passed;
     }
 
     void ResultBuilder::translateException() {
@@ -4177,116 +4931,107 @@
         m_exception = translateActiveException();
     }
 
     bool ResultBuilder::log() {
         if(m_at & assertType::is_throws) { //!OCLINT bitwise operator in conditional
             m_failed = !m_threw;
         } else if((m_at & assertType::is_throws_as) && (m_at & assertType::is_throws_with)) { //!OCLINT
-            m_failed = !m_threw_as || (m_exception != m_exception_string);
+            m_failed = !m_threw_as || !m_exception_string.check(m_exception);
         } else if(m_at & assertType::is_throws_as) { //!OCLINT bitwise operator in conditional
             m_failed = !m_threw_as;
         } else if(m_at & assertType::is_throws_with) { //!OCLINT bitwise operator in conditional
-            m_failed = m_exception != m_exception_string;
+            m_failed = !m_exception_string.check(m_exception);
         } else if(m_at & assertType::is_nothrow) { //!OCLINT bitwise operator in conditional
             m_failed = m_threw;
         }
 
         if(m_exception.size())
-            m_exception = String("\"") + m_exception + "\"";
+            m_exception = "\"" + m_exception + "\"";
 
         if(is_running_in_test) {
             addAssert(m_at);
             DOCTEST_ITERATE_THROUGH_REPORTERS(log_assert, *this);
 
             if(m_failed)
                 addFailedAssert(m_at);
         } else if(m_failed) {
             failed_out_of_a_testing_context(*this);
         }
 
-        return m_failed && isDebuggerActive() &&
-               !getContextOptions()->no_breaks; // break into debugger
+        return m_failed && isDebuggerActive() && !getContextOptions()->no_breaks &&
+            (g_cs->currentTest == nullptr || !g_cs->currentTest->m_no_breaks); // break into debugger
     }
 
     void ResultBuilder::react() const {
         if(m_failed && checkIfShouldThrow(m_at))
             throwException();
     }
 
     void failed_out_of_a_testing_context(const AssertData& ad) {
         if(g_cs->ah)
             g_cs->ah(ad);
         else
             std::abort();
     }
 
-    void decomp_assert(assertType::Enum at, const char* file, int line, const char* expr,
-                       Result result) {
+    bool decomp_assert(assertType::Enum at, const char* file, int line, const char* expr,
+                       const Result& result) {
         bool failed = !result.m_passed;
 
         // ###################################################################################
         // IF THE DEBUGGER BREAKS HERE - GO 1 LEVEL UP IN THE CALLSTACK FOR THE FAILING ASSERT
         // THIS IS THE EFFECT OF HAVING 'DOCTEST_CONFIG_SUPER_FAST_ASSERTS' DEFINED
         // ###################################################################################
         DOCTEST_ASSERT_OUT_OF_TESTS(result.m_decomp);
         DOCTEST_ASSERT_IN_TESTS(result.m_decomp);
+        return !failed;
     }
 
     MessageBuilder::MessageBuilder(const char* file, int line, assertType::Enum severity) {
-        m_stream   = getTlsOss();
+        m_stream   = tlssPush();
         m_file     = file;
         m_line     = line;
         m_severity = severity;
     }
 
-    IExceptionTranslator::IExceptionTranslator()  = default;
-    IExceptionTranslator::~IExceptionTranslator() = default;
+    MessageBuilder::~MessageBuilder() {
+        if (!logged)
+            tlssPop();
+    }
+
+    DOCTEST_DEFINE_INTERFACE(IExceptionTranslator)
 
     bool MessageBuilder::log() {
-        m_string = getTlsOssResult();
+        if (!logged) {
+            m_string = tlssPop();
+            logged = true;
+        }
+
         DOCTEST_ITERATE_THROUGH_REPORTERS(log_message, *this);
 
         const bool isWarn = m_severity & assertType::is_warn;
 
         // warn is just a message in this context so we don't treat it as an assert
         if(!isWarn) {
             addAssert(m_severity);
             addFailedAssert(m_severity);
         }
 
-        return isDebuggerActive() && !getContextOptions()->no_breaks && !isWarn; // break
+        return isDebuggerActive() && !getContextOptions()->no_breaks && !isWarn &&
+            (g_cs->currentTest == nullptr || !g_cs->currentTest->m_no_breaks); // break into debugger
     }
 
     void MessageBuilder::react() {
         if(m_severity & assertType::is_require) //!OCLINT bitwise operator in conditional
             throwException();
     }
-
-    MessageBuilder::~MessageBuilder() = default;
 } // namespace detail
 namespace {
     using namespace detail;
 
-    template <typename Ex>
-    DOCTEST_NORETURN void throw_exception(Ex const& e) {
-#ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
-        throw e;
-#else  // DOCTEST_CONFIG_NO_EXCEPTIONS
-        std::cerr << "doctest will terminate because it needed to throw an exception.\n"
-                  << "The message was: " << e.what() << '\n';
-        std::terminate();
-#endif // DOCTEST_CONFIG_NO_EXCEPTIONS
-    }
-
-#ifndef DOCTEST_INTERNAL_ERROR
-#define DOCTEST_INTERNAL_ERROR(msg)                                                                \
-    throw_exception(std::logic_error(                                                              \
-            __FILE__ ":" DOCTEST_TOSTR(__LINE__) ": Internal doctest error: " msg))
-#endif // DOCTEST_INTERNAL_ERROR
-
     // clang-format off
 
 // =================================================================================================
 // The following code has been taken verbatim from Catch2/include/internal/catch_xmlwriter.h/cpp
 // This is done so cherry-picking bug fixes is trivial - even the style/formatting is untouched.
 // =================================================================================================
 
@@ -4325,15 +5070,19 @@
                 return *this;
             }
 
         private:
             mutable XmlWriter* m_writer = nullptr;
         };
 
+#ifndef DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
         XmlWriter( std::ostream& os = std::cout );
+#else // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+        XmlWriter( std::ostream& os );
+#endif // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
         ~XmlWriter();
 
         XmlWriter( XmlWriter const& ) = delete;
         XmlWriter& operator=( XmlWriter const& ) = delete;
 
         XmlWriter& startElement( std::string const& name );
 
@@ -4360,18 +5109,18 @@
 
         //void writeStylesheetRef( std::string const& url );
 
         //XmlWriter& writeBlankLine();
 
         void ensureTagClosed();
 
-    private:
-
         void writeDeclaration();
 
+    private:
+
         void newlineIfNecessary();
 
         bool m_tagIsOpen = false;
         bool m_needsNewline = false;
         std::vector<std::string> m_tags;
         std::string m_indent;
         std::ostream& m_os;
@@ -4552,15 +5301,15 @@
     XmlWriter::ScopedElement& XmlWriter::ScopedElement::writeText( std::string const& text, bool indent ) {
         m_writer->writeText( text, indent );
         return *this;
     }
 
     XmlWriter::XmlWriter( std::ostream& os ) : m_os( os )
     {
-        writeDeclaration();
+        // writeDeclaration(); // called explicitly by the reporters that use the writer class - see issue #627
     }
 
     XmlWriter::~XmlWriter() {
         while( !m_tags.empty() )
             endElement();
     }
 
@@ -4663,16 +5412,16 @@
 // End of copy-pasted code from Catch
 // =================================================================================================
 
     // clang-format on
 
     struct XmlReporter : public IReporter
     {
-        XmlWriter  xml;
-        std::mutex mutex;
+        XmlWriter xml;
+        DOCTEST_DECLARE_MUTEX(mutex)
 
         // caching pointers/references to objects of these types - safe to do
         const ContextOptions& opt;
         const TestCaseData*   tc = nullptr;
 
         XmlReporter(const ContextOptions& co)
                 : xml(*co.cout)
@@ -4741,15 +5490,16 @@
                             .writeAttribute("priority", curr.first.first)
                             .writeAttribute("name", curr.first.second);
             } else if(opt.count || opt.list_test_cases) {
                 for(unsigned i = 0; i < in.num_data; ++i) {
                     xml.scopedElement("TestCase").writeAttribute("name", in.data[i]->m_name)
                         .writeAttribute("testsuite", in.data[i]->m_test_suite)
                         .writeAttribute("filename", skipPathFromFilename(in.data[i]->m_file.c_str()))
-                        .writeAttribute("line", line(in.data[i]->m_line));
+                        .writeAttribute("line", line(in.data[i]->m_line))
+                        .writeAttribute("skipped", in.data[i]->m_skip);
                 }
                 xml.scopedElement("OverallResultsTestCases")
                         .writeAttribute("unskipped", in.run_stats->numTestCasesPassingFilters);
             } else if(opt.list_test_suites) {
                 for(unsigned i = 0; i < in.num_data; ++i)
                     xml.scopedElement("TestSuite").writeAttribute("name", in.data[i]->m_test_suite);
                 xml.scopedElement("OverallResultsTestCases")
@@ -4757,14 +5507,16 @@
                 xml.scopedElement("OverallResultsTestSuites")
                         .writeAttribute("unskipped", in.run_stats->numTestSuitesPassingFilters);
             }
             xml.endElement();
         }
 
         void test_run_start() override {
+            xml.writeDeclaration();
+
             // remove .exe extension - mainly to have the same output on UNIX and Windows
             std::string binary_name = skipPathFromFilename(opt.binary_name.c_str());
 #ifdef DOCTEST_PLATFORM_WINDOWS
             if(binary_name.rfind(".exe") != std::string::npos)
                 binary_name = binary_name.substr(0, binary_name.length() - 4);
 #endif // DOCTEST_PLATFORM_WINDOWS
 
@@ -4804,56 +5556,55 @@
             xml.endElement();
         }
 
         void test_case_start(const TestCaseData& in) override {
             test_case_start_impl(in);
             xml.ensureTagClosed();
         }
-        
+
         void test_case_reenter(const TestCaseData&) override {}
 
         void test_case_end(const CurrentTestCaseStats& st) override {
             xml.startElement("OverallResultsAsserts")
                     .writeAttribute("successes",
                                     st.numAssertsCurrentTest - st.numAssertsFailedCurrentTest)
-                    .writeAttribute("failures", st.numAssertsFailedCurrentTest);
+                    .writeAttribute("failures", st.numAssertsFailedCurrentTest)
+                    .writeAttribute("test_case_success", st.testCaseSuccess);
             if(opt.duration)
                 xml.writeAttribute("duration", st.seconds);
             if(tc->m_expected_failures)
                 xml.writeAttribute("expected_failures", tc->m_expected_failures);
             xml.endElement();
 
             xml.endElement();
         }
 
         void test_case_exception(const TestCaseException& e) override {
-            std::lock_guard<std::mutex> lock(mutex);
+            DOCTEST_LOCK_MUTEX(mutex)
 
             xml.scopedElement("Exception")
                     .writeAttribute("crash", e.is_crash)
                     .writeText(e.error_string.c_str());
         }
 
         void subcase_start(const SubcaseSignature& in) override {
-            std::lock_guard<std::mutex> lock(mutex);
-
             xml.startElement("SubCase")
                     .writeAttribute("name", in.m_name)
                     .writeAttribute("filename", skipPathFromFilename(in.m_file))
                     .writeAttribute("line", line(in.m_line));
             xml.ensureTagClosed();
         }
 
         void subcase_end() override { xml.endElement(); }
 
         void log_assert(const AssertData& rb) override {
             if(!rb.m_failed && !opt.success)
                 return;
 
-            std::lock_guard<std::mutex> lock(mutex);
+            DOCTEST_LOCK_MUTEX(mutex)
 
             xml.startElement("Expression")
                     .writeAttribute("success", !rb.m_failed)
                     .writeAttribute("type", assertString(rb.m_at))
                     .writeAttribute("filename", skipPathFromFilename(rb.m_file))
                     .writeAttribute("line", line(rb.m_line));
 
@@ -4861,25 +5612,25 @@
 
             if(rb.m_threw)
                 xml.scopedElement("Exception").writeText(rb.m_exception.c_str());
 
             if(rb.m_at & assertType::is_throws_as)
                 xml.scopedElement("ExpectedException").writeText(rb.m_exception_type);
             if(rb.m_at & assertType::is_throws_with)
-                xml.scopedElement("ExpectedExceptionString").writeText(rb.m_exception_string);
+                xml.scopedElement("ExpectedExceptionString").writeText(rb.m_exception_string.c_str());
             if((rb.m_at & assertType::is_normal) && !rb.m_threw)
                 xml.scopedElement("Expanded").writeText(rb.m_decomp.c_str());
 
             log_contexts();
 
             xml.endElement();
         }
 
         void log_message(const MessageData& mb) override {
-            std::lock_guard<std::mutex> lock(mutex);
+            DOCTEST_LOCK_MUTEX(mutex)
 
             xml.startElement("Message")
                     .writeAttribute("type", failureString(mb.m_severity))
                     .writeAttribute("filename", skipPathFromFilename(mb.m_file))
                     .writeAttribute("line", line(mb.m_line));
 
             xml.scopedElement("Text").writeText(mb.m_string.c_str());
@@ -4896,14 +5647,307 @@
                 xml.endElement();
             }
         }
     };
 
     DOCTEST_REGISTER_REPORTER("xml", 0, XmlReporter);
 
+    void fulltext_log_assert_to_stream(std::ostream& s, const AssertData& rb) {
+        if((rb.m_at & (assertType::is_throws_as | assertType::is_throws_with)) ==
+            0) //!OCLINT bitwise operator in conditional
+            s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << " ) "
+                << Color::None;
+
+        if(rb.m_at & assertType::is_throws) { //!OCLINT bitwise operator in conditional
+            s << (rb.m_threw ? "threw as expected!" : "did NOT throw at all!") << "\n";
+        } else if((rb.m_at & assertType::is_throws_as) &&
+                    (rb.m_at & assertType::is_throws_with)) { //!OCLINT
+            s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", \""
+                << rb.m_exception_string.c_str()
+                << "\", " << rb.m_exception_type << " ) " << Color::None;
+            if(rb.m_threw) {
+                if(!rb.m_failed) {
+                    s << "threw as expected!\n";
+                } else {
+                    s << "threw a DIFFERENT exception! (contents: " << rb.m_exception << ")\n";
+                }
+            } else {
+                s << "did NOT throw at all!\n";
+            }
+        } else if(rb.m_at &
+                    assertType::is_throws_as) { //!OCLINT bitwise operator in conditional
+            s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", "
+                << rb.m_exception_type << " ) " << Color::None
+                << (rb.m_threw ? (rb.m_threw_as ? "threw as expected!" :
+                                                "threw a DIFFERENT exception: ") :
+                                "did NOT throw at all!")
+                << Color::Cyan << rb.m_exception << "\n";
+        } else if(rb.m_at &
+                    assertType::is_throws_with) { //!OCLINT bitwise operator in conditional
+            s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", \""
+                << rb.m_exception_string.c_str()
+                << "\" ) " << Color::None
+                << (rb.m_threw ? (!rb.m_failed ? "threw as expected!" :
+                                                "threw a DIFFERENT exception: ") :
+                                "did NOT throw at all!")
+                << Color::Cyan << rb.m_exception << "\n";
+        } else if(rb.m_at & assertType::is_nothrow) { //!OCLINT bitwise operator in conditional
+            s << (rb.m_threw ? "THREW exception: " : "didn't throw!") << Color::Cyan
+                << rb.m_exception << "\n";
+        } else {
+            s << (rb.m_threw ? "THREW exception: " :
+                                (!rb.m_failed ? "is correct!\n" : "is NOT correct!\n"));
+            if(rb.m_threw)
+                s << rb.m_exception << "\n";
+            else
+                s << "  values: " << assertString(rb.m_at) << "( " << rb.m_decomp << " )\n";
+        }
+    }
+
+    // TODO:
+    // - log_message()
+    // - respond to queries
+    // - honor remaining options
+    // - more attributes in tags
+    struct JUnitReporter : public IReporter
+    {
+        XmlWriter xml;
+        DOCTEST_DECLARE_MUTEX(mutex)
+        Timer timer;
+        std::vector<String> deepestSubcaseStackNames;
+
+        struct JUnitTestCaseData
+        {
+            static std::string getCurrentTimestamp() {
+                // Beware, this is not reentrant because of backward compatibility issues
+                // Also, UTC only, again because of backward compatibility (%z is C++11)
+                time_t rawtime;
+                std::time(&rawtime);
+                auto const timeStampSize = sizeof("2017-01-16T17:06:45Z");
+
+                std::tm timeInfo;
+#ifdef DOCTEST_PLATFORM_WINDOWS
+                gmtime_s(&timeInfo, &rawtime);
+#else // DOCTEST_PLATFORM_WINDOWS
+                gmtime_r(&rawtime, &timeInfo);
+#endif // DOCTEST_PLATFORM_WINDOWS
+
+                char timeStamp[timeStampSize];
+                const char* const fmt = "%Y-%m-%dT%H:%M:%SZ";
+
+                std::strftime(timeStamp, timeStampSize, fmt, &timeInfo);
+                return std::string(timeStamp);
+            }
+
+            struct JUnitTestMessage
+            {
+                JUnitTestMessage(const std::string& _message, const std::string& _type, const std::string& _details)
+                    : message(_message), type(_type), details(_details) {}
+
+                JUnitTestMessage(const std::string& _message, const std::string& _details)
+                    : message(_message), type(), details(_details) {}
+
+                std::string message, type, details;
+            };
+
+            struct JUnitTestCase
+            {
+                JUnitTestCase(const std::string& _classname, const std::string& _name)
+                    : classname(_classname), name(_name), time(0), failures() {}
+
+                std::string classname, name;
+                double time;
+                std::vector<JUnitTestMessage> failures, errors;
+            };
+
+            void add(const std::string& classname, const std::string& name) {
+                testcases.emplace_back(classname, name);
+            }
+
+            void appendSubcaseNamesToLastTestcase(std::vector<String> nameStack) {
+                for(auto& curr: nameStack)
+                    if(curr.size())
+                        testcases.back().name += std::string("/") + curr.c_str();
+            }
+
+            void addTime(double time) {
+                if(time < 1e-4)
+                    time = 0;
+                testcases.back().time = time;
+                totalSeconds += time;
+            }
+
+            void addFailure(const std::string& message, const std::string& type, const std::string& details) {
+                testcases.back().failures.emplace_back(message, type, details);
+                ++totalFailures;
+            }
+
+            void addError(const std::string& message, const std::string& details) {
+                testcases.back().errors.emplace_back(message, details);
+                ++totalErrors;
+            }
+
+            std::vector<JUnitTestCase> testcases;
+            double totalSeconds = 0;
+            int totalErrors = 0, totalFailures = 0;
+        };
+
+        JUnitTestCaseData testCaseData;
+
+        // caching pointers/references to objects of these types - safe to do
+        const ContextOptions& opt;
+        const TestCaseData*   tc = nullptr;
+
+        JUnitReporter(const ContextOptions& co)
+                : xml(*co.cout)
+                , opt(co) {}
+
+        unsigned line(unsigned l) const { return opt.no_line_numbers ? 0 : l; }
+
+        // =========================================================================================
+        // WHAT FOLLOWS ARE OVERRIDES OF THE VIRTUAL METHODS OF THE REPORTER INTERFACE
+        // =========================================================================================
+
+        void report_query(const QueryData&) override {
+            xml.writeDeclaration();
+        }
+
+        void test_run_start() override {
+            xml.writeDeclaration();
+        }
+
+        void test_run_end(const TestRunStats& p) override {
+            // remove .exe extension - mainly to have the same output on UNIX and Windows
+            std::string binary_name = skipPathFromFilename(opt.binary_name.c_str());
+#ifdef DOCTEST_PLATFORM_WINDOWS
+            if(binary_name.rfind(".exe") != std::string::npos)
+                binary_name = binary_name.substr(0, binary_name.length() - 4);
+#endif // DOCTEST_PLATFORM_WINDOWS
+            xml.startElement("testsuites");
+            xml.startElement("testsuite").writeAttribute("name", binary_name)
+                    .writeAttribute("errors", testCaseData.totalErrors)
+                    .writeAttribute("failures", testCaseData.totalFailures)
+                    .writeAttribute("tests", p.numAsserts);
+            if(opt.no_time_in_output == false) {
+                xml.writeAttribute("time", testCaseData.totalSeconds);
+                xml.writeAttribute("timestamp", JUnitTestCaseData::getCurrentTimestamp());
+            }
+            if(opt.no_version == false)
+                xml.writeAttribute("doctest_version", DOCTEST_VERSION_STR);
+
+            for(const auto& testCase : testCaseData.testcases) {
+                xml.startElement("testcase")
+                    .writeAttribute("classname", testCase.classname)
+                    .writeAttribute("name", testCase.name);
+                if(opt.no_time_in_output == false)
+                    xml.writeAttribute("time", testCase.time);
+                // This is not ideal, but it should be enough to mimic gtest's junit output.
+                xml.writeAttribute("status", "run");
+
+                for(const auto& failure : testCase.failures) {
+                    xml.scopedElement("failure")
+                        .writeAttribute("message", failure.message)
+                        .writeAttribute("type", failure.type)
+                        .writeText(failure.details, false);
+                }
+
+                for(const auto& error : testCase.errors) {
+                    xml.scopedElement("error")
+                        .writeAttribute("message", error.message)
+                        .writeText(error.details);
+                }
+
+                xml.endElement();
+            }
+            xml.endElement();
+            xml.endElement();
+        }
+
+        void test_case_start(const TestCaseData& in) override {
+            testCaseData.add(skipPathFromFilename(in.m_file.c_str()), in.m_name);
+            timer.start();
+        }
+
+        void test_case_reenter(const TestCaseData& in) override {
+            testCaseData.addTime(timer.getElapsedSeconds());
+            testCaseData.appendSubcaseNamesToLastTestcase(deepestSubcaseStackNames);
+            deepestSubcaseStackNames.clear();
+
+            timer.start();
+            testCaseData.add(skipPathFromFilename(in.m_file.c_str()), in.m_name);
+        }
+
+        void test_case_end(const CurrentTestCaseStats&) override {
+            testCaseData.addTime(timer.getElapsedSeconds());
+            testCaseData.appendSubcaseNamesToLastTestcase(deepestSubcaseStackNames);
+            deepestSubcaseStackNames.clear();
+        }
+
+        void test_case_exception(const TestCaseException& e) override {
+            DOCTEST_LOCK_MUTEX(mutex)
+            testCaseData.addError("exception", e.error_string.c_str());
+        }
+
+        void subcase_start(const SubcaseSignature& in) override {
+            deepestSubcaseStackNames.push_back(in.m_name);
+        }
+
+        void subcase_end() override {}
+
+        void log_assert(const AssertData& rb) override {
+            if(!rb.m_failed) // report only failures & ignore the `success` option
+                return;
+
+            DOCTEST_LOCK_MUTEX(mutex)
+
+            std::ostringstream os;
+            os << skipPathFromFilename(rb.m_file) << (opt.gnu_file_line ? ":" : "(")
+              << line(rb.m_line) << (opt.gnu_file_line ? ":" : "):") << std::endl;
+
+            fulltext_log_assert_to_stream(os, rb);
+            log_contexts(os);
+            testCaseData.addFailure(rb.m_decomp.c_str(), assertString(rb.m_at), os.str());
+        }
+
+        void log_message(const MessageData& mb) override {
+            if(mb.m_severity & assertType::is_warn) // report only failures
+                return;
+
+            DOCTEST_LOCK_MUTEX(mutex)
+
+            std::ostringstream os;
+            os << skipPathFromFilename(mb.m_file) << (opt.gnu_file_line ? ":" : "(")
+              << line(mb.m_line) << (opt.gnu_file_line ? ":" : "):") << std::endl;
+
+            os << mb.m_string.c_str() << "\n";
+            log_contexts(os);
+
+            testCaseData.addFailure(mb.m_string.c_str(),
+                mb.m_severity & assertType::is_check ? "FAIL_CHECK" : "FAIL", os.str());
+        }
+
+        void test_case_skipped(const TestCaseData&) override {}
+
+        void log_contexts(std::ostringstream& s) {
+            int num_contexts = get_num_active_contexts();
+            if(num_contexts) {
+                auto contexts = get_active_contexts();
+
+                s << "  logged: ";
+                for(int i = 0; i < num_contexts; ++i) {
+                    s << (i == 0 ? "" : "          ");
+                    contexts[i]->stringify(&s);
+                    s << std::endl;
+                }
+            }
+        }
+    };
+
+    DOCTEST_REGISTER_REPORTER("junit", 0, JUnitReporter);
+
     struct Whitespace
     {
         int nrSpaces;
         explicit Whitespace(int nr)
                 : nrSpaces(nr) {}
     };
 
@@ -4915,15 +5959,15 @@
 
     struct ConsoleReporter : public IReporter
     {
         std::ostream&                 s;
         bool                          hasLoggedCurrentTestStart;
         std::vector<SubcaseSignature> subcasesStack;
         size_t                        currentSubcaseLevel;
-        std::mutex                    mutex;
+        DOCTEST_DECLARE_MUTEX(mutex)
 
         // caching pointers/references to objects of these types - safe to do
         const ContextOptions& opt;
         const TestCaseData*   tc;
 
         ConsoleReporter(const ContextOptions& co)
                 : s(*co.cout)
@@ -4973,14 +6017,15 @@
                     s << "\n";
                 }
             }
 
             s << "\n";
         }
 
+        // this was requested to be made virtual so users could override it
         virtual void file_line_to_stream(const char* file, int line,
                                         const char* tail = "") {
             s << Color::LightGrey << skipPathFromFilename(file) << (opt.gnu_file_line ? ":" : "(")
             << (opt.no_line_numbers ? 0 : line) // 0 or the real num depending on the option
             << (opt.gnu_file_line ? ":" : "):") << tail;
         }
 
@@ -5019,17 +6064,19 @@
         void printVersion() {
             if(opt.no_version == false)
                 s << Color::Cyan << "[doctest] " << Color::None << "doctest version is \""
                   << DOCTEST_VERSION_STR << "\"\n";
         }
 
         void printIntro() {
-            printVersion();
-            s << Color::Cyan << "[doctest] " << Color::None
-              << "run with \"--" DOCTEST_OPTIONS_PREFIX_DISPLAY "help\" for options\n";
+            if(opt.no_intro == false) {
+                printVersion();
+                s << Color::Cyan << "[doctest] " << Color::None
+                  << "run with \"--" DOCTEST_OPTIONS_PREFIX_DISPLAY "help\" for options\n";
+            }
         }
 
         void printHelp() {
             int sizePrefixDisplay = static_cast<int>(strlen(DOCTEST_OPTIONS_PREFIX_DISPLAY));
             printVersion();
             // clang-format off
             s << Color::Cyan << "[doctest]\n" << Color::None;
@@ -5083,15 +6130,15 @@
               << Whitespace(sizePrefixDisplay*1) << "filters OUT subcases by their name\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "r,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "reporters=<filters>           "
               << Whitespace(sizePrefixDisplay*1) << "reporters to use (console is default)\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "o,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "out=<string>                  "
               << Whitespace(sizePrefixDisplay*1) << "output filename\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "ob,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "order-by=<string>             "
               << Whitespace(sizePrefixDisplay*1) << "how the tests should be ordered\n";
-            s << Whitespace(sizePrefixDisplay*3) << "                                       <string> - by [file/suite/name/rand]\n";
+            s << Whitespace(sizePrefixDisplay*3) << "                                       <string> - [file/suite/name/rand/none]\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "rs,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "rand-seed=<int>               "
               << Whitespace(sizePrefixDisplay*1) << "seed for random ordering\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "f,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "first=<int>                   "
               << Whitespace(sizePrefixDisplay*1) << "the first test passing the filters to\n";
             s << Whitespace(sizePrefixDisplay*3) << "                                       execute - for range-based execution\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "l,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "last=<int>                    "
               << Whitespace(sizePrefixDisplay*1) << "the last test passing the filters to\n";
@@ -5106,20 +6153,26 @@
               << Whitespace(sizePrefixDisplay*1) << "include successful assertions in output\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "cs,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "case-sensitive=<bool>         "
               << Whitespace(sizePrefixDisplay*1) << "filters being treated as case sensitive\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "e,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "exit=<bool>                   "
               << Whitespace(sizePrefixDisplay*1) << "exits after the tests finish\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "d,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "duration=<bool>               "
               << Whitespace(sizePrefixDisplay*1) << "prints the time duration of each test\n";
+            s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "m,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "minimal=<bool>                "
+              << Whitespace(sizePrefixDisplay*1) << "minimal console output (only failures)\n";
+            s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "q,   --" DOCTEST_OPTIONS_PREFIX_DISPLAY "quiet=<bool>                  "
+              << Whitespace(sizePrefixDisplay*1) << "no console output\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "nt,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-throw=<bool>               "
               << Whitespace(sizePrefixDisplay*1) << "skips exceptions-related assert checks\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "ne,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-exitcode=<bool>            "
               << Whitespace(sizePrefixDisplay*1) << "returns (or exits) always with success\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "nr,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-run=<bool>                 "
               << Whitespace(sizePrefixDisplay*1) << "skips all runtime doctest operations\n";
+            s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "ni,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-intro=<bool>               "
+              << Whitespace(sizePrefixDisplay*1) << "omit the framework intro in the output\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "nv,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-version=<bool>             "
               << Whitespace(sizePrefixDisplay*1) << "omit the framework version in the output\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "nc,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-colors=<bool>              "
               << Whitespace(sizePrefixDisplay*1) << "disables colors in output\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "fc,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "force-colors=<bool>           "
               << Whitespace(sizePrefixDisplay*1) << "use colors even when not in a tty\n";
             s << " -" DOCTEST_OPTIONS_PREFIX_DISPLAY "nb,  --" DOCTEST_OPTIONS_PREFIX_DISPLAY "no-breaks=<bool>              "
@@ -5149,30 +6202,14 @@
                           << " name: " << curr.first.second << "\n";
                 }
             };
             printReporters(getListeners(), "listeners");
             printReporters(getReporters(), "reporters");
         }
 
-        void list_query_results() {
-            separator_to_stream();
-            if(opt.count || opt.list_test_cases) {
-                s << Color::Cyan << "[doctest] " << Color::None
-                  << "unskipped test cases passing the current filters: "
-                  << g_cs->numTestCasesPassingFilters << "\n";
-            } else if(opt.list_test_suites) {
-                s << Color::Cyan << "[doctest] " << Color::None
-                  << "unskipped test cases passing the current filters: "
-                  << g_cs->numTestCasesPassingFilters << "\n";
-                s << Color::Cyan << "[doctest] " << Color::None
-                  << "test suites with unskipped test cases passing the current filters: "
-                  << g_cs->numTestSuitesPassingFilters << "\n";
-            }
-        }
-
         // =========================================================================================
         // WHAT FOLLOWS ARE OVERRIDES OF THE VIRTUAL METHODS OF THE REPORTER INTERFACE
         // =========================================================================================
 
         void report_query(const QueryData& in) override {
             if(opt.version) {
                 printVersion();
@@ -5210,61 +6247,73 @@
                   << g_cs->numTestCasesPassingFilters << "\n";
                 s << Color::Cyan << "[doctest] " << Color::None
                   << "test suites with unskipped test cases passing the current filters: "
                   << g_cs->numTestSuitesPassingFilters << "\n";
             }
         }
 
-        void test_run_start() override { printIntro(); }
+        void test_run_start() override {
+            if(!opt.minimal)
+                printIntro();
+        }
 
         void test_run_end(const TestRunStats& p) override {
+            if(opt.minimal && p.numTestCasesFailed == 0)
+                return;
+
             separator_to_stream();
             s << std::dec;
 
+            auto totwidth = int(std::ceil(log10(static_cast<double>(std::max(p.numTestCasesPassingFilters, static_cast<unsigned>(p.numAsserts))) + 1)));
+            auto passwidth = int(std::ceil(log10(static_cast<double>(std::max(p.numTestCasesPassingFilters - p.numTestCasesFailed, static_cast<unsigned>(p.numAsserts - p.numAssertsFailed))) + 1)));
+            auto failwidth = int(std::ceil(log10(static_cast<double>(std::max(p.numTestCasesFailed, static_cast<unsigned>(p.numAssertsFailed))) + 1)));
             const bool anythingFailed = p.numTestCasesFailed > 0 || p.numAssertsFailed > 0;
-            s << Color::Cyan << "[doctest] " << Color::None << "test cases: " << std::setw(6)
+            s << Color::Cyan << "[doctest] " << Color::None << "test cases: " << std::setw(totwidth)
               << p.numTestCasesPassingFilters << " | "
               << ((p.numTestCasesPassingFilters == 0 || anythingFailed) ? Color::None :
                                                                           Color::Green)
-              << std::setw(6) << p.numTestCasesPassingFilters - p.numTestCasesFailed << " passed"
+              << std::setw(passwidth) << p.numTestCasesPassingFilters - p.numTestCasesFailed << " passed"
               << Color::None << " | " << (p.numTestCasesFailed > 0 ? Color::Red : Color::None)
-              << std::setw(6) << p.numTestCasesFailed << " failed" << Color::None << " | ";
+              << std::setw(failwidth) << p.numTestCasesFailed << " failed" << Color::None << " |";
             if(opt.no_skipped_summary == false) {
                 const int numSkipped = p.numTestCases - p.numTestCasesPassingFilters;
-                s << (numSkipped == 0 ? Color::None : Color::Yellow) << std::setw(6) << numSkipped
+                s << " " << (numSkipped == 0 ? Color::None : Color::Yellow) << numSkipped
                   << " skipped" << Color::None;
             }
             s << "\n";
-            s << Color::Cyan << "[doctest] " << Color::None << "assertions: " << std::setw(6)
+            s << Color::Cyan << "[doctest] " << Color::None << "assertions: " << std::setw(totwidth)
               << p.numAsserts << " | "
               << ((p.numAsserts == 0 || anythingFailed) ? Color::None : Color::Green)
-              << std::setw(6) << (p.numAsserts - p.numAssertsFailed) << " passed" << Color::None
-              << " | " << (p.numAssertsFailed > 0 ? Color::Red : Color::None) << std::setw(6)
+              << std::setw(passwidth) << (p.numAsserts - p.numAssertsFailed) << " passed" << Color::None
+              << " | " << (p.numAssertsFailed > 0 ? Color::Red : Color::None) << std::setw(failwidth)
               << p.numAssertsFailed << " failed" << Color::None << " |\n";
             s << Color::Cyan << "[doctest] " << Color::None
               << "Status: " << (p.numTestCasesFailed > 0 ? Color::Red : Color::Green)
               << ((p.numTestCasesFailed > 0) ? "FAILURE!" : "SUCCESS!") << Color::None << std::endl;
         }
 
         void test_case_start(const TestCaseData& in) override {
             hasLoggedCurrentTestStart = false;
             tc                        = &in;
             subcasesStack.clear();
             currentSubcaseLevel = 0;
         }
-        
+
         void test_case_reenter(const TestCaseData&) override {
             subcasesStack.clear();
         }
 
         void test_case_end(const CurrentTestCaseStats& st) override {
+            if(tc->m_no_output)
+                return;
+
             // log the preamble of the test case only if there is something
             // else to print - something other than that an assert has failed
             if(opt.duration ||
-               (st.failure_flags && st.failure_flags != TestCaseFailureReason::AssertFailure))
+               (st.failure_flags && st.failure_flags != static_cast<int>(TestCaseFailureReason::AssertFailure)))
                 logTestStart();
 
             if(opt.duration)
                 s << Color::None << std::setprecision(6) << std::fixed << st.seconds
                   << " s: " << tc->m_name << "\n";
 
             if(st.failure_flags & TestCaseFailureReason::Timeout)
@@ -5287,14 +6336,18 @@
             if(st.failure_flags & TestCaseFailureReason::TooManyFailedAsserts) {
                 s << Color::Red << "Aborting - too many failed asserts!\n";
             }
             s << Color::None; // lgtm [cpp/useless-expression]
         }
 
         void test_case_exception(const TestCaseException& e) override {
+            DOCTEST_LOCK_MUTEX(mutex)
+            if(tc->m_no_output)
+                return;
+
             logTestStart();
 
             file_line_to_stream(tc->m_file.c_str(), tc->m_line, " ");
             successOrFailColoredStringToStream(false, e.is_crash ? assertType::is_require :
                                                                    assertType::is_check);
             s << Color::Red << (e.is_crash ? "test case CRASHED: " : "test case THREW exception: ")
               << Color::Cyan << e.error_string << "\n";
@@ -5308,89 +6361,45 @@
                       << stringified_contexts[i - 1] << "\n";
                 }
             }
             s << "\n" << Color::None;
         }
 
         void subcase_start(const SubcaseSignature& subc) override {
-            std::lock_guard<std::mutex> lock(mutex);
             subcasesStack.push_back(subc);
             ++currentSubcaseLevel;
             hasLoggedCurrentTestStart = false;
         }
 
         void subcase_end() override {
-            std::lock_guard<std::mutex> lock(mutex);
             --currentSubcaseLevel;
             hasLoggedCurrentTestStart = false;
         }
 
         void log_assert(const AssertData& rb) override {
-            if(!rb.m_failed && !opt.success)
+            if((!rb.m_failed && !opt.success) || tc->m_no_output)
                 return;
 
-            std::lock_guard<std::mutex> lock(mutex);
+            DOCTEST_LOCK_MUTEX(mutex)
 
             logTestStart();
 
             file_line_to_stream(rb.m_file, rb.m_line, " ");
             successOrFailColoredStringToStream(!rb.m_failed, rb.m_at);
-            if((rb.m_at & (assertType::is_throws_as | assertType::is_throws_with)) ==
-               0) //!OCLINT bitwise operator in conditional
-                s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << " ) "
-                  << Color::None;
-
-            if(rb.m_at & assertType::is_throws) { //!OCLINT bitwise operator in conditional
-                s << (rb.m_threw ? "threw as expected!" : "did NOT throw at all!") << "\n";
-            } else if((rb.m_at & assertType::is_throws_as) &&
-                      (rb.m_at & assertType::is_throws_with)) { //!OCLINT
-                s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", \""
-                  << rb.m_exception_string << "\", " << rb.m_exception_type << " ) " << Color::None;
-                if(rb.m_threw) {
-                    if(!rb.m_failed) {
-                        s << "threw as expected!\n";
-                    } else {
-                        s << "threw a DIFFERENT exception! (contents: " << rb.m_exception << ")\n";
-                    }
-                } else {
-                    s << "did NOT throw at all!\n";
-                }
-            } else if(rb.m_at &
-                      assertType::is_throws_as) { //!OCLINT bitwise operator in conditional
-                s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", "
-                  << rb.m_exception_type << " ) " << Color::None
-                  << (rb.m_threw ? (rb.m_threw_as ? "threw as expected!" :
-                                                    "threw a DIFFERENT exception: ") :
-                                   "did NOT throw at all!")
-                  << Color::Cyan << rb.m_exception << "\n";
-            } else if(rb.m_at &
-                      assertType::is_throws_with) { //!OCLINT bitwise operator in conditional
-                s << Color::Cyan << assertString(rb.m_at) << "( " << rb.m_expr << ", \""
-                  << rb.m_exception_string << "\" ) " << Color::None
-                  << (rb.m_threw ? (!rb.m_failed ? "threw as expected!" :
-                                                   "threw a DIFFERENT exception: ") :
-                                   "did NOT throw at all!")
-                  << Color::Cyan << rb.m_exception << "\n";
-            } else if(rb.m_at & assertType::is_nothrow) { //!OCLINT bitwise operator in conditional
-                s << (rb.m_threw ? "THREW exception: " : "didn't throw!") << Color::Cyan
-                  << rb.m_exception << "\n";
-            } else {
-                s << (rb.m_threw ? "THREW exception: " :
-                                   (!rb.m_failed ? "is correct!\n" : "is NOT correct!\n"));
-                if(rb.m_threw)
-                    s << rb.m_exception << "\n";
-                else
-                    s << "  values: " << assertString(rb.m_at) << "( " << rb.m_decomp << " )\n";
-            }
+
+            fulltext_log_assert_to_stream(s, rb);
 
             log_contexts();
         }
 
         void log_message(const MessageData& mb) override {
-            std::lock_guard<std::mutex> lock(mutex);
+            if(tc->m_no_output)
+                return;
+
+            DOCTEST_LOCK_MUTEX(mutex)
 
             logTestStart();
 
             file_line_to_stream(mb.m_file, mb.m_line, " ");
             s << getSuccessOrFailColor(false, mb.m_severity)
               << getSuccessOrFailString(mb.m_severity & assertType::is_warn, mb.m_severity,
                                         "MESSAGE") << ": ";
@@ -5412,16 +6421,18 @@
                 : ConsoleReporter(co, oss) {}
 
 #define DOCTEST_DEBUG_OUTPUT_REPORTER_OVERRIDE(func, type, arg)                                    \
     void func(type arg) override {                                                                 \
         bool with_col = g_no_colors;                                                               \
         g_no_colors   = false;                                                                     \
         ConsoleReporter::func(arg);                                                                \
-        DOCTEST_OUTPUT_DEBUG_STRING(oss.str().c_str());                                            \
-        oss.str("");                                                                               \
+        if(oss.tellp() != std::streampos{}) {                                                      \
+            DOCTEST_OUTPUT_DEBUG_STRING(oss.str().c_str());                                        \
+            oss.str("");                                                                           \
+        }                                                                                          \
         g_no_colors = with_col;                                                                    \
     }
 
         DOCTEST_DEBUG_OUTPUT_REPORTER_OVERRIDE(test_run_start, DOCTEST_EMPTY, DOCTEST_EMPTY)
         DOCTEST_DEBUG_OUTPUT_REPORTER_OVERRIDE(test_run_end, const TestRunStats&, in)
         DOCTEST_DEBUG_OUTPUT_REPORTER_OVERRIDE(test_case_start, const TestCaseData&, in)
         DOCTEST_DEBUG_OUTPUT_REPORTER_OVERRIDE(test_case_reenter, const TestCaseData&, in)
@@ -5491,26 +6502,50 @@
     }
 
     // parses a comma separated list of words after a pattern in one of the arguments in argv
     bool parseCommaSepArgs(int argc, const char* const* argv, const char* pattern,
                            std::vector<String>& res) {
         String filtersString;
         if(parseOption(argc, argv, pattern, &filtersString)) {
-            // tokenize with "," as a separator
-            // cppcheck-suppress strtokCalled
-            DOCTEST_CLANG_SUPPRESS_WARNING_WITH_PUSH("-Wdeprecated-declarations")
-            auto pch = std::strtok(filtersString.c_str(), ","); // modifies the string
-            while(pch != nullptr) {
-                if(strlen(pch))
-                    res.push_back(pch);
-                // uses the strtok() internal state to go to the next token
-                // cppcheck-suppress strtokCalled
-                pch = std::strtok(nullptr, ",");
+            // tokenize with "," as a separator, unless escaped with backslash
+            std::ostringstream s;
+            auto flush = [&s, &res]() {
+                auto string = s.str();
+                if(string.size() > 0) {
+                    res.push_back(string.c_str());
+                }
+                s.str("");
+            };
+
+            bool seenBackslash = false;
+            const char* current = filtersString.c_str();
+            const char* end = current + strlen(current);
+            while(current != end) {
+                char character = *current++;
+                if(seenBackslash) {
+                    seenBackslash = false;
+                    if(character == ',' || character == '\\') {
+                        s.put(character);
+                        continue;
+                    }
+                    s.put('\\');
+                }
+                if(character == '\\') {
+                    seenBackslash = true;
+                } else if(character == ',') {
+                    flush();
+                } else {
+                    s.put(character);
+                }
+            }
+
+            if(seenBackslash) {
+                s.put('\\');
             }
-            DOCTEST_CLANG_SUPPRESS_WARNING_POP
+            flush();
             return true;
         }
         return false;
     }
 
     enum optionType
     {
@@ -5521,38 +6556,38 @@
     // parses an int/bool option from the command line
     bool parseIntOption(int argc, const char* const* argv, const char* pattern, optionType type,
                         int& res) {
         String parsedValue;
         if(!parseOption(argc, argv, pattern, &parsedValue))
             return false;
 
-        if(type == 0) {
+        if(type) {
+            // integer
+            // TODO: change this to use std::stoi or something else! currently it uses undefined behavior - assumes '0' on failed parse...
+            int theInt = std::atoi(parsedValue.c_str());
+            if (theInt != 0) {
+                res = theInt; //!OCLINT parameter reassignment
+                return true;
+            }
+        } else {
             // boolean
-            const char positive[][5] = {"1", "true", "on", "yes"};  // 5 - strlen("true") + 1
-            const char negative[][6] = {"0", "false", "off", "no"}; // 6 - strlen("false") + 1
+            const char positive[][5] = { "1", "true", "on", "yes" };  // 5 - strlen("true") + 1
+            const char negative[][6] = { "0", "false", "off", "no" }; // 6 - strlen("false") + 1
 
             // if the value matches any of the positive/negative possibilities
-            for(unsigned i = 0; i < 4; i++) {
-                if(parsedValue.compare(positive[i], true) == 0) {
+            for (unsigned i = 0; i < 4; i++) {
+                if (parsedValue.compare(positive[i], true) == 0) {
                     res = 1; //!OCLINT parameter reassignment
                     return true;
                 }
-                if(parsedValue.compare(negative[i], true) == 0) {
+                if (parsedValue.compare(negative[i], true) == 0) {
                     res = 0; //!OCLINT parameter reassignment
                     return true;
                 }
             }
-        } else {
-            // integer
-            // TODO: change this to use std::stoi or something else! currently it uses undefined behavior - assumes '0' on failed parse...
-            int theInt = std::atoi(parsedValue.c_str()); // NOLINT
-            if(theInt != 0) {
-                res = theInt; //!OCLINT parameter reassignment
-                return true;
-            }
         }
         return false;
     }
 } // namespace
 
 Context::Context(int argc, const char* const* argv)
         : p(new detail::ContextState) {
@@ -5600,15 +6635,15 @@
 
     int    intRes = 0;
     String strRes;
 
 #define DOCTEST_PARSE_AS_BOOL_OR_FLAG(name, sname, var, default)                                   \
     if(parseIntOption(argc, argv, DOCTEST_CONFIG_OPTIONS_PREFIX name "=", option_bool, intRes) ||  \
        parseIntOption(argc, argv, DOCTEST_CONFIG_OPTIONS_PREFIX sname "=", option_bool, intRes))   \
-        p->var = !!intRes;                                                                         \
+        p->var = static_cast<bool>(intRes);                                                        \
     else if(parseFlag(argc, argv, DOCTEST_CONFIG_OPTIONS_PREFIX name) ||                           \
             parseFlag(argc, argv, DOCTEST_CONFIG_OPTIONS_PREFIX sname))                            \
         p->var = true;                                                                             \
     else if(withDefaults)                                                                          \
     p->var = default
 
 #define DOCTEST_PARSE_INT_OPTION(name, sname, var, default)                                        \
@@ -5635,26 +6670,31 @@
     DOCTEST_PARSE_INT_OPTION("abort-after", "aa", abort_after, 0);
     DOCTEST_PARSE_INT_OPTION("subcase-filter-levels", "scfl", subcase_filter_levels, INT_MAX);
 
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("success", "s", success, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("case-sensitive", "cs", case_sensitive, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("exit", "e", exit, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("duration", "d", duration, false);
+    DOCTEST_PARSE_AS_BOOL_OR_FLAG("minimal", "m", minimal, false);
+    DOCTEST_PARSE_AS_BOOL_OR_FLAG("quiet", "q", quiet, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-throw", "nt", no_throw, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-exitcode", "ne", no_exitcode, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-run", "nr", no_run, false);
+    DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-intro", "ni", no_intro, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-version", "nv", no_version, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-colors", "nc", no_colors, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("force-colors", "fc", force_colors, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-breaks", "nb", no_breaks, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-skip", "ns", no_skip, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("gnu-file-line", "gfl", gnu_file_line, !bool(DOCTEST_MSVC));
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-path-filenames", "npf", no_path_in_filenames, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-line-numbers", "nln", no_line_numbers, false);
+    DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-debug-output", "ndo", no_debug_output, false);
     DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-skipped-summary", "nss", no_skipped_summary, false);
+    DOCTEST_PARSE_AS_BOOL_OR_FLAG("no-time-in-output", "ntio", no_time_in_output, false);
     // clang-format on
 
     if(withDefaults) {
         p->help             = false;
         p->version          = false;
         p->count            = false;
         p->list_test_cases  = false;
@@ -5699,15 +6739,20 @@
 
 // allows the user to clear all filters from the command line
 void Context::clearFilters() {
     for(auto& curr : p->filters)
         curr.clear();
 }
 
-// allows the user to override procedurally the int/bool options from the command line
+// allows the user to override procedurally the bool options from the command line
+void Context::setOption(const char* option, bool value) {
+    setOption(option, value ? "true" : "false");
+}
+
+// allows the user to override procedurally the int options from the command line
 void Context::setOption(const char* option, int value) {
     setOption(option, toString(value).c_str());
 }
 
 // allows the user to override procedurally the string options from the command line
 void Context::setOption(const char* option, const char* value) {
     auto argv   = String("-") + option + "=" + value;
@@ -5718,36 +6763,68 @@
 // users should query this in their main() and exit the program if true
 bool Context::shouldExit() { return p->exit; }
 
 void Context::setAsDefaultForAssertsOutOfTestCases() { g_cs = p; }
 
 void Context::setAssertHandler(detail::assert_handler ah) { p->ah = ah; }
 
+void Context::setCout(std::ostream* out) { p->cout = out; }
+
+static class DiscardOStream : public std::ostream
+{
+private:
+    class : public std::streambuf
+    {
+    private:
+        // allowing some buffering decreases the amount of calls to overflow
+        char buf[1024];
+
+    protected:
+        std::streamsize xsputn(const char_type*, std::streamsize count) override { return count; }
+
+        int_type overflow(int_type ch) override {
+            setp(std::begin(buf), std::end(buf));
+            return traits_type::not_eof(ch);
+        }
+    } discardBuf;
+
+public:
+    DiscardOStream()
+            : std::ostream(&discardBuf) {}
+} discardOut;
+
 // the main function that does all the filtering and test running
 int Context::run() {
     using namespace detail;
 
     // save the old context state in case such was setup - for using asserts out of a testing context
     auto old_cs = g_cs;
     // this is the current contest
     g_cs               = p;
     is_running_in_test = true;
 
     g_no_colors = p->no_colors;
     p->resetRunData();
 
-    // stdout by default
-    p->cout = &std::cout;
-    p->cerr = &std::cerr;
-
-    // or to a file if specified
     std::fstream fstr;
-    if(p->out.size()) {
-        fstr.open(p->out.c_str(), std::fstream::out);
-        p->cout = &fstr;
+    if(p->cout == nullptr) {
+        if(p->quiet) {
+            p->cout = &discardOut;
+        } else if(p->out.size()) {
+            // to a file if specified
+            fstr.open(p->out.c_str(), std::fstream::out);
+            p->cout = &fstr;
+        } else {
+#ifndef DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+            // stdout by default
+            p->cout = &std::cout;
+#else // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+            return EXIT_FAILURE;
+#endif // DOCTEST_CONFIG_NO_INCLUDE_IOSTREAM
+        }
     }
 
     FatalConditionHandler::allocateAltStackMem();
 
     auto cleanup_and_return = [&]() {
         FatalConditionHandler::freeAltStackMem();
 
@@ -5781,15 +6858,15 @@
     // TODO: check if there is nothing in reporters_currently_used
 
     // prepend all listeners
     for(auto& curr : getListeners())
         p->reporters_currently_used.insert(p->reporters_currently_used.begin(), curr.second(*g_cs));
 
 #ifdef DOCTEST_PLATFORM_WINDOWS
-    if(isDebuggerActive())
+    if(isDebuggerActive() && p->no_debug_output == false)
         p->reporters_currently_used.push_back(new DebugOutputWindowReporter(*g_cs));
 #endif // DOCTEST_PLATFORM_WINDOWS
 
     // handle version, help and no_run
     if(p->no_run || p->version || p->help || p->list_reporters) {
         DOCTEST_ITERATE_THROUGH_REPORTERS(report_query, QueryData());
 
@@ -5811,21 +6888,24 @@
             std::sort(testArray.begin(), testArray.end(), nameOrderComparator);
         } else if(p->order_by.compare("rand", true) == 0) {
             std::srand(p->rand_seed);
 
             // random_shuffle implementation
             const auto first = &testArray[0];
             for(size_t i = testArray.size() - 1; i > 0; --i) {
-                int idxToSwap = std::rand() % (i + 1); // NOLINT
+                int idxToSwap = std::rand() % (i + 1);
 
                 const auto temp = first[i];
 
                 first[i]         = first[idxToSwap];
                 first[idxToSwap] = temp;
             }
+        } else if(p->order_by.compare("none", true) == 0) {
+            // means no sorting - beneficial for death tests which call into the executable
+            // with a specific test case in mind - we don't want to slow down the startup times
         }
     }
 
     std::set<String> testSuitesPassingFilt;
 
     bool                             query_mode = p->count || p->list_test_cases || p->list_test_suites;
     std::vector<const TestCaseData*> queryResults;
@@ -5895,40 +6975,44 @@
             p->failure_flags = TestCaseFailureReason::None;
             p->seconds       = 0;
 
             // reset atomic counters
             p->numAssertsFailedCurrentTest_atomic = 0;
             p->numAssertsCurrentTest_atomic       = 0;
 
-            p->subcasesPassed.clear();
+            p->fullyTraversedSubcases.clear();
 
             DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_start, tc);
 
             p->timer.start();
-            
+
             bool run_test = true;
 
             do {
                 // reset some of the fields for subcases (except for the set of fully passed ones)
-                p->should_reenter          = false;
-                p->subcasesCurrentMaxLevel = 0;
-                p->subcasesStack.clear();
+                p->reachedLeaf = false;
+                // May not be empty if previous subcase exited via exception.
+                p->subcaseStack.clear();
+                p->currentSubcaseDepth = 0;
 
                 p->shouldLogCurrentException = true;
 
                 // reset stuff for logging with INFO()
                 p->stringifiedContexts.clear();
 
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
                 try {
 #endif // DOCTEST_CONFIG_NO_EXCEPTIONS
+// MSVC 2015 diagnoses fatalConditionHandler as unused (because reset() is a static method)
+DOCTEST_MSVC_SUPPRESS_WARNING_WITH_PUSH(4101) // unreferenced local variable
                     FatalConditionHandler fatalConditionHandler; // Handle signals
                     // execute the test
                     tc.m_test();
                     fatalConditionHandler.reset();
+DOCTEST_MSVC_SUPPRESS_WARNING_POP
 #ifndef DOCTEST_CONFIG_NO_EXCEPTIONS
                 } catch(const TestFailureException&) {
                     p->failure_flags |= TestCaseFailureReason::AssertFailure;
                 } catch(...) {
                     DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_exception,
                                                       {translateActiveException(), false});
                     p->failure_flags |= TestCaseFailureReason::Exception;
@@ -5937,18 +7021,18 @@
 
                 // exit this loop if enough assertions have failed - even if there are more subcases
                 if(p->abort_after > 0 &&
                    p->numAssertsFailed + p->numAssertsFailedCurrentTest_atomic >= p->abort_after) {
                     run_test = false;
                     p->failure_flags |= TestCaseFailureReason::TooManyFailedAsserts;
                 }
-                
-                if(p->should_reenter && run_test)
+
+                if(!p->nextSubcaseStack.empty() && run_test)
                     DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_reenter, tc);
-                if(!p->should_reenter)
+                if(p->nextSubcaseStack.empty())
                     run_test = false;
             } while(run_test);
 
             p->finalizeTestCaseData();
 
             DOCTEST_ITERATE_THROUGH_REPORTERS(test_case_end, *g_cs);
 
@@ -5966,25 +7050,18 @@
         QueryData qdata;
         qdata.run_stats = g_cs;
         qdata.data      = queryResults.data();
         qdata.num_data  = unsigned(queryResults.size());
         DOCTEST_ITERATE_THROUGH_REPORTERS(report_query, qdata);
     }
 
-    // see these issues on the reasoning for this:
-    // - https://github.com/onqtam/doctest/issues/143#issuecomment-414418903
-    // - https://github.com/onqtam/doctest/issues/126
-    auto DOCTEST_FIX_FOR_MACOS_LIBCPP_IOSFWD_STRING_LINK_ERRORS = []() DOCTEST_NOINLINE
-        { std::cout << std::string(); };
-    DOCTEST_FIX_FOR_MACOS_LIBCPP_IOSFWD_STRING_LINK_ERRORS();
-
     return cleanup_and_return();
 }
 
-IReporter::~IReporter() = default;
+DOCTEST_DEFINE_INTERFACE(IReporter)
 
 int IReporter::get_num_active_contexts() { return detail::g_infoContexts.size(); }
 const IContextScope* const* IReporter::get_active_contexts() {
     return get_num_active_contexts() ? &detail::g_infoContexts[0] : nullptr;
 }
 
 int IReporter::get_num_stringified_contexts() { return detail::g_cs->stringifiedContexts.size(); }
@@ -6011,9 +7088,21 @@
 DOCTEST_MSVC_SUPPRESS_WARNING_POP
 #endif // DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN
 
 DOCTEST_CLANG_SUPPRESS_WARNING_POP
 DOCTEST_MSVC_SUPPRESS_WARNING_POP
 DOCTEST_GCC_SUPPRESS_WARNING_POP
 
+DOCTEST_SUPPRESS_COMMON_WARNINGS_POP
+
 #endif // DOCTEST_LIBRARY_IMPLEMENTATION
 #endif // DOCTEST_CONFIG_IMPLEMENT
+
+#ifdef DOCTEST_UNDEF_WIN32_LEAN_AND_MEAN
+#undef WIN32_LEAN_AND_MEAN
+#undef DOCTEST_UNDEF_WIN32_LEAN_AND_MEAN
+#endif // DOCTEST_UNDEF_WIN32_LEAN_AND_MEAN
+
+#ifdef DOCTEST_UNDEF_NOMINMAX
+#undef NOMINMAX
+#undef DOCTEST_UNDEF_NOMINMAX
+#endif // DOCTEST_UNDEF_NOMINMAX
```

### Comparing `gemmi-0.6.5/third_party/linalg.h` & `gemmi-0.6.6/third_party/linalg.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/optionparser.h` & `gemmi-0.6.6/third_party/optionparser.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/sajson.h` & `gemmi-0.6.6/third_party/sajson.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/stb_sprintf.h` & `gemmi-0.6.6/third_party/stb_sprintf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/LICENSE` & `gemmi-0.6.6/third_party/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/adler32.c` & `gemmi-0.6.6/third_party/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/crc32.c` & `gemmi-0.6.6/third_party/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/gzguts.h` & `gemmi-0.6.6/third_party/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/gzlib.c` & `gemmi-0.6.6/third_party/zlib/gzlib.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/gzread.c` & `gemmi-0.6.6/third_party/zlib/gzread.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inffast.c` & `gemmi-0.6.6/third_party/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inffixed.h` & `gemmi-0.6.6/third_party/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inflate.c` & `gemmi-0.6.6/third_party/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inflate.h` & `gemmi-0.6.6/third_party/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inftrees.c` & `gemmi-0.6.6/third_party/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/inftrees.h` & `gemmi-0.6.6/third_party/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/zconf.h` & `gemmi-0.6.6/third_party/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/zlib.h` & `gemmi-0.6.6/third_party/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/zutil.c` & `gemmi-0.6.6/third_party/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/third_party/zlib/zutil.h` & `gemmi-0.6.6/third_party/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.5/PKG-INFO` & `gemmi-0.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gemmi
-Version: 0.6.5
+Version: 0.6.6
 Summary: library for structural biology
-Keywords: structural bioinformatics structural biology crystallography CIF mmCIF PDB CCP4 MTZ
+Keywords: structural bioinformatics,structural biology,crystallography,CIF,mmCIF,PDB,CCP4,MTZ
 Author-Email: Marcin Wojdyr <wojdyr@gmail.com>
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

