# Comparing `tmp/STEAM_materials-2024.4.2.tar.gz` & `tmp/steam_materials-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEAM_materials-2024.4.2.tar", last modified: Mon Apr  8 14:29:21 2024, max compression
+gzip compressed data, was "steam_materials-2024.5.1.tar", last modified: Tue May 28 11:34:33 2024, max compression
```

## Comparing `STEAM_materials-2024.4.2.tar` & `steam_materials-2024.5.1.tar`

### file list

```diff
@@ -1,163 +1,309 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:29:21.639511 STEAM_materials-2024.4.2/
--rw-rw-rw-   0        0        0       37 2022-04-11 08:27:26.000000 STEAM_materials-2024.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      487 2024-04-08 14:29:21.635000 STEAM_materials-2024.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       68 2022-04-05 13:59:57.000000 STEAM_materials-2024.4.2/README.md
--rw-rw-rw-   0        0        0       86 2022-04-05 14:02:07.000000 STEAM_materials-2024.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 14:29:21.639511 STEAM_materials-2024.4.2/setup.cfg
--rw-rw-rw-   0        0        0      704 2024-04-08 14:28:55.000000 STEAM_materials-2024.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:29:18.614456 STEAM_materials-2024.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:29:21.635000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/
--rw-rw-rw-   0        0        0      487 2024-04-08 14:29:18.000000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7618 2024-04-08 14:29:18.000000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:29:18.000000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-08 14:29:18.000000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 14:29:18.000000 STEAM_materials-2024.4.2/src/STEAM_materials.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:29:18.646349 STEAM_materials-2024.4.2/src/steammaterials/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:29:21.635000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:03.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/BHAir_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/BHIron2_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CpHeMass_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAg_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAlAlloy_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAl_v1_deriv.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvAl_v2_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
--rw-rw-rw-   0        0        0   105984 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBeCu_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:04.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvBrass_v1_deriv.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvCu_CUDI_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvCu_NIST_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
--rw-rw-rw-   0        0        0   124416 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvCu_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvG10_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
--rw-rw-rw-   0        0        0   126464 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHast_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHeMass_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHe_CUDI_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHe_NIST_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:05.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvIn_v0.dll
--rw-rw-rw-   0        0        0   126464 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvIn_v0_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvKapton_v1_deriv.dll
--rw-rw-rw-   0        0        0   124416 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNb3Sn_Arp_Knapp_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNb3Sn_v2.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNbTi_CUDI_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvNbTi_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvSS316_NIST_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvSteel_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_CvTi_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_anisotropic_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:14.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_homogenized_v1.dll
--rw-rw-rw-   0        0        0   127488 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1.dll
--rw-rw-rw-   0        0        0   130048 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1_deriv.dll
--rw-rw-rw-   0        0        0   127488 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1.dll
--rw-rw-rw-   0        0        0   130048 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1_deriv.dll
--rw-rw-rw-   0        0        0   127488 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1.dll
--rw-rw-rw-   0        0        0   130048 2024-04-08 14:27:15.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1_deriv.dll
--rw-rw-rw-   0        0        0   129536 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
--rw-rw-rw-   0        0        0   124416 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_IcNbTi_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1_deriv.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Bordini_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bordini_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bottura_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bottura_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Summers_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Summers_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_NbTi_Bottura_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:16.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_NbTi_Bottura_v1_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_fit1_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_fit1_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_v1.dll
--rw-rw-rw-   0        0        0   126976 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_Power_Gosh_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_Power_Jiang_Wesche_v1.dll
--rw-rw-rw-   0        0        0   115712 2024-04-08 14:27:08.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_new_v1.dll
--rw-rw-rw-   0        0        0   115712 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_new_v1_deriv.dll
--rw-rw-rw-   0        0        0   115712 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_P2vsT2_cryocooler_SHI_SRDE_418D4_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_PvsT_cryocooler_SHI_SRDE_418D4_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
--rw-rw-rw-   0        0        0   126464 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_QHCircuit_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_QHCircuit_v2.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_QHCircuit_v2_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_Tcs_Nb3Sn_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:06.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_densityHe_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_fisc_I_Ic_n_rhom_Am_BSCCO2212_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:07.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_hHe_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAg_RRR30_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAg_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAg_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
--rw-rw-rw-   0        0        0   123904 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAlAlloy_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kAl_v1_deriv.dll
--rw-rw-rw-   0        0        0   105472 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kBeCu_WiedemannFranz_v1.dll
--rw-rw-rw-   0        0        0   105472 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kBeCu_WiedemannFranz_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
--rw-rw-rw-   0        0        0   105472 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1.dll
--rw-rw-rw-   0        0        0   105472 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:09.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kCu_v1.dll
--rw-rw-rw-   0        0        0   126976 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kCu_v1_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kG10_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kG10_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kHast_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:17.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kHast_v1_deriv.dll
--rw-rw-rw-   0        0        0   124416 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kHe_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kIn_v0.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kIn_v0_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kKapton_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
--rw-rw-rw-   0        0        0   126464 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kSteel_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kSteel_v2.dll
--rw-rw-rw-   0        0        0   124416 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
--rw-rw-rw-   0        0        0   112640 2024-04-08 14:27:10.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_n_T_B_BSCCO2212_Jiang_Wesche_v1.dll
--rw-rw-rw-   0        0        0   105984 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
--rw-rw-rw-   0        0        0   129024 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAg_v1_deriv.dll
--rw-rw-rw-   0        0        0   125440 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:11.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAlAlloy_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl_v1_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoAl_v2.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoBeCu_v1.dll
--rw-rw-rw-   0        0        0   105984 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoBeCu_v1_deriv.dll
--rw-rw-rw-   0        0        0   122880 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoCu_CUDI_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoCu_NIST_v1.dll
--rw-rw-rw-   0        0        0   125952 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
--rw-rw-rw-   0        0        0   129024 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoCu_v1_deriv.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
--rw-rw-rw-   0        0        0   124928 2024-04-08 14:27:18.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoHast_v1_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoHast_v2.dll
--rw-rw-rw-   0        0        0   123392 2024-04-08 14:27:12.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoIn_v0.dll
--rw-rw-rw-   0        0        0   126464 2024-04-08 14:27:19.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoIn_v0_deriv.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:13.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
--rw-rw-rw-   0        0        0   122368 2024-04-08 14:27:19.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/CFUN_rhoSS_v1_deriv.dll
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2024.4.2/src/steammaterials/CFUN/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-04-19 07:04:52.000000 STEAM_materials-2024.4.2/src/steammaterials/STEAM_materials.py
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2024.4.2/src/steammaterials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:34:33.820548 steam_materials-2024.5.1/
+-rwxrwxrwx   0 root         (0) root         (0)       74 2024-05-28 11:34:12.000000 steam_materials-2024.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-28 11:34:33.819548 steam_materials-2024.5.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       66 2024-05-28 11:34:12.000000 steam_materials-2024.5.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       84 2024-05-28 11:34:12.000000 steam_materials-2024.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:34:33.820548 steam_materials-2024.5.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      710 2024-05-28 11:34:12.000000 steam_materials-2024.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:34:33.571538 steam_materials-2024.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:34:33.819548 steam_materials-2024.5.1/src/STEAM_materials.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-28 11:34:33.000000 steam_materials-2024.5.1/src/STEAM_materials.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14844 2024-05-28 11:34:33.000000 steam_materials-2024.5.1/src/STEAM_materials.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:34:33.000000 steam_materials-2024.5.1/src/STEAM_materials.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-28 11:34:33.000000 steam_materials-2024.5.1/src/STEAM_materials.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 11:34:33.000000 steam_materials-2024.5.1/src/STEAM_materials.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:34:33.573538 steam_materials-2024.5.1/src/steammaterials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:34:33.818548 steam_materials-2024.5.1/src/steammaterials/CFUN/
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/BHAir_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/BHIron2_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CpHeMass_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAg_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAlAlloy_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAl_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvAl_v2_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBeCu_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvBrass_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvCu_CUDI_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvCu_NIST_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvCu_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvG10_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHast_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHeMass_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHe_CUDI_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHe_NIST_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvIn_v0.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvIn_v0_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvKapton_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_Arp_Knapp_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_v2.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNbTi_CUDI_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvNbTi_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvSS316_NIST_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvSteel_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_CvTi_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_anisotropic_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_homogenized_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_Fujikura_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12800 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12800 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12800 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    13824 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_IcNbTi_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Bordini_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bordini_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bottura_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Bottura_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Summers_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_Nb3Sn_Summers_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_NbTi_Bottura_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_NbTi_Bottura_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_fit1_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_fit1_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_NbTi_Cudi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_Power_Gosh_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_Power_Jiang_Wesche_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_new_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_new_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Jc_T_B_BSCCO2212_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_P2vsT2_cryocooler_SHI_SRDE_418D4_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_PvsT_cryocooler_SHI_SRDE_418D4_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_QHCircuit_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_QHCircuit_v2.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_QHCircuit_v2_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_Tcs_Nb3Sn_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_densityHe_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_fisc_I_Ic_n_rhom_Am_BSCCO2212_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_hHe_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAg_RRR30_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAg_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAg_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAlAlloy_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kAl_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kBeCu_WiedemannFranz_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kBeCu_WiedemannFranz_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kCu_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kCu_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kG10_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kG10_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kHast_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kHast_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kHe_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kIn_v0.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kIn_v0_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kKapton_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kSteel_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kSteel_v2.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_n_T_B_BSCCO2212_Jiang_Wesche_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAg_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    12288 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAlAlloy_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoAl_v2.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoBeCu_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoBeCu_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoCu_CUDI_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoCu_NIST_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11776 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoCu_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoHast_v1_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoHast_v2.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoIn_v0.dll
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoIn_v0_deriv.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
+-rw-r--r--   0 root         (0) root         (0)    10752 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/CFUN_rhoSS_v1_deriv.dll
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:34:13.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libBHAir_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libBHIron2_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CpHeMass_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAg_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAg_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAl5083_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAlAlloy_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAl_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAl_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvAl_v2_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBSCCO2212_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBSCCO2212_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBeCu_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16408 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBeCu_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBrass_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvBrass_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvCu_CUDI_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvCu_NIST_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvCu_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvCu_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvG10_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvG10_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHast_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHast_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHeMass_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHe_CUDI_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHe_NIST_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvHe_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvIn_v0.so
+-rwxr-xr-x   0 root         (0) root         (0)    16584 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvIn_v0_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvKapton_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvKapton_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16504 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNb3Sn_Arp_Knapp_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNb3Sn_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNb3Sn_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNb3Sn_v2.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNbTi_CUDI_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNbTi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvNbTi_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvSS316_NIST_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvSteel_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvSteel_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvTi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_CvTi_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16504 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_CurrentSharing_anisotropic_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16456 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_CurrentSharing_fK_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16456 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_CurrentSharing_f_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16464 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_CurrentSharing_homogenized_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16528 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_Fujikura_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16528 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_SUPERPOWER_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    20632 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_SUPERPOWER_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_THEVA_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    20624 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_THEVA_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_sunam_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    20624 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_sunam_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_HTS_JcFit_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16568 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNb3Sn_HiLumi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16568 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNb3Sn_HiLumi_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16568 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNb3Sn_WithStress_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16560 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNb3Sn_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16560 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNb3Sn_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNbTi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16528 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_IcNbTi_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_JcNbTiLowCurrent_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_JcNbTiLowCurrent_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Bordini_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Nb3Sn_Bordini_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Nb3Sn_Bottura_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16496 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Nb3Sn_Bottura_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Nb3Sn_Summers_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16528 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_Nb3Sn_Summers_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_NbTi_Bottura_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16496 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_NbTi_Bottura_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_NbTi_Cudi_fit1_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16456 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_NbTi_Cudi_fit1_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_NbTi_Cudi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16536 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_T_B_BSCCO2212_Power_Gosh_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16504 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_T_B_BSCCO2212_Power_Jiang_Wesche_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_T_B_BSCCO2212_new_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16496 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_T_B_BSCCO2212_new_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Jc_T_B_BSCCO2212_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16592 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_P2vsT2_cryocooler_SHI_SRDE_418D4_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16528 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_PvsT_cryocooler_SHI_SRDE_418D4_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_QHCircuit_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16568 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_QHCircuit_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_QHCircuit_v2.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_QHCircuit_v2_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_TcsNbTi_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_Tcs_Nb3Sn_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_densityHe_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16464 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_fisc_I_Ic_n_rhom_Am_BSCCO2212_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_hHe_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAg_RRR30_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAg_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAg_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAl1350_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAl5083_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAl6061_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAlAlloy_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kAl_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16416 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kBeCu_WiedemannFranz_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16424 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kBeCu_WiedemannFranz_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kBrass_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16408 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kCu_Wiedemann_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16416 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kCu_Wiedemann_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kCu_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kCu_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16472 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kG10_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kG10_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kHast_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kHast_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kHe_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kIn_v0.so
+-rwxr-xr-x   0 root         (0) root         (0)    16552 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kIn_v0_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kKapton_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kKapton_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kSteel_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16552 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kSteel_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kSteel_v2.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_kStycast_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16464 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_n_T_B_BSCCO2212_Jiang_Wesche_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16408 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_quenchState_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAgMg_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAg_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAg_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl1350_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl5083_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl6061_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAlAlloy_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoAl_v2.so
+-rwxr-xr-x   0 root         (0) root         (0)    16408 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoBeCu_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16408 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoBeCu_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoCu_CUDI_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoCu_NIST_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16512 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoCu_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16520 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoCu_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoHast_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16488 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoHast_v1_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoHast_v2.so
+-rwxr-xr-x   0 root         (0) root         (0)    16480 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoIn_v0.so
+-rwxr-xr-x   0 root         (0) root         (0)    16552 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoIn_v0_deriv.so
+-rwxr-xr-x   0 root         (0) root         (0)    16440 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoSS_v1.so
+-rwxr-xr-x   0 root         (0) root         (0)    16448 2024-05-28 11:34:28.000000 steam_materials-2024.5.1/src/steammaterials/CFUN/libCFUN_rhoSS_v1_deriv.so
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-28 11:34:12.000000 steam_materials-2024.5.1/src/steammaterials/STEAM_materials.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:34:13.000000 steam_materials-2024.5.1/src/steammaterials/__init__.py
```

### Comparing `STEAM_materials-2024.4.2/setup.py` & `steam_materials-2024.5.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="STEAM_materials",
-    version="2024.04.2",
-    author="STEAM Team",
-    author_email="steam-team@cern.ch",
-    description="Python wrapper for the steam materials package.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://gitlab.cern.ch/steam/steam-material-library",
-    keywords={'STEAM', 'API', 'MATERIALS', 'CERN'},
-    install_requires=['numpy'],
-    python_requires='>=3.8',
-    include_package_data=True,
-    classifiers=[
-        "Programming Language :: Python :: 3.8"
-        ],
-)
+import setuptools
+import os
+
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="STEAM_materials",
+    version=os.environ['RELEASE_NAME'],
+    author="STEAM Team",
+    author_email="steam-team@cern.ch",
+    description="Python wrapper for the steam materials package.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://gitlab.cern.ch/steam/steam-material-library",
+    keywords=['STEAM', 'API', 'MATERIALS', 'CERN'],
+    install_requires=['numpy'],
+    python_requires='>=3.8',
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python :: 3.8"
+        ],
+)
```

### Comparing `STEAM_materials-2024.4.2/src/steammaterials/STEAM_materials.py` & `steam_materials-2024.5.1/src/steammaterials/STEAM_materials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import ctypes as ct
 import os
