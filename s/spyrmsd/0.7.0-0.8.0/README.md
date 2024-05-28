# Comparing `tmp/spyrmsd-0.7.0.tar.gz` & `tmp/spyrmsd-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyrmsd-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spyrmsd-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spyrmsd-0.7.0.tar` & `spyrmsd-0.8.0.tar`

### file list

```diff
@@ -1,221 +1,220 @@
--rw-r--r--   0        0        0      258 2024-04-05 21:55:07.867047 spyrmsd-0.7.0/.codecov.yml
--rw-r--r--   0        0        0      315 2024-04-05 21:55:07.867047 spyrmsd-0.7.0/.coveragerc
--rw-r--r--   0        0        0     2245 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      604 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      547 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/empty-issue.md
--rw-r--r--   0        0        0      142 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      787 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0      826 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      464 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      636 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     2095 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      948 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.gitignore
--rw-r--r--   0        0        0      792 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      359 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0     4115 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      820 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CITATION.cff
--rw-r--r--   0        0        0     3562 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1073 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/LICENSE
--rw-r--r--   0        0        0       93 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/MANIFEST.in
--rw-r--r--   0        0        0     7346 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/README.md
--rw-r--r--   0        0        0      126 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/credits.sh
--rw-r--r--   0        0        0      843 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/README.md
--rw-r--r--   0        0        0      518 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-all.yaml
--rw-r--r--   0        0        0      243 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-docs.yaml
--rw-r--r--   0        0        0      275 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-gt.yaml
--rw-r--r--   0        0        0      276 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-nx.yaml
--rw-r--r--   0        0        0      274 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-rx.yaml
--rw-r--r--   0        0        0      311 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-all.yaml
--rw-r--r--   0        0        0      281 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-gt.yaml
--rw-r--r--   0        0        0      282 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-nx.yaml
--rw-r--r--   0        0        0      280 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-rx.yaml
--rw-r--r--   0        0        0      133 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd.yaml
--rw-r--r--   0        0        0      636 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/Makefile
--rw-r--r--   0        0        0      997 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/README.md
--rw-r--r--   0        0        0      799 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/make.bat
--rw-r--r--   0        0        0       77 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api.rst
--rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.constants.rst
--rw-r--r--   0        0        0      121 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.due.rst
--rw-r--r--   0        0        0      142 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.exceptions.rst
--rw-r--r--   0        0        0      127 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graph.rst
--rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.gt.rst
--rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.nx.rst
--rw-r--r--   0        0        0      228 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.rst
--rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.hungarian.rst
--rw-r--r--   0        0        0      118 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.io.rst
--rw-r--r--   0        0        0      136 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.molecule.rst
--rw-r--r--   0        0        0      157 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.obabel.rst
--rw-r--r--   0        0        0      154 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.rdkit.rst
--rw-r--r--   0        0        0      245 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.rst
--rw-r--r--   0        0        0      121 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.qcp.rst
--rw-r--r--   0        0        0      124 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.rmsd.rst
--rw-r--r--   0        0        0      437 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.rst
--rw-r--r--   0        0        0      127 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.utils.rst
--rw-r--r--   0        0        0     5319 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/conf.py
--rw-r--r--   0        0        0      307 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/index.rst
--rw-r--r--   0        0        0     1502 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/installation.rst
--rw-r--r--   0        0        0    31852 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_dock.sdf
--rw-r--r--   0        0        0     4286 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_ligand.sdf
--rw-r--r--   0        0        0     9093 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/tutorial.ipynb
--rw-r--r--   0        0        0     4568 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/tutorial.rst
--rw-r--r--   0        0        0      458 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      521 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/setup.cfg
--rw-r--r--   0        0        0     1002 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/setup.py
--rw-r--r--   0        0        0      631 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/__main__.py
--rw-r--r--   0        0        0     4173 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/constants.py
--rw-r--r--   0        0        0     2019 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/due.py
--rw-r--r--   0        0        0      107 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/exceptions.py
--rw-r--r--   0        0        0     6984 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graph.py
--rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/__init__.py
--rw-r--r--   0        0        0      324 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/_common.py
--rw-r--r--   0        0        0     4802 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/gt.py
--rw-r--r--   0        0        0     3699 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/nx.py
--rw-r--r--   0        0        0     3588 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/rx.py
--rw-r--r--   0        0        0     2878 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/hungarian.py
--rw-r--r--   0        0        0     1649 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/io.py
--rw-r--r--   0        0        0     7074 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/molecule.py
--rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/__init__.py
--rw-r--r--   0        0        0     3160 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/obabel.py
--rw-r--r--   0        0        0     4852 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/rdkit.py
--rw-r--r--   0        0        0     7125 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/qcp.py
--rw-r--r--   0        0        0    10000 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/rmsd.py
--rw-r--r--   0        0        0     3418 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     2030 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0      510 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/README.md
--rw-r--r--   0        0        0     6610 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/docking/1a28/1a28_dock.sdf
--rw-r--r--   0        0        0     3431 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/docking/1a28/1a28_ligand.sdf
--rw-r--r--   0        0        0       29 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a28/obrms-min.dat
--rw-r--r--   0        0        0       25 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a28/obrms.dat
--rw-r--r--   0        0        0    31852 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_dock.sdf
--rw-r--r--   0        0        0     4286 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_ligand.sdf
--rw-r--r--   0        0        0       83 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/obrms-min.dat
--rw-r--r--   0        0        0       76 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/obrms.dat
--rw-r--r--   0        0        0    34320 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_dock.sdf
--rw-r--r--   0        0        0     4025 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_ligand.sdf
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/obrms-min.dat
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/obrms.dat
--rw-r--r--   0        0        0    22750 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/1a69_dock.sdf
--rw-r--r--   0        0        0     2973 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/1a69_ligand.sdf
--rw-r--r--   0        0        0       86 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/obrms.dat
--rw-r--r--   0        0        0    67930 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/1a94_dock.sdf
--rw-r--r--   0        0        0     7748 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/1a94_ligand.sdf
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/obrms.dat
--rw-r--r--   0        0        0     7776 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/1a99_dock.sdf
--rw-r--r--   0        0        0     1347 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/1a99_ligand.sdf
--rw-r--r--   0        0        0       69 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/obrms-min.dat
--rw-r--r--   0        0        0       64 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/obrms.dat
--rw-r--r--   0        0        0    49070 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_dock.sdf
--rw-r--r--   0        0        0     5591 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_ligand.sdf
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/obrms.dat
--rw-r--r--   0        0        0    11880 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_dock.sdf
--rw-r--r--   0        0        0     1833 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_ligand.sdf
--rw-r--r--   0        0        0      120 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/obrms.dat
--rw-r--r--   0        0        0    43730 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_dock.sdf
--rw-r--r--   0        0        0     5521 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_ligand.sdf
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/obrms-min.dat
--rw-r--r--   0        0        0       77 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/obrms.dat
--rw-r--r--   0        0        0    11375 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/1add_dock.sdf
--rw-r--r--   0        0        0     2955 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/1add_ligand.sdf
--rw-r--r--   0        0        0       42 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/obrms-min.dat
--rw-r--r--   0        0        0       41 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/obrms.dat
--rw-r--r--   0        0        0    21290 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/1adl_dock.sdf
--rw-r--r--   0        0        0     3162 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/1adl_ligand.sdf
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/obrms-min.dat
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/obrms.dat
--rw-r--r--   0        0        0    12400 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/1ado_dock.sdf
--rw-r--r--   0        0        0     1829 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/1ado_ligand.sdf
--rw-r--r--   0        0        0       85 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/obrms-min.dat
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/obrms.dat
--rw-r--r--   0        0        0    36100 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/1afk_dock.sdf
--rw-r--r--   0        0        0     4340 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/1afk_ligand.sdf
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/obrms-min.dat
--rw-r--r--   0        0        0       79 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/obrms.dat
--rw-r--r--   0        0        0    36100 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/1afl_dock.sdf
--rw-r--r--   0        0        0     4346 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/1afl_ligand.sdf
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/obrms.dat
--rw-r--r--   0        0        0    14360 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_dock.sdf
--rw-r--r--   0        0        0     2053 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_ligand.sdf
--rw-r--r--   0        0        0       89 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/obrms-min.dat
--rw-r--r--   0        0        0       79 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/obrms.dat
--rw-r--r--   0        0        0    13810 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_dock.sdf
--rw-r--r--   0        0        0     2191 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_ligand.sdf
--rw-r--r--   0        0        0       86 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/obrms-min.dat
--rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/obrms.dat
--rw-r--r--   0        0        0     8130 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_dock.sdf
--rw-r--r--   0        0        0     1441 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_ligand.sdf
--rw-r--r--   0        0        0      120 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/obrms-min.dat
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/obrms.dat
--rw-r--r--   0        0        0    28280 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/1aid_dock.sdf
--rw-r--r--   0        0        0     4086 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/1aid_ligand.sdf
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/obrms-min.dat
--rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/obrms.dat
--rw-r--r--   0        0        0    20210 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_dock.sdf
--rw-r--r--   0        0        0     3017 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_ligand.sdf
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/obrms-min.dat
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/obrms.dat
--rw-r--r--   0        0        0    13810 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_dock.sdf
--rw-r--r--   0        0        0     2189 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_ligand.sdf
--rw-r--r--   0        0        0       89 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/obrms-min.dat
--rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/obrms.dat
--rw-r--r--   0        0        0    14360 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_dock.sdf
--rw-r--r--   0        0        0     2078 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_ligand.sdf
--rw-r--r--   0        0        0       90 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/obrms-min.dat
--rw-r--r--   0        0        0       80 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/obrms.dat
--rw-r--r--   0        0        0     9910 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_dock.sdf
--rw-r--r--   0        0        0     1709 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_ligand.sdf
--rw-r--r--   0        0        0       85 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/obrms-min.dat
--rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/obrms.dat
--rw-r--r--   0        0        0    12015 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_dock.sdf
--rw-r--r--   0        0        0     5461 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_ligand.sdf
--rw-r--r--   0        0        0       25 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/obrms-min.dat
--rw-r--r--   0        0        0       25 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/obrms.dat
--rw-r--r--   0        0        0    39156 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_dock.sdf
--rw-r--r--   0        0        0     5343 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_ligand.sdf
--rw-r--r--   0        0        0       82 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/obrms-min.dat
--rw-r--r--   0        0        0       78 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/obrms.dat
--rw-r--r--   0        0        0     2112 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb
--rw-r--r--   0        0        0      568 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb.gz
--rw-r--r--   0        0        0    23500 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.mol2
--rw-r--r--   0        0        0    24394 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.pdb
--rw-r--r--   0        0        0    20730 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf
--rw-r--r--   0        0        0     3283 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf.gz
--rwxr-xr-x   0        0        0     4963 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_ligand.mol2
--rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_1.sdf
--rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_2.sdf
--rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_3.sdf
--rw-r--r--   0        0        0     1296 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.mol2
--rw-r--r--   0        0        0      310 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.mol2.gz
--rw-r--r--   0        0        0     1188 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.sdf
--rw-r--r--   0        0        0      230 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.sdf.gz
--rw-r--r--   0        0        0      599 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.xyz
--rw-r--r--   0        0        0     3601 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/dialanine.sdf
--rw-r--r--   0        0        0      894 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/ethanol.sdf
--rw-r--r--   0        0        0      444 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/ethanol.xyz
--rw-r--r--   0        0        0     1096 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/pyridine.sdf
--rw-r--r--   0        0        0      550 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/pyridine.xyz
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp0.pdb
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp1.pdb
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp2.pdb
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp3.pdb
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp4.pdb
--rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp5.pdb
--rw-r--r--   0        0        0     1893 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/molecules.py
--rw-r--r--   0        0        0     1426 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_benchmarks.py
--rw-r--r--   0        0        0     5713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_graph.py
--rw-r--r--   0        0        0     1314 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_hungarian.py
--rw-r--r--   0        0        0      596 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_import.py
--rw-r--r--   0        0        0     4112 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_io.py
--rw-r--r--   0        0        0     3508 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_large.py
--rw-r--r--   0        0        0     7555 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_molecule.py
--rw-r--r--   0        0        0     2403 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_qcp.py
--rw-r--r--   0        0        0    26471 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_rmsd.py
--rw-r--r--   0        0        0     1423 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_utils.py
--rw-r--r--   0        0        0     7776 1970-01-01 00:00:00.000000 spyrmsd-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.codecov.yml
+-rw-r--r--   0        0        0      315 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.coveragerc
+-rw-r--r--   0        0        0     2245 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      604 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      547 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/ISSUE_TEMPLATE/empty-issue.md
+-rw-r--r--   0        0        0      142 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      787 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/workflows/flake8.yml
+-rw-r--r--   0        0        0      826 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      464 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      636 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     2166 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      948 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.gitignore
+-rw-r--r--   0        0        0      792 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      359 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4830 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      820 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/CITATION.cff
+-rw-r--r--   0        0        0     3562 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1073 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/LICENSE
+-rw-r--r--   0        0        0       93 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/MANIFEST.in
+-rw-r--r--   0        0        0     7190 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/README.md
+-rw-r--r--   0        0        0      126 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/credits.sh
+-rw-r--r--   0        0        0      843 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/README.md
+-rw-r--r--   0        0        0      532 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-all.yaml
+-rw-r--r--   0        0        0      257 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-docs.yaml
+-rw-r--r--   0        0        0      313 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-obabel-all.yaml
+-rw-r--r--   0        0        0      298 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-obabel-nogt.yaml
+-rw-r--r--   0        0        0      274 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-obabel-rx.yaml
+-rw-r--r--   0        0        0      319 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-rdkit-all.yaml
+-rw-r--r--   0        0        0      304 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-rdkit-nogt.yaml
+-rw-r--r--   0        0        0      280 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-test-rdkit-rx.yaml
+-rw-r--r--   0        0        0      147 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/devtools/conda-envs/spyrmsd.yaml
+-rw-r--r--   0        0        0      636 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0      997 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/README.md
+-rw-r--r--   0        0        0      799 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0       77 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api.rst
+-rw-r--r--   0        0        0      139 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.constants.rst
+-rw-r--r--   0        0        0      121 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.due.rst
+-rw-r--r--   0        0        0      142 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.exceptions.rst
+-rw-r--r--   0        0        0      127 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.graph.rst
+-rw-r--r--   0        0        0      139 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.graphs.gt.rst
+-rw-r--r--   0        0        0      139 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.graphs.nx.rst
+-rw-r--r--   0        0        0      228 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.graphs.rst
+-rw-r--r--   0        0        0      139 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.hungarian.rst
+-rw-r--r--   0        0        0      118 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.io.rst
+-rw-r--r--   0        0        0      136 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.molecule.rst
+-rw-r--r--   0        0        0      157 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.optional.obabel.rst
+-rw-r--r--   0        0        0      154 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.optional.rdkit.rst
+-rw-r--r--   0        0        0      245 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.optional.rst
+-rw-r--r--   0        0        0      121 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.qcp.rst
+-rw-r--r--   0        0        0      124 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.rmsd.rst
+-rw-r--r--   0        0        0      437 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.rst
+-rw-r--r--   0        0        0      127 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/api/spyrmsd.utils.rst
+-rw-r--r--   0        0        0     5319 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/conf.py
+-rw-r--r--   0        0        0      307 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1575 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/installation.rst
+-rw-r--r--   0        0        0    31852 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/tutorials/molecules/1a4k_dock.sdf
+-rw-r--r--   0        0        0     4286 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/tutorials/molecules/1a4k_ligand.sdf
+-rw-r--r--   0        0        0     9093 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/tutorials/tutorial.ipynb
+-rw-r--r--   0        0        0     4568 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/docs/source/tutorials/tutorial.rst
+-rw-r--r--   0        0        0      456 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      521 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/setup.cfg
+-rw-r--r--   0        0        0     1030 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/setup.py
+-rw-r--r--   0        0        0      631 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/spyrmsd/__init__.py
+-rw-r--r--   0        0        0     2458 2024-05-28 21:44:32.393201 spyrmsd-0.8.0/spyrmsd/__main__.py
+-rw-r--r--   0        0        0     4173 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/constants.py
+-rw-r--r--   0        0        0     2019 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/due.py
+-rw-r--r--   0        0        0      107 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/exceptions.py
+-rw-r--r--   0        0        0     7158 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graph.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graphs/__init__.py
+-rw-r--r--   0        0        0      324 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graphs/_common.py
+-rw-r--r--   0        0        0     4802 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graphs/gt.py
+-rw-r--r--   0        0        0     3699 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graphs/nx.py
+-rw-r--r--   0        0        0     3588 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/graphs/rx.py
+-rw-r--r--   0        0        0     2878 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/hungarian.py
+-rw-r--r--   0        0        0     1649 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/io.py
+-rw-r--r--   0        0        0     7074 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/molecule.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/optional/__init__.py
+-rw-r--r--   0        0        0     3160 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/optional/obabel.py
+-rw-r--r--   0        0        0     4852 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/optional/rdkit.py
+-rw-r--r--   0        0        0     7125 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/qcp.py
+-rw-r--r--   0        0        0    10000 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/rmsd.py
+-rw-r--r--   0        0        0     3418 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/spyrmsd/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     4322 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      510 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/README.md
+-rw-r--r--   0        0        0     6610 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a28/1a28_dock.sdf
+-rw-r--r--   0        0        0     3431 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a28/1a28_ligand.sdf
+-rw-r--r--   0        0        0       29 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a28/obrms-min.dat
+-rw-r--r--   0        0        0       25 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a28/obrms.dat
+-rw-r--r--   0        0        0    31852 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4k/1a4k_dock.sdf
+-rw-r--r--   0        0        0     4286 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4k/1a4k_ligand.sdf
+-rw-r--r--   0        0        0       83 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4k/obrms-min.dat
+-rw-r--r--   0        0        0       76 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4k/obrms.dat
+-rw-r--r--   0        0        0    34320 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4r/1a4r_dock.sdf
+-rw-r--r--   0        0        0     4025 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4r/1a4r_ligand.sdf
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4r/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a4r/obrms.dat
+-rw-r--r--   0        0        0    22750 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a69/1a69_dock.sdf
+-rw-r--r--   0        0        0     2973 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a69/1a69_ligand.sdf
+-rw-r--r--   0        0        0       86 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a69/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a69/obrms.dat
+-rw-r--r--   0        0        0    67930 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a94/1a94_dock.sdf
+-rw-r--r--   0        0        0     7748 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a94/1a94_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a94/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a94/obrms.dat
+-rw-r--r--   0        0        0     7776 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a99/1a99_dock.sdf
+-rw-r--r--   0        0        0     1347 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a99/1a99_ligand.sdf
+-rw-r--r--   0        0        0       69 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a99/obrms-min.dat
+-rw-r--r--   0        0        0       64 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a99/obrms.dat
+-rw-r--r--   0        0        0    49070 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9m/1a9m_dock.sdf
+-rw-r--r--   0        0        0     5591 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9m/1a9m_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9m/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9m/obrms.dat
+-rw-r--r--   0        0        0    11880 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9q/1a9q_dock.sdf
+-rw-r--r--   0        0        0     1833 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9q/1a9q_ligand.sdf
+-rw-r--r--   0        0        0      120 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9q/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1a9q/obrms.dat
+-rw-r--r--   0        0        0    43730 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1aaq/1aaq_dock.sdf
+-rw-r--r--   0        0        0     5521 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1aaq/1aaq_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1aaq/obrms-min.dat
+-rw-r--r--   0        0        0       77 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1aaq/obrms.dat
+-rw-r--r--   0        0        0    11375 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1add/1add_dock.sdf
+-rw-r--r--   0        0        0     2955 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1add/1add_ligand.sdf
+-rw-r--r--   0        0        0       42 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1add/obrms-min.dat
+-rw-r--r--   0        0        0       41 2024-05-28 21:44:32.397201 spyrmsd-0.8.0/tests/data/docking/1add/obrms.dat
+-rw-r--r--   0        0        0    21290 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1adl/1adl_dock.sdf
+-rw-r--r--   0        0        0     3162 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1adl/1adl_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1adl/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1adl/obrms.dat
+-rw-r--r--   0        0        0    12400 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ado/1ado_dock.sdf
+-rw-r--r--   0        0        0     1829 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ado/1ado_ligand.sdf
+-rw-r--r--   0        0        0       85 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ado/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ado/obrms.dat
+-rw-r--r--   0        0        0    36100 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afk/1afk_dock.sdf
+-rw-r--r--   0        0        0     4340 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afk/1afk_ligand.sdf
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afk/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afk/obrms.dat
+-rw-r--r--   0        0        0    36100 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afl/1afl_dock.sdf
+-rw-r--r--   0        0        0     4346 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afl/1afl_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afl/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1afl/obrms.dat
+-rw-r--r--   0        0        0    14360 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai4/1ai4_dock.sdf
+-rw-r--r--   0        0        0     2053 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai4/1ai4_ligand.sdf
+-rw-r--r--   0        0        0       89 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai4/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai4/obrms.dat
+-rw-r--r--   0        0        0    13810 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai5/1ai5_dock.sdf
+-rw-r--r--   0        0        0     2191 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai5/1ai5_ligand.sdf
+-rw-r--r--   0        0        0       86 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai5/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai5/obrms.dat
+-rw-r--r--   0        0        0     8130 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai7/1ai7_dock.sdf
+-rw-r--r--   0        0        0     1441 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai7/1ai7_ligand.sdf
+-rw-r--r--   0        0        0      120 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai7/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ai7/obrms.dat
+-rw-r--r--   0        0        0    28280 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aid/1aid_dock.sdf
+-rw-r--r--   0        0        0     4086 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aid/1aid_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aid/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aid/obrms.dat
+-rw-r--r--   0        0        0    20210 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aj7/1aj7_dock.sdf
+-rw-r--r--   0        0        0     3017 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aj7/1aj7_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aj7/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1aj7/obrms.dat
+-rw-r--r--   0        0        0    13810 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajn/1ajn_dock.sdf
+-rw-r--r--   0        0        0     2189 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajn/1ajn_ligand.sdf
+-rw-r--r--   0        0        0       89 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajn/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajn/obrms.dat
+-rw-r--r--   0        0        0    14360 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajp/1ajp_dock.sdf
+-rw-r--r--   0        0        0     2078 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajp/1ajp_ligand.sdf
+-rw-r--r--   0        0        0       90 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajp/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajp/obrms.dat
+-rw-r--r--   0        0        0     9910 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajq/1ajq_dock.sdf
+-rw-r--r--   0        0        0     1709 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajq/1ajq_ligand.sdf
+-rw-r--r--   0        0        0       85 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajq/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajq/obrms.dat
+-rw-r--r--   0        0        0    12015 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajv/1ajv_dock.sdf
+-rw-r--r--   0        0        0     5461 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajv/1ajv_ligand.sdf
+-rw-r--r--   0        0        0       25 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajv/obrms-min.dat
+-rw-r--r--   0        0        0       25 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajv/obrms.dat
+-rw-r--r--   0        0        0    39156 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajx/1ajx_dock.sdf
+-rw-r--r--   0        0        0     5343 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajx/1ajx_ligand.sdf
+-rw-r--r--   0        0        0       82 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajx/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/docking/1ajx/obrms.dat
+-rw-r--r--   0        0        0     2112 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1a99_ligand.pdb
+-rw-r--r--   0        0        0      568 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1a99_ligand.pdb.gz
+-rw-r--r--   0        0        0    23500 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.mol2
+-rw-r--r--   0        0        0    24394 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.pdb
+-rw-r--r--   0        0        0    20730 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.sdf
+-rw-r--r--   0        0        0     3283 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.sdf.gz
+-rwxr-xr-x   0        0        0     4963 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/1cbr_ligand.mol2
+-rw-r--r--   0        0        0     4713 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/2viz_1.sdf
+-rw-r--r--   0        0        0     4713 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/2viz_2.sdf
+-rw-r--r--   0        0        0     4713 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/2viz_3.sdf
+-rw-r--r--   0        0        0     1296 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/benzene.mol2
+-rw-r--r--   0        0        0      310 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/benzene.mol2.gz
+-rw-r--r--   0        0        0     1188 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/benzene.sdf
+-rw-r--r--   0        0        0      230 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/benzene.sdf.gz
+-rw-r--r--   0        0        0      599 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/benzene.xyz
+-rw-r--r--   0        0        0     3601 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/dialanine.sdf
+-rw-r--r--   0        0        0      894 2024-05-28 21:44:32.401201 spyrmsd-0.8.0/tests/data/molecules/ethanol.sdf
+-rw-r--r--   0        0        0      444 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/ethanol.xyz
+-rw-r--r--   0        0        0     1096 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/pyridine.sdf
+-rw-r--r--   0        0        0      550 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/pyridine.xyz
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp0.pdb
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp1.pdb
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp2.pdb
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp3.pdb
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp4.pdb
+-rw-r--r--   0        0        0    22113 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/data/molecules/trp5.pdb
+-rw-r--r--   0        0        0     2876 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_backends.py
+-rw-r--r--   0        0        0     1453 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     6220 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_graph.py
+-rw-r--r--   0        0        0     1142 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_hungarian.py
+-rw-r--r--   0        0        0      596 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_import.py
+-rw-r--r--   0        0        0     4479 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_io.py
+-rw-r--r--   0        0        0     3595 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_large.py
+-rw-r--r--   0        0        0     5536 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_molecule.py
+-rw-r--r--   0        0        0     2210 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_qcp.py
+-rw-r--r--   0        0        0    27274 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_rmsd.py
+-rw-r--r--   0        0        0     1465 2024-05-28 21:44:32.405201 spyrmsd-0.8.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7618 1970-01-01 00:00:00.000000 spyrmsd-0.8.0/PKG-INFO
```

