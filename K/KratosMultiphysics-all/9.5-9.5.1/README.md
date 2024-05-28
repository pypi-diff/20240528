# Comparing `tmp/KratosMultiphysics_all-9.5-py3-none-any.whl.zip` & `tmp/KratosMultiphysics_all-9.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 5232 bytes, number of entries: 4
--rw-r--r--  2.0 unx    12835 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      351 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/RECORD
-4 files, 13297 bytes uncompressed, 4546 bytes compressed:  65.8%
+Zip file size: 5359 bytes, number of entries: 4
+-rw-r--r--  2.0 unx    13153 b- defN 24-May-27 10:17 KratosMultiphysics_all-9.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 10:17 KratosMultiphysics_all-9.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-27 10:17 KratosMultiphysics_all-9.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      359 b- defN 24-May-27 10:17 KratosMultiphysics_all-9.5.1.dist-info/RECORD
+4 files, 13623 bytes uncompressed, 4657 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: KratosMultiphysics_all-9.5.dist-info/METADATA
+Filename: KratosMultiphysics_all-9.5.1.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics_all-9.5.dist-info/WHEEL
+Filename: KratosMultiphysics_all-9.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics_all-9.5.dist-info/top_level.txt
+Filename: KratosMultiphysics_all-9.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics_all-9.5.dist-info/RECORD
+Filename: KratosMultiphysics_all-9.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `KratosMultiphysics_all-9.5.dist-info/METADATA` & `KratosMultiphysics_all-9.5.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
 Name: KratosMultiphysics-all
-Version: 9.5
+Version: 9.5.1
 Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
 Home-page: https://github.com/KratosMultiphysics/
 Author: Kratos Team
 Author-email: kratos@listas.cimne.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: KratosMultiphysics ==9.5
-Requires-Dist: KratosContactStructuralMechanicsApplication ==9.5
-Requires-Dist: KratosConvectionDiffusionApplication ==9.5
-Requires-Dist: KratosConstitutiveLawsApplication ==9.5
-Requires-Dist: KratosCoSimulationApplication ==9.5
-Requires-Dist: KratosDEMApplication ==9.5
-Requires-Dist: KratosDamApplication ==9.5
-Requires-Dist: KratosFluidDynamicsApplication ==9.5
-Requires-Dist: KratosFSIApplication ==9.5
-Requires-Dist: KratosLinearSolversApplication ==9.5
-Requires-Dist: KratosMappingApplication ==9.5
-Requires-Dist: KratosMeshingApplication ==9.5
-Requires-Dist: KratosMPMApplication ==9.5
-Requires-Dist: KratosPoroMechanicsApplication ==9.5
-Requires-Dist: KratosShallowWaterApplication ==9.5
-Requires-Dist: KratosStructuralMechanicsApplication ==9.5
-Requires-Dist: KratosGeoMechanicsApplication ==9.5
+Requires-Dist: KratosMultiphysics ==9.5.1
+Requires-Dist: KratosContactStructuralMechanicsApplication ==9.5.1
+Requires-Dist: KratosConvectionDiffusionApplication ==9.5.1
+Requires-Dist: KratosConstitutiveLawsApplication ==9.5.1
+Requires-Dist: KratosCoSimulationApplication ==9.5.1
+Requires-Dist: KratosDEMApplication ==9.5.1
+Requires-Dist: KratosDamApplication ==9.5.1
+Requires-Dist: KratosFluidDynamicsApplication ==9.5.1
+Requires-Dist: KratosFSIApplication ==9.5.1
+Requires-Dist: KratosLinearSolversApplication ==9.5.1
+Requires-Dist: KratosMappingApplication ==9.5.1
+Requires-Dist: KratosMeshingApplication ==9.5.1
+Requires-Dist: KratosMPMApplication ==9.5.1
+Requires-Dist: KratosPoroMechanicsApplication ==9.5.1
+Requires-Dist: KratosShallowWaterApplication ==9.5.1
+Requires-Dist: KratosStructuralMechanicsApplication ==9.5.1
+Requires-Dist: KratosGeoMechanicsApplication ==9.5.1
 
 <p align=center><img height="72.125%" width="72.125%" src="https://raw.githubusercontent.com/KratosMultiphysics/Documentation/master/Wiki_files/Home/kratos.png"></p>
 
 [![License][license-image]][license] [![C++][c++-image]][c++standard] [![Github CI][Nightly-Build]][Nightly-link] [![DOI][DOI-image]][DOI] [![GitHub stars][stars-image]][stars] [![Twitter][twitter-image]][twitter] [![Youtube][youtube-image]][youtube]
 
 [![Release][release-image]][releases]
 <a href="https://github.com/KratosMultiphysics/Kratos/releases/latest"><img src="https://img.shields.io/github/release-date/KratosMultiphysics/Kratos?label="></a>
-<a href="https://github.com/KratosMultiphysics/Kratos/compare/Release-8.1...master"><img src="https://img.shields.io/github/commits-since/KratosMultiphysics/Kratos/latest?label=commits%20since"></a>
+<a href="https://github.com/KratosMultiphysics/Kratos/compare/Release-9.5...master"><img src="https://img.shields.io/github/commits-since/KratosMultiphysics/Kratos/latest?label=commits%20since"></a>
 <a href="https://github.com/KratosMultiphysics/Kratos/commit/master"><img src="https://img.shields.io/github/last-commit/KratosMultiphysics/Kratos?label=latest%20commit"></a>
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/KratosMultiphysics.svg)](https://pypi.org/project/KratosMultiphysics/)
 [![Downloads](https://pepy.tech/badge/KratosMultiphysics/month)](https://pepy.tech/project/KratosMultiphysics)
 
-[release-image]: https://img.shields.io/badge/release-9.4-green.svg?style=flat
+[release-image]: https://img.shields.io/badge/release-9.5-green.svg?style=flat
 [releases]: https://github.com/KratosMultiphysics/Kratos/releases
 
 [license-image]: https://img.shields.io/badge/license-BSD-green.svg?style=flat
 [license]: https://github.com/KratosMultiphysics/Kratos/blob/master/kratos/license.txt
 
 [c++-image]: https://img.shields.io/badge/C++-17-blue.svg?style=flat&logo=c%2B%2B
 [c++standard]: https://isocpp.org/std/the-standard
@@ -197,10 +198,10 @@
 - [CoSimIO](https://github.com/KratosMultiphysics/CoSimIO) for performing coupled simulations with external solvers within the [CoSimulationApplication](applications/CoSimulationApplication/README.md). The CoSimIO in Kratos uses the following libraries:
   - [Boost](http://www.boost.org/) for the `intrusive_ptr`
   - [filesystem](https://github.com/gulrak/filesystem) Header-only single-file std::filesystem compatible helper library, based on the C++17 specs
   - [asio](https://think-async.com/Asio/) for socket based interprocess communication
 
 # How to cite Kratos?
 Please, use the following references when citing Kratos in your work.
-- Dadvand, P., Rossi, R. & Oñate, E. An Object-oriented Environment for Developing Finite Element Codes for Multi-disciplinary Applications. Arch Computat Methods Eng 17, 253–297 (2010). https://doi.org/10.1007/s11831-010-9045-2
-- Dadvand, P., Rossi, R., Gil, M., Martorell, X., Cotela, J., Juanpere, E., Idelsohn, S., Oñate, E. (2013). Migration of a generic multi-physics framework to HPC environments. Computers & Fluids. 80. 301–309. 10.1016/j.compfluid.2012.02.004.
-- Vicente Mataix Ferrándiz, Philipp Bucher, Rubén Zorrilla, Riccardo Rossi, Jordi Cotela, Alejandro Cornejo Velázquez, Miguel Angel Celigueta, Josep Maria, Tobias Teschemacher, Carlos Roig, Miguel Maso, Guillermo Casas, Suneth Warnakulasuriya, Marc Núñez, Pooyan Dadvand, Salva Latorre, Ignasi de Pouplana, Joaquín Irazábal González, Ferran Arrufat, … Javi Gárate. (2022). KratosMultiphysics/Kratos: Release 9.2 (v9.2). Zenodo. https://doi.org/10.5281/zenodo.3234644
+- [Dadvand, P., Rossi, R. & Oñate, E. An Object-oriented Environment for Developing Finite Element Codes for Multi-disciplinary Applications. Arch Computat Methods Eng 17, 253–297 (2010). https://doi.org/10.1007/s11831-010-9045-2](https://doi.org/10.1007/s11831-010-9045-2)
+- [Dadvand, P., Rossi, R., Gil, M., Martorell, X., Cotela, J., Juanpere, E., Idelsohn, S., Oñate, E. (2013). Migration of a generic multi-physics framework to HPC environments. Computers & Fluids. 80. 301–309. 10.1016/j.compfluid.2012.02.004.](10.1016/j.compfluid.2012.02.004)
+- [Vicente Mataix Ferrándiz, Philipp Bucher, Rubén Zorrilla, Suneth Warnakulasuriya, Riccardo Rossi, Alejandro Cornejo, jcotela, Carlos Roig, Josep Maria, tteschemacher, Miguel Masó, Guillermo Casas, Marc Núñez, Pooyan Dadvand, Salva Latorre, Ignasi de Pouplana, Joaquín Irazábal González, AFranci, Ferran Arrufat, riccardotosi, Aditya Ghantasala, Klaus Bernd Sautter, Peter Wilson, dbaumgaertner, Bodhinanda Chandra, Armin Geiser, Inigo Lopez, lluís, jgonzalezusua, Javi Gárate. (2024). KratosMultiphysics/Kratos: Release 9.5 (v9.5). Zenodo. https://doi.org/10.5281/zenodo.3234644](https://zenodo.org/records/6926179)
```

### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: KratosMultiphysics-all Version: 9.5 Summary: KRATOS
-Multiphysics ("Kratos") is a framework for building parallel, multi-
+Metadata-Version: 2.1 Name: KratosMultiphysics-all Version: 9.5.1 Summary:
+KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-
 disciplinary simulation software, aiming at modularity, extensibility, and high
 performance. Kratos is written in C++, and counts with an extensive Python
 interface. Home-page: https://github.com/KratosMultiphysics/ Author: Kratos
 Team Author-email: kratos@listas.cimne.upc.edu Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Physics Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: License :: OSI Approved :: BSD License Classifier:
-Natural Language :: English Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Other Audience Classifier: Intended Audience
-:: Developers Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console Requires-Python: >=3.8 Description-Content-
-Type: text/markdown Requires-Dist: KratosMultiphysics ==9.5 Requires-Dist:
-KratosContactStructuralMechanicsApplication ==9.5 Requires-Dist:
-KratosConvectionDiffusionApplication ==9.5 Requires-Dist:
-KratosConstitutiveLawsApplication ==9.5 Requires-Dist:
-KratosCoSimulationApplication ==9.5 Requires-Dist: KratosDEMApplication ==9.5
-Requires-Dist: KratosDamApplication ==9.5 Requires-Dist:
-KratosFluidDynamicsApplication ==9.5 Requires-Dist: KratosFSIApplication ==9.5
-Requires-Dist: KratosLinearSolversApplication ==9.5 Requires-Dist:
-KratosMappingApplication ==9.5 Requires-Dist: KratosMeshingApplication ==9.5
-Requires-Dist: KratosMPMApplication ==9.5 Requires-Dist:
-KratosPoroMechanicsApplication ==9.5 Requires-Dist:
-KratosShallowWaterApplication ==9.5 Requires-Dist:
-KratosStructuralMechanicsApplication ==9.5 Requires-Dist:
-KratosGeoMechanicsApplication ==9.5
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: License
+:: OSI Approved :: BSD License Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Other Audience Classifier: Intended Audience :: Developers Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Console
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist:
+KratosMultiphysics ==9.5.1 Requires-Dist:
+KratosContactStructuralMechanicsApplication ==9.5.1 Requires-Dist:
+KratosConvectionDiffusionApplication ==9.5.1 Requires-Dist:
+KratosConstitutiveLawsApplication ==9.5.1 Requires-Dist:
+KratosCoSimulationApplication ==9.5.1 Requires-Dist: KratosDEMApplication
+==9.5.1 Requires-Dist: KratosDamApplication ==9.5.1 Requires-Dist:
+KratosFluidDynamicsApplication ==9.5.1 Requires-Dist: KratosFSIApplication
+==9.5.1 Requires-Dist: KratosLinearSolversApplication ==9.5.1 Requires-Dist:
+KratosMappingApplication ==9.5.1 Requires-Dist: KratosMeshingApplication
+==9.5.1 Requires-Dist: KratosMPMApplication ==9.5.1 Requires-Dist:
+KratosPoroMechanicsApplication ==9.5.1 Requires-Dist:
+KratosShallowWaterApplication ==9.5.1 Requires-Dist:
+KratosStructuralMechanicsApplication ==9.5.1 Requires-Dist:
+KratosGeoMechanicsApplication ==9.5.1
   [https://raw.githubusercontent.com/KratosMultiphysics/Documentation/master/
                           Wiki_files/Home/kratos.png]
 [![License][license-image]][license] [![C++][c++-image]][c++standard] [![Github
 CI][Nightly-Build]][Nightly-link] [![DOI][DOI-image]][DOI] [![GitHub stars]
 [stars-image]][stars] [![Twitter][twitter-image]][twitter] [![Youtube][youtube-
 image]][youtube] [![Release][release-image]][releases] _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _g_i_t_h_u_b_/_r_e_l_e_a_s_e_-_d_a_t_e_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_?_l_a_b_e_l_=_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _g_i_t_h_u_b_/_c_o_m_m_i_t_s_-_s_i_n_c_e_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_/_l_a_t_e_s_t_?_l_a_b_e_l_=_c_o_m_m_i_t_s_%_2_0_s_i_n_c_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/
 _K_r_a_t_o_s_?_l_a_b_e_l_=_l_a_t_e_s_t_%_2_0_c_o_m_m_i_t_][![PyPI pyversions](https://img.shields.io/pypi/
 pyversions/KratosMultiphysics.svg)](https://pypi.org/project/
 KratosMultiphysics/) [![Downloads](https://pepy.tech/badge/KratosMultiphysics/
 month)](https://pepy.tech/project/KratosMultiphysics) [release-image]: https://
-img.shields.io/badge/release-9.4-green.svg?style=flat [releases]: https://
+img.shields.io/badge/release-9.5-green.svg?style=flat [releases]: https://
 github.com/KratosMultiphysics/Kratos/releases [license-image]: https://
 img.shields.io/badge/license-BSD-green.svg?style=flat [license]: https://
 github.com/KratosMultiphysics/Kratos/blob/master/kratos/license.txt [c++-
 image]: https://img.shields.io/badge/C++-17-blue.svg?style=flat&logo=c%2B%2B
 [c++standard]: https://isocpp.org/std/the-standard [Nightly-Build]: https://
 github.com/KratosMultiphysics/Kratos/workflows/Nightly%20Build/badge.svg
 [Nightly-link]: https://github.com/KratosMultiphysics/Kratos/
@@ -153,20 +154,24 @@
 solvers within the [CoSimulationApplication](applications/
 CoSimulationApplication/README.md). The CoSimIO in Kratos uses the following
 libraries: - [Boost](http://www.boost.org/) for the `intrusive_ptr` -
 [filesystem](https://github.com/gulrak/filesystem) Header-only single-file
 std::filesystem compatible helper library, based on the C++17 specs - [asio]
 (https://think-async.com/Asio/) for socket based interprocess communication #
 How to cite Kratos? Please, use the following references when citing Kratos in
-your work. - Dadvand, P., Rossi, R. & OÃ±ate, E. An Object-oriented Environment
-for Developing Finite Element Codes for Multi-disciplinary Applications. Arch
-Computat Methods Eng 17, 253â297 (2010). https://doi.org/10.1007/s11831-010-
-9045-2 - Dadvand, P., Rossi, R., Gil, M., Martorell, X., Cotela, J., Juanpere,
-E., Idelsohn, S., OÃ±ate, E. (2013). Migration of a generic multi-physics
-framework to HPC environments. Computers & Fluids. 80. 301â309. 10.1016/
-j.compfluid.2012.02.004. - Vicente Mataix FerrÃ¡ndiz, Philipp Bucher, RubÃ©n
-Zorrilla, Riccardo Rossi, Jordi Cotela, Alejandro Cornejo VelÃ¡zquez, Miguel
-Angel Celigueta, Josep Maria, Tobias Teschemacher, Carlos Roig, Miguel Maso,
-Guillermo Casas, Suneth Warnakulasuriya, Marc NÃºÃ±ez, Pooyan Dadvand, Salva
-Latorre, Ignasi de Pouplana, JoaquÃ­n IrazÃ¡bal GonzÃ¡lez, Ferran Arrufat, â¦
-Javi GÃ¡rate. (2022). KratosMultiphysics/Kratos: Release 9.2 (v9.2). Zenodo.
-https://doi.org/10.5281/zenodo.3234644
+your work. - [Dadvand, P., Rossi, R. & OÃ±ate, E. An Object-oriented
+Environment for Developing Finite Element Codes for Multi-disciplinary
+Applications. Arch Computat Methods Eng 17, 253â297 (2010). https://doi.org/
+10.1007/s11831-010-9045-2](https://doi.org/10.1007/s11831-010-9045-2) -
+[Dadvand, P., Rossi, R., Gil, M., Martorell, X., Cotela, J., Juanpere, E.,
+Idelsohn, S., OÃ±ate, E. (2013). Migration of a generic multi-physics framework
+to HPC environments. Computers & Fluids. 80. 301â309. 10.1016/
+j.compfluid.2012.02.004.](10.1016/j.compfluid.2012.02.004) - [Vicente Mataix
+FerrÃ¡ndiz, Philipp Bucher, RubÃ©n Zorrilla, Suneth Warnakulasuriya, Riccardo
+Rossi, Alejandro Cornejo, jcotela, Carlos Roig, Josep Maria, tteschemacher,
+Miguel MasÃ³, Guillermo Casas, Marc NÃºÃ±ez, Pooyan Dadvand, Salva Latorre,
+Ignasi de Pouplana, JoaquÃ­n IrazÃ¡bal GonzÃ¡lez, AFranci, Ferran Arrufat,
+riccardotosi, Aditya Ghantasala, Klaus Bernd Sautter, Peter Wilson,
+dbaumgaertner, Bodhinanda Chandra, Armin Geiser, Inigo Lopez, lluÃ­s,
+jgonzalezusua, Javi GÃ¡rate. (2024). KratosMultiphysics/Kratos: Release 9.5
+(v9.5). Zenodo. https://doi.org/10.5281/zenodo.3234644](https://zenodo.org/
+records/6926179)
```