+import platform
 import numpy as np
+from pathlib import Path
 from numpy.ctypeslib import ndpointer
+#import matlab.engine
+
 
 class STEAM_materials:
 
-    def __init__(self, func_name, n_arg, n_points, C_FUN_folder=None):
+    def __init__(self, func_name, n_arg, n_points, material_objects_path: os.PathLike=None):
         """
-
         :param func_name: string with function name corresponding to dll file name (without the .dll in the string)
         :param n_arg:	number of arguments of the func_name function. This corresponds to number of columns in 2D numpy array, numpy2d, to be used in the method. Use numpy2d.shape[1] to get the number.
         :param n_points: number of points to evaluate. This corresponds to number of rows in 2D numpy array, numpy2d, to be used in the eval method. Use numpy2d.shape[0] to get the number.
-        :param C_FUN_folder: If not specified, the code assumes the .dll files are in a folder called CFUN in the same directory as this script. Otherwise a full path to a folder needs to be given.
+        :param material_objects_path: If not specified, the code assumes the .dll files are in a folder called CFUN in the same directory as this script. Otherwise a full path to a folder needs to be given.
         """
-        if C_FUN_folder:
-            self.C_FUN_folder = C_FUN_folder  # allows user to specify full path to folder with .dlls
+        if material_objects_path is not None:
+            dll_path: Path = Path(material_objects_path)  # allows user to specify full path to folder with .dlls
+        else:
+            dll_path: Path = Path(__file__).parent / 'CFUN'  # Assumes .dlls are in a folder called CFUN in the same directory as this script
+
+        if platform.system() == 'Windows':
+            self._dll_name = f'{func_name}.dll'
+        elif platform.system() == 'Linux':
+            self._dll_name = f'lib{func_name}.so'
         else:
-            self.C_FUN_folder = os.path.join(os.getcwd(), "CFUN")  # Assumes .dlls are in a folder called CFUN in the same directory as this script
-        _dll = ct.CDLL(os.path.join(self.C_FUN_folder + os.sep + 'CFUN', f'{func_name}.dll'))
+            raise NotImplementedError(f'Platform "{platform.system()}" is not supported!')
+
+        _dll = ct.CDLL(dll_path / self._dll_name)
         self.func_name = func_name.encode('ascii')
         self.n_points = n_points
         self.n_arg = n_arg
         array_type = ct.c_double * self.n_points
         self.RealPtr = array_type()
         self.Int_Ptr = array_type()
         _doublepp = ndpointer(dtype=np.uintp, ndim=1, flags='C')
@@ -42,10 +53,44 @@
         :return: Numpy array with values calculated by .dll function
         """
         inReal = (numpy2d.__array_interface__['data'][0] + np.arange(numpy2d.shape[0]) * numpy2d.strides[0]).astype(np.uintp)
         error_out = self.eval(self.func_name, self.n_arg, inReal, inReal, self.n_points, self.RealPtr, self.Int_Ptr)
         if error_out == 1:
             pass
         else:
-            raise ValueError(f"There was a problem with calling {self.func_name}.dll with arguments {numpy2d}. Check if dll file exists or if number of arguments is correct.")
+            raise ValueError(f"There was a problem with calling {self._dll_name} with arguments {numpy2d}. Check if library file exists or if number of arguments is correct.")
         return np.array(self.RealPtr)
 
+class STEAM_materials_Matlab:
+    def __init__(self,func_name:str,arg_list:str):
+        self.arguments=arg_list
+        self.func=func_name
+
+
+    def evaluate(self):
+        eng = matlab.engine.start_matlab()
+        result=eng.eval(self.func+self.arguments)
+        print(result)
+
+if __name__ == "__main__":
+   # STEAM_materials_Matlab("rhoCu_nist","(1.8,1,120.0,5)").evaluate()
+
+
+
+    func_4d = 'CFUN_rhoCuNIST'  # function name, this one takes 4 arguments as input and returns a single float for resistivity
+    T_min = 1.8
+    T_max = 300
+    B = 1.
+    RRR = 120.0
+    T_ref_RRR = 273.
+    num_elem = 1000
+    T = np.linspace(T_min, T_max, num_elem)
+
+    # make numpy array
+    numpy2d = np.vstack((T, np.ones(num_elem) * B, np.ones(num_elem) * RRR, np.ones(num_elem) * T_ref_RRR))
+
+    # make dll func object
+    sm = STEAM_materials(func_4d, numpy2d.shape[0], numpy2d.shape[1], r'G:\Projects\lhccm\STEAM\MaterialsLibrary\V0.1')
+
+    # call with 2D numpy array and get results back
+    result_numpy = sm.evaluate(numpy2d)
+    print(result_numpy)
```