### Comparing `spyrmsd-0.7.0/.github/CONTRIBUTING.md` & `spyrmsd-0.8.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/.github/FUNDING.yml` & `spyrmsd-0.8.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/bug-report.md` & `spyrmsd-0.8.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/.github/workflows/flake8.yml` & `spyrmsd-0.8.0/.github/workflows/mypy.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: flake8
+name: mypy
 
 on:
   push:
     branches: [ master, develop ]
   pull_request:
     branches: [ master, develop ]
 
@@ -12,23 +12,26 @@
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v5
       with:
           python-version: ${{ matrix.python-version }}
     - name: Install Dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install setuptools
-        python -m pip install flake8
+        python -m pip install mypy
+    - name: Install Types
+      run: |
+        python -m pip install types-requests
     - name: Install  package
       run: |
         python setup.py develop --no-deps
-    - name: Lint with flake8
+    - name: Lint with mypy
       run: |
-        flake8 . --count --show-source --statistics
+        mypy
```

### Comparing `spyrmsd-0.7.0/.github/workflows/mypy.yml` & `spyrmsd-0.8.0/.github/workflows/pypi.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-name: mypy
+name: pypi
 
 on:
-  push:
-    branches: [ master, develop ]
-  pull_request:
-    branches: [ master, develop ]
+  release:
+    types: [created]
+    branches: [master]
 
 jobs:
-  build:
+  deploy:
 
     runs-on: ubuntu-latest
 
-    strategy:
-      matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
-
     steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+    - uses: actions/checkout@v4
+    - name: Set up Python
+      uses: actions/setup-python@v5
       with:
-          python-version: ${{ matrix.python-version }}
-    - name: Install Dependencies
+        python-version: '3.x'
+    - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install setuptools
-        python -m pip install mypy
-    - name: Install Types
-      run: |
-        python -m pip install types-requests
-    - name: Install  package
-      run: |
-        python setup.py develop --no-deps
-    - name: Lint with mypy
+        pip install setuptools wheel flit
+    - name: Build and publish
+      env:
+        FLIT_USERNAME: ${{ secrets.FLIT_USERNAME }}
+        FLIT_PASSWORD: ${{ secrets.FLIT_PASSWORD }}
       run: |
-        mypy
+        python -m pip install . --no-deps
+        flit build
+        flit publish
```

### Comparing `spyrmsd-0.7.0/.github/workflows/pytest.yml` & `spyrmsd-0.8.0/.github/workflows/pytest.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,27 @@
     name: Test ${{ matrix.os }}-${{ matrix.python-version }}-${{ matrix.chemlib }}-${{ matrix.graphlib }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macOS-latest, ubuntu-latest, windows-latest]
         python-version: ["3.9", "3.10", "3.11", "3.12"]
         chemlib: [obabel, rdkit]
-        graphlib: [nx, gt, rx, all]
+        graphlib: [nogt, all]
         exclude:
-        # graph-tools does not work on Windows
-        - {os: "windows-latest", graphlib: "gt"}
-        - {os: "windows-latest", graphlib: "all"}
-        - {graphlib: "all", chemlib: "obabel"}
+          # graph-tool does not work on Windows
+          - {os: "windows-latest", graphlib: "all"}
+          # Don't run without graph-tool on Ubuntu and macOS
+          - {os: "ubuntu-latest", graphlib: "nogt"}
+          - {os: "macOS-latest", graphlib: "nogt"}
         include:
-        - {os: "macOS-14", graphlib: "gt", chemlib: "obabel", python-version: "3.12"}
-        - {os: "macOS-14", graphlib: "nx", chemlib: "rdkit", python-version: "3.12"}
+          - {os: "macOS-14", graphlib: "all", chemlib: "obabel", python-version: "3.12"}
+          - {os: "macOS-14", graphlib: "all", chemlib: "rdkit", python-version: "3.12"}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Info
       shell: bash
       run: |
         uname -a
         df -h
         ulimit -a
@@ -65,12 +66,12 @@
         mamba list
 
     - name: Test
       run: |
         pytest -v --benchmark --cov=spyrmsd --cov-report=xml --color=yes tests/
 
     - name: CodeCov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: ./coverage.xml
         flags: unittests
         name: codecov-${{ matrix.os }}-py${{ matrix.python-version }}-${{ matrix.chemlib }}-${{ matrix.graphlib }}
```

### Comparing `spyrmsd-0.7.0/.gitignore` & `spyrmsd-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/.pre-commit-config.yaml` & `spyrmsd-0.8.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 exclude: |
             (?x)^(
                 docs/source/conf.py
             )$
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     - id: check-json
     - id: check-merge-conflict
     - id: check-yaml
     - id: check-toml
     - id: debug-statements
     - id: end-of-file-fixer
     - id: trailing-whitespace
 -   repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 24.4.0
     hooks:
     -   id: black
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
     -   id: isort
         args: ["--profile", "black"]
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.9.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests]
```

### Comparing `spyrmsd-0.7.0/CHANGELOG.md` & `spyrmsd-0.8.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,55 @@
 
 # `spyrmsd` CHANGELOG
 
 ------------------------------------------------------------------------------
 
