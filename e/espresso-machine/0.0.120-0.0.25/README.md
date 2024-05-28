# Comparing `tmp/espresso_machine-0.0.120.tar.gz` & `tmp/espresso_machine-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "espresso_machine-0.0.25.tar", last modified: Tue May 28 04:46:04 2024, max compression
```

## Comparing `espresso_machine-0.0.120.tar` & `espresso_machine-0.0.25.tar`

### file list

```diff
@@ -1,222 +1,47 @@
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/requirements.txt
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/FeO.ipynb
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/MaterialsProject.ipynb
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/MnPS3-yaml.ipynb
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/MnPS3.ipynb
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/NbSe2.ipynb
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/Notebook.ipynb
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/Si_parameter_test.ipynb
--rw-r--r--   0        0        0   403768 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/plot.ipynb
--rw-r--r--   0        0        0    47832 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/TODO/test.ipynb
--rw-r--r--   0        0        0    74668 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/1-Si-Band.ipynb
--rw-r--r--   0        0        0    49531 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/2-Si-DOS.ipynb
--rw-r--r--   0        0        0    67793 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/3-Si-PDOS.ipynb
--rw-r--r--   0        0        0   159721 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/4-Si-KDOS.ipynb
--rw-r--r--   0        0        0   170420 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/5-Al-PDOS.ipynb
--rw-r--r--   0        0        0   311430 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/6-Fe-Band.ipynb
--rw-r--r--   0        0        0    44370 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/7-Fe-DOS.ipynb
--rw-r--r--   0        0        0    85506 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/8-C-Band.ipynb
--rw-r--r--   0        0        0    78644 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/9-C-Phonon.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/config.json
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/Al.poscar
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/C.poscar
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/Fe.poscar
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/FeO.poscar
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/MnPS3.poscar
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/NbSe2.poscar
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/Si.poscar
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/Structures/UTe2.poscar
--rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/NC/Al.UPF
--rw-r--r--   0        0        0    90153 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/NC/C.UPF
--rw-r--r--   0        0        0   115566 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/NC/Nb.UPF
--rw-r--r--   0        0        0   115528 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/NC/Se.UPF
--rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/NC/Si.UPF
--rw-r--r--   0        0        0  1308566 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/Al.UPF
--rw-r--r--   0        0        0   606527 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/Co.UPF
--rw-r--r--   0        0        0  1431019 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/Fe.UPF
--rw-r--r--   0        0        0  1426269 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/Mn.UPF
--rw-r--r--   0        0        0   376736 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/O.UPF
--rw-r--r--   0        0        0  1322288 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/P.UPF
--rw-r--r--   0        0        0  1326847 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/S.UPF
--rw-r--r--   0        0        0  1315428 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/Tutorials/pseudos/US/Si.UPF
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/adiabatic.sh
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/check.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/compute.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/config.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/generate.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/kpoints.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/ph.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/ph_plot.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/plot_band.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/plot_sigma_energy.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/plots.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/project.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/reads.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/run.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/scaffold.py
--rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/structure.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/utils.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/writes.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/__init__.py
--rw-r--r--   0        0        0    26349 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/getpaths.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/brillouinzone/__init__.py
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
--rw-r--r--   0        0        0    21490 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/__init__.py
--rw-r--r--   0        0        0     9666 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/spg_db.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/spg_mapping.py
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/tools.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_inversion
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/path.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/path.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/points.txt
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/k_vector_parameters.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/path.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/path.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/path.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/points.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/path.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/points.txt
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_inversion
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/path.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/points.txt
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/path.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/points.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_inversion
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/path.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/points.txt
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/k_vector_parameters.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/path.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/points.txt
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/path.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/points.txt
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/k_vector_parameters.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/path.txt
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/points.txt
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/k_vector_parameters.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/path.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/k_vector_parameters.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/path.txt
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_inversion
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/path.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/path.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/path.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_inversion
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/path.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/path.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/points.txt
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/path.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/points.txt
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/k_vector_parameters.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/path.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/points.txt
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/k_vector_parameters.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/path.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/path.txt
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/points.txt
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/k_vector_parameters.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/path.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/points.txt
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/k_vector_parameters.txt
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/path.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/points.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_inversion
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/path.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/points.txt
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/path.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/points.txt
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_inversion
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_noinversion
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/path.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/points.txt
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/path.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/points.txt
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/LICENSE
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/pyproject.toml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 espresso_machine-0.0.120/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/espresso_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 04:46:02.000000 espresso_machine-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/espresso_machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/kpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/ph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/ph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plot_band.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plot_sigma_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/espresso_machine/seekpath/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26349 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/getpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/writes.py
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/compute.py` & `espresso_machine-0.0.25/src/espresso_machine/compute.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/config.py` & `espresso_machine-0.0.25/src/espresso_machine/config.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/generate.py` & `espresso_machine-0.0.25/src/espresso_machine/generate.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/kpoints.py` & `espresso_machine-0.0.25/src/espresso_machine/kpoints.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/ph.py` & `espresso_machine-0.0.25/src/espresso_machine/ph.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/ph_plot.py` & `espresso_machine-0.0.25/src/espresso_machine/ph_plot.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/plot_band.py` & `espresso_machine-0.0.25/src/espresso_machine/plot_band.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/plot_sigma_energy.py` & `espresso_machine-0.0.25/src/espresso_machine/plot_sigma_energy.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/plots.py` & `espresso_machine-0.0.25/src/espresso_machine/plots.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/project.py` & `espresso_machine-0.0.25/src/espresso_machine/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from . import utils
 from . import reads
 from . import generate
 from . import compute
 from . import kpoints
 from . import plots
 from . import structure
