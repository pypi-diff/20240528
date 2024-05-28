# Comparing `tmp/massivechem-5.1.tar.gz` & `tmp/massivechem-5.2.tar.gz`

## Comparing `massivechem-5.1.tar` & `massivechem-5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.1/Focused_spectrum.png
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.1/Logo.jpg
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.1/MASSIVEChem.yml
--rw-r--r--   0        0        0    26315 2020-02-02 00:00:00.000000 massivechem-5.1/Schematic_mass_spectrum.png
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.1/Spectrum_output.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.1/project_final.yml
--rw-r--r--   0        0        0   103430 2020-02-02 00:00:00.000000 massivechem-5.1/notebooks/backup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.1/notebooks/checklist.txt
--rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 massivechem-5.1/notebooks/project_report.ipynb
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/all_in_one.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/functional_group_display.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/main_function.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/mol_web_show.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/peak_merger.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/spectrum.py
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/spectrum_3D.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.1/scripts/sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0   103430 2020-02-02 00:00:00.000000 massivechem-5.1/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.1/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.1/test/__init__.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_SMILEs_interpreter.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_calculate_unsaturation.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_delta_function_plotter.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_double_plot.py
--rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_functional_group_display.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_functional_group_finder.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_ionisation_method.py
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_main_function.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_mol_web_show.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_molecule_list_generator.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_peak_merger.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_peak_sorter.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_smiles_to_3D_plot.py
--rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_spectrum.py
--rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_spectrum_3D.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.1/test/test_sulphur_nitrogen_finder.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.1/LICENSE.txt
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 massivechem-5.1/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.1/pyproject.toml
--rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 massivechem-5.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.2/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-5.2/Logo.jpg
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-5.2/MASSIVEChem.yml
+-rw-r--r--   0        0        0    26315 2020-02-02 00:00:00.000000 massivechem-5.2/Schematic_mass_spectrum.png
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-5.2/Spectrum_output.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-5.2/project_final.yml
+-rw-r--r--   0        0        0   104043 2020-02-02 00:00:00.000000 massivechem-5.2/notebooks/backup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.2/notebooks/checklist.txt
+-rw-r--r--   0        0        0   106554 2020-02-02 00:00:00.000000 massivechem-5.2/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/spectrum.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-5.2/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103430 2020-02-02 00:00:00.000000 massivechem-5.2/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.2/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-5.2/test/__init__.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_double_plot.py
+-rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_functional_group_display.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_ionisation_method.py
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_main_function.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_mol_web_show.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_peak_merger.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_spectrum.py
+-rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-5.2/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-5.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-5.2/LICENSE.txt
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 massivechem-5.2/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-5.2/pyproject.toml
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 massivechem-5.2/PKG-INFO
```

### Comparing `massivechem-5.1/Logo.jpg` & `massivechem-5.2/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/MASSIVEChem.yml` & `massivechem-5.2/MASSIVEChem.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/Schematic_mass_spectrum.png` & `massivechem-5.2/Schematic_mass_spectrum.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/Spectrum_output.png` & `massivechem-5.2/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/project_final.yml` & `massivechem-5.2/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/notebooks/backup.py` & `massivechem-5.2/src/MASSiveChem/MASSiveChem.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/SMILEs_interpreter.py` & `massivechem-5.2/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/all_in_one.py` & `massivechem-5.2/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/calculate_unsaturation.py` & `massivechem-5.2/scripts/calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/delta_function_plotter.py` & `massivechem-5.2/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/double_plot.py` & `massivechem-5.2/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/functional_group_display.py` & `massivechem-5.2/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/functional_group_finder.py` & `massivechem-5.2/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/ionisation_method.py` & `massivechem-5.2/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/main_function.py` & `massivechem-5.2/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/mol_web_show.py` & `massivechem-5.2/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/molecule_list_generator.py` & `massivechem-5.2/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/peak_merger.py` & `massivechem-5.2/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/peak_sorter.py` & `massivechem-5.2/scripts/peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/smiles_to_3D_plot.py` & `massivechem-5.2/scripts/smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/spectrum.py` & `massivechem-5.2/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/spectrum_3D.py` & `massivechem-5.2/scripts/spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/sulphur_nitrogen_adder.py` & `massivechem-5.2/scripts/sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/scripts/sulphur_nitrogen_finder.py` & `massivechem-5.2/scripts/sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/src/MASSiveChem/MASSiveChem.py` & `massivechem-5.2/notebooks/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,19 @@
             N += 1
         elif atom.GetSymbol() in halogens_hydrogen:
             HX += 1
 
     unsaturation = C + 1 + (N - HX) / 2
 
     return unsaturation