+## Version 0.8.0
+
+Date:            28/05/2024
+Contributors:    @RMeli
+
+### Added
+
+* Warnings filter for tests of multiple backends [PR #118 | @RMeli]
+* Parametrized fixture to run tests with all available backends [PR #118 | @RMeli]
+
+### Improved
+
+* Test IDs [PR #117 | @RMeli]
+
+### Changed
+
+* the default backend for `pip` installations to `rustworkx` [PR#122 | @RMeli]
+* `pre-commit` versions [PR #120 | @RMeli]
+* Versions of several GitHub Actions [PR #120 | @RMeli]
+* Location of backend tests to standalone file [PR #118 | @RMeli]
+
+### Removed
+
+* Many CI configurations in favour of running tests for all available backends [PR #118 | @RMeli]
+* `tests/molecule.py` in favour of fixtures [PR #118 | @RMeli]
+
 ## Version 0.7.0
 
 Date:            05/04/2024
 Contributors:    @RMeli, @takluyver, @Jnelen
 
 ### Added
 
-* Support for `rustworkx` graph library [PR 111 | @RMeli]
+* Support for `rustworkx` graph library [PR #111 | @RMeli]
 * Functionality to manually select the backend from CLI [PR #108 | @RMeli]
 * Functionality to manually select the backend [PR  #107 | @Jnelen]
 * Python `3.12` to CI [PR  #102 | @RMeli]
 * macOS M1 (`macoOS-14`) to CI [PR  #102 | @RMeli]
 
 ### Changed
 
 * Molecular graphs cache to cache by backend [PR  #107 | @Jnelen]
-* Python build system to use flit_core directly [PR #103 | @takluyver]
+* Python build system to use `flit_core` directly [PR #103 | @takluyver]
 * Minimum version of Python to `3.9` (to reduce CI matrix) [PR  #102 | @RMeli]
 
 ### Fixed
 
 * Failing tests with `pytest=8.0.0` [PR #101 | @RMeli]
 
 ### Improved
```

### Comparing `spyrmsd-0.7.0/CITATION.cff` & `spyrmsd-0.8.0/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 - family-names: "Meli"
   given-names: "Rocco"
   orcid: "https://orcid.org/0000-0002-2845-3410"
 - family-names: "Nelen"
   given-names: "Jochem"
   orcid: "https://orcid.org/0000-0002-9970-4950"
 title: "spyrmsd"
-version: 0.7.0
+version: 0.8.0
 doi: 10.5281/zenodo.3631876
 date-released: 2021-06-21
 url: "https://github.com/RMeli/spyrmsd"
 preferred-citation:
   type: article
   authors:
   - family-names: "Meli"
```

### Comparing `spyrmsd-0.7.0/CODE_OF_CONDUCT.md` & `spyrmsd-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/LICENSE` & `spyrmsd-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/README.md` & `spyrmsd-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 
 ## Installation
 
 `spyrmsd` is available on [PyPI](https://pypi.org/project/spyrmsd/) and [conda-forge](https://github.com/conda-forge/spyrmsd-feedstock) and can be easily installed from source. See [Dependencies](###Dependencies) for a description of all the dependencies.
 
 > [!NOTE]
-> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install the other backends for higher performance.
+> `spyrmsd` will install [rustworkx] (multi-platform) when using `pip` or `conda`. You can install other backends manually.
 
 > [!WARNING]
 > If `spyrmsd` is used as a standalone tool, it is required to install either [RDKit](https://rdkit.org/) or [Open Babel](http://openbabel.org/). Neither is automatically installed with `pip` nor `conda`.
 
 ### PyPI
 
 ```bash
@@ -72,19 +72,19 @@
 The following packages are required to use `spyrmsd` as a module:
 
 * [numpy](https://numpy.org/)
 * [scipy](https://www.scipy.org/)
 
 One of the following graph libraries is required:
 * [graph-tool]
-* [NetworkX]
 * [rustworkx]
+* [NetworkX]
 
 > [!NOTE]
-> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [NetworkX], [rustworkx]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.* However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and the other graph library need to be installed manually.
+> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [rustworkx], [NetworkX]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.*
 
 #### Standalone Tool
 
 Additionally, one of the following packages is required to use `spyrmsd` as a standalone tool:
 
 * [Open Babel](http://openbabel.org/)
 * [RDKit](https://rdkit.org/)
@@ -174,18 +174,18 @@
 
 ## Development
 
 To ensure code quality and consistency the following tools are used during development:
 
 * [black](https://black.readthedocs.io/en/stable/)
 * [Flake 8](http://flake8.pycqa.org/en/latest/) (CI)
-* [isort]()
+* [isort](https://pycqa.github.io/isort/)
 * [mypy](http://mypy-lang.org/) (CI)
 
-Pre-commit `git` hooks can be installed with [pre-commit](https://pre-commit.com/).
+Pre-commit `git` hooks can be installed with [pre-commit].
 
 ## Copyright
 
 Copyright (c) 2019-2024, Rocco Meli.
 
 ## References
 
@@ -194,7 +194,8 @@
 ### Acknowledgements
 
 Project based on the [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version `1.1`.
 
 [rustworkx]: https://www.rustworkx.org
 [NetworkX]: https://networkx.github.io/
 [graph-tool]: https://graph-tool.skewed.de/
+[pre-commit]: https://pre-commit.com/
```

### Comparing `spyrmsd-0.7.0/devtools/README.md` & `spyrmsd-0.8.0/devtools/README.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-all.yaml` & `spyrmsd-0.8.0/devtools/conda-envs/spyrmsd-all.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,17 @@
   # Jupyter
   - jupyterlab
 
   # Maths
   - numpy
   - pandas
   - scipy
-  - networkx>=2
   - graph-tool
+  - rustworkx
+  - networkx>=2
   - scikit-learn
 
   # Chemistry
   - openbabel
   - rdkit
 
   # Plotting
```

### Comparing `spyrmsd-0.7.0/docs/Makefile` & `spyrmsd-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/README.md` & `spyrmsd-0.8.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/make.bat` & `spyrmsd-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/source/conf.py` & `spyrmsd-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/source/installation.rst` & `spyrmsd-0.8.0/docs/source/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -40,20 +40,20 @@
 ``spyrmsd`` can be used both as a module or as a standalone tool.
 
 Module
 ~~~~~~
 
 The following packages are required to use ``spyrmsd`` as a module:
 
-* graph-tool_ or NetworkX_
+* graph-tool_, rustworkx_, or NetworkX_
 * numpy_
 * scipy_
 
 .. note::
-   ``spyrmsd`` uses graph-tool_ by default but will  fall back  to NetworkX_ if the former is not installed (e.g. on Windows).
+   ``spyrmsd`` uses graph-tool_ by default but will fall back to either rustworkx_ or NetworkX_ if the former is not installed (e.g. on Windows).
 
 Standalone Tool
 ~~~~~~~~~~~~~~~
 
 Additionally, one of the following packages is required to use ``spyrmsd`` as a standalone tool:
 
 * `Open Babel`_
@@ -63,7 +63,8 @@
 .. _conda-forge: https://github.com/conda-forge/spyrmsd-feedstock
 .. _RDKit: https://rdkit.org/
 .. _Open Babel: http://openbabel.org/
 .. _graph-tool: https://graph-tool.skewed.de/
 .. _NetworkX: https://networkx.github.io/
 .. _numpy: https://numpy.org/
 .. _scipy: https://www.scipy.org/
+.. _rustworkx: https://www.rustworkx.org
```

### Comparing `spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_dock.sdf` & `spyrmsd-0.8.0/docs/source/tutorials/molecules/1a4k_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_ligand.sdf` & `spyrmsd-0.8.0/docs/source/tutorials/molecules/1a4k_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/source/tutorials/tutorial.ipynb` & `spyrmsd-0.8.0/docs/source/tutorials/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/docs/source/tutorials/tutorial.rst` & `spyrmsd-0.8.0/docs/source/tutorials/tutorial.rst`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/setup.cfg` & `spyrmsd-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/setup.py` & `spyrmsd-0.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,22 @@
     # Self-descriptive entries which should always be present
     name="spyrmsd",
     author="Rocco Meli",
     author_email="rocco.meli@cscs.ch",
     description=short_description[0],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.7.0-dev",
+    version="0.8.0",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     url="https://spyrmsd.readthedocs.io",
-    install_requires=["numpy", "scipy", "networkx>=2"],
+    install_requires=["numpy", "scipy", "rustworkx"],
     extras_require={
         "bib": ["duecredit"],
         "rdkit": ["rdkit"],
         "openbabel": ["openbabel"],
+        "networkx": ["networkx"],
     },
     platforms=["Linux", "Mac OS-X", "Unix", "Windows"],
     python_requires=">=3.9",
 )
```

### Comparing `spyrmsd-0.7.0/spyrmsd/__init__.py` & `spyrmsd-0.8.0/spyrmsd/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Make the backend related functions available from base spyrmsd
 # Add noqa to avoid flake8 error
 from .graph import _available_backends as available_backends  # noqa: F401
 from .graph import _get_backend as get_backend  # noqa: F401
 from .graph import _set_backend as set_backend  # noqa: F401
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 # This will print latest Zenodo version
 due.cite(
     Doi("10.5281/zenodo.3631876"),
     path="spyrmsd",
     description="spyrmsd",
 )
```

### Comparing `spyrmsd-0.7.0/spyrmsd/__main__.py` & `spyrmsd-0.8.0/spyrmsd/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         exit(-1)
 
     if args.graph_backend is not None:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             spyrmsd.set_backend(args.graph_backend)
 
-            if args.verbose:
-                print(f"Graph library: {spyrmsd.get_backend()}")
+    if args.verbose:
+        print(f"Graph library: {spyrmsd.get_backend()}")
 
     # Loop over molecules within fil
     RMSDlist = rmsdwrapper(
         ref,
         mols,
         symmetry=args.nosymm,  # args.nosymm store False
         center=args.center,
```

### Comparing `spyrmsd-0.7.0/spyrmsd/constants.py` & `spyrmsd-0.8.0/spyrmsd/constants.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/due.py` & `spyrmsd-0.8.0/spyrmsd/due.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/graph.py` & `spyrmsd-0.8.0/spyrmsd/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import importlib.util
 import warnings
 
 import numpy as np
 
 from spyrmsd import constants
 
-_supported_backends = ("graph_tool", "networkx", "rustworkx")
+# The first backend found from this list is set as default
+# TODO: Need to determine if graph_tool or rustworkx is better
+# NetworkX is slow, therefore it is the last resort
+_supported_backends = ("graph_tool", "rustworkx", "networkx")
 
 _available_backends = []
 _current_backend = None
 
 _backend_to_alias = {
     "graph_tool": ["graph_tool", "graphtool", "graph-tool", "graph tool", "gt"],
     "networkx": ["networkx", "nx"],
```

### Comparing `spyrmsd-0.7.0/spyrmsd/graphs/gt.py` & `spyrmsd-0.8.0/spyrmsd/graphs/gt.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/graphs/nx.py` & `spyrmsd-0.8.0/spyrmsd/graphs/nx.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/graphs/rx.py` & `spyrmsd-0.8.0/spyrmsd/graphs/rx.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/hungarian.py` & `spyrmsd-0.8.0/spyrmsd/hungarian.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/io.py` & `spyrmsd-0.8.0/spyrmsd/io.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/molecule.py` & `spyrmsd-0.8.0/spyrmsd/molecule.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/optional/obabel.py` & `spyrmsd-0.8.0/spyrmsd/optional/obabel.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/optional/rdkit.py` & `spyrmsd-0.8.0/spyrmsd/optional/rdkit.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/qcp.py` & `spyrmsd-0.8.0/spyrmsd/qcp.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/rmsd.py` & `spyrmsd-0.8.0/spyrmsd/rmsd.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/spyrmsd/utils.py` & `spyrmsd-0.8.0/spyrmsd/utils.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a28/1a28_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a28/1a28_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a28/1a28_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a28/1a28_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a4k/1a4k_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a4k/1a4k_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a4r/1a4r_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a4r/1a4r_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a69/1a69_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a69/1a69_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a69/1a69_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a69/1a69_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a94/1a94_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a94/1a94_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a94/1a94_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a94/1a94_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a99/1a99_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a99/1a99_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a99/1a99_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a99/1a99_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a9m/1a9m_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a9m/1a9m_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a9q/1a9q_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1a9q/1a9q_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aaq/1aaq_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aaq/1aaq_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1add/1add_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1add/1add_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1add/1add_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1add/1add_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1adl/1adl_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1adl/1adl_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1adl/1adl_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1adl/1adl_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ado/1ado_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ado/1ado_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ado/1ado_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ado/1ado_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1afk/1afk_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1afk/1afk_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1afk/1afk_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1afk/1afk_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1afl/1afl_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1afl/1afl_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1afl/1afl_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1afl/1afl_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai4/1ai4_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai4/1ai4_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai5/1ai5_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai5/1ai5_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai7/1ai7_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ai7/1ai7_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aid/1aid_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aid/1aid_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aid/1aid_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aid/1aid_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aj7/1aj7_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1aj7/1aj7_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajn/1ajn_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajn/1ajn_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajp/1ajp_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajp/1ajp_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajq/1ajq_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajq/1ajq_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajv/1ajv_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajv/1ajv_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_dock.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajx/1ajx_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_ligand.sdf` & `spyrmsd-0.8.0/tests/data/docking/1ajx/1ajx_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb` & `spyrmsd-0.8.0/tests/data/molecules/1a99_ligand.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb.gz` & `spyrmsd-0.8.0/tests/data/molecules/1a99_ligand.pdb.gz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.mol2` & `spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.pdb` & `spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf` & `spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf.gz` & `spyrmsd-0.8.0/tests/data/molecules/1cbr_docking.sdf.gz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/1cbr_ligand.mol2` & `spyrmsd-0.8.0/tests/data/molecules/1cbr_ligand.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/2viz_1.sdf` & `spyrmsd-0.8.0/tests/data/molecules/2viz_1.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/2viz_2.sdf` & `spyrmsd-0.8.0/tests/data/molecules/2viz_2.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/2viz_3.sdf` & `spyrmsd-0.8.0/tests/data/molecules/2viz_3.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/benzene.mol2` & `spyrmsd-0.8.0/tests/data/molecules/benzene.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/benzene.sdf` & `spyrmsd-0.8.0/tests/data/molecules/benzene.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/benzene.xyz` & `spyrmsd-0.8.0/tests/data/molecules/benzene.xyz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/dialanine.sdf` & `spyrmsd-0.8.0/tests/data/molecules/dialanine.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/ethanol.sdf` & `spyrmsd-0.8.0/tests/data/molecules/ethanol.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/pyridine.sdf` & `spyrmsd-0.8.0/tests/data/molecules/pyridine.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/pyridine.xyz` & `spyrmsd-0.8.0/tests/data/molecules/pyridine.xyz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp0.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp0.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp1.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp1.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp2.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp2.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp3.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp3.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp4.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp4.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/data/molecules/trp5.pdb` & `spyrmsd-0.8.0/tests/data/molecules/trp5.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/test_benchmarks.py` & `spyrmsd-0.8.0/tests/test_benchmarks.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     for mol in mols:
         mol.strip()
 
     return ref, mols, system
 
 
 @pytest.mark.benchmark
-@pytest.mark.parametrize("cache", [True, False])
+@pytest.mark.parametrize("cache", [True, False], ids=["cache", "no_cache"])
 def test_benchmark_symmrmsd(cache, molecules, benchmark):
     ref, mols, system = molecules
 
     coords = [mol.coordinates for mol in mols]
 
     RMSDs = benchmark(
         rmsd.symmrmsd,
```

### Comparing `spyrmsd-0.7.0/tests/test_graph.py` & `spyrmsd-0.8.0/tests/test_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import pytest
 
 import spyrmsd
-from spyrmsd import constants, graph, io, molecule
+from spyrmsd import constants, graph, io
 from spyrmsd.exceptions import NonIsomorphicGraphs
 from spyrmsd.graphs import _common as gc
-from tests import molecules
 
 
 def test_adjacency_matrix_from_atomic_coordinates_distance() -> None:
     # Lithium hydride (LiH)
     # H and Li have very different covalent radii
     atomicnums = np.array([1, 3])
 
@@ -24,69 +23,68 @@
 
     A = graph.adjacency_matrix_from_atomic_coordinates(atomicnums, coordinates)
     G = graph.graph_from_adjacency_matrix(A)
 
     assert graph.num_edges(G) == 1
 
 
-@pytest.mark.parametrize(
-    "mol, n_bonds",
-    [(molecules.benzene, 12), (molecules.ethanol, 8), (molecules.dialanine, 22)],
-)
-def test_adjacency_matrix_from_atomic_coordinates(
-    mol: molecule.Molecule, n_bonds: int
-) -> None:
-    A = graph.adjacency_matrix_from_atomic_coordinates(mol.atomicnums, mol.coordinates)
+def test_adjacency_matrix_from_atomic_coordinates(mol) -> None:
+    A = graph.adjacency_matrix_from_atomic_coordinates(
+        mol.mol.atomicnums, mol.mol.coordinates
+    )
 
     G = graph.graph_from_adjacency_matrix(A)
 
-    assert graph.num_vertices(G) == len(mol)
-    assert graph.num_edges(G) == n_bonds
+    assert graph.num_vertices(G) == mol.n_atoms
+    assert graph.num_edges(G) == mol.n_bonds
 
 
-@pytest.mark.parametrize("mol", molecules.allobmolecules)
-def test_adjacency_matrix_from_mol(mol) -> None:
-    natoms = io.numatoms(mol)
-    nbonds = io.numbonds(mol)
+def test_adjacency_matrix_from_mol(rawmol) -> None:
+    natoms = io.numatoms(rawmol.rawmol)
+    nbonds = io.numbonds(rawmol.rawmol)
 
-    A = io.adjacency_matrix(mol)
+    assert natoms == rawmol.n_atoms
+    assert nbonds == rawmol.n_bonds
+
+    A = io.adjacency_matrix(rawmol.rawmol)
 
     assert A.shape == (natoms, natoms)
     assert np.all(A == A.T)
     assert np.sum(A) == nbonds * 2
 
-    for i, j in io.bonds(mol):
+    for i, j in io.bonds(rawmol.rawmol):
         assert A[i, j] == 1
 
 
-@pytest.mark.parametrize("mol", molecules.allobmolecules)
-def test_graph_from_adjacency_matrix(mol) -> None:
-    natoms = io.numatoms(mol)
-    nbonds = io.numbonds(mol)
+def test_graph_from_adjacency_matrix(rawmol) -> None:
+    natoms = io.numatoms(rawmol.rawmol)
+    nbonds = io.numbonds(rawmol.rawmol)
+
+    assert natoms == rawmol.n_atoms
+    assert nbonds == rawmol.n_bonds
 
-    A = io.adjacency_matrix(mol)
+    A = io.adjacency_matrix(rawmol.rawmol)
 
     assert A.shape == (natoms, natoms)
     assert np.all(A == A.T)
     assert np.sum(A) == nbonds * 2
 
     G = graph.graph_from_adjacency_matrix(A)
 
     assert graph.num_vertices(G) == natoms
     assert graph.num_edges(G) == nbonds
 
 
-@pytest.mark.parametrize(
-    "rawmol, mol", zip(molecules.allobmolecules, molecules.allmolecules)
-)
-def test_graph_from_adjacency_matrix_atomicnums(rawmol, mol) -> None:
-    natoms = io.numatoms(rawmol)
-    nbonds = io.numbonds(rawmol)
+def test_graph_from_adjacency_matrix_atomicnums(rawmol) -> None:
+    mol = rawmol.mol
 
-    A = io.adjacency_matrix(rawmol)
+    natoms = io.numatoms(rawmol.rawmol)
+    nbonds = io.numbonds(rawmol.rawmol)
+
+    A = io.adjacency_matrix(rawmol.rawmol)
 
     assert len(mol) == natoms
     assert mol.adjacency_matrix.shape == (natoms, natoms)
     assert np.all(mol.adjacency_matrix == A)
     assert np.sum(mol.adjacency_matrix) == nbonds * 2
 
     G = mol.to_graph()
@@ -94,36 +92,52 @@
     assert graph.num_vertices(G) == natoms
     assert graph.num_edges(G) == nbonds
 
     for idx, atomicnum in enumerate(mol.atomicnums):
         assert graph.vertex_property(G, "aprops", idx) == atomicnum
 
 
-@pytest.mark.parametrize(
-    "G1, G2",
-    [
-        *[(graph.lattice(n, n), graph.lattice(n, n)) for n in range(2, 5)],
-        *[(graph.cycle(n), graph.cycle(n)) for n in range(2, 5)],
-    ],
-)
-def test_match_graphs_isomorphic(G1, G2) -> None:
+@pytest.mark.parametrize("n", list(range(2, 5)))
+def test_match_graphs_isomorphic_lattice(n) -> None:
+    G1 = graph.lattice(n, n)
+    G2 = graph.lattice(n, n)
+
     with pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
         isomorphisms = graph.match_graphs(G1, G2)
 
     assert len(isomorphisms) != 0
 
 
-@pytest.mark.parametrize(
-    "G1, G2",
-    [
-        *[(graph.lattice(n, n), graph.lattice(n + 1, n)) for n in range(2, 5)],
-        *[(graph.cycle(n), graph.cycle(n + 1)) for n in range(1, 5)],
-    ],
-)
-def test_match_graphs_not_isomorphic(G1, G2) -> None:
+@pytest.mark.parametrize("n", list(range(2, 5)))
+def test_match_graphs_isomorphic_cycle(n) -> None:
+    G1 = graph.cycle(n)
+    G2 = graph.cycle(n)
+
+    with pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
+        isomorphisms = graph.match_graphs(G1, G2)
+
+    assert len(isomorphisms) != 0
+
+
+@pytest.mark.parametrize("n", list(range(2, 5)))
+def test_match_graphs_not_isomorphic_lattice(n) -> None:
+    G1 = graph.lattice(n, n)
+    G2 = graph.lattice(n + 1, n)
+
+    with pytest.raises(
+        NonIsomorphicGraphs, match=gc.error_non_isomorphic_graphs
+    ), pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
+        graph.match_graphs(G1, G2)
+
+
+@pytest.mark.parametrize("n", range(2, 5))
+def test_match_graphs_not_isomorphic_cycle(n) -> None:
+    G1 = graph.cycle(n)
+    G2 = graph.cycle(n + 1)
+
     with pytest.raises(
         NonIsomorphicGraphs, match=gc.error_non_isomorphic_graphs
     ), pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
         graph.match_graphs(G1, G2)
 
 
 @pytest.mark.parametrize(
@@ -144,14 +158,19 @@
 
 
 @pytest.mark.skipif(
     spyrmsd.get_backend() != "graph_tool",
     reason="NetworkX supports all Python objects as node properties.",
 )
 def test_build_graph_node_features_unsupported() -> None:
+    if spyrmsd.get_backend() != "graph-tool":
+        pytest.skip(
+            "NetworkX and RustworkX support all Python objects as node properties."
+        )
+
     A = np.array([[0, 1, 1], [1, 0, 0], [1, 0, 1]])
 
     property = [True, False, True]
 
     with pytest.raises(ValueError, match="Unsupported property type:"):
         _ = graph.graph_from_adjacency_matrix(A, property)
```

### Comparing `spyrmsd-0.7.0/tests/test_import.py` & `spyrmsd-0.8.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.7.0/tests/test_io.py` & `spyrmsd-0.8.0/tests/test_io.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,61 +7,66 @@
 fdir = os.path.dirname(os.path.abspath(__file__))
 molpath = os.path.join(fdir, "data/molecules/")
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("benzene.sdf", 12, 12), ("ethanol.sdf", 9, 8), ("dialanine.sdf", 23, 22)],
+    ids=["benzene", "ethanol", "dialanine"],
 )
 def test_load_sdf(molfile, natoms: int, nbonds: int) -> None:
     m = io.load(os.path.join(molpath, molfile))
 
     assert io.numatoms(m) == natoms
     assert io.numbonds(m) == nbonds
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("1cbr_ligand.mol2", 49, 49)],
+    ids=["1cbr_ligand"],
 )
 def test_load_mol2(molfile, natoms: int, nbonds: int) -> None:
     m = io.load(os.path.join(molpath, molfile))
 
     assert io.numatoms(m) == natoms
     assert io.numbonds(m) == nbonds
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("trp0.pdb", 217, 224), ("trp1.pdb", 217, 224), ("trp2.pdb", 217, 224)],
+    ids=["trp0", "trp1", "trp2"],
 )
 def test_load_pdb(molfile, natoms: int, nbonds: int) -> None:
     m = io.load(os.path.join(molpath, molfile))
 
     assert io.numatoms(m) == natoms
     assert io.numbonds(m) == nbonds
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("1cbr_docking.sdf", 22, 22)],
+    ids=["1cbr_docking"],
 )
 def test_loadall_sdf(molfile, natoms: int, nbonds: int) -> None:
     ms = io.loadall(os.path.join(molpath, molfile))
 
     assert len(ms) == 10
 
     for m in ms:
         assert io.numatoms(m) == natoms
         assert io.numbonds(m) == nbonds
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("1cbr_docking.mol2", 22, 22)],
+    ids=["1cbr_docking"],
 )
 def test_loadall_mol2(molfile, natoms: int, nbonds: int) -> None:
     try:
         ms = io.loadall(os.path.join(molpath, molfile))
 
         assert len(ms) == 10
 
@@ -71,14 +76,15 @@
     except NotImplementedError:  # Mol2MolSupplier in RDkit is not supported
         pass  # TODO: Warning
 
 
 @pytest.mark.parametrize(
     "molfile, natoms, nbonds",
     [("1cbr_docking.pdb", 22, 22)],
+    ids=["1cbr_docking"],
 )
 def test_loadall_pdb(molfile, natoms: int, nbonds: int) -> None:
     try:
         ms = io.loadall(os.path.join(molpath, molfile))
 
         assert len(ms) == 10
 
@@ -106,57 +112,62 @@
     except NotImplementedError:  # PDBMolSupplier in RDkit is not supported
         pass  # TODO: Warning
 
 
 @pytest.mark.parametrize(
     "molfile, natoms",
     [("benzene.sdf", 12), ("ethanol.sdf", 9), ("dialanine.sdf", 23)],
+    ids=["benzene", "ethanol", "dialanine"],
 )
 def test_loadmol_sdf(molfile, natoms: int) -> None:
     m = io.loadmol(os.path.join(molpath, molfile))
 
     assert len(m) == natoms
 
 
 @pytest.mark.parametrize(
     "molfile, natoms",
     [("benzene.mol2", 12), ("1cbr_ligand.mol2", 49)],
+    ids=["benzene", "1cbr_ligand"],
 )
 def test_loadmol_mol2(molfile, natoms: int) -> None:
     m = io.loadmol(os.path.join(molpath, molfile))
 
     assert len(m) == natoms
 
 
 @pytest.mark.parametrize(
     "molfile, natoms",
     [("1cbr_docking.sdf", 22)],
+    ids=["1cbr_docking"],
 )
 def test_loadallmols_sdf(molfile, natoms: int) -> None:
     ms = io.loadallmols(os.path.join(molpath, molfile))
 
     assert len(ms) == 10
 
     for m in ms:
         assert len(m) == natoms
 
 
 @pytest.mark.parametrize(
     "molfile, natoms",
     [("benzene.sdf.gz", 12), ("benzene.mol2.gz", 12), ("1a99_ligand.pdb.gz", 20)],
+    ids=["benzene", "benzene_mol2", "1a99_ligand"],
 )
 def test_loadmol_gz(molfile, natoms: int) -> None:
     m = io.loadmol(os.path.join(molpath, molfile))
 
     assert len(m) == natoms
 
 
 @pytest.mark.parametrize(
     "molfile, natoms",
     [("1cbr_docking.sdf.gz", 22)],
+    ids=["1cbr_docking"],
 )
 def test_loadallmols_sdf_gz(molfile, natoms: int) -> None:
     ms = io.loadallmols(os.path.join(molpath, molfile))
 
     assert len(ms) == 10
 
     for m in ms:
```

### Comparing `spyrmsd-0.7.0/tests/test_large.py` & `spyrmsd-0.8.0/tests/test_large.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import numpy as np
 import pytest
 import requests
 
 from spyrmsd import io, qcp, rmsd
 
 
-@pytest.fixture(autouse=True, params=[True, False])
+@pytest.fixture(
+    autouse=True, params=[True, False], ids=["lamnda_max_fast", "lambda_max_fallback"]
+)
 def lambda_max_failure(monkeypatch, request):
     """
     Monkey patch fixture for :code:`lambda_max` function to simulate convergence
     failures.
 
     Notes
     -----
@@ -91,15 +93,15 @@
     assert len(download) == pytest.n_systems
 
     for id in download:
         assert os.path.isdir(path_from_id(id, path))
 
 
 @pytest.mark.large
-@pytest.mark.parametrize("minimize", [True, False])
+@pytest.mark.parametrize("minimize", [True, False], ids=["minimize", "no_minimize"])
 def test_rmsd(idx, download, path, minimize):
     id = download[idx]
 
     p = path_from_id(id, path)
 
     try:
         ref = io.loadmol(os.path.join(p, f"{id}_ligand.sdf"))
```

### Comparing `spyrmsd-0.7.0/tests/test_molecule.py` & `spyrmsd-0.8.0/tests/test_molecule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,94 @@
 import copy
 import os
 from collections import defaultdict
-from typing import DefaultDict, List, Tuple
+from typing import DefaultDict
 
 import numpy as np
 import pytest
 
-import spyrmsd
 from spyrmsd import constants, graph, io, molecule, utils
-from tests import molecules
 
 
-# atoms is a list of atomic numbers and atom counts
-@pytest.mark.parametrize(
-    "mol, atoms",
-    [
-        (molecules.benzene, [(1, 6), (6, 6)]),
-        (molecules.ethanol, [(1, 6), (6, 2), (8, 1)]),
-        (molecules.dialanine, [(1, 12), (6, 6), (7, 2), (8, 3)]),
-    ],
-)
-def test_load(mol: molecule.Molecule, atoms: List[Tuple[int, int]]) -> None:
-    n = sum([n_atoms for _, n_atoms in atoms])
-
-    assert len(mol) == n
-    assert mol.atomicnums.shape == (n,)
-    assert mol.coordinates.shape == (n, 3)
+def test_load(mol) -> None:
+    # Atoms for each type
+    atoms = {
+        "benzene": [(1, 6), (6, 6)],
+        "ethanol": [(1, 6), (6, 2), (8, 1)],
+        "pyridine": [(1, 5), (6, 5), (7, 1)],
+        "dialanine": [(1, 12), (6, 6), (7, 2), (8, 3)],
+    }
+
+    n = sum([n_atoms for _, n_atoms in atoms[mol.name]])
+
+    assert mol.n_atoms == n
+    assert mol.mol.atomicnums.shape == (n,)
+    assert mol.mol.coordinates.shape == (n, 3)
 
     # Count number of atoms of different elements
     atomcount: DefaultDict[int, int] = defaultdict(int)
-    for atomicnum in mol.atomicnums:
+    for atomicnum in mol.mol.atomicnums:
         atomcount[atomicnum] += 1
 
-    assert len(atomcount) == len(atoms)
+    assert len(atomcount) == len(atoms[mol.name])
 
-    for Z, n_atoms in atoms:
+    for Z, n_atoms in atoms[mol.name]:
         assert atomcount[Z] == n_atoms
 
 
-def test_loadall() -> None:
-    path = os.path.join(molecules.molpath, "1cbr_docking.sdf")
+def test_loadall(molpath) -> None:
+    path = os.path.join(molpath, "1cbr_docking.sdf")
 
     mols = io.loadall(path)
 
     assert len(mols) == 10
 
 
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_molecule_translate(mol: molecule.Molecule) -> None:
-    mt = copy.deepcopy(mol)
+def test_molecule_translate(mol) -> None:
+    mt = copy.deepcopy(mol.mol)
 
     t = np.array([0.5, 1.1, -0.1])
     mt.translate(t)
 
-    for tcoord, coord in zip(mt.coordinates, mol.coordinates):
+    for tcoord, coord in zip(mt.coordinates, mol.mol.coordinates):
         assert np.allclose(tcoord - t, coord)
 
 
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_molecule_rotate_z(mol: molecule.Molecule) -> None:
+def test_molecule_rotate_z(mol) -> None:
     z_axis = np.array([0, 0, 1])
 
     for angle in [0, 45, 90]:
-        rotated = np.zeros((len(mol), 3))
-        for i, coord in enumerate(mol.coordinates):
+        rotated = np.zeros((mol.n_atoms, 3))
+        for i, coord in enumerate(mol.mol.coordinates):
             rotated[i] = utils.rotate(coord, angle, z_axis, units="deg")
 
-        mol.rotate(angle, z_axis, units="deg")
+        mol.mol.rotate(angle, z_axis, units="deg")
 
-        assert np.allclose(mol.coordinates, rotated)
+        assert np.allclose(mol.mol.coordinates, rotated)
 
-        # Reset
-        mol.rotate(-angle, z_axis, units="deg")
 
-
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_molecule_rotate(mol: molecule.Molecule) -> None:
+def test_molecule_rotate(mol) -> None:
     axis = np.random.rand(3)
 
     for angle in np.random.rand(10) * 180:
-        rotated = np.zeros((len(mol), 3))
-        for i, coord in enumerate(mol.coordinates):
+        rotated = np.zeros((mol.n_atoms, 3))
+        for i, coord in enumerate(mol.mol.coordinates):
             rotated[i] = utils.rotate(coord, angle, axis, units="deg")
 
-        mol.rotate(angle, axis, units="deg")
-
-        assert np.allclose(mol.coordinates, rotated)
+        mol.mol.rotate(angle, axis, units="deg")
 
-        # Reset
-        mol.rotate(-angle, axis, units="deg")
+        assert np.allclose(mol.mol.coordinates, rotated)
 
 
-def test_molecule_center_of_geometry_benzene() -> None:
-    mol = molecules.benzene
+def test_molecule_center_of_geometry_benzene(benzene) -> None:
+    assert np.allclose(benzene.mol.center_of_geometry(), np.zeros(3))
 
-    assert np.allclose(mol.center_of_geometry(), np.zeros(3))
 
-
-def test_molecule_center_of_mass_benzene() -> None:
-    mol = molecules.benzene
-
-    assert np.allclose(mol.center_of_mass(), np.zeros(3))
+def test_molecule_center_of_mass_benzene(benzene) -> None:
+    assert np.allclose(benzene.mol.center_of_mass(), np.zeros(3))
 
 
 def test_molecule_center_of_mass_H2() -> None:
     atomicnums = [1, 1]
     coordinates = [[0.0, 0.0, -1.0], [0.0, 0.0, 1.0]]
 
     mol = molecule.Molecule(atomicnums, coordinates)
@@ -122,80 +106,63 @@
     z_com = (-H_mass + F_mass) / (H_mass + F_mass)
 
     mol = molecule.Molecule(atomicnums, coordinates)
 
     assert np.allclose(mol.center_of_mass(), np.array([0, 0, z_com]))
 
 
-@pytest.mark.parametrize(
-    "mol, n_atoms, stripped",
-    [
-        (molecules.benzene, 12, 6),
-        (molecules.ethanol, 9, 6),
-        (molecules.dialanine, 23, 12),
-    ],
-)
-def test_molecule_strip(mol: molecule.Molecule, n_atoms: int, stripped: int) -> None:
-    m = copy.deepcopy(mol)
+def test_molecule_strip(mol) -> None:
+    m = copy.deepcopy(mol.mol)
 
-    assert len(m) == n_atoms
+    assert len(m) == mol.n_atoms
 
     m.strip()
 
-    assert len(m) == n_atoms - stripped
+    assert len(m) == mol.n_atoms - mol.n_h
 
 
-@pytest.mark.parametrize(
-    "mol, n_bonds",
-    [(molecules.benzene, 12), (molecules.ethanol, 8), (molecules.dialanine, 22)],
-)
-def test_graph_from_adjacency_matrix(mol: molecule.Molecule, n_bonds: int) -> None:
-    G = mol.to_graph()
+def test_graph_from_adjacency_matrix(mol) -> None:
+    G = mol.mol.to_graph()
 
-    assert graph.num_vertices(G) == len(mol)
-    assert graph.num_edges(G) == n_bonds
+    assert graph.num_vertices(G) == mol.n_atoms
+    assert graph.num_edges(G) == mol.n_bonds
 
-    for idx, atomicnum in enumerate(mol.atomicnums):
+    for idx, atomicnum in enumerate(mol.mol.atomicnums):
         assert graph.vertex_property(G, "aprops", idx) == atomicnum
 
 
-@pytest.mark.parametrize(
-    "mol, n_bonds",
-    [(molecules.benzene, 12), (molecules.ethanol, 8), (molecules.dialanine, 22)],
-)
-def test_graph_from_atomic_coordinates_perception(
-    mol: molecule.Molecule, n_bonds: int
-) -> None:
-    m = copy.deepcopy(mol)
+def test_graph_from_atomic_coordinates_perception(mol) -> None:
+    m = copy.deepcopy(mol.mol)
 
     delattr(m, "adjacency_matrix")
     m.G = {}
 
     with pytest.warns(UserWarning):
         # Uses automatic bond perception
         G = m.to_graph()
 
-        assert graph.num_vertices(G) == len(m)
-        assert graph.num_edges(G) == n_bonds
+        assert graph.num_vertices(G) == mol.n_atoms
+        assert graph.num_edges(G) == mol.n_bonds
 
-        for idx, atomicnum in enumerate(mol.atomicnums):
+        for idx, atomicnum in enumerate(mol.mol.atomicnums):
             assert graph.vertex_property(G, "aprops", idx) == atomicnum
 
 
 @pytest.mark.parametrize(
     "adjacency",
     [True, False],
+    ids=["adjacency", "no_adjacency"],
 )
-def test_from_obmol(adjacency):
+def test_from_obmol(molpath, adjacency):
     pytest.importorskip("openbabel")
 
     from spyrmsd.optional import obabel as ob
 
     # Load molecules with OpenBabel
-    path = os.path.join(molecules.molpath, "1cbr_docking.sdf")
+    path = os.path.join(molpath, "1cbr_docking.sdf")
     mols = ob.loadall(path)
 
     # Convert OpenBabel molecules to spyrmsd molecules
     mols = [molecule.Molecule.from_obabel(mol, adjacency) for mol in mols]
 
     assert len(mols) == 10
 
@@ -209,22 +176,23 @@
                 # No adjacency_matrix attribute
                 mol.adjacency_matrix
 
 
 @pytest.mark.parametrize(
     "adjacency",
     [True, False],
+    ids=["adjacency", "no_adjacency"],
 )
-def test_from_rdmol(adjacency):
+def test_from_rdmol(molpath, adjacency):
     pytest.importorskip("rdkit")
 
     from spyrmsd.optional import rdkit as rd
 
     # Load molecules with RDKit
-    path = os.path.join(molecules.molpath, "1cbr_docking.sdf")
+    path = os.path.join(molpath, "1cbr_docking.sdf")
     mols = rd.loadall(path)
 
     # Convert OpenBabel molecules to spyrmsd molecules
     mols = [molecule.Molecule.from_rdkit(mol, adjacency) for mol in mols]
 
     assert len(mols) == 10
 
@@ -233,45 +201,7 @@
 
         if adjacency:
             assert mol.adjacency_matrix is not None
         else:
             with pytest.raises(AttributeError):
                 # No adjacency_matrix attribute
                 mol.adjacency_matrix
-
-
-@pytest.mark.skipif(
-    # Run test if all supported backends are installed
-    not set(spyrmsd.graph._supported_backends) <= set(spyrmsd.available_backends),
-    reason="Not all of the required backends are installed",
-)
-@pytest.mark.parametrize(
-    "mol", [(molecules.benzene), (molecules.ethanol), (molecules.dialanine)]
-)
-def test_molecule_graph_cache(mol) -> None:
-    import graph_tool as gt
-    import networkx as nx
-    import rustworkx as rx
-
-    ## Graph cache persists from previous tests, manually reset them
-    mol.G = {}
-    spyrmsd.set_backend("networkx")
-    mol.to_graph()
-
-    assert isinstance(mol.G["networkx"], nx.Graph)
-    assert "graph_tool" not in mol.G.keys()
-
-    spyrmsd.set_backend("graph-tool")
-    mol.to_graph()
-
-    spyrmsd.set_backend("rustworkx")
-    mol.to_graph()
-
-    ## Make sure all backends (still) have a cache
-    assert isinstance(mol.G["networkx"], nx.Graph)
-    assert isinstance(mol.G["graph_tool"], gt.Graph)
-    assert isinstance(mol.G["rustworkx"], rx.PyGraph)
-
-    ## Strip the molecule to ensure the cache is reset
-    mol.strip()
-
-    assert len(mol.G.items()) == 0
```

### Comparing `spyrmsd-0.7.0/tests/test_rmsd.py` & `spyrmsd-0.8.0/tests/test_rmsd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import copy
 from typing import List
 
 import numpy as np
 import pytest
 
-from spyrmsd import molecule, qcp, rmsd
-from tests import molecules
+from spyrmsd import qcp, rmsd
 
 
-@pytest.fixture(autouse=True, params=[True, False])
+@pytest.fixture(
+    autouse=True, params=[True, False], ids=["lambda_max_fast", "lambda_max_fallback"]
+)
 def lambda_max_failure(monkeypatch, request):
     """
     Monkey patch fixture for :code:`lambda_max` function to simulate convergence
     failures.
 
     Notes
     -----
@@ -33,60 +34,66 @@
         def lambda_max_failure(Ga, Gb, c2, c1, c0):
             # Simulate Newton method convergence failure
             raise RuntimeError
 
         monkeypatch.setattr(qcp, "lambda_max", lambda_max_failure)
 
 
-@pytest.mark.parametrize("t, RMSD", [(0.0, 0.0), (1.0, 1.0), (2.0, 2.0)])
-def test_rmsd_benzene(t: float, RMSD: float) -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+@pytest.mark.parametrize(
+    "t, RMSD", [(0.0, 0.0), (1.0, 1.0), (2.0, 2.0)], ids=["t0", "t1", "t2"]
+)
+def test_rmsd_benzene(benzene, t: float, RMSD: float) -> None:
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     mol2.translate(np.array([0, 0, t]))
 
     assert rmsd.rmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(RMSD)
 
 
 # Results obtained with PyTraj
 #   pytraj.analysis.rmsd.rmsd(i, ref=j, nofit=True)
 @pytest.mark.parametrize(
-    "i, j, result", [(1, 2, 2.60065218), (1, 3, 9.94411523), (2, 3, 9.4091711)]
-)
-def test_rmsd_2viz(i: int, j: int, result: float) -> None:
-    moli = copy.deepcopy(molecules.docking_2viz[i])
-    molj = copy.deepcopy(molecules.docking_2viz[j])
+    "i, j, result",
+    [(1, 2, 2.60065218), (1, 3, 9.94411523), (2, 3, 9.4091711)],
+    ids=["1-2", "1-3", "2-3"],
+)
+def test_rmsd_2viz(docking_2viz, i: int, j: int, result: float) -> None:
+    moli = copy.deepcopy(docking_2viz[i])
+    molj = copy.deepcopy(docking_2viz[j])
 
     assert rmsd.rmsd(
         moli.coordinates, molj.coordinates, moli.atomicnums, molj.atomicnums
     ) == pytest.approx(result)
 
 
 # Results obtained with PyTraj
 #   pytraj.analysis.rmsd.rmsd(i, mask="!@H=", ref=j, ref_mask="!@H=", nofit=True)
 @pytest.mark.parametrize(
-    "i, j, result", [(1, 2, 2.65327362), (1, 3, 10.11099065), (2, 3, 9.57099612)]
-)
-def test_rmsd_2viz_stripped(i: int, j: int, result: float) -> None:
-    moli = copy.deepcopy(molecules.docking_2viz[i])
-    molj = copy.deepcopy(molecules.docking_2viz[j])
+    "i, j, result",
+    [(1, 2, 2.65327362), (1, 3, 10.11099065), (2, 3, 9.57099612)],
+    ids=["1-2", "1-3", "2-3"],
+)
+def test_rmsd_2viz_stripped(docking_2viz, i: int, j: int, result: float) -> None:
+    moli = copy.deepcopy(docking_2viz[i])
+    molj = copy.deepcopy(docking_2viz[j])
 
     moli.strip()
     molj.strip()
 
     assert rmsd.rmsd(
         moli.coordinates, molj.coordinates, moli.atomicnums, molj.atomicnums
     ) == pytest.approx(result)
 
 
-def test_rmsd_centred_benzene() -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+def test_rmsd_centred_benzene(benzene) -> None:
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     mol2.translate(np.array([0, 0, 1]))
 
     assert rmsd.rmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(1)
 
@@ -95,18 +102,17 @@
         mol2.coordinates,
         mol1.atomicnums,
         mol2.atomicnums,
         center=True,
     ) == pytest.approx(0)
 
 
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_rmsd_minimize(mol: molecule.Molecule) -> None:
-    mol1 = copy.deepcopy(mol)
-    mol2 = copy.deepcopy(mol)
+def test_rmsd_minimize(mol) -> None:
+    mol1 = copy.deepcopy(mol.mol)
+    mol2 = copy.deepcopy(mol.mol)
 
     assert rmsd.rmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(0)
 
     assert rmsd.rmsd(
         mol1.coordinates,
@@ -135,37 +141,41 @@
             minimize=True,
         ) == pytest.approx(0)
 
 
 # Results obtained with PyTraj
 #   pytraj.analysis.rmsd.rmsd(i, ref=j)
 @pytest.mark.parametrize(
-    "i, j, result", [(1, 2, 1.95277757), (1, 3, 3.11801105), (2, 3, 2.98609758)]
-)
-def test_rmsd_qcp_2viz(i: int, j: int, result: float) -> None:
-    moli = copy.deepcopy(molecules.docking_2viz[i])
-    molj = copy.deepcopy(molecules.docking_2viz[j])
+    "i, j, result",
+    [(1, 2, 1.95277757), (1, 3, 3.11801105), (2, 3, 2.98609758)],
+    ids=["1-2", "1-3", "2-3"],
+)
+def test_rmsd_qcp_2viz(docking_2viz, i: int, j: int, result: float) -> None:
+    moli = copy.deepcopy(docking_2viz[i])
+    molj = copy.deepcopy(docking_2viz[j])
 
     assert rmsd.rmsd(
         moli.coordinates,
         molj.coordinates,
         moli.atomicnums,
         molj.atomicnums,
         minimize=True,
     ) == pytest.approx(result)
 
 
 # Results obtained with PyTraj
 #   pytraj.analysis.rmsd.rmsd(i, "!@H=", ref=j, ref_mask="!@H=")
 @pytest.mark.parametrize(
-    "i, j, result", [(1, 2, 1.98171656), (1, 3, 3.01799306), (2, 3, 2.82917355)]
-)
-def test_rmsd_qcp_2viz_stripped(i: int, j: int, result: float) -> None:
-    moli = copy.deepcopy(molecules.docking_2viz[i])
-    molj = copy.deepcopy(molecules.docking_2viz[j])
+    "i, j, result",
+    [(1, 2, 1.98171656), (1, 3, 3.01799306), (2, 3, 2.82917355)],
+    ids=["1-2", "1-3", "2-3"],
+)
+def test_rmsd_qcp_2viz_stripped(docking_2viz, i: int, j: int, result: float) -> None:
+    moli = copy.deepcopy(docking_2viz[i])
+    molj = copy.deepcopy(docking_2viz[j])
 
     # Strip hydrogen atoms
     moli.strip()
     molj.strip()
 
     assert rmsd.rmsd(
         moli.coordinates,
@@ -190,18 +200,19 @@
     [
         (1, 4.812480551076202, 1.6578281551053196),
         (2, 6.772045449820714, 1.7175638492348284),
         (3, 9.344911262612964, 1.5946081072641485),
         (4, 9.772939589989000, 2.1234944939308220),
         (5, 8.901837608843241, 2.4894805175766606),
     ],
+    ids=["1", "2", "3", "4", "5"],
 )
-def test_rmsd_qcp_protein(i: int, rmsd_dummy: float, rmsd_min: float):
-    mol0 = copy.deepcopy(molecules.trp[0])
-    mol = copy.deepcopy(molecules.trp[i])
+def test_rmsd_qcp_protein(trps, i: int, rmsd_dummy: float, rmsd_min: float):
+    mol0 = copy.deepcopy(trps[0])
+    mol = copy.deepcopy(trps[i])
 
     assert rmsd.rmsd(
         mol0.coordinates, mol.coordinates, mol0.atomicnums, mol.atomicnums
     ) == pytest.approx(rmsd_dummy)
 
     assert rmsd.rmsd(
         mol0.coordinates,
@@ -209,19 +220,21 @@
         mol0.atomicnums,
         mol.atomicnums,
         minimize=True,
     ) == pytest.approx(rmsd_min)
 
 
 @pytest.mark.parametrize(
-    "angle, tol", [(60, 1e-4), (120, 1e-4), (180, 1e-4), (240, 1e-4), (300, 1e-4)]
-)
-def test_rmsd_hungarian_benzene_rotated(angle: float, tol: float) -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+    "angle, tol",
+    [(60, 1e-4), (120, 1e-4), (180, 1e-4), (240, 1e-4), (300, 1e-4)],
+    ids=["60", "120", "180", "240", "300"],
+)
+def test_rmsd_hungarian_benzene_rotated(benzene, angle: float, tol: float) -> None:
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     assert rmsd.rmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(0)
 
     assert rmsd.hrmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
@@ -235,23 +248,27 @@
         > 0
     )
     assert rmsd.hrmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(0, abs=tol)
 
 
-@pytest.mark.parametrize("d", [-0.5, 0.0, 0.5, 1.0, 1.5])
 @pytest.mark.parametrize(
-    "angle, tol", [(60, 1e-4), (120, 1e-4), (180, 1e-4), (240, 1e-4), (300, 1e-4)]
+    "d", [-0.5, 0.0, 0.5, 1.0, 1.5], ids=["t1", "t2", "t3", "t4", "t5"]
+)
+@pytest.mark.parametrize(
+    "angle, tol",
+    [(60, 1e-4), (120, 1e-4), (180, 1e-4), (240, 1e-4), (300, 1e-4)],
+    ids=["60", "120", "180", "240", "300"],
 )
 def test_rmsd_hungarian_benzene_shifted_rotated(
-    d: float, angle: float, tol: float
+    benzene, d: float, angle: float, tol: float
 ) -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     mol2.translate([0, 0, d])
 
     assert rmsd.rmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(abs(d))
 
@@ -266,18 +283,17 @@
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) > abs(d)
     assert rmsd.hrmsd(
         mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums
     ) == pytest.approx(abs(d), abs=tol)
 
 
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_rmsd_hungarian_centred(mol: molecule.Molecule) -> None:
-    mol1 = copy.deepcopy(mol)
-    mol2 = copy.deepcopy(mol)
+def test_rmsd_hungarian_centred(mol) -> None:
+    mol1 = copy.deepcopy(mol.mol)
+    mol2 = copy.deepcopy(mol.mol)
 
     mol2.translate(np.random.rand(3))
 
     assert (
         rmsd.hrmsd(mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums)
         > 0
     )
@@ -287,18 +303,17 @@
         mol2.coordinates,
         mol1.atomicnums,
         mol2.atomicnums,
         center=True,
     ) == pytest.approx(0)
 
 
-@pytest.mark.parametrize("mol", molecules.allmolecules)
-def test_symmrmsd_centred(mol: molecule.Molecule) -> None:
-    mol1 = copy.deepcopy(mol)
-    mol2 = copy.deepcopy(mol)
+def test_symmrmsd_centred(mol) -> None:
+    mol1 = copy.deepcopy(mol.mol)
+    mol2 = copy.deepcopy(mol.mol)
 
     mol2.translate(np.random.rand(3))
 
     assert (
         rmsd.symmrmsd(
             mol1.coordinates,
             mol2.coordinates,
@@ -318,17 +333,17 @@
         mol1.adjacency_matrix,
         mol2.adjacency_matrix,
         center=True,
     ) == pytest.approx(0)
 
 
 @pytest.mark.parametrize("angle", [60, 120, 180, 240, 300, 360])
-def test_symmrmsd_rotated_benzene(angle: float) -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+def test_symmrmsd_rotated_benzene(benzene, angle: float) -> None:
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     mol2.rotate(angle, np.array([0, 0, 1]), units="deg")
 
     assert (
         rmsd.rmsd(mol1.coordinates, mol2.coordinates, mol1.atomicnums, mol2.atomicnums)
         > 0
     )
@@ -352,17 +367,17 @@
         mol2.atomicnums,
         mol1.adjacency_matrix,
         mol2.adjacency_matrix,
     ) == pytest.approx(0, abs=1e-4)
 
 
 @pytest.mark.parametrize("angle", [60, 120, 180, 240, 300, 360])
-def test_symmrmsd_rotated_benzene_stripped(angle: float) -> None:
-    mol1 = copy.deepcopy(molecules.benzene)
-    mol2 = copy.deepcopy(molecules.benzene)
+def test_symmrmsd_rotated_benzene_stripped(benzene, angle: float) -> None:
+    mol1 = copy.deepcopy(benzene.mol)
+    mol2 = copy.deepcopy(benzene.mol)
 
     mol2.rotate(angle, np.array([0, 0, 1]), units="deg")
 
     mol1.strip()
     mol2.strip()
 
     assert (
@@ -388,17 +403,17 @@
         mol1.atomicnums,
         mol2.atomicnums,
         mol1.adjacency_matrix,
         mol2.adjacency_matrix,
     ) == pytest.approx(0, abs=1e-4)
 
 
-def test_symmrmsd_atomicnums_matching_pyridine_stripped() -> None:
-    mol1 = copy.deepcopy(molecules.pyridine)
-    mol2 = copy.deepcopy(molecules.pyridine)
+def test_symmrmsd_atomicnums_matching_pyridine_stripped(pyridine) -> None:
+    mol1 = copy.deepcopy(pyridine.mol)
+    mol2 = copy.deepcopy(pyridine.mol)
 
     mol2.rotate(60, np.array([0, 0, 1]), units="deg")
 
     mol1.strip()
     mol2.strip()
 
     # Standard RMSD, correct in this case
@@ -439,18 +454,40 @@
         (5, 1.01324, True),
         (6, 1.31716, True),
         (7, 1.11312, True),
         (8, 1.06044, True),
         (9, 0.965387, True),
         (10, 1.37842, True),
     ],
+    ids=[
+        "1-no_minimize",
+        "2-no_minimize",
+        "3-no_minimize",
+        "4-no_minimize",
+        "5-no_minimize",
+        "6-no_minimize",
+        "7-no_minimize",
+        "8-no_minimize",
+        "9-no_minimize",
+        "10-no_minimize",
+        "1-minimize",
+        "2-minimize",
+        "3-minimize",
+        "4-minimize",
+        "5-minimize",
+        "6-minimize",
+        "7-minimize",
+        "8-minimize",
+        "9-minimize",
+        "10-minimize",
+    ],
 )
-def test_rmsd_symmrmsd(index: int, RMSD: float, minimize: bool) -> None:
-    molc = copy.deepcopy(molecules.docking_1cbr[0])
-    mol = copy.deepcopy(molecules.docking_1cbr[index])
+def test_rmsd_symmrmsd(docking_1cbr, index: int, RMSD: float, minimize: bool) -> None:
+    molc = copy.deepcopy(docking_1cbr[0])
+    mol = copy.deepcopy(docking_1cbr[index])
 
     molc.strip()
     mol.strip()
 
     assert rmsd.symmrmsd(
         molc.coordinates,
         mol.coordinates,
@@ -504,18 +541,21 @@
                 1.11312,
                 1.06044,
                 0.965387,
                 1.37842,
             ],
         ),
     ],
+    ids=["no_minimize", "minimize"],
 )
-def test_multi_spyrmsd(minimize: bool, referenceRMSDs: List[float]) -> None:
-    molc = copy.deepcopy(molecules.docking_1cbr[0])
-    mols = [copy.deepcopy(mol) for mol in molecules.docking_1cbr[1:]]
+def test_multi_spyrmsd(
+    docking_1cbr, minimize: bool, referenceRMSDs: List[float]
+) -> None:
+    molc = copy.deepcopy(docking_1cbr[0])
+    mols = [copy.deepcopy(mol) for mol in docking_1cbr[1:]]
 
     molc.strip()
 
     for mol in mols:
         mol.strip()
 
     RMSDs = rmsd.symmrmsd(
@@ -563,18 +603,21 @@
                 1.11312,
                 1.06044,
                 0.965387,
                 1.37842,
             ],
         ),
     ],