+import numpy as np 
 
 class project:
     def __init__(self,project_id,config=False):
         self.project_id = project_id
         self.config = utils.configure(config)
         self.atom = False
         self.lattice = False
@@ -54,16 +55,19 @@
         self.file_path = f"./Projects/{self.project_id}/{self.job_id}/{self.calculation}.in"
 
     def hubbard(self,atom,orbital,value,interaction='U',projection="atomic"):
         self.config['pw']['hubbard']['projection']=projection
         self.config['pw']['hubbard']['terms'].append({"interaction":interaction,'atom':atom,'orbital':orbital,'value':value})
     
 
-    def set_pseudo(self,pseudo_type):
-        self.config['pw']['control']['pseudo_dir']='./pseudos/'+pseudo_type.upper()+'/'
+    def set_pseudo(self,pseudo_type=False,path=False):
+        if path is not False:
+            self.config['pw']['control']['pseudo_dir']=f'{path}'
+        elif pseudo_type is not False:
+            self.config['pw']['control']['pseudo_dir']='./pseudos/'+pseudo_type.upper()+'/'
     
     def make_afm(self,magnetic_atom,angle1=False,angle2=False):
         afm_models = utils.afm_maker(self,magnetic_atom,angle1=angle1,angle2=angle2)
         return afm_models
     def make_fm(self,magnetic_atom,angle1=False,angle2=False):
         fm = utils.fm_maker(self,magnetic_atom,angle1=angle1,angle2=angle2)
         return fm
@@ -82,25 +86,38 @@
         self.config['pw']['system']['occupations'] = occupation
     def ecutwfc(self,number):
         self.config['pw']['system']['ecutwfc'] = number
     def ecutrho(self,number):
         self.config['pw']['system']['ecutrho'] = number
     def conv_thr(self,number):
         self.config['pw']['electrons']['conv_thr']=number
-    def make_layer(self,layer_type):
+    def make_layer(self,layer_type='mono',direction='z'):
         if layer_type=='mono':
-            self.config['pw']['atomic_positions'] = utils.make_monolayer(self.config['pw']['atomic_positions'])
+            self.config['pw']['atomic_positions'] = utils.make_monolayer(self.config['pw']['atomic_positions'],direction)
     def k_points(self,number):
         if type(number) == int :
             self.config['pw']['k_points']=f'{number} {number} {number} 0 0 0'
         elif len(number) == 3:
             self.config['pw']['k_points']=f'{number[0]} {number[1]} {number[2]} 0 0 0'
         else:
             raise Exception("K points can be either a number or an array with 3 enteries")
 