-
+import time
 #2
 def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
-
+    begin = time.time()
+    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
     #tests for wether the input is valid
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     if imprecision_True_False not in [True, False]:
         raise ValueError('Enter a boolean value')
     if apparatus_resolution < 0:
         raise ValueError('Enter a positive value')
@@ -138,15 +139,15 @@
                 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
                 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
                 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
                 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
                 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
     
 
-    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+    
 
 
     
     mol = Chem.AddHs(mol_without_Hs)
 
     '''molecule list generator'''
     list_atoms = []
@@ -619,16 +620,30 @@
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
+    end = time.time()
+    print(f' {end-begin} seconds')
     return final
+from rdkit import Chem
+from rdkit.Chem import Draw
 
+from bokeh.plotting import figure, show, row
+from bokeh.models.tickers import FixedTicker
+from bokeh.layouts import row, column
+from bokeh.io import show
+from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
+from bokeh.models.widgets import DataTable, TableColumn
+
+import base64
+from io import BytesIO
+show(spectrum('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C', False, 0.01))
 #3
 def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
     mol_smi_3D = mol_smi
```

### Comparing `massivechem-5.1/test/test_SMILEs_interpreter.py` & `massivechem-5.2/test/test_SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_calculate_unsaturation.py` & `massivechem-5.2/test/test_calculate_unsaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_delta_function_plotter.py` & `massivechem-5.2/test/test_delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_double_plot.py` & `massivechem-5.2/test/test_double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_functional_group_display.py` & `massivechem-5.2/test/test_functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_functional_group_finder.py` & `massivechem-5.2/test/test_functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_ionisation_method.py` & `massivechem-5.2/test/test_ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_main_function.py` & `massivechem-5.2/test/test_main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_mol_web_show.py` & `massivechem-5.2/test/test_mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_molecule_list_generator.py` & `massivechem-5.2/test/test_molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_peak_merger.py` & `massivechem-5.2/test/test_peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_peak_sorter.py` & `massivechem-5.2/test/test_peak_sorter.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_smiles_to_3D_plot.py` & `massivechem-5.2/test/test_smiles_to_3D_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_spectrum.py` & `massivechem-5.2/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_spectrum_3D.py` & `massivechem-5.2/test/test_spectrum_3D.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_sulphur_nitrogen_adder.py` & `massivechem-5.2/test/test_sulphur_nitrogen_adder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/test/test_sulphur_nitrogen_finder.py` & `massivechem-5.2/test/test_sulphur_nitrogen_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/.gitignore` & `massivechem-5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/LICENSE.txt` & `massivechem-5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-5.1/README.md` & `massivechem-5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
+<img width="600" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
@@ -138,15 +138,15 @@
 #and the third is the resolution of the apparatus (typically, this value is of 0.01
 #the second computes an approximate spectrum if True and the precise spectrum if False
 
 ```
 
 The output of this command will be:
 
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
 
 Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
 
 <img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
 
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
```

### Comparing `massivechem-5.1/pyproject.toml` & `massivechem-5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2235 2e31 220d  version = "5.1".
+00000070: 7665 7273 696f 6e20 3d20 2235 2e32 220d  version = "5.2".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-5.1/PKG-INFO` & `massivechem-5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 5.1
+Version: 5.2
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: bokeh
 Requires-Dist: panel
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
+<img width="600" alt="logo" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Logo.jpg">
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
@@ -160,15 +160,15 @@
 #and the third is the resolution of the apparatus (typically, this value is of 0.01
 #the second computes an approximate spectrum if True and the precise spectrum if False
 
 ```
 
 The output of this command will be:
 
-<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
+<img width="600" alt="spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/blob/main/Spectrum_output.png">
 
 Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
 
 <img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
 
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
```