+    ids=["no_minimize", "minimize"],
 )
-def test_symmrmsd_cache(minimize: bool, referenceRMSDs: List[float]) -> None:
-    molc = copy.deepcopy(molecules.docking_1cbr[0])
-    mols = [copy.deepcopy(mol) for mol in molecules.docking_1cbr[1:]]
+def test_symmrmsd_cache(
+    docking_1cbr, minimize: bool, referenceRMSDs: List[float]
+) -> None:
+    molc = copy.deepcopy(docking_1cbr[0])
+    mols = [copy.deepcopy(mol) for mol in docking_1cbr[1:]]
 
     molc.strip()
 
     for mol in mols:
         mol.strip()
 
     RMSDs = rmsd.symmrmsd(
@@ -705,26 +748,28 @@
         minimize=True,
     )
 
     assert r == pytest.approx(0.0)
 
 
 @pytest.mark.parametrize(
-    "i, j, result", [(1, 2, 1.95277757), (1, 3, 3.11801105), (2, 3, 2.98609758)]
+    "i, j, result",
+    [(1, 2, 1.95277757), (1, 3, 3.11801105), (2, 3, 2.98609758)],
+    ids=["1-2", "1-3", "2-3"],
 )
-def test_rmsd_atol(i: int, j: int, result: float):
+def test_rmsd_atol(docking_2viz, i: int, j: int, result: float):
     """
     Test usage of the :code:`atol` parameter for the QCP method.
 
     This parameter has been exposed to users following Issue 35 from @kjelljorner
     (https://github.com/RMeli/spyrmsd/issues/35)
     """
 