+
+    def shift_atoms(self,vector):
+        atoms = np.array(self.config['pw']['atomic_positions']).T[1:].T.astype(float)
+        shifted = utils.shift_frac(atoms=atoms,vector=vector)
+        for i,atom in enumerate(shifted):
+            for j in range(3):
+                self.config['pw']['atomic_positions'][i][1+j]=atom[j].astype(str)
+
+
+
+        self.config['pw']['atomic_positions']
+
+
     def plot(self,calculation,save=False,xlim=False,ylim=False):
         plots.plot(self,calculation,save,xlim,ylim)
 
     def nbnd(self,number):
         self.config['pw']['system']['nbnd']=number
     
     def get_nbnd(self):
@@ -111,22 +128,26 @@
     def smearing(self,value):
         self.config['pw']['system']['smearing'] = value
     def degauss(self,value):
         self.config['pw']['system']['degauss'] = value
     def nosym(self,value):
         self.config['pw']['system']['nosym'] = value
     def get_primitive(self,file='vasp-ase'):
-        lattice,atoms,kpoints = structure.primitive(self.poscar,file)
+        lattice,atoms,k_points = structure.primitive(self.poscar,file)
         self.config['pw']['atomic_positions'] = atoms
         self.config['pw']['cell_parameters']=lattice
         
-    def get_points(self,file='vasp-ase'):
-        lattice,atoms,kpoints = structure.primitive(self.poscar,file)
-        self.points=kpoints
-        return kpoints
+    def get_points(self,file_path=False,file_format=False):
+        if file_format==False:
+            file_format='qeinp-qetools'
+        if file_path==False:
+            file_path=f'./Projects/{self.project_id}/{self.job_id}/scf.in'
+        k_points = structure.get_k(file_path,file_format)
+        self.points=k_points
+        return k_points
     def get_structure(self,format,name=False,path=False,project_id=False,job_id=False,config=False):
         # self.poscar=f'./Structures/{self.project_id}.poscar'
         reads.read_structure(self,format,name=name,path=path)
 
     def calculate(self,calculation):
         self.set_calculation(calculation_type=calculation) #set calculation
         generate.input(self) #create input
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/reads.py` & `espresso_machine-0.0.25/src/espresso_machine/reads.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         config['cell_parameters'], config['atomic_positions'] = cell,atom
     except:
         try:
             config['atomic_positions'] = atom
         except:
             return cell,atom
     config['atomic_species']=utils.default_pseudo(atom)
+    ntyp = len(config['atomic_species'])
+    config['system']['ntyp']=ntyp
 
 
     try:
         if self.magnetic_order=='afm':
             #Check magnetic atoms order 
             for k,i in enumerate(config['atomic_species']):
                 for j in i['atom']:
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/run.py` & `espresso_machine-0.0.25/src/espresso_machine/run.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/scaffold.py` & `espresso_machine-0.0.25/src/espresso_machine/scaffold.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/structure.py` & `espresso_machine-0.0.25/src/espresso_machine/structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -294,15 +294,16 @@
             fileformat,
             flask_request,
             call_source,
             reason="codeexception",
             extra={"traceback": traceback.extract_stack(), "form_data": form_data,},
         )
         raise