-    moli = copy.deepcopy(molecules.docking_2viz[i])
-    molj = copy.deepcopy(molecules.docking_2viz[j])
+    moli = copy.deepcopy(docking_2viz[i])
+    molj = copy.deepcopy(docking_2viz[j])
 
     # Check results are different from 0.0
     assert not result == pytest.approx(0.0)
 
     assert rmsd.rmsd(
         moli.coordinates,
         molj.coordinates,
@@ -740,18 +785,20 @@
         molj.atomicnums,
         minimize=True,
         atol=1e9,
     ) == pytest.approx(0.0)
 
 
 # Results obtained with OpenBabel
-@pytest.mark.parametrize("i, reference", [(1, 0.476858), (2, 1.68089), (3, 1.50267)])
-def test_symmrmsd_atol(i: bool, reference: float) -> None:
-    moli = copy.deepcopy(molecules.docking_1cbr[0])
-    molj = copy.deepcopy(molecules.docking_1cbr[i])
+@pytest.mark.parametrize(
+    "i, reference", [(1, 0.476858), (2, 1.68089), (3, 1.50267)], ids=["1", "2", "3"]
+)
+def test_symmrmsd_atol(docking_1cbr, i: bool, reference: float) -> None:
+    moli = copy.deepcopy(docking_1cbr[0])
+    molj = copy.deepcopy(docking_1cbr[i])
 
     moli.strip()
     molj.strip()
 
     # Check results are different from 0.0
     assert not reference == pytest.approx(0.0)
 