-
+    # print(raw_code_dict)
+    # print(direct_vectors)
     return dict(
         jsondata=json.dumps(out_json_data),
         volume_ratio_prim=int(round(path_results["volume_original_wrt_prim"])),
         raw_code=raw_code,
         kpoints=kpoints,
         kpoints_rel=kpoints_rel,
         bravais_lattice=path_results["bravais_lattice"],
@@ -331,8 +332,13 @@
     structure = process_structure_core(filecontent=fileContent,fileformat=fileformat)
     lattice = (structure["primitive_vectors"].astype('str')).tolist()
     atoms = structure["atoms_scaled"]
     kpoints = structure['kpoints_rel']
     return (lattice,atoms,kpoints)
 
 
-
+def get_k(fileContent,fileformat):
+    with open(fileContent) as file:
+        fileContent = file.read()
+    structure = process_structure_core(filecontent=fileContent,fileformat=fileformat)
+    kpoints = structure['kpoints_rel']
+    return (kpoints)
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/utils.py` & `espresso_machine-0.0.25/src/espresso_machine/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,35 @@
 import untangle
 import copy
 import math
 import glob
 from . import compute
 from .config import default_config
 
-def make_monolayer(atoms):
+def shift_frac(atoms,vector):
+    return np.mod(atoms+vector,1)
+
+def make_monolayer(atoms,direction='z'):
+    direction = direction.lower()
+    if direction not in ['x','y','z']:
+        raise Exception("Direction should be x y or z")
     df = pd.DataFrame()
     atoms=np.array(atoms)
     df['Atoms'] = atoms.T[0]
     df['x'] = atoms.T[1].astype(float)
     df['y'] = atoms.T[2].astype(float)
     df['z'] = atoms.T[3].astype(float)
-    df = df.query('z<0.5')
+    df = df.query(f'{direction}<0.5')
     df_shifted = pd.DataFrame()
     df_shifted["Atoms"] = df['Atoms'].values
-    df_shifted["x"] = df['x'].values
-    df_shifted["y"] = df['y'].values
-    df_shifted["z"] = df['z'].values+0.25
+    for i in ['x','y','z']:
+        if direction==i:
+            df_shifted[i] = df[i].values+0.25
+        else:
+            df_shifted[i] = df[i].values
     return df_shifted.values
 
 
 def plot_sigma_energy(path):
     out_files = os.listdir(path)
     total_energy = []
     e_fermi = []
@@ -98,22 +106,25 @@
             if (angle2):
                 model.config['pw']['system'][f'angle2({j+1})']=angle2
                 self.angle2=angle2
             if angle1 or angle2:
                 model.config['pw']['system']['noncolin']='true'
             else:
                 model.config['pw']['system']['nspin']=2
+    ntyp = len(model.config['pw']['atomic_species'])
+    model.config['pw']['system']['ntyp']=ntyp
     return model #send it back
 
 
-def afm_maker(model,magnetic_atom,mag_start=[1,-1],angle1=False,angle2=False):
+def afm_maker(self,magnetic_atom,mag_start=[1,-1],angle1=False,angle2=False):
     #1 - Give initial model
     #2 - Define magnetic atom
     #3 - Return magnetic states
     #4 - FM and AFM
+    model = copy.deepcopy(self)
     model.magnetic_atom=magnetic_atom
     model.magnetic_order='afm'
     """
     FM is easier to do. Only starting magnetization parameter should be added for the relevent atom
     Number of AFM states can be changing depending on the number of magnetic atoms. 
     The number of magnetic atoms should be divided into two for spin up and down. 
     Total magnetism is going to be zero but the order of spins are going to be change.
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/writes.py` & `espresso_machine-0.0.25/src/espresso_machine/writes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 def write_atom_species(file,atomic_species):
     with open(file, "a") as file_object:
         file_object.write("ATOMIC_SPECIES \n")
         for atom in atomic_species:
             listed = list(atom.values())
             file_object.write(" ".join(listed)+'\n')
 
@@ -15,25 +16,24 @@
             except:
                 try:
                     file_object.write(" ".join(i.astype(str))+'\n')
                 except:
                     file_object.write(" ".join(str(i))+'\n')
 
 def write_cell_parameters(file, cell):
+    try:
+        cell = np.array(cell,float)
+    except:
+        print('Something is wrong with the cell parameters. The error got caught on input file writing step.')
     with open(file, "a") as file_object:
         file_object.write("CELL_PARAMETERS (angstrom) \n")
         for i in cell:
-            try:
-                file_object.write(" ".join(i)+'\n')
-            except:
-                try:
-                    file_object.write(" ".join(i.astype(str))+'\n')
-                except:
-                    file_object.write(" ".join(str(i))+'\n')
-            # print(i.astype(str))
+            for k,j in enumerate(i):
+                file_object.write(f"{np.around(j,8):<.10f}  ")
+            file_object.write("\n")
 
 
 def write_k_points(file, k):
     with open(file, "a") as file_object:
         file_object.write("K_POINTS automatic \n")
         file_object.write(k+'\n')
```

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/__init__.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/getpaths.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/getpaths.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/util.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/util.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/__init__.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/spg_db.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_db.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/spg_mapping.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_mapping.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/src/espresso_machine/seekpath/hpkot/tools.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/tools.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.120/LICENSE` & `espresso_machine-0.0.25/LICENSE`

 * *Files identical despite different names*