@@ -773,19 +820,19 @@
         moli.adjacency_matrix,
         molj.adjacency_matrix,
         minimize=True,
         atol=1e9,
     ) == pytest.approx(0.0)
 
 
-def test_symmrmsd_atol_multi() -> None:
+def test_symmrmsd_atol_multi(docking_1cbr) -> None:
     references = [0.476858, 1.68089, 1.50267]
 
-    molc = copy.deepcopy(molecules.docking_1cbr[0])
-    mols = [copy.deepcopy(mol) for mol in molecules.docking_1cbr[1:4]]
+    molc = copy.deepcopy(docking_1cbr[0])
+    mols = [copy.deepcopy(mol) for mol in docking_1cbr[1:4]]
 
     molc.strip()
 
     for mol in mols:
         mol.strip()
 
     # Check results are different from 0.0
@@ -848,18 +895,19 @@
                 1.7175638492348284,
                 1.5946081072641485,
                 2.1234944939308220,
                 2.4894805175766606,
             ],
         ),
     ],
+    ids=["no_minimize", "minimize"],
 )
-def test_rmsdwrapper_nosymm_protein(minimize: bool, referenceRMSDs: List[float]):
-    mol0 = copy.deepcopy(molecules.trp[0])
-    mols = [copy.deepcopy(mol) for mol in molecules.trp[1:]]
+def test_rmsdwrapper_nosymm_protein(trps, minimize: bool, referenceRMSDs: List[float]):
+    mol0 = copy.deepcopy(trps[0])
+    mols = [copy.deepcopy(mol) for mol in trps[1:]]
 
     RMSDs = rmsd.rmsdwrapper(mol0, mols, symmetry=False, minimize=minimize, strip=False)
 
     for RMSD, referenceRMSD in zip(RMSDs, referenceRMSDs):
         assert RMSD == pytest.approx(referenceRMSD)
 
 
@@ -894,30 +942,36 @@
                 9.59758,
                 9.55076,
                 2.44067,
                 9.6171,
             ],
         ),
     ],
+    ids=["minimize", "no_minimize"],
 )
-def test_rmsdwrapper_isomorphic(minimize: bool, referenceRMSDs: List[float]) -> None:
-    molref = copy.deepcopy(molecules.docking_1cbr[0])
-    mols = [copy.deepcopy(mol) for mol in molecules.docking_1cbr[1:]]
+def test_rmsdwrapper_isomorphic(
+    docking_1cbr, minimize: bool, referenceRMSDs: List[float]
+) -> None:
+    molref = copy.deepcopy(docking_1cbr[0])
+    mols = [copy.deepcopy(mol) for mol in docking_1cbr[1:]]
 
     RMSDs = rmsd.rmsdwrapper(molref, mols, minimize=minimize, strip=True)
 
     for RMSD, referenceRMSD in zip(RMSDs, referenceRMSDs):
         assert RMSD == pytest.approx(referenceRMSD, abs=1e-5)
 
 
 @pytest.mark.parametrize(
     # Reference results obtained with OpenBabel
     "minimize, referenceRMSD",
     [(True, 0.476858), (False, 0.592256)],
+    ids=["minimize", "no_minimize"],
 )
-def test_rmsdwrapper_single_molecule(minimize: bool, referenceRMSD: float) -> None:
-    molref = copy.deepcopy(molecules.docking_1cbr[0])
-    mols = copy.deepcopy(molecules.docking_1cbr[1])
+def test_rmsdwrapper_single_molecule(
+    docking_1cbr, minimize: bool, referenceRMSD: float
+) -> None:
+    molref = copy.deepcopy(docking_1cbr[0])
+    mols = copy.deepcopy(docking_1cbr[1])
 
     RMSD = rmsd.rmsdwrapper(molref, mols, minimize=minimize, strip=True)
 
     assert RMSD[0] == pytest.approx(referenceRMSD, abs=1e-5)
```

### Comparing `spyrmsd-0.7.0/tests/test_utils.py` & `spyrmsd-0.8.0/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         fmt = utils.molformat(f"{fname}.{extin}")
         assert fmt == extout
 
 
 @pytest.mark.parametrize(
     "deg, rad",
     [(0, 0), (90, np.pi / 2), (180, np.pi), (270, 3 * np.pi / 2), (360, 2 * np.pi)],
+    ids=["0", "90", "180", "270", "360"],
 )
 def test_deg_to_rad(deg: float, rad: float) -> None:
     assert utils.deg_to_rad(deg) == pytest.approx(rad)
 
 
 def test_rotate_invalid():
     with pytest.raises(ValueError):
```

### Comparing `spyrmsd-0.7.0/PKG-INFO` & `spyrmsd-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: spyrmsd
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python RMSD tool with symmetry correction.
 Home-page: https://spyrmsd.readthedocs.io
 Author: Rocco Meli
 Author-email: rocco.meli@cscs.ch
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: networkx>=2
+Requires-Dist: rustworkx
 
 # sPyRMSD
 
 [![pytest](https://github.com/RMeli/spyrmsd/actions/workflows/pytest.yml/badge.svg?branch=develop)](https://github.com/RMeli/spyrmsd/actions/workflows/pytest.yml)
 ![flake8](https://github.com/RMeli/spyrmsd/workflows/flake8/badge.svg)
 ![mypy](https://github.com/RMeli/spyrmsd/workflows/mypy/badge.svg)
 [![codecov](https://codecov.io/gh/RMeli/spyrmsd/branch/develop/graph/badge.svg)](https://codecov.io/gh/RMeli/spyrmsd/branch/master)
@@ -49,15 +49,15 @@
 ```
 
 ## Installation
 
 `spyrmsd` is available on [PyPI](https://pypi.org/project/spyrmsd/) and [conda-forge](https://github.com/conda-forge/spyrmsd-feedstock) and can be easily installed from source. See [Dependencies](###Dependencies) for a description of all the dependencies.
 
 > [!NOTE]
-> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install the other backends for higher performance.
+> `spyrmsd` will install [rustworkx] (multi-platform) when using `pip` or `conda`. You can install other backends manually.
 
 > [!WARNING]
 > If `spyrmsd` is used as a standalone tool, it is required to install either [RDKit](https://rdkit.org/) or [Open Babel](http://openbabel.org/). Neither is automatically installed with `pip` nor `conda`.
 
 ### PyPI
 
 ```bash
@@ -87,19 +87,19 @@
 The following packages are required to use `spyrmsd` as a module:
 
 * [numpy](https://numpy.org/)
 * [scipy](https://www.scipy.org/)
 
 One of the following graph libraries is required:
 * [graph-tool]
-* [NetworkX]
 * [rustworkx]
+* [NetworkX]
 
 > [!NOTE]
-> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [NetworkX], [rustworkx]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.* However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and the other graph library need to be installed manually.
+> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [rustworkx], [NetworkX]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.*
 
 #### Standalone Tool
 
 Additionally, one of the following packages is required to use `spyrmsd` as a standalone tool:
 
 * [Open Babel](http://openbabel.org/)
 * [RDKit](https://rdkit.org/)
@@ -189,18 +189,18 @@
 
 ## Development
 
 To ensure code quality and consistency the following tools are used during development:
 
 * [black](https://black.readthedocs.io/en/stable/)
 * [Flake 8](http://flake8.pycqa.org/en/latest/) (CI)
-* [isort]()
+* [isort](https://pycqa.github.io/isort/)
 * [mypy](http://mypy-lang.org/) (CI)
 
-Pre-commit `git` hooks can be installed with [pre-commit](https://pre-commit.com/).
+Pre-commit `git` hooks can be installed with [pre-commit].
 
 ## Copyright
 
 Copyright (c) 2019-2024, Rocco Meli.
 
 ## References
 
@@ -209,8 +209,9 @@
 ### Acknowledgements
 
 Project based on the [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version `1.1`.
 
 [rustworkx]: https://www.rustworkx.org
 [NetworkX]: https://networkx.github.io/
 [graph-tool]: https://graph-tool.skewed.de/
+[pre-commit]: https://pre-commit.com/
```

