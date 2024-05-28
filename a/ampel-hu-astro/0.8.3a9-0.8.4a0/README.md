# Comparing `tmp/ampel_hu_astro-0.8.3a9.tar.gz` & `tmp/ampel_hu_astro-0.8.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_hu_astro-0.8.3a9.tar", max compression
+gzip compressed data, was "ampel_hu_astro-0.8.4a0.tar", max compression
```

## Comparing `ampel_hu_astro-0.8.3a9.tar` & `ampel_hu_astro-0.8.4a0.tar`

### file list

```diff
@@ -1,114 +1,129 @@
--rw-r--r--   0        0        0     1512 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/LICENSE
--rw-r--r--   0        0        0     1607 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/README.md
--rw-r--r--   0        0        0     1970 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/channel_notes.txt
--rw-r--r--   0        0        0        0 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/py.typed
--rwxr-xr-x   0        0        0      981 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/LensedTransientFilter.py
--rw-r--r--   0        0        0      689 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RandFilter.py
--rwxr-xr-x   0        0        0    15870 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RcfFilter.py
--rw-r--r--   0        0        0     5605 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
--rwxr-xr-x   0        0        0    10665 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/SimpleDecentFilter.py
--rwxr-xr-x   0        0        0     3283 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/TransientInClusterFilter.py
--rwxr-xr-x   0        0        0     4861 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/XShooterFilter.py
--rwxr-xr-x   0        0        0     4807 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2BrightSNProb.py
--rwxr-xr-x   0        0        0    11373 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
--rw-r--r--   0        0        0    17341 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2DigestRedshifts.py
--rw-r--r--   0        0        0    10753 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
--rw-r--r--   0        0        0    19846 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2ElasticcReport.py
--rwxr-xr-x   0        0        0     2383 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2FastDecliner.py
--rw-r--r--   0        0        0     7460 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2GetLensSNParameters.py
--rw-r--r--   0        0        0    14954 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2InfantCatalogEval.py
--rwxr-xr-x   0        0        0    10196 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2LCQuality.py
--rw-r--r--   0        0        0    10115 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2LSPhotoZTap.py
--rw-r--r--   0        0        0     3608 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2MatchBTS.py
--rwxr-xr-x   0        0        0     4139 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
--rw-r--r--   0        0        0     8377 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
--rwxr-xr-x   0        0        0     5210 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2NedSNCosmo.py
--rwxr-xr-x   0        0        0     6042 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2NedTap.py
--rwxr-xr-x   0        0        0     4222 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2Observability.py
--rwxr-xr-x   0        0        0     2957 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
--rwxr-xr-x   0        0        0     4527 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
--rwxr-xr-x   0        0        0     3689 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
--rwxr-xr-x   0        0        0     2167 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
--rw-r--r--   0        0        0     7678 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PhaseLimit.py
--rw-r--r--   0        0        0     2067 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PropagateStockInfo.py
--rwxr-xr-x   0        0        0    15973 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RiseDeclineStat.py
--rw-r--r--   0        0        0    19499 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunParsnip.py
--rw-r--r--   0        0        0     6836 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunPossis.py
--rw-r--r--   0        0        0    18061 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunSncosmo.py
--rw-r--r--   0        0        0    10840 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunSnoopy.py
--rw-r--r--   0        0        0     7924 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunTDE.py
--rw-r--r--   0        0        0      257 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2SNCosmo.py
--rw-r--r--   0        0        0    20750 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2TNSEval.py
--rw-r--r--   0        0        0    18329 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
--rw-r--r--   0        0        0     9210 2022-12-19 14:44:43.305760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2XgbClassifier.py
--rw-r--r--   0        0        0   139314 2022-12-19 14:44:43.309760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
--rw-r--r--   0        0        0    91172 2022-12-19 14:44:43.309760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
--rw-r--r--   0        0        0    71112 2022-12-19 14:44:43.309760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
--rw-r--r--   0        0        0  4758373 2022-12-19 14:44:43.321760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/xgb_trees.py
--rw-r--r--   0        0        0     3094 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/AstroColibriClient.py
--rw-r--r--   0        0        0     9577 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/AstroColibriPublisher.py
--rwxr-xr-x   0        0        0     5618 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
--rwxr-xr-x   0        0        0    13423 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/DCachePublisher.py
--rw-r--r--   0        0        0     8718 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ElasticcClassPublisher.py
--rw-r--r--   0        0        0     3308 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ElasticcTomClient.py
--rw-r--r--   0        0        0     7903 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/HealpixCorrPlotter.py
--rw-r--r--   0        0        0    11743 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/PlotLightcurveSample.py
--rwxr-xr-x   0        0        0     5306 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidBase.py
--rwxr-xr-x   0        0        0    12541 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidLco.py
--rwxr-xr-x   0        0        0     3949 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidSedm.py
--rwxr-xr-x   0        0        0    12021 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/SlackSummaryPublisher.py
--rwxr-xr-x   0        0        0     1936 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TNSMirrorUpdater.py
--rwxr-xr-x   0        0        0    21403 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TNSTalker.py
--rwxr-xr-x   0        0        0     2482 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TransientInfoPrinter.py
--rw-r--r--   0        0        0     8188 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TransientTablePublisher.py
--rwxr-xr-x   0        0        0     3952 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TransientViewDumper.py
--rw-r--r--   0        0        0     5380 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/VOEventPublisher.py
--rwxr-xr-x   0        0        0    12955 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ampel_tns.py
--rwxr-xr-x   0        0        0     2326 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
--rwxr-xr-x   0        0        0     4898 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSClient.py
--rw-r--r--   0        0        0     4103 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
--rwxr-xr-x   0        0        0     1725 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSName.py
--rw-r--r--   0        0        0      129 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSToken.py
--rw-r--r--   0        0        0      100 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/__init__.py
--rw-r--r--   0        0        0    20855 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
--rw-r--r--   0        0        0      397 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_config.py
--rw-r--r--   0        0        0     4678 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_slackpublisher.py
--rw-r--r--   0        0        0     3321 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_t2brightsnprob.py
--rw-r--r--   0        0        0     1354 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_tns.py
--rw-r--r--   0        0        0     1837 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_tnstalker.py
--rw-r--r--   0        0        0      975 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/util/ned.py
--rw-r--r--   0        0        0      108 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/ampel/contrib/hu/utils.py
--rw-r--r--   0        0        0     5328 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/alias.yml
--rw-r--r--   0        0        0      907 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_10.yml
--rw-r--r--   0        0        0      647 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_16.yml
--rw-r--r--   0        0        0      957 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_59.yml
--rw-r--r--   0        0        0      725 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml
--rw-r--r--   0        0        0      816 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml
--rw-r--r--   0        0        0      952 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml
--rw-r--r--   0        0        0      973 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml
--rw-r--r--   0        0        0      181 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RANDOM.yml
--rw-r--r--   0        0        0      229 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID.yml
--rw-r--r--   0        0        0      787 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
--rw-r--r--   0        0        0      982 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml
--rw-r--r--   0        0        0      679 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml
--rw-r--r--   0        0        0      280 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_SOUTH.yml
--rw-r--r--   0        0        0      280 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_UL.yml
--rw-r--r--   0        0        0      960 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml
--rw-r--r--   0        0        0      954 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml
--rw-r--r--   0        0        0      794 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/AmpelAutoLco.yml
--rw-r--r--   0        0        0      992 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/ChannelSummary.yml
--rw-r--r--   0        0        0      481 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/ClusterSummary.yml
--rw-r--r--   0        0        0     1369 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/CosmologySummary.yaml
--rw-r--r--   0        0        0      456 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/DesiSkyportal.yml
--rw-r--r--   0        0        0      585 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml
--rw-r--r--   0        0        0      568 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml
--rw-r--r--   0        0        0      431 2022-12-19 14:44:43.325760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/LensingSummary.yml
--rw-r--r--   0        0        0      371 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/RapidAllz.yml
--rw-r--r--   0        0        0      645 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/RapidReact.yml
--rw-r--r--   0        0        0      451 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/TNSSubmitComplete.yml
--rw-r--r--   0        0        0      573 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/TNSSubmitNew.yml
--rw-r--r--   0        0        0      205 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
--rw-r--r--   0        0        0     1944 2022-12-19 14:44:43.329760 ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/unit.yml
--rw-r--r--   0        0        0     3410 2022-12-19 14:44:43.333760 ampel_hu_astro-0.8.3a9/pyproject.toml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.3a9/setup.py
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.3a9/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/LICENSE
+-rw-r--r--   0        0        0     1794 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/README.md
+-rw-r--r--   0        0        0     3122 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py
+-rw-r--r--   0        0        0     8895 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py
+-rw-r--r--   0        0        0     3592 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/ResourceDependentConsumer.py
+-rwxr-xr-x   0        0        0     1461 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py
+-rw-r--r--   0        0        0     1970 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/channel_notes.txt
+-rwxr-xr-x   0        0        0     2185 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py
+-rw-r--r--   0        0        0        0 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/py.typed
+-rwxr-xr-x   0        0        0      981 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/LensedTransientFilter.py
+-rw-r--r--   0        0        0     2066 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/PredetectionFilter.py
+-rw-r--r--   0        0        0      732 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RandFilter.py
+-rwxr-xr-x   0        0        0    15789 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RcfFilter.py
+-rw-r--r--   0        0        0     6142 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
+-rwxr-xr-x   0        0        0    10713 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/SimpleDecentFilter.py
+-rwxr-xr-x   0        0        0     3844 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/TransientInClusterFilter.py
+-rwxr-xr-x   0        0        0     4843 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/XShooterFilter.py
+-rw-r--r--   0        0        0    59244 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BayesianBlocks.py
+-rwxr-xr-x   0        0        0     4932 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BrightSNProb.py
+-rwxr-xr-x   0        0        0    11158 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
+-rw-r--r--   0        0        0    17872 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DigestRedshifts.py
+-rw-r--r--   0        0        0    33136 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DustEchoEval.py
+-rw-r--r--   0        0        0    11549 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
+-rw-r--r--   0        0        0    24754 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcReport.py
+-rwxr-xr-x   0        0        0     2378 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2FastDecliner.py
+-rw-r--r--   0        0        0     8706 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2GetLensSNParameters.py
+-rwxr-xr-x   0        0        0     5369 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2HealpixProb.py
+-rw-r--r--   0        0        0    15055 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2InfantCatalogEval.py
+-rw-r--r--   0        0        0    35526 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2KilonovaEval.py
+-rwxr-xr-x   0        0        0    10191 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LCQuality.py
+-rw-r--r--   0        0        0    10357 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LSPhotoZTap.py
+-rw-r--r--   0        0        0     2250 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LoadRedshift.py
+-rw-r--r--   0        0        0     3633 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchBTS.py
+-rw-r--r--   0        0        0     5353 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchGRB.py
+-rwxr-xr-x   0        0        0     5240 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
+-rw-r--r--   0        0        0     9680 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
+-rwxr-xr-x   0        0        0     6607 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedSNCosmo.py
+-rwxr-xr-x   0        0        0     7132 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedTap.py
+-rwxr-xr-x   0        0        0     5646 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2Observability.py
+-rwxr-xr-x   0        0        0     3364 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
+-rwxr-xr-x   0        0        0     5965 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
+-rwxr-xr-x   0        0        0     4538 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
+-rwxr-xr-x   0        0        0     2831 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
+-rw-r--r--   0        0        0    10489 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PhaseLimit.py
+-rw-r--r--   0        0        0     1979 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PropagateStockInfo.py
+-rwxr-xr-x   0        0        0    15779 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RiseDeclineStat.py
+-rw-r--r--   0        0        0    19608 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunParsnip.py
+-rw-r--r--   0        0        0    10460 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunPossis.py
+-rw-r--r--   0        0        0    21719 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSncosmo.py
+-rw-r--r--   0        0        0    10795 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSnoopy.py
+-rw-r--r--   0        0        0     5933 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunTDE.py
+-rw-r--r--   0        0        0      236 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2SNCosmo.py
+-rw-r--r--   0        0        0    20983 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TNSEval.py
+-rw-r--r--   0        0        0    25895 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
+-rw-r--r--   0        0        0    10470 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2XgbClassifier.py
+-rw-r--r--   0        0        0   139314 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
+-rw-r--r--   0        0        0    91172 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
+-rw-r--r--   0        0        0    71112 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
+-rw-r--r--   0        0        0  8028781 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/xgb_trees.py
+-rw-r--r--   0        0        0     3980 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriClient.py
+-rw-r--r--   0        0        0    11364 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriPublisher.py
+-rwxr-xr-x   0        0        0     5598 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
+-rwxr-xr-x   0        0        0    13326 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/DCachePublisher.py
+-rw-r--r--   0        0        0    10625 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcClassPublisher.py
+-rw-r--r--   0        0        0     3565 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcTomClient.py
+-rw-r--r--   0        0        0    10021 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixCorrPlotter.py
+-rw-r--r--   0        0        0     7004 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixTokenGenerator.py
+-rw-r--r--   0        0        0    11976 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/PlotLightcurveSample.py
+-rw-r--r--   0        0        0     4246 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RandomMapGenerator.py
+-rwxr-xr-x   0        0        0     5253 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidBase.py
+-rwxr-xr-x   0        0        0    12504 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidLco.py
+-rwxr-xr-x   0        0        0     4008 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidSedm.py
+-rwxr-xr-x   0        0        0    11948 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/SlackSummaryPublisher.py
+-rwxr-xr-x   0        0        0     1957 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSMirrorUpdater.py
+-rwxr-xr-x   0        0        0    21702 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSTalker.py
+-rwxr-xr-x   0        0        0     2849 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientInfoPrinter.py
+-rw-r--r--   0        0        0    12544 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientTablePublisher.py
+-rwxr-xr-x   0        0        0     4304 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientViewDumper.py
+-rw-r--r--   0        0        0     5173 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/VOEventPublisher.py
+-rwxr-xr-x   0        0        0    13060 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ampel_tns.py
+-rwxr-xr-x   0        0        0     2267 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
+-rwxr-xr-x   0        0        0     4905 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSClient.py
+-rw-r--r--   0        0        0     4100 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
+-rwxr-xr-x   0        0        0     1738 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSName.py
+-rw-r--r--   0        0        0      130 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSToken.py
+-rw-r--r--   0        0        0        0 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/__init__.py
+-rw-r--r--   0        0        0    20855 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
+-rw-r--r--   0        0        0      634 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_config.py
+-rw-r--r--   0        0        0      150 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_flatten.py
+-rw-r--r--   0        0        0     4750 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_slackpublisher.py
+-rw-r--r--   0        0        0     3350 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_t2brightsnprob.py
+-rw-r--r--   0        0        0      468 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_tns.py
+-rw-r--r--   0        0        0     1879 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_tnstalker.py
+-rw-r--r--   0        0        0     8107 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/AmpelHealpix.py
+-rw-r--r--   0        0        0     1043 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/ned.py
+-rw-r--r--   0        0        0      408 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/utils.py
+-rw-r--r--   0        0        0     5328 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/alias.yml
+-rw-r--r--   0        0        0      920 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_10.yml
+-rw-r--r--   0        0        0      660 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_16.yml
+-rw-r--r--   0        0        0      970 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_59.yml
+-rw-r--r--   0        0        0      738 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml
+-rw-r--r--   0        0        0      829 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml
+-rw-r--r--   0        0        0      965 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml
+-rw-r--r--   0        0        0      986 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml
+-rw-r--r--   0        0        0      194 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RANDOM.yml
+-rw-r--r--   0        0        0      242 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID.yml
+-rw-r--r--   0        0        0      800 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
+-rw-r--r--   0        0        0      995 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml
+-rw-r--r--   0        0        0      692 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml
+-rw-r--r--   0        0        0      293 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SOUTH.yml
+-rw-r--r--   0        0        0      293 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_UL.yml
+-rw-r--r--   0        0        0      973 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml
+-rw-r--r--   0        0        0      967 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml
+-rw-r--r--   0        0        0      794 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/AmpelAutoLco.yml
+-rw-r--r--   0        0        0      992 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ChannelSummary.yml
+-rw-r--r--   0        0        0      481 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ClusterSummary.yml
+-rw-r--r--   0        0        0     1369 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/CosmologySummary.yaml
+-rw-r--r--   0        0        0      456 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportal.yml
+-rw-r--r--   0        0        0      585 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml
+-rw-r--r--   0        0        0      568 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml
+-rw-r--r--   0        0        0      431 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/LensingSummary.yml
+-rw-r--r--   0        0        0      371 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidAllz.yml
+-rw-r--r--   0        0        0      645 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidReact.yml
+-rw-r--r--   0        0        0      451 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/TNSSubmitComplete.yml
+-rw-r--r--   0        0        0      573 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/TNSSubmitNew.yml
+-rw-r--r--   0        0        0      205 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
+-rw-r--r--   0        0        0     2545 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/unit.yml
+-rw-r--r--   0        0        0     4774 2024-01-22 10:37:01.782132 ampel_hu_astro-0.8.4a0/pyproject.toml
+-rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.4a0/PKG-INFO
```

### Comparing `ampel_hu_astro-0.8.3a9/LICENSE` & `ampel_hu_astro-0.8.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/README.md` & `ampel_hu_astro-0.8.4a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+<img align="left" src="https://user-images.githubusercontent.com/17532220/213287034-0209aa19-f8a1-418f-a325-7472510542cb.png" width="150" height="150"/>
+<br>
+
+# AMPEL-HU-astro
+<br><br>
+
+
 Contributed Ampel units from HU/DESY group
 ==========================================
 
 Demo install instructions:
 ==========================
 
 Create environment with python 3.10+ / poetry. Then run:
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/channel_notes.txt` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/channel_notes.txt`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/LensedTransientFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/LensedTransientFilter.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                04.27.2018
 # Last Modified Date:  19.03.2021
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 from ampel.ztf.base.CatalogMatchFilter import CatalogMatchFilter
 
-class LensedTransientFilter(CatalogMatchFilter):
 
+class LensedTransientFilter(CatalogMatchFilter):
     ClusListSearchRadius: float
     MasterlensSearchRadius: float
     CastleQSOSearchRadius: float
 
     def __init__(self, **kwargs):
         kwargs["accept"] = {
             "any_of": [
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RandFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RandFilter.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                14.12.2017
 # Last Modified Date:  24.11.2021
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 from random import uniform
+
 from ampel.abstract.AbsAlertFilter import AbsAlertFilter
 
 
 class RandFilter(AbsAlertFilter):
+    passing_rate: float
 
-	passing_rate: float
-
-	def post_init(self):
-		self.logger.info(f"RandFilter initialized with passing rate {self.passing_rate}")
+    def post_init(self):
+        self.logger.info(
+            f"RandFilter initialized with passing rate {self.passing_rate}"
+        )
 
-	def process(self, alert) -> bool:
-		return uniform(0, 1) < self.passing_rate
+    def process(self, alert) -> bool:
+        return uniform(0, 1) < self.passing_rate
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RcfFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RcfFilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License           : BSD-3-Clause
 # Author            : j. nordin <j.nordin@physik.hu-berlin.de>
 # Date              : 06.07.2019
 # Last Modified Date: 08.11.2022
 # Last Modified By  : j. nordin <j.nordin@physik.hu-berlin.de>
 
 import enum
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
 from astropy.coordinates import SkyCoord
 
 from ampel.abstract.AbsAlertFilter import AbsAlertFilter
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 
 
@@ -64,66 +64,65 @@
         min_age = -7
         max_ipac_age = -8
         star_under = -9
         is_not_real = -10
         is_bright_star = -11
         is_variable_star = -12
 
-    def _alert_has_keys(self, alert: Dict[str, Any]) -> bool:
+    def _alert_has_keys(self, alert: dict[str, Any]) -> bool:
         """
         check that given photopoint contains all the keys needed to filter
         """
         for el in self.keys_to_check:
             if el not in alert:
                 self.logger.debug(None, extra={"missing": el})
                 return False
             if alert[el] is None:
                 self.logger.debug(None, extra={"isNone": el})
                 return False
         return True
 
-    def get_galactic_latitude(self, alert: Dict[str, Any]) -> float:
+    def get_galactic_latitude(self, alert: dict[str, Any]) -> float:
         """
         compute galactic latitude of the transient
         """
         coordinates = SkyCoord(alert["ra"], alert["dec"], unit="deg")
-        b = coordinates.galactic.b.deg
-        return b
+        return coordinates.galactic.b.deg
 
-    def previous_pointsource(self, alert: Dict[str, Any], age: float) -> bool:
+    def previous_pointsource(self, alert: dict[str, Any], age: float) -> bool:
         """
         Sets of cases under which a previous source likely existed.
 
         Reject if a previous point source (star) exists beneath. Assumed to be the case if any of:
         - sgscore1>0.76 & 0<distpsnr1<2
         - sgscore>0.2 & distpsnr1 < 1 & srmag1 > 0 &
           (szmag1 > 0 & srmag1 - szmag1 > 3.0) or (simag1 > 0 & srmag1 - simag1 > 3.0)
         """
 
         if (
             alert["sgscore1"] > 0.76
-            and 0 < alert["distpsnr1"]
+            and alert["distpsnr1"] > 0
             and alert["distpsnr1"] < 2
         ):
             return True
         if (
             alert["sgscore1"] > 0.2
-            and 0 < alert["distpsnr1"]
+            and alert["distpsnr1"] > 0
             and alert["distpsnr1"] < 1
             and alert["srmag1"] > 0
         ):
             if alert["szmag1"] > 0 and (alert["srmag1"] - alert["szmag1"]) > 3.0:
                 return True
             if alert["simag1"] > 0 and (alert["srmag1"] - alert["simag1"]) > 3.0:
                 return True
 
         # No clause fulfilled
         return False
 
-    def is_not_real(self, alert: Dict[str, Any], age: float) -> bool:
+    def is_not_real(self, alert: dict[str, Any], age: float) -> bool:
         """
         # Require a high RB score.
         # Generally requires >0.2, but is more stringent if close to a bright catalogued star.
         real = False;
         if (rbscore > 0.2) {
                 real = True;
         }
@@ -155,15 +154,15 @@
         if ps1mag <= 0:
             ps1mag = 99
 
         if alert["rb"] < 0.2:
             return True
         if alert["rb"] < 0.35:
             if (
-                0 < alert["neargaia"]
+                alert["neargaia"] > 0
                 and alert["neargaia"] < 1.0
                 and alert["maggaia"] > 0
                 and alert["maggaia"] < 17.0
             ):
                 return True
             if (
                 alert["distpsnr1"] > 0
@@ -174,15 +173,15 @@
                     return True
                 if alert["simag1"] > 0 and alert["simag1"] < 17:
                     return True
                 if alert["szmag1"] > 0 and alert["szmag1"] < 16.5:
                     return True
         if alert["rb"] < 0.45:
             if (
-                0 < alert["neargaia"]
+                alert["neargaia"] > 0
                 and alert["neargaia"] < 1.5
                 and alert["maggaia"] > 0
                 and alert["maggaia"] < 15.5
             ):
                 return True
             if (
                 alert["distpsnr1"] > 0
@@ -194,81 +193,81 @@
                 if alert["simag1"] > 0 and alert["simag1"] < 15.5:
                     return True
                 if alert["szmag1"] > 0 and alert["szmag1"] < 15.0:
                     return True
 
         if alert["drb"] < 0.5:
             if (
-                0 < alert["distpsnr1"]
+                alert["distpsnr1"] > 0
                 and alert["distpsnr1"] < 3.0
                 and ps1mag < 16
                 and age > 90
             ):
                 return True
             if (
-                0 < alert["distpsnr1"]
+                alert["distpsnr1"] > 0
                 and alert["distpsnr1"] < 1.1
                 and ps1mag < 18
                 and age > 90
             ):
                 return True
 
         if alert["drb"] < 0.8:
             if (
-                0 < alert["distpsnr1"]
+                alert["distpsnr1"] > 0
                 and alert["distpsnr1"] < 1.5
                 and ps1mag < 15.5
                 and age > 90
             ):
                 return True
             if (
-                0 < alert["distpsnr1"]
+                alert["distpsnr1"] > 0
                 and alert["distpsnr1"] < 0.8
                 and ps1mag < 17.5
                 and age > 90
             ):
                 return True
 
         # Passed tests
         return False
 
-    def is_bright_star(self, alert: Dict[str, Any], age: float) -> bool:
+    def is_bright_star(self, alert: dict[str, Any], age: float) -> bool:
         """
         # Could this be residuals from a bright star?
         * Rejected as a bright star if any of:
                 - 0 < neargaiabright < 20 & 0 < maggaiabright < 12
                 - for i in 1,2,3 and f in r,i,z any of:
                         distpsnri<20 & 0<sfmagi<14 & sgscorei > 0.49
           (original filter only cuts around 10" from z-band and ignored 2,3 for i/z)
         """
 
         if (
-            0 < alert["neargaiabright"]
+            alert["neargaiabright"] > 0
             and alert["neargaiabright"] < 20
-            and 0 < alert["maggaiabright"]
+            and alert["maggaiabright"] > 0
             and alert["maggaiabright"] < 12
         ):
             return True
 
         for d in ["1", "2", "3"]:
             for f in ["r", "i", "z"]:
                 if (
-                    0 < alert[f"distpsnr{d}"]
+                    alert[f"distpsnr{d}"] > 0
                     and alert[f"distpsnr{d}"] < 20
-                    and 0 < alert[f"s{f}mag{d}"]
+                    and alert[f"s{f}mag{d}"] > 0
                     and alert[f"s{f}mag{d}"] < 14
                     and alert[f"sgscore{d}"] > 0.9
                 ):
                     return True
 
         # Passed tests
         return False
 
     def is_variable_star(
-        self, alert: Dict[str, Any], age: float, m_peak: float, bright_detections: int
+        self, alert: dict[str, Any], age: float, m_peak: float, bright_detections: int
     ) -> bool:
         """
         Rejected as a variable source if any of:
           - age>90 & not peaking below 18.5 & >= 2 prev. det (>=1 if older than 1 yr) & one of:
             - 0<magnr<19.5 & distnr<0.4
             - 0<magnr<17.5 & distnr<0.8
             - 0<magnr<15.5 & distnr<1.2
@@ -284,54 +283,50 @@
         if alert["sgmag1"] > 0 and alert["sgmag1"] < ps1maxmag:
             ps1maxmag = alert["sgmag1"]
         if alert["szmag1"] > 0 and alert["szmag1"] < ps1maxmag:
             ps1maxmag = alert["szmag1"]
         if ps1maxmag <= 0:
             ps1maxmag = 99
 
-        if m_peak == alert["magpsf"]:
-            is_at_peak = True
-        else:
-            is_at_peak = False
+        is_at_peak = m_peak == alert["magpsf"]
 
         if (
             (age > 90 and bright_detections > 2)
             or (age > 365 and bright_detections > 1)
         ) and not (is_at_peak and alert["magpsf"] < 18.5):
             if (
-                0 < alert["magnr"]
+                alert["magnr"] > 0
                 and alert["magnr"] < 19.5
-                and 0 < alert["distnr"]
+                and alert["distnr"] > 0
                 and alert["distnr"] < 0.4
             ):
                 return True
             if (
-                0 < alert["magnr"]
+                alert["magnr"] > 0
                 and alert["magnr"] < 17.5
-                and 0 < alert["distnr"]
+                and alert["distnr"] > 0
                 and alert["distnr"] < 0.8
             ):
                 return True
             if (
-                0 < alert["magnr"]
+                alert["magnr"] > 0
                 and alert["magnr"] < 15.5
-                and 0 < alert["distnr"]
+                and alert["distnr"] > 0
                 and alert["distnr"] < 1.2
             ):
                 return True
 
-        if 0 < alert["maggaia"] and 0 < alert["neargaia"]:
+        if alert["maggaia"] > 0 and alert["neargaia"] > 0:
             if alert["neargaia"] < 0.35:
                 if age > 30 and alert["maggaia"] < 17:
                     return True
                 if age > 300 and alert["maggaia"] < 19 and alert["magpsf"] > 18.5:
                     return True
-            if alert["neargaia"] < 0.20:
-                if age > 90 and alert["maggaia"] < 18:
-                    return True
+            if alert["neargaia"] < 0.20 and age > 90 and alert["maggaia"] < 18:
+                return True
 
         if (
             alert["sgscore1"] > 0.25
             and alert["distpsnr1"] < 3
             and age > 90
             and ps1maxmag < 16
         ):
@@ -343,26 +338,26 @@
             and age > 90
             and ps1maxmag < 17
         ):
             return True
 
         if (
             age > 90
-            and 0 < alert["distnr"]  # shouldn't this be distnr?  was distnbr
+            and alert["distnr"] > 0  # shouldn't this be distnr?  was distnbr
             and alert["distnr"] < 0.5
             and not is_at_peak
+            and alert["magnr"] > 0
+            and alert["magnr"] < (alert["magpsf"] - 1)
         ):
-            if 0 < alert["magnr"] and alert["magnr"] < (alert["magpsf"] - 1):
-                return True
+            return True
 
         # Passed tests
         return False
 
     def process(self, alert: AmpelAlertProtocol) -> None | bool | int:
-
         # BASE REQUIREMENTS
 
         codes = self.RejectionCode
 
         # Number of detections (not in default)
         npp = len(alert.datapoints)
         if npp < self.min_ndet:
@@ -391,33 +386,36 @@
 
         # check for closeby ss objects
         if 0 <= latest["ssdistnr"] < self.min_dist_to_sso:
             self.logger.debug(None, extra={"ssdistnr": latest["ssdistnr"]})
             return codes.min_ssdistnr
 
         # find first detection date (with pos. detection)
-        jd_first_pps = 10 ** 30
+        jd_first_pps = 10**30
         m_peak = 100
         bright_detections = 0
         for al in alert.datapoints:
-            if not 'isdiffpos' in al.keys() or al["isdiffpos"] == "f" or al["isdiffpos"] == "0":
+            if (
+                "isdiffpos" not in al
+                or al["isdiffpos"] == "f"
+                or al["isdiffpos"] == "0"
+            ):
                 continue
             if al["jd"] < jd_first_pps:
                 jd_first_pps = al["jd"]
             if al["magpsf"] < m_peak:
                 m_peak = al["magpsf"]
             if al["magpsf"] < self.max_magpsf:
                 bright_detections += 1
 
         # print(latest['jd'])
         age = latest["jd"] - latest["jdstarthist"]
 
         self.logger.debug(
-            "%s age %s m now %.2f m peak %.2f nbr previous bright %s"
-            % (alert.id, age, latest["magpsf"], m_peak, bright_detections),
+            f"{alert.id} age {age} m now {latest['magpsf']:.2f} m peak {m_peak:.2f} nbr previous bright {bright_detections}",
             extra={"age": age},
         )
         if age < self.min_age:
             self.logger.debug(None, extra={"age": age})
             return codes.min_age
 
         if self.max_ipac_age > 0:
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/RedshiftCatalogFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RedshiftCatalogFilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,126 +3,137 @@
 # File:                Ampel-HU_astro/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
 # License:             BSD-3-Clause
 # Author:              Jakob Nordin <jnordin@physik.hu-berlin.de>
 # Date:                02.11.2022
 # Last Modified Date:  02.11.2022
 # Last Modified By:    jnordin <jnordin@physik.hu-berlin.de>
 
-from typing import Literal
-import numpy as np
 from functools import partial
+from typing import Literal
 
-from ampel.ztf.t0.DecentFilter import DecentFilter
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
+from ampel.ztf.t0.DecentFilter import DecentFilter
 
 
 class RedshiftCatalogFilter(DecentFilter):
-	"""
-	Filter derived from DecentFilter designed to only accept transients
-	located close to a galaxy in a catalog, and within redshift bounds.
-
-	Default parameters focused on matching with nearby catalogs.
-	Current generation of filter uses a copy of the NED galaxy archive
-	to z 0.02x (0.03?), downloaded ~2020.
-
-	If any match within the radius is found, the candidate will be stat_accepted
-	(even if it, for example, is not the closest match).
-
-	Many DecentFilter parameters are set as defaults, including turning
-	off matching to Gaia for stars (it is assumed that the catalog matching
-	is sufficient for rejection).
-
-	Notes: Much catalog match functions, including combining multiple catalogs
-	already exist in CatalogMatchFilter. Here we wished to also make use of
-	DecentFilter setup, hence the partial code repetition.
-	Similarly, extcat filters could use the post_filter option for immediate
-	filtering, but it is not sure how general this can be made.
-	"""
-
-	# Catalog matching parameters
-	catalog_name: str = 'NEDz_extcats'
-	catalog_type: Literal["extcats","catsHTM"] = "extcats"
-	catalog_match_radius: float = 60.   # Match radius in arcsec
-	catalog_zkey: str = 'z'  # Should match redshift key in catalog
-	min_z: float = 0.002  # Some stars found in e.g. NED.
-	max_z: float = 0.03   # Max redshift (after catalog match)
-	# Remaining decent filter parameters
-	max_tspan: float  # maximum duration of alert detection history [days]
-	max_archive_tspan: float # maximum duration of alert detection history [days]
-	min_drb: float = 0.0  # deep learning real bogus score
-	min_rb: float  # real bogus score
+    """
+    Filter derived from DecentFilter designed to only accept transients
+    located close to a galaxy in a catalog, and within redshift bounds.
+
+    Default parameters focused on matching with nearby catalogs.
+    Current generation of filter uses a copy of the NED galaxy archive
+    to z 0.02x (0.03?), downloaded ~2020.
+
+    If any match within the radius is found, the candidate will be stat_accepted
+    (even if it, for example, is not the closest match).
+
+    Many DecentFilter parameters are set as defaults, including turning
+    off matching to Gaia for stars (it is assumed that the catalog matching
+    is sufficient for rejection).
+
+    Notes: Much catalog match functions, including combining multiple catalogs
+    already exist in CatalogMatchFilter. Here we wished to also make use of
+    DecentFilter setup, hence the partial code repetition.
+    Similarly, extcat filters could use the post_filter option for immediate
+    filtering, but it is not sure how general this can be made.
+    """
+
+    # Catalog matching parameters
+    catalog_name: str = "NEDz_extcats"
+    catalog_type: Literal["extcats", "catsHTM"] = "extcats"
+    catalog_match_radius: float = 60.0  # Match radius in arcsec
+    catalog_zkey: str = "z"  # Should match redshift key in catalog
+    min_z: float = 0.002  # Some stars found in e.g. NED.
+    max_z: float = 0.03  # Max redshift (after catalog match)
+    # Remaining decent filter parameters
+    max_tspan: float  # maximum duration of alert detection history [days]
+    max_archive_tspan: float  # maximum duration of alert detection history [days]
+    min_drb: float = 0.0  # deep learning real bogus score
+    min_rb: float  # real bogus score
 
-	# DecentFilter default parameter overrides to match this purpose
+    # DecentFilter default parameter overrides to match this purpose
     # Tuned based on 2021 infant SN search comparison (contact J Nordin)
-	min_ndet: int  = 0# number of previous detections
-	min_tspan: float = -666.  # minimum duration of alert detection history [days]
-	min_archive_tspan: float = -666. # minimum duration of alert detection history [days]
-	max_fwhm: float  = 4.5 # sexctrator FWHM (assume Gaussian) [pix]
-	max_elong: float = 1.4 # Axis ratio of image: aimage / bimage
-	max_magdiff: float  = 1 # Difference: magap - magpsf [mag]
-	max_nbad: int  = 0# number of bad pixels in a 5 x 5 pixel stamp
-	min_sso_dist: float = 20.  # distance to nearest solar system object [arcsec]
-	min_gal_lat: float  = 14. # minium distance from galactic plane. Set to negative to disable cut.
-	ps1_sgveto_rad: float = 2. # maximum distance to closest PS1 source for SG score veto [arcsec]
-	ps1_sgveto_th: float = 0.8  # maximum allowed SG score for PS1 source within PS1_SGVETO_RAD
-	ps1_confusion_rad: float = 3. # reject alerts if the three PS1 sources are all within this radius [arcsec]
-	ps1_confusion_sg_tol: float = 0.1  # and if the SG score of all of these 3 sources is within this tolerance to 0.5
-	# Gaia matching is here turned off, standard match radius is 20.
-	gaia_rs: float = -999. # search radius for GAIA DR2 matching [arcsec]
-	gaia_pm_signif: float = 3.  # significance of proper motion detection of GAIA counterpart [sigma]
-	gaia_plx_signif: float = 3. # significance of parallax detection of GAIA counterpart [sigma]
-	gaia_veto_gmag_min: float = 9. # min gmag for normalized distance cut of GAIA counterparts [mag]
-	gaia_veto_gmag_max: float = 20. # max gmag for normalized distance cut of GAIA counterparts [mag]
-	gaia_excessnoise_sig_max: float = 999.  # maximum allowed noise (expressed as significance) for Gaia match to be trusted.
-
-
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-		query = {
-				"name": self.catalog_name,
-				"use": self.catalog_type,
-				"rs_arcsec": self.catalog_match_radius,
-				"keys_to_append": [self.catalog_zkey],
-				}
-		# For exctcats, directly add the z filter
-		if self.catalog_type=='extcats':
-			query['post_filter'] = {self.catalog_zkey: {
-														"$gte":self.min_z,
-														"$lte":self.max_z}
-									}
-
-		self.catalog_query = partial(
-			self.cone_search_all,
-			catalogs=[ query ]
-		)
-
-
-	def process(self, alert: AmpelAlertProtocol):
-		"""
-		Run the filter on the alert. First we run the decent filter, then we match
-		with the infant catalog.
-		"""
-
-		# First make default DefentFilter check
-		if not (decent_result := super().process(alert)):
-			return decent_result
-
-		# if the candidate has passed the decent filter, check if it is compatible
-		# with the position of some nearby galaxy cluster
-		latest = alert.datapoints[0]
-		alert_ra = latest['ra']
-		alert_dec = latest['dec']
-
-		# Check for catalog matches .
-		catalog_matches = self.catalog_query(alert_ra, alert_dec)[0]
-		if catalog_matches is None:
-			return None
-
-		# For all catalog matches, check redshift range
-		matched = None
-		for catmatch in catalog_matches:
-			# CatalogItem object
-			if (matched := (self.min_z <= catmatch['body'][self.catalog_zkey] <= self.max_z ) ):
-				break
+    min_ndet: int = 0  # number of previous detections
+    min_tspan: float = -666.0  # minimum duration of alert detection history [days]
+    min_archive_tspan: float = (
+        -666.0
+    )  # minimum duration of alert detection history [days]
+    max_fwhm: float = 4.5  # sexctrator FWHM (assume Gaussian) [pix]
+    max_elong: float = 1.4  # Axis ratio of image: aimage / bimage
+    max_magdiff: float = 1  # Difference: magap - magpsf [mag]
+    max_nbad: int = 0  # number of bad pixels in a 5 x 5 pixel stamp
+    min_sso_dist: float = 20.0  # distance to nearest solar system object [arcsec]
+    min_gal_lat: float = (
+        14.0  # minium distance from galactic plane. Set to negative to disable cut.
+    )
+    ps1_sgveto_rad: float = (
+        2.0  # maximum distance to closest PS1 source for SG score veto [arcsec]
+    )
+    ps1_sgveto_th: float = (
+        0.8  # maximum allowed SG score for PS1 source within PS1_SGVETO_RAD
+    )
+    ps1_confusion_rad: float = 3.0  # reject alerts if the three PS1 sources are all within this radius [arcsec]
+    ps1_confusion_sg_tol: float = 0.1  # and if the SG score of all of these 3 sources is within this tolerance to 0.5
+    # Gaia matching is here turned off, standard match radius is 20.
+    gaia_rs: float = -999.0  # search radius for GAIA DR2 matching [arcsec]
+    gaia_pm_signif: float = (
+        3.0  # significance of proper motion detection of GAIA counterpart [sigma]
+    )
+    gaia_plx_signif: float = (
+        3.0  # significance of parallax detection of GAIA counterpart [sigma]
+    )
+    gaia_veto_gmag_min: float = (
+        9.0  # min gmag for normalized distance cut of GAIA counterparts [mag]
+    )
+    gaia_veto_gmag_max: float = (
+        20.0  # max gmag for normalized distance cut of GAIA counterparts [mag]
+    )
+    gaia_excessnoise_sig_max: float = 999.0  # maximum allowed noise (expressed as significance) for Gaia match to be trusted.
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        query = {
+            "name": self.catalog_name,
+            "use": self.catalog_type,
+            "rs_arcsec": self.catalog_match_radius,
+            "keys_to_append": [self.catalog_zkey],
+        }
+        # For exctcats, directly add the z filter
+        if self.catalog_type == "extcats":
+            query["post_filter"] = {
+                self.catalog_zkey: {"$gte": self.min_z, "$lte": self.max_z}
+            }
+
+        self.catalog_query = partial(self.cone_search_all, catalogs=[query])
+
+    def process(self, alert: AmpelAlertProtocol):
+        """
+        Run the filter on the alert. First we run the decent filter, then we match
+        with the infant catalog.
+        """
+
+        # First make default DefentFilter check
+        if not (decent_result := super().process(alert)):
+            return decent_result
+
+        # if the candidate has passed the decent filter, check if it is compatible
+        # with the position of some nearby galaxy cluster
+        latest = alert.datapoints[0]
+        alert_ra = latest["ra"]
+        alert_dec = latest["dec"]
+
+        # Check for catalog matches .
+        catalog_matches = self.catalog_query(alert_ra, alert_dec)[0]
+        if catalog_matches is None:
+            return None
+
+        # For all catalog matches, check redshift range
+        matched = None
+        for catmatch in catalog_matches:
+            # CatalogItem object
+            if matched := (
+                self.min_z <= catmatch["body"][self.catalog_zkey] <= self.max_z
+            ):
+                break
 
-		return matched
+        return matched
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/SimpleDecentFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/SimpleDecentFilter.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,59 +3,63 @@
 # File:                Ampel-HU-astro/ampel/contrib/hu/t0/SimpleDecentFilter.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                12.02.2019
 # Last Modified Date:  2.11.2021
 # Last Modified By:    jn <jnordin@physik.hu-berlin.de>
 
-import numpy as np
-from typing import Any
-from astropy.table import Table
 from astropy.coordinates import SkyCoord
 
-from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 from ampel.abstract.AbsAlertFilter import AbsAlertFilter
+from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 
 
 class SimpleDecentFilter(AbsAlertFilter):
     """
-	General-purpose filter devloped alongside DecentFilter but without use of external catalogs.
-	It selects alerts based on:
-	* numper of previous detections
-	* positive subtraction flag
-	* loose cuts on image quality (fwhm, elongation, number of bad pixels, and the
-	difference between PSF and aperture magnitude)
-	* distance to known SS objects
-	* (d) real-bogus
-	* Whether it seems a PS source exists at the transient position (as per alert properties).
-	"""
-
-	# history
-    min_ndet: int = 2 # number of previous detections
-    min_tspan: float = 0.02 # minimum duration of alert detection history [days]
-    max_tspan: float = 25. # maximum duration of alert detection history [days]
-    min_archive_tspan: float = 0. # minimum duration of alert detection history [days]
-    max_archive_tspan: float = 10**5. # maximum duration of alert detection history [days]
+    General-purpose filter devloped alongside DecentFilter but without use of external catalogs.
+    It selects alerts based on:
+    * numper of previous detections
+    * positive subtraction flag
+    * loose cuts on image quality (fwhm, elongation, number of bad pixels, and the
+    difference between PSF and aperture magnitude)
+    * distance to known SS objects
+    * (d) real-bogus
+    * Whether it seems a PS source exists at the transient position (as per alert properties).
+    """
+
+    # history
+    min_ndet: int = 2  # number of previous detections
+    min_tspan: float = 0.02  # minimum duration of alert detection history [days]
+    max_tspan: float = 25.0  # maximum duration of alert detection history [days]
+    min_archive_tspan: float = 0.0  # minimum duration of alert detection history [days]
+    max_archive_tspan: float = (
+        10**5.0
+    )  # maximum duration of alert detection history [days]
 
     # Image quality
-    min_drb: float = 0. # deep learning real bogus score
-    min_rb: float = 0.3 # real bogus score
-    max_fwhm: float = 5. # sexctrator FWHM (assume Gaussian) [pix]
-    max_elong: float = 1.4 # Axis ratio of image: aimage / bimage
-    max_magdiff: float = 0.4 # Difference: magap - magpsf [mag]
-    max_nbad: int = 0 # number of bad pixels in a 5 x 5 pixel stamp
+    min_drb: float = 0.0  # deep learning real bogus score
+    min_rb: float = 0.3  # real bogus score
+    max_fwhm: float = 5.0  # sexctrator FWHM (assume Gaussian) [pix]
+    max_elong: float = 1.4  # Axis ratio of image: aimage / bimage
+    max_magdiff: float = 0.4  # Difference: magap - magpsf [mag]
+    max_nbad: int = 0  # number of bad pixels in a 5 x 5 pixel stamp
 
     # astro
-    min_sso_dist: float = 20. # distance to nearest solar system object [arcsec]
-    min_gal_lat: float = 0. # minium distance from galactic plane. Set to negative to disable cut.
-    ps1_sgveto_rad: float = 2. # maximum distance to closest PS1 source for SG score veto [arcsec]
-    ps1_sgveto_th: float = 0.8 # maximum allowed SG score for PS1 source within PS1_SGVETO_RAD
-    ps1_confusion_rad: float = 1. # reject alerts if the three PS1 sources are all within this radius [arcsec]
-    ps1_confusion_sg_tol: float = 0.5 # and if the SG score of all of these 3 sources is within this tolerance to 0.5
-
+    min_sso_dist: float = 20.0  # distance to nearest solar system object [arcsec]
+    min_gal_lat: float = (
+        0.0  # minium distance from galactic plane. Set to negative to disable cut.
+    )
+    ps1_sgveto_rad: float = (
+        2.0  # maximum distance to closest PS1 source for SG score veto [arcsec]
+    )
+    ps1_sgveto_th: float = (
+        0.8  # maximum allowed SG score for PS1 source within PS1_SGVETO_RAD
+    )
+    ps1_confusion_rad: float = 1.0  # reject alerts if the three PS1 sources are all within this radius [arcsec]
+    ps1_confusion_sg_tol: float = 0.5  # and if the SG score of all of these 3 sources is within this tolerance to 0.5
 
     def post_init(self):
         # feedback
         for k in self.__annotations__:
             self.logger.info(f"Using {k}={getattr(self, k)}")
 
         # To make this tenable we should create this list dynamically depending on what entries are required
@@ -75,53 +79,49 @@
             "ra",
             "dec",
             "rb",
             "ssdistnr",
         )
 
         # How to filter for detections in alert
-        self.filter_pps = [{'attribute': 'magpsf', 'operator': 'is not', 'value': None}]
-
+        self.filter_pps = [{"attribute": "magpsf", "operator": "is not", "value": None}]
 
     def _alert_has_keys(self, photop) -> bool:
         """
         check that given photopoint contains all the keys needed to filter
         """
         for el in self.keys_to_check:
             if el not in photop:
                 self.logger.info(None, extra={"missing": el})
                 return False
             if photop[el] is None:
                 self.logger.info(None, extra={"isNone": el})
                 return False
         return True
 
-
     def get_galactic_latitude(self, transient):
         """
         compute galactic latitude of the transient
         """
         coordinates = SkyCoord(transient["ra"], transient["dec"], unit="deg")
         return coordinates.galactic.b.deg
 
-
     def is_star_in_PS1(self, transient) -> bool:
         """
         apply combined cut on sgscore1 and distpsnr1 to reject the transient if
         there is a PS1 star-like object in it's immediate vicinity
         """
 
         # TODO: consider the case of alert moving wrt to the position of a star
         # maybe cut on the minimum of the distance!
         return (
             transient["distpsnr1"] < self.ps1_sgveto_rad
             and transient["sgscore1"] > self.ps1_sgveto_th
         )
 
-
     def is_confused_in_PS1(self, transient) -> bool:
         """
         check in PS1 for source confusion, which can induce subtraction artifatcs.
         These cases are selected requiring that all three PS1 cps are in the imediate
         vicinity of the transient and their sgscore to be close to 0.5 within given tolerance.
         """
         very_close = (
@@ -144,63 +144,60 @@
                 abs(transient["sgscore3"] - 0.5),
             )
             < self.ps1_confusion_sg_tol
         )
 
         return sg_confused and very_close
 
-
     # Override
     def process(self, alert: AmpelAlertProtocol) -> None | bool | int:
         """
         Mandatory implementation.
         To exclude the alert, return *None*
         To accept it, either return
         * self.on_match_t2_units
         * or a custom combination of T2 unit names
         """
 
-
         # CUT ON THE HISTORY OF THE ALERT
         #################################
 
-        detection_jds = alert.get_values('jd',filters=self.filter_pps)
+        detection_jds = alert.get_values("jd", filters=self.filter_pps)
         npp = len(detection_jds)
         if npp < self.min_ndet:
             # self.logger.debug("rejected: %d photopoints in alert (minimum required %d)"% (npp, self.min_ndet))
             self.logger.info(None, extra={"nDet": npp})
             return None
 
         # cut on length of detection history
         det_tspan = max(detection_jds) - min(detection_jds)
         if not (self.min_tspan <= det_tspan <= self.max_tspan):
             # self.logger.debug("rejected: detection history is %.3f d long, \
             # requested between %.3f and %.3f d"% (det_tspan, self.min_tspan, self.max_tspan))
             self.logger.info(None, extra={"tSpan": det_tspan})
             return None
 
-
         # IMAGE QUALITY CUTS
         ####################
 
-        latest = alert.datapoints[0]   # Assuming alert structure where det comes first
+        latest = alert.datapoints[0]  # Assuming alert structure where det comes first
         if not self._alert_has_keys(latest):
             return None
 
         if latest["isdiffpos"] == "f" or latest["isdiffpos"] == "0":
             # self.logger.debug("rejected: 'isdiffpos' is %s", latest['isdiffpos'])
             self.logger.info(None, extra={"isdiffpos": latest["isdiffpos"]})
             return None
 
         if latest["rb"] < self.min_rb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
             self.logger.info(None, extra={"rb": latest["rb"]})
             return None
 
-        if self.min_drb > 0.0 and latest["drb"] < self.min_drb:
+        if latest.get("drb") and self.min_drb > 0.0 and latest["drb"] < self.min_drb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
             self.logger.info(None, extra={"drb": latest["drb"]})
             return None
 
         if latest["fwhm"] > self.max_fwhm:
             # self.logger.debug("rejected: fwhm %.2f above threshod (%.2f)"% (latest['fwhm'], self.max_fwhm))
             self.logger.info(None, extra={"fwhm": latest["fwhm"]})
@@ -213,21 +210,20 @@
 
         if abs(latest["magdiff"]) > self.max_magdiff:
             # self.logger.debug("rejected: magdiff (AP-PSF) %.2f above threshod (%.2f)"% (latest['magdiff'], self.max_magdiff))
             self.logger.info(None, extra={"magdiff": latest["magdiff"]})
             return None
 
         # cut on archive length
-        if 'jdendhist' in latest.keys() and 'jdstarthist' in latest.keys():
-            archive_tspan = latest['jdendhist'] - latest['jdstarthist']
+        if "jdendhist" in latest and "jdstarthist" in latest:
+            archive_tspan = latest["jdendhist"] - latest["jdstarthist"]
             if not (self.min_archive_tspan < archive_tspan < self.max_archive_tspan):
-                self.logger.info(None, extra={'archive_tspan': archive_tspan})
+                self.logger.info(None, extra={"archive_tspan": archive_tspan})
                 return None
 
-
         # ASTRONOMY
         ###########
 
         # check for closeby ss objects
         if 0 <= latest["ssdistnr"] < self.min_sso_dist:
             # self.logger.debug("rejected: solar-system object close to transient (max allowed: %d)."% (self.min_sso_dist))
             self.logger.info(None, extra={"ssdistnr": latest["ssdistnr"]})
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/TransientInClusterFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/TransientInClusterFilter.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,92 +3,96 @@
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t0/TransientInClusterFilter.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                28.08.2018
 # Last Modified Date:  24.11.2021
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
-import numpy as np
 from functools import partial
-from ampel.ztf.t0.DecentFilter import DecentFilter
+
+import numpy as np
+
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
+from ampel.ztf.t0.DecentFilter import DecentFilter
 
 
 class TransientInClusterFilter(DecentFilter):
-	"""
-	Filter derived from the DecentFilter, in addition selecting candidates
-	with position compatible with that of nearby galaxy clusters.
-	"""
-
-	big_search_radius_arcmin: float	# conservative search radius around cluster position. Max in RASSEBCS is 16.a arcmin
-	cluserter_rad_multiplier: float # if we want to enlarge the search region around each cluster.
-
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-		# feedback
-		for k in self.__annotations__:
-			self.logger.info(f"Using {k}={getattr(self, k)}")
-
-		self.rassebcs_query = partial(
-			self.cone_search_all,
-			catalogs=[
-				{
-					"name": "RASSEBCS",
-					"use": "extcats",
-					"rs_arcsec": self.big_search_radius_arcmin * 60 * self.cluserter_rad_multiplier,
-					"keys_to_append": ["ANGULAR_RADIUS"],
-				}
-			]
-		)
-
-
-	def process(self, alert: AmpelAlertProtocol):
-		"""
-		run the filter on the alert. First we run the decent filter, then we match
-		with the cluster catalog.
-		"""
-
-		# if the candidate has passed the decent filter, check if it is compatible
-		# with the position of some nearby galaxy cluster
-		latest = alert.datapoints[0]
-		alert_ra = latest['ra']
-		alert_dec = latest['dec']
-
-		# A) find position of all the nearby clusters. If none is found, reject alert.
-		nearby_clusters = self.rassebcs_query(alert_ra, alert_dec)[0]
-
-		if nearby_clusters is None:
-			self.logger.debug(
-				f"rejected: no cluster from RASSEBCS within {self.big_search_radius_arcmin*60:.2f} arcsec from alert position"
-			)
-			return None
-
-		# B) for all the nearby clusters, compute their distances to the alert
-		# (extcats works in arcsec but ANGULAR_RADIUS is in arcmin)
-		clust_dists_2_alert = np.array([d["dist_arcsec"] for d in nearby_clusters]) / 60.
-		clust_radius = np.array([d["body"]["ANGULAR_RADIUS"] for d in nearby_clusters])
-
-		# C) if, for any of the nearby clusters, the distance to the alert is smaller
-		# than the cluster size, count this as a match
-		if not any(clust_radius > clust_dists_2_alert):
-
-			self.logger.debug(
-				"rejected: distance to alert is larger than the cluster size for all the nearby clusters"
-			)
-
-			for ii in range(len(nearby_clusters)):
-				self.logger.debug(
-					f"Angular radius: {clust_radius[ii]:.2f}, "
-					f"distance to alert: {clust_dists_2_alert[ii]:.2f} (both arcmin)"
-				)
-
-			return None
-
-		for ii in range(len(nearby_clusters)):
-			self.logger.debug(
-				f"Angular radius: {clust_radius[ii]:.2f}, "
-				f"distance to alert: {clust_dists_2_alert[ii]:.2f} (both arcmin)"
-			)
+    """
+    Filter derived from the DecentFilter, in addition selecting candidates
+    with position compatible with that of nearby galaxy clusters.
+    """
+
+    big_search_radius_arcmin: float  # conservative search radius around cluster position. Max in RASSEBCS is 16.a arcmin
+    cluserter_rad_multiplier: float  # if we want to enlarge the search region around each cluster.
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # feedback
+        for k in self.__annotations__:
+            self.logger.info(f"Using {k}={getattr(self, k)}")
+
+        self.rassebcs_query = partial(
+            self.cone_search_all,
+            catalogs=[
+                {
+                    "name": "RASSEBCS",
+                    "use": "extcats",
+                    "rs_arcsec": self.big_search_radius_arcmin
+                    * 60
+                    * self.cluserter_rad_multiplier,
+                    "keys_to_append": ["ANGULAR_RADIUS"],
+                }
+            ],
+        )
+
+    def process(self, alert: AmpelAlertProtocol):
+        """
+        run the filter on the alert. First we run the decent filter, then we match
+        with the cluster catalog.
+        """
+
+        # if the candidate has passed the decent filter, check if it is compatible
+        # with the position of some nearby galaxy cluster
+        latest = alert.datapoints[0]
+        alert_ra = latest["ra"]
+        alert_dec = latest["dec"]
+
+        # A) find position of all the nearby clusters. If none is found, reject alert.
+        nearby_clusters = self.rassebcs_query(alert_ra, alert_dec)[0]
+
+        if nearby_clusters is None:
+            self.logger.debug(
+                f"rejected: no cluster from RASSEBCS within {self.big_search_radius_arcmin*60:.2f} arcsec from alert position"
+            )
+            return None
+
+        # B) for all the nearby clusters, compute their distances to the alert
+        # (extcats works in arcsec but ANGULAR_RADIUS is in arcmin)
+        clust_dists_2_alert = (
+            np.array([d["dist_arcsec"] for d in nearby_clusters]) / 60.0
+        )
+        clust_radius = np.array([d["body"]["ANGULAR_RADIUS"] for d in nearby_clusters])
+
+        # C) if, for any of the nearby clusters, the distance to the alert is smaller
+        # than the cluster size, count this as a match
+        if not any(clust_radius > clust_dists_2_alert):
+            self.logger.debug(
+                "rejected: distance to alert is larger than the cluster size for all the nearby clusters"
+            )
+
+            for ii in range(len(nearby_clusters)):
+                self.logger.debug(
+                    f"Angular radius: {clust_radius[ii]:.2f}, "
+                    f"distance to alert: {clust_dists_2_alert[ii]:.2f} (both arcmin)"
+                )
+
+            return None
+
+        for ii in range(len(nearby_clusters)):
+            self.logger.debug(
+                f"Angular radius: {clust_radius[ii]:.2f}, "
+                f"distance to alert: {clust_dists_2_alert[ii]:.2f} (both arcmin)"
+            )
 
-		# now run the decent filter (faster to do it afterwards ;-)
-		return super().process(alert)
+        # now run the decent filter (faster to do it afterwards ;-)
+        return super().process(alert)
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t0/XShooterFilter.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/XShooterFilter.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t0/XShooterFilter.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                28.08.2018
 # Last Modified Date:  24.11.2021
 # Last Modified By:    jnordin
 
-from typing import Optional
 from numpy import array
+
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 from ampel.ztf.t0.DecentFilter import DecentFilter
 
 
 class XShooterFilter(DecentFilter):
     """
     Filter derived from the DecentFilter, in addition selecting very new
@@ -21,24 +21,26 @@
     during the last 5 days (and no detection during this time).
     """
 
     max_dec: float  # maximum allowed value for the declination
     det_within: float  # the transient must have been detected within the last 'DET_WITHIN' days
     ul_within: float  # the transient must AT LEAST one ulim within the last 'UL_WITHIN' days
     # Updated parameters based on infant detections spring 2021. Defaults conservative
-    max_chipsf: float = 4        # Best guess value 2
-    max_seeratio: float = 2      # Best guess value 1.3
-    min_sumrat: float = 0.6      # Best guess value 0.8
+    max_chipsf: float = 4  # Best guess value 2
+    max_seeratio: float = 2  # Best guess value 1.3
+    min_sumrat: float = 0.6  # Best guess value 0.8
 
     def post_init(self):
         super().post_init()
-        #self.keys_to_check += ("jd",)
+        # self.keys_to_check += ("jd",)
         # Is none not working, now doing this manually
-        #self.select_upper_limits = [{'attribute': 'magpsf', 'operator': 'is', 'value': None}]
-        self.select_photopoints = [{'attribute': 'magpsf', 'operator': 'is not', 'value': None}]
+        # self.select_upper_limits = [{'attribute': 'magpsf', 'operator': 'is', 'value': None}]
+        self.select_photopoints = [
+            {"attribute": "magpsf", "operator": "is not", "value": None}
+        ]
 
     # Override
     def process(self, alert: AmpelAlertProtocol) -> None | bool | int:
         """
         run the decent filter on the alert
         """
 
@@ -69,15 +71,14 @@
         if latest["sumrat"] < self.min_sumrat:
             self.logger.debug(
                 f"Rejected: sumrat {latest['sumrat']:.2f}  "
                 f"below min allowed of {self.min_sumrat:.2f}"
             )
             return None
 
-
         # CUT ON THE HISTORY OF THE ALERT
         #################################
 
         now_jd = latest["jd"]
         self.logger.debug(f"Setting 'now' to JD {now_jd:.4f} to cut on alert history")
 
         # check on history 1: detected in the last 6h
@@ -88,15 +89,15 @@
                 f"Rejected: no detection within the last {self.det_within:.3f} days "
                 f"(latest one {(now_jd - max(detection_jds)):.3f} days ago)"
             )
             return None
 
         # check on the history 2: at least one upper limit in the last 5 days
         # old version to look for upper limits not working...
-        ulim_jds = [el['jd'] for el in alert.datapoints if el.get("candid") is  None]
+        ulim_jds = [el["jd"] for el in alert.datapoints if el.get("candid") is None]
         if ulim_jds is None:
             self.logger.debug("Rejected: this alert has no upper limits")
             return None
 
         if not any(array(ulim_jds) > (now_jd - self.ul_within)):
             self.logger.debug(
                 f"Rejected: no upper limit in the last {self.ul_within:.3f} days"
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2BrightSNProb.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BrightSNProb.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 # File:                ampel/contrib/hu/t2/T2GuessSN.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                06.04.2020
 # Last Modified Date:  03.08.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
+from typing import TypedDict
+
 import numpy as np
-from typing import Union
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.view.LightCurve import LightCurve
+
 from ampel.abstract.AbsLightCurveT2Unit import AbsLightCurveT2Unit
+from ampel.contrib.hu.t2 import xgb_trees
 from ampel.contrib.hu.t2.T2RiseDeclineStat import T2RiseDeclineBase
-import ampel.contrib.hu.t2.xgb_trees as xgb_trees
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
+from ampel.view.LightCurve import LightCurve
+
+
+class XgbTreeParam(TypedDict):
+    max_duration: float
+    max_predetect: float
+    min_detmag: float
 
 
 class T2BrightSNProb(AbsLightCurveT2Unit, T2RiseDeclineBase):
     """
     Derive a number of simple metrics describing the rise, peak and decline of a lc.
     Run a XGB tree trained to check whether this transient are likely to be an RCF SN.
     """
@@ -37,28 +45,26 @@
             "magnr_med",
             "classtar_med",
             "sgscore1_med",
             "distpsnr1_med",
             "neargaia_med",
             "maggaia_med",
         ]
-        self.xgb_tree_param = {
+        self.xgb_tree_param: dict[int, XgbTreeParam] = {
             2: {"max_duration": 3.5, "max_predetect": 3.5, "min_detmag": 16},
             3: {"max_duration": 6.5, "max_predetect": 3.5, "min_detmag": 16},
             4: {"max_duration": 6.5, "max_predetect": 3.5, "min_detmag": 16},
             5: {"max_duration": 10, "max_predetect": 3.5, "min_detmag": 16},
             6: {"max_duration": 10, "max_predetect": 3.5, "min_detmag": 16},
             100: {"max_duration": 90, "max_predetect": 10, "min_detmag": 16},
         }
         # Load the (large) set of trees
         self.xgb_tree = xgb_trees.xgboost_tree()
 
-
     def process(self, light_curve: LightCurve) -> UBson | UnitResult:
-
         # Output dict that we will start to populate
         o = self.compute_stats(light_curve)
 
         if not o["success"]:
             return o
 
         # This is where the data collection stops and evaluation starts.
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2CatalogMatchLocal.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2CatalogMatchLocal.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,57 +3,54 @@
 # File:                ampel-hu-astro/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
 # License:             BSD-3-Clause
 # Author:              matteo.giomi@desy.de
 # Date:                24.08.2018
 # Last Modified Date:  2.12.2021
 # Last Modified By:    jn <jnordin@physik.hu-berlin.de>
 
-from typing import Any, ClassVar, Literal
 from functools import cached_property
-from ampel.types import UBson
+from typing import Any, ClassVar, Literal
 
-from extcats import CatalogQuery
-from pymongo import MongoClient
-from pymongo.errors import AutoReconnect
 import backoff
-
-
 from astropy.coordinates import SkyCoord
 from astropy.table import Table
+from extcats import CatalogQuery
 from extcats.catquery_utils import get_closest, get_distances
 from numpy import asarray, degrees
+from pymongo import MongoClient
+from pymongo.errors import AutoReconnect
 
 from ampel.abstract.AbsPointT2Unit import AbsPointT2Unit
 from ampel.content.DataPoint import DataPoint
 from ampel.enum.DocumentCode import DocumentCode
-from ampel.struct.UnitResult import UnitResult
-
 from ampel.model.DPSelection import DPSelection
-
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.ztf.t2.T2CatalogMatch import CatalogModel
 
 
-
 class ExtcatsUnit:
     """
     Interface to standard extcats
     """
 
-#    require = ("extcats",)
+    #    require = ("extcats",)
     extcat_path: None | str = None
 
     max_query_time: float = 300
 
     @cached_property
     def catq_client(self):
         # As this is for local use we assume authorization is not needed
-        #return MongoClient(self.resource["extcats"], **self.extcats.auth.get())
+        # return MongoClient(self.resource["extcats"], **self.extcats.auth.get())
         return MongoClient(self.extcat_path)
 
-    def get_extcats_query(self, catalog, logger, ra_key="ra", dec_key="dec", *args, **kwargs):
+    def get_extcats_query(
+        self, catalog, logger, ra_key="ra", dec_key="dec", *args, **kwargs
+    ):
         q = CatalogQuery.CatalogQuery(
             catalog,
             *args,
             **kwargs,
             ra_key=ra_key,
             dec_key=dec_key,
             logger=logger,
@@ -61,61 +58,57 @@
         )
         decorate = backoff.on_exception(
             backoff.expo,
             AutoReconnect,
             logger=logger,
             max_time=self.max_query_time,
         )
-        for method in 'binaryserach', 'findclosest', 'findwithin':
-            setattr(
-                q,
-                method,
-                decorate(getattr(q, method))
-            )
+        for method in "binaryserach", "findclosest", "findwithin":
+            setattr(q, method, decorate(getattr(q, method)))
         return q
 
 
 class ExtcatsCatalogModel(CatalogModel):
-    catq_kwargs: dict[str,Any] = {}
+    catq_kwargs: dict[str, Any] = {}
     use: Literal["extcats"]
 
+
 class T2CatalogMatchLocal(ExtcatsUnit, AbsPointT2Unit):
     """
     Cross matches the position of a transient to those of sources in a set of catalogs
 
     :param catalogs: each value specifies a catalog in extcats or catsHTM format
      and the query parameters.
 
     .. note:: This requires access to a mongod hosting extcats databases and a
       filesystem containing catsHTM catalogs. For a similar unit that uses hosted
       services, see :class:`~ampel.ztf.t2.T2CatalogMatch`.
     """
 
     # run only on first datapoint by default
-    eligible: ClassVar[DPSelection] = DPSelection(filter='PPSFilter', sort='jd', select='first')
+    eligible: ClassVar[DPSelection] = DPSelection(
+        filter="PPSFilter", sort="jd", select="first"
+    )
 
     # Each value specifies a catalog in extcats or catsHTM format and the query parameters
     catalogs: dict[str, ExtcatsCatalogModel]
 
     # Default behavior is to return the closest match, but can be switched to returning all
     closest_match: bool = True
 
     # Extcat config from context. Could add auhtorization
     require = ("extcats",)
 
-
-
     def post_init(self):
-
         # Select extcat
+        assert self.resource
         self.extcat_path = self.resource["extcats"]
 
         # dict for catalog query objects
         self.catq_objects = {}
-        self.debug = self.logger.verbose > 1
 
     def init_extcats_query(self, catalog, **kwargs) -> "CatalogQuery":
         """
         Return the extcats.CatalogQuery object corresponding to the desired
         catalog. Repeated requests to the same catalog will not cause new duplicated
         CatalogQuery instances to be created.
         """
@@ -146,42 +139,35 @@
 
         try:
             transient_ra = datapoint["body"]["ra"]
             transient_dec = datapoint["body"]["dec"]
         except KeyError:
             return UnitResult(code=DocumentCode.T2_MISSING_INFO)
 
-        if self.debug:
-            self.logger.debug(
-                "Transient position (ra, dec): {transient_ra:.4f}, {transient_dec:.4f} deg"
-            )
+        self.logger.debug(
+            "Transient position (ra, dec): {transient_ra:.4f}, {transient_dec:.4f} deg"
+        )
 
         # initialize the catalog quer(ies). Use instance variable to aviod duplicates
         out_dict: dict[str, Any] = {}
         for catalog, cat_opts in self.catalogs.items():
-
             src = None
-            if self.debug:
-                self.logger.debug(
-                    f"Loading catalog {catalog} using options: {str(cat_opts)}"
-                )
+            self.logger.debug(f"Loading catalog {catalog} using options: {cat_opts!s}")
             # find out how ra/dec are called in the catalog
             catq_kwargs = cat_opts.catq_kwargs
             if catq_kwargs is None:
                 ra_key, dec_key = "ra", "dec"
             else:
                 ra_key, dec_key = (
                     catq_kwargs.get("ra_key", "ra"),
                     catq_kwargs.get("dec_key", "dec"),
                 )
 
-
             # how do you want to support the catalog?
             if cat_opts.use == "extcats":
-
                 # get the catalog query object and do the query
                 catq = self.init_extcats_query(catalog, **cat_opts.catq_kwargs)
 
                 if self.closest_match:
                     src, dist = catq.findclosest(
                         transient_ra,
                         transient_dec,
@@ -209,26 +195,24 @@
                             src,
                             ra_key,
                             dec_key,
                         )
                         src["dist2transient"] = dist
 
             elif cat_opts.use == "catsHTM":
-
                 # catshtm needs coordinates in radians
                 transient_coords = SkyCoord(transient_ra, transient_dec, unit="deg")
                 srcs, colnames, colunits = self.catshtm.cone_search(
                     catalog,
                     transient_coords.ra.rad,
                     transient_coords.dec.rad,
                     cat_opts.rs_arcsec,
                 )
 
-                if len(srcs) > 0:   # JN: Always true if at least one match is done?
-
+                if len(srcs) > 0:  # JN: Always true if at least one match is done?
                     # format to astropy Table
                     srcs_tab = Table(asarray(srcs), names=colnames)
 
                     # convert distances to degrees (catsHTM stuff is in radians)
                     srcs_tab[ra_key] = degrees(srcs_tab[ra_key])
                     srcs_tab[dec_key] = degrees(srcs_tab[dec_key])
 
@@ -273,22 +257,18 @@
                     cat_opts.keys_to_append if cat_opts.keys_to_append else src.colnames
                 )
                 if cat_opts.use == "extcats":
                     keys_to_append.difference_update({"_id", "pos"})
                 # Always include dist2transient
                 keys_to_append.add("dist2transient")
 
-
-
                 out_dict[catalog] = []
 
-
                 # Can skip full loop if we know there are no errors or weird formats?
                 for one_src in src:
-
                     to_add = {}
                     for field in keys_to_append:
                         try:
                             val = one_src[field].tolist()
                         except AttributeError:
                             val = one_src[field]
                         except KeyError:
@@ -299,16 +279,15 @@
                 # To be backwards compatible we directly return dict if only one match was requested, a list otherwise
                 if self.closest_match:
                     # Above checks should have returned a dict with exactly one entry
                     assert len(out_dict[catalog]) == 1
                     out_dict[catalog] = out_dict[catalog][0]
 
             else:
-                if self.debug:
-                    self.logger.debug(
-                        f"no match found in catalog {catalog} within "
-                        f"{cat_opts.rs_arcsec:.2f} arcsec from transient"
-                    )
+                self.logger.debug(
+                    f"no match found in catalog {catalog} within "
+                    f"{cat_opts.rs_arcsec:.2f} arcsec from transient"
+                )
                 out_dict[catalog] = False
 
         # return the info as dictionary
         return out_dict
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2DigestRedshifts.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DigestRedshifts.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # File:                ampel/contrib/hu/t2/T2DigestRedshifts.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                06.06.2021
 # Last Modified Date:  19.10.2022
 # Last Modified By:    atownsend@physik.hu-berlin.de
 
-from typing import Any, Literal
 from collections.abc import Sequence
-from ampel.struct.UnitResult import UnitResult
+from typing import Any, Literal
 
-from ampel.types import UBson
+import numpy as np
+
+from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
 from ampel.enum.DocumentCode import DocumentCode
 from ampel.model.StateT2Dependency import StateT2Dependency
-from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
-from ampel.view.T2DocView import T2DocView
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
-import numpy as np
+from ampel.view.T2DocView import T2DocView
 
 
 class T2DigestRedshifts(AbsTiedLightCurveT2Unit):
     """
 
     Compare potential matches from different T2 units providing redshifts.
 
@@ -37,111 +38,108 @@
 
     """
 
     # Max redshift uncertainty category: 1-7
     # (where 7 is any, and 1 only nearby spectroscopic matches)
     max_redshift_category: int
 
-
     # Redshift estimates associated with each region ( only rough guideline!!! )
     category_precision: list[float] = [0.0003, 0.003, 0.01, 0.02, 0.04, 0.1, 0.3]
 
-
     # CatalogMatch(Local) results might be overriden,
     # for example if specialized catalog is being used
     # Each override dict is assumed to be built asmed to be built according to
     # "catalog_name" : {
     #                    "z_keyword": "redshift field in catalog",
     #                    "max_distance": "max arcsec in which to allow match,
     #                    "max_redshift": "max redshift to use",
     #                    "z_group": "which redshift group to assign to" }
     catalogmatch_override: None | dict[str, Any]
 
-
-
     # These are the units through which we look for redshifts
     # Which units should this be changed to
-    t2_dependency: Sequence[StateT2Dependency[Literal[
-        "T2CatalogMatch",
-        "T2LSPhotoZTap",
-        "T2CatalogMatchLocal",
-        "T2MatchBTS"
-        ]]]
-
-
-
-
-    def _get_lsphotoz_groupz(self, t2_res: dict[str, Any]) -> tuple[list[list[float]],list[list[float]]]:
+    t2_dependency: Sequence[
+        StateT2Dependency[
+            Literal[
+                "T2CatalogMatch", "T2LSPhotoZTap", "T2CatalogMatchLocal", "T2MatchBTS"
+            ]
+        ]
+    ]
+
+    def _get_lsphotoz_groupz(
+        self, t2_res: dict[str, Any]
+    ) -> tuple[list[list[float]], list[list[float]]]:
         """
         Parse output from T2LSPhotoZTap and investigate whether any matches fulfill group
         redshift criteria.
 
         Return:
         One list for each of the seven redshift cateogries
         """
 
         group_z: list[list[float]] = [[], [], [], [], [], [], []]
         group_dist: list[list[float]] = [[], [], [], [], [], [], []]
-        for lsname, lsdata in t2_res.items():
+        for lsdata in t2_res.values():
             if lsdata is None:
                 continue
 
             # Warning: all LS checks done with a 10" matching radius,
             # this is thus enforced (in case T2 run with larger radius)
-            if lsdata['dist2transient'] > 10:
-                self.logger.debug('No Digest redshift LS estimate.',
-                                  extra={'dist2transient': lsdata['dist2transient']})
+            if lsdata["dist2transient"] > 10:
+                self.logger.debug(
+                    "No Digest redshift LS estimate.",
+                    extra={"dist2transient": lsdata["dist2transient"]},
+                )
                 continue
 
             # First investigate LS spectroscopic redshift
-            if lsdata['z_spec'] is not None and lsdata['z_spec'] > -1:
-                if lsdata['z_spec'] < 0.03:
+            if lsdata["z_spec"] is not None and lsdata["z_spec"] > -1:
+                if lsdata["z_spec"] < 0.03:
                     # Group I
-                    group_z[0].append(lsdata['z_spec'])
-                    group_dist[0].append(lsdata['dist2transient'])
-                elif lsdata['z_spec'] < 0.15:
+                    group_z[0].append(lsdata["z_spec"])
+                    group_dist[0].append(lsdata["dist2transient"])
+                elif lsdata["z_spec"] < 0.15:
                     # Group II
-                    group_z[1].append(lsdata['z_spec'])
-                    group_dist[1].append(lsdata['dist2transient'])
-                elif lsdata['z_spec'] < 0.4:
+                    group_z[1].append(lsdata["z_spec"])
+                    group_dist[1].append(lsdata["dist2transient"])
+                elif lsdata["z_spec"] < 0.4:
                     # Group III
-                    group_z[2].append(lsdata['z_spec'])
-                    group_dist[2].append(lsdata['dist2transient'])
+                    group_z[2].append(lsdata["z_spec"])
+                    group_dist[2].append(lsdata["dist2transient"])
                 else:
                     # Group V
-                    group_z[4].append(lsdata['z_spec'])
-                    group_dist[4].append(lsdata['dist2transient'])
-            self.logger.debug('LS debug spec: %s yield %s'%(lsdata, group_z))
+                    group_z[4].append(lsdata["z_spec"])
+                    group_dist[4].append(lsdata["dist2transient"])
+            self.logger.debug(f"LS debug spec: {lsdata} yield {group_z}")
 
             # Now, photometric redshifts
-            if lsdata['z_phot_median'] is not None and lsdata['z_phot_median'] > -1:
-
-                if lsdata['z_phot_median'] < 0.1:
+            if lsdata["z_phot_median"] is not None and lsdata["z_phot_median"] > -1:
+                if lsdata["z_phot_median"] < 0.1:
                     # Group IV
-                    group_z[3].append(lsdata['z_phot_median'])
-                    group_dist[3].append(lsdata['dist2transient'])
-                elif lsdata['z_phot_median'] < 0.2:
+                    group_z[3].append(lsdata["z_phot_median"])
+                    group_dist[3].append(lsdata["dist2transient"])
+                elif lsdata["z_phot_median"] < 0.2:
                     # Group V
-                    group_z[4].append(lsdata['z_phot_median'])
-                    group_dist[4].append(lsdata['dist2transient'])
-                elif lsdata['z_phot_median'] < 0.4:
+                    group_z[4].append(lsdata["z_phot_median"])
+                    group_dist[4].append(lsdata["dist2transient"])
+                elif lsdata["z_phot_median"] < 0.4:
                     # Group VI
-                    group_z[5].append(lsdata['z_phot_median'])
-                    group_dist[5].append(lsdata['dist2transient'])
+                    group_z[5].append(lsdata["z_phot_median"])
+                    group_dist[5].append(lsdata["dist2transient"])
                 else:
                     # Group VII
-                    group_z[6].append(lsdata['z_phot_median'])
-                    group_dist[6].append(lsdata['dist2transient'])
-            self.logger.debug('LS debug phot: %s yield %s'%(lsdata, group_z))
+                    group_z[6].append(lsdata["z_phot_median"])
+                    group_dist[6].append(lsdata["dist2transient"])
+            self.logger.debug(f"LS debug phot: {lsdata} yield {group_z}")
 
         return group_z, group_dist
 
-
-
-    def _get_catalogmatch_groupz(self, t2_res: dict[str, Any]) -> tuple[list[list[float]],list[list[float]]]:
+    def _get_catalogmatch_groupz(
+        self, t2_res: dict[str, Any]
+    ) -> tuple[list[list[float]], list[list[float]]]:
         """
         Parse output from T2CatalogMatch.
 
         Made complicated as returns can be both single and lists.
 
 
         Return:
@@ -159,229 +157,240 @@
                 cat_match_list = cat_matches
             elif isinstance(cat_matches, tuple):
                 cat_match_list = list(cat_matches)
             else:
                 cat_match_list = [cat_matches]
 
             for cat_match in cat_match_list:
-
                 # All catalogs have different structure, so doing this individually
 
-                if cat_name == 'NEDz_extcats':
+                if cat_name == "NEDz_extcats":
                     # at some point: verify whether 0.03 was the NEDz_extcats cut.
-                    if cat_match['dist2transient'] < 2 and cat_match['z'] < 0.03:
-                        group_z[0].append(cat_match['z'])
-                        group_dist[0].append(cat_match['dist2transient'])
-                    elif cat_match['dist2transient'] < 20 and cat_match['z'] < 0.05:
-                        group_z[2].append(cat_match['z'])
-                        group_dist[2].append(cat_match['dist2transient'])
+                    if cat_match["dist2transient"] < 2 and cat_match["z"] < 0.03:
+                        group_z[0].append(cat_match["z"])
+                        group_dist[0].append(cat_match["dist2transient"])
+                    elif cat_match["dist2transient"] < 20 and cat_match["z"] < 0.05:
+                        group_z[2].append(cat_match["z"])
+                        group_dist[2].append(cat_match["dist2transient"])
                     else:
-                        group_z[3].append(cat_match['z'])
-                        group_dist[3].append(cat_match['dist2transient'])
+                        group_z[3].append(cat_match["z"])
+                        group_dist[3].append(cat_match["dist2transient"])
 
-                if cat_name == 'SDSS_spec':
                     # Implicit restriction as tests where done with this max matching radius
-                    if cat_match['dist2transient'] < 10:
-                        group_z[1].append(cat_match['z'])
-                        group_dist[1].append(cat_match['dist2transient'])
+
+                if cat_name == "SDSS_spec" and cat_match["dist2transient"] < 10:
+                    group_z[1].append(cat_match["z"])
+                    group_dist[1].append(cat_match["dist2transient"])
                 # Implicit restriction as tests where done with this max matching radius
-                if (cat_name == 'GLADEv23' and cat_match['dist2transient'] < 10
-                        and cat_match['z'] is not None):
-                    if cat_match['z'] < 0.05:
-                        group_z[2].append(cat_match['z'])
-                        group_dist[2].append(cat_match['dist2transient'])
+                if (
+                    cat_name == "GLADEv23"
+                    and cat_match["dist2transient"] < 10
+                    and cat_match["z"] is not None
+                ):
+                    if cat_match["z"] < 0.05:
+                        group_z[2].append(cat_match["z"])
+                        group_dist[2].append(cat_match["dist2transient"])
                     else:
-                        group_z[3].append(cat_match['z'])
-                        group_dist[3].append(cat_match['dist2transient'])
+                        group_z[3].append(cat_match["z"])
+                        group_dist[3].append(cat_match["dist2transient"])
 
-                if cat_name == 'LSPhotoZZou':
+                if cat_name == "LSPhotoZZou":
                     # Spec
-                    if cat_match['specz'] is not None and cat_match['specz'] > -0.1:
-                        if cat_match['specz'] < 0.15 and cat_match['dist2transient'] < 10:
-                            group_z[1].append(cat_match['specz'])
-                            group_dist[1].append(cat_match['dist2transient'])
-                        elif cat_match['specz'] < 0.2:
-                            group_z[2].append(cat_match['specz'])
-                            group_dist[2].append(cat_match['dist2transient'])
+                    if cat_match["specz"] is not None and cat_match["specz"] > -0.1:
+                        if (
+                            cat_match["specz"] < 0.15
+                            and cat_match["dist2transient"] < 10
+                        ):
+                            group_z[1].append(cat_match["specz"])
+                            group_dist[1].append(cat_match["dist2transient"])
+                        elif cat_match["specz"] < 0.2:
+                            group_z[2].append(cat_match["specz"])
+                            group_dist[2].append(cat_match["dist2transient"])
                         else:
-                            group_z[4].append(cat_match['specz'])
-                            group_dist[4].append(cat_match['dist2transient'])
+                            group_z[4].append(cat_match["specz"])
+                            group_dist[4].append(cat_match["dist2transient"])
 
                     # Photo-z
-                    if cat_match['photoz'] is not None and cat_match['photoz'] > -0.1:
-                        if cat_match['photoz'] < 0.1:
-                            group_z[3].append(cat_match['photoz'])
-                            group_dist[3].append(cat_match['dist2transient'])
-                        elif cat_match['photoz'] < 0.2:
-                            group_z[4].append(cat_match['photoz'])
-                            group_dist[4].append(cat_match['dist2transient'])
-                        elif cat_match['dist2transient'] < 20:
-                            group_z[5].append(cat_match['photoz'])
-                            group_dist[5].append(cat_match['dist2transient'])
+                    if cat_match["photoz"] is not None and cat_match["photoz"] > -0.1:
+                        if cat_match["photoz"] < 0.1:
+                            group_z[3].append(cat_match["photoz"])
+                            group_dist[3].append(cat_match["dist2transient"])
+                        elif cat_match["photoz"] < 0.2:
+                            group_z[4].append(cat_match["photoz"])
+                            group_dist[4].append(cat_match["dist2transient"])
+                        elif cat_match["dist2transient"] < 20:
+                            group_z[5].append(cat_match["photoz"])
+                            group_dist[5].append(cat_match["dist2transient"])
                         else:
-                            group_z[6].append(cat_match['photoz'])
-                            group_dist[6].append(cat_match['dist2transient'])
-
-                if cat_name == 'wiseScosPhotoz':
-                    if cat_match['zPhoto_Corr'] is not None and cat_match['zPhoto_Corr'] > -0.1:
-                        if cat_match['zPhoto_Corr'] < 0.2:
-                            group_z[4].append(cat_match['zPhoto_Corr'])
-                            group_dist[4].append(cat_match['dist2transient'])
-                        else:
-                            group_z[5].append(cat_match['zPhoto_Corr'])
-                            group_dist[5].append(cat_match['dist2transient'])
+                            group_z[6].append(cat_match["photoz"])
+                            group_dist[6].append(cat_match["dist2transient"])
 
+                if cat_name == "wiseScosPhotoz" and (
+                    cat_match["zPhoto_Corr"] is not None
+                    and cat_match["zPhoto_Corr"] > -0.1
+                ):
+                    if cat_match["zPhoto_Corr"] < 0.2:
+                        group_z[4].append(cat_match["zPhoto_Corr"])
+                        group_dist[4].append(cat_match["dist2transient"])
+                    else:
+                        group_z[5].append(cat_match["zPhoto_Corr"])
+                        group_dist[5].append(cat_match["dist2transient"])
 
-                if cat_name == 'twoMPZ':
+                if cat_name == "twoMPZ":
                     # Photoz
-                    if cat_match['zPhoto'] is not None and cat_match['zPhoto'] > -0.1:
-                        if cat_match['zPhoto'] < 0.03:
-                            group_z[2].append(cat_match['zPhoto'])
-                            group_dist[2].append(cat_match['dist2transient'])
+                    if cat_match["zPhoto"] is not None and cat_match["zPhoto"] > -0.1:
+                        if cat_match["zPhoto"] < 0.03:
+                            group_z[2].append(cat_match["zPhoto"])
+                            group_dist[2].append(cat_match["dist2transient"])
                         else:
-                            group_z[3].append(cat_match['zPhoto'])
-                            group_dist[3].append(cat_match['dist2transient'])
+                            group_z[3].append(cat_match["zPhoto"])
+                            group_dist[3].append(cat_match["dist2transient"])
                     # Specz
-                    if cat_match['zSpec'] is not None and cat_match['zSpec'] > -0.1:
-                        group_z[1].append(cat_match['zSpec'])
-                        group_dist[1].append(cat_match['dist2transient'])
-
-                if cat_name == 'PS1_photoz':
-                    ps1_z_phot = float(cat_match['z_phot'])/1000
-                    if cat_match['z_phot'] is not None and ps1_z_phot > -0.1:
+                    if cat_match["zSpec"] is not None and cat_match["zSpec"] > -0.1:
+                        group_z[1].append(cat_match["zSpec"])
+                        group_dist[1].append(cat_match["dist2transient"])
+
+                if cat_name == "PS1_photoz":
+                    ps1_z_phot = float(cat_match["z_phot"]) / 1000
+                    if cat_match["z_phot"] is not None and ps1_z_phot > -0.1:
                         if ps1_z_phot < 0.2:
                             group_z[3].append(ps1_z_phot)
-                            group_dist[3].append(cat_match['dist2transient'])
+                            group_dist[3].append(cat_match["dist2transient"])
                         elif ps1_z_phot < 0.4:
                             group_z[4].append(ps1_z_phot)
-                            group_dist[4].append(cat_match['dist2transient'])
-                        elif cat_match['dist2transient'] < 20:
+                            group_dist[4].append(cat_match["dist2transient"])
+                        elif cat_match["dist2transient"] < 20:
                             group_z[5].append(ps1_z_phot)
-                            group_dist[5].append(cat_match['dist2transient'])
+                            group_dist[5].append(cat_match["dist2transient"])
                         else:
                             group_z[6].append(ps1_z_phot)
-                            group_dist[6].append(cat_match['dist2transient'])
-                
-                # Implicit restriction as tests where done with this max matching radius
-                if cat_name == 'NEDz' and cat_match['dist2transient'] < 10:
-                    if cat_match['z'] < 0.4:
-                        group_z[2].append(cat_match['z'])
-                        group_dist[2].append(cat_match['dist2transient'])
+                            group_dist[6].append(cat_match["dist2transient"])
 
+                # Implicit restriction as tests where done with this max matching radius
+                if (
+                    cat_name == "NEDz"
+                    and cat_match["dist2transient"] < 10
+                    and cat_match["z"] < 0.4
+                ):
+                    group_z[2].append(cat_match["z"])
+                    group_dist[2].append(cat_match["dist2transient"])
 
                 # Also check for manual override
                 if self.catalogmatch_override:
                     for or_catname, or_catdict in self.catalogmatch_override.items():
                         if or_catname == cat_name:
                             try:
                                 cat_z = float(cat_match[or_catdict["z_keyword"]])
-                                if (float(cat_match['dist2transient']) < or_catdict["max_distance"]
-                                        and cat_z < or_catdict["max_redshift"]):
-                                    group_z[or_catdict["z_group"]-1].append(cat_z)
+                                if (
+                                    float(cat_match["dist2transient"])
+                                    < or_catdict["max_distance"]
+                                    and cat_z < or_catdict["max_redshift"]
+                                ):
+                                    group_z[or_catdict["z_group"] - 1].append(cat_z)
                             except ValueError:
-                                self.logger.info('Cannot parse z', extra={'catdict':cat_match})
-
+                                self.logger.info(
+                                    "Cannot parse z", extra={"catdict": cat_match}
+                                )
 
         return group_z, group_dist
 
-
-
-    def _get_matchbts_groupz(self, t2_res: dict[str, Any])->list[list[float]]:
+    def _get_matchbts_groupz(self, t2_res: dict[str, Any]) -> list[list[float]]:
         """
-        Parse output from T2MatachBTS.
+        Parse output from T2MatchBTS.
 
         Any transient with a redshift with two decimals (from SN template matching) is put in Group II,
         those with more (from host, high-res spec) are put into Group I.
 
         Return:
         One list for each of the seven redshift cateogries
         """
 
         group_z: list[list[float]] = [[], [], [], [], [], [], []]
 
-        if isinstance(bts_redshift := t2_res.get("bts_redshift"), str) and bts_redshift != "-":
+        if (
+            isinstance(bts_redshift := t2_res.get("bts_redshift"), str)
+            and bts_redshift != "-"
+        ):
             # BTS redshifts are stored as strings. Crude way to get to redshift precision for evaluation:
             # Take decimal part, remove initial zeroes and cound digits
             decimals = len(bts_redshift.split(".")[1].lstrip("0"))
             z = float(bts_redshift)
 
             if decimals > 2:
                 group_z[0].append(z)
             else:
                 group_z[1].append(z)
 
-        self.logger.debug(' bts match yield %s'%(group_z))
+        self.logger.debug(" bts match yield %s" % (group_z))
 
         return group_z
 
-
-
-
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self,
-        light_curve: LightCurve, t2_views: Sequence[T2DocView]
+    def process(
+        self, light_curve: LightCurve, t2_views: Sequence[T2DocView]
     ) -> UBson | UnitResult:
         """
 
-            Parse t2_views from catalogs that were part of the redshift studies.
-            Return these together with a "best estimate" - ampel_z
+        Parse t2_views from catalogs that were part of the redshift studies.
+        Return these together with a "best estimate" - ampel_z
 
         """
 
-        if not t2_views: # Should not happen actually, T2Processor catches that case
+        if not t2_views:  # Should not happen actually, T2Processor catches that case
             self.logger.error("Missing tied t2 views")
             return UnitResult(code=DocumentCode.T2_MISSING_INFO)
 
-
         # Loop through all potential T2s with redshift information.
         # Each should return an array of arrays, corresponding to redshift maches
         # found in each category. These will be added to sn redshifts
         group_redshifts: list[list[float]] = [[], [], [], [], [], [], []]
         group_distances: list[list[float]] = [[], [], [], [], [], [], []]
 
-
-		# Loop through t2_views and collect information.
+        # Loop through t2_views and collect information.
         for t2_view in t2_views:
-
-            self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
+            self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
             t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
             # v0.8:
-			#t2_res =  t2_view.get_data()
+            # t2_res =  t2_view.get_data()
 
-            if t2_view.unit == 'T2LSPhotoZTap':
+            if t2_view.unit == "T2LSPhotoZTap":
                 new_zs, new_dists = self._get_lsphotoz_groupz(t2_res)
-            elif t2_view.unit == 'T2CatalogMatch' or t2_view.unit == 'T2CatalogMatchLocal':
+            elif t2_view.unit in {"T2CatalogMatch", "T2CatalogMatchLocal"}:
                 new_zs, new_dists = self._get_catalogmatch_groupz(t2_res)
-            elif t2_view.unit == 'T2MatchBTS':
+            elif t2_view.unit == "T2MatchBTS":
                 new_zs = self._get_matchbts_groupz(t2_res)
             else:
-                self.logger.error("No instructions for dealing with {}".format(t2_view.unit))
+                self.logger.error(f"No instructions for dealing with {t2_view.unit}")
                 return UnitResult(code=DocumentCode.T2_MISSING_INFO)
 
             for k in range(7):
                 if len(new_zs[k]) > 0:
                     group_redshifts[k].extend(new_zs[k])
                 if len(new_dists[k]) > 0:
                     group_distances[k].extend(new_dists[k])
-            self.logger.debug('group_z after %s: %s'%(t2_view.unit, group_redshifts))
-
+            self.logger.debug(f"group_z after {t2_view.unit}: {group_redshifts}")
 
         # Check for best match
-        t2_output: dict[str,UBson] = {'group_zs': group_redshifts, 'group_dists': group_distances}
+        t2_output: dict[str, UBson] = {
+            "group_zs": group_redshifts,
+            "group_dists": group_distances,
+        }
         for k in range(7):
-            if (k+1) > self.max_redshift_category:
+            if (k + 1) > self.max_redshift_category:
                 # No matches with sufficient precision
                 break
             if len(group_redshifts[k]) > 0:
-                t2_output['ampel_z'] = float(np.mean(group_redshifts[k]))
-                t2_output['group_z_precision'] = self.category_precision[k]
-                t2_output['group_z_nbr'] = k+1
-                t2_output['ampel_dist'] = float(np.mean(group_distances[k]))
+                t2_output["ampel_z"] = float(np.mean(group_redshifts[k]))
+                t2_output["group_z_precision"] = self.category_precision[k]
+                t2_output["group_z_nbr"] = k + 1
+                t2_output["ampel_dist"] = float(
+                    np.mean(group_distances[k])
+                )  # distance transient to matched z sources NOT TO EARTH
                 # We then do *not* look for higher group (more uncertain) matches
                 break
         if self.catalogmatch_override:
             t2_output["AmpelZ-Warning"] = "Override catalog in use."
 
-        self.logger.debug('digest redshift: %s'%(t2_output))
+        self.logger.debug("digest redshift: %s" % (t2_output))
         return t2_output
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,63 @@
 # File              : ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
 # License           : BSD-3-Clause
 # Author            : jnordin@physik.hu-berlin.de
 # Date              : 12.04.2022
 # Last Modified Date: 12.04.2022
 # Last Modified By  : jnordin@physik.hu-berlin.de
 
-from typing import Sequence, Union, TypedDict, cast
+from typing import TypedDict, cast
+
 import numpy as np
 
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.content.DataPoint import DataPoint
 from ampel.abstract.AbsPointT2Unit import AbsPointT2Unit
+from ampel.content.DataPoint import DataPoint
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
+
 
 class QuantileEntry(TypedDict):
     w: float
     q: list[str]
 
+
 class RedshiftSamples(TypedDict):
     z_source: str
     host_sep: float
     galaxy_color: float | None
     z_samples: list[float]
     z_weights: list[float]
 
+
 # Quantile subselections and weights
 # Dictionaries of redhift weights together with the accompaning quantile entries.
 QUANT_WEIGHTS: dict[int, list[QuantileEntry]] = {
     3: [
-        {'w':0.2, 'q': ['000', '010', '020', '030', '040']},
-        {'w':0.6, 'q': ['030', '040', '050', '060', '070']},  # Will always be 050?
-        {'w':0.2, 'q': ['060', '070', '080', '090', '100']},
-        ],
+        {"w": 0.2, "q": ["000", "010", "020", "030", "040"]},
+        {"w": 0.6, "q": ["030", "040", "050", "060", "070"]},  # Will always be 050?
+        {"w": 0.2, "q": ["060", "070", "080", "090", "100"]},
+    ],
     5: [
-        {'w':0.2, 'q': ['000', '010', '020']},
-        {'w':0.2, 'q': ['020', '030', '040']},
-        {'w':0.2, 'q': ['060', '070', '080']},
-        {'w':0.2, 'q': ['040', '050', '060']},
-        {'w':0.2, 'q': ['080', '090', '100']},
-        ]
-    }
+        {"w": 0.2, "q": ["000", "010", "020"]},
+        {"w": 0.2, "q": ["020", "030", "040"]},
+        {"w": 0.2, "q": ["060", "070", "080"]},
+        {"w": 0.2, "q": ["040", "050", "060"]},
+        {"w": 0.2, "q": ["080", "090", "100"]},
+    ],
+}
 
 # For the gaussian case, which sigma deviations should be used for
 # each number of samples?
-NORM_SIGMAS: dict[int,list[float]] = {
+NORM_SIGMAS: dict[int, list[float]] = {
     1: [0],
-    3: [-1.5,0,1.5],
-    5: [-2.,-1.,0,1.,2.],
+    3: [-1.5, 0, 1.5],
+    5: [-2.0, -1.0, 0, 1.0, 2.0],
 }
 
+
 class T2ElasticcRedshiftSampler(AbsPointT2Unit):
     """
     Parse the elasticc diaSource host information and
     returns a list of redshifts and weights.
 
     Note 1:
     Elasticc alerts contain both quantiles and mean value + error.
@@ -107,70 +112,79 @@
     # Check for final/spectroscopic redshifts, and use if present
     # Usually would be the case, but for testing we might not want to
     use_final_z: bool = False
 
     # Which bands should be used to estimate the galaxy color?
     # Should these be corrected for MW absorption?
     # Quick trial did not find a strong correlation.
-    use_galcol: list[str] = ['u','i']
+    use_galcol: list[str] = ["u", "i"]
 
     # Can potentially have different metrics for how to choose host galaxy.
     # (could even involve spanning the joint redshifts according to location prob)
     # minDDLR: Select the host with smallest DDLR
-    #host_selection: Literal['minDDLR'] = 'minDDLR'
-
+    # host_selection: Literal['minDDLR'] = 'minDDLR'
 
     def get_hostprob(self, hostinfo: dict) -> tuple[float, float, float]:
         """
         Use the information from the alert info to guess relative prob
         for the two different host galaxies.
 
         To calculate delta/DLR one would need, except SN and galaxy position,
         some estimate on size, orientation and ellipticity (e.g. moments).
         As these are not contained in the latest test alerts we will for know
         choose the host with the smallest separation / radius.
 
         """
 
         # Does sqradius mean what I believe?
-        if hostinfo.get('hostgal_sqradius',-99)>=0:
-            hostgal_sigsep = hostinfo['hostgal_snsep'] / np.sqrt(hostinfo['hostgal_sqradius'])
+        if hostinfo.get("hostgal_sqradius", -99) >= 0:
+            hostgal_sigsep = hostinfo["hostgal_snsep"] / np.sqrt(
+                hostinfo["hostgal_sqradius"]
+            )
         else:
-            hostgal_sigsep = -99.
-        if hostinfo.get('hostgal2_sqradius',-99)>=0:
-            hostgal2_sigsep = hostinfo['hostgal2_snsep'] / np.sqrt(hostinfo['hostgal2_sqradius'])
+            hostgal_sigsep = -99.0
+        if hostinfo.get("hostgal2_sqradius", -99) >= 0:
+            hostgal2_sigsep = hostinfo["hostgal2_snsep"] / np.sqrt(
+                hostinfo["hostgal2_sqradius"]
+            )
         else:
-            hostgal2_sigsep = -99.
-        self.logger.debug('hostselect', extra={'hostgal_sigsep':hostgal_sigsep,
-                                              'hostgal2_sigsep':hostgal2_sigsep})
+            hostgal2_sigsep = -99.0
+        self.logger.debug(
+            "hostselect",
+            extra={
+                "hostgal_sigsep": hostgal_sigsep,
+                "hostgal2_sigsep": hostgal2_sigsep,
+            },
+        )
 
         # SNsep can be exactly zero.
-        if hostinfo.get('hostgal_snsep',-99)>=0 and hostinfo.get('hostgal2_snsep',-99)<0:
+        if (
+            hostinfo.get("hostgal_snsep", -99) >= 0
+            and hostinfo.get("hostgal2_snsep", -99) < 0
+        ):
             # The easy case, only have first galaxy
-            return (1.0, 0.0, hostinfo['hostgal_snsep'])
-        elif hostinfo.get('hostgal_snsep',-99)<0 and hostinfo.get('hostgal2_snsep',-99)<0:
+            return (1.0, 0.0, hostinfo["hostgal_snsep"])
+        if (
+            hostinfo.get("hostgal_snsep", -99) < 0
+            and hostinfo.get("hostgal2_snsep", -99) < 0
+        ):
             # "Hostless" - if these exist
-            self.logger.debug('Hostless')
-            return (0.0, 0.0, -99.)
-
+            self.logger.debug("Hostless")
+            return (0.0, 0.0, -99.0)
 
         # In principle one could calculate relative weights based on this sigma
         # distances, but skipping for now.
-        if hostgal_sigsep<hostgal2_sigsep:
-            return (1.0, 0., hostinfo['hostgal_snsep'])
-        else:
-            return (0.0, 1.0, hostinfo['hostgal2_snsep'])
-
-
-
+        if hostgal_sigsep < hostgal2_sigsep:
+            return (1.0, 0.0, hostinfo["hostgal_snsep"])
+        return (0.0, 1.0, hostinfo["hostgal2_snsep"])
 
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self, datapoint: DataPoint) -> Union[UBson, UnitResult]:
+    def process(self, datapoint: DataPoint) -> UBson | UnitResult:
         """
 
         Parses the provided datapoint for information regarding
         which redshifts should be sampled (and weighted).
 
 
         Parameters
@@ -178,99 +192,125 @@
         datapoint: "DataPoint" instance.
 
         Returns
         -------
         dict
         """
 
-        dp = datapoint['body']
+        dp = datapoint["body"]
 
         # Eventually we assume that we can use the directive ingest setting
         # to make sure that we here get the diaSource object.
 
         # Guess at relative host galaxy probabilities
         (probH1, probH2, host_sep) = self.get_hostprob(dp)
 
         # Depending on the above relative probabilities, choose which redshifts
         z, dz, zsource, galcol = 0.0, 0.0, None, None
 
         # Final (simulated) data available and used?
         if self.use_final_z:
             # TODO: implement galaxy color determination - but not using final z anyway?
-            if dp.get('z_final',-1)>0:
-                z, dz, zsource = dp.get('z_final',-1), dp.get('z_final_err', 0), 'Z_FINAL'
-            elif dp.get('redshift_helio',-1)>0:
-                z, dz, zsource = dp.get('redshift_helio',-1), dp.get('redshift_helio_err', 0), 'REDSHIFT_HELIO'
+            if dp.get("z_final", -1) > 0:
+                z, dz, zsource = (
+                    dp.get("z_final", -1),
+                    dp.get("z_final_err", 0),
+                    "Z_FINAL",
+                )
+            elif dp.get("redshift_helio", -1) > 0:
+                z, dz, zsource = (
+                    dp.get("redshift_helio", -1),
+                    dp.get("redshift_helio_err", 0),
+                    "REDSHIFT_HELIO",
+                )
 
         # Both sources need to be weighted together
-        if zsource is None and probH1>0 and probH2>0:
+        if zsource is None and probH1 > 0 and probH2 > 0:
             raise NotImplementedError
 
         # Get spectroscopiy host redshift if available
-        if zsource is None and probH1>0 and dp.get('hostgal_zspec',-1)>0:
-            z, dz, zsource = dp.get('hostgal_zspec',-1), dp.get('hostgal_zspec_err',0), 'HOSTGAL_ZSPEC'
-        if zsource is None and probH2>0 and dp.get('hostgal2_zspec',-1)>0:
-            z, dz, zsource = dp.get('hostgal2_zspec',-1), dp.get('hostgal2_zspec_err',0), 'HOSTGAL2_ZSPEC'
+        if zsource is None and probH1 > 0 and dp.get("hostgal_zspec", -1) > 0:
+            z, dz, zsource = (
+                dp.get("hostgal_zspec", -1),
+                dp.get("hostgal_zspec_err", 0),
+                "HOSTGAL_ZSPEC",
+            )
+        if zsource is None and probH2 > 0 and dp.get("hostgal2_zspec", -1) > 0:
+            z, dz, zsource = (
+                dp.get("hostgal2_zspec", -1),
+                dp.get("hostgal2_zspec_err", 0),
+                "HOSTGAL2_ZSPEC",
+            )
 
         # Get galaxy color for most likely host
         # Hostless events will get prefix hostgal2, but if statement should fail
         prefix = "hostgal_mag_" if probH1 > 0 else "hostgal2_mag_"
-        if ( (bluemag:= dp.get(prefix+self.use_galcol[0], 99)) <90 and
-                (redmag:= dp.get(prefix+self.use_galcol[1], 99)) <90  ):
-                galcol = bluemag-redmag
+        if (bluemag := dp.get(prefix + self.use_galcol[0], 99)) < 90 and (
+            redmag := dp.get(prefix + self.use_galcol[1], 99)
+        ) < 90:
+            galcol = bluemag - redmag
 
         # Finish up gaussian case
         if zsource is not None:
             # Calculate weights
             pulls = NORM_SIGMAS[self.nbr_samples]
-            weights = np.exp(-0.5 * np.array(pulls)**2) / np.sqrt(2)
+            weights = np.exp(-0.5 * np.array(pulls) ** 2) / np.sqrt(2)
             weights /= np.sum(weights)
             t2_output: RedshiftSamples = {
                 "z_source": zsource,
                 "host_sep": host_sep,
                 "galaxy_color": galcol,
                 "z_weights": list(weights),
-                "z_samples": [z + p*dz for p in pulls]
+                "z_samples": [z + p * dz for p in pulls],
             }
 
             return cast(UBson, t2_output)
 
         # Extract values from photo-z quantiles
         # (assuming these always exist)
         # Final cases should be the hostless (default)
-        if probH1>0 or probH2>0:
-
-
+        if probH1 > 0 or probH2 > 0:
             t2_output = {
                 "z_source": "HOSTGAL_ZQUANT" if probH1 > 0 else "HOSTGAL2_ZQUANT",
                 "host_sep": host_sep,
                 "galaxy_color": galcol,
                 "z_samples": [],
-                "z_weights": []
+                "z_weights": [],
             }
-            prefix = "hostgal_zphot_q" if t2_output["z_source"] == "HOSTGAL_ZQUANT" else "hostgal2_zphot_q"
+            prefix = (
+                "hostgal_zphot_q"
+                if t2_output["z_source"] == "HOSTGAL_ZQUANT"
+                else "hostgal2_zphot_q"
+            )
             # Get some redshifts
-            if self.nbr_samples==1:
+            if self.nbr_samples == 1:
                 t2_output["z_samples"] = [dp.get(f"{prefix}050", -1)]
                 t2_output["z_weights"] = [1.0]
-            if self.nbr_samples==3 or self.nbr_samples==5:
+            if self.nbr_samples in (3, 5):
                 t2_output["z_samples"], t2_output["z_weights"] = [], []
                 for weight_quantiles in QUANT_WEIGHTS[self.nbr_samples]:
-                    weight = weight_quantiles['w']
-                    quantiles = weight_quantiles['q']
-                    t2_output["z_samples"].append( np.mean( [qv
-                                for q in quantiles if (qv := dp.get(prefix+q,-9))>-9] ) ) # -9 seems to be null
+                    weight = weight_quantiles["w"]
+                    quantiles = weight_quantiles["q"]
+                    t2_output["z_samples"].append(
+                        np.mean(
+                            [
+                                qv
+                                for q in quantiles
+                                if (qv := dp.get(prefix + q, -9)) is not None
+                                and qv > -9
+                            ]
+                        )
+                    )  # -9 seems to be null
                     t2_output["z_weights"].append(weight)
 
-
             return cast(UBson, t2_output)
 
         # Only left with output dict for defult/hostless SNe
         t2_output = {
             "z_source": "default",
             "host_sep": np.nan,
             "galaxy_color": None,
-		    "z_samples": self.default_zs,
+            "z_samples": self.default_zs,
             "z_weights": self.default_weights,
         }
 
         return cast(UBson, t2_output)
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2FastDecliner.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2FastDecliner.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 # File:                ampel/contrib/hu/t2/T2FastDecliner.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                28.06.2022
 # Last Modified Date:  26.09.2022
 # Last Modified By:    Jakob Nordin <jnordin@physik.hu-berlin.de>
 
-from astropy.table import Table
-from typing import Any, TYPE_CHECKING
-from ampel.types import UBson
 from ampel.abstract.AbsLightCurveT2Unit import AbsLightCurveT2Unit
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 
 
 class T2FastDecliner(AbsLightCurveT2Unit):
     """
     Determine decline rate in two last obs.
     Check whether above some limit.
@@ -27,35 +25,38 @@
 
     :return: dict, decline rate in each filter and
             bool: fast_decliner
     """
 
     min_declinerate: float = 0.1
     min_trange: float = 0.1
-    max_trange: float = 2.
+    max_trange: float = 2.0
     filter_keys: dict[str, str] = {"1": "g", "2": "R"}
 
     def process(self, light_curve: LightCurve) -> UBson | UnitResult:
-
         # For each filter, check datapoints for latest datapoints
-        t2_output: dict[str,UBson] = {'fast_decliner': False}
+        t2_output: dict[str, UBson] = {"fast_decliner": False}
         for filt_id, filt_name in self.filter_keys.items():
-            pps = light_curve.get_ntuples( ["jd", "magpsf", "sigmapsf"],
-                 filters = [
+            pps = light_curve.get_ntuples(
+                ["jd", "magpsf", "sigmapsf"],
+                filters=[
                     {"attribute": "fid", "operator": "==", "value": int(filt_id)},
-                ]
+                ],
             )
-            if pps is None or len(pps)<2:
+            if pps is None or len(pps) < 2:
                 continue
             # Simple diffs of two most resent observations
             pps = sorted(pps, key=lambda d: d[0])
             delta_t = pps[-1][0] - pps[-2][0]
             delta_mag = pps[-1][1] - pps[-2][1]
             decline_rate = delta_mag / delta_t
 
             # Create output structure, annotating if lc "fast declining"
-            t2_output[filt_name] = {'delta_t': delta_t, 'decline_rate': decline_rate}
-            if (delta_t>self.min_trange and delta_t<self.max_trange and
-                    decline_rate>self.min_declinerate):
-                t2_output['fast_decliner'] = True
+            t2_output[filt_name] = {"delta_t": delta_t, "decline_rate": decline_rate}
+            if (
+                delta_t > self.min_trange
+                and delta_t < self.max_trange
+                and decline_rate > self.min_declinerate
+            ):
+                t2_output["fast_decliner"] = True
 
         return t2_output
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2GetLensSNParameters.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2GetLensSNParameters.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,118 +4,206 @@
 # License           : BSD-3-Clause
 # Author            : alice.townsend@physik.hu-berlin.de
 # Date              : 22.11.2021
 # Last Modified Date: 19.10.2022
 # Last Modified By  : alice.townsend@physik.hu-berlin.de
 
 
+from bisect import bisect_left
+
 import numpy as np
 from astropy.table import Table
+
 from ampel.contrib.hu.t2.T2RunSncosmo import T2RunSncosmo
-from bisect import bisect_left
+
 
 class T2GetLensSNParameters(T2RunSncosmo):
     unc: float
 
     def _get_fit_metrics(self, sncosmo_result, sncosmo_table, sncosmo_model) -> dict:
-        #-------------------------------- Overriden method -----------------------------#
-        lc_metrics = super()._get_fit_metrics(sncosmo_result, sncosmo_table, sncosmo_model)
+        # -------------------------------- Overriden method -----------------------------#
+        lc_metrics = super()._get_fit_metrics(
+            sncosmo_result, sncosmo_table, sncosmo_model
+        )
         # Record the closest detection to peak in each band
-        t0 = sncosmo_model.get('t0') # get time at peak of light curve
-        sncosmo_table.add_column('temporary', name='epoch', index = 0) # add column with temp values for epoch
-        sncosmo_table.sort(['time']) # sort data chronologically
-        
+        t0 = sncosmo_model.get("t0")  # get time at peak of light curve
+        sncosmo_table.add_column(
+            "temporary", name="epoch", index=0
+        )  # add column with temp values for epoch
+        sncosmo_table.sort(["time"])  # sort data chronologically
+
         def take_closest(myList, myNumber):
-            '''
+            """
             Assumes myList is sorted. Returns closest value to myNumber.
             If two numbers are equally close, return the smallest number.
-            '''
+            """
             pos = bisect_left(myList, myNumber)
             if pos == 0:
                 return myList[0]
             if pos == len(myList):
                 return myList[-1]
             before = myList[pos - 1]
             after = myList[pos]
             if after - myNumber < myNumber - before:
                 return after
-            else:
-                return before
-        
-        for band in np.unique(sncosmo_table['band']):
-            table_name = str(band) + 'cut'
-            globals()[table_name] = Table(sncosmo_table[0:0]) # create empty table for each band
-            band_table = sncosmo_table[(sncosmo_table['band'] == band)] # split data into different bands
-            time_minus7 = take_closest(band_table['time'], t0 - 7) # find closest time to t0-7 days in each band
+            return before
+
+        for band in np.unique(sncosmo_table["band"]):
+            table_name = str(band) + "cut"
+            globals()[table_name] = Table(
+                sncosmo_table[0:0]
+            )  # create empty table for each band
+            band_table = sncosmo_table[
+                (sncosmo_table["band"] == band)
+            ]  # split data into different bands
+            time_minus7 = take_closest(
+                band_table["time"], t0 - 7
+            )  # find closest time to t0-7 days in each band
             if (t0 - 7 - self.unc) <= time_minus7 <= (t0 - 7 + self.unc):
-                band_table['epoch'][np.where(band_table['time'] == time_minus7)] = 'minus7'
-                for row in band_table[np.where(band_table['time'] == time_minus7)]:  # iterate over temporary table that is a subset of data  
+                band_table["epoch"][
+                    np.where(band_table["time"] == time_minus7)
+                ] = "minus7"
+                for row in band_table[
+                    np.where(band_table["time"] == time_minus7)
+                ]:  # iterate over temporary table that is a subset of data
                     globals()[table_name].add_row(row)
-            time_closest = take_closest(band_table['time'], t0) # find closest time to peak in each band
+            time_closest = take_closest(
+                band_table["time"], t0
+            )  # find closest time to peak in each band
             if (t0 - self.unc) <= time_closest <= (t0 + self.unc):
-                band_table['epoch'][np.where(band_table['time'] == time_closest)] = 't0'
-                for row in band_table[np.where(band_table['time'] == time_closest)]:  # iterate over temporary table that is a subset of data  
+                band_table["epoch"][np.where(band_table["time"] == time_closest)] = "t0"
+                for row in band_table[
+                    np.where(band_table["time"] == time_closest)
+                ]:  # iterate over temporary table that is a subset of data
                     globals()[table_name].add_row(row)
-            time_plus7 = take_closest(band_table['time'], t0 + 7) # find closest time to t0+7 days in each band
+            time_plus7 = take_closest(
+                band_table["time"], t0 + 7
+            )  # find closest time to t0+7 days in each band
             if (t0 + 7 - self.unc) <= time_plus7 <= (t0 + 7 + self.unc):
-                band_table['epoch'][np.where(band_table['time'] == time_plus7)] = 'plus7'
-                for row in band_table[np.where(band_table['time'] == time_plus7)]:  # iterate over temporary table that is a subset of data  
+                band_table["epoch"][
+                    np.where(band_table["time"] == time_plus7)
+                ] = "plus7"
+                for row in band_table[
+                    np.where(band_table["time"] == time_plus7)
+                ]:  # iterate over temporary table that is a subset of data
                     globals()[table_name].add_row(row)
 
         # Calculate the colour at different epochs
         def calculate_colour_peak(band1, band2, epoch):
-            '''
+            """
             Calculate the colour from two different bands of a user's choosing.
             Bluer colour is band1.
             epoch is the epoch within which we are searching (i.e. t0, minus7, or plus7).
-            '''
-            band1_table = str(band1) + 'cut'
-            band2_table = str(band2) + 'cut'
-            if band1 not in sncosmo_table['band'] or band2 not in sncosmo_table['band']:
+            """
+            band1_table = str(band1) + "cut"
+            band2_table = str(band2) + "cut"
+            if band1 not in sncosmo_table["band"] or band2 not in sncosmo_table["band"]:
                 return None, None
-            elif epoch not in globals()[band1_table]['epoch'] or epoch not in globals()[band2_table]['epoch']:
+            if (
+                epoch not in globals()[band1_table]["epoch"]
+                or epoch not in globals()[band2_table]["epoch"]
+            ):
                 return None, None
-            else:
-                colour = -2.5 * np.log10(globals()[band1_table][np.where(globals()[band1_table]['epoch'] == epoch)]['flux']
-                                 / globals()[band2_table][np.where(globals()[band2_table]['epoch'] == epoch)]['flux'])
-                unc1 = 2.5 * 0.434 * (globals()[band1_table][np.where(globals()[band1_table]['epoch'] == epoch)]['fluxerr']
-                              /globals()[band1_table][np.where(globals()[band1_table]['epoch'] == epoch)]['flux'])
-                unc2 = 2.5 * 0.434 * (globals()[band2_table][np.where(globals()[band2_table]['epoch'] == epoch)]['fluxerr']
-                              /globals()[band2_table][np.where(globals()[band2_table]['epoch'] == epoch)]['flux'])
-                unc = (unc1**2 + unc2**2)**0.5
-                return colour.data[0], unc.data[0]
-        
-        lc_metrics['r_i_colour_peak'], lc_metrics['r_i_colour_peak_err'] = calculate_colour_peak('ztfr', 'ztfi', 't0')
-        lc_metrics['r_i_colour_plus7'], lc_metrics['r_i_colour_plus7_err'] = calculate_colour_peak('ztfr', 'ztfi', 'plus7')
-        lc_metrics['r_i_colour_minus7'], lc_metrics['r_i_colour_minus7_err'] = calculate_colour_peak('ztfr', 'ztfi', 'minus7')
-        lc_metrics['g_r_colour_peak'], lc_metrics['g_r_colour_peak_err']  = calculate_colour_peak('ztfg', 'ztfr', 't0')
-        lc_metrics['g_r_colour_plus7'], lc_metrics['g_r_colour_plus7_err'] = calculate_colour_peak('ztfg', 'ztfr', 'plus7')
-        lc_metrics['g_r_colour_minus7'], lc_metrics['g_r_colour_minus7_err'] = calculate_colour_peak('ztfg', 'ztfr', 'minus7') 
-        lc_metrics['g_i_colour_peak'], lc_metrics['g_i_colour_peak_err']  = calculate_colour_peak('ztfg', 'ztfi', 't0')
-        lc_metrics['g_i_colour_plus7'], lc_metrics['g_i_colour_plus7_err'] = calculate_colour_peak('ztfg', 'ztfi', 'plus7')
-        lc_metrics['g_i_colour_minus7'], lc_metrics['g_i_colour_minus7_err'] = calculate_colour_peak('ztfg', 'ztfi', 'minus7')        
+            colour = -2.5 * np.log10(
+                globals()[band1_table][
+                    np.where(globals()[band1_table]["epoch"] == epoch)
+                ]["flux"]
+                / globals()[band2_table][
+                    np.where(globals()[band2_table]["epoch"] == epoch)
+                ]["flux"]
+            )
+            unc1 = (
+                2.5
+                * 0.434
+                * (
+                    globals()[band1_table][
+                        np.where(globals()[band1_table]["epoch"] == epoch)
+                    ]["fluxerr"]
+                    / globals()[band1_table][
+                        np.where(globals()[band1_table]["epoch"] == epoch)
+                    ]["flux"]
+                )
+            )
+            unc2 = (
+                2.5
+                * 0.434
+                * (
+                    globals()[band2_table][
+                        np.where(globals()[band2_table]["epoch"] == epoch)
+                    ]["fluxerr"]
+                    / globals()[band2_table][
+                        np.where(globals()[band2_table]["epoch"] == epoch)
+                    ]["flux"]
+                )
+            )
+            unc = (unc1**2 + unc2**2) ** 0.5
+            return colour.data[0], unc.data[0]
+
+        (
+            lc_metrics["r_i_colour_peak"],
+            lc_metrics["r_i_colour_peak_err"],
+        ) = calculate_colour_peak("ztfr", "ztfi", "t0")
+        (
+            lc_metrics["r_i_colour_plus7"],
+            lc_metrics["r_i_colour_plus7_err"],
+        ) = calculate_colour_peak("ztfr", "ztfi", "plus7")
+        (
+            lc_metrics["r_i_colour_minus7"],
+            lc_metrics["r_i_colour_minus7_err"],
+        ) = calculate_colour_peak("ztfr", "ztfi", "minus7")
+        (
+            lc_metrics["g_r_colour_peak"],
+            lc_metrics["g_r_colour_peak_err"],
+        ) = calculate_colour_peak("ztfg", "ztfr", "t0")
+        (
+            lc_metrics["g_r_colour_plus7"],
+            lc_metrics["g_r_colour_plus7_err"],
+        ) = calculate_colour_peak("ztfg", "ztfr", "plus7")
+        (
+            lc_metrics["g_r_colour_minus7"],
+            lc_metrics["g_r_colour_minus7_err"],
+        ) = calculate_colour_peak("ztfg", "ztfr", "minus7")
+        (
+            lc_metrics["g_i_colour_peak"],
+            lc_metrics["g_i_colour_peak_err"],
+        ) = calculate_colour_peak("ztfg", "ztfi", "t0")
+        (
+            lc_metrics["g_i_colour_plus7"],
+            lc_metrics["g_i_colour_plus7_err"],
+        ) = calculate_colour_peak("ztfg", "ztfi", "plus7")
+        (
+            lc_metrics["g_i_colour_minus7"],
+            lc_metrics["g_i_colour_minus7_err"],
+        ) = calculate_colour_peak("ztfg", "ztfi", "minus7")
 
-        #Calculate observed magnitude close to peak
+        # Calculate observed magnitude close to peak
         def calculate_obsmag_peak(band1, epoch):
-            '''
+            """
             Calculates observed magnitude for a particular epoch
-            '''
-            band1_table = str(band1) + 'cut'
-            if band1 not in sncosmo_table['band']:
+            """
+            band1_table = str(band1) + "cut"
+            if band1 not in sncosmo_table["band"]:
                 return None
-            elif epoch not in globals()[band1_table]['epoch']:
+            if epoch not in globals()[band1_table]["epoch"]:
                 return None
-            else:
-                obs_mag = -2.5 *np.log10( globals()[band1_table][np.where(globals()[band1_table]['epoch'] == epoch)]['flux'] ) + 25
-                return obs_mag.data[0]
-        
-        lc_metrics['obsmag_ztfg_peak'] = calculate_obsmag_peak('ztfg', 't0')
-        lc_metrics['obsmag_ztfr_peak'] = calculate_obsmag_peak('ztfr', 't0')
-        lc_metrics['obsmag_ztfi_peak'] = calculate_obsmag_peak('ztfi', 't0')
-        lc_metrics['obsmag_ztfg_plus7'] = calculate_obsmag_peak('ztfg', 'plus7')
-        lc_metrics['obsmag_ztfr_plus7'] = calculate_obsmag_peak('ztfr', 'plus7')
-        lc_metrics['obsmag_ztfi_plus7'] = calculate_obsmag_peak('ztfi', 'plus7')
-        lc_metrics['obsmag_ztfg_minus7'] = calculate_obsmag_peak('ztfg', 'minus7')
-        lc_metrics['obsmag_ztfr_minus7'] = calculate_obsmag_peak('ztfr', 'minus7')
-        lc_metrics['obsmag_ztfi_minus7'] = calculate_obsmag_peak('ztfi', 'minus7')
+            obs_mag = (
+                -2.5
+                * np.log10(
+                    globals()[band1_table][
+                        np.where(globals()[band1_table]["epoch"] == epoch)
+                    ]["flux"]
+                )
+                + 25
+            )
+            return obs_mag.data[0]
+
+        lc_metrics["obsmag_ztfg_peak"] = calculate_obsmag_peak("ztfg", "t0")
+        lc_metrics["obsmag_ztfr_peak"] = calculate_obsmag_peak("ztfr", "t0")
+        lc_metrics["obsmag_ztfi_peak"] = calculate_obsmag_peak("ztfi", "t0")
+        lc_metrics["obsmag_ztfg_plus7"] = calculate_obsmag_peak("ztfg", "plus7")
+        lc_metrics["obsmag_ztfr_plus7"] = calculate_obsmag_peak("ztfr", "plus7")
+        lc_metrics["obsmag_ztfi_plus7"] = calculate_obsmag_peak("ztfi", "plus7")
+        lc_metrics["obsmag_ztfg_minus7"] = calculate_obsmag_peak("ztfg", "minus7")
+        lc_metrics["obsmag_ztfr_minus7"] = calculate_obsmag_peak("ztfr", "minus7")
+        lc_metrics["obsmag_ztfi_minus7"] = calculate_obsmag_peak("ztfi", "minus7")
 
-        return lc_metrics
+        return lc_metrics
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2InfantCatalogEval.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2InfantCatalogEval.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,86 +3,91 @@
 # File:                ampel/contrib/hu/t2/T2TNSEval.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                27.01.2021
 # Last Modified Date:  17.03.2021
 # Last Modified By:    jnordin@physik.hu-berlin.de
 
-import numpy as np
-from typing import Any
 from collections.abc import Sequence
+from typing import Any
+
+import numpy as np
 from astropy.coordinates import Distance, SkyCoord
 from astropy.cosmology import Planck15
 
-from ampel.types import UBson
+from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 from ampel.view.T2DocView import T2DocView
-from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
 
 
 class T2InfantCatalogEval(AbsTiedLightCurveT2Unit):
     """
     Evaluate whether a transient fulfills criteria for being a potentially
     infant (extragalactic) transient.
 
     This implementation requires a catalog match with redshift.
     """
 
     # Cuts based on T2 catalog redshifts
 
     # List of catalog-like output to search for redshift. It is assumed that
     # redshifts are stored as 'z'
-    redshift_catalogs: list[str] = ['SDSS_spec', 'NEDz', 'GLADEv23', 'NEDz_extcats']  # Otherwise more
+    redshift_catalogs: list[str] = [
+        "SDSS_spec",
+        "NEDz",
+        "GLADEv23",
+        "NEDz_extcats",
+    ]  # Otherwise more
     # maximum redshift from T2 CATALOGMATCH catalogs (e.g. NEDz and SDSSspec)
-    max_redshift: float = 0.05 # 0.1
+    max_redshift: float = 0.05  # 0.1
     # minimum redshift from T2 CATALOGMATCH catalogs (e.g. NEDz and SDSSspec)
     min_redshift: float = 0.001
     # max abs mag through peak mag and redshift from catalog mach (require both)
-    max_absmag: float = -12 # Originally -13, moved to -12 due to ZTF22aafoqrd
+    max_absmag: float = -12  # Originally -13, moved to -12 due to ZTF22aafoqrd
     # min abs mag through peak mag and redshift from catalog mach (require both)
-    min_absmag: float = -20 # -17
+    min_absmag: float = -20  # -17
     # arcsec, minimum distance to remove star matches to transient if found (eg in SDSSDR10)
     min_dist: float = 1.5
     # arcsec, maximum distance
     max_dist: float = 50
     # kpc, maximum distance
     max_kpc_dist: float = 999
 
     # Cut on alert properties
 
     # A candidate need to have at least this many detections
     min_ndet: int = 1
     min_ndet_postul: int = 0  # and if it has this minimum nr of detection after the last significant (max_maglim) UL.
 
     # days, If a detection has an age older than this, skip (stars,age).
-    max_age: float = 3.
+    max_age: float = 3.0
 
     # Min age of detection history
     min_age: float = 0
     # range of peak magnitudes for submission
     min_peak_mag: float = 20
-    max_peak_mag: float = 16
+    max_peak_mag: float = 14
     # Reported detections in at least this many filters
     min_n_filters: int = 1
     # Require a detection in one of these filters (e.g. ZTF I-band more often spurious)
-    det_filterids: list[int] = [1, 2, 3]   # default to any of them
+    det_filterids: list[int] = [1, 2, 3]  # default to any of them
     # Minimal galactic latitide
     min_gal_lat: float = 14
     # reject alert if ssdistnr smaller than this value for any pp
     ssdistnr_max: float = 1
     # reject alert if PS1 star for any pp
     ps1_sgveto_rad: float = 1
     ps1_sgveto_sgth: float = 0.8
     # Minimal median RB.
     rb_minmed: float = 0.3
     # Minimal median RB.
     drb_minmed: float = 0.995
 
-
     # Limiting magnitude to consider upper limits as 'significant'
     maglim_min: float = 19.5
     # A limiting magnitude max this time ago
     maglim_maxago: float = 2.5
 
     # Cut to apply to all the photopoints in the light curve.
     # This will affect most operations, i.e. evaluating the position,
@@ -99,84 +104,81 @@
 
         # P1. # Loop through listed catalogs for redshift matches
         zmatchs = []
         info = {}
         for catname in self.redshift_catalogs:
             catinfo = cat_res.get(catname, False)
             if (
-                catinfo and
-                (self.min_redshift < catinfo["z"] < self.max_redshift) and
-                (self.min_dist < catinfo["dist2transient"] < self.max_dist)
+                catinfo
+                and isinstance(catinfo.get("z", None), float)
+                and (self.min_redshift < catinfo["z"] < self.max_redshift)
+                and (self.min_dist < catinfo["dist2transient"] < self.max_dist)
             ):
                 self.logger.info(
                     "Found z.",
                     extra={
                         "catalog": catname,
                         "z": catinfo["z"],
                         "dist": catinfo["dist2transient"],
                     },
                 )
                 # Calculate physical distance
                 dst_kpc = (
-                    catinfo["dist2transient"] *
-                    Planck15.kpc_proper_per_arcmin(catinfo["z"]).value / 60.0
+                    catinfo["dist2transient"]
+                    * Planck15.kpc_proper_per_arcmin(catinfo["z"]).value
+                    / 60.0
                 )
                 if self.max_kpc_dist > 0 and dst_kpc > self.max_kpc_dist:
                     self.logger.info(
                         "Skip, physical distance too large.",
                         extra={"distance_kpc": dst_kpc},
                     )
                     continue
                 zmatchs.append([catinfo["z"]])
                 info[f"{catname}_z"] = catinfo["z"]
                 info[f"{catname}_dist2transient"] = catinfo["dist2transient"]
 
         if len(zmatchs) == 0:
-            self.logger.info("No z match.")
             return None
-        info['zs'] = zmatchs
+        info["zs"] = zmatchs
 
         # Special catalog searches - mark transients close to AGNs
         milliquas = cat_res.get("milliquas", False)
         sdss_spec = cat_res.get("SDSS_spec", False)
         if milliquas and milliquas["redshift"] > 0:
             info["milliAGN"] = True
         if sdss_spec and sdss_spec["bptclass"] in [4, 5]:
             info["sdssAGN"] = True
 
         # Return collected info
         return info
 
-
-
     def inspect_lc(self, lc: LightCurve) -> None | dict[str, Any]:
         """
         Verify whether the transient lightcurve fulfill criteria for submission.
 
         """
 
         # apply cut on history: consider photophoints which are sharp enough
         pps = lc.get_photopoints(filters=self.lc_filters)
         assert pps is not None
         info: dict[str, Any] = {}
 
         # cut on number of detection
         if len(pps) < self.min_ndet:
-            self.logger.info(
-                'Rejected', extra={'det': len(pps)}
-            )
+            self.logger.info("Rejected", extra={"det": len(pps)})
             return None
         info["detections"] = len(pps)
 
         # cut on age
         jds = [pp["body"]["jd"] for pp in pps]
         most_recent_detection, first_detection = max(jds), min(jds)
         age = most_recent_detection - first_detection
         if age > self.max_age or age < self.min_age:
-            self.logger.info('Rejected', extra={'age': age})
+            self.logger.info("Rejected", extra={"age": age})
             return None
         info["age"] = age
 
         # cut on number of detection after last SIGNIFICANT UL
         ulims = lc.get_upperlimits(
             filters={
                 "attribute": "diffmaglim",
@@ -184,20 +186,23 @@
                 "value": self.maglim_min,
             }
         )
 
         if ulims and len(ulims) > 0:
             last_ulim_jd = sorted([x["body"]["jd"] for x in ulims])[-1]
             pps_after_ndet = lc.get_photopoints(
-                filters=self.lc_filters + [{"attribute": "jd", "operator": ">=", "value": last_ulim_jd}]
+                filters=[
+                    *self.lc_filters,
+                    {"attribute": "jd", "operator": ">=", "value": last_ulim_jd},
+                ]
             )
             # Check if there are enough positive detection after the last significant UL
             if (
-                pps_after_ndet is not None and
-                len(pps_after_ndet) < self.min_ndet_postul
+                pps_after_ndet is not None
+                and len(pps_after_ndet) < self.min_ndet_postul
             ):
                 self.logger.info(
                     "not enough consecutive detections after last significant UL.",
                     extra={"NDet": len(pps), "lastUlimJD": last_ulim_jd},
                 )
                 return None
             # Check that there is a recent ul
@@ -214,32 +219,28 @@
         else:
             self.logger.info("no UL")
             return None
 
         # cut on number of filters
         used_filters = set([pp["body"]["fid"] for pp in pps])
         if len(used_filters) < self.min_n_filters:
-            self.logger.info(
-                "Rejected", extra={'nbr_filt': len(used_filters)}
-            )
+            self.logger.info("Rejected", extra={"nbr_filt": len(used_filters)})
             return None
         # cut on which filters used
         if used_filters.isdisjoint(self.det_filterids):
             self.logger.info(
-                "Rejected (wrong filter det)", extra={'det_filters': used_filters}
+                "Rejected (wrong filter det)", extra={"det_filters": used_filters}
             )
             return None
 
         # cut on range of peak magnitude
         mags = [pp["body"]["magpsf"] for pp in pps]
         peak_mag = min(mags)
         if peak_mag > self.min_peak_mag or peak_mag < self.max_peak_mag:
-            self.logger.info(
-                "Rejected", extra={'peak_mag': peak_mag}
-            )
+            self.logger.info("Rejected", extra={"peak_mag": peak_mag})
             return None
         info["peak_mag"] = peak_mag
 
         # For rapidly declining sources the latest magnitude is probably more relevant
         latest_pps = lc.get_photopoints(
             filters={
                 "attribute": "jd",
@@ -258,40 +259,43 @@
         if pos := lc.get_pos(ret="mean", filters=self.lc_filters):
             ra, dec = pos
         else:
             raise ValueError("Light curve contains no points")
         coordinates = SkyCoord(ra, dec, unit="deg")
         b = coordinates.galactic.b.deg
         if abs(b) < self.min_gal_lat:
-            self.logger.info(
-                "Rejected (galactic plane)", extra={'gal_lat_b': b}
-            )
+            self.logger.info("Rejected (galactic plane)", extra={"gal_lat_b": b})
             return None
         info["ra"] = ra
         info["dec"] = dec
 
         # cut on distance to closest solar system object
         # TODO: how to make this check: ('0.0' in list(phot["ssdistnr"])
-        ssdist = np.array([pp["body"]["ssdistnr"] for pp in pps
-            if "ssdistnr" in pp['body'].keys() and pp["body"]["ssdistnr"] is not None])
+        ssdist = np.array(
+            [
+                pp["body"]["ssdistnr"]
+                for pp in pps
+                if "ssdistnr" in pp["body"] and pp["body"]["ssdistnr"] is not None
+            ]
+        )
         close_to_sso = np.logical_and(ssdist < self.ssdistnr_max, ssdist > 0)
 
         # TODO: Note that this discards a transient if it was ever close to a ss object!
         if np.any(close_to_sso):
             self.logger.info(
                 "Rejected (close to solar system object)",
                 extra={"ssdistnr": ssdist.tolist()},
             )
             return None
 
         # check PS1 sg for the full alert history
         # Note that we for this check do *not* use the lightcurve filter criteria
         # TODO: Evaluate whether we should use the filters, and do a check for sufficient number of datapoints remaining
         if psdata := lc.get_tuples("distpsnr1", "sgscore1"):
-            distpsnr1, sgscore1 = zip(*psdata)
+            distpsnr1, sgscore1 = zip(*psdata, strict=False)
             is_ps1_star = np.logical_and(
                 np.array(distpsnr1) < self.ps1_sgveto_rad,
                 np.array(sgscore1) > self.ps1_sgveto_sgth,
             )
             if np.any(is_ps1_star):
                 self.logger.info(
                     "Rejected (PS1 SG cut)",
@@ -305,40 +309,41 @@
         rbs = [pp["body"]["rb"] for pp in pps]
         if np.median(rbs) < self.rb_minmed:
             self.logger.info(
                 "Rejected (RB)",
                 extra={"median_rd": np.median(rbs)},
             )
             return None
-        elif (len(rbs) == 0) and self.rb_minmed > 0:
+        if (len(rbs) == 0) and self.rb_minmed > 0:
             self.logger.info("Rejected (No rb info)")
             return None
         info["rb"] = np.median(rbs)
 
         # drb might not exist
         drbs = [pp["body"]["drb"] for pp in pps if "drb" in pp["body"]]
         if len(drbs) > 0 and np.median(drbs) < self.drb_minmed:
             self.logger.info(
                 "Rejected (dRB)",
                 extra={"median_drd": np.median(drbs)},
             )
             return None
-        elif (len(drbs) == 0) and self.drb_minmed > 0:
+        if (len(drbs) == 0) and self.drb_minmed > 0:
             self.logger.info("Rejected (No drb info)")
             return None
 
         info["drb"] = np.median(drbs)
 
         # Transient passed pure LC criteria
         self.logger.info("Passed T2infantCatalogEval", extra=info)
         return info
 
-
     # MANDATORY
-    def process(self, light_curve: LightCurve, t2_views: Sequence[T2DocView]) -> UBson | UnitResult:
+    def process(
+        self, light_curve: LightCurve, t2_views: Sequence[T2DocView]
+    ) -> UBson | UnitResult:
         """
 
         Evaluate whether a transient passes thresholds for being a nearby (young) transient.
 
         Parameters
         -----------
         light_curve: "ampel.view.LightCurve" instance.
@@ -351,47 +356,43 @@
         dict
 
         Containing transient info, and in particular the 'action' key. This will be set to true
         for transients passing all selection criteria.
 
         """
 
-
         # i. Check the catalog matching criteria
         # There might be multiple CatalogMatch associated with the transient
         # we here only take the first without specific origin
         t2_cat_match = t2_views[0]
 
         catalog_result = t2_cat_match.get_payload()
         if not isinstance(catalog_result, dict):
-            return {'action': False, 'eval': 'No catlog match result'}
+            return {"action": False, "eval": "No catlog match result"}
         transient_info = self.inspect_catalog(catalog_result)
         if not transient_info:
-            return {'action': False, 'eval': 'No cat match in z-range'}
-
+            return {"action": False, "eval": "No cat match in z-range"}
 
         # ii. Check whether the lightcurve passes selection criteria
         lc_info = self.inspect_lc(light_curve)
 
         if not lc_info:
-            transient_info['action'] = False
-            transient_info['eval'] = 'LC fail selection.'
+            transient_info["action"] = False
+            transient_info["eval"] = "LC fail selection."
             return transient_info
         transient_info.update(lc_info)
 
-
         # iii. Check absolute magnitude
-        sndist = Distance(z=np.mean(transient_info['zs']), cosmology=Planck15)
+        sndist = Distance(z=np.mean(transient_info["zs"]), cosmology=Planck15)
         absmag = transient_info["peak_mag"] - sndist.distmod.value
         transient_info["absmag"] = absmag
         if not (self.min_absmag < absmag < self.max_absmag):
             self.logger.info("Rejected (absmag)", extra={"absmag": absmag})
-            transient_info['action'] = False
-            transient_info['eval'] = 'Absmag'
+            transient_info["action"] = False
+            transient_info["eval"] = "Absmag"
             return transient_info
 
         # Passed all criteria - ready for action
-        transient_info['action'] = True
-        transient_info['eval'] = 'Pass'
-
+        transient_info["action"] = True
+        transient_info["eval"] = "Pass"
 
         return transient_info
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2LCQuality.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LCQuality.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 # License:             BSD-3-Clause
 # Author:              matteo.giomi@desy.de
 # Date:                11.09.2018
 # Last Modified Date:  06.06.2020
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 from typing import Any
+
 from astropy.table import Table
 from scipy.interpolate import interp1d
 
-from ampel.types import UBson
 from ampel.abstract.AbsLightCurveT2Unit import AbsLightCurveT2Unit
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 
 
 class T2LCQuality(AbsLightCurveT2Unit):
     """
     determine the 'quality' of the light curve by computing ratios between
     the number of detection and that of upper limits.
@@ -191,34 +192,33 @@
                 }
         }
         """
 
         # run on the single bands individually
         out_dict = {}
         for fid in self.filter_ids:
-
             self.logger.debug(
                 f"computing light curve quality for filter id {fid} "
                 f"({self.filter_names[fid]}-band)"
             )
 
             # concatenate the filters
             filters: list[dict[str, Any]] = [
                 {"attribute": "fid", "operator": "==", "value": fid}
             ]
-            if isinstance(self.lc_filter, (list, tuple)):
+            if isinstance(self.lc_filter, list | tuple):
                 filters += self.lc_filter
             elif isinstance(self.lc_filter, dict):
                 filters += [self.lc_filter]
             else:
                 raise ValueError(
                     f"parameter 'lc_filter' must be either list or tuple. got {type(self.lc_filter)} instead"
                 )
 
-            self.logger.debug(f"applying filter: {repr(filters)}")
+            self.logger.debug(f"applying filter: {filters!r}")
 
             # get upper limits and detections time series
             pps = light_curve.get_tuples("jd", "magpsf", filters=filters)
             uls = light_curve.get_tuples(
                 "jd", "diffmaglim", filters=filters, of_upper_limits=True
             )
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2LSPhotoZTap.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LSPhotoZTap.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,47 +3,43 @@
 # File              : Ampel-contrib-HU/ampel/contrib/hu/t2/T2LSPhotoZTap.py
 # License           : BSD-3-Clause
 # Author            : jnordin
 # Date              : 20.04.2021
 # Last Modified Date: 21.04.2021
 # Last Modified By  : jnordin
 
-from typing import Any, Sequence, TYPE_CHECKING, Union
-
-from astropy.table import Table
-
-from ampel.abstract.AbsPointT2Unit import AbsPointT2Unit
-from ampel.content.DataPoint import DataPoint
-
-from ampel.struct.UnitResult import UnitResult
-from ampel.enum.DocumentCode import DocumentCode
-from ampel.types import UBson
-
-from math import cos, sin, acos, pi
-# Datalab
-from dl import authClient
-
 from collections import OrderedDict
-import numpy as np
-from pandas import read_csv
-from astropy.table import Table
-from astropy.io.votable import parse_single_table
+from collections.abc import Sequence
 from functools import partial
 from io import BytesIO
+from math import acos, cos, pi, sin
+from typing import Any
 
 import backoff
+import numpy as np
 import requests
+from astropy.io.votable import parse_single_table
+from astropy.table import Table
+
+# Datalab
+from dl import authClient
+from pandas import read_csv
 
+from ampel.abstract.AbsPointT2Unit import AbsPointT2Unit
+from ampel.content.DataPoint import DataPoint
+from ampel.enum.DocumentCode import DocumentCode
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 
-def convert(inp,outfmt='pandas',verbose=False,**kwargs):
 
+def convert(inp, outfmt="pandas", verbose=False, **kwargs):
     """
     *** Taken from datalab dl/helpers/util/convert ***
     (to avoid loading alld ependencies)
-    
+
     Convert input `inp` to a data structure defined by `outfmt`.
 
     Parameters
     ----------
     inp : str
         String representation of the result of a query. Usually this
         is a CSV-formatted string, but can also be, e.g. an
@@ -84,53 +80,71 @@
        df.head()  # df is as Pandas dataframe, with all its methods
 
        df = convert(inp,'pandas',na_values='Infinity') # na_values is a kwarg; adds 'Infinity' to list of values converter to np.inf
 
     """
     # When there are duplicate column names in the table, it would not work when converting to Astropy Table and Votable, so we
     # have to add '_n' as an identifier to the duplicate column names.
-    index = inp.find('\n')
+    index = inp.find("\n")
     header = inp[0:index]
-    inp = inp[index+1:]
-    list = header.split(',')
-    col_dict = {}
-    new_s = ''
+    inp = inp[index + 1 :]
+    list = header.split(",")
+    col_dict: dict[str, int] = {}
+    new_s = ""
     for l in list:
-        if l in col_dict.keys():
-            n = col_dict.get(l)
-            col_dict[l] = n+1
-            new_s += (l+'_'+str(n)+',')
+        if l in col_dict:
+            n = col_dict[l]
+            col_dict[l] = n + 1
+            new_s += l + "_" + str(n) + ","
         else:
-            new_s += (l+',')
-            col_dict[l]=1
-    inp = new_s[:-1]+'\n'+inp
-
+            new_s += l + ","
+            col_dict[l] = 1
+    inp = new_s[:-1] + "\n" + inp
 
     # map outfmt container types to a tuple:
     # (:func:`queryClient.query()` fmt-value, descriptive title,
     # processing function for the result string)
-    mapping = OrderedDict([
-        ('string'      , ('csv',     'CSV formatted table as a string', lambda x: x.getvalue())),
-        ('array'       , ('csv',     'Numpy array',                     partial(np.loadtxt,unpack=False,skiprows=1,delimiter=','))),
-        ('structarray' , ('csv',     'Numpy structured / record array', partial(np.genfromtxt,dtype=float,delimiter=',',names=True))),
-        ('pandas'      , ('csv',     'Pandas dataframe',                read_csv)),
-        ('table'       , ('csv',     'Astropy Table',                   partial(Table.read,format='csv'))),
-        ('votable'     , ('votable', 'Astropy VOtable',                 parse_single_table))
-    ])
+    mapping = OrderedDict(
+        [
+            (
+                "string",
+                ("csv", "CSV formatted table as a string", lambda x: x.getvalue()),
+            ),
+            (
+                "array",
+                (
+                    "csv",
+                    "Numpy array",
+                    partial(np.loadtxt, unpack=False, skiprows=1, delimiter=","),
+                ),
+            ),
+            (
+                "structarray",
+                (
+                    "csv",
+                    "Numpy structured / record array",
+                    partial(np.genfromtxt, dtype=float, delimiter=",", names=True),
+                ),
+            ),
+            ("pandas", ("csv", "Pandas dataframe", read_csv)),
+            ("table", ("csv", "Astropy Table", partial(Table.read, format="csv"))),
+            ("votable", ("votable", "Astropy VOtable", parse_single_table)),
+        ]
+    )
 
-    if isinstance(inp,bytes):
+    if isinstance(inp, bytes):
         b = BytesIO(inp)
-    elif isinstance(inp,str):
+    elif isinstance(inp, str):
         b = BytesIO(inp.encode())
     else:
-        raise TypeError('Input must be of bytes or str type.')
+        raise TypeError("Input must be of bytes or str type.")
 
-    output = mapping[outfmt][2](b,**kwargs)
+    output = mapping[outfmt][2](b, **kwargs)
 
-    if isinstance(output,bytes):
+    if isinstance(output, bytes):
         output = output.decode()
 
     if verbose:
         print("Returning %s" % mapping[outfmt][1])
 
     return output
 
@@ -139,110 +153,116 @@
     """
     Query the NOIR DataLab service for photometric redshifts from the
     Legacy Survey.
 
     Other queries can in principle be made as long as the string format parameters are the same (ra, dec, match_radius).
 
     """
-   
+
     # Astro DataLab user id
-    datalab_user : str
-    datalab_pwd : str
+    datalab_user: str
+    datalab_pwd: str
     ##datalab_str : Secret
 
     # Match parameters
-    match_radius: float = 10    # in arcsec
+    match_radius: float = 10  # in arcsec
 
     # Query. Candidate position and radius will be added
     query: str = "SELECT ra, dec, photo_z.z_phot_median, photo_z.z_phot_mean, photo_z.z_phot_l68, z_phot_u68, photo_z.z_spec, tractor.dered_mag_g, tractor.dered_mag_r, tractor.dered_mag_z, tractor.dered_mag_w1, tractor.dered_mag_w2 , tractor.dered_mag_w3, tractor.dered_mag_w4, tractor.snr_g, tractor.snr_r, tractor.snr_z, tractor.snr_w1, tractor.snr_w2, tractor.snr_w3, tractor.snr_w4 FROM ls_dr8.tractor as tractor JOIN ls_dr8.photo_z as photo_z on photo_z.ls_id = tractor.ls_id WHERE 't' = Q3C_RADIAL_QUERY(ra, dec,%.6f,%.6f,%.6f)"
 
-
     # run only on first datapoint by default
     # NB: this assumes that docs are created by DualPointT2Ingester
     ingest: dict = {"eligible": {"pps": "first"}}
 
     # Path to noir queries
-    datalab_query_url: str = 'https://datalab.noirlab.edu/query'
-    
-
+    datalab_query_url: str = "https://datalab.noirlab.edu/query"
 
     def post_init(self) -> None:
         # obtain security token
-        self.token = authClient.login(self.datalab_user, self.datalab_pwd) 
-#        self.token = authClient.login(self.datalab_user, self.datalab_str) 
+        self.token = authClient.login(self.datalab_user, self.datalab_pwd)
+
+    #        self.token = authClient.login(self.datalab_user, self.datalab_str)
 
     @backoff.on_exception(
         backoff.expo,
         requests.ConnectionError,
         max_tries=5,
         factor=10,
     )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: isinstance(e, requests.HTTPError) and e.response.status_code not in {503, 429},
+        giveup=lambda e: isinstance(e, requests.HTTPError)
+        and e.response.status_code not in {503, 429},
         max_time=60,
     )
-    def _astrolab_query(self,
-        ra: float,
-        dec: float 
-        )-> Sequence[ dict[str,Any] ]:    # Does one need to add List[None] here for empty returns?
- 
-        self.logger.debug("Querying %s %s"%(ra,dec))
-        
+    def _astrolab_query(
+        self, ra: float, dec: float
+    ) -> Sequence[
+        dict[str, Any]
+    ]:  # Does one need to add List[None] here for empty returns?
+        self.logger.debug(f"Querying {ra} {dec}")
+
         # Original qery, using the wrong path (and also a lot of dependencies)
         ## should be possible to adjust this:
         ## qc = queryClient.queryClient()
         ## qc.set_svc_url( 'https://datalab.noirlab.edu/query' )
         ## But this yiels a split error
         # Old query
-        #ret = queryClient.query(self.token, self.query % (ra, dec, float(self.match_radius) / 3600) )
-        #ret_dict = convert(ret,'pandas').to_dict(orient='records')
+        # ret = queryClient.query(self.token, self.query % (ra, dec, float(self.match_radius) / 3600) )
+        # ret_dict = convert(ret,'pandas').to_dict(orient='records')
         # New manual:
-        headers = { 'X-DL-AuthToken': (self.token)   }
+        headers = {"X-DL-AuthToken": (self.token)}
         sql = self.query % (ra, dec, float(self.match_radius) / 3600)
-        qfmt = 'csv'
-        async_ = False
         timeout = 300
-        dburl = '%s/query?sql=%s&ofmt=%s&async=%s' % ( self.datalab_query_url, sql, qfmt, async_ )
-        r = requests.get (dburl, headers=headers, timeout=timeout )
+        r = requests.get(
+            f"{self.datalab_query_url}/query",
+            params={"sql": sql, "qfmt": "csv", "async": "0"},
+            headers=headers,
+            timeout=timeout,
+        )
         if not r.ok:
-            self.logger.debug("DL query failed at %s %s"%(ra,dec))
+            self.logger.debug(f"DL query failed at {ra} {dec}" % (ra, dec))
             return []
-        
+
         # First convert to string and then to dict
-        ret_dict = convert( str(r.content.decode()) ,'pandas').to_dict(orient='records')
-        
-        self.logger.debug("Got %s matches"%(len(ret_dict)))
-        
-        return ret_dict	
+        ret_dict = convert(str(r.content.decode()), "pandas").to_dict(orient="records")
+
+        self.logger.debug("Got %s matches" % (len(ret_dict)))
 
+        return ret_dict
 
-    def add_separation(self, 
-        match_dict: Sequence[ dict[str,Any] ], target_ra: float, target_dec: float
-        )-> Sequence[ dict[str, Any] ]:
+    def add_separation(
+        self, match_dict: Sequence[dict[str, Any]], target_ra: float, target_dec: float
+    ) -> Sequence[dict[str, Any]]:
         """
         Iterate through catalog entries (dict) and add separation to target.
         """
         c = pi / 180
 
         for el in match_dict:
-            if 'dec' in el.keys() and 'ra' in el.keys():
-                el['dist2transient'] = acos(
-                    sin(target_dec * c) * sin(el['dec'] * c) +
-                    cos(target_dec * c) * cos(el['dec'] * c) * cos((target_ra - el['ra']) * c)
-                ) * 206264.8062 # to arcsecs
+            if "dec" in el and "ra" in el:
+                el["dist2transient"] = (
+                    acos(
+                        sin(target_dec * c) * sin(el["dec"] * c)
+                        + cos(target_dec * c)
+                        * cos(el["dec"] * c)
+                        * cos((target_ra - el["ra"]) * c)
+                    )
+                    * 206264.8062
+                )  # to arcsecs
             else:
-                el['dist2transient'] = None
+                el["dist2transient"] = None
 
         return match_dict
 
-
-    def process(self, datapoint: DataPoint) -> Union[UBson, UnitResult]:
-        return_all: bool = False #whether to return all matches or closest match (default)
+    def process(self, datapoint: DataPoint) -> UBson | UnitResult:
+        return_all: bool = (
+            False  # whether to return all matches or closest match (default)
+        )
         """
         Query DataLab through the unit query string combined with 
         transient position. 
 
         :returns: 
         {
         0:  {'ra': 247.033806830109,
@@ -269,19 +289,17 @@
             ##return T2RunState.MISSING_INFO
             return UnitResult(code=DocumentCode.T2_MISSING_INFO)
 
         # Query Datalab
         match_list = self._astrolab_query(transient_ra, transient_dec)
 
         # Add separation between target and query detection
-        if len(match_list)>0:
-            match_list = self.add_separation( match_list, transient_ra, transient_dec )
+        if len(match_list) > 0:
+            match_list = self.add_separation(match_list, transient_ra, transient_dec)
 
         # Return a T2 result (dict-like)
-        if len(match_list)>0:
-            if return_all == True:
-                return {'T2LSPhotoZTap{}'.format(k) :item for k, item in enumerate(match_list)}
-            else:
-                min_dist = min(match_list, key=lambda x:x['dist2transient'])
-                return {'T2LSPhotoZTap': min_dist}
-        else:
-            return {'T2LSPhotoZTap':None}
+        if len(match_list) > 0:
+            if return_all:
+                return {f"T2LSPhotoZTap{k}": item for k, item in enumerate(match_list)}
+            min_dist = min(match_list, key=lambda x: x["dist2transient"])
+            return {"T2LSPhotoZTap": min_dist}
+        return {"T2LSPhotoZTap": None}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2MatchBTS.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchBTS.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,77 +3,76 @@
 # File:                ampel/contrib/hu/t2/T2MatchBts.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                01.06.2021
 # Last Modified Date:  13.12.2021
 # Last Modified By:    jnordin@physik.hu-berlin.de
 
-from typing import Union
-import requests
-import backoff
-import pandas as pd
 import io
 from datetime import datetime
 
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.view.LightCurve import LightCurve
+import backoff
+import pandas as pd
+import requests
+from bson import tz_util
 
-#from ampel.view.T2DocView import T2DocView
+# from ampel.view.T2DocView import T2DocView
 from ampel.abstract.AbsLightCurveT2Unit import AbsLightCurveT2Unit
-from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
 from ampel.enum.DocumentCode import DocumentCode
-from bson import tz_util
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
+from ampel.view.LightCurve import LightCurve
+from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
 
 
 class T2MatchBTS(AbsLightCurveT2Unit):
     """
 
     Add information from the BTS explorer page.
 
     Warning: This will be synced once at init, and the unit output thus depends on
     external sources!
     """
 
     # Query used to get data from https://sites.astro.caltech.edu/ztf/bts/bts.php
-    bts_query: str = "https://sites.astro.caltech.edu/ztf/bts/explorer.php?f=s&format=csv"
-
+    bts_query: str = (
+        "https://sites.astro.caltech.edu/ztf/bts/explorer.php?f=s&format=csv"
+    )
 
     @backoff.on_exception(
         backoff.expo,
         requests.ConnectionError,
         max_tries=5,
         factor=10,
     )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: not isinstance(e, requests.HTTPError) or e.response.status_code not in {503, 429},
+        giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response.status_code not in {503, 429},
         max_time=60,
     )
-    def post_init(self)->None:
+    def post_init(self) -> None:
         """
         Obtain a synced copy of the BTS explorer output.
         """
 
         self.bts_df = None
 
         req = requests.get(self.bts_query)
         req.raise_for_status()
 
         if req.ok:
             df = pd.read_csv(io.StringIO(req.content.decode()))
-            df['synced_at'] = datetime.now(tz_util.utc).timestamp()
+            df["synced_at"] = datetime.now(tz_util.utc).timestamp()
             cols = df.columns
-            newcols = {col:'bts_'+col for col in cols}
+            newcols = {col: "bts_" + col for col in cols}
             df.rename(columns=newcols, inplace=True)
             self.bts_df = df
 
-
-
     def process(self, light_curve: LightCurve) -> UBson | UnitResult:
         """
         Check whether transient exists in the bts df.
         If so, return content
 
         :returns: dict with content of BTS explorer for transient, together with timestamp.
         E.g.:
@@ -98,16 +97,17 @@
         # Get name used by BTS
         assert isinstance(light_curve.stock_id, int)
         ztf_name = ZTFIdMapper.to_ext_id(light_curve.stock_id)
 
         if self.bts_df is None:
             return UnitResult(code=DocumentCode.T2_MISSING_INFO)
 
-
-        match = self.bts_df[self.bts_df['bts_ZTFID'] == ztf_name].to_dict(orient='index')
+        match = self.bts_df[self.bts_df["bts_ZTFID"] == ztf_name].to_dict(
+            orient="index"
+        )
 
         if len(match) == 0:
             # In case of now match, only returned timestamp when check was made
-            return {'bts_synced_at' : self.bts_df['bts_synced_at'][0]}
+            return {"bts_synced_at": self.bts_df["bts_synced_at"][0]}
 
         # Otherwise, return full match dictionary. Assuming unique BTS match, otherwise first entry is retrieved
-        return list(match.values())[0]
+        return next(iter(match.values()))
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2MultiXgbClassifier.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MultiXgbClassifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,190 +3,282 @@
 # File:                ampel/contrib/hu/t2/T2MultiXgbClassifier.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                03.07.2022
 # Last Modified Date:  12.12.2022
 # Last Modified By:    jnordin@physik.hu-berlin.de
 
-from typing import Literal, Union, Dict
+import os
 from collections.abc import Sequence
-
+from typing import Literal
 
 import numpy as np
 import xgboost as xgb
-import os
 
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.abstract.AbsTabulatedT2Unit import AbsTabulatedT2Unit
-from ampel.model.StateT2Dependency import StateT2Dependency
-from ampel.content.T1Document import T1Document
+from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.content.DataPoint import DataPoint
+from ampel.content.T1Document import T1Document
+from ampel.contrib.hu.t2.T2TabulatorRiseDecline import (
+    FitFailed,
+    T2TabulatorRiseDeclineBase,
+)
+from ampel.enum.DocumentCode import DocumentCode
+from ampel.model.StateT2Dependency import StateT2Dependency
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.T2DocView import T2DocView
-from ampel.contrib.hu.t2.T2TabulatorRiseDecline import T2TabulatorRiseDeclineBase
 
-class T2MultiXgbClassifier(AbsTiedStateT2Unit, AbsTabulatedT2Unit, T2TabulatorRiseDeclineBase):
+
+class T2MultiXgbClassifier(
+    AbsTiedStateT2Unit, AbsTabulatedT2Unit, T2TabulatorRiseDeclineBase
+):
     """
     For a range of xgboost classifier models, find a classification.
     This unit differs from T2XgbClassifier in that this unit assumes
     that a classifier applies to any number of detections and that every
     unit in the input dict is run.
 
     Will test whether the first (null) model of each classifier is
     more likely, P(model 0)>0.5. What this means is determined by the training.
 
     E.g. For the elasticc1v2 model, the null model corresponds to Elasticc class 1
     (and model 1 to class 2.)
 
     """
 
-
-    model_folder: str = '/home/jnordin/github/zweilasticc/ml_workshop/elasticc/iter100'
+    model_folder: str = "/home/jnordin/github/zweilasticc/ml_workshop/elasticc/iter100"
     # Dict with names and path (in model_folder) for each classifier
     model_dict: dict[str, str] = {}
 
-    _classifiers: dict[str,xgb.XGBClassifier]
+    _classifiers: dict[str, xgb.XGBClassifier]
 
     # Columns (in order) used for training
     # Which columsn to use for training. But these seem not to align with
     # parquet file!!!!
-    use_cols: list[str] = ['ndet', 'jd_det', 'jd_last', 't_predetect', 'mag_det',
-        'band_det_id', 'mag_last', 'band_last_id', 't_lc', 'bool_pure',
-        'jd_peak_lsstz', 'bool_rise', 'bool_fall', 'bool_peaked', 'bool_fastrise',
-        'bool_fastfall', 'bool_hasgaps', 'det_bands', 'last_bands',
-        'jd_peak_lsstr', 'rise_slope_lsstz', 'rise_slopesig_lsstz',
-        'fall_slope_lsstz', 'fall_slopesig_lsstz', 'jd_peak', 't_rise', 't_fall',
-        'peak_bands', 'jd_peak_lssty', 'lsstz-lssty_last', 'lsstz-lssty_peak',
-        'fall_slope_lssty', 'fall_slopesig_lssty', 'jd_peak_lssti',
-        'fall_slope_lssti', 'fall_slopesig_lssti', 'jd_peak_lsstu',
-        'fall_slope_lsstr', 'fall_slopesig_lsstr', 'jd_peak_lsstg',
-        'rise_slope_lsstg', 'rise_slopesig_lsstg', 'rise_slope_lsstu',
-        'rise_slopesig_lsstu', 'rise_slope_lssti', 'rise_slopesig_lssti',
-        'lsstu-lsstg_last', 'fall_slope_lsstu', 'fall_slopesig_lsstu',
-        'lssti-lsstz_last', 'rise_slope_lssty', 'rise_slopesig_lssty',
-        'fall_slope_lsstg', 'fall_slopesig_lsstg', 'lsstg-lsstr_last',
-        'lsstr-lssti_last', 'lsstu-lsstg_peak', 'rise_slope_lsstr',
-        'rise_slopesig_lsstr', 'lsstg-lsstr_peak', 'lsstz-lssty_det',
-        'lssti-lsstz_peak', 'lsstr-lssti_peak', 'lssti-lsstz_det',
-        'lsstg-lsstr_det', 'lsstr-lssti_det', 'lsstu-lsstg_det',
-        'z', 'z_err', 'host_sep']
+    use_cols: list[str] = [
+        "ndet",
+        "jd_det",
+        "jd_last",
+        "t_predetect",
+        "mag_det",
+        "band_det_id",
+        "mag_last",
+        "band_last_id",
+        "t_lc",
+        "bool_pure",
+        "jd_peak_lsstz",
+        "bool_rise",
+        "bool_fall",
+        "bool_peaked",
+        "bool_fastrise",
+        "bool_fastfall",
+        "bool_hasgaps",
+        "det_bands",
+        "last_bands",
+        "jd_peak_lsstr",
+        "rise_slope_lsstz",
+        "rise_slopesig_lsstz",
+        "fall_slope_lsstz",
+        "fall_slopesig_lsstz",
+        "jd_peak",
+        "t_rise",
+        "t_fall",
+        "peak_bands",
+        "jd_peak_lssty",
+        "lsstz-lssty_last",
+        "lsstz-lssty_peak",
+        "fall_slope_lssty",
+        "fall_slopesig_lssty",
+        "jd_peak_lssti",
+        "fall_slope_lssti",
+        "fall_slopesig_lssti",
+        "jd_peak_lsstu",
+        "fall_slope_lsstr",
+        "fall_slopesig_lsstr",
+        "jd_peak_lsstg",
+        "rise_slope_lsstg",
+        "rise_slopesig_lsstg",
+        "rise_slope_lsstu",
+        "rise_slopesig_lsstu",
+        "rise_slope_lssti",
+        "rise_slopesig_lssti",
+        "lsstu-lsstg_last",
+        "fall_slope_lsstu",
+        "fall_slopesig_lsstu",
+        "lssti-lsstz_last",
+        "rise_slope_lssty",
+        "rise_slopesig_lssty",
+        "fall_slope_lsstg",
+        "fall_slopesig_lsstg",
+        "lsstg-lsstr_last",
+        "lsstr-lssti_last",
+        "lsstu-lsstg_peak",
+        "rise_slope_lsstr",
+        "rise_slopesig_lsstr",
+        "lsstg-lsstr_peak",
+        "lsstz-lssty_det",
+        "lssti-lsstz_peak",
+        "lsstr-lssti_peak",
+        "lssti-lsstz_det",
+        "lsstg-lsstr_det",
+        "lsstr-lssti_det",
+        "lsstu-lsstg_det",
+        "z",
+        "z_err",
+        "host_sep",
+    ]
 
     # Which units should this be changed to
-    t2_dependency: Sequence[StateT2Dependency[Literal["T2TabulatorRiseDecline", "T2ElasticcRedshiftSampler"]]]
-
+    t2_dependency: Sequence[
+        StateT2Dependency[
+            Literal["T2TabulatorRiseDecline", "T2ElasticcRedshiftSampler"]
+        ]
+    ]
 
     def post_init(self) -> None:
         """
         Load models
         """
 
         self._classifiers = {}
 
         for modelid, modelpath in self.model_dict.items():
-            fname = os.path.join(self.model_folder, modelpath )
+            fname = os.path.join(self.model_folder, modelpath)
             model = xgb.XGBClassifier()
             model.load_model(fname=fname)
-            self._classifiers[modelid] =  model
-
-
+            self._classifiers[modelid] = model
 
-    def process(self,
+    def process(
+        self,
         compound: T1Document,
         datapoints: Sequence[DataPoint],
-        t2_views: Sequence[T2DocView]
-    ) -> Union[UBson, UnitResult]:
+        t2_views: Sequence[T2DocView],
+    ) -> UBson | UnitResult:
         """
 
         Extract results from TabulatorRiseDecline and apply suitable model.
 
         Parameters
         -----------
 
         t2_records: List of T2Records from (here) TabulatorRiseDecline.
 
         Returns
         -------
         dict
         """
 
-
         t2data = {}
         # Parse t2views - should not be more than one.
         for t2_view in t2_views:
-            self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
+            self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
             # So far only knows how to parse phases from T2TabulatorRiseDecline
-            if t2_view.unit == 'T2TabulatorRiseDecline':
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+            if t2_view.unit == "T2TabulatorRiseDecline":
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
                 t2data.update(t2_res)
-            if t2_view.unit == 'T2ElasticcRedshiftSampler':
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+            if t2_view.unit == "T2ElasticcRedshiftSampler":
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
                 # For some reason we trained xgb using z, zerr and host_sep
-                zdata = {'z':None, 'z_err':None, 'host_sep': None}
-                if t2_res['z_source'] in ['HOSTGAL2_ZQUANT', 'HOSTGAL_ZQUANT', 'HOSTGAL_ZSPEC', 'default']:
-                    if len(t2_res['z_samples'])==3:
+                zdata = {"z": None, "z_err": None, "host_sep": None}
+                if t2_res["z_source"] in [
+                    "HOSTGAL2_ZQUANT",
+                    "HOSTGAL_ZQUANT",
+                    "HOSTGAL_ZSPEC",
+                    "default",
+                ]:
+                    if len(t2_res["z_samples"]) == 3:
                         # This was the sampling used for job_training
-                        zdata['z'] = t2_res['z_samples'][1]
-                        zdata['z_err'] = t2_res['z_samples'][1] - t2_res['z_samples'][0]
-                        zdata['host_sep'] = t2_res['host_sep']
-                    elif len(t2_res['z_samples'])==4 and t2_res['z_samples'][0]==0.01:
+                        zdata["z"] = t2_res["z_samples"][1]
+                        zdata["z_err"] = t2_res["z_samples"][1] - t2_res["z_samples"][0]
+                        zdata["host_sep"] = t2_res["host_sep"]
+                    elif (
+                        len(t2_res["z_samples"]) == 4 and t2_res["z_samples"][0] == 0.01
+                    ):
                         # ... unless the event was hostless, in which case
                         # xgboost use None values.
                         pass
                     else:
-                        self.logger.info('Do not know how to handle z info', extra=t2_res)
-                        return {'model': None, 'xgbsuccess': False}
+                        self.logger.info(
+                            "Do not know how to handle z info", extra=t2_res
+                        )
+                        return {"model": None, "xgbsuccess": False}
                 t2data.update(zdata)
 
-
         # If we did not find chained results from TabulatorRiseDecline,
         # then run the feature extraction
-        if not 'ndet' in t2data.keys():
+        if "ndet" not in t2data:
             flux_table = self.get_flux_table(datapoints)
 
             # Cut the flux table if requested
-            if self.max_ndet>0 and len(flux_table)>self.max_ndet:
+            if self.max_ndet > 0 and len(flux_table) > self.max_ndet:
                 flux_table = self.cut_flux_table(flux_table)
 
             # Calculate features
-            features = self.compute_stats(flux_table)
-            t2data.update( features )
-
-
-
+            try:
+                features = self.compute_stats(flux_table)
+            except FitFailed:
+                return UnitResult(code=DocumentCode.ERROR)
+            t2data.update(features)
 
         # No detections - none of the models will work
-        if t2data['ndet']==0:
+        if t2data["ndet"] == 0:
             # Explore whether negative detections can be used to parse type
-            if 'nnegdet' in t2data.keys() and t2data['nnegdet']>0:
-                if t2data['z'] is not None and t2data['z']>0.001:
+            if "nnegdet" in t2data and t2data["nnegdet"] > 0:
+                if t2data["z"] is not None and t2data["z"] > 0.001:
                     # High redshifts are typically AGNs
-                    return {'model': 'directEval', 'xgbsuccess': False, 'cause': 'No pos det', 'direct_eval':'AGN'}
-                else:
-                    # Low redshifts are (typically) either uLens or EB.
-                    # The former have a large fraction of neg det (if any)
-                    nfrac = float(t2data['nnegdet']) / t2data['alldet']
-                    if nfrac > 0.2:
-                        return {'model': 'directEval', 'xgbsuccess': False, 'cause': 'No pos det', 'direct_eval':'uLens'}
-                    else:
-                        return {'model': 'directEval', 'xgbsuccess': False, 'cause': 'No pos det', 'direct_eval':'EB'}
+                    return {
+                        "model": "directEval",
+                        "xgbsuccess": False,
+                        "cause": "No pos det",
+                        "direct_eval": "AGN",
+                    }
+                # Low redshifts are (typically) either uLens or EB.
+                # The former have a large fraction of neg det (if any)
+                nfrac = float(t2data["nnegdet"]) / t2data["alldet"]
+                if nfrac > 0.2:
+                    return {
+                        "model": "directEval",
+                        "xgbsuccess": False,
+                        "cause": "No pos det",
+                        "direct_eval": "uLens",
+                    }
+                return {
+                    "model": "directEval",
+                    "xgbsuccess": False,
+                    "cause": "No pos det",
+                    "direct_eval": "EB",
+                }
             # Otherwise, not much to go by
-            return {'model': 'directEval', 'xgbsuccess': False, 'imodel':-1, 'cause': 'No sig. det'}
-        if t2data['success']==False:
-            return {'model': 'directEval', 'xgbsuccess': False, 'imodel':-1, 'cause': 'RiseDecline error.'}
-
+            return {
+                "model": "directEval",
+                "xgbsuccess": False,
+                "imodel": -1,
+                "cause": "No sig. det",
+            }
+        if not t2data["success"]:
+            return {
+                "model": "directEval",
+                "xgbsuccess": False,
+                "imodel": -1,
+                "cause": "RiseDecline error.",
+            }
 
         # Loop through and apply all models
-        t2out: Dict[str, UBson] = {'model':'multiXgb'}
-        classifications = t2out['classifications'] = {}
+        t2out: dict[str, UBson] = {"model": "multiXgb"}
+        classifications = t2out["classifications"] = {}
         for modelid, model in self._classifiers.items():
             # Run model
             # Can we find away round creating a numpy array?
-            prob = model.predict_proba( np.array([ [t2data.get(col)
-                                        for col in self.use_cols] ]) )
+            prob = model.predict_proba(
+                np.array([[t2data.get(col) for col in self.use_cols]])
+            )
             classifications[modelid] = {
-                'prob0': float( prob[0][0] ),
-                'is_0': (float(prob[0][0])>0.5)
+                "prob0": float(prob[0][0]),
+                "is_0": (float(prob[0][0]) > 0.5),
             }
 
-
         return t2out
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,92 +3,91 @@
 # File:                Ampel-HU-astro/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
 # Date:                31.01.2021
 # Last Modified Date:  14.09.2021
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-from typing import Literal
 from collections.abc import Sequence
-from ampel.types import UBson
-from ampel.contrib.hu.t2.T2PanStarrThumbPrint import T2PanStarrThumbPrint
+from typing import Literal
+
 from ampel.abstract.AbsTiedPointT2Unit import AbsTiedPointT2Unit
-from ampel.util.collections import ampel_iter
 from ampel.content.DataPoint import DataPoint
+from ampel.contrib.hu.t2.T2PanStarrThumbPrint import T2PanStarrThumbPrint
+from ampel.enum.DocumentCode import DocumentCode
+from ampel.model.PlotProperties import FormatModel, PlotProperties
+from ampel.model.UnitModel import UnitModel
 from ampel.plot.create import create_plot_record
 from ampel.struct.UnitResult import UnitResult
-from ampel.model.PlotProperties import PlotProperties
-from ampel.model.UnitModel import UnitModel
+from ampel.types import UBson
+from ampel.util.collections import ampel_iter
 from ampel.view.T2DocView import T2DocView
-from ampel.enum.DocumentCode import DocumentCode
 
 
 class T2PS1ThumbExtCat(AbsTiedPointT2Unit):
-	"""
-	Retrieve panstarrs images at datapoint location and for each tied extcat catalog matching result:
-	- create a new image
-	- mark the datapoint location
-	- mark the matched location from the catalog
-
-	A dict structure containing each image as a compressed svg is returned.
-	"""
-
-	t2_dependency: Sequence[UnitModel[Literal['T2CatalogMatch']]]
-
-	cmaps: Sequence[str] = ["cividis"]
-	band: str | Sequence[str] = "g"
-	plot_props: PlotProperties = PlotProperties(
-		tags = ["THUMBPRINT", "PANSTARRS"],
-		file_name = {
-			"format_str": "%s_%s_%s_ps1_thumb.svg",
-			"arg_keys": ["stock", "band", "catalog"]
-		},
-		title = {
-			"format_str": "%s %s (%s band) ",
-			"arg_keys": ["stock", "catalog", "band"]
-		},
-		id_mapper = "ZTFIdMapper"
-	)
-
-
-	def process(self, datapoint: DataPoint, t2_views: Sequence[T2DocView]) -> UBson | UnitResult:
-		""" """
-
-		# That would be a config error
-		if not t2_views[0].is_point_type():
-			return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
-
-		cat_results = t2_views[0].get_payload()
-		if not isinstance(cat_results, dict):
-			return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
-
-		if 'data' not in cat_results:
-			return UnitResult(code=DocumentCode.T2_MISSING_INFO)
-
-		pt = T2PanStarrThumbPrint.get_ps1_target(datapoint, self.band)
-		plots = []
-
-		for cat_name, cat_res in cat_results['data'].items():
-
-			if not cat_res:
-				continue
-
-			for band in ampel_iter(self.band):
-				for cmap in ampel_iter(self.cmaps):
-					plots.append(
-						create_plot_record(
-							pt.show(
-								ellipse=False, band=band, cmap=cmap, show=False,
-								show_target = False, show_coord = (cat_res['ra'], cat_res['dec'])
-							),
-							self.plot_props,
-							extra = {
-								"band": band,
-								"stock": datapoint["stock"][0], # type: ignore[index]
-								"catalog": cat_name,
-								"cmap": cmap
-							},
-							logger = self.logger
-						)
-					)
+    """
+    Retrieve panstarrs images at datapoint location and for each tied extcat catalog matching result:
+    - create a new image
+    - mark the datapoint location
+    - mark the matched location from the catalog
+
+    A dict structure containing each image as a compressed svg is returned.
+    """
+
+    t2_dependency: Sequence[UnitModel[Literal["T2CatalogMatch"]]]
+
+    cmaps: Sequence[str] = ["cividis"]
+    band: str | Sequence[str] = "g"
+    plot_props: PlotProperties = PlotProperties(
+        tags=["THUMBPRINT", "PANSTARRS"],
+        file_name=FormatModel(
+            format_str="%s_%s_%s_ps1_thumb.svg", arg_keys=["stock", "band", "catalog"]
+        ),
+        title=FormatModel(
+            format_str="%s %s (%s band) ", arg_keys=["stock", "catalog", "band"]
+        ),
+        id_mapper="ZTFIdMapper",
+    )
+
+    def process(
+        self, datapoint: DataPoint, t2_views: Sequence[T2DocView]
+    ) -> UBson | UnitResult:
+        """ """
+
+        # That would be a config error
+        if not t2_views[0].is_point_type():
+            return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
+
+        cat_results = t2_views[0].get_payload()
+        if not isinstance(cat_results, dict):
+            return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
+
+        if "data" not in cat_results:
+            return UnitResult(code=DocumentCode.T2_MISSING_INFO)
+
+        pt = T2PanStarrThumbPrint.get_ps1_target(datapoint, self.band)
+        plots = [
+            create_plot_record(
+                pt.show(
+                    ellipse=False,
+                    band=band,
+                    cmap=cmap,
+                    show=False,
+                    show_target=False,
+                    show_coord=(cat_res["ra"], cat_res["dec"]),
+                ),
+                self.plot_props,
+                extra={
+                    "band": band,
+                    "stock": datapoint["stock"][0],  # type: ignore[index]
+                    "catalog": cat_name,
+                    "cmap": cmap,
+                },
+                logger=self.logger,
+            )
+            for cat_name, cat_res in cat_results["data"].items()
+            if cat_res
+            for band in ampel_iter(self.band)
+            for cmap in ampel_iter(self.cmaps)
+        ]
 
-		return {'data': {'plots': plots}}
+        return {"data": {"plots": plots}}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,118 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# File:                Ampel-HU-astro/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
+# File:                Ampel-HU-astro/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
-# Date:                12.09.2021
-# Last Modified Date:  14.10.2021
+# Date:                10.03.2021
+# Last Modified Date:  14.09.2021
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-from typing import Literal
 from collections.abc import Sequence
-from ampel.types import UBson
+from typing import Literal
+
+from ampel.abstract.AbsTiedPointT2Unit import AbsTiedPointT2Unit
+from ampel.content.DataPoint import DataPoint
 from ampel.contrib.hu.t2.T2PanStarrThumbPrint import T2PanStarrThumbPrint
-from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
-from ampel.util.collections import ampel_iter
-from ampel.plot.create import create_plot_record
+from ampel.contrib.hu.util.ned import check_ned_res
 from ampel.enum.DocumentCode import DocumentCode
+from ampel.model.PlotProperties import FormatModel, PlotProperties
+from ampel.model.UnitModel import UnitModel
+from ampel.plot.create import create_plot_record
 from ampel.struct.UnitResult import UnitResult
-from ampel.model.PlotProperties import PlotProperties
-from ampel.model.StateT2Dependency import StateT2Dependency
+from ampel.types import UBson
+from ampel.util.collections import ampel_iter
 from ampel.view.T2DocView import T2DocView
-from ampel.view.LightCurve import LightCurve
 
 
-class T2PS1ThumbNedSNCosmo(AbsTiedLightCurveT2Unit):
-	"""
-	This state t2 unit is tied with the state T2 unit T2NedSNCosmo.
-	It retrieves panstarrs images at a location encoded in the first datapoint and for each SNCosmo result:
-	- creates a new image
-	- marks the (first) datapoint location
-	- marks the matched location from the NED (encoded in the NedSNComso result under key 'ned')
-	"""
-
-	#: band: example: ["g", "r", "i", "z", "y"]
-	band: str | Sequence[str] = "g"
-	cmaps: Sequence[str] = ["cividis"]
-	plot_all: bool = False
-	z_range: None | tuple[float, float]
-	spectroscopic: bool = True
-	merge_tags: bool = True
-	# Copy selected keys from T2NedCosmo results such as 'fit_results' or 'sncosmo_info'
-	copy_keys: list[str] = []
-	t2_dependency: Sequence[StateT2Dependency[Literal['T2NedSNCosmo']]]
-
-	plot_props: PlotProperties = PlotProperties(
-		tags = ["THUMBPRINT", "PANSTARRS"],
-		file_name = {
-			"format_str": "%s_%s_%s_ps1_%s_%i_thumb.svg",
-			"arg_keys": ["stock", "obj_name", "band", "cmap", "index_pos"]
-		},
-		title = {
-			"format_str": "%s - %s\nz=%s (%s band, pos %i) ",
-			"arg_keys": ["stock", "obj_name", "z", "band", "index_pos"]
-		},
-		id_mapper = "ZTFIdMapper"
-	)
-
-
-	def process(self, light_curve: LightCurve, t2_views: Sequence[T2DocView]) -> UBson | UnitResult:
-		"""
-		:param light_curve: see "ampel.view.LightCurve" docstring for more info.
-		"""
-
-		if not light_curve.photopoints:
-			self.logger.info("Lightcurve does not contain any photopoints")
-			return UnitResult(code=DocumentCode.T2_MISSING_INFO)
-
-		# That would be a config error
-		if not t2_views[0].is_state_type():
-			return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
-
-		snc_result = t2_views[0].get_payload()
-		if not isinstance(snc_result, dict):
-			return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
-
-		if 'data' not in snc_result:
-			return UnitResult(code=DocumentCode.T2_MISSING_INFO)
-
-		if not isinstance(snc_result['data'], list):
-			return 1
-
-		ret: dict = {'data': []}
-		datapoint = light_curve.photopoints[0]
-		pt = T2PanStarrThumbPrint.get_ps1_target(datapoint, self.band)
-
-		for i, d in enumerate(snc_result['data']):
-
-			for k in ('model_analysis', 'fit_results'):
-				if k not in d:
-					self.logger.info(f"Skipping incompatible sncosmo with index {i} ('{k}' missing)")
-					continue
-
-			for k in ('has_premax_data', 'has_postmax_data'):
-				if not d.get('model_analysis', {}).get(k, False):
-					self.logger.info(f"Skipping sncosmo with index {i}: {k} is False or missing")
-					continue
-
-			for band in ampel_iter(self.band):
-				for cmap in ampel_iter(self.cmaps):
-					d2 = {
-						'plot': [
-							create_plot_record(
-								pt.show(
-									ellipse=False, band=band, cmap=cmap, show=False,
-									show_target = False, show_coord = (d['catalog']['ra'], d['catalog']['dec'])
-								),
-								self.plot_props,
-								extra = {
-									"band": band,
-									"stock": datapoint["stock"][0], # type: ignore[index]
-									"cmap": cmap,
-									"obj_name": d['catalog']['prefname'].replace(" ", "_"),
-									"z": d['catalog']['z'],
-									"index_pos": i
-								},
-								logger = self.logger
-							)
-						]
-					}
-
-					for k in self.copy_keys:
-						if k in d:
-							d2[k] = d[k]
-
-					ret['data'].append(d2)
-
-			if not self.plot_all:
-				break
-
-		# Assimilate T2NedSNCosmo tags into the T2PS1ThumbNedSNCosmo doc tags for convenience
-		if self.merge_tags:
-			return UnitResult(tag=t2_views[0].tag, body=ret if ret['data'] else None)
+class T2PS1ThumbNedTap(AbsTiedPointT2Unit):
+    """
+    This point t2 unit is tied with the point T2 unit T2NedTap.
+    It retrieves panstarrs images at a datapoint location and for each NED catalog matching result:
+    - creates a new image
+    - marks the datapoint location
+    - marks the matched location from the catalog
+
+    If you use custom 'ingest options', please make sure that these are the same between T2NedTap and T2NedTapPS1ThumbPrint.
+    Please note that the variant t2 class T2PS1ThumbNedSNCosmo exists and allows to restrict image retrieval
+    based on SNCosmo convergence criteria.
+
+    :param band: example: ["g", "r", "i", "z", "y"]
+    """
+
+    t2_dependency: Sequence[UnitModel[Literal["T2NedTap"]]]
+
+    cmaps: Sequence[str] = ["cividis"]
+    band: str | Sequence[str] = "g"
+    plot_all: bool = False
+    z_range: None | tuple[float, float]
+    spectroscopic: bool = True
+
+    plot_props: PlotProperties = PlotProperties(
+        tags=["THUMBPRINT", "PANSTARRS"],
+        file_name=FormatModel(
+            format_str="%s_%s_%s_ps1_%s_thumb.svg",
+            arg_keys=["stock", "obj_name", "band", "cmap"],
+        ),
+        title=FormatModel(
+            format_str="%s - %s z=%s (%s band) ",
+            arg_keys=["stock", "obj_name", "z", "band"],
+        ),
+        id_mapper="ZTFIdMapper",
+    )
+
+    def process(
+        self, datapoint: DataPoint, t2_views: Sequence[T2DocView]
+    ) -> UBson | UnitResult:
+        """ """
+
+        # That would be a config error
+        if not t2_views[0].is_point_type():
+            return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
+
+        cat_results = t2_views[0].get_payload()
+        if not isinstance(cat_results, dict):
+            return UnitResult(code=DocumentCode.T2_UNEXPECTED_DEPENDENCY)
+
+        if "data" not in cat_results:
+            return UnitResult(code=DocumentCode.T2_MISSING_INFO)
+
+        if not isinstance(cat_results["data"], list):
+            return 1
+
+        plots = []
+
+        for i, cat_res in enumerate(cat_results["data"]):
+            if check_ned_res(cat_res, self.logger, self.spectroscopic, self.z_range):
+                self.logger.info(f"Skipping cat result with index {i}")
+                continue
+
+            for band in ampel_iter(self.band):
+                pt = T2PanStarrThumbPrint.get_ps1_target(datapoint, band)
+
+                for cmap in ampel_iter(self.cmaps):
+                    plots.append(  # noqa: PERF401
+                        create_plot_record(
+                            pt.show(
+                                ellipse=False,
+                                band=band,
+                                cmap=cmap,
+                                show=False,
+                                show_target=False,
+                                show_coord=(cat_res["ra"], cat_res["dec"]),
+                            ),
+                            self.plot_props,
+                            extra={
+                                "band": band,
+                                "stock": datapoint["stock"][0],  # type: ignore[index]
+                                "cmap": cmap,
+                                "obj_name": cat_res["prefname"].replace(" ", "_"),
+                                "z": cat_res["z"],
+                            },
+                            logger=self.logger,
+                        )
+                    )
+
+            if not self.plot_all:
+                break
 
-		return ret if ret['data'] else None
+        return {"data": {"plots": plots}}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2PropagateStockInfo.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PropagateStockInfo.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,63 +3,61 @@
 # File:               ampel/contrib/hu/t2/T2PropagateStockInfo.py
 # License:            BSD-3-Clause
 # Author:             jnordin@physik.hu-berlin.de
 # Date:               04.01.2022
 # Last Modified Date: 04.01.2022
 # Last Modified By:   jnordin@physik.hu-berlin.de
 
-from functools import reduce
+from collections.abc import Generator
+from typing import Any
+
 from ampel.abstract.AbsStockT2Unit import AbsStockT2Unit
 
-def get_recursively(search_dict, field):
+
+def get_recursively(
+    search_dict: dict[str, Any], field: str
+) -> Generator[str, None, None]:
     """
     Takes a dict with nested lists and dicts,
     and searches all dicts for a key of the field
     provided.
     """
-    fields_found = []
 
     for key, value in search_dict.items():
-
         if key == field:
-            fields_found.append(key+'_found_'+value)
+            yield f"{key}_found_{value}"
 
         elif isinstance(value, dict):
-            results = get_recursively(value, field)
-            for result in results:
-                fields_found.append(key+'.'+result)
+            for result in get_recursively(value, field):
+                yield f"{key}.{result}"
 
         elif isinstance(value, list):
             for item in value:
                 if isinstance(item, dict):
-                    more_results = get_recursively(item, field)
-                    for another_result in more_results:
-                        fields_found.append(key+'.'+another_result)
-
-    return fields_found
+                    for result in get_recursively(item, field):
+                        yield f"{key}.{result}"
 
 
 class T2PropagateStockInfo(AbsStockT2Unit):
     """
     Collects a set of info from the transient stock collection and propagates.
-    Potentially useful as chained T2
+    Potentially useful as chained T2.
+
+    All entries are converted to strings.
+
     """
 
     # Paths to properties to search for
     # dict keys corresponds to output dict labels
     # dict values are reduce path list to intended values
-#    prop_paths: dict[str,list[str]] = {'explosion_time':['journal','healpix','time']}
-    prop_paths: dict[str,list[str]]
-
-
+    #    prop_paths: dict[str,list[str]] = {'explosion_time':['journal','healpix','time']}
+    prop_paths: dict[str, list[str]]
 
     def process(self, stock_doc):
-        print(stock_doc)
         outd = {}
         for label, pathlist in self.prop_paths.items():
-            paths = get_recursively(stock_doc, pathlist[-1])
-            for path in paths:
-                (dictpath, dictval) = path.split('_found_')
-                if '.'.join(pathlist)==dictpath:
+            for path in get_recursively(stock_doc, pathlist[-1]):
+                (dictpath, dictval) = path.split("_found_")
+                if ".".join(pathlist) == dictpath:
                     outd[label] = dictval
 
         return outd
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RiseDeclineStat.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RiseDeclineStat.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 # File:                ampel/contrib/hu/t2/T2LCQuality.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                28.12.2018
 # Last Modified Date:  03.08.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
+from typing import TYPE_CHECKING, Any
+
 import numpy as np
 from astropy.table import Table
-from typing import Any, TYPE_CHECKING
-from ampel.types import UBson
+
 from ampel.abstract.AbsLightCurveT2Unit import AbsLightCurveT2Unit
 from ampel.base.AmpelBaseModel import AmpelBaseModel
 from ampel.protocol.LoggerProtocol import LoggerProtocol
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 
 
 class T2RiseDeclineBase(AmpelBaseModel):
     """
     Derive a number of simple metrics describing the rise, peak and decline of a lc.
 
@@ -83,15 +85,14 @@
     # Through setting this we manually just keep the first of each occurance
     # Check ZTF18aacbccj,ZTF17aaaekyn for example. Has something to do whether a detection
     # is from a prv history or is new. Will for now use the one with highest rb
     # ZTF18aaaorhy is another funny case with a repeated mag.
     del_duplicate_rows: bool = True
 
     def compute_stats(self, light_curve: LightCurve) -> dict[str, Any]:
-
         # Output dict that we will start to populate
         o: dict[str, Any] = {}
 
         # Step 1. Base determinations based on combined detections
         self.logger.debug("Starting joint band RiseDeclineStat estimations")
 
         # Detection photo-points
@@ -111,15 +112,15 @@
         # cast to tables for convenience
         try:
             dets = Table(rows=pps, names=("jd", "filter", "magpsf", "sigmapsf", "rb"))
             o["cut_pp"] = 0
             if self.del_duplicate_rows:
                 unique_jd, counts = np.unique(dets["jd"], return_counts=True)
                 double_jd = list(unique_jd[(counts > 1)])
-                if not len(double_jd) == 0:
+                if len(double_jd) != 0:
                     self.logger.info(
                         "Cuting duplicate jd photopoints at %s" % (double_jd)
                     )
                     for jd in double_jd:
                         bDoubleJD = dets["jd"] == jd
                         MaxRb = dets["rb"][bDoubleJD].max()
                         bCut = dets["rb"][bDoubleJD] != MaxRb
@@ -178,15 +179,15 @@
             ulims = Table(rows=uls, names=("jd", "diffmaglim"))
             # Check for presence of upper limits after first detection
             if (ulims["jd"] > o["jd_det"]).sum() > 0:
                 o["bool_pure"] = False
             else:
                 o["bool_pure"] = True
             # Latest upper limit prior to detection
-            if np.any((ulims["jd"] < o["jd_det"])):
+            if np.any(ulims["jd"] < o["jd_det"]):
                 o["t_predetect"] = (
                     o["jd_det"] - ulims["jd"][(ulims["jd"] < o["jd_det"])].max()
                 )
             else:
                 o["t_predetect"] = None
         else:
             ulims = Table(([None], [None]), names=("jd", "diffmaglim"))
@@ -211,47 +212,43 @@
 
         det_mag_err = float(dets["sigmapsf"][dets["jd"] == o["jd_det"]])
         if (o["jd_last"] - min_mag_jd) < self.max_tsep:
             self.logger.info(
                 "Latest detection too close to peak light to calculate peak stats"
             )
             o["bool_peaked"] = False
+        elif (o["mag_last"] - min_mag) > np.sqrt(min_mag_err**2 + last_mag_err**2):
+            o["bool_peaked"] = True
         else:
-            if (o["mag_last"] - min_mag) > np.sqrt(
-                min_mag_err ** 2 + last_mag_err ** 2
-            ):
-                o["bool_peaked"] = True
-            else:
-                o["bool_peaked"] = False
+            o["bool_peaked"] = False
 
         # If we concluded a peak was there, collect info
         if o["bool_peaked"]:
-
             self.logger.debug("Calculating peak based statistics")
             o["jd_max"] = min_mag_jd
             o["mag_peak"] = min_mag
             o["bool_rising"] = False  # If it has peaked it is def not rising
 
             # Other chracteristics
             # Did it not rise at all?
             if (o["mag_det"] - o["mag_peak"]) > np.sqrt(
-                det_mag_err ** 2 + min_mag_err ** 2
+                det_mag_err**2 + min_mag_err**2
             ):
                 o["bool_norise"] = False
             else:
                 o["bool_norise"] = True
 
         else:
             self.logger.debug("Calculating statistics assuming no peak reached")
             o["jd_max"] = None
             o["mag_peak"] = None
 
             # Did it not rise at all from first detection detection?
             if (o["mag_det"] - o["mag_last"]) > np.sqrt(
-                det_mag_err ** 2 + last_mag_err ** 2
+                det_mag_err**2 + last_mag_err**2
             ):
                 o["bool_norise"] = False
             else:
                 o["bool_norise"] = True
 
             # Here it makese sense to check whether it is still rising
             if (o["jd_last"] - min_mag_jd) < self.max_tsep:
@@ -276,15 +273,14 @@
             if filtid not in self.filter_ids:
                 continue
 
             self.logger.debug(f"Starting slope fit filt {filtid}")
             filter_det = dets[dets["filter"] == filtid]
 
             if o["bool_peaked"]:
-
                 filter_det_rise = filter_det[filter_det["jd"] <= o["jd_max"]]
                 filter_det_fall = filter_det[filter_det["jd"] >= o["jd_max"]]
 
                 # Rise
                 # Check that lc had rise with sufficient detections
                 if o["bool_norise"] or filter_det_rise["jd"].size < 2:
                     o[f"slope_rise_{band}"] = None
@@ -308,31 +304,31 @@
                         filter_det_fall["magpsf"],
                         1,
                         w=1.0 / filter_det_fall["sigmapsf"],
                     )
                     o[f"slope_fall_{band}"] = p[0]
                 else:
                     o[f"slope_fall_{band}"] = None
+            # Will use all the data to fit rise parameter, set others to none
+            elif o["bool_norise"] or filter_det["jd"].size < 2:
+                o[f"slope_rise_{band}"] = None
             else:
-                # Will use all the data to fit rise parameter, set others to none
-                if o["bool_norise"] or filter_det["jd"].size < 2:
-                    o[f"slope_rise_{band}"] = None
-                else:
-                    p = np.polyfit(
-                        filter_det["jd"],
-                        filter_det["magpsf"],
-                        1,
-                        w=1.0 / filter_det["sigmapsf"],
-                    )
-                    o[f"slope_rise_{band}"] = p[0]
+                p = np.polyfit(
+                    filter_det["jd"],
+                    filter_det["magpsf"],
+                    1,
+                    w=1.0 / filter_det["sigmapsf"],
+                )
+                o[f"slope_rise_{band}"] = p[0]
 
         # Colors at specific phases
         for coljd, colname in zip(
             [o["jd_det"], o["jd_last"], o["jd_max"]],
             ["col_det", "col_last", "col_peak"],
+            strict=False,
         ):
             self.logger.debug(f"Checking col {colname} at jd {coljd}")
             # Check if time defined (e.g. if peak not known)
             if coljd is None:
                 o[colname] = None
                 continue
             dets_attime = dets[np.abs(dets["jd"] - coljd) <= self.max_tsep]
@@ -350,33 +346,32 @@
                 o[colname] = None
 
         o["success"] = True
         return o
 
 
 class T2RiseDeclineStat(AbsLightCurveT2Unit, T2RiseDeclineBase):
-
     do_testplot: bool = False
     path_testplot: str = "/home/jnordin/tmp/t2test/"
 
     def test_plot(self, dets, ulims, outdict, path):
         """
         but useful for debugging
         """
 
         import matplotlib.pyplot as plt
 
         # Lightcurve
-        for filtid in self.default_filter_ids:
+        for name, filtid in self.filters.items():
             filter_det = dets[dets["filter"] == filtid]
             plt.plot(
                 filter_det["jd"],
                 filter_det["magpsf"],
                 "o",
-                label="Filt %s" % (self.default_filter_names[filtid]),
+                label=f"Filt {name}",
             )
 
         plt.plot(ulims["jd"], ulims["diffmaglim"], "o", label="ulims")
         # plt.plot(jd_int, interp_lc(jd_int), label="interp")
         plt.gca().invert_yaxis()
 
         # Detection props
@@ -388,24 +383,19 @@
             plt.axvline(outdict["jd_last"], label="Last")
 
         plt.legend()
         plt.xlabel("JD")
         plt.ylabel("Mag")
 
         # Create text string
-        title = "ndet: %s rb %.2f drb %.2f " % (
-            outdict["ndet"],
-            outdict["rb_med"],
-            outdict["drb_med"],
-        )
+        title = f'ndet: {outdict["ndet"]} rb {outdict["rb_med"]:.2f} drb {outdict["drb_med"]:.2f} '
 
         for boolprop in ["peaked", "pure", "rising", "norise", "hasgaps"]:
             if outdict[f"bool_{boolprop}"]:
                 title += f"{boolprop} "
 
         plt.title(title)
         plt.savefig(path)
         plt.clf()
 
     def process(self, light_curve: LightCurve) -> UBson | UnitResult:
-
         return self.compute_stats(light_curve)
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunParsnip.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunParsnip.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,68 +3,70 @@
 # File              : ampel/contrib/hu/t2/T2RunParsnip.py
 # License           : BSD-3-Clause
 # Author            : jnordin@physik.hu-berlin.de
 # Date              : 24.09.2021
 # Last Modified Date: 06.04.2022
 # Last Modified By  : jnordin@physik.hu-berlin.de
 
-from typing import Sequence, Literal, Optional
-import os, backoff
-from scipy.stats import chi2
 import gc
-import numpy as np
-from astropy.table import Table
+import os
+import warnings
+from collections.abc import Sequence
+from typing import Literal
+
+import backoff
 import matplotlib.pyplot as plt
-import timeout_decorator
+import numpy as np
 import packaging
 import scipy
-import warnings
+import timeout_decorator
+from astropy.table import Table
+from scipy.stats import chi2
 
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.abstract.AbsTabulatedT2Unit import AbsTabulatedT2Unit
-from ampel.content.T1Document import T1Document
+from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.content.DataPoint import DataPoint
-from ampel.view.T2DocView import T2DocView
-from ampel.enum.DocumentCode import DocumentCode
+from ampel.content.T1Document import T1Document
 from ampel.model.StateT2Dependency import StateT2Dependency
-from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
+from ampel.view.T2DocView import T2DocView
 
 # do not warning about scipy.stats.mode(keepdims=None)
-if packaging.version.parse(scipy.__version__) < packaging.version.parse('1.11'):
-    warnings.filterwarnings("ignore", category=FutureWarning, module="parsnip.light_curve", lineno=31)
+if packaging.version.parse(scipy.__version__) < packaging.version.parse("1.11"):
+    warnings.filterwarnings(
+        "ignore", category=FutureWarning, module="parsnip.light_curve", lineno=31
+    )
 
-import parsnip
+import extinction  # type: ignore[import]
 import lcdata
+import parsnip
+import sncosmo  # type: ignore[import]
 
 # The following three only used if correcting for MW dust
-from sfdmap import SFDMap  # type: ignore[import]
-import sncosmo             # type: ignore[import]
-import extinction          # type: ignore[import]
-
-
+from sfdmap2.sfdmap import SFDMap  # type: ignore[import]
 
 # All parsnip predictions that are not floats
 dcast_pred = {
-    'object_id' : str,
-    'type' : str,
-    'count' : int,
-    'count_s2n_3' : int,
-    'count_s2n_5' : int,
-    'count_s2n_3_pre' : int,
-    'count_s2n_3_rise' : int,
-    'count_s2n_3_post' : int,
-    'model_dof' : int,
+    "object_id": str,
+    "type": str,
+    "count": int,
+    "count_s2n_3": int,
+    "count_s2n_5": int,
+    "count_s2n_3_pre": int,
+    "count_s2n_3_rise": int,
+    "count_s2n_3_post": int,
+    "model_dof": int,
 }
 
 dcast_class = {
-    'object_id' : str,
+    "object_id": str,
 }
 
+
 class T2RunParsnip(AbsTiedStateT2Unit, AbsTabulatedT2Unit):
     """
     Gathers information and runs the parsnip model and classifier.
     - Obtain model (read from file unless not in sncosmo registry)
     - Parse previous (chained) T2results for redshift or phase limits.
     - Creates suitable photometry, using the converter provided and  phase limits.
     - Defines model appropritately, including fit ranges and fixed parameters.
@@ -75,239 +77,243 @@
     - Add option for redoing fits with disturbed initial conditions to avoid local minima
     - Add option for masking data?
     """
 
     # Name (in case standard) or path to parsnip model to load
     parsnip_model: str
     # Path to classifier to apply to lightcurve fit. If not set, no classification will be done.
-    parsnip_classifier: Optional[str]
+    parsnip_classifier: None | str
 
     # Redshift usage options. Current options
     # T2MatchBTS : Use the redshift published by BTS and  synced by that T2.
     # T2DigestRedshifts : Use the best redshift as parsed by DigestRedshift.
     # T2ElasticcRedshiftSampler: Use a list of redshifts and weights from the sampler.
     # None : run sncosmo template fit with redshift as free parameter OR use backup_z if set
-    redshift_kind: Optional[str]
+    redshift_kind: None | str
     # If loading redshifts from DigestRedshifts, provide the max ampel z group to make use of.
     # (note that filtering based on this can also be done for a potential t3)
     max_ampelz_group: int = 3
     # It is also possible to use fixed redshift whenever a dynamic redshift kind is not possible
     # This could be either a single value or a list
-    fixed_z: Optional[float | Sequence[float]]
+    fixed_z: None | float | Sequence[float]
     # Finally, the provided lens redshift might be multiplied with a scale
     # Useful for lensing studies, or when trying multiple values
-    scale_z: Optional[float]
+    scale_z: None | float
 
     max_fit_z: None | float = None
 
     # Remove MW dust absorption.
     # MWEBV is either derived from SFD maps using the position from light_curve
     # (assuming the SFD_DIR env var is set) OR retrieved from stock (ELASTICHOW?)
     # The default value of Rv will be used.
     apply_mwcorrection: bool = False
 
-
     # Further fit parameters
     # Bounds - not yet implemented
     # sncosmo_bounds : Dict[ str, List[float] ] = {}
     # Remove MW dust absorption using SFD maps.
-	# assumes that the position can be retrieved from the light_curve and
+    # assumes that the position can be retrieved from the light_curve and
     # that the SFD_DIR env var is set to allow them to be found.
-	# The default value of Rv will be used.
+    # The default value of Rv will be used.
     # apply_mwcorrection : bool = False
 
     # Phase range usage. Current option:
     # T2PhaseLimit : use the jdmin jdmax provided in this unit output
     # None : use full datapoint range
     # (T2BayesianBlocks should be added)
-    phaseselect_kind: Optional[str]
+    phaseselect_kind: None | str
 
     # Abort veto (if fulfilled, skip run)
-    abort_map: Optional[dict[str, list]]
+    abort_map: None | dict[str, list]
 
     # Zeropoint parameters
     # These are separately set in the Parsnip model settings. The zeropoint
     # can does vary between input data, training data and the model.
     # Try to adjust this relative to the 'zp' field of the input tabulated lc
-    training_zeropoint: float = 27.5    # Used in Elasticc training sample
-    default_zeropoint: float = 25.      # Default parsnip value
-
+    training_zeropoint: float = 27.5  # Used in Elasticc training sample
+    default_zeropoint: float = 25.0  # Default parsnip value
 
     # Save / plot parameters
-    plot_suffix: Optional[str]
-    plot_dir: Optional[str]
-
+    plot_suffix: None | str
+    plot_dir: None | str
 
     # Which units should this be changed to
-    t2_dependency: Sequence[StateT2Dependency[Literal[
-        "T2ElasticcRedshiftSampler",
-        "T2DigestRedshifts",
-        "T2MatchBTS",
-        "T2PhaseLimit",
-        "T2XgbClassifier"]]]
-
-
+    t2_dependency: Sequence[
+        StateT2Dependency[
+            Literal[
+                "T2ElasticcRedshiftSampler",
+                "T2DigestRedshifts",
+                "T2MatchBTS",
+                "T2PhaseLimit",
+                "T2XgbClassifier",
+            ]
+        ]
+    ]
 
-
-    def post_init(self)-> None:
+    def post_init(self) -> None:
         """
         Retrieve models.
         """
 
         # Load model and classifier
         self.model = parsnip.load_model(self.parsnip_model, threads=1)
         self.classifier = None
         if self.parsnip_classifier:
             self.classifier = parsnip.Classifier.load(self.parsnip_classifier)
 
         if self.apply_mwcorrection:
             self.dustmap = SFDMap()
 
-
-
-    def _get_redshift(self, t2_views) -> tuple[Optional[list[float]], Optional[str], Optional[list[float]]]:
+    def _get_redshift(
+        self, t2_views
+    ) -> tuple[None | list[float], None | str, None | list[float]]:
         """
         Can potentially also be replaced with some sort of T2DigestRershift tabulator?
 
         Assuming that only one instance of redshift sources exist
         """
 
         # Examine T2s for eventual information
-        z: Optional[list[float]] = None
-        z_source: Optional[str] = None
-        z_weights: Optional[list[float]] = None
-
-
-        if self.redshift_kind in ['T2MatchBTS', 'T2DigestRedshifts', 'T2ElasticcRedshiftSampler']:
+        z: None | list[float] = None
+        z_source: None | str = None
+        z_weights: None | list[float] = None
+
+        if self.redshift_kind in [
+            "T2MatchBTS",
+            "T2DigestRedshifts",
+            "T2ElasticcRedshiftSampler",
+        ]:
             for t2_view in t2_views:
-                if not t2_view.unit == self.redshift_kind:
+                if t2_view.unit != self.redshift_kind:
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
                 # Parse this
-                if self.redshift_kind == 'T2MatchBTS':
-                    if 'bts_redshift' in t2_res.keys() and not t2_res['bts_redshift'] == '-':
-                        z = [float(t2_res['bts_redshift'])]
+                if self.redshift_kind == "T2MatchBTS":
+                    if "bts_redshift" in t2_res and t2_res["bts_redshift"] != "-":
+                        z = [float(t2_res["bts_redshift"])]
                         z_source = "BTS"
-                elif self.redshift_kind == 'T2DigestRedshifts':
-                    if ('ampel_z' in t2_res.keys() and t2_res['ampel_z'] is not None
-                            and t2_res['group_z_nbr'] <= self.max_ampelz_group):
-                        z = [float(t2_res['ampel_z'])]
-                        z_source = "AMPELz_group" + str(t2_res['group_z_nbr'])
-                elif self.redshift_kind == 'T2ElasticcRedshiftSampler':
-                    z = t2_res['z_samples']
-                    z_source = t2_res['z_source']
-                    z_weights = t2_res['z_weights']
-        else:
-            # Check if there is a fixed z set for this run, otherwise keep as free parameter
-            if self.fixed_z is not None:
-                if isinstance(self.fixed_z, float):
-                    z = [self.fixed_z]
-                else:
-                    z = list(self.fixed_z)
-                z_source = "Fixed"
+                elif self.redshift_kind == "T2DigestRedshifts":
+                    if (
+                        "ampel_z" in t2_res
+                        and t2_res["ampel_z"] is not None
+                        and t2_res["group_z_nbr"] <= self.max_ampelz_group
+                    ):
+                        z = [float(t2_res["ampel_z"])]
+                        z_source = "AMPELz_group" + str(t2_res["group_z_nbr"])
+                elif self.redshift_kind == "T2ElasticcRedshiftSampler":
+                    z = t2_res["z_samples"]
+                    z_source = t2_res["z_source"]
+                    z_weights = t2_res["z_weights"]
+        # Check if there is a fixed z set for this run, otherwise keep as free parameter
+        elif self.fixed_z is not None:
+            if isinstance(self.fixed_z, float):
+                z = [self.fixed_z]
             else:
-                z = None
-                z_source = "Fitted"
+                z = list(self.fixed_z)
+            z_source = "Fixed"
+        else:
+            z = None
+            z_source = "Fitted"
 
         if (z is not None) and (z_source is not None) and self.scale_z:
-            z = [onez*self.scale_z for onez in z]
-            z_source += " + scaled {}".format(self.scale_z)
-
+            z = [onez * self.scale_z for onez in z]
+            z_source += f" + scaled {self.scale_z}"
 
         return z, z_source, z_weights
 
     def _get_abort(self, t2_views) -> tuple[bool, dict]:
         """
         Check potential previous t2s for whether the run should be aborted.
         (For perfomance reasons).
 
         Implemented case is concerns T2XgbClassifier.
         """
 
-        if not self.abort_map or len(self.abort_map)==0:
+        if not self.abort_map or len(self.abort_map) == 0:
             # Not looking for any
             return (False, {})
 
         abort, abort_maps = False, {}
         for t2_view in t2_views:
-            if not t2_view.unit in self.abort_map.keys():
+            if t2_view.unit not in self.abort_map:
                 continue
-            self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
+            self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
             t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
             abort_maps.update(t2_res)
 
             for abort_map in self.abort_map[t2_view.unit]:
-                if all(t2_res.get(key, None) == val for key, val
-                                 in abort_map.items()):
+                if all(t2_res.get(key, None) == val for key, val in abort_map.items()):
                     abort = True
 
         return (abort, abort_maps)
 
-
-    def _get_phaselimit(self, t2_views) -> tuple[Optional[float], Optional[float]]:
+    def _get_phaselimit(self, t2_views) -> tuple[None | float, None | float]:
         """
         Can potentially also be replaced with some sort of tabulator?
 
         """
 
         # Examine T2s for eventual information
-        jdstart: Optional[float] = None
-        jdend: Optional[float] = None
+        jdstart: None | float = None
+        jdend: None | float = None
 
         if self.phaseselect_kind is None:
             jdstart = -np.inf
             jdend = np.inf
         else:
-
             for t2_view in t2_views:
                 # So far only knows how to parse phases from T2PhaseLimit
-                if not t2_view.unit == 'T2PhaseLimit':
+                if t2_view.unit != "T2PhaseLimit":
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
-                jdstart = t2_res['t_start']
-                jdend = t2_res['t_end']
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
+                jdstart = t2_res["t_start"]
+                jdend = t2_res["t_end"]
 
         return jdstart, jdend
 
-
     def _deredden_mw_extinction(self, ebv, phot_tab, rv=3.1) -> Table:
         """
         For an input photometric table, try to correct for mw extinction.
         """
 
         # Find effective wavelength for all filters in phot_tab
-        filterlist = set( phot_tab['band'] )
+        filterlist = set(phot_tab["band"])
         eff_wave = [sncosmo.get_bandpass(f).wave_eff for f in filterlist]
 
         # Determine flux correction (dereddening) factors
-        flux_corr = 10**(0.4* extinction.ccm89( np.array(eff_wave), ebv*rv, rv) )
+        flux_corr = 10 ** (0.4 * extinction.ccm89(np.array(eff_wave), ebv * rv, rv))
 
         # Assign this appropritately to Table
-        phot_tab['flux_original'] = phot_tab['flux']
-        phot_tab['fluxerr_original'] = phot_tab['fluxerr']
+        phot_tab["flux_original"] = phot_tab["flux"]
+        phot_tab["fluxerr_original"] = phot_tab["fluxerr"]
         for k, band in enumerate(filterlist):
-            phot_tab['flux'][(phot_tab['band']==band)] *= flux_corr[k]
-            phot_tab['fluxerr'][(phot_tab['band']==band)] *= flux_corr[k]
+            phot_tab["flux"][(phot_tab["band"] == band)] *= flux_corr[k]
+            phot_tab["fluxerr"][(phot_tab["band"] == band)] *= flux_corr[k]
 
         return phot_tab
 
     @backoff.on_exception(
         backoff.constant,
         timeout_decorator.timeout_decorator.TimeoutError,
         max_tries=3,
     )
     @timeout_decorator.timeout(5, use_signals=True)
     def _classify_parsnip(self, predictions):
         """
         Carry out the parsnip classification.
         """
-
-        return self.classifier.classify(predictions)
+        if self.classifier is not None:
+            return self.classifier.classify(predictions)
+        raise RuntimeError("No classifier configured")
 
     @backoff.on_exception(
         backoff.constant,
         timeout_decorator.timeout_decorator.TimeoutError,
         max_tries=3,
     )
     @timeout_decorator.timeout(5, use_signals=True)
@@ -316,18 +322,19 @@
         Carry out the parsnip predictions.
         """
         return self.model.predict_dataset(dataset)
 
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self,
-                compound: T1Document,
-                datapoints: Sequence[DataPoint],
-                t2_views: Sequence[T2DocView]
+    def process(
+        self,
+        compound: T1Document,
+        datapoints: Sequence[DataPoint],
+        t2_views: Sequence[T2DocView],
     ) -> UBson | UnitResult:
         """
 
         Fit the parameters of the initiated snocmo_model to the light_curve
         provided. Depending on the configuration, the provided T2DovViews
         are used to look for redshift information and any phase (time)
         limits for the fit.
@@ -345,157 +352,166 @@
 
         Returns
         -------
         dict
         """
 
         # Initialize output dict
-        t2_output: dict[str, UBson] = {"model" : self.parsnip_model,
-		                              "classifier" : self.parsnip_classifier}
+        t2_output: dict[str, UBson] = {
+            "model": self.parsnip_model,
+            "classifier": self.parsnip_classifier,
+        }
 
         # Check whether no computation should be done (due to previous fit)
         (abort_run, abort_info) = self._get_abort(t2_views)
-        t2_output['abort_maps'] = abort_info
+        t2_output["abort_maps"] = abort_info
         if abort_run:
-            t2_output['aborted'] = True
+            t2_output["aborted"] = True
             return t2_output
 
-
         # Check for phase limits
         (jdstart, jdend) = self._get_phaselimit(t2_views)
-        t2_output['jdstart'] = jdstart
-        t2_output['jdend'] = jdend
-        if t2_output['jdstart'] is None:
+        t2_output["jdstart"] = jdstart
+        t2_output["jdend"] = jdend
+        if t2_output["jdstart"] is None:
             return t2_output
 
         # Obtain photometric table
         sncosmo_table = self.get_flux_table(datapoints)
         sncosmo_table = sncosmo_table[
-                                    (sncosmo_table["time"]>=jdstart) &
-                                    (sncosmo_table["time"]<=jdend)
-                                    ]
-        self.logger.debug('Sncosmo table {}'.format(sncosmo_table))
+            (sncosmo_table["time"] >= jdstart) & (sncosmo_table["time"] <= jdend)
+        ]
+        self.logger.debug(f"Sncosmo table {sncosmo_table}")
 
         # Adjust zeropoint - does this matter? and should we have changed it?
-        run_zeropoints = set( sncosmo_table['zp'] )
-        if len(run_zeropoints)>1:
-            self.logger.info('Warning, multiple zeropoints, using avg.')
+        run_zeropoints = set(sncosmo_table["zp"])
+        if len(run_zeropoints) > 1:
+            self.logger.info("Warning, multiple zeropoints, using avg.")
             run_zeropoint = np.mean(list(run_zeropoints))
         else:
             run_zeropoint = run_zeropoints.pop()
-        self.model.settings['zeropoint'] = self.default_zeropoint + run_zeropoint - self.training_zeropoint
-
+        self.model.settings["zeropoint"] = (
+            self.default_zeropoint + run_zeropoint - self.training_zeropoint
+        )
 
         # Potentially correct for dust absorption
         if self.apply_mwcorrection:
             # Get ebv from coordiantes.
             # Here there should be some option to read it from journal/stock etc
             mwebv = self.dustmap.ebv(*self.get_pos(datapoints, which="mean"))
-            t2_output['mwebv'] = mwebv
+            t2_output["mwebv"] = mwebv
             sncosmo_table = self._deredden_mw_extinction(mwebv, sncosmo_table)
 
-
         ## Obtain redshift(s) from catalog fit or a RedshiftSample
         z, z_source, z_weights = self._get_redshift(t2_views)
-        t2_output['z'] = z
-        t2_output['z_source'] = z_source
-        t2_output['z_weights'] = z_weights
+        t2_output["z"] = z
+        t2_output["z_source"] = z_source
+        t2_output["z_weights"] = z_weights
         # A source class of None indicates that a redshift source was required, but not found.
         if z is None or z_source is None:
             return t2_output
 
         # If redshift should be fitted, we start with getting samples
-        if z_source == 'Fitted':
-            if not hasattr(self.model, 'predict_redshift_distribution'):
-                self.logger.warn("Redshift fitting is not supported in that version of parsnip")
+        if z_source == "Fitted":
+            if not hasattr(self.model, "predict_redshift_distribution"):
+                self.logger.warn(
+                    "Redshift fitting is not supported in that version of parsnip"
+                )
                 return t2_output
             z, z_probabilities = self.model.predict_redshift_distribution(
-                                sncosmo_table, max_redshift=self.max_fit_z)
+                sncosmo_table, max_redshift=self.max_fit_z
+            )
         assert z is not None
 
         # Create a list of lightcurves, each at a discrete redshift
         lcs = []
         for redshift in z:
             use_lc = sncosmo_table.copy()
-            use_lc.meta['object_id']  = f'parsnip_z{redshift:4f}'
-            use_lc.meta['redshift'] = redshift
+            use_lc.meta["object_id"] = f"parsnip_z{redshift:4f}"
+            use_lc.meta["redshift"] = redshift
             lcs.append(use_lc)
         lc_dataset = lcdata.from_light_curves(lcs)
 
         lc_predictions = self._predict_parsnip(lc_dataset)
         lc_classifications = self._classify_parsnip(lc_predictions)
 
-
         # Cast result for storage and look at relative probabilities
         predictions = {}
         classifcations = {}
         for i, redshift in enumerate(z):
             foo = dict(lc_predictions[i][lc_predictions.colnames[1:]])
-            predictions[str(redshift)] = {k: dcast_pred[k](v)
-                                        if k in dcast_pred and v is not None
-								        else float(v) for k, v in foo.items()}
+            predictions[str(redshift)] = {
+                k: dcast_pred[k](v) if k in dcast_pred and v is not None else float(v)
+                for k, v in foo.items()
+            }
             # Not sure whether the dof could change? Normalizing now
-            if foo['model_dof']>0:
-                predictions[str(redshift)]['chi2pdf'] = chi2.pdf(
-                                        foo['model_chisq'], foo['model_dof'] )
+            if foo["model_dof"] > 0:
+                predictions[str(redshift)]["chi2pdf"] = chi2.pdf(
+                    foo["model_chisq"], foo["model_dof"]
+                )
             else:
                 # Not enough data - earlier check?
-                predictions[str(redshift)]['chi2pdf'] = 0.
+                predictions[str(redshift)]["chi2pdf"] = 0.0
             foo = dict(lc_classifications[i][lc_classifications.colnames[1:]])
-            classifcations[str(redshift)] = {k: dcast_class[k](v)
-		                                  if k in dcast_class and v is not None
-									      else float(v) for k, v in foo.items()}
+            classifcations[str(redshift)] = {
+                k: dcast_class[k](v) if k in dcast_class and v is not None else float(v)
+                for k, v in foo.items()
+            }
 
         # Marginalize over the redshift
         # p(c|y) = Integral[p(c|z,y) p(z|y) dz]
         types = lc_classifications.colnames[1:]
         dtype = lc_classifications[types[0]].dtype
         probabilities = lc_classifications[types].as_array().view((dtype, len(types)))
         # Now we could normalize these z prob and normalize types over redshifts
-        z_probabilities = np.array( [lcfit['chi2pdf']
-                    for redshift, lcfit in predictions.items()] )
+        z_probabilities = np.array(
+            [lcfit["chi2pdf"] for redshift, lcfit in predictions.items()]
+        )
 
         t2_output["predictions"] = predictions
         t2_output["classifications"] = classifcations
 
-        if np.sum(z_probabilities)>0:
+        if np.sum(z_probabilities) > 0:
             # Take redshift probabilities into account, if available
             if z_weights is not None:
                 z_probabilities *= z_weights
             integrated_probabilities = z_probabilities.dot(probabilities)
             integrated_probabilities /= np.sum(integrated_probabilities)
-            t2_output["marginal_lc_classifications"] = dict(zip(types, integrated_probabilities))
+            t2_output["marginal_lc_classifications"] = dict(
+                zip(types, integrated_probabilities, strict=False)
+            )
             # Find the best redshifts
             t2_output["z_at_minchi"] = z[np.argmax(z_probabilities)]
             # Map these to singular value predictions/lc_classifications
             # (wastes DB space, but possible to filter based on)
             t2_output["prediction"] = predictions[str(t2_output["z_at_minchi"])]
             t2_output["classification"] = classifcations[str(t2_output["z_at_minchi"])]
         else:
             # Not enough data for a chi2 estimate
-            t2_output["Failed"] = 'NoDOF'
+            t2_output["Failed"] = "NoDOF"
             return t2_output
 
         # Plot
         if self.plot_suffix and self.plot_dir:
-
             # How to construct name?
-            tname = compound.get('stock')
+            tname = compound.get("stock")
             # Need plotting tools to define id mapper
-            #tname = ZTFIdMapper.to_ext_id(light_curve.stock_id)
+            # tname = ZTFIdMapper.to_ext_id(light_curve.stock_id)
 
             fig = plt.figure()
             ax = plt.gca()
 
             # Set redshift to best value and plot this fit
-            lc_dataset.light_curves[0].meta['redshift'] = t2_output["z_at_minchi"]
+            lc_dataset.light_curves[0].meta["redshift"] = t2_output["z_at_minchi"]
 
             parsnip.plot_light_curve(lc_dataset.light_curves[0], self.model, ax=ax)
             plt.tight_layout()
-            plt.savefig(os.path.join(self.plot_dir, 't2parsnip_%s.%s'%(tname, self.plot_suffix)))
-
-            plt.close('fig')
-            plt.close('all')
-            del(fig)
+            plt.savefig(
+                os.path.join(self.plot_dir, f"t2parsnip_{tname}.{self.plot_suffix}")
+            )
+
+            plt.close("fig")
+            plt.close("all")
+            del fig
             gc.collect()
 
         return t2_output
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunSncosmo.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSncosmo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                ampel/contrib/hu/t2/T2RunSncosmo.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                11.05.2021
-# Last Modified Date:  19.10.2022
-# Last Modified By:    alice.townsend@physik.hu-berlin.de
+# Last Modified Date:  18.02.2022
+# Last Modified By:    simeon.reusch@desy.de
 
 
-from typing import Literal
+import copy
+import errno
+import os
 from collections.abc import Sequence
-import errno, backoff, copy
-
+from typing import Literal
 
+import backoff
 import numpy as np
-import sncosmo # type: ignore[import]
+import sncosmo  # type: ignore[import]
+from sfdmap2.sfdmap import SFDMap  # type: ignore[import]
 from sncosmo.fitting import DataQualityError
-from astropy.table import Table
-from sfdmap import SFDMap  # type: ignore[import]
 
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
-from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.abstract.AbsTabulatedT2Unit import AbsTabulatedT2Unit
-from ampel.content.T1Document import T1Document
+from ampel.abstract.AbsTiedStateT2Unit import AbsTiedStateT2Unit
 from ampel.content.DataPoint import DataPoint
-from ampel.view.T2DocView import T2DocView
-from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
+from ampel.content.T1Document import T1Document
+from ampel.model.PlotProperties import PlotProperties
 from ampel.model.StateT2Dependency import StateT2Dependency
 from ampel.plot.create import create_plot_record
-from ampel.model.PlotProperties import PlotProperties
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
+from ampel.view.T2DocView import T2DocView
+from ampel.ztf.util.ZTFNoisifiedIdMapper import ZTFNoisifiedIdMapper
 
 
 class T2RunSncosmo(AbsTiedStateT2Unit, AbsTabulatedT2Unit):
     """
     Gathers information and runs Sncosmo. Steps include:
     - Obtain model (read from file unless not in sncosmo registry)
     - Parse previous (chained) T2results for redshift or phase limits.
@@ -78,27 +79,30 @@
     # Parameters regulating model
     # This unit requires that the model either exists in the current registry, or can be retrieved.
     # Non-standard models thus first have to be stored into the registry as part of the AMPEL init.
     sncosmo_model_name: str
 
     # Redshift usage options. Current options
     # T2MatchBTS : Use the redshift published by BTS and  synced by that T2.
+    # T2LoadRedshift: Use the redshift from a separate df.
     # T2DigestRedshifts : Use the best redshift as parsed by DigestRedshift.
     # None : run sncosmo template fit with redshift as free parameter OR use backup_z if set
     redshift_kind: None | str
     # If loading redshifts from DigestRedshifts, provide the max ampel z group to make use of.
     # (note that filtering based on this can also be done for a potential t3)
     max_ampelz_group: int = 3
+    # If none of the above is selected, a fixed redshift can be provided.
+    # If this is None, the redshift will be included as a free parameter in the fit
+    fixed_z: None | float
     # It is also possible to use fixed redshift whenever a dynamic redshift kind is not possible
     backup_z: None | float
     # Finally, the provided lens redshift might be multiplied with a scale
     # Useful for lensing studies, or when trying multiple values
     scale_z: None | float
 
-
     # Sncosmo parameters
     # Bounds - This is propagated directly into sncosmo. Beware e.g. clashed with catalog redshifts
     # When fitting redshift this needs to be included here, e.g. "sncosmo_bounds": {"z":(0.001,0.3)}
     sncosmo_bounds: dict[str, list[float]] = {}
     # Remove MW dust absorption using SFD maps. This assumes that the position
     # can be retrieved from the light_curve and that the SFD_DIR env var is set
     # to allow them to be found. The default value of Rv will be used.
@@ -106,207 +110,272 @@
 
     # Phase range usage. Current option:
     # T2PhaseLimit : use the jdmin jdmax provided in this unit output
     # None : use full datapoint range
     # (T2BayesianBlocks should be added)
     phaseselect_kind: None | str
 
+    noisified: bool = False
+
     # Plot parameters
     plot_db: bool = False
-    plot_props: None | PlotProperties = None
-
-    # Which units should this be changed to
-    t2_dependency: Sequence[StateT2Dependency[Literal[
-                            "T2DigestRedshifts", "T2MatchBTS", "T2PhaseLimit"]]]
-
+    plot_props: None | PlotProperties = None  # Plot properties for SvgRecord creation
+    plot_matplotlib_suffix: None | str = None  # Suffix if stored (locally) through matplotlib (e.g. _crayzmodel.png). Will add transient name
+    plot_matplotlib_dir: str = "."  # Suffix if stored (locally) through matplotlib (e.g. _crayzmodel.png). Will add transient name
+
+    # Units from which time limits to use or redshifts can be picked.
+    t2_dependency: Sequence[
+        StateT2Dependency[
+            Literal[
+                "T2ElasticcRedshiftSampler",
+                "T2DigestRedshifts",
+                "T2MatchBTS",
+                "T2LoadRedshift",
+                "T2PhaseLimit",
+                "T2XgbClassifier",
+            ]
+        ]
+    ]
 
     def post_init(self) -> None:
         """
         Retrieve models.
         """
 
         # Setup model. Currently only parsnip treated separatly
         # If possible, use T2RunParnsip as the parsnip
         # sncosmo model is very slow.
         if self.sncosmo_model_name == "parsnip_plasticc":
-            import parsnip # type: ignore[import]
-            source = parsnip.ParsnipSncosmoSource('plasticc')
-        else:
-            source = self.sncosmo_model_name   # Directly loaded
+            import parsnip  # type: ignore[import]
 
+            source = parsnip.ParsnipSncosmoSource("plasticc")
+        else:
+            source = self.sncosmo_model_name  # Directly loaded
 
         # Setup model, with or without MW correction
         if self.apply_mwcorrection:
             dust = sncosmo.models.CCM89Dust()
             self.sncosmo_model = sncosmo.Model(
-                source=source, effects=[dust], effect_names=["mw"], effect_frames=["obs"]
+                source=source,
+                effects=[dust],
+                effect_names=["mw"],
+                effect_frames=["obs"],
             )
             self.dustmap = SFDMap()
             self.fit_params = copy.deepcopy(self.sncosmo_model.param_names)
             self.fit_params.remove("mwebv")
             self.fit_params.remove("mwr_v")
         else:
             self.sncosmo_model = sncosmo.Model(source=source)
             self.fit_params = copy.deepcopy(self.sncosmo_model.param_names)
 
-
         # If redshift _should_ be provided we remove this from fit parameters
         if self.redshift_kind is not None or self.backup_z is not None:
             self.fit_params.remove("z")
 
         self.default_param_vals = self.sncosmo_model.parameters
 
         # retry on with exponential backoff on "too many open files"
-        self.process = backoff.on_exception( # type: ignore[assignment]
+        self.process = backoff.on_exception(  # type: ignore[assignment]
             backoff.expo,
             OSError,
-            giveup=lambda exc: not isinstance(exc, OSError) or exc.errno != errno.EMFILE,
-            logger=self.logger, # type: ignore[arg-type]
+            giveup=lambda exc: not isinstance(exc, OSError)
+            or exc.errno != errno.EMFILE,
+            logger=self.logger,  # type: ignore[arg-type]
             max_time=300,
         )(self.process)
 
-
+    # Should be rearranged to provide a list of redshifts a la T2RunParsnip with signature as this
+    #    def _get_redshift(self, t2_views) -> tuple[Optional[list[float]], Optional[str], Optional[list[float]]]:
     def _get_redshift(self, t2_views) -> tuple[None | float, None | str]:
         """
         Can potentially also be replaced with some sort of T2DigestRershift tabulator?
 
         Assuming that only one instance of redshift sources exist
         """
 
         # Examine T2s for eventual information
-        z: None | float = None
+        z: None | list[float] = None
         z_source: None | str = None
+        z_weights: None | list[float] = None
 
-
-        if self.redshift_kind in ['T2MatchBTS', 'T2DigestRedshifts']:
+        if self.redshift_kind in [
+            "T2MatchBTS",
+            "T2LoadRedshift",
+            "T2DigestRedshifts",
+            "T2ElasticcRedshiftSampler",
+        ]:
             for t2_view in t2_views:
-                if not t2_view.unit == self.redshift_kind:
+                if t2_view.unit != self.redshift_kind:
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
                 # Parse this
-                if self.redshift_kind == 'T2MatchBTS':
-                    if 'bts_redshift' in t2_res.keys() and not t2_res['bts_redshift'] == '-':
-                        z = float(t2_res['bts_redshift'])
+                if self.redshift_kind == "T2MatchBTS":
+                    if "bts_redshift" in t2_res and t2_res["bts_redshift"] != "-":
+                        z = [float(t2_res["bts_redshift"])]
                         z_source = "BTS"
-                elif self.redshift_kind == 'T2DigestRedshifts':
-                    if ('ampel_z' in t2_res.keys() and t2_res['ampel_z'] is not None
-                            and t2_res['group_z_nbr'] <= self.max_ampelz_group):
-                        z = float(t2_res['ampel_z'])
-                        z_source = "AMPELz_group" + str(t2_res['group_z_nbr'])
-        else:
-            # Check if there is a fixed z set for this run, otherwise keep as free parameter
-            if self.backup_z:
-                z = self.backup_z
-                z_source = "Fixed"
+                elif self.redshift_kind == "T2LoadRedshift":
+                    print(t2_res.keys)
+                    if "T2LoadRedshift_z" in t2_res:
+                        z = [float(t2_res["T2LoadRedshift_z"])]
+                        z_source = "T2LoadRedshift"
+                elif self.redshift_kind == "T2DigestRedshifts":
+                    if (
+                        "ampel_z" in t2_res
+                        and t2_res["ampel_z"] is not None
+                        and t2_res["group_z_nbr"] <= self.max_ampelz_group
+                    ):
+                        z = [float(t2_res["ampel_z"])]
+                        z_source = "AMPELz_group" + str(t2_res["group_z_nbr"])
+                elif self.redshift_kind == "T2ElasticcRedshiftSampler":
+                    z = t2_res["z_samples"]
+                    z_source = t2_res["z_source"]
+                    z_weights = t2_res["z_weights"]
+        # Check if there is a fixed z set for this run, otherwise keep as free parameter
+        elif self.fixed_z is not None:
+            if isinstance(self.fixed_z, float):
+                z = [self.fixed_z]
             else:
-                z = None
-                z_source = "Fitted"
+                z = list(self.fixed_z)
+            z_source = "Fixed"
+        else:
+            z = None
+            z_source = "Fitted"
 
         if (z is not None) and (z_source is not None) and self.scale_z:
-            z *= self.scale_z
-            z_source += " + scaled {}".format(self.scale_z)
+            z = [onez * self.scale_z for onez in z]
+            z_source += f" + scaled {self.scale_z}"
 
-        return z, z_source
+        # TODO: return the list instead of this
+        # return z, z_source, z_weights
+        # We now simply pick the middle number
+        if isinstance(z_weights, list):
+            z = z[z_weights.index(max(z_weights))]  # type: ignore
+            print("INPUT")
+            print(z, z_weights)
+            print("SNCOSMOS z", z)
+        elif isinstance(z, list):
+            if len(z) % 2 != 0:
+                z = z[int(len(z) / 2)]  # type: ignore
+            else:
+                z = ((z[int(len(z) / 2)]) + (z[int(len(z) / 2) - 1])) / 2  # type: ignore
 
+        return z, z_source  # type: ignore
 
-    def _get_phaselimit(self, t2_views) -> tuple[None | float,None | float]:
+    def _get_phaselimit(self, t2_views) -> tuple[None | float, None | float]:
         """
         Can potentially also be replaced with some sort of tabulator?
 
         """
 
         # Examine T2s for eventual information
         jdstart: None | float = None
         jdend: None | float = None
 
         if self.phaseselect_kind is None:
             jdstart = -np.inf
             jdend = np.inf
         else:
-
             for t2_view in t2_views:
                 # So far only knows how to parse phases from T2PhaseLimit
-                if not t2_view.unit == 'T2PhaseLimit':
+                if t2_view.unit != "T2PhaseLimit":
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
-                jdstart = t2_res['t_start']
-                jdend = t2_res['t_end']
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
+                jdstart = t2_res["t_start"]
+                jdend = t2_res["t_end"]
 
         return jdstart, jdend
 
     def _get_fit_metrics(self, sncosmo_result, sncosmo_table, sncosmo_model) -> dict:
         """
         Obtain metrics such as peak magnitude and lc residuals.
         Assumes that all models have at least z and t0 parameters.
         """
 
         # Fixing method parameters here, to avoid overloading unit params.
-        detection_sigma = 3    # Detection sigma threshold to look for phase of first detection
+        detection_sigma = (
+            3  # Detection sigma threshold to look for phase of first detection
+        )
         pull_range = [-10, 20]  # Phase range used when calculating uniform chi2/dof
 
-
-        z = sncosmo_model.get('z')
+        z = sncosmo_model.get("z")
 
         lc_metrics = {}
-        lc_metrics['restpeak_model_absmag_B'] = sncosmo_model.source_peakabsmag('bessellb', 'ab')
+        lc_metrics["restpeak_model_absmag_B"] = sncosmo_model.source_peakabsmag(
+            "bessellb", "ab"
+        )
         # Assuming all models have t0 as peak time parameter
         try:
-            lc_metrics['obspeak_model_B'] = sncosmo_model.bandmag(
-                'bessellb', 'ab', sncosmo_model.get('t0'))
+            lc_metrics["obspeak_model_B"] = sncosmo_model.bandmag(
+                "bessellb", "ab", sncosmo_model.get("t0")
+            )
         except ValueError:
             # Likely too high redshift for predicting mag
-            lc_metrics['obspeak_model_B'] = None
+            lc_metrics["obspeak_model_B"] = None
 
-
-        sncosmo_table['phase'] = (sncosmo_table["time"] - sncosmo_model.get('t0')) / (1 + z)
+        sncosmo_table["phase"] = (sncosmo_table["time"] - sncosmo_model.get("t0")) / (
+            1 + z
+        )
         # Determine the phase of the first 3 sigma detection
-        i_first = np.where((sncosmo_table["flux"] / sncosmo_table["fluxerr"]) > detection_sigma)[0]
+        i_first = np.where(
+            (sncosmo_table["flux"] / sncosmo_table["fluxerr"]) > detection_sigma
+        )[0]
         # table might not be ordered
-        lc_metrics['phase_{}sigma'.format(detection_sigma)] = np.min(sncosmo_table['phase'][i_first])
+        lc_metrics[f"phase_{detection_sigma}sigma"] = np.min(
+            sncosmo_table["phase"][i_first]
+        )
 
         # Determine the explosion time (JD) according to the model
         # i.e. first time when model was defined.
-        lc_metrics['jd_model_start'] = sncosmo_model.source.minphase() + sncosmo_model.get('t0')
-
+        lc_metrics["jd_model_start"] = (
+            sncosmo_model.source.minphase() + sncosmo_model.get("t0")
+        )
 
         # Determine the chi/dof and dof for observations around peak light
         pulls = []
-        for band in np.unique(sncosmo_table['band']):
+        for band in np.unique(sncosmo_table["band"]):
             band_tab = sncosmo_table[
-                (sncosmo_table['band'] == band) &
-                (sncosmo_table['phase'] >= pull_range[0]) &
-                (sncosmo_table['phase'] <= pull_range[1])
+                (sncosmo_table["band"] == band)
+                & (sncosmo_table["phase"] >= pull_range[0])
+                & (sncosmo_table["phase"] <= pull_range[1])
             ]
-            #band_pulls = (band_tab["flux"] - sncosmo_model.bandflux(
+            # band_pulls = (band_tab["flux"] - sncosmo_model.bandflux(
             #    band, band_tab["jd"], zp=25., zpsys='ab'))
             try:
                 # Using the same zeropoint / sys as when creating the table above
-                band_pulls = (band_tab["flux"] - sncosmo_model.bandflux(
-                    band, band_tab["time"], zp=25., zpsys='ab')) / band_tab["fluxerr"]
+                band_pulls = (
+                    band_tab["flux"]
+                    - sncosmo_model.bandflux(
+                        band, band_tab["time"], zp=25.0, zpsys="ab"
+                    )
+                ) / band_tab["fluxerr"]
                 pulls.extend(list(band_pulls))
-            except ValueError as e:
-                self.logger.info('Sncosmo get fit metric error')
-                lc_metrics['pull_retrieval_error'] = True
-
+            except ValueError:
+                self.logger.info("Sncosmo get fit metric error")
+                lc_metrics["pull_retrieval_error"] = True
 
-        lc_metrics['nbr_peak_pulls'] = len(pulls)
-        lc_metrics['absmean_peak_pull'] = np.mean(np.abs(pulls))
+        lc_metrics["nbr_peak_pulls"] = len(pulls)
+        lc_metrics["absmean_peak_pull"] = np.mean(np.abs(pulls))
 
         return lc_metrics
 
-
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self,
+    def process(
+        self,
         compound: T1Document,
         datapoints: Sequence[DataPoint],
-        t2_views: Sequence[T2DocView]
+        t2_views: Sequence[T2DocView],
     ) -> UBson | UnitResult:
         """
 
         Fit the parameters of the initiated snocmo_model to the light_curve
         provided. Depending on the configuration, the provided T2DovViews
         are used to look for redshift information and any phase (time)
         limits for the fit.
@@ -316,141 +385,167 @@
         -----------
         light_curve: "ampel.view.LightCurve" instance.
         See the LightCurve docstring for more info.
 
         t2_records: List of T2Records from the following units (if available)
         T2DigestRedshifts (redshift parsed from catalogs)
         T2MatchBTS (redshifts synced from BTS page)
+        T2LoadRedshift (redshift from .csv file)
         T2PhaseLimit (fit time-limits as determined from lightcurve)
 
         Returns
         -------
         dict
         """
 
         # Initialize output dict
         t2_output: dict[str, UBson] = {"model_name": self.sncosmo_model_name}
 
         # Obtain redshift
         z, z_source = self._get_redshift(t2_views)
-        t2_output['z'] = z
-        t2_output['z_source'] = z_source
+        t2_output["z"] = z
+        t2_output["z_source"] = z_source
         # A source class of None indicates that a redshift source was required, but not found.
-        if t2_output['z_source'] is None:
+        if t2_output["z_source"] is None:
             return t2_output
 
         # Check for phase limits
         (jdstart, jdend) = self._get_phaselimit(t2_views)
-        t2_output['jdstart'] = jdstart
-        t2_output['jdend'] = jdend
-        if t2_output['jdstart'] is None:
+        t2_output["jdstart"] = jdstart
+        t2_output["jdend"] = jdend
+        if t2_output["jdstart"] is None:
             return t2_output
 
         # Obtain photometric table
         sncosmo_table = self.get_flux_table(datapoints)
+        # print("T2RUNSNCOSMO:: ", sncosmo_table)
         sncosmo_table = sncosmo_table[
-                                    (sncosmo_table["time"]>=jdstart) &
-                                    (sncosmo_table["time"]<=jdend)
-                                    ]
-        print(sncosmo_table)
+            (sncosmo_table["time"] >= jdstart) & (sncosmo_table["time"] <= jdend)
+        ]
 
-        self.logger.debug('Sncosmo table {}'.format(sncosmo_table))
+        self.logger.debug(f"Sncosmo table {sncosmo_table}")
 
         # Fitting section
-        self.sncosmo_model.parameters = self.default_param_vals # Reset
+        # To handle multiple redshifts, fitting section below should be put into function.
+        # Do we keep the best fit, or all fits (as in t2parsnip)
+
+        self.sncosmo_model.parameters = self.default_param_vals  # Reset
 
         # Define fit parameter and ranges
         if self.apply_mwcorrection:
             transient_mwebv = self.dustmap.ebv(*self.get_pos(datapoints, which="mean"))
             self.sncosmo_model.set(mwebv=transient_mwebv)
 
         # Set redshift if provided
-        if isinstance(t2_output['z'], float):
-            self.sncosmo_model.set(z=t2_output['z'])
+        if isinstance(t2_output["z"], float):
+            self.sncosmo_model.set(z=t2_output["z"])
 
-        self.logger.debug('Starting fit with fit params {}, all parameters {} and start values {}'.format(
-            self.fit_params, self.sncosmo_model.param_names, self.sncosmo_model.parameters))
+        self.logger.debug(
+            "Starting fit with fit params {}, all parameters {} and start values {}".format(
+                self.fit_params,
+                self.sncosmo_model.param_names,
+                self.sncosmo_model.parameters,
+            )
+        )
 
         # Carry out fit. Bounds are directly carried from parameters
         # todo: gravefully check which observed bands cover redshifted model
         try:
             sncosmo_result, fitted_model = sncosmo.fit_lc(
-                sncosmo_table, self.sncosmo_model, self.fit_params, bounds=self.sncosmo_bounds)
+                sncosmo_table,
+                self.sncosmo_model,
+                self.fit_params,
+                bounds=self.sncosmo_bounds,
+            )
         except ValueError as e:
-            self.logger.info('Sncosmo fit error')
-            print('value error', e)
-            t2_output['run_error'] = True
+            self.logger.info("Sncosmo fit error")
+            print("value error", e)
+            t2_output["run_error"] = True
             return t2_output
         except RuntimeError as e:
             # Might have worked with different initial conditions?
-            print('value error', e)
-            self.logger.info('Sncosmo fit error')
-            t2_output['run_error'] = True
+            print("value error", e)
+            self.logger.info("Sncosmo fit error")
+            t2_output["run_error"] = True
             return t2_output
         except DataQualityError as e:
-            print('value error', e)
-            self.logger.info('Sncosmo fit error')
-            t2_output['run_error'] = True
+            print("value error", e)
+            self.logger.info("Sncosmo fit error")
+            t2_output["run_error"] = True
             return t2_output
 
-
-        self.logger.debug('Run results {}'.format(sncosmo_result))
+        self.logger.debug(f"Run results {sncosmo_result}")
 
         # Derive model metrics
-        t2_output['fit_metrics'] = self._get_fit_metrics(sncosmo_result,
-                                                         sncosmo_table, fitted_model)
+        t2_output["fit_metrics"] = self._get_fit_metrics(
+            sncosmo_result, sncosmo_table, fitted_model
+        )
 
         # How to best serialize these for mongo storage?
         sncosmo_result["parameters"] = sncosmo_result["parameters"].tolist()
         sncosmo_result["data_mask"] = sncosmo_result["data_mask"].tolist()
         try:
             sncosmo_result["covariance"] = sncosmo_result["covariance"].tolist()
-        except:
+        except KeyError:
             sncosmo_result["covariance"] = []
 
-
         # For filtering purposes we want a proper dict
         sncosmo_result["paramdict"] = {}
         for ix, pname in enumerate(sncosmo_result["param_names"]):
             sncosmo_result["paramdict"][pname] = sncosmo_result["parameters"][ix]
 
         # Finish up
         t2_output["sncosmo_result"] = sncosmo_result
 
         # Save plot
-        if self.plot_props:
-
-            # Construct name
-            stock_id = '-'.join([str(v) for v in self.get_stock_id(datapoints)])
-            tname = '-'.join([str(v) for v in self.get_stock_name(datapoints)])
+        if self.plot_props or self.plot_matplotlib_suffix:
+            # Construct name JN: What are the standards for noisified?
+            stock_id = "-".join([str(v) for v in self.get_stock_id(datapoints)])
+            tname = "-".join([str(v) for v in self.get_stock_name(datapoints)])
+
+            if self.noisified:
+                stock_id = "-".join([str(v) for v in self.get_stock_id(datapoints)])
+                tname = ZTFNoisifiedIdMapper().to_ext_id(stock_id)
 
             # Add some info
             plot_fig_text = "{} {} {} \nchisq {:.2f}\nndof {}".format(
-                tname, self.sncosmo_model_name, self.redshift_kind,
-                sncosmo_result["chisq"], sncosmo_result["ndof"]
-                )
+                tname,
+                self.sncosmo_model_name,
+                self.redshift_kind,
+                sncosmo_result["chisq"],
+                sncosmo_result["ndof"],
+            )
             plot_extra = {
-                'model': self.sncosmo_model_name,
-                'redshift_kind': self.redshift_kind,
-                'chisq': sncosmo_result["chisq"],
-                'ndof': sncosmo_result["ndof"],
-                'stock': stock_id
+                "model": self.sncosmo_model_name,
+                "redshift_kind": self.redshift_kind,
+                "chisq": sncosmo_result["chisq"],
+                "ndof": sncosmo_result["ndof"],
+                "stock": self.get_stock_id(datapoints)[
+                    0
+                ],  # Only using first name, assuming this is from ZTF
             }
 
             fig = sncosmo.plot_lc(
                 sncosmo_table,
                 model=fitted_model,
                 pulls=True,
                 figtext=plot_fig_text,
                 ncol=3,
                 # fill_data_marker = self.fit_mask, # Activate if add fit mask
             )
 
-            # Also store to DB if requested
-            plots = [
-                create_plot_record(fig,
-                                    self.plot_props, plot_extra, logger=self.logger)
-            ]
-            if self.plot_db:
-                t2_output['plots'] = plots
+            if self.plot_props:
+                plots = [
+                    create_plot_record(
+                        fig, self.plot_props, plot_extra, logger=self.logger
+                    )
+                ]
+                # Also store to DB if requested
+                if self.plot_db:
+                    t2_output["plots"] = plots
+            if self.plot_matplotlib_suffix:
+                fpath = os.path.join(
+                    self.plot_matplotlib_dir, tname + self.plot_matplotlib_suffix
+                )
+                fig.savefig(fpath)
 
         return t2_output
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunSnoopy.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSnoopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,29 @@
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                01.06.2022
 # Last Modified Date:  01.06.2021
 # Last Modified By:    jnordin@physik.hu-berlin.de
 
 
-from typing import Any, Optional, Union, Literal
-from collections.abc import Sequence
 import os
-
+from collections.abc import Sequence
+from typing import Literal
 
 import numpy as np
-import snpy # type: ignore[import]
-from astropy.table import Table
+import snpy  # type: ignore[import]
 from sfdmap import SFDMap  # type: ignore[import]
 
-from ampel.types import StockId, UBson
-from ampel.struct.UnitResult import UnitResult
 from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
-from ampel.view.T2DocView import T2DocView
+from ampel.model.StateT2Dependency import StateT2Dependency
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
+from ampel.view.T2DocView import T2DocView
 from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
-from ampel.model.StateT2Dependency import StateT2Dependency
-from ampel.model.PlotProperties import PlotProperties
 
 
 class T2RunSnoopy(AbsTiedLightCurveT2Unit):
     """
     Gathers information and runs snoopy. Steps include:
     - Parse previous (chained) T2results for redshift or phase limits.
     - Converts lightcurve content to Snoopy lc.
@@ -48,178 +45,175 @@
     # Default include EBV_model, EBV_model2, color_model, max_model
     snoopy_model_name: str
 
     # Redshift usage options. Current options
     # T2MatchBTS : Use the redshift published by BTS and  synced by that T2.
     # T2DigestRedshifts : Use the best redshift as parsed by DigestRedshift.
     # None : use backup_z as fixed redshift
-    redshift_kind: Optional[str]
+    redshift_kind: None | str
     # If loading redshifts from DigestRedshifts, provide the max ampel z group to make use of.
     # (note that filtering based on this can also be done for a potential t3)
     max_ampelz_group: int = 3
     # It is also possible to use fixed redshift whenever a dynamic redshift kind is not available
-    backup_z: Optional[float]
+    backup_z: None | float
     # Finally, the provided lens redshift might be multiplied with a scale
     # Useful for lensing studies, or when trying multiple values
-    scale_z: Optional[float]
-
+    scale_z: None | float
 
     # TODO: Additional snoopy parameters and Bounds
     # Snoopy can also be run in emcee fit mode, where priors can be included.
 
     # Remove MW dust absorption using SFD maps.
     # If set, needs to have access to local maps through SFDMap
     # If not, will be requested through URSA (slow, requires connection)
     # The default value of Rv will be used.
     apply_mwcorrection: bool = False
 
     # Phase range usage. Current option:
     # T2PhaseLimit : use the jdmin jdmax provided in this unit output
     # None : use full datapoint range
     # (T2BayesianBlocks should be added)
-    phaseselect_kind: Optional[str]
+    phaseselect_kind: None | str
 
     # Plot behaviour. Default is to not produce any plots.
     # If set, will store png to this directory.
-    plot_dir: Optional[str]
+    plot_dir: None | str
     # If true, will "draw" matplotlib figure to current env.
     plot_draw: bool = False
 
     # The snoopy filter naming scheme is not consistent with the observatories.
     # This is used to map from ampel fid to snoopy filter name
-    filter_name_map: dict = {1:'ztf_g', 2:'ztf_r', 3:'ztf_i'}
+    filter_name_map: dict = {1: "ztf_g", 2: "ztf_r", 3: "ztf_i"}
 
     # Which units should this be changed to
-    t2_dependency: Sequence[StateT2Dependency[Literal[
-                            "T2DigestRedshifts", "T2MatchBTS", "T2PhaseLimit"]]]
-
+    t2_dependency: Sequence[
+        StateT2Dependency[Literal["T2DigestRedshifts", "T2MatchBTS", "T2PhaseLimit"]]
+    ]
 
     def post_init(self) -> None:
         """
         Retrieve models.
         """
 
-
         # Setup model, with or without MW correction
         if self.apply_mwcorrection:
             self.dustmap = SFDMap()
 
-
-    def _get_redshift(self, t2_views) -> tuple[Optional[float],Optional[str]]:
+    def _get_redshift(self, t2_views) -> tuple[None | float, None | str]:
         """
         Can potentially also be replaced with some sort of T2DigestRershift tabulator?
 
         Assuming that only one instance of redshift sources exist
         """
 
         # Examine T2s for eventual information
-        z: Optional[float] = None
-        z_source: Optional[str] = None
-
+        z: None | float = None
+        z_source: None | str = None
 
-        if self.redshift_kind in ['T2MatchBTS', 'T2DigestRedshifts']:
+        if self.redshift_kind in ["T2MatchBTS", "T2DigestRedshifts"]:
             for t2_view in t2_views:
-                if not t2_view.unit == self.redshift_kind:
+                if t2_view.unit != self.redshift_kind:
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
                 # Parse this
-                if self.redshift_kind == 'T2MatchBTS':
-                    if 'bts_redshift' in t2_res.keys() and not t2_res['bts_redshift'] == '-':
-                        z = float(t2_res['bts_redshift'])
+                if self.redshift_kind == "T2MatchBTS":
+                    if "bts_redshift" in t2_res and t2_res["bts_redshift"] != "-":
+                        z = float(t2_res["bts_redshift"])
                         z_source = "BTS"
-                elif self.redshift_kind == 'T2DigestRedshifts':
-                    if ('ampel_z' in t2_res.keys() and t2_res['ampel_z'] is not None
-                            and t2_res['group_z_nbr'] <= self.max_ampelz_group):
-                        z = float(t2_res['ampel_z'])
-                        z_source = "AMPELz_group" + str(t2_res['group_z_nbr'])
+                elif self.redshift_kind == "T2DigestRedshifts" and (
+                    "ampel_z" in t2_res
+                    and t2_res["ampel_z"] is not None
+                    and t2_res["group_z_nbr"] <= self.max_ampelz_group
+                ):
+                    z = float(t2_res["ampel_z"])
+                    z_source = "AMPELz_group" + str(t2_res["group_z_nbr"])
+        # Check if there is a fixed z set for this run, otherwise keep as free parameter
+        elif self.backup_z:
+            z = self.backup_z
+            z_source = "Fixed"
         else:
-            # Check if there is a fixed z set for this run, otherwise keep as free parameter
-            if self.backup_z:
-                z = self.backup_z
-                z_source = "Fixed"
-            else:
-                z = None
-                z_source = "Fitted"
+            z = None
+            z_source = "Fitted"
 
         if (z is not None) and (z_source is not None) and self.scale_z:
             z *= self.scale_z
-            z_source += " + scaled {}".format(self.scale_z)
+            z_source += f" + scaled {self.scale_z}"
 
         return z, z_source
 
-
-    def _get_phaselimit(self, t2_views) -> tuple[Optional[float],Optional[float]]:
+    def _get_phaselimit(self, t2_views) -> tuple[None | float, None | float]:
         """
         Can potentially also be replaced with some sort of tabulator?
 
         """
 
         # Examine T2s for eventual information
-        jdstart: Optional[float] = None
-        jdend: Optional[float] = None
+        jdstart: None | float = None
+        jdend: None | float = None
 
         if self.phaseselect_kind is None:
             jdstart = -np.inf
             jdend = np.inf
         else:
-
             for t2_view in t2_views:
                 # So far only knows how to parse phases from T2PhaseLimit
-                if not t2_view.unit == 'T2PhaseLimit':
+                if t2_view.unit != "T2PhaseLimit":
                     continue
-                self.logger.debug('Parsing t2 results from {}'.format(t2_view.unit))
-                t2_res = res[-1] if isinstance(res := t2_view.get_payload(), list) else res
-                jdstart = t2_res['t_start']
-                jdend = t2_res['t_end']
+                self.logger.debug(f"Parsing t2 results from {t2_view.unit}")
+                t2_res = (
+                    res[-1] if isinstance(res := t2_view.get_payload(), list) else res
+                )
+                jdstart = t2_res["t_start"]
+                jdend = t2_res["t_end"]
 
         return jdstart, jdend
 
-
     def _get_snoopy_lcs(self, snpy_sn, light_curve, jdstart, jdend) -> dict:
         """
         Convert the light_curve instance to a dict with snoopy lc's:
         return {'filter_name': lc}
 
         The filter map defined above will be used to conver between
         ampel "fid" and snoopy filter name.
 
         This step is to be replaced by a tabulator.
         """
 
         # Limit phase range
         jd_filter = [
-            {'attribute': 'jd', 'operator': '>=', 'value': jdstart},
-            {'attribute': 'jd', 'operator': '<=', 'value': jdend}
+            {"attribute": "jd", "operator": ">=", "value": jdstart},
+            {"attribute": "jd", "operator": "<=", "value": jdend},
         ]
 
         # Check each filter for match
         lcs = {}
         for f_ampel, f_snoopy in self.filter_name_map.items():
-            dp_filter = [{'attribute': 'fid', 'operator':'==', 'value': f_ampel}]
+            dp_filter = [{"attribute": "fid", "operator": "==", "value": f_ampel}]
             dp_filter.extend(jd_filter)
-            dps = light_curve.get_ntuples(('jd', 'magpsf', 'sigmapsf'),
-                        filters=dp_filter)
+            dps = light_curve.get_ntuples(
+                ("jd", "magpsf", "sigmapsf"), filters=dp_filter
+            )
             # Sort tuples based on jd
             dps = sorted(dps)
             df = np.asarray(dps)
-            jd, mag, sigmamag = df[:,0], df[:,1], df[:,2]
-            if len(jd)>0:
+            jd, mag, sigmamag = df[:, 0], df[:, 1], df[:, 2]
+            if len(jd) > 0:
                 lcs[f_snoopy] = snpy.lc(snpy_sn, f_snoopy, jd, mag, sigmamag)
 
         return lcs
 
-
-
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self,
-                light_curve: LightCurve, t2_views: Sequence[T2DocView]
-                ) -> Union[UBson, UnitResult]:
+    def process(
+        self, light_curve: LightCurve, t2_views: Sequence[T2DocView]
+    ) -> UBson | UnitResult:
         """
 
         Fit the parameters of the specified snoopy model to the light_curve
         provided. Depending on the configuration, the provided T2DovViews
         are used to look for redshift information and any phase (time)
         limits for the fit.
 
@@ -240,62 +234,68 @@
         """
 
         # Initialize output dict
         t2_output: dict[str, UBson] = {"model_name": self.snoopy_model_name}
 
         # Obtain redshift
         z, z_source = self._get_redshift(t2_views)
-        t2_output['z'] = z
-        t2_output['z_source'] = z_source
+        t2_output["z"] = z
+        t2_output["z_source"] = z_source
         # A source class of None indicates that a redshift source was required, but not found.
         if z is None or z_source is None:
             return t2_output
 
         # Check for phase limits
         (jdstart, jdend) = self._get_phaselimit(t2_views)
-        t2_output['jdstart'] = jdstart
-        t2_output['jdend'] = jdend
-        if t2_output['jdstart'] is None:
+        t2_output["jdstart"] = jdstart
+        t2_output["jdend"] = jdend
+        if t2_output["jdstart"] is None:
             return t2_output
 
         # Initialize SN
         assert isinstance(pos := light_curve.get_pos(), tuple)
         (ra, dec) = pos
         assert isinstance(light_curve.stock_id, int)
         if self.apply_mwcorrection:
             transient_mwebv = self.dustmap.ebv(ra, dec)
-            snoopy_sn = snpy.sn(name=ZTFIdMapper.to_ext_id(light_curve.stock_id),
-                        z=z, ra=ra, dec=dec, EBVgal=transient_mwebv)
+            snoopy_sn = snpy.sn(
+                name=ZTFIdMapper.to_ext_id(light_curve.stock_id),
+                z=z,
+                ra=ra,
+                dec=dec,
+                EBVgal=transient_mwebv,
+            )
         else:
-            snoopy_sn = snpy.sn(name=ZTFIdMapper.to_ext_id(light_curve.stock_id),
-                        z=z, ra=ra, dec=dec)
+            snoopy_sn = snpy.sn(
+                name=ZTFIdMapper.to_ext_id(light_curve.stock_id), z=z, ra=ra, dec=dec
+            )
 
         snoopy_sn.choose_model(self.snoopy_model_name)
-        snoopy_sn.replot = 0 # default plot is off
+        snoopy_sn.replot = 0  # default plot is off
 
         # Obtain and add photometric table
         lc_dict = self._get_snoopy_lcs(snoopy_sn, light_curve, jdstart, jdend)
         for fname, lc in lc_dict.items():
             snoopy_sn.data[fname] = lc
         snoopy_sn.get_restbands()
 
         # Do the fit
         snoopy_sn.fit()
 
         # Collect output
-        t2_output['parameters'] = snoopy_sn.parameters
-        t2_output['errors'] = snoopy_sn.errors
-
-
+        t2_output["parameters"] = snoopy_sn.parameters
+        t2_output["errors"] = snoopy_sn.errors
 
         # Save plot
         if self.plot_dir:
             # Construct name
-            fname = os.path.join(self.plot_dir,'{}_snoopy_{}.png'.format(
-                    ZTFIdMapper.to_ext_id(light_curve.stock_id), self.snoopy_model_name))
-            p = snoopy_sn.plot(outfile=fname)
+            fname = os.path.join(
+                self.plot_dir,
+                "{}_snoopy_{}.png".format(
+                    ZTFIdMapper.to_ext_id(light_curve.stock_id), self.snoopy_model_name
+                ),
+            )
+            snoopy_sn.plot(outfile=fname)
         if self.plot_draw:
-            p = snoopy_sn.plot()
-
-
+            snoopy_sn.plot()
 
         return t2_output
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2RunTDE.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunTDE.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,143 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                ampel/contrib/hu/t2/T2RunTDE.py
 # License:             BSD-3-Clause
 # Author:              simeon.reusch@desy.de
 # Date:                17.05.2022
-# Last Modified Date:  18.05.2022
+# Last Modified Date:  19.04.2023
 # Last Modified By:    simeon.reusch@desy.de
 
 
+import copy
+import errno
+
+# from astropy.time import Time
+import backoff
 import numpy as np
 import sncosmo  # type: ignore[import]
+from astropy import constants as c
+from astropy import units as u
+from astropy.units import Quantity
 from sfdmap import SFDMap  # type: ignore[import]
-from typing import Union
-import errno, os, backoff, copy
-
-# from astropy.time import Time
-import astropy.cosmology as cospy
-from typing import Literal, Sequence
 
-# from urllib.request import urlopen
-# from urllib.parse import urljoin
-
-from ampel.types import UBson
-from ampel.struct.UnitResult import UnitResult
 from ampel.contrib.hu.t2.T2RunSncosmo import T2RunSncosmo
 
+# from ampel.enum.DocumentCode import DocumentCode
+
 # from ampel.model.StateT2Dependency import StateT2Dependency
-from ampel.view.T2DocView import T2DocView
 
-# from ampel.enum.DocumentCode import DocumentCode
-from ampel.view.LightCurve import LightCurve
+# from urllib.request import urlopen
+# from urllib.parse import urljoin
 
 
 class TDESource(sncosmo.Source):
-
     _param_names: list = ["risetime", "decaytime", "temperature", "amplitude"]
     param_names_latex: list = [
-        "Rise Time",
-        "Decay Time",
+        "Rise Time~[log10 day]",
+        "Decay Time~[log10 day]",
         "Temperature~[log10~K]",
         "Amplitude",
     ]
 
     def __init__(
         self,
         phase: np.ndarray,
         wave: np.ndarray,
         name: str = "TDE",
         version: str = "1.0",
     ) -> None:
-
         self.name: str = name  # mandatory for SNCosmo
         self.version: str = version  # mandatory for
         self._phase: np.ndarray = phase
         self._wave: np.ndarray = wave
 
-        self.nu_kc: float = 3e8 / 4770e-10  # Reference wavelength used for K-correction
-        self.z: float = 0.1
-
-        # Some constants
-        self.sigma_SB: float = 5.6704e-5  # Stefan-Boltzmann constant (erg/s/cm^2/K^4)
-        self.c: float = 2.9979e10  # Speed of light (cm/s)
-        self.h: float = 6.6261e-27  # Planck's constant (erg s)
-        self.k: float = 1.3806e-16  # Boltzman's constant (erg/K)
-        self.h_over_k: float = self.h / self.k
-        self.lumdis: float = float(
-            cospy.FlatLambdaCDM(H0=70, Om0=0.3).luminosity_distance(self.z).value
-            * 1e6
-            * 3.08568e18
-        )
-
         # Fit parameters
-        # defaults - peaktime = 0, rise=0.85 / decay=1.5 / T=4.5 / peakflux = 32
-        self._parameters: np.ndarray = np.array([0.85, 1.5, 4.5, 32])
+        # defaults: peaktime = 0, rise=1.584 / decay=2.278 / T=4.0 / peakflux = 1e-25
+        self._parameters: np.ndarray = np.array([1.584, 2.278, 4.0, 1e-25])
 
     @staticmethod
-    def _wl_to_nu(self, wl: np.ndarray) -> np.ndarray:
+    def _planck_lam(self, wave: np.ndarray, T: np.ndarray) -> np.float64 | np.ndarray:
         """
-        Convert wavelength in Angstrom to frequency in Hz
-
+        Calculate the spectral radiance of a blackbody
+        :wave: np.ndarray, array containing wavelength in AA
+        :T: np.ndarray, array containing temperatures in K
         """
-        nu = 2.9979e18 / wl
+        wave_aa: Quantity = wave * u.AA
+        wave_m: Quantity = wave_aa.to(u.m)
 
-        return nu
+        prefactor = 2 * c.h * c.c**2 / wave_m**5
 
-    @staticmethod
-    def _Planck(self, nu: np.ndarray, T: float) -> Union[np.float64, np.ndarray]:
-        """
-        Calculate the spectral radiance of a blackbody
-        :nu: np.ndarray, Array containing frequencies in Hz
-        :T: np.float, temperature in K
-        """
-        bb = (
-            2
-            * self.h
-            / self.c**2
-            * nu**3
-            / (np.exp(self.h * nu / (self.k * T)) - 1)
+        prefactor = np.tile(prefactor, (len(T), 1)).transpose()
+
+        exponential_term = (
+            c.h.value * c.c.value * 1 / np.outer(wave_m.value, T) / c.k_B.value
         )
-        return bb
 
-    @staticmethod
-    def _cc_bol(self, nu: Union[float, np.ndarray], T: float):
-        return self._Planck(self, nu, T) * nu / (self.sigma_SB * T**4 / np.pi)
+        # returns spectral radiance: J s-1 sr-1 m-3
+        return prefactor * 1 / (np.exp(exponential_term) - 1) / u.sr
 
     @staticmethod
-    def _get_cc(self, nu: np.ndarray, T: Union[float, np.float64] = None) -> np.ndarray:
-        """
-        Calculate a k-correction for each wavelength
-        """
-        if T is None:
-            T = self._parameters[2]
-        T = 10**T
-        kc = (
-            (np.exp(self.h_over_k * self.nu_kc / T) - 1)
-            / (np.exp(self.h_over_k * nu / T) - 1)
-            * (nu / self.nu_kc) ** 4
-        )
-        return kc
+    def _cc_bol_lam(self, wave: float | np.ndarray, T: np.ndarray):
+        return self._planck_lam(self, wave, T) * u.sr
 
     @staticmethod
-    def _gauss(x: int, sigma: Union[float, np.float64]) -> Union[float, np.float64]:
+    def _gauss(x: float, sigma: float | np.float64) -> float | np.float64:
         """
         Calculate a Gaussian
         """
-        gauss = np.exp(-0.5 * x**2 / (sigma**2))
-        return gauss
+        return np.exp(-0.5 * x**2 / (sigma**2))
 
     @staticmethod
-    def _gauss_exp(self, phase: np.float64, nu: np.ndarray) -> np.ndarray:
-        """
-        Calculate a gaussian rise and decay for the lightcurve
-        """
+    def _gauss_exp(self, phases: np.ndarray) -> np.ndarray:
         risetime = self._parameters[0]
         decaytime = self._parameters[1]
-        temp = self._parameters[2]
         peakflux = self._parameters[3]
 
-        a1 = (
-            10**peakflux
-        )  # luminosity/flux at peak (this can be bolometric or L(nu_kc) depending on the setting)
-        b1 = 10**risetime  # rise rate
-        b2 = 10**decaytime  # decay rate
+        # Gaussian rise
+        a1 = peakflux
+        b1 = 10**risetime
+        b2 = 10**decaytime
         a2 = a1 * self._gauss(0, b1)
 
-        # are we in the rise or decay phase?
-        # risephase
-        if phase <= 0:
-            val = a1 * self._gauss(phase, b1)
+        phases_rise = phases[(phases <= 0)]
+        phases_decay = phases[(phases > 0)]
 
-        # decayphase
-        else:
-            val = a2 * np.exp(-(phase) / b2)
+        vals_rise = a1 * self._gauss(phases_rise, b1)
 
-        cc = self._get_cc(self, nu)  # conversion from model curve to nuLnu of the data
+        phases_decay = phases[(phases > 0)]
 
-        return val * cc
+        # exponential decay
+        vals_decay = a2 * np.exp(-(phases_decay) / b2)
 
-    @staticmethod
-    def _lum2flux(
-        L: np.ndarray,
-        cm: float,
-        nu: np.ndarray,
-    ):
-        """
-        erg/s to Jansky
-        >> flux = lum2flux(L, z, nu=1.4e9) # in Jy
-        input:
-         - L: luminosity in erg/s
-         - cm: luminosity distance in cm
+        return np.concatenate((vals_rise, vals_decay))
 
-        note, no K-correction
+    def _temp_evolution(self, phase: np.ndarray) -> np.ndarray:
         """
-        return L / (nu * 4 * np.pi * cm**2) * 1e23
+        Create an array with a linear temperature evolution
+        """
+        temp = self._parameters[2]
+
+        return (10**temp) + phase * 0
 
     def _flux(self, phase: np.ndarray, wave: np.ndarray) -> np.ndarray:
         """
         Calculate the model flux for given wavelengths and phases
         """
-        temp = self._parameters[2]
-
-        if np.ndim(phase) == 0:
-            # phase_iter = [phase]
-            phase_iter = np.asarray(phase)
-        else:
-            phase_iter = phase
-
-        model_flux = np.empty((len(phase_iter), len(wave)))
+        t_evo = self._temp_evolution(phase=phase)
 
-        for i, ph in enumerate(phase_iter):
+        phase_iter = np.asarray(phase) if np.ndim(phase) == 0 else phase
 
-            nu = self._wl_to_nu(self, wave)
-            model = self._gauss_exp(self, phase=ph, nu=nu)
-            model_bol = model / self._cc_bol(self, T=10**temp, nu=self.nu_kc)
-            cc = self._cc_bol(self, T=10**temp, nu=nu * (1 + self.z))
+        bb_lam = self._cc_bol_lam(self, T=t_evo, wave=wave)
 
-            model_flux_at_phase = self._lum2flux(
-                L=(model_bol * cc), cm=self.lumdis, nu=nu * (1 + self.z)
-            ) * (1 + self.z)
+        rise_decay = self._gauss_exp(self, phases=phase_iter)
 
-            model_flux[i] = model_flux_at_phase
+        model_flux = (rise_decay * bb_lam).transpose()
 
-        return model_flux
+        return model_flux.to(u.erg / u.s / u.cm**2 / u.AA)
 
 
 class T2RunTDE(T2RunSncosmo):
     """
     Create a TDE model and fit to a LightCurve object as process is called.
 
     Create a TDE sncosmo_model for fit by T2RunSncosmo.
@@ -246,11 +178,12 @@
 
         self.default_param_vals = self.sncosmo_model.parameters
 
         # retry on with exponential backoff on "too many open files"
         self.process = backoff.on_exception(  # type: ignore[assignment]
             backoff.expo,
             OSError,
-            giveup=lambda exc: not isinstance(exc, OSError) or exc.errno != errno.EMFILE,
-            logger=self.logger, # type: ignore[arg-type]
+            giveup=lambda exc: not isinstance(exc, OSError)
+            or exc.errno != errno.EMFILE,
+            logger=self.logger,  # type: ignore[arg-type]
             max_time=300,
         )(self.process)
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2TNSEval.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TNSEval.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,29 @@
 # File:                ampel/contrib/hu/t2/T2TNSEval.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                27.01.2021
 # Last Modified Date:  27.01.2021
 # Last Modified By:    jnordin@physik.hu-berlin.de
 
+from collections.abc import Sequence
+from typing import Any
+
 import numpy as np
 from astropy.coordinates import SkyCoord
-from typing import Any
-from collections.abc import Sequence
-from ampel.types import UBson
+
+# T2 importing info from T3. Restructure?
+from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
+from ampel.contrib.hu.t3.ampel_tns import (
+    TNSFILTERID,
+)
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 from ampel.view.T2DocView import T2DocView
-from ampel.contrib.hu.t3.ampel_tns import TNSFILTERID   # T2 importing info from T3. Restructure?
-from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
 
 
 class T2TNSEval(AbsTiedLightCurveT2Unit):
     """
     Evalute whether a transient fulfills criteria for submission to TNS.
     This is done partially based on the lightcurve content and partially on the results of catalog maches.
     The T2 result will be a dictionary with the information used for TNS submission (e.g. recent upper limit).
@@ -64,15 +69,15 @@
     # reject alert if ssdistnr smaller than this value for any pp
     ssdistnr_max: float = 1
     # reject alert if PS1 star for any pp
     ps1_sgveto_rad: float = 1
     ps1_sgveto_sgth: float = 0.8
     # Minimal median RB.
     rb_minmed: float = 0.3
-    drb_minmed: float = 0.95   # if drb found!
+    drb_minmed: float = 0.95  # if drb found!
     # Try to reject likely CV through rejecting objects that quickly get very bright
     cut_fastrise: bool = True
     # Require each PP to have a magpsf lower than the diffmaglim
     require_lowerthanlim: bool = True
 
     # Cut to apply to all the photopoints in the light curve.
     # This will affect most operations, i.e. evaluating the position,
@@ -95,27 +100,25 @@
     ztf_tns_at: dict = {  # Default values to tag ZTF detections / ulims
         "flux_units": "1",
         "instrument_value": "196",
         "exptime": "30",
         "Observer": "Robot",
     }
 
-
     def inspect_catalog(self, cat_res: dict[str, Any]) -> bool:
         """
         Verify whether any catalog matching criteria prevents submission.
 
         """
 
         # Check that we got any catalogmatching results (that it was run)
         if self.require_catalogmatch and len(cat_res) == 0:
             self.logger.debug("no T2CATALOGMATCH results")
             return False
 
-
         # check that you have positive match in all of the necessary cataslogs:
         for needed_cat in self.needed_catalogs:
             if not cat_res.get(needed_cat, False):
                 self.logger.debug(
                     "no T2CATALOGMATCH results for %s" % needed_cat,
                     extra={"catalog_matches": cat_res},
                 )
@@ -170,15 +173,14 @@
             return False
 
         # TODO: Check for fast moving stars
 
         # congratulation catalog, you made it!
         return True
 
-
     def inspect_lc(self, lc: LightCurve) -> bool:
         """
         Verify whether the transient lightcurve fulfill criteria for submission.
 
         """
 
         # apply cut on history: consider photophoints which are sharp enough
@@ -229,21 +231,21 @@
                 "operator": ">=",
                 "value": self.max_maglim,
             }
         ):
             last_ulim = sorted(ulims, key=lambda x: x["body"]["jd"])[-1]
             pps_after_ndet = (
                 lc.get_photopoints(
-                    filters=self.lc_filters
-                    + [
+                    filters=[
+                        *self.lc_filters,
                         {
                             "attribute": "jd",
                             "operator": ">=",
                             "value": last_ulim["body"]["jd"],
-                        }
+                        },
                     ]
                 )
                 or []
             )
             # Can this work? - It does not seem like it
             # filters = self.lc_filters + [{'attribute': 'jd', 'operator': '>=', 'value': last_ulim["body"]['jd']}, {'attribute': 'magpsf', 'operator': '<', 'attribute': 'diffmaglim'}]
             # Current filters cannot sort two attributes
@@ -271,31 +273,33 @@
                     self.logger.info(
                         "Likely CV", extra={"deltaT": delta_t, "deltaM": delta_m}
                     )
                     return False
 
         # cut on distance to closest solar system object
         # TODO: how to make this check: ('0.0' in list(phot["ssdistnr"])
-        ssdist = np.array([pp["body"]["ssdistnr"] for pp in pps if "ssdistnr" in pp['body']])
-        ssdist[ssdist == None] = -999
+        ssdist = np.array(
+            [pp["body"]["ssdistnr"] for pp in pps if "ssdistnr" in pp["body"]]
+        )
+        ssdist[ssdist == None] = -999  # noqa: E711
 
         close_to_sso = np.logical_and(ssdist < self.ssdistnr_max, ssdist > 0)
         if np.any(close_to_sso):
             self.logger.info(
                 "transient too close to solar system object",
                 extra={"ssdistnr": ssdist.tolist()},
             )
             return False
 
         # check PS1 sg for the full alert history
         # Note that we for this check do *not* use the lightcurve filter criteria
         # TODO: Evaluate whether we should use the filters, and do a check for sufficient number of datapoints remaining
         # distpsnr1, sgscore1 = zip(*lc.get_tuples('distpsnr1', 'sgscore1', filters=self.lc_filters))
         if tups := lc.get_tuples("distpsnr1", "sgscore1"):
-            distpsnr1, sgscore1 = zip(*tups)
+            distpsnr1, sgscore1 = zip(*tups, strict=False)
         else:
             return False
         is_ps1_star = np.logical_and(
             np.array(distpsnr1) < self.ps1_sgveto_rad,
             np.array(sgscore1) > self.ps1_sgveto_sgth,
         )
         if np.any(is_ps1_star):
@@ -307,63 +311,69 @@
 
         # cut on median RB score
         rbs = [pp["body"]["rb"] for pp in pps]
         if np.median(rbs) < self.rb_minmed:
             return False
 
         # cut on median dRB score
-        drbs = [pp["body"]["drb"] for pp in pps if "drb" in pp["body"].keys()]
+        drbs = [pp["body"]["drb"] for pp in pps if "drb" in pp["body"]]
         if len(drbs) > 0 and np.median(drbs) < self.drb_minmed:
             return False
 
         # congratulation Lightcurve, you made it!
         return True
 
-    def get_catalog_remarks(self, lc: LightCurve, cat_res: dict[str, Any]) -> None | dict[str, Any]:
+    def get_catalog_remarks(
+        self, lc: LightCurve, cat_res: dict[str, Any]
+    ) -> None | dict[str, Any]:
         """
         Look through catalogs for remarks to be added to report.
         """
 
         # Start building dict with remarks
-        remarks : dict[str, Any] = {"remarks":""}
+        remarks: dict[str, Any] = {"remarks": ""}
 
         # Check redshift
         nedz = cat_res.get("NEDz", False)
         sdss_spec = cat_res.get("SDSS_spec", False)
         if sdss_spec:
-            remarks["remarks"] = remarks["remarks"] + "SDSS spec-z %.3f. "%(sdss_spec["z"])
+            remarks["remarks"] = (
+                remarks["remarks"] + "SDSS spec-z %.3f. " % (sdss_spec["z"])
+            )
         elif nedz:
-            remarks["remarks"] = remarks["remarks"] + "NED z %.3f. "%(nedz["z"])
+            remarks["remarks"] = remarks["remarks"] + "NED z %.3f. " % (nedz["z"])
 
         # tag AGNs
         milliquas = cat_res.get("milliquas", False)
         sdss_spec = cat_res.get("SDSS_spec", False)
-        if (milliquas and milliquas["redshift"] is not None and milliquas["redshift"] > 0) or (
-            sdss_spec and sdss_spec["bptclass"] in [4, 5]
-        ):
-            remarks["remarks"] = remarks["remarks"] + "Known SDSS and/or MILLIQUAS QSO/AGN. "
+        if (
+            milliquas
+            and milliquas["redshift"] is not None
+            and milliquas["redshift"] > 0
+        ) or (sdss_spec and sdss_spec["bptclass"] in [4, 5]):
+            remarks["remarks"] = (
+                remarks["remarks"] + "Known SDSS and/or MILLIQUAS QSO/AGN. "
+            )
             remarks["at_type"] = 3
 
         # tag nuclear
         sdss_dr10 = cat_res.get("SDSSDR10", False)
         if (
             sdss_dr10
             and sdss_dr10["type"] == 3
             and sdss_dr10["dist2transient"] < self.nuclear_dist
         ):
-            remarks["remarks"] = remarks["remarks"] + "Close to core of SDSS DR10 galaxy. "
+            remarks["remarks"] = (
+                remarks["remarks"] + "Close to core of SDSS DR10 galaxy. "
+            )
             remarks["at_type"] = 4
 
         # tag noisy gaia
-        if (
-            tups := lc.get_tuples(
-                "distpsnr1", "sgscore1", filters=self.lc_filters
-            )
-        ):
-            distpsnr1, sgscore1 = zip(*tups)
+        if tups := lc.get_tuples("distpsnr1", "sgscore1", filters=self.lc_filters):
+            distpsnr1, sgscore1 = zip(*tups, strict=False)
             galaxylike_ps1 = np.logical_and(
                 np.array(distpsnr1) < 1.5, np.array(sgscore1) < 0.5
             )
             gaia_dr2 = cat_res.get("GAIADR2", False)
             nedz = cat_res.get("NEDz", False)
             if (
                 (
@@ -376,29 +386,30 @@
                     sdss_dr10
                     and not (sdss_dr10["type"] == 3 and sdss_dr10["dist2transient"] < 3)
                 )
                 and (  # and if it's not a galaxy
                     not np.any(galaxylike_ps1)
                 )  # TODO: check the logic
             ):
-                remarks["remarks"] = remarks["remarks"] + "Significant noise in Gaia DR2 - variable star cannot be excluded. "
+                remarks["remarks"] = (
+                    remarks["remarks"]
+                    + "Significant noise in Gaia DR2 - variable star cannot be excluded. "
+                )
 
-        if len(remarks["remarks"])==0:
+        if len(remarks["remarks"]) == 0:
             return None
-        else:
-            return remarks
+        return remarks
 
-
-    def get_lightcurve_info(self,  lc: LightCurve) -> None | dict[str, Any]:
+    def get_lightcurve_info(self, lc: LightCurve) -> None | dict[str, Any]:
         """
         Collect the data needed for the atreport. Return None in case
         you have to skip this transient for some reason.
         """
 
-        if (pos := lc.get_pos(ret="mean", filters=self.lc_filters)):
+        if pos := lc.get_pos(ret="mean", filters=self.lc_filters):
             ra, dec = pos
         else:
             return None
 
         # Start defining AT dict: name and position
         atdict: dict[str, Any] = {}
         # atdict.update(self.base_at_dict)
@@ -429,40 +440,43 @@
             }
 
         atdict["non_detection"].update(self.ztf_tns_at)  # Add the default ZTF values
 
         # now add info on photometric detections: consider only candidates which
         # have some consecutive detection after the last ulim
         if pps := lc.get_photopoints(
-            filters=self.lc_filters
-            + [{"attribute": "jd", "operator": ">=", "value": last_non_obs}]
+            filters=[
+                *self.lc_filters,
+                {"attribute": "jd", "operator": ">=", "value": last_non_obs},
+            ]
         ):
             # Lets create a few photometry points: TODO: should they be the latest or the first?
             atdict["photometry"] = {"photometry_group": {}}
-            atdict["discovery_datetime"] = 10 ** 30
+            atdict["discovery_datetime"] = 10**30
             for ipp, pp in enumerate(pps[: self.nphot_submit]):
                 photdict = {  # TODO: do we need to round the numerical values?
                     "obsdate": pp["body"]["jd"],
-                    "flux": float("{0:.2f}".format(pp["body"]["magpsf"])),
-                    "flux_error": float("{0:.2f}".format(pp["body"]["sigmapsf"])),
-                    "limiting_flux": float("{0:.2f}".format(pp["body"]["diffmaglim"])),
+                    "flux": float("{:.2f}".format(pp["body"]["magpsf"])),
+                    "flux_error": float("{:.2f}".format(pp["body"]["sigmapsf"])),
+                    "limiting_flux": float("{:.2f}".format(pp["body"]["diffmaglim"])),
                     "filter_value": TNSFILTERID.get(pp["body"]["fid"]),
                 }
                 if pp["body"]["jd"] < atdict["discovery_datetime"]:
                     atdict["discovery_datetime"] = pp["body"]["jd"]
                 photdict.update(self.ztf_tns_at)
                 atdict["photometry"]["photometry_group"][str(ipp)] = photdict
 
         return atdict
 
-
     # ==================== #
     # AMPEL T2 MANDATORY   #
     # ==================== #
-    def process(self, light_curve: LightCurve, t2_views: Sequence[T2DocView]) -> UBson | UnitResult:
+    def process(
+        self, light_curve: LightCurve, t2_views: Sequence[T2DocView]
+    ) -> UBson | UnitResult:
         """
 
         Evaluate whether a transient passes thresholds for submission to TNS.
         If so, collects the required submission info.
         This unit does *not* verify whether a transient already exists in TNS.
 
         Parameters
@@ -479,41 +493,37 @@
         Warning: this dict does *not* contain the internal name (atdict['internal_name']) required.
         This will have to be added by the T3. Similarly, the base atdict entries are not included.
 
         In further changes, the photometry_group keys are now str instead of int (to be able to store)
         If needed by TNS, they need to be converted back at T3
         """
 
-        self.logger.debug('starting eval from %s'%(t2_views) )
-
-
+        self.logger.debug("starting eval from %s" % (t2_views))
 
         # i. Check whether the lightcurve passes selection criteria
         if not self.inspect_lc(light_curve):
-            return { 'tns_candidate' : False, 'tns_eval' : 'Poor lightcurve.' }
-
+            return {"tns_candidate": False, "tns_eval": "Poor lightcurve."}
 
         # ii. Check the catalog matching criteria
         t2_cat_match = t2_views[0]
         assert t2_cat_match.unit in (dep.unit for dep in self.t2_dependency)
         catalog_result = t2_cat_match.get_payload()
         assert isinstance(catalog_result, dict)
         if not self.inspect_catalog(catalog_result):
-            return { 'tns_candidate' : False, 'tns_eval' : 'Catalog match rejection.' }
-
-
+            return {"tns_candidate": False, "tns_eval": "Catalog match rejection."}
 
         # iii. Collect information for submission
 
         # These methods repeat a lot of calculations from above, but are kept separate
         # to easier override selection method
         atdict = self.get_lightcurve_info(light_curve)
         if atdict is None:
-            return { 'tns_candidate' : False, 'tns_eval' : 'Passes criteria, fails in info collection.' }
+            return {
+                "tns_candidate": False,
+                "tns_eval": "Passes criteria, fails in info collection.",
+            }
 
         catremarks = self.get_catalog_remarks(light_curve, catalog_result)
         if catremarks is not None:
             atdict.update(catremarks)
 
-        t2result = { 'tns_candidate' : True, 'tns_eval' : 'Good', 'atdict':atdict }
-
-        return t2result
+        return {"tns_candidate": True, "tns_eval": "Good", "atdict": atdict}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,301 +3,417 @@
 # File:                ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                28.12.2018
 # Last Modified Date:  03.08.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
-from typing import Any, Union, TYPE_CHECKING, Sequence, Iterable
 import os
+import re
+from collections.abc import Iterable, Sequence
+from typing import TYPE_CHECKING, Any
+
+import light_curve
 import numpy as np
 from astropy.table import Table
 from scipy.optimize import curve_fit
 
-from ampel.types import UBson
 from ampel.abstract.AbsStateT2Unit import AbsStateT2Unit
 from ampel.abstract.AbsTabulatedT2Unit import AbsTabulatedT2Unit
 from ampel.base.AmpelBaseModel import AmpelBaseModel
-from ampel.protocol.LoggerProtocol import LoggerProtocol
-from ampel.struct.UnitResult import UnitResult
-
+from ampel.base.LogicalUnit import LogicalUnit
 from ampel.content.DataPoint import DataPoint
 from ampel.content.T1Document import T1Document
+from ampel.protocol.LoggerProtocol import LoggerProtocol
 
 
-
-def getMag(tab: Table, err=False):
+def getMag(tab: Table, err=False, time=False):
     """
     Shorthand to getting the magnitude from flux.
     """
 
-    m = -2.5* np.log10(tab['flux']) + tab['zp']
+    iPos = tab["flux"] > 0
+    m = -2.5 * np.log10(tab["flux"][iPos]) + tab["zp"][iPos]
     if err:
         # Simple symmetric method
-        merr = 2.5 / np.log(10) * (tab['fluxerr']/tab['flux'])
+        merr = 2.5 / np.log(10) * (tab["fluxerr"][iPos] / tab["flux"][iPos])
+        if time:
+            return m, merr, tab["time"][iPos]
         return m, merr
-    else:
-        return m
+    if time:
+        return m, tab["time"][iPos]
+    return m
+
 
 def getMeanflux(tab: Table, jdstart, jdend):
     """
     Return dict with the mean flux for all bands
     with data in the selected range.
     """
 
     means = {}
     used_bands = []
-    tt = tab[ (tab['time'] >= jdstart) & (tab['time'] <= jdend) ]
-    for band in set(tt['band']):
-        btt = tt[tt['band']==band]
-        means[band] = np.average( btt['flux'], weights=1./btt['fluxerr']**2)
+    tt = tab[(tab["time"] >= jdstart) & (tab["time"] <= jdend)]
+    for band in set(tt["band"]):
+        btt = tt[tt["band"] == band]
+        means[band] = np.average(btt["flux"], weights=1.0 / btt["fluxerr"] ** 2)
+        #        means[band] = 1
         used_bands.append(band)
     return means, used_bands
 
+
 def getBandBits(bands: Sequence):
     """
     Return number quantifying which bands are included.
     """
-    bandval = {'lsstu':1, 'lsstg':2, 'lsstr':4, 'lssti':8, 'lsstz':16, 'lssty':32}
+    bandval = {
+        "lsstu": 1,
+        "lsstg": 2,
+        "lsstr": 4,
+        "lssti": 8,
+        "lsstz": 16,
+        "lssty": 32,
+        "ztfg": 64,
+        "ztfr": 128,
+        "ztfi": 256,
+    }
     index = 0
     for band in bands:
         index += bandval[band]
     return index
 
 
+class FitFailed(RuntimeError):
+    ...
+
+
 class T2TabulatorRiseDeclineBase(AmpelBaseModel):
     """
-    Derive a number of simple metrics describing the rise, peak and decline of a lc.
+     Derive a number of simple metrics describing the rise, peak and decline of a lc.
 
-    This version assumes input provided by flux table.
+     This version assumes input provided by flux table.
 
-    Derived values:
-    * t_predetect : time between first detection and previous non-detection
-                    in "significant bands". Todo: add min error?
-    * t_lc : duration (time between first and most recent detection)
-    * jd_max : jd of peak light. None unless bool_peaked
-    * jd_det : jd of first detection
-    * jd_last : jd of last detection
-    * ndet : number of significant detections
-    * bool_peaked : is the lc estimated to be declining?
-    * bool_pure : has there been no significant non-detections after first detection?
-    * bool_rise : was the peak light within "cadence" days of the most recent detection?
-   # Not yet implemented    * bool_norise : was the first detection NOT significantly fainter than
-        mag_peak IF bool_peaked, ELSE mag_lst
-    * bool_hasgaps : The lc has a gap between detections of at least 30 days,
-        indicating either a recurrent event or a chance coincidental detection.
-    * mag_peak : magnitude at peak light (significant band). Only calculated if bool_peaked
-    * mag_det : detection magnitude (significant band)
-    * mag_last : magnitude of last detection (significant band)
-    Following done for each "color_list" i-ii
-    * i-ii_peak : color at peak. None unless bool_peaked AND i+ii obs made within
-                 "cadence"  days of jd_max
-    * i-ii_det : color at detection. None unless i+ii obs made within "cadence"
-                  days of jd_det
-    * i-ii_last : color at last detection. None unless i+ii obs made within
-                  "cadence" days of jd_last
-    * slope_rise_{i,ii} : magnitude slope between jd_det and jd_max. None if bool_norise
-    * slope_decline_{i,ii} : magnitude slope between jd_max and jd_lst. None unless bool_peaked
-
-    Additionally, we would like to access host properties like distance and host mags and sizes.
-    Would that have to be a different T2?.
-    Rather make a different T2 which is chained to the redshift sampler and this.
-
-    "t_cadence" is meant to approximate the rough practical cadence, i.e. how often repeated
-    observations should come and what can be seen as "simulateneous"
+     Derived values:
+     * t_predetect : time between first detection and previous non-detection
+                     in "significant bands". Todo: add min error?
+     * t_lc : duration (time between first and most recent detection)
+     * jd_max : jd of peak light. None unless bool_peaked
+     * jd_det : jd of first detection
+     * jd_last : jd of last detection
+     * ndet : number of significant detections
+     * bool_peaked : is the lc estimated to be declining?
+     * bool_pure : has there been no significant non-detections after first detection?
+     * bool_rise : was the peak light within "cadence" days of the most recent detection?
+    # Not yet implemented    * bool_norise : was the first detection NOT significantly fainter than
+         mag_peak IF bool_peaked, ELSE mag_lst
+     * bool_hasgaps : The lc has a gap between detections of at least 30 days,
+         indicating either a recurrent event or a chance coincidental detection.
+     * mag_peak : magnitude at peak light (significant band). Only calculated if bool_peaked
+     * mag_det : detection magnitude (significant band)
+     * mag_last : magnitude of last detection (significant band)
+     Following done for each "color_list" i-ii
+     * i-ii_peak : color at peak. None unless bool_peaked AND i+ii obs made within
+                  "cadence"  days of jd_max
+     * i-ii_det : color at detection. None unless i+ii obs made within "cadence"
+                   days of jd_det
+     * i-ii_last : color at last detection. None unless i+ii obs made within
+                   "cadence" days of jd_last
+     * slope_rise_{i,ii} : magnitude slope between jd_det and jd_max. None if bool_norise
+     * slope_decline_{i,ii} : magnitude slope between jd_max and jd_lst. None unless bool_peaked
+
+     Additionally, we would like to access host properties like distance and host mags and sizes.
+     Would that have to be a different T2?.
+     Rather make a different T2 which is chained to the redshift sampler and this.
+
+     "t_cadence" is meant to approximate the rough practical cadence, i.e. how often repeated
+     observations should come and what can be seen as "simulateneous"
 
-    "significant_bands" is a list of "deep bands". Collected data from these will be
-    used to calculate ages, peak magnitude etc.
+     "significant_bands" is a list of "deep bands". Collected data from these will be
+     used to calculate ages, peak magnitude etc.
 
-    "sigma_det" quantifies what should be seen as a detection.
+     "sigma_det" quantifies what should be seen as a detection.
 
-    "color_list" contains a list of lists of colors which should be considered
+     "color_list" contains a list of lists of colors which should be considered
 
     """
 
-
-    t_cadence: float = 5.
-    significant_bands: Sequence[str] = ['lsstg', 'lsstr', 'lssti', 'lsstz']
-    sigma_det: float = 5.
-    sigma_slope: float = 3. # Threshold for having detected a slope
-    color_list: Sequence[Sequence[str]] = [['lsstu','lsstg'], ['lsstg','lsstr'],
-                        ['lsstr','lssti'], ['lssti','lsstz'],['lsstz','lssty']]
+    t_cadence: float = 5.0
+    significant_bands: Sequence[str] = ["lsstg", "lsstr", "lssti", "lsstz"]
+    sigma_det: float = 5.0
+    sigma_slope: float = 3.0  # Threshold for having detected a slope
+    color_list: Sequence[Sequence[str]] = [
+        ["lsstu", "lsstg"],
+        ["lsstg", "lsstr"],
+        ["lsstr", "lssti"],
+        ["lssti", "lsstz"],
+        ["lsstz", "lssty"],
+        ["ztg", "ztfr"],
+        ["ztfr", "ztfi"],
+    ]
     max_tgap: int = 30
 
     # Cut the lightcurve if longer than this limit.
     # Motivated by worse classification for longer (inbalanced training?)
-    max_ndet: int = 20
+    # max_ndet: int = 20
+    # For new training round, change this
+    max_ndet: int = 200000
 
     if TYPE_CHECKING:
         logger: LoggerProtocol
 
     def get_bandfeatures(self, ftable):
         """
         Go through all bands of input table and:
         - Try to find a peak, together with rise and fall slopes.
         - Based on this try to determine if it is rising, falling and have peaked.
         - Storing slopes where possible.
         """
 
-        def linearFunc(x,intercept,slope):
-            y = intercept + slope * x
-            return y
+        def linearFunc(x, intercept, slope):
+            return intercept + slope * x
 
         banddata = {}
-        tscale = np.mean(ftable['time'])
+        tscale = np.mean(ftable["time"])
 
-        for band in set(ftable['band']):
-            bt = ftable[ftable['band'] == band]
+        for band in set(ftable["band"]):
+            bt = ftable[ftable["band"] == band]
 
-            max_flux = bt['flux'].max()
-            max_flux_time = bt[bt['flux']==max_flux]['time'][0]
-            banddata['jd_peak_'+band] = max_flux_time
+            max_flux = bt["flux"].max()
+            max_flux_time = bt[bt["flux"] == max_flux]["time"][0]
+            banddata["jd_peak_" + band] = max_flux_time
 
             # Divide Table
-            riset = bt[ bt['time']<=max_flux_time ]
-            fallt = bt[ bt['time']>=max_flux_time ]
+            riset = bt[bt["time"] <= max_flux_time]
+            fallt = bt[bt["time"] >= max_flux_time]
 
             # Examine rise
-            if len(riset)>1:
-                fit, cov=curve_fit(linearFunc,riset['time']-tscale,riset['flux'],
-                                    sigma=riset['fluxerr'],absolute_sigma=True)
-                banddata['rise_slope_'+band] = fit[1]
-                banddata['rise_slopesig_'+band] = fit[1] / np.sqrt(cov[1][1])
-            if len(fallt)>1:
-                fit, cov=curve_fit(linearFunc,fallt['time']-tscale,fallt['flux'],
-                                    sigma=fallt['fluxerr'],absolute_sigma=True)
-                banddata['fall_slope_'+band] = fit[1]
-                banddata['fall_slopesig_'+band] = fit[1] / np.sqrt(cov[1][1])
+            if len(riset) > 1:
+                try:
+                    fit, cov = curve_fit(
+                        linearFunc,
+                        riset["time"] - tscale,
+                        riset["flux"],
+                        sigma=riset["fluxerr"],
+                        absolute_sigma=True,
+                    )
+                    banddata["rise_slope_" + band] = fit[1]
+                    banddata["rise_slopesig_" + band] = fit[1] / np.sqrt(cov[1][1])
+                except RuntimeError:
+                    self.logger.info("Risetime curve fit failed.")
+            if len(fallt) > 1:
+                try:
+                    fit, cov = curve_fit(
+                        linearFunc,
+                        fallt["time"] - tscale,
+                        fallt["flux"],
+                        sigma=fallt["fluxerr"],
+                        absolute_sigma=True,
+                    )
+                    banddata["fall_slope_" + band] = fit[1]
+                    banddata["fall_slopesig_" + band] = fit[1] / np.sqrt(cov[1][1])
+                except RuntimeError:
+                    self.logger.info("Falltime curve fit failed.")
 
         # In v1 we also had a requirement that a sufficient time should have
         # passed after peak, such that we "should" have seen a decline.
         # We here skip this, hopefully the slope fit is sufficient
 
         # Check whether we have a significant rise detected in any band.
-        risepulls = [ banddata.get('rise_slopesig_'+band,0)
-                        for band in set(ftable['band']) ]
-        if sum(risepulls)>self.sigma_slope:
-            banddata['bool_rise'] = True
+        risepulls = [
+            banddata.get("rise_slopesig_" + band, 0) for band in set(ftable["band"])
+        ]
+        if sum(risepulls) > self.sigma_slope:
+            banddata["bool_rise"] = True
         else:
-            banddata['bool_rise'] = False
+            banddata["bool_rise"] = False
         # Check whether we see a decline
-        decpulls = [ banddata.get('fall_slopesig_'+band,0)
-                        for band in set(ftable['band']) ]
+        decpulls = [
+            banddata.get("fall_slopesig_" + band, 0) for band in set(ftable["band"])
+        ]
         if sum(decpulls) < -self.sigma_slope:
-            banddata['bool_fall'] = True
+            banddata["bool_fall"] = True
         else:
-            banddata['bool_fall'] = False
+            banddata["bool_fall"] = False
 
         # If the transient has both a rise and a fall we can
         # define a central peak
-        if banddata['bool_rise'] and banddata['bool_fall']:
-            banddata['bool_peaked'] = True
+        if (
+            banddata["bool_rise"]
+            and banddata["bool_fall"]
+            and (
+                len(
+                    peakjds := [
+                        banddata["jd_peak_" + band]
+                        for band in set(ftable["band"])
+                        if "rise_slope_" + band in banddata
+                        and "fall_slope_" + band in banddata
+                    ]
+                )
+                > 0
+            )
+        ):
+            banddata["bool_peaked"] = True
             # Use jd of all bands for which we could estimate rise+fall
-            banddata['jd_peak'] = np.median(
-                                [ banddata['jd_peak_'+band]
-                                       for band in set(ftable['band'])
-                                  if 'rise_slope_'+band in banddata and
-                                     'fall_slope_'+band in banddata] )
+            banddata["jd_peak"] = np.median(peakjds)
         else:
-            banddata['bool_peaked'] = False
+            banddata["bool_peaked"] = False
 
         # Could include the abs mag at peak, but we argued this would not
         # be as useful?
 
         return banddata
 
-
-
     def cut_flux_table(self, flux_table: Table) -> Table:
         """
         Limit to some _total_ set of significant detections.
         """
-        sig_mask = (flux_table['flux']) / flux_table['fluxerr']>self.sigma_det
-        sig_time = list( flux_table['time'][sig_mask] )
-        if len(sig_time)>self.max_ndet:
+        sig_mask = np.abs((flux_table["flux"]) / flux_table["fluxerr"]) > self.sigma_det
+        sig_time = list(flux_table["time"][sig_mask])
+        if len(sig_time) > self.max_ndet:
             max_time = sorted(sig_time)[self.max_ndet]
-            flux_table = flux_table[ flux_table['time']<=max_time ]
+            flux_table = flux_table[flux_table["time"] <= max_time]
 
         return flux_table
 
+    def average_filtervalues(
+        self, features: dict[str, Any], matchlist: Iterable[str] = tuple()
+    ) -> dict[str, Any]:
+        """
+        Many (most) features calculated per band or color, with available filter/color varying from object
+        to object.
 
+        This method will attempt to average over any filter or color-specific fields available and create an averaged entry.
 
+        A base matchlist is created based on significant bands. (plus potentially an input matchlist)
 
-    def compute_stats(self, flux_table: Table) -> dict[str, Any]:
+        """
+
+        mymatchlist = [f"_{band}_" for band in self.significant_bands]
+        # Ignore the colors for now, would need to rework how these averages are described.
+        # mymatchlist.extend(
+        # ['{}-{}_'.format(col[0],col[1]) for col in self.color_list]
+        #    )
+        mymatchlist.extend(matchlist)
+
+        matchedvalues: dict[str, list] = {}
+        # Can this be redone to avoid nested loop?
+        for match in mymatchlist:
+            p = re.compile(match)
+            for key, val in features.items():
+                stub = p.sub("_", key)  # Name of averaged entry in return dict
+                if stub == key:  # Match string not found
+                    continue
+                if stub not in matchedvalues:
+                    matchedvalues[stub] = []
+                matchedvalues[stub].append(val)
 
+        return {k: np.nanmean(v) for k, v in matchedvalues.items()}
+
+    def compute_stats(self, flux_table: Table) -> dict[str, Any]:
         # Output dict that we will start to populate
         o: dict[str, Any] = {}
 
-        # Step 1. Base determinations based on combined detections
-        self.logger.debug("Starting joint band RiseDeclineStat estimations")
-
         # Create subset of table with significant detections in significant bands
-        band_mask = [bandobs in self.significant_bands for bandobs in flux_table['band'] ]
-        sig_mask = (flux_table['flux']) / flux_table['fluxerr']>self.sigma_det
+        band_mask = [
+            bandobs in self.significant_bands for bandobs in flux_table["band"]
+        ]
+        sig_mask = np.abs((flux_table["flux"]) / flux_table["fluxerr"]) > self.sigma_det
         det_table = flux_table[band_mask & sig_mask]
+        # Calculate fraction negative detection (we no longer cut only because of this)
+        o["ndet"] = len(det_table)
 
-        o['ndet'] = len(det_table)
-        if o['ndet']==0:
-            o['success'] = False
-            o['cause'] = "No data survive significance criteria."
+        if o["ndet"] == 0:
+            o["success"] = False
+            o["cause"] = "No data survive significance criteria."
             # Gather additional information for evaluation
-            o['alldet'] = len(flux_table)
-            neg_mask = (-flux_table['flux']) / flux_table['fluxerr']>self.sigma_det
-            o['nnegdet'] = len( flux_table[band_mask & neg_mask] )
+            o["alldet"] = len(flux_table)
+            neg_mask = (-flux_table["flux"]) / flux_table["fluxerr"] > self.sigma_det
+            o["nnegdet"] = len(flux_table[band_mask & neg_mask])
 
             return o
 
-        o["jd_det"] = det_table['time'].min()
-        o["jd_last"] = det_table['time'].max()
+        o["frac_pos"] = np.sum(det_table["flux"] > 0) / o["ndet"]
+
+        o["jd_det"] = det_table["time"].min()
+        o["jd_last"] = det_table["time"].max()
+        o["t_lc"] = o["jd_last"] - o["jd_det"]
 
         # Get the max time of obs in signifant bands prior to jd_det
-        if flux_table[band_mask]['time'].min()<o['jd_det']:
-            o["t_predetect"] = o['jd_det'] - flux_table[band_mask][
-                    flux_table['time'][band_mask]<o["jd_det"] ]['time'].max()
+        if flux_table[band_mask]["time"].min() < o["jd_det"]:
+            o["t_predetect"] = (
+                o["jd_det"]
+                - flux_table[band_mask][flux_table["time"][band_mask] < o["jd_det"]][
+                    "time"
+                ].max()
+            )
         else:
             o["t_predetect"] = None
 
-        o["mag_det"] = float( getMag(flux_table[flux_table['time']==o["jd_det"]]) )
-        o["band_det_id"] = getBandBits( [flux_table[flux_table['time']==o["jd_det"]]['band'][0]] )
-
-        o["mag_last"] = float( getMag(flux_table[flux_table['time']==o["jd_last"]]) )
-        o["band_last_id"] = getBandBits( [flux_table[flux_table['time']==o["jd_last"]]['band'][0]] )
+        # Magnitude and color calculations below assume detections are positive
+        if (
+            flux_table[flux_table["time"] == o["jd_det"]]["flux"] < 0
+            or flux_table[flux_table["time"] == o["jd_last"]]["flux"] < 0
+        ):
+            # Did we succeed with feature calculation or not?
+            o["success"] = True
+            return o
 
-        o["t_lc"] = o["jd_last"] - o["jd_det"]
+        o["mag_det"] = float(getMag(flux_table[flux_table["time"] == o["jd_det"]]))
+        o["band_det_id"] = getBandBits(
+            [flux_table[flux_table["time"] == o["jd_det"]]["band"][0]]
+        )
+
+        o["mag_last"] = float(getMag(flux_table[flux_table["time"] == o["jd_last"]]))
+        o["band_last_id"] = getBandBits(
+            [flux_table[flux_table["time"] == o["jd_last"]]["band"][0]]
+        )
+
+        # Check fails irregularly
+        try:
+            o["mag_min"] = float(
+                getMag(flux_table[flux_table["flux"] == max(flux_table["flux"])])
+            )
+        except TypeError:
+            self.logger.info("Mag min extraction failed.")
+
+        try:
+            o["jd_min"] = float(flux_table["time"][np.argmax(flux_table["flux"])])
+        except TypeError:
+            self.logger.info("JD at mag min extraction failed.")
 
         # Check for non-signficant obs between det and last
         ultab = flux_table[band_mask & ~sig_mask]
-        if sum( (ultab['time']>=o["jd_det"]) & (ultab['time']<=o["jd_last"]) )==0:
+        if sum((ultab["time"] >= o["jd_det"]) & (ultab["time"] <= o["jd_last"])) == 0:
             # No non-detection among signifcant bands between start and end
             o["bool_pure"] = True
         else:
             o["bool_pure"] = False
 
         # We start measuring bandfeatures t_cadence days prior to first detection
         # to allow some nondetection data to be included.
         # (Note: we previously only used significant bands here. Prob wrong. )
-        time_mask = ( (flux_table['time']>(o['jd_det']-self.t_cadence)) &
-                      (flux_table['time']<(o['jd_last']+self.t_cadence)) )
-        o.update( self.get_bandfeatures(flux_table[time_mask]) )
-
+        time_mask = (flux_table["time"] > (o["jd_det"] - self.t_cadence)) & (
+            flux_table["time"] < (o["jd_last"] + self.t_cadence)
+        )
+        o.update(self.get_bandfeatures(flux_table[time_mask]))
 
         # If there is a peak we additionally check whether this is within t_cadence
         # days of detector or last, and call this fastrise and fastfall
-        o['bool_fastrise'], o['bool_fastfall'] = None, None
-        if o['bool_peaked']:
-            if np.abs(o['jd_det']-o['jd_peak'])<self.t_cadence:
-                o['bool_fastrise'] = True
+        o["bool_fastrise"], o["bool_fastfall"] = None, None
+        if o.get("bool_peaked", False):
+            if np.abs(o["jd_det"] - o["jd_peak"]) < self.t_cadence:
+                o["bool_fastrise"] = True
             else:
-                o['bool_fastrise'] = False
-            if np.abs(o['jd_last']-o['jd_peak'])<self.t_cadence:
-                o['bool_fastfall'] = True
+                o["bool_fastrise"] = False
+            if np.abs(o["jd_last"] - o["jd_peak"]) < self.t_cadence:
+                o["bool_fastfall"] = True
             else:
-                o['bool_fastfall'] = False
-            o['t_rise'] = o['jd_peak'] - o['jd_det']
-            o['t_fall'] = o['jd_last'] - o['jd_peak']
+                o["bool_fastfall"] = False
+            o["t_rise"] = o["jd_peak"] - o["jd_det"]
+            o["t_fall"] = o["jd_last"] - o["jd_peak"]
 
         # Are there long gaps among the detections?
         jdsorted = np.unique(flux_table["time"])
         if len(jdsorted) > 1:
             if (jdsorted[1:] - jdsorted[0:-1]).max() > self.max_tgap:
                 o["bool_hasgaps"] = True
             else:
@@ -308,46 +424,156 @@
         # Color
         # Define time subsets at detection, last (significant) and peak (if defined)
         # In each, get the mean flux in each band.
         # We assume that the zeropoint is the same for these fluxes!
         # Also, only exist for positive fluxes (...)
 
         # Detection colors
-        fluxdict, fluxbands =  getMeanflux(flux_table, o["jd_det"]-self.t_cadence/2,
-                                            o["jd_det"]+self.t_cadence/2)
-        o['det_bands'] = getBandBits(fluxbands)
+        fluxdict, fluxbands = getMeanflux(
+            flux_table,
+            o["jd_det"] - self.t_cadence / 2,
+            o["jd_det"] + self.t_cadence / 2,
+        )
+        o["det_bands"] = getBandBits(fluxbands)
         for colbands in self.color_list:
-            if fluxdict.get(colbands[0],-1)>0 and fluxdict.get(colbands[1],-1)>0:
-                o[f"{colbands[0]}-{colbands[1]}_det"] = -2.5 * np.log10(fluxdict[colbands[0]] / fluxdict[colbands[1]])
+            if fluxdict.get(colbands[0], -1) > 0 and fluxdict.get(colbands[1], -1) > 0:
+                o[f"{colbands[0]}-{colbands[1]}_det"] = -2.5 * np.log10(
+                    fluxdict[colbands[0]] / fluxdict[colbands[1]]
+                )
         # Last obs colors
-        fluxdict, fluxbands =  getMeanflux(flux_table, o["jd_last"]-self.t_cadence/2,
-                                            o["jd_last"]+self.t_cadence/2)
-        o['last_bands'] = getBandBits(fluxbands)
+        fluxdict, fluxbands = getMeanflux(
+            flux_table,
+            o["jd_last"] - self.t_cadence / 2,
+            o["jd_last"] + self.t_cadence / 2,
+        )
+        o["last_bands"] = getBandBits(fluxbands)
         for colbands in self.color_list:
-            if fluxdict.get(colbands[0],-1)>0 and fluxdict.get(colbands[1],-1)>0:
-                o[f"{colbands[0]}-{colbands[1]}_last"] = -2.5 * np.log10(fluxdict[colbands[0]] / fluxdict[colbands[1]])
+            if fluxdict.get(colbands[0], -1) > 0 and fluxdict.get(colbands[1], -1) > 0:
+                o[f"{colbands[0]}-{colbands[1]}_last"] = -2.5 * np.log10(
+                    fluxdict[colbands[0]] / fluxdict[colbands[1]]
+                )
         # Peak colors, if found
-        if o['bool_peaked']:
-            fluxdict, fluxbands =  getMeanflux(flux_table, o["jd_peak"]-self.t_cadence/2,
-                                                o["jd_peak"]+self.t_cadence/2)
-            o['peak_bands'] = getBandBits(fluxbands)
+        if o.get("bool_peaked", False):
+            fluxdict, fluxbands = getMeanflux(
+                flux_table,
+                o["jd_peak"] - self.t_cadence / 2,
+                o["jd_peak"] + self.t_cadence / 2,
+            )
+            o["peak_bands"] = getBandBits(fluxbands)
             for colbands in self.color_list:
-                if fluxdict.get(colbands[0],-1)>0 and fluxdict.get(colbands[1],-1)>0:
-                    o[f"{colbands[0]}-{colbands[1]}_peak"] = -2.5 * np.log10(fluxdict[colbands[0]] / fluxdict[colbands[1]])
-
+                if (
+                    fluxdict.get(colbands[0], -1) > 0
+                    and fluxdict.get(colbands[1], -1) > 0
+                ):
+                    o[f"{colbands[0]}-{colbands[1]}_peak"] = -2.5 * np.log10(
+                        fluxdict[colbands[0]] / fluxdict[colbands[1]]
+                    )
 
         o["success"] = True
         return o
 
 
-class T2TabulatorRiseDecline(AbsStateT2Unit, AbsTabulatedT2Unit, T2TabulatorRiseDeclineBase):
+class BaseLightCurveFeatures(LogicalUnit, AmpelBaseModel):
+    """
+    Calculate various features of the light curve using the light-curve
+    package described in https://ui.adsabs.harvard.edu/abs/2021MNRAS.502.5147M%2F/abstract
+
+    Lifted from T2LightCurveFeatures
+    Installed as  python3 -mpip install light-curve
 
-    plot_prob: float = 0.
+    This v2 contains feature selection and choice of flux as unit based on most common features to influence
+    a binary tree classifier (compare rank_tabulator_features and previous version of this unit).
+    Also decided to require 4 detection in a band for using.
+    """
+
+    #: Features to extract from the light curve.
+    #: See: https://docs.rs/light-curve-feature/0.2.2/light_curve_feature/features/index.html
+    lightcurve_features_flux: dict[str, None | dict[str, Any]] = {
+        "Eta": None,  # 2
+        "MaximumSlope": None,  # 2
+        "Periodogram": {"peaks": 1},  # 4?
+        "Skew": None,  # 3
+        "StandardDeviation": None,  # 2
+        "ExcessVariance": None,  # 2
+        "LinearFit": None,  # 3
+        "AndersonDarlingNormal": None,  # 4
+        "Kurtosis": None,  # 4
+        "StetsonK": None,  # 2
+    }
+
+    #: Bandpasses to use
+    lightcurve_bands: dict[str, Any] = {
+        "ztfg": "ztfg",
+        "ztfr": "ztfr",
+        "ztfi": "ztfi",
+        "lsstu": "lsstu",
+        "lsstg": "lsstg",
+        "lsstr": "lsstr",
+        "lssti": "lssti",
+        "lsstz": "lsstz",
+        "lssty": "lssty",
+    }
+
+    def init_lightcurve_extractor(self) -> None:
+        self.fluxextractor = light_curve.Extractor(
+            *(
+                getattr(light_curve, k)(**(v or {}))
+                for k, v in self.lightcurve_features_flux.items()
+            )
+        )
+
+    def post_init(self) -> None:
+        self.init_lightcurve_extractor()
+
+    def extract_lightcurve_features(self, flux_table: Table) -> dict[str, float]:
+        result = {}
+        #
+        for band, fid in self.lightcurve_bands.items():
+            if (in_band := flux_table[flux_table["band"] == fid]) is None:
+                continue
+
+            # Conversion to mag not used if features determined in flux space
+            # m, merr, mtime = getMag(in_band, err=True, time=True)
+
+            # We wrap this in a try statement, since there are a few ways these can fail, typically with poor data in one or another aspect
+            try:
+                # Flux based, requires at least 4 detections
+                if len(in_band["flux"]) >= 4:
+                    lcout = {
+                        f"{k}_{band}_flux": v
+                        for k, v in zip(
+                            self.fluxextractor.names,
+                            self.fluxextractor(
+                                in_band["time"], in_band["flux"], in_band["fluxerr"]
+                            ),
+                            strict=False,
+                        )
+                    }
+                    result.update(lcout)
+            except ValueError:
+                self.logger.info("lightkurve extract fail")
+                pass
+
+        return result
+
+
+class T2TabulatorRiseDecline(
+    AbsStateT2Unit,
+    AbsTabulatedT2Unit,
+    T2TabulatorRiseDeclineBase,
+    BaseLightCurveFeatures,
+):
+    plot_prob: float = 0.0
     path_testplot: str = "/home/jnordin/tmp/t2test/"
 
+    #    def __init__(self, **kwargs):
+    #        super().__init__(**kwargs)
+    #    def super().post_init(self):
+    #        super().__init__(**kwargs)
+
     def test_plot(self, name, table, t2result):
         """
         for debugging
 
         Create panel for each band, showing data + the significant dets.
 
         Mark times for detection, last det + peak (if set)
@@ -356,98 +582,112 @@
 
         Save as stockid + ndet
 
         """
 
         import matplotlib.pyplot as plt
 
-        bands = set(table['band'])
+        bands = set(table["band"])
 
         fig, axs = plt.subplots(2, 3)
 
         for k, band in enumerate(bands):
-            bt = table[table['band']==band]
-            ax = axs[int(k/3), k%3]
+            bt = table[table["band"] == band]
+            ax = axs[int(k / 3), k % 3]
 
-            ax.errorbar(bt['time'], bt['flux'], yerr=bt['fluxerr'],
-                            fmt='o', label=band)
+            ax.errorbar(bt["time"], bt["flux"], yerr=bt["fluxerr"], fmt="o", label=band)
 
             # Detection times
-            if 'jd_det' in t2result:
-                ax.axvline(t2result["jd_det"], color='grey', linewidth=3, alpha=0.5 )
-            if 'jd_last' in t2result:
-                ax.axvline(t2result["jd_last"], color='grey', linewidth=3, alpha=0.5 )
-            if t2result['bool_peaked']:
-                ax.axvline(t2result["jd_peak"], color='red', linewidth=2, alpha=0.8 )
-            if 'jd_peak_'+band in t2result:
-                ax.axvline(t2result["jd_peak_"+band], color='green', linewidth=1)
+            if "jd_det" in t2result:
+                ax.axvline(t2result["jd_det"], color="grey", linewidth=3, alpha=0.5)
+            if "jd_last" in t2result:
+                ax.axvline(t2result["jd_last"], color="grey", linewidth=3, alpha=0.5)
+            if t2result["bool_peaked"]:
+                ax.axvline(t2result["jd_peak"], color="red", linewidth=2, alpha=0.8)
+            if "jd_peak_" + band in t2result:
+                ax.axvline(t2result["jd_peak_" + band], color="green", linewidth=1)
 
             # We next wich to indicate the slopes we have measured
-            if 'rise_slope_'+band in t2result:
-                slope = t2result['rise_slope_'+band]
-                startpoint = t2result['jd_det']
-                xvals = np.array([-t2result['t_lc']/4, t2result['t_lc']/4])
-                yvals = xvals * t2result['rise_slope_'+band] + np.mean(bt['flux'])
-                xvals += (t2result['jd_det']+t2result['t_lc']/4)
-                col = 'black'
-                if np.abs(t2result['rise_slopesig_'+band])>3:
-                    col = 'red'
-                ax.plot(xvals,yvals,color=col)
-            if 'fall_slope_'+band in t2result:
-                xvals = np.array([-t2result['t_lc']/4, t2result['t_lc']/4])
-                yvals = xvals * t2result['fall_slope_'+band] + np.mean(bt['flux'])
-                xvals += (t2result['jd_last']-t2result['t_lc']/4)
-                col = 'black'
-                if np.abs(t2result['fall_slopesig_'+band])>3:
-                    col = 'red'
-                ax.plot(xvals,yvals,color=col)
+            if "rise_slope_" + band in t2result:
+                xvals = np.array([-t2result["t_lc"] / 4, t2result["t_lc"] / 4])
+                yvals = xvals * t2result["rise_slope_" + band] + np.mean(bt["flux"])
+                xvals += t2result["jd_det"] + t2result["t_lc"] / 4
+                col = "black"
+                if np.abs(t2result["rise_slopesig_" + band]) > 3:
+                    col = "red"
+                ax.plot(xvals, yvals, color=col)
+            if "fall_slope_" + band in t2result:
+                xvals = np.array([-t2result["t_lc"] / 4, t2result["t_lc"] / 4])
+                yvals = xvals * t2result["fall_slope_" + band] + np.mean(bt["flux"])
+                xvals += t2result["jd_last"] - t2result["t_lc"] / 4
+                col = "black"
+                if np.abs(t2result["fall_slopesig_" + band]) > 3:
+                    col = "red"
+                ax.plot(xvals, yvals, color=col)
 
-
-#            ax.legend()
-            ax.set_xlabel('MJD')
+            #            ax.legend()
+            ax.set_xlabel("MJD")
             ax.set_ylabel(band)
 
             # Create text string
-            title = "ndet: %s " % (
-                t2result["ndet"]
-                )
+            title = "ndet: %s " % (t2result["ndet"])
 
-            for boolprop in ["peaked", "pure", "rise", "hasgaps", "fall", "fastrise", "fastfall"]:
+            for boolprop in [
+                "peaked",
+                "pure",
+                "rise",
+                "hasgaps",
+                "fall",
+                "fastrise",
+                "fastfall",
+            ]:
                 if t2result[f"bool_{boolprop}"]:
                     title += f"{boolprop} "
 
-            ax.set_title(title,{'fontsize':8})
+            ax.set_title(title, {"fontsize": 8})
 
         # Store figure
-        path = os.path.join(self.path_testplot, "{}_{}.pdf".format(name, t2result['ndet']))
+        path = os.path.join(
+            self.path_testplot, "{}_{}.pdf".format(name, t2result["ndet"])
+        )
         plt.tight_layout()
         plt.savefig(path)
         plt.clf()
 
-
-
-    def process(self,
+    def process(
+        self,
         compound: T1Document,
         datapoints: Iterable[DataPoint],
-        ) -> Union[UBson, UnitResult]:
+    ) -> dict[str, Any]:
         """
         Process datapoints belonging to one state of one transient.
         A commong Table is generated which is used as input
         to the feature generator.
         """
 
         # Convert input datapoints to standardized Astropy Table
         # Using standard tabulators
         flux_table = self.get_flux_table(datapoints)
 
         # Cut the flux table if requested
-        if self.max_ndet>0 and len(flux_table)>self.max_ndet:
+        if self.max_ndet > 0 and len(flux_table) > self.max_ndet:
             flux_table = self.cut_flux_table(flux_table)
 
         # Calculate get_features
         features = self.compute_stats(flux_table)
 
-        #if self.do_testplot:
-        if features['success'] and np.random.uniform()<self.plot_prob:
-            self.test_plot(compound.get('stock'), flux_table, features)
+        # Calculate light_curve features
+        lcfeat = self.extract_lightcurve_features(flux_table)
+        features.update(lcfeat)
+        # features.update(
+        #    self.extract_lightcurve_features(flux_table)
+        #    )
+
+        # Create averaged values
+        avgfeat = self.average_filtervalues(features)
+        features.update(avgfeat)
+
+        # if self.do_testplot:
+        if features.get("success") and np.random.uniform() < self.plot_prob:
+            self.test_plot(compound.get("stock"), flux_table, features)
 
         return features
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/AstroColibriClient.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,92 +6,115 @@
 # Date:                13.11.2022
 # Last Modified Date:  13.11.2022
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
 # FIXME: restore mypy when this is actually ready
 # type: ignore
 
-from typing import Sequence, Dict, Any, Union
+import base64
+import json
+from typing import Any
 
-import requests
-#import json
 import backoff
+import requests
 from requests import HTTPError
 from requests.auth import HTTPBasicAuth
-#from datetime import datetime
-#from astropy.time import Time
 
-url = 'https://astro-colibri.herokuapp.com/add_ampel_transient'
+# from datetime import datetime
+# from astropy.time import Time
+
+# url = 'https://astro-colibri.herokuapp.com/add_ampel_transient'
+
 
 class AstroColibriPhot:
     mag: float
     band: str
-    datetime: str # e.g. datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
+    datetime: str  # e.g. datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
+
 
 class AstroColibriPost:
-    timestamp: str            # Timestamp of first detection
-    trigger_id: str           # AstroColibri identifier -> should be TNS ID
-    # ampel_id: str             # Internal AMPEL ID. To be added
-    # ivorn: str | None = None  # If existing, this can be added.
+    timestamp: str  # Timestamp of first detection
+    trigger_id: str  # AstroColibri identifier -> should be TNS ID
+    source_name: str  #  SN|AT[space]2022ajn
     ra: float
     dec: float
     err: float
-    type: str = 'ot_sn'       # 'ot_sn'
-    observatory: str | None = 'ztf'
-    source_name: str          #  SN|AT[space]2022ajn
+    type: str = "ot_sn"  # 'ot_sn'
+    observatory: str | None = "ztf"
     ampel_attributes: list[str] = []
-    photometry:  dict[str, AstroColibriPhot]
-    discovery_name: str      #  ZTFxxx
+    photometry: dict[str, AstroColibriPhot]
+    discovery_name: str  #  ZTFxxx
+    # dev
+    # ampel_id: str             # Internal AMPEL ID. To be added
+    # ivorn: str | None = None  # If existing, this can be added.
 
 
 class AstroColibriClient:
     """
     Initiate a session for communicating with an AstroColibri instance.
 
     """
 
     # url (currently test version)
-    colibri_url = 'https://astro-colibri.herokuapp.com/add_ampel_transient'
-
+    # colibri_url = 'https://astro-colibri.herokuapp.com/add_ampel_transient'
+    api_url = "https://astro-colibri.science"
 
     def __init__(self, colibri_username: str, colibri_password: str, logger):
         self.logger = logger
 
         self.session = requests.session()
         self.session.auth = HTTPBasicAuth(colibri_username, colibri_password)
         # or ?
         # self.auth=HTTPBasicAuth(colibri_username, colibri_password)
 
+    def store_image(self, image_file: str):
+        with open(image_file, "rb") as f:
+            im_bytes = f.read()
+        im_b64 = base64.b64encode(im_bytes).decode("utf8")
+        headers = {"Content-type": "application/json", "Accept": "text/plain"}
+        payload = json.dumps(
+            {"image": im_b64, "file_name": image_file, "other_key": "value"}
+        )
+        #        print('image payload', payload)
+        #        response = requests.post(self.api_url+'/add_image_to_storage',
+        #                            data=payload, headers=headers, auth=self.session.auth)
+        response = self.session.post(
+            self.api_url + "/add_image_to_storage", data=payload, headers=headers
+        )
+        return response.json()["url_lc"]
 
     # robustify post
     @backoff.on_exception(
         backoff.expo,
         requests.ConnectionError,
         max_tries=5,
         factor=10,
-        )
+    )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: not isinstance(e, HTTPError) or e.response.status_code not in {503, 504, 429, 408},
+        giveup=lambda e: not isinstance(e, HTTPError)
+        or e.response.status_code not in {503, 504, 429, 408},
         max_time=60,
-        )
-    def firestore_post(self, data: AstroColibriPost )->Dict[Any,Any]:
-
-        print('Post input', data)
+    )
+    def firestore_post(
+        self, data: AstroColibriPost, image_path: str | None = None
+    ) -> dict[Any, Any]:
+        # Upload image file if provided
+        if image_path is not None:
+            lc_url = self.store_image(image_path)
+            self.logger.info(
+                "AstroClibri image upload", extra={"local": image_path, "url": lc_url}
+            )
+            data["lc_url"] = lc_url
 
         # TODO: not working
-        response = self.session.post(self.colibri_url, json=data)
-                                #, headers=self.csrfheader)
-
-        #request = requests.post(self.colibri_url, json=data, auth=self.session.auth)
-
-        print('Post response ok ', response.ok)
-        print('post response', response.json())
-
+        response = self.session.post(self.api_url + "/add_ampel_transient", json=data)
 
         if response.ok:
-            self.logger.debug('AstroColibriClient submit success', extra={"payload": data})
-            return {'success':True, **response.json()}
+            self.logger.debug(
+                "AstroColibriClient submit success", extra={"payload": data}
+            )
+            return {"success": True, **response.json()}
 
-        self.logger.info('AstroColibriClient submit fail', extra={"payload": classification})
-        return {'success':False, 'response':response.status_code}
+        self.logger.info("AstroColibriClient submit fail", extra={"payload": data})
+        return {"success": False, "response": response.status_code}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/AstroColibriPublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriPublisher.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,263 +6,301 @@
 # Date:                12.11.2022
 # Last Modified Date:  13.11.2022
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
 # FIXME: restore mypy when this is actually ready
 # type: ignore
 
-#from itertools import islice
-from typing import TYPE_CHECKING
-from collections.abc import Generator
-from functools import partial
+# from itertools import islice
+import os
 import re
+from collections.abc import Generator
+
 import numpy as np
 from astropy.time import Time
 
+from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
+from ampel.content.JournalRecord import JournalRecord
+from ampel.contrib.hu.t3.AstroColibriClient import (
+    AstroColibriClient,
+    AstroColibriPhot,
+)
 from ampel.struct.JournalAttributes import JournalAttributes
+from ampel.struct.T3Store import T3Store
 from ampel.view.TransientView import TransientView
-from ampel.view.T3Store import T3Store
-
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
-from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
-from ampel.content.JournalRecord import JournalRecord
-
-from ampel.contrib.hu.t3.AstroColibriClient import AstroColibriClient, AstroColibriPhot, AstroColibriPost
 
 
-
-def dps_to_astrocolobri( dps_det: list[dict] )-> dict[str, AstroColibriPhot]:
+def dps_to_astrocolobri(dps_det: list[dict]) -> dict[str, AstroColibriPhot]:
     """
     From a list of datapoints, construct a dict with the photometry
     information expected by AstroColibri
     {
         'first': {'mag','band','datetime'},
         'peak': {'mag','band','datetime'},
         'last': {'mag','band','datetime'},
     }
 
     """
+
     def convert_dp(dp):
-        bandmap = {1:'ZTFg', 2:'ZTFR', 3:'ZTFi'}
+        bandmap = {1: "ZTFg", 2: "ZTFR", 3: "ZTFi"}
         return {
-                'mag':dp['body']['magpsf'],
-                'band':bandmap[dp['body']['fid']],
-                'datetime': Time(dp['body']['jd'], format='jd').iso
-                }
+            "mag": dp["body"]["magpsf"],
+            "band": bandmap[dp["body"]["fid"]],
+            "datetime": Time(dp["body"]["jd"], format="jd").iso,
+        }
 
     outphot = {}
 
     # Get the first and last
     dps_sort = sorted(dps_det, key=lambda pp: pp["body"]["jd"])
-    outphot['first'] = convert_dp(dps_sort[0])
-    outphot['last'] = convert_dp(dps_sort[-1])
+    outphot["first"] = convert_dp(dps_sort[0])
+    outphot["last"] = convert_dp(dps_sort[-1])
 
     # Get the peak
     dps_sort = sorted(dps_det, key=lambda pp: pp["body"]["magpsf"])
-    outphot['peak'] = convert_dp(dps_sort[0])
+    outphot["peak"] = convert_dp(dps_sort[0])
 
     return outphot
 
 
-
 class AstroColibriPublisher(AbsPhotoT3Unit):
     """
 
     Publish results to AstroColibri. This demo version will:
     - Find the first, brightest and last photometry.
     - Get the position.
     Collect attributes:
     - "Nearby" if AmpelZ<0.02
     - "ProbSNIa" if ParsnipP(SNIa)>0.5
     - "ProbSN" if SNGuess=True at any phase.
+    - Kilonovaness if available.
 
     Will update if new obs was made after last posting.
 
     """
 
     # Limits for attributes
     nearby_z: float = 0.02
     snia_minprob: float = 0.7  # Parsnip class prob to call something SNIa
+    min_kilonovaness: float = 0.0  # Parsnip class prob to call something SNIa
+
+    # Image upload
+    # ZTFNAME will be replaced with the ZTF interpreted stock id
+    image_path: None | str = None
 
     # TODO: What is the use here, when selecting matching journal entries.
     process_name: None | str = None
 
-    # testrun
-    testrun: bool = True
-
-#    user: NamedSecret[str]
-#    password: NamedSecret[str]
-    user: str = 'AMPEL'
-    password: str =  'AMPEL_in_Astro-COLIBRI'
+    # Testcollect (will not try to post)
+    testcollect: bool = False
+    # randname (for repeat submission to dev AstroColibri, not checking TNS)
+    randname: bool = False
+
+    #    user: NamedSecret[str]
+    #    password: NamedSecret[str]
+    user: str = "AMPEL"
+    password: str = "AMPEL_in_Astro-COLIBRI"
 
     def post_init(self) -> None:
-#        self.colibriclient = AstroColibriClient(self.user.get(), self.password.get(), self.logger)
+        #        self.colibriclient = AstroColibriClient(self.user.get(), self.password.get(), self.logger)
         self.colibriclient = AstroColibriClient(self.user, self.password, self.logger)
 
     def _filter_journal_astrocolobri(self, jentry: JournalRecord, after: float):
         """
-            Select journal entries from AstroColibriPublisher newer than last update
-            Does not work when passed as a function to get_journal_entries...
+        Select journal entries from AstroColibriPublisher newer than last update
+        Does not work when passed as a function to get_journal_entries...
         """
         return (
             jentry["unit"] == "AstroColibriPublisher"
             and (self.process_name is None or jentry["process"] == self.process_name)
             and jentry["ts"] >= after
-            and jentry.get("extra") is not None and jentry['extra']['success']
-            and not jentry['extra'].get("testrun", False)
+            and jentry.get("extra") is not None
+            and jentry["extra"]["success"]
+            and not jentry["extra"].get("testcollect", False)
+            and not jentry["extra"].get("randname", True)  # Allow submission of same
             # Possibly add check for whether submit was ok: sucess=True. But see how this looks in journal.
-            #and (jentry.get("extra") is not None and ("descPutComplete" in entry["extra"]) )
-            #and (entry["extra"]["descPutComplete"]) )
-            )
-
+            # and (jentry.get("extra") is not None and ("descPutComplete" in entry["extra"]) )
+            # and (entry["extra"]["descPutComplete"]) )
+        )
 
     def requires_update(self, view: TransientView) -> bool:
         if not view.stock:
             return False
         # find latest activity activity at lower tiers
         latest_activity = max(
             (
                 jentry["ts"]
                 for jentry in view.get_journal_entries() or []
                 if jentry.get("tier") in {0, 1, 2}
             ),
             default=float("inf"),
         )
         # Manual
-        t3journals = [je for je in
-                view.get_journal_entries(tier=3)
-                if self._filter_journal_astrocolobri(je, latest_activity) ]
+        t3journals = [
+            je
+            for je in view.get_journal_entries(tier=3)
+            if self._filter_journal_astrocolobri(je, latest_activity)
+        ]
         return bool(t3journals)
 
-
     def submitted(self, view: "TransientView") -> bool:
         # Was transient (successfully pushed)
         if not view.stock:
             return False
-        return bool( [je for je in
-                view.get_journal_entries(tier=3)
-                if self._filter_journal_astrocolobri(je, 0) ] )
+        return bool(
+            [
+                je
+                for je in view.get_journal_entries(tier=3)
+                if self._filter_journal_astrocolobri(je, 0)
+            ]
+        )
 
     def get_tnsname(self, view: "TransientView") -> bool:
         # Was transient (successfully pushed)
         if not view.stock:
             return False
         # Check whether the name is found in the name collection
-        if len( (names:=view.stock.get('name',[]) ) )>0:
+        if len(names := view.stock.get("name", [])) > 0:
             # Will only be able to require TNS name through format
             # dddd
             for name in names:
-                if re.search(r'\d{4}\D{3}\D?', name):
+                if re.search(r"\d{4}\D{3}\D?", name):
                     return name
 
         # Should we look through the Journal for entries from the TNSTalker?
         # It *should* also save these entries to name so should not be needed...
 
         return None
 
-
-
-    def process(self,
+    def process(
+        self,
         tviews: Generator[TransientView, JournalAttributes, None],
-        t3s: 'None | T3Store' = None
+        t3s: "None | T3Store" = None,
     ) -> None:
         """
         Iterate through TransientView and check which should be
         submitted / updated.
         """
-        print('starting')
 
         for tview in tviews:
+            if self.randname:
+                import random
 
-            # Find TNS name (required for AstroColibri posting)
-            # Currently assumes that this is stored either in the
-            # stock name list or can be found in the T3 journal
-            # (probably from the TNSTalker)
-            tns_name = self.get_tnsname(tview)
-            if not tns_name:
-                self.logger.info('No TNS.',extra={'tnsName':None})
-                continue
+                # Generate random name (assuming publishing to dev AC)
+                tns_name = f"AmpelRand{random.randint(1, 999)}"
+            else:
+                # Find TNS name (required for AstroColibri posting)
+                # Currently assumes that this is stored either in the
+                # stock name list or can be found in the T3 journal
+                # (probably from the TNSTalker)
+                tns_name = self.get_tnsname(tview)
+                if not tns_name:
+                    self.logger.info("No TNS.", extra={"tnsName": None})
+                    continue
 
             # Check if this was submitted
             # TODO: How should the first submit differ from updates?
             if self.submitted(tview):
                 # Check if it needs an update
                 if self.requires_update(tview):
                     post_update = True
                 else:
                     continue
             else:
                 post_update = False
 
-
             # Gather general information
             payload = {
-                'type': 'ot_sn',      # for optical? when to change to ot_sn?
-                'observatory': 'ztf',
-                'source_name': to_ztf_id(int(tview.id)),
-#                'trigger_id': self.trigger_id+':'+str(tview.id),  # How do these work?
-                'trigger_id': 'TNS'+tns_name,
-#                'ivorn': self.trigger_id+':'+str(tview.id),       # Need ivorn schema
-                'timestamp': Time.now().iso
+                "type": "ot_sn",  # for optical? when to change to ot_sn?
+                "observatory": "ztf",
+                "source_name": to_ztf_id(int(tview.id)),
+                #                'trigger_id': self.trigger_id+':'+str(tview.id),  # How do these work?
+                "trigger_id": "TNS" + tns_name,
+                #                'ivorn': self.trigger_id+':'+str(tview.id),       # Need ivorn schema
+                "timestamp": Time.now().iso,
             }
 
-
             # Gather photometry based information
             assert tview.t0 is not None
             # Get subset of real detections.
             # Could be complemented with further restrictions, e.g. filter / RB
-            dps_det = [pp for pp in tview.t0 if (pp['id']>0 and pp['body'].get('isdiffpos',False) )  ]
-            payload['photometry'] = dps_to_astrocolobri( dps_det  )
-            payload['ra'] = np.mean( [pp['body']['ra'] for pp in dps_det] )
-            payload['dec'] = np.mean( [pp['body']['dec'] for pp in dps_det] )
-            payload['err'] = 1. / 3600  # position err ~1 arcsec in dec
-
+            dps_det = [
+                pp
+                for pp in tview.t0
+                if (pp["id"] > 0 and pp["body"].get("isdiffpos", False))
+            ]
+            payload["photometry"] = dps_to_astrocolobri(dps_det)
+            payload["ra"] = np.mean([pp["body"]["ra"] for pp in dps_det])
+            payload["dec"] = np.mean([pp["body"]["dec"] for pp in dps_det])
+            payload["err"] = 1.0 / 3600  # position err ~1 arcsec in dec
+
+            # If part of random testing, perturb coordinates
+            if self.randname:
+                payload["ra"] += random.randrange(-1, 1)
+                payload["dec"] += random.randrange(-1, 1)
+                payload["source_name"] += payload["trigger_id"][12:]
 
             # Gather attributes
             attributes = []
             # Nearby attribute
             t2res = tview.get_t2_body(unit="T2DigestRedshifts")
-            if isinstance(t2res, dict) and t2res['ampel_z']<self.nearby_z:
-                attributes.append('Nearby')
+            if isinstance(t2res, dict) and t2res.get("ampel_z", 999) < self.nearby_z:
+                attributes.append("Nearby")
+                attributes.append("AmpelZ{:.2f}".format(t2res["ampel_z"]))
             # Infant attribute
             t2res = tview.get_t2_body(unit="T2InfantCatalogEval")
-            if isinstance(t2res, dict) and t2res['action']:
-                attributes.append('Young')
+            if isinstance(t2res, dict) and t2res.get("action", False):
+                attributes.append("Young")
             # SNIa
             t2res = tview.get_t2_body(unit="T2RunParsnip")
-            if isinstance(t2res, dict) and 'classification' in t2res.keys():
-                if t2res['classification']['SNIa'] > self.snia_minprob:
-                    attributes.append('ProbSNIa')
-            attributes.append('AnExtraAttribute')
+            if (
+                isinstance(t2res, dict)
+                and "classification" in t2res
+                and t2res["classification"]["SNIa"] > self.snia_minprob
+            ):
+                attributes.append("ProbSNIa")
+            # Kilonovaness
+            t2res = tview.get_t2_body(unit="T2KilonovaEval")
+            if (
+                isinstance(t2res, dict)
+                and t2res.get("kilonovaness", -99) > self.min_kilonovaness
+            ):
+                attributes.append("Kilonovaness{}".format(t2res["kilonovaness"]))
+                attributes.append("LVKmap{}".format(t2res["map_name"]))
+
+            # Check whether we have a figure to upload.
+            # Assuming this exists locally under {stock}.png
+            if self.image_path is not None:
+                ipath = self.image_path.replace("ZTFNAME", to_ztf_id(int(tview.id)))
+                # Only upload if it actually exists:
+                if not os.path.isfile(ipath):
+                    ipath = None
+            else:
+                ipath = None
+
             payload["ampel_attributes"] = attributes
-            payload["ampel_attributes"] = ['Nearby','AThirdAttribute']
-            print('payload', payload)
             self.logger.debug("reacting", extra={"payload": payload})
 
             # Ok, so we have a transient to react to
-            if self.testrun:
+            if self.testcollect:
                 if post_update:
-                    print('Should send an update')
+                    print("Should send an update")
                 else:
-                    print('New submission')
-                print('*** Posting ***')
+                    print("New submission")
+                print("*** Posting ***")
                 print(payload)
-                print('*** Done ***')
+                print("*** Done ***")
 
                 # Journal submission
-                jcontent = {"reaction": "fake submission", "success": True, "testrun": True}
+                jcontent = {
+                    "reaction": "fake submission",
+                    "success": True,
+                    "testcollect": True,
+                }
 
             else:
-
-                print('DEBUG POSTING')
-                print('send', payload)
-                jcontent = self.colibriclient.firestore_post(payload)
-
-                print('got', jcontent)
-
+                jcontent = self.colibriclient.firestore_post(payload, image_path=ipath)
 
             if jcontent:
                 tviews.send(JournalAttributes(extra=jcontent))
-
-            break
-
-        return None
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ChannelSummaryPublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ChannelSummaryPublisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                13.11.2018
 # Last Modified Date:  16.12.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
-import datetime, backoff, requests
+import datetime
+from collections.abc import Generator
 from io import BytesIO, StringIO
+from typing import Any
+
+import backoff
+import requests
 from astropy.time import Time
 from pytz import timezone
 from requests.auth import HTTPBasicAuth
-from typing import Any
-from collections.abc import Generator
 
-from ampel.types import ChannelId, UBson, T3Send
-from ampel.view.T3Store import T3Store
+from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.secret.NamedSecret import NamedSecret
+from ampel.struct.T3Store import T3Store
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import ChannelId, T3Send, UBson
 from ampel.util.json import AmpelEncoder, load
 from ampel.view.TransientView import TransientView
-from ampel.struct.UnitResult import UnitResult
-from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 
 
 class ChannelSummaryPublisher(AbsPhotoT3Unit):
     """
     Create a json file with summary statistics for the channel. For the transients
     detected in the last N days, this json file contains, i.e. coords, RB score,
     first detection, latest detection, and the total number of transients detected
@@ -33,24 +36,21 @@
     T2LightCurveSummary.
     """
 
     dry_run: bool = False
     base_url: str = "https://desycloud.desy.de/remote.php/webdav/AMPEL/ZTF"
     auth: NamedSecret[list] = NamedSecret(label="desycloud/valery")
 
-
     def post_init(self) -> None:
-
         self.summary: dict[str, Any] = {}
         self._jd_range = [float("inf"), -float("inf")]
         self._channels: set[ChannelId] = set()
         self.session = requests.Session()
         self.session.auth = HTTPBasicAuth(*self.auth.get())
 
-
     def extract_from_transient_view(
         self, tran_view: TransientView
     ) -> None | dict[str, Any]:
         """
         given transient view object return a dictionary
         with the desired metrics
         """
@@ -76,16 +76,17 @@
             if last_detection < self._jd_range[0]:
                 self._jd_range[0] = last_detection
             if last_detection > self._jd_range[1]:
                 self._jd_range[1] = last_detection
 
         return out
 
-
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None) -> UBson | UnitResult:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None
+    ) -> UBson | UnitResult:
         """
         load the stats from the alerts
         """
         for tran_view in gen:
             assert tran_view.stock
             if len(channels := tran_view.stock.get("channel") or []) != 1:
                 raise ValueError("Only single-channel views are supported")
@@ -95,40 +96,39 @@
             key = info_dict.pop("ztf_name")
             self.summary[key] = info_dict
             self._channels.add(channels[0])
 
         self.done()
         return None
 
-
     @backoff.on_exception(
         backoff.expo,
         (TimeoutError, requests.exceptions.HTTPError),
-        giveup=lambda exc: isinstance(exc, requests.exceptions.HTTPError) and
-        exc.response.status_code not in {400, 403, 405, 423, 500}
+        giveup=lambda exc: isinstance(exc, requests.exceptions.HTTPError)
+        and exc.response.status_code not in {400, 403, 405, 423, 500},
     )
     def done(self) -> None:
         """"""
         if len(self._channels) == 0:
             return
-        elif len(self._channels) > 1:
+        if len(self._channels) > 1:
             raise ValueError(
                 f"Got multiple channels ({list(self._channels)}) in summary"
             )
 
         # Find the date of the most recent observation, in Pacific time
         timestamp = Time(self._jd_range[-1], format="jd").to_datetime(
             timezone("US/Pacific")
         )
         # If before noon, it belongs to the night that started yesterday
         if timestamp.hour < 12:
             timestamp -= datetime.timedelta(days=1)
         filename = timestamp.strftime("channel-summary-%Y%m%d.json")
 
-        channel = list(self._channels)[0]
+        channel = next(iter(self._channels))
         basedir = f"{self.base_url}/{channel}"
         rep = self.session.head(basedir)
         if not (rep.ok or self.dry_run):
             self.session.request("MKCOL", basedir).raise_for_status()
         try:
             rep = self.session.get(f"{basedir}/{filename}")
             rep.raise_for_status()
@@ -137,15 +137,13 @@
             self.summary = partial_summary
         except (requests.exceptions.HTTPError, StopIteration):
             pass
 
         outfile = StringIO()
         outfile.write(AmpelEncoder(lossy=True).encode(self.summary))
         outfile.write("\n")
-        mb = len(outfile.getvalue().encode()) / 2.0 ** 20
-        self.logger.info(
-            "{}: {} transients {:.1f} MB".format(filename, len(self.summary), mb)
-        )
+        mb = len(outfile.getvalue().encode()) / 2.0**20
+        self.logger.info(f"{filename}: {len(self.summary)} transients {mb:.1f} MB")
         if not self.dry_run:
             self.session.put(
-                "{}/{}".format(basedir, filename), data=outfile.getvalue()
+                f"{basedir}/{filename}", data=outfile.getvalue()
             ).raise_for_status()
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/DCachePublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/DCachePublisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,48 @@
 # License:             BSD-3-Clause
 # Author:              Jakob van Santen <jakob.van.santen@desy.de>
 # Date:                27.02.2020
 # Last Modified Date:  27.02.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 
-import asyncio, datetime, gzip, io, os, ssl, sys, time, traceback, backoff, pytz
+import asyncio
+import datetime
+import gzip
+import io
+import os
+import ssl
+import sys
+import time
+import traceback
+from collections.abc import Generator
 from functools import partial
 from typing import Any
-from collections.abc import Generator
 from xml.etree import ElementTree
-from aiohttp import ClientSession, helpers, TCPConnector
+
+import backoff
+import pytz
+from aiohttp import ClientSession, TCPConnector, helpers
 from aiohttp.client_exceptions import (
-    ClientConnectionError, ClientConnectorError, ClientConnectorSSLError,
-    ClientResponseError, ServerDisconnectedError
+    ClientConnectionError,
+    ClientConnectorError,
+    ClientConnectorSSLError,
+    ClientResponseError,
+    ServerDisconnectedError,
 )
 
-from ampel.types import UBson
-from ampel.view.T3Store import T3Store
 from ampel.abstract.AbsT3ReviewUnit import AbsT3ReviewUnit
 from ampel.secret.NamedSecret import NamedSecret
+from ampel.struct.JournalAttributes import JournalAttributes
+from ampel.struct.T3Store import T3Store
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import UBson
 from ampel.util.json import AmpelEncoder
 from ampel.view.SnapView import SnapView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
-from ampel.struct.UnitResult import UnitResult
-from ampel.struct.JournalAttributes import JournalAttributes
 
 
 class DCachePublisher(AbsT3ReviewUnit):
     """
     Publish TransientViews to DCache in gzipped JSON format
 
     Each run writes a manifest file to {baseDir}/{channel}/manifest/latest.json.gz
@@ -66,22 +80,20 @@
         self.dt = 0.0
 
         # don't bother preserving immutable types
         self.encoder = AmpelEncoder(lossy=True)
         assert self.resource
         self.base_dest = self.resource["dcache"] + self.base_dir
 
-
     def serialize(self, tran_view: SnapView | dict[str, Any]) -> bytes:
         buf = io.BytesIO()
         with gzip.GzipFile(fileobj=buf, mode="w") as f:
             f.write(self.encoder.encode(tran_view).encode("utf-8"))
         return buf.getvalue()
 
-
     async def create_directory(self, request, path_parts) -> None:
         path = []
         while len(path_parts) > 0:
             # NB: os.path.join drops any parts before those that start with /
             path.append(path_parts.pop(0).lstrip("/"))
             if tuple(path) in self.existing_paths:
                 continue
@@ -91,135 +103,128 @@
                 if not await self.exists(request, url):
                     resp = await request("MKCOL", url, raise_for_status=False)
                     # MKCOL on an existing directory returns 'Method not allowed'
                     if not (resp.status < 400 or resp.status == 405):
                         resp.raise_for_status()
             self.existing_paths.add(tuple(path))
 
-
     async def put(self, request, url, data, timeout=1.0):
         if self.dry_run:
             return
         await request("PUT", url, data=data)
 
-
     async def exists(self, request, url):
         if self.dry_run:
-            return
+            return None
         resp = await request("HEAD", url, raise_for_status=False)
         return resp.status in {200, 201, 204}
 
-
     @staticmethod
     def is_permanent_error(exc):
         if isinstance(exc, ClientResponseError):
             return exc.code not in {403, 423, 500}
-        elif isinstance(exc, ClientConnectorSSLError):
+        if isinstance(exc, ClientConnectorSSLError):
             return True
-        else:
-            return False
-
+        return False
 
     def _on_backoff(self, details):
         exc_typ, exc, _ = sys.exc_info()
-        if exc is not None:
-            exc = traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+        err = (
+            traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+            if exc
+            else None
+        )
         self.logger.warn(
             "backoff",
             extra={
-                "exc": exc,
+                "exc": err,
                 "target_args": details["args"],
                 "wait": details["wait"],
                 "tries": details["tries"],
             },
         )
 
-
     def _on_giveup(self, details):
         exc_typ, exc, _ = sys.exc_info()
-        if exc is not None:
-            exc = traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+        err = (
+            traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+            if exc
+            else None
+        )
         self.logger.warn(
             "gave up",
             extra={
-                "exc": exc,
+                "exc": err,
                 "target_args": details["args"],
                 "tries": details["tries"],
             },
         )
 
-
     async def publish_transient(self, request, tran_view: SnapView) -> str:
-
         assert isinstance(tran_view.id, int)
         ztf_name = to_ztf_id(tran_view.id)
         # group such that there are a maximum of 17576 in the same directory
         prefix = [ztf_name[:7], ztf_name[7:9]]
 
         await self.create_directory(request, [self.channel, *prefix])
         base_dir = os.path.join(self.base_dest, self.channel, *prefix)
         fname = base_dir + f"/{ztf_name}.json.gz"
         await self.put(request, fname, data=self.serialize(tran_view))
 
         return fname
 
-
     async def send_requests(self, unbound_tasks):
         """
         Send a batch of requests
 
         :param unbound_tasks: sequence of callables that take a single argument
             that is an aiohttp request object
         """
         ssl_context = ssl.create_default_context(
             capath=os.environ.get("X509_CERT_DIR", None)
         )
         async with TCPConnector(
             limit=self.max_parallel_requests, ssl_context=ssl_context
-        ) as connector:
-            async with ClientSession(
-                connector=connector,
-                headers={"Authorization": f"BEARER {self.authz.get()}"},
-                raise_for_status=True,
-            ) as session:
-                if self.dry_run:
-                    session = None
-                else:
-                    # ClientSession.request is a normal function returning an
-                    # async context manager. While this is kind of equivalent
-                    # to a coroutine, it can't be decorated with backoff. Wrap
-                    # it so it can be.
-                    # Note that it is important to not actually enter the
-                    # context manager here, as this would close the response
-                    # on exit, causing read() to raise ClientConnectionError.
-                    async def async_request(*args, **kwargs):
-                        return await session.request(*args, **kwargs)
-
-                    # robustify Session.request() against transitory failures
-                    request = backoff.on_exception(
-                        backoff.expo,
-                        (
-                            asyncio.TimeoutError,
-                            ClientResponseError,
-                            ClientConnectorError,
-                            ClientConnectionError,
-                            ServerDisconnectedError,
-                        ),
-                        logger=None,
-                        giveup=self.is_permanent_error,
-                        on_giveup=self._on_giveup,
-                        on_backoff=self._on_backoff,
-                    )(async_request)
-
-                tasks = [task(request) for task in unbound_tasks]
-                return await asyncio.gather(*tasks)
-
-
-    def process(self, gen: Generator[SnapView, JournalAttributes, None], t3s: T3Store) -> UBson | UnitResult:
-
+        ) as connector, ClientSession(
+            connector=connector,
+            headers={"Authorization": f"BEARER {self.authz.get()}"},
+            raise_for_status=True,
+        ) as session:
+            # ClientSession.request is a normal function returning an
+            # async context manager. While this is kind of equivalent
+            # to a coroutine, it can't be decorated with backoff. Wrap
+            # it so it can be.
+            # Note that it is important to not actually enter the
+            # context manager here, as this would close the response
+            # on exit, causing read() to raise ClientConnectionError.
+            async def async_request(*args, **kwargs):
+                return await session.request(*args, **kwargs)
+
+            # robustify Session.request() against transitory failures
+            request = backoff.on_exception(
+                backoff.expo,
+                (
+                    asyncio.TimeoutError,
+                    ClientResponseError,
+                    ClientConnectorError,
+                    ClientConnectionError,
+                    ServerDisconnectedError,
+                ),
+                logger=None,
+                giveup=self.is_permanent_error,
+                on_giveup=self._on_giveup,
+                on_backoff=self._on_backoff,
+            )(async_request)
+
+            tasks = [task(request) for task in unbound_tasks]
+            return await asyncio.gather(*tasks)
+
+    def process(
+        self, gen: Generator[SnapView, JournalAttributes, None], t3s: T3Store
+    ) -> UBson | UnitResult:
         """
         Publish a transient batch
         """
         loop = asyncio.get_event_loop()
         t0 = time.time()
         self.updated_urls += loop.run_until_complete(
             self.send_requests(
@@ -238,46 +243,50 @@
         if not self.dry_run:
             asyncio.get_event_loop().run_until_complete(
                 self.send_requests([self.publish_manifest])
             )
 
         return None
 
-
     async def publish_manifest(self, request) -> None:
         prefix = os.path.join(self.base_dest, self.channel)
         manifest_dir = os.path.join(prefix, "manifest")
         # create any directories that descend from the base path
         await self.create_directory(
             request,
             list(
                 os.path.split(
-                    prefix[len(os.path.commonprefix((self.base_dest, manifest_dir))):]
+                    prefix[len(os.path.commonprefix((self.base_dest, manifest_dir))) :]
                 )
             ),
         )
 
         latest = os.path.join(manifest_dir, "latest.json.gz")
         previous = None
 
         # Move the previous manifest aside.
         async with await request(
             "PROPFIND", latest, raise_for_status=False
         ) as response:
-            if response.status < 400 and (
-                element := ElementTree.fromstring(await response.text()).find(
-                    "**/{DAV:}prop/{DAV:}creationdate"
+            if (
+                response.status < 400
+                and (
+                    element := ElementTree.fromstring(await response.text()).find(
+                        "**/{DAV:}prop/{DAV:}creationdate"
+                    )
                 )
+                and (date := element.text)
             ):
-                if date := element.text:
-                    previous = os.path.join(manifest_dir, date + ".json.gz")
-                    self.logger.info(f"Moving {latest} to {previous}")
-                    await request(
-                        "MOVE", latest, headers={"Destination": previous},
-                    )
+                previous = os.path.join(manifest_dir, date + ".json.gz")
+                self.logger.info(f"Moving {latest} to {previous}")
+                await request(
+                    "MOVE",
+                    latest,
+                    headers={"Destination": previous},
+                )
 
         # Write a new manifest with a link to previous manifest.
         await request(
             "PUT",
             latest,
             data=self.serialize(
                 {
@@ -296,25 +305,27 @@
             json={
                 "caveats": ["activity:DOWNLOAD,LIST,READ_METADATA"],
                 "validity": "PT48h",
             },
         ) as response:
             authz = await response.json()
         await request(
-            "PUT", os.path.join(prefix, "macaroon"), data=authz["macaroon"],
+            "PUT",
+            os.path.join(prefix, "macaroon"),
+            data=authz["macaroon"],
         )
         self.logger.info(f"Access token: {authz}")
 
 
 def get_macaroon(
     user: helpers.BasicAuth,
     path: str,
     validity: str,
-    activity: list[str] = [],
-    ip: list[str] = [],
+    activity: None | list[str] = None,
+    ip: None | list[str] = None,
     host: str = "globe-door.ifh.de",
     port: int = 2880,
 ):
     """
     Request a DCache macaroon
     """
     caveats = []
@@ -326,22 +337,23 @@
     if caveats:
         body["caveats"] = caveats
 
     async def fetch():
         ssl_context = ssl.create_default_context(
             capath=os.environ.get("X509_CERT_DIR", None)
         )
-        async with TCPConnector(ssl_context=ssl_context) as connector:
-            async with ClientSession(auth=user, connector=connector) as session:
-                resp = await session.post(
-                    f"https://{host}:{port}{path}",
-                    headers={"Content-Type": "application/macaroon-request"},
-                    json=body,
-                )
-                return (await resp.json())["macaroon"]
+        async with TCPConnector(ssl_context=ssl_context) as connector, ClientSession(
+            auth=user, connector=connector
+        ) as session:
+            resp = await session.post(
+                f"https://{host}:{port}{path}",
+                headers={"Content-Type": "application/macaroon-request"},
+                json=body,
+            )
+            return (await resp.json())["macaroon"]
 
     return asyncio.get_event_loop().run_until_complete(fetch())
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ElasticcClassPublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcClassPublisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 # File:                ampel/contrib/hu/t3/ElasticcClassPublisher.py
 # License:             BSD-3-Clause
 # Author:              jno <jnordin@physik.hu-berlin.de>
 # Date:                11.04.2022
 # Last Modified Date:  11.04.2022
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
+from collections.abc import Generator, Iterable
 from itertools import islice
-from typing import Iterable, TYPE_CHECKING
-from collections.abc import Generator
+from typing import TYPE_CHECKING, TypeVar
 
-from ampel.struct.StockAttributes import StockAttributes
-from ampel.struct.JournalAttributes import JournalAttributes
-from ampel.enum.DocumentCode import DocumentCode
 from ampel.abstract.AbsT3ReviewUnit import AbsT3ReviewUnit, T3Send
+from ampel.contrib.hu.t3.ElasticcTomClient import ElasticcTomClient
+from ampel.enum.DocumentCode import DocumentCode
+from ampel.log import LogFlag
 from ampel.secret.NamedSecret import NamedSecret
+from ampel.struct.JournalAttributes import JournalAttributes
+from ampel.struct.StockAttributes import StockAttributes
+from ampel.struct.T3Store import T3Store
 from ampel.view.TransientView import TransientView
-from ampel.view.T2DocView import T2DocView
-from ampel.view.T3Store import T3Store
-
-from ampel.contrib.hu.t3.ElasticcTomClient import ElasticcTomClient
 
 if TYPE_CHECKING:
     from ampel.content.JournalRecord import JournalRecord
 
-def chunks(l: Iterable, n: int) -> Generator[list, None, None]:
+T = TypeVar("T")
+
+
+def chunks(l: Iterable[T], n: int) -> Generator[list[T], None, None]:
     source = iter(l)
     while True:
         chunk = list(islice(source, n))
         if chunk:
             yield chunk
         if len(chunk) < n:
             break
 
+
 class ElasticcClassPublisher(AbsT3ReviewUnit):
     """
 
     This unit is intended to submit classifications to the DESC TOM db during
     the ELAsTICC LSST alert simulation.
 
     This will have to proceed through the following stages for each stock:
@@ -56,33 +59,35 @@
     (like submitting the rest after some time?)
 
     Note: still not sure whether we need to track also the diaSourceId and
     issue timestamp.
 
     """
 
-    broker_name: str = 'AMPEL'
-    broker_version: str = 'v0.1'
+    broker_name: str = "AMPEL"
+    broker_version: str = "v0.1"
     tom_url: str = "https://desc-tom.lbl.gov"
     desc_user: NamedSecret[str]
     desc_password: NamedSecret[str]
 
     #: prepare report, but do not submit to TOM
     dry_run: bool = False
     #: submit reports in batches
     batch_size: int = 1000
+    #: raise an exception on submission failure
+    raise_exc: bool = True
 
     unit: str = "T2ElasticcReport"
 
     def post_init(self) -> None:
-        self.tomclient = ElasticcTomClient(self.desc_user.get(), self.desc_password.get(), self.logger, self.tom_url)
+        self.tomclient = ElasticcTomClient(
+            self.desc_user.get(), self.desc_password.get(), self.logger, self.tom_url
+        )
 
-    def search_journal_elasticc(
-        self, tran_view: TransientView
-    ) -> dict[int,bool]:
+    def search_journal_elasticc(self, tran_view: TransientView) -> dict[int, bool]:
         """
         Look through the journal for mapping between alert ID, timestampe and state id.
 
         Assuming journal entries from this unit has the following layout
         extra = {
             "t1State": t1_link,
             "descPutResponse": response,
@@ -97,113 +102,173 @@
          ...}
 
         """
 
         # Create a list of states for which the list of units
         def select_submitted(entry: "JournalRecord") -> bool:
             return bool(
-                (entry.get("extra") is not None and ("descPutComplete" in entry["extra"])
-                and (entry["extra"]["descPutComplete"]) )
-                and (entry["extra"]["descPutUnit"]==self.unit)
-                and entry["unit"] and entry["unit"] == self.__class__.__name__
+                (
+                    entry.get("extra") is not None
+                    and ("descPutComplete" in entry["extra"])
+                    and (entry["extra"]["descPutComplete"])
+                )
+                and (entry["extra"]["descPutUnit"] == self.unit)
+                and entry["unit"]
+                and entry["unit"] == self.__class__.__name__
             )
 
         done_t1states = set()
 
         # All entries which we found should correspond to correctly sumitted classifications
-        if jentries := list(tran_view.get_journal_entries(tier=3, filter_func=select_submitted)):
+        if jentries := list(
+            tran_view.get_journal_entries(tier=3, filter_func=select_submitted)
+        ):
             for entry in jentries:
-                done_t1states.add( entry['extra']['t1State'])
+                done_t1states.add(entry["extra"]["t1State"])
 
         # Next section would look through the journal and find the elasticc alert
         # data needed. Here we are doing some short version of it
         # Perform another journal search and check whether this unit was run
         # for this state
         state_map = {}
+
         def select_alerts(entry: "JournalRecord") -> bool:
             return bool(
                 entry.get("alert") is not None and entry.get("link") is not None
             )
-        if jentries := list(tran_view.get_journal_entries(tier=0, filter_func=select_alerts)):
+
+        if jentries := list(
+            tran_view.get_journal_entries(tier=0, filter_func=select_alerts)
+        ):
             for entry in jentries:
                 assert isinstance(link := entry.get("link"), int)
                 if link in done_t1states:
                     state_map[link] = True
                 else:
-                    state_map[link]= False
+                    state_map[link] = False
         return state_map
 
-    def _get_reports(self, gen: Generator[TransientView, T3Send, None]) -> Generator[tuple[TransientView,int,dict],None,None]:
+    def _get_reports(
+        self, gen: Generator[TransientView, T3Send, None]
+    ) -> Generator[tuple[TransientView, int, dict], None, None]:
+        stats = {
+            "stocks": 0,
+            "views": 0,
+            "pending": 0,
+            "submitted": 0,
+        }
 
         for tran_view in gen:
             # Check journal for state/alertId combos and whether already
             # submitted (for this t2classifiers list).
             state_alert = self.search_journal_elasticc(tran_view)
 
+            stats["stocks"] += 1
+
             for t1_link, submitted in state_alert.items():
+                stats["views"] += 1
                 if submitted:
-                    self.logger.debug('submitted', extra={'t1':t1_link})
+                    self.logger.debug("submitted", extra={"t1": t1_link})
+                    stats["submitted"] += 1
                     continue
-                if t2views := tran_view.get_t2_views(unit=self.unit, link=t1_link, code=DocumentCode.OK):
+                if t2views := tran_view.get_t2_views(
+                    unit=self.unit, link=t1_link, code=DocumentCode.OK
+                ):
                     t2view = next(t2views, None)
                     if t2view is None:
-                        self.logger.info('No T2Doc found', extra={'unit':self.unit})
-                        continue   # No T2 ticket found
+                        self.logger.debug("No T2Doc found", extra={"unit": self.unit})
+                        stats["pending"] += 1
+                        continue  # No T2 ticket found
                     # Only reason there could be multiple views here is if we
                     # are running different configs... if so this unit wont work
                     # and needs to be redesigned!
-                    if next(t2views, None) is not None:
-                        raise RuntimeError('ElasticcClassPublisher cannot parse multiple configs.')
+                    if (
+                        t2_view_extra := next(t2views, None)
+                    ) is not None and t2_view_extra.config != t2view.config:
+                        raise RuntimeError(
+                            "ElasticcClassPublisher cannot parse multiple configs. "
+                            f"Got configs={t2view.config},{t2_view_extra.config} for "
+                            f"stock:{t2view.stock},link:{t2view.link},unit:{t2view.unit}"  # type: ignore[str-bytes-safe]
+                        )
                     if not isinstance((body := t2view.get_payload()), dict):
                         continue
                     yield tran_view, t1_link, body["report"]
+        self.logger.log(LogFlag.SHOUT, "filtered states", extra=stats)
 
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: T3Store) -> None:
-        """
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: T3Store
+    ) -> None:
+        """ """
 
-        """
+        submitted = 0
+        failed = 0
 
         for chunk in chunks(self._get_reports(gen), self.batch_size):
-            tran_views, t1_links, class_reports = zip(*chunk)
+            tran_views: tuple[TransientView, ...]
+            t1_links: tuple[int, ...]
+            class_reports: tuple[dict, ...]
+            tran_views, t1_links, class_reports = zip(*chunk, strict=False)
 
             if self.dry_run:
                 continue
 
             # use the ElasticcTomClient
-            desc_response = self.tomclient.tom_post(class_reports)
+            desc_response = self.tomclient.tom_post(class_reports)  # type: ignore[arg-type]
+
+            if desc_response["success"]:
+                submitted += len(class_reports)
+            else:
+                failed += len(class_reports)
+                body = desc_response.pop("response_body")
+                self.logger.error(
+                    "desc post failed",
+                    extra={
+                        "descResponse": desc_response,
+                        "descReport": class_reports[0],
+                    },
+                )
+                if self.raise_exc:
+                    raise RuntimeError(f"Post failed: {body}")
 
             # Check output:
             # if as expected store to journal that transfer is complete.
             # if not as expected, log what data is available and possible
             # a t3 document with this content??
-            for tran_view, t1_link, class_report in zip(tran_views, t1_links, class_reports):
-                if desc_response['success']:
-                    gen.send((
-                        tran_view.id,
-                        StockAttributes(
-                            journal=JournalAttributes(
-                                extra={
-                                    "t1State": t1_link,
-                                    "descPutResponse": desc_response,
-                                    "descPutComplete": True,
-                                    "descPutUnit": self.unit,
+            for tran_view, t1_link, _ in zip(
+                tran_views, t1_links, class_reports, strict=False
+            ):
+                if desc_response["success"]:
+                    gen.send(
+                        (
+                            tran_view.id,
+                            StockAttributes(
+                                journal=JournalAttributes(
+                                    extra={
+                                        "t1State": t1_link,
+                                        "descPutResponse": desc_response,
+                                        "descPutComplete": True,
+                                        "descPutUnit": self.unit,
                                     },
-                                    ),
-                                    )
-                                ))
+                                ),
+                            ),
+                        )
+                    )
                 else:
-                    gen.send((
-                        tran_view.id,
-                        StockAttributes(
-                            journal=JournalAttributes(
-                                extra={
-                                    "t1State": t1_link,
-                                    "descPutResponse": desc_response,
-                                    "descPutComplete": False,
-                                    "descPutUnits": self.unit,
+                    gen.send(
+                        (
+                            tran_view.id,
+                            StockAttributes(
+                                journal=JournalAttributes(
+                                    extra={
+                                        "t1State": t1_link,
+                                        "descPutResponse": desc_response,
+                                        "descPutComplete": False,
+                                        "descPutUnits": self.unit,
                                     },
-                                    ),
-                                    )
-                                ))
-                    self.logger.info('desc post failed', extra={
-                        "descResponse":desc_response,
-                        "descReport": class_report, })
+                                ),
+                            ),
+                        )
+                    )
+
+        self.logger.log(
+            LogFlag.SHOUT, "reported", extra={"submitted": submitted, "failed": failed}
+        )
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ElasticcTomClient.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcTomClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 # File:                ampel/contrib/hu/t3/ElasticcTomClient.py
 # License:             BSD-3-Clause
 # Author:              jno <jnordin@physik.hu-berlin.de>
 # Date:                11.04.2022
 # Last Modified Date:  11.04.2022
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
-from typing import Sequence, Dict, Any, Union
+from collections.abc import Sequence
+from typing import Any
 
-import requests
-import json
 import backoff
+import requests
 from requests import HTTPError
 
 
-class ClassificationDict():
+class ClassificationDict:
     classifierName: str
     classifierParams: str
     classId: int
     probability: float
 
-class ElasticcClassification():
+
+class ElasticcClassification:
     alertId: int
     diaSourceId: int
     elasticcPublishTimestamp: int
     brokerIngestTimestamp: int
     brokerName: str
     brokerVersion: str
     classifications: Sequence[ClassificationDict]
@@ -41,55 +42,79 @@
 
     A successful put returns a 'dbMessageIndex' value.
 
     todo: do we need to robustify also the step where the session is created?
     (is the session best started in a post_init()?)
 
     """
-    def __init__(self, desc_username: str, desc_password: str, logger, tom_url: str = "https://desc-tom.lbl.gov"):
+
+    def __init__(
+        self,
+        desc_username: str,
+        desc_password: str,
+        logger,
+        tom_url: str = "https://desc-tom.lbl.gov",
+    ):
         self.logger = logger
 
         # Debug url
-#        self.tom_url = "https://desc-tom-rknop-dev.lbl.gov"
+        #        self.tom_url = "https://desc-tom-rknop-dev.lbl.gov"
         # Production
         # self.tom_url = "https://desc-tom.lbl.gov"
         self.tom_url = tom_url
 
         # Setup django connection. From Rob Knop:
         # There's a bit of a dance to log in since django
         # requires a csrftoken not only in its headers, but
         # also in the POST data to log in; do a quick GET
         # to the login URI to get that token.  (There must
         # be a cleaner way.)
         self.session = requests.session()
-        self.session.get( f'{self.tom_url}/accounts/login/' )
-        self.session.post( f'{self.tom_url}/accounts/login/',
-              data={ "username": desc_username,
-                     "password": desc_password,
-                     "csrfmiddlewaretoken": self.session.cookies['csrftoken'] } )
-        self.csrfheader = { 'X-CSRFToken': self.session.cookies['csrftoken'] }
-
-
+        self.session.get(f"{self.tom_url}/accounts/login/")
+        self.session.post(
+            f"{self.tom_url}/accounts/login/",
+            data={
+                "username": desc_username,
+                "password": desc_password,
+                "csrfmiddlewaretoken": self.session.cookies["csrftoken"],
+            },
+        )
+        self.csrfheader = {"X-CSRFToken": self.session.cookies["csrftoken"]}
 
     # robustify post
     @backoff.on_exception(
         backoff.expo,
         requests.ConnectionError,
         max_tries=5,
         factor=10,
-        )
+    )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: not isinstance(e, HTTPError) or e.response.status_code not in {503, 504, 429, 408},
+        giveup=lambda e: not isinstance(e, HTTPError)
+        or e.response.status_code not in {503, 504, 429, 408},
         max_time=60,
+    )
+    def tom_post(
+        self,
+        classification: ElasticcClassification | list[ElasticcClassification],
+    ) -> dict[Any, Any]:
+        response = self.session.put(
+            f"{self.tom_url}/elasticc/brokermessage/",
+            json=classification,
+            headers=self.csrfheader,
         )
-    def tom_post(self, classification: Union[ElasticcClassification,list[ElasticcClassification]])->Dict[Any,Any]:
-        response = self.session.put(f'{self.tom_url}/elasticc/brokermessage/',
-                                json=classification, headers=self.csrfheader)
 
         if response.ok:
-            self.logger.debug('ElasticcTomClient submit fail', extra={"payload": classification})
-            return {'success':True, **response.json()}
+            self.logger.debug(
+                "ElasticcTomClient submit done", extra={"payload": classification}
+            )
+            return {"success": True, **response.json()}
 
-        self.logger.info('ElasticcTomClient submit fail', extra={"payload": classification})
-        return {'success':False, 'response':response.status_code}
+        self.logger.info(
+            "ElasticcTomClient submit fail", extra={"payload": classification}
+        )
+        return {
+            "success": False,
+            "response": response.status_code,
+            "response_body": response.text,
+        }
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/PlotLightcurveSample.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/PlotLightcurveSample.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 # File              : Ampel-contrib-HU/ampel/contrib/hu/t3/PlotLightcurveSample.py
 # License           : BSD-3-Clause
 # Author            : jnordin@physik.hu-berlin.de
 # Date              : 28.09.2021
 # Last Modified Date: 28.09.2021
 # Last Modified By  : jnordin@physik.hu-berlin.de
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+import os
+import re
 from collections.abc import Generator
-import os, re
-import pandas as pd
+from contextlib import suppress
+from typing import Any
+
 import matplotlib.pyplot as plt
+import pandas as pd
 import seaborn as sns
-import numpy as np
 
-from ampel.types import UBson, T3Send
-from ampel.view.T3Store import T3Store
-from ampel.struct.UnitResult import UnitResult
-
-from ampel.view.TransientView import TransientView
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
+from ampel.struct.T3Store import T3Store
+from ampel.types import T3Send, UBson
+from ampel.view.TransientView import TransientView
 
 
 class PlotLightcurveSample(AbsPhotoT3Unit):
     """
 
     Unit plots results from lightcurve fitters (RunSncosmo, RunParsnip).
     Potentially differentiate between BTS classes, include peak magnitude and correlation strength.
@@ -48,242 +48,261 @@
         },
         'z_source' : 'AMPELz'
     }
     """
 
     # Which model config should be used? Will be matched to either
     # model (T2RunParsnip) or model_name (T2RunSncosmo)
-    unit_name: str = 'T2RunSncosmo'
+    unit_name: str = "T2RunSncosmo"
     lc_model: str
-    model_config: Optional[int]
+    model_config: None | int
 
     # Which parameters to plot (correlate)
-    param: List[str]
-    param_bounds: Optional[ Dict[str,List[float]] ]
+    param: list[str]
+    param_bounds: None | dict[str, list[float]]
     include_absmag: bool = False
 
     # Which BTS classes should be highlighted (with key as title)?
-    bts_classes: Dict[ str,List[str] ] = {
-        'SN Ia' : ['SN Ia', 'SN Ia-91T'],
-        'SN II' : ['SN II', 'SN IIP', 'SN IIb', 'SN IIb', 'SN IIn'],
-        'SN Ibc' : ['SN Ic-BL', 'SN Ib/c', 'SN Ic', 'SN Ib', 'SN Ibn'],
-        'SLSNL' : ['SLSN-I', 'SLSN-II'],
-        'TDE' : ['TDE'],
-        }
-    name_filter: dict[str, str] = {'ZTF name': 'ZTF', 'TNS ID': 'TNS'}
-
+    bts_classes: dict[str, list[str]] = {
+        "SN Ia": ["SN Ia", "SN Ia-91T"],
+        "SN II": ["SN II", "SN IIP", "SN IIb", "SN IIb", "SN IIn"],
+        "SN Ibc": ["SN Ic-BL", "SN Ib/c", "SN Ic", "SN Ib", "SN Ibn"],
+        "SLSNL": ["SLSN-I", "SLSN-II"],
+        "TDE": ["TDE"],
+    }
+    name_filter: dict[str, str] = {"ZTF name": "ZTF", "TNS ID": "TNS"}
 
     ## Methods for filtering data
     # Limit results to one of the two redshift sources (BTS, AMPELz)
-    z_source: Optional[str]
+    z_source: None | str
     # If an ampel_z_group is provided, only use values at or lower than this value
-    max_ampelz_group : Optional[int]
+    max_ampelz_group: None | int
     # Cut on a minimal number of df
-    min_dof: Optional[int]
+    min_dof: None | int
     # Cut on an allowed range of chisq / dof
-    chidof_range: Optional[List[float]]
-
+    chidof_range: None | list[float]
 
     # Output parametrs
-    plot_dir: str       # Plots will be stored here. Can be made Optional w db save
+    plot_dir: str  # Plots will be stored here. Can be made Optional w db save
     save_table: bool = False
-    plot_suffix: str = 'pdf'    # ex pdf / png
-
+    plot_suffix: str = "pdf"  # ex pdf / png
 
-    def _get_t2results(self, tran_view, t2unit, config = None):
+    def _get_t2results(self, tran_view, t2unit, config=None):
         """
         Stable method for getting the latest completed t2result for a unit.
         """
 
         t2results = []
-        if (t2docs := tran_view.get_t2_docs( unit_id = t2unit ) ):
-            for t2doc in list(t2docs) :
-                if not t2doc['status']>=0:
+        if t2docs := tran_view.get_t2_docs(unit_id=t2unit):
+            for t2doc in list(t2docs):
+                if not t2doc["status"] >= 0:
                     continue
-                if config is not None:
-                    if not t2doct['config']==config:
-                        continue
-                try:
-                    t2results.append( t2doc['body'][-1]['result'] )
-                except KeyError:
-                    pass
+                if config is not None and t2doc["config"] != config:
+                    continue
+                with suppress(KeyError):
+                    t2results.append(t2doc["body"][-1]["result"])
         return t2results
 
-
     def _get_parsnip_results(self, tran_view):
         """
         Look for results from RunParsnip corresponding to the config, if present.
         """
 
-        t2res = self._get_t2results(tran_view, 'T2RunParsnip', self.model_config)
-        t2res = [t2 for t2 in t2res if self.lc_model==t2['model']]
-        t2res = [t2 for t2 in t2res if 'prediction' in t2.keys() ]
+        t2res = self._get_t2results(tran_view, "T2RunParsnip", self.model_config)
+        t2res = [t2 for t2 in t2res if self.lc_model == t2["model"]]
+        t2res = [t2 for t2 in t2res if "prediction" in t2]
         if self.z_source:
-            t2res = [t2 for t2 in t2res if t2['z_source'] and re.match(self.z_source, t2['z_source'])]
-        if not len(t2res)>0:
+            t2res = [
+                t2
+                for t2 in t2res
+                if t2["z_source"] and re.match(self.z_source, t2["z_source"])
+            ]
+        if not len(t2res) > 0:
             return None
-        if len(t2res)>1:
-            self.logger.info('Multiple T2 results, grabbing one', extra={'stock':tran_view.id, 't2res': t2res} )
+        if len(t2res) > 1:
+            self.logger.info(
+                "Multiple T2 results, grabbing one",
+                extra={"stock": tran_view.id, "t2res": t2res},
+            )
         # Check fit quality
-        if self.min_dof and self.min_dof>t2res[0]['prediction']['model_dof']:
+        if self.min_dof and self.min_dof > t2res[0]["prediction"]["model_dof"]:
             return None
         if self.chidof_range:
-            chidof = t2res[0]['prediction']['model_chisq'] / self.min_dof>t2res[0]['prediction']['model_dof']
-            if chidof<self.chidof_range[0] or chidof>self.chidof_range[1]:
+            chidof = (
+                t2res[0]["prediction"]["model_chisq"] / self.min_dof
+                > t2res[0]["prediction"]["model_dof"]
+            )
+            if chidof < self.chidof_range[0] or chidof > self.chidof_range[1]:
                 return None
         # Now get the results
         params = {}
         for pname in self.param:
-            params[pname] = t2res[0]['prediction'][pname]
-            try:
-                params[pname+'_err'] = t2res[0]['prediction'][pname+'_error']
-            except KeyError:
-                pass
+            params[pname] = t2res[0]["prediction"][pname]
+            with suppress(KeyError):
+                params[pname + "_err"] = t2res[0]["prediction"][pname + "_error"]
         if self.include_absmag:
-            params['absmag'] = t2res[0]['prediction']['luminosity']
-            params['absmag_err'] = t2res[0]['prediction']['luminosity_error']
+            params["absmag"] = t2res[0]["prediction"]["luminosity"]
+            params["absmag_err"] = t2res[0]["prediction"]["luminosity_error"]
 
         return params
 
-
     def _get_sncosmo_results(self, tran_view):
         """
         Look for results from RunSncosmo corresponding to the config, if present.
         """
 
         if t2res := tran_view.get_t2_views(unit=self.unit_name):
-            t2res = [t2 for t2 in t2res if t2.body and 'sncosmo_result' in t2.body[-1].keys()]
-            t2res = [t2 for t2 in t2res if t2.body[-1]['sncosmo_result']['success']]
-            t2res = [t2 for t2 in t2res if self.lc_model==t2.body[-1]['model_name']]
+            t2res = [t2 for t2 in t2res if t2.body and "sncosmo_result" in t2.body[-1]]
+            t2res = [t2 for t2 in t2res if t2.body[-1]["sncosmo_result"]["success"]]
+            t2res = [t2 for t2 in t2res if self.lc_model == t2.body[-1]["model_name"]]
             if self.z_source:
-                t2res = [t2 for t2 in t2res if re.match(self.z_source, t2.body[-1]['z_source'])]
+                t2res = [
+                    t2
+                    for t2 in t2res
+                    if re.match(self.z_source, t2.body[-1]["z_source"])
+                ]
             if self.model_config:
-                t2res = [t2 for t2 in t2res if self.model_config==t2.config]
-            if not len(t2res)>0:
+                t2res = [t2 for t2 in t2res if self.model_config == t2.config]
+            if not len(t2res) > 0:
                 return None
-            if len(t2res)>1:
-                #self.logger.info('Multiple T2 results, grabbing last', extra={'stock':tran_view.id, 't2res': t2res} )
-                print('why multiple?')
+            if len(t2res) > 1:
+                # self.logger.info('Multiple T2 results, grabbing last', extra={'stock':tran_view.id, 't2res': t2res} )
+                print("why multiple?")
                 print(t2res)
             t2body = t2res[-1].body[-1]
 
             # Check fit quality
-            if self.min_dof and self.min_dof>t2body['sncosmo_result']['ndof']:
+            if self.min_dof and self.min_dof > t2body["sncosmo_result"]["ndof"]:
                 return None
             if self.chidof_range:
-                chidof = t2body['sncosmo_result']['chisq'] / t2body['sncosmo_result']['ndof']
-                if chidof<self.chidof_range[0] or chidof>self.chidof_range[1]:
+                chidof = (
+                    t2body["sncosmo_result"]["chisq"] / t2body["sncosmo_result"]["ndof"]
+                )
+                if chidof < self.chidof_range[0] or chidof > self.chidof_range[1]:
                     return None
 
             # Now get the results
             params = {}
             for pname in self.param:
-                ix = t2body['sncosmo_result']['param_names'].index(pname)
-                params[pname] = t2body['sncosmo_result']['parameters'][t2body['sncosmo_result']['param_names'].index(pname)]
-                params[pname+'_err'] = t2body['sncosmo_result']['errors'][pname]
+                ix = t2body["sncosmo_result"]["param_names"].index(pname)
+                params[pname] = t2body["sncosmo_result"]["parameters"][ix]
+                params[pname + "_err"] = t2body["sncosmo_result"]["errors"][pname]
 
             # For some reason not always showing up?
             if self.include_absmag:
-                params['absmag'] = t2body['fit_metrics']['restpeak_model_absmag_B']
-                #params['absmag_err'] = -2.5 / np.log(10) * df['x0_err'] / df['x0']
+                params["absmag"] = t2body["fit_metrics"]["restpeak_model_absmag_B"]
+                # params['absmag_err'] = -2.5 / np.log(10) * df['x0_err'] / df['x0']
             return params
-        else:
-            return None # Explicit, nothing found.
+        return None  # Explicit, nothing found.
 
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: Optional[T3Store] = None) -> Union[UBson, UnitResult]:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None
+    ) -> None:
         """
         Loop through provided TransientViews and retrieve data to plot.
         """
 
-
         table_rows: list[dict[str, Any]] = []
-        for k, tran_view in enumerate(gen, 1):
-
-            sninfo: dict[str,UBson] = {}
+        for tran_view in gen:
+            sninfo: dict[str, UBson] = {}
             # Collect base information applying to all states
             # If here, add stock info (name, channel etcs)
             if names := (tran_view.stock or {}).get("name", []):
                 for label, name_str in self.name_filter.items():
                     r = re.compile(name_str)
                     # While names will mostly be unique, it might not always be the case.
-                    sninfo[label] = list(filter(r.match, names)) # type: ignore[arg-type]
+                    sninfo[label] = list(filter(r.match, names))  # type: ignore[arg-type]
                     # Avoid list when possible
-                    if isinstance((item := sninfo[label]), (list, tuple)) and len(item) == 1:
+                    if (
+                        isinstance((item := sninfo[label]), list | tuple)
+                        and len(item) == 1
+                    ):
                         sninfo[label] = item[0]
-            sninfo['stock'] = tran_view.id
+            sninfo["stock"] = tran_view.id
             assert tran_view.stock
-            sninfo['channels'] = tran_view.stock.get("channel") # type: ignore[assignment]
+            sninfo["channels"] = tran_view.stock.get("channel")  # type: ignore[assignment]
 
             # Get AmpelZ info
-            ampelz, ampelz_group = None, 99
-            if isinstance(t2res := tran_view.get_latest_t2_body(unit='T2DigestRedshifts'), dict):
-                if 'ampel_z' in t2res.keys():
-                    # In case of multiple entries, no way to distinguish these (would have to add config selection to get_t2results)
-                    sninfo['ampel_z_group'] = t2res['group_z_nbr']
-                    sninfo['ampel_z'] = t2res['ampel_z']
-            if self.max_ampelz_group:
-                if isinstance(ampel_z_group := sninfo.get("ampel_z_group"), int) and self.max_ampelz_group < ampel_z_group:
-                    # Skip this one, z too uncertain
-                    continue
+            if (
+                isinstance(
+                    t2res := tran_view.get_latest_t2_body(unit="T2DigestRedshifts"),
+                    dict,
+                )
+                and "ampel_z" in t2res
+            ):
+                # In case of multiple entries, no way to distinguish these (would have to add config selection to get_t2results)
+                sninfo["ampel_z_group"] = t2res["group_z_nbr"]
+                sninfo["ampel_z"] = t2res["ampel_z"]
+            if self.max_ampelz_group and (
+                isinstance(ampel_z_group := sninfo.get("ampel_z_group"), int)
+                and self.max_ampelz_group < ampel_z_group
+            ):
+                # Skip this one, z too uncertain
+                continue
 
             # Get BTS class if available
-            if isinstance(t2res := tran_view.get_latest_t2_body(unit='T2MatchBTS'), dict):
+            if isinstance(
+                t2res := tran_view.get_latest_t2_body(unit="T2MatchBTS"), dict
+            ):
                 # Get plot class from BTS matching (if any)
-                bts_class = 'Unknown'
-                if 'bts_type' in t2res.keys():
+                bts_class = "Unknown"
+                if "bts_type" in t2res:
                     for bts_name, bts_subclasses in self.bts_classes.items():
-                        if t2res['bts_type'] in bts_subclasses:
+                        if t2res["bts_type"] in bts_subclasses:
                             bts_class = bts_name
-                sninfo['class_from_bts'] = bts_class
+                sninfo["class_from_bts"] = bts_class
 
             # Finally, we collect fit information from either T2RunSncosmo or T2RunParsnip
             lcinfo = self._get_sncosmo_results(tran_view)
             # Have to reawaken parsnip before this can be tested
-            #if not lcinfo:
+            # if not lcinfo:
             #    lcinfo = self._get_parsnip_results(tran_view)
             if lcinfo:
                 # No fit info fulfilling requirements
-                #continue
+                # continue
                 sninfo.update(lcinfo)
 
-
-
             table_rows.append(sninfo)
 
-
         # Convert
-        df = pd.DataFrame.from_dict( table_rows )
+        df = pd.DataFrame.from_dict(table_rows)
 
         # Cut down based on parameter bounds
         if self.param_bounds:
             for pname, pbound in self.param_bounds.items():
-                df = df[ (df[pname]>=pbound[0]) & (df[pname]<=pbound[1]) ]
+                df = df[(df[pname] >= pbound[0]) & (df[pname] <= pbound[1])]
 
         # Create main pairgrid plot
-        plt.figure(1, figsize=(20,20) )
-        g = sns.PairGrid(df, hue='class_from_bts', vars=self.param)
+        plt.figure(1, figsize=(20, 20))
+        g = sns.PairGrid(df, hue="class_from_bts", vars=self.param)
         g.map_lower(plt.scatter)
         g.map_upper(sns.kdeplot)
         g.map_diag(sns.kdeplot, lw=3, legend=True)
         g.add_legend()
-        ppath = os.path.join( self.plot_dir, 't3plotlightcurvesample.'+self.plot_suffix )
-        plt.savefig( ppath, dpi=300 )
+        ppath = os.path.join(
+            self.plot_dir, "t3plotlightcurvesample." + self.plot_suffix
+        )
+        plt.savefig(ppath, dpi=300)
         plt.clf()
         plt.close()
 
         # Compare properties with absolute mag, if chosen
         if self.include_absmag:
-            plt.figure(2, figsize=(20,10) )
-            g = sns.PairGrid(df, hue="class_from_bts", x_vars=["absmag"] + self.param, y_vars="absmag")
+            plt.figure(2, figsize=(20, 10))
+            g = sns.PairGrid(
+                df,
+                hue="class_from_bts",
+                x_vars=["absmag", *self.param],
+                y_vars="absmag",
+            )
             g.map_diag(sns.histplot, color=".3")
             g.map_offdiag(sns.scatterplot)
             g.add_legend()
-            ppath = os.path.join( self.plot_dir, 't3plotlightcurvesample_absmag.'+self.plot_suffix )
-            plt.savefig( ppath, dpi=300 )
+            ppath = os.path.join(
+                self.plot_dir, "t3plotlightcurvesample_absmag." + self.plot_suffix
+            )
+            plt.savefig(ppath, dpi=300)
             plt.clf()
             plt.close()
 
-
         if self.save_table:
-            df.to_csv( os.path.join( self.plot_dir, 'plot_lightcurvesample.csv' ) )
-        
-        return None
+            df.to_csv(os.path.join(self.plot_dir, "plot_lightcurvesample.csv"))
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidBase.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t3/RapidBase.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                15.07.2019
 # Last Modified Date:  06.02.2020
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-from typing import Any
 from collections.abc import Generator
+from typing import Any
 
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.secret.NamedSecret import NamedSecret
 from ampel.struct.JournalAttributes import JournalAttributes
+from ampel.struct.T3Store import T3Store
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import T3Send, UBson
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
-from ampel.types import UBson, T3Send
-from ampel.view.T3Store import T3Store
 
 
 # get the science records for the catalog match
 def get_catalogmatch_srecs(tran_view, logger):
     cat_res = tran_view.get_science_records(t2_class_name="CATALOGMATCH")
     if len(cat_res) == 0 or cat_res is None or cat_res[-1].get_results() is None:
         logger.info("NO CATALOG MATCH FOR THIS TRANSIENT")
@@ -53,33 +53,31 @@
 
     slack_channel: str = "#ztf_auto"
     slack_username: str = "AMPEL"
 
     # List of T2 unit names which should be collected for reaction
     t2info_from: list[str] = []
 
-
     def post_init(self) -> None:
-
         self.name = "RapidBase"
         self.logger.info(f"Initialized T3 RapidBase instance {self.name}")
 
         # feedback
         for k in self.__annotations__:
             self.logger.info(f"Using {k}={getattr(self, k)}")
 
-
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None) -> UBson | UnitResult:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None
+    ) -> UBson | UnitResult:
         """
         Loop through transients and check for TNS names and/or candidates to submit
         """
 
         # We will here loop through transients and react individually
         for tv in gen:
-
             transientinfo = self.collect_info(tv)
             self.logger.info("reacting", extra={"tranId": tv.id})
 
             # Ok, so we have a transient to react to
             if self.do_react:
                 success, jcontent = self.react(tv, transientinfo)
             # Otherwise, test
@@ -87,69 +85,61 @@
                 test_success, jcontent = self.test_react(tv, transientinfo)
 
             if jcontent:
                 gen.send(JournalAttributes(extra=jcontent))
 
         return None
 
-
     def react(
         self, tran_view: TransientView, info: None | dict[str, Any]
     ) -> tuple[bool, None | dict[str, Any]]:
         """
         Replace with react method adopted to particular facility or output
         """
 
         raise NotImplementedError("No real reaction implemented in RapidBase")
         return self.test_react(tran_view, info)
 
-
     def test_react(
         self, tran_view: TransientView, info: None | dict[str, Any]
     ) -> tuple[bool, None | dict[str, Any]]:
-        """ Trigger a test slack report """
+        """Trigger a test slack report"""
 
         success = False
 
         if not self.slack_token:
             return False, None
 
         from slack import WebClient
         from slack.errors import SlackClientError
         from slack.web.slack_response import SlackResponse
 
-
         sc = WebClient(self.slack_token.get())
         assert isinstance(tran_view.id, int)
         ztf_name = to_ztf_id(tran_view.id)
-        msg = "Ampel RapidReact says: Look up %s. Provided info %s" % (
-            ztf_name,
-            info,
-        )
+        msg = f"Ampel RapidReact says: Look up {ztf_name}. Provided info {info}"
         api = sc.chat_postMessage(
             channel=self.slack_channel,
             text=msg,
             username=self.slack_username,
             as_user=False,
         )
         assert isinstance(api, SlackResponse)
         if not api["ok"]:
             raise SlackClientError(api["error"])
-        else:
-            success = True
+        success = True
 
         description = "Sent SLACK msg"
         self.logger.info(description, extra={"channel": self.slack_channel})
 
         # Document what we did
         jcontent = {"reaction": description, "success": success}
 
         return success, jcontent
 
-
     def collect_info(self, tran_view: TransientView) -> None | dict[str, Any]:
         """
         Create an information dict from T2 outputs, which can be used by reactors.
         """
 
         info: dict[str, Any] = {}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidLco.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidLco.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 # File:                ampel/contrib/hu/t3/rapidBase
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                05.08.2019
 # Last Modified Date:  20.08.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
-import datetime, requests
-from typing import Any, Tuple
+import datetime
+from typing import Any
+
+import requests
 
 from ampel.contrib.hu.t3.RapidBase import RapidBase
 from ampel.secret.NamedSecret import NamedSecret
 from ampel.util.freeze import recursive_unfreeze
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
 
@@ -166,15 +168,14 @@
                         "location": {"telescope_class": "1m0"},
                     }
                 ],
             },
         },
     }
 
-
     def react(
         self, tran_view: TransientView, info: None | dict[str, Any]
     ) -> tuple[bool, dict[str, Any]]:
         """
         Send a trigger to the LCO
         """
 
@@ -182,67 +183,65 @@
             return False, {"success": False}
         assert isinstance(tran_view.id, int)
         transient_name = to_ztf_id(tran_view.id)
 
         # Look for coordinates in the T2 info dicts.
         # Assuming ra and dec exists in there
         ra, dec = None, None
-        for t2unit, t2info in info.items():
-            if 'ra' in t2info.keys():
-                ra = t2info['ra']
-            if 'dec' in t2info.keys():
-                dec = t2info['dec']
+        for t2info in info.values():
+            if "ra" in t2info:
+                ra = t2info["ra"]
+            if "dec" in t2info:
+                dec = t2info["dec"]
         if ra is None or dec is None:
             # Look at the response
             self.logger.info(
                 "No LCO trigger: Could not find ra/dec",
                 extra={
                     "target": transient_name,
                 },
             )
 
-
         # Step through all LCO submit forms
         success = True  # Will be set to false if any submit fails
         submitted = []
         responses = []
 
         for submit_name, submit_info in self.lco_payload.items():
-
             # Create submit dictionary
             react_dict = recursive_unfreeze(submit_info["api_form"])
 
             # Update with information
             react_dict["name"] = submit_name + "_" + transient_name
             react_dict["requests"][0]["configurations"][0]["target"][
                 "name"
             ] = transient_name
             react_dict["requests"][0]["configurations"][0]["target"]["ra"] = str(ra)
             react_dict["requests"][0]["configurations"][0]["target"]["dec"] = str(dec)
             # Some keys are not necessarily there
-            timenow = datetime.datetime.utcnow()
-            if "start" in react_dict["requests"][0]["windows"][0].keys():
+            timenow = datetime.datetime.now(tz=datetime.timezone.utc)
+            if "start" in react_dict["requests"][0]["windows"][0]:
                 dtime = datetime.timedelta(days=submit_info["start_delay"])
                 react_dict["requests"][0]["windows"][0]["start"] = "%s" % (
-                    (timenow + dtime)
+                    timenow + dtime
                 )
-            if "end" in react_dict["requests"][0]["windows"][0].keys():
+            if "end" in react_dict["requests"][0]["windows"][0]:
                 dtime = datetime.timedelta(days=submit_info["end_delay"])
                 react_dict["requests"][0]["windows"][0]["end"] = "%s" % (
-                    (timenow + dtime)
+                    timenow + dtime
                 )
 
             self.logger.debug(
                 "Starting LCO trigger",
                 extra={"target": transient_name, "react_dict": react_dict},
             )
             # Make a test to validate
             testreply = requests.post(
                 "https://observe.lco.global/api/requestgroups/validate/",
-                headers={"Authorization": "Token {}".format(self.lco_api.get())},
+                headers={"Authorization": f"Token {self.lco_api.get()}"},
                 json=react_dict,
             )
 
             # Abort if we have errors
             if len(testreply.json()["errors"]) > 0:
                 self.logger.info(
                     "Validating LCO trigger fails for for %s" % (transient_name),
@@ -250,15 +249,15 @@
                 )
                 success = False
                 continue
 
             # Submit full trigger
             response = requests.post(
                 "https://observe.lco.global/api/requestgroups/",
-                headers={"Authorization": "Token {}".format(self.lco_api.get())},
+                headers={"Authorization": f"Token {self.lco_api.get()}"},
                 json=react_dict,
             )
 
             # Check whether this was successful
             try:
                 response.raise_for_status()
             except requests.exceptions.HTTPError:
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/RapidSedm.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidSedm.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t3/RapidSedm.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                05.08.2019
 # Last Modified Date:  06.02.2020
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-import datetime, requests
-from typing import Any, Tuple
-from ampel.secret.NamedSecret import NamedSecret
+import datetime
+from typing import Any
+
+import requests
+
 from ampel.contrib.hu.t3.RapidBase import RapidBase
+from ampel.secret.NamedSecret import NamedSecret
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
 
 
 class RapidSedm(RapidBase):
     """
     Select transients for rapid reactions. Intended as base class where the react method can be
@@ -92,22 +95,24 @@
         react_dict.update(self.sedm_payload)
         react_dict["obj_ra"] = info["ra"]
         react_dict["obj_dec"] = info["dec"]
         react_dict["obj_mag"] = info[
             "latest_mag"
         ]  # Assuming that the object is not declining?
         react_dict["obj_name"] = to_ztf_id(tran_view.id)
-        react_dict["inidate"] = datetime.datetime.utcnow()
-        react_dict["enddate"] = datetime.datetime.utcnow() + datetime.timedelta(days=2)
+        react_dict["inidate"] = datetime.datetime.now(tz=datetime.timezone.utc)
+        react_dict["enddate"] = datetime.datetime.now(
+            tz=datetime.timezone.utc
+        ) + datetime.timedelta(days=2)
 
         # We are still in debug stage, turn down priority
         # react_dict['priority'] = 1
 
         self.logger.debug(
-            "SEDM trigger for %s w dict %s" % (to_ztf_id(tran_view.id), react_dict)
+            f"SEDM trigger for {to_ztf_id(tran_view.id)} w dict {react_dict}"
         )
 
         # Make the post
         response = requests.post(
             self.sedm_url,
             data=react_dict,
             auth=(self.sedm_username, self.sedm_password.get()),
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/SlackSummaryPublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/SlackSummaryPublisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 # Author:              robert stein
 # Date:                11.03.2018
 # Last Modified Date:  14.11.2018
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 import datetime
 import io
-from collections.abc import Mapping
-from typing import cast
-from collections.abc import Iterable, Generator
+from collections.abc import Generator, Iterable, Mapping
+from typing import Any, cast
 
 import numpy as np
 import pandas as pd
 import requests
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackClientError
+from slack_sdk.web import SlackResponse
 
-from ampel.types import T3Send
-from ampel.view.T3Store import T3Store
 from ampel.abstract.AbsT3ReviewUnit import AbsT3ReviewUnit
 from ampel.log.utils import log_exception
 from ampel.secret.NamedSecret import NamedSecret
+from ampel.struct.T3Store import T3Store
+from ampel.types import T3Send
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
-from slack_sdk.web import SlackResponse
 
 
 class SlackSummaryPublisher(AbsT3ReviewUnit):
     """"""
 
     dry_run: bool = False
     quiet: bool = False
@@ -46,23 +45,25 @@
         "sgscore1",
         "rb",
         "distnr",
         "distpsnr1",
         "isdiffpos",
     ]
 
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: T3Store) -> None:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: T3Store
+    ) -> None:
         """"""
         channels: set[str] = set()
         frames, photometry = self.combine_transients(gen, channels)
 
         if len(frames) == 0 and self.quiet:
             return
 
-        date = str(datetime.date.today())
+        date = str(datetime.datetime.now(tz=datetime.timezone.utc).date())
 
         sc = WebClient(self.slack_token.get())
 
         m = calculate_excitement(len(frames), date=date, thresholds=self.excitement)
 
         if self.dry_run:
             self.logger.info(m)
@@ -80,15 +81,14 @@
                     },
                 ),
             )
             if not api["ok"]:
                 raise SlackClientError(api["error"])
 
         if len(frames) > 0:
-
             df = pd.DataFrame.from_records(frames)
             # Set fill value for channel columns to False
             for channel in channels:
                 df[channel].fillna(False, inplace=True)
             # Set fill value for all other columns to MISSING
             for field in set(df.columns.values).difference(channels):
                 df[field].fillna("MISSING", inplace=True)
@@ -143,15 +143,16 @@
                     photometry_df[channel].fillna(False, inplace=True)
                 # Set fill value for all other columns to MISSING
                 for field in set(photometry_df.columns.values).difference(channels):
                     photometry_df[field].fillna("MISSING", inplace=True)
                 # Move channel info at end
                 photometry_df = photometry_df.reindex(
                     copy=False,
-                    columns=[c for c in df.columns if c not in channels] + list(channels)
+                    columns=[c for c in df.columns if c not in channels]
+                    + list(channels),
                 )
 
                 filename = "Photometry_%s.csv" % date
 
                 buffer = io.StringIO(filename)
                 photometry_df.to_csv(buffer)
 
@@ -188,50 +189,49 @@
     ) -> tuple[list[pd.DataFrame], list[pd.DataFrame]]:
         """"""
 
         frames = []
         photometry = []
 
         for transient in transients:
-
             mycols = set(self.cols)
 
             frame = {
                 "tranId": transient.id,
                 "ztf_name": to_ztf_id(transient.id),
             }
 
             if summary := transient.get_t2_body(unit="T2LightCurveSummary"):
                 frame.update(summary)  # type: ignore[arg-type]
 
             # include other T2 results, flattened
             for t2record in transient.t2 or []:
                 if (
-                    t2record.unit == "T2LightCurveSummary" or
-                    not (output := t2record.get_payload()) or
-                    not isinstance(output, dict)
+                    t2record.unit == "T2LightCurveSummary"
+                    or not (output := t2record.get_payload())
+                    or not isinstance(output, dict)
                 ):
                     continue
 
                 # Flatten T2 output dictionary
                 # If this is not a dictionry it will be through
                 res_flat = flat_dict(output, prefix="T2-")
 
                 # Add these to the dataframe (could we just join the dictionaries?)
                 for key, value in res_flat.items():
                     try:
                         frame[key] = str(value)
-                    except ValueError as ve:
+                    except ValueError as ve:  # noqa: PERF203
                         log_exception(self.logger, ve)
 
             assert transient.stock
             frame.update(
                 {str(channel): True for channel in (transient.stock["channel"] or [])}
             )
-            channels.update((str(c) for c in transient.stock["channel"] or []))
+            channels.update(str(c) for c in transient.stock["channel"] or [])
 
             frames.append(frame)
 
             if self.full_photometry:
                 if transient.t0 is None:
                     raise ValueError(
                         "Full photometry requested, but no T0 records loaded"
@@ -267,83 +267,82 @@
         message += (
             "It might be worth checking the ZTF-General Slack channel "
             "for detector issues."
         )
 
         return message
 
+    if not np.isnan(n_alerts):
+        message += " In total, " + str(n_alerts) + " alerts were ingested. \n"
     else:
-        if not np.isnan(n_alerts):
-            message += " In total, " + str(n_alerts) + " alerts were ingested. \n"
-        else:
-            message += "\n"
+        message += "\n"
 
-        if n_transients == 0:
-            message += (
-                "TRAGEDY! Sadly, it seems that no transients passed the "
-                "filters last night"
-            )
-            return message
+    if n_transients == 0:
+        message += (
+            "TRAGEDY! Sadly, it seems that no transients passed the "
+            "filters last night"
+        )
+        return message
 
-        elif n_transients == 1:
-            message += (
-                "LONE WOLF! It seems that there was just one transient"
-                " which passed the filters. Guess it's better than "
-                "nothing... :shrug: \n ~The results are summarised "
-                "below.~ That one result is shown below."
-            )
-            return message
+    if n_transients == 1:
+        message += (
+            "LONE WOLF! It seems that there was just one transient"
+            " which passed the filters. Guess it's better than "
+            "nothing... :shrug: \n ~The results are summarised "
+            "below.~ That one result is shown below."
+        )
+        return message
 
-        elif n_transients < thresholds["Low"]:
-            message += (
-                "MEH! We only found " + str(n_transients) + " "
-                "transients last night. :unamused: That's "
-                "disappointing. Hopefully we get more tomorrow!"
-            )
+    if n_transients < thresholds["Low"]:
+        message += (
+            "MEH! We only found " + str(n_transients) + " "
+            "transients last night. :unamused: That's "
+            "disappointing. Hopefully we get more tomorrow!"
+        )
 
-        elif n_transients < thresholds["Mid"]:
-            message += (
-                "NOT BAD! We found " + str(n_transients) + " "
-                "transients last night. :slightly_smiling_face: "
-                "Let's keep up the good work!"
-            )
+    elif n_transients < thresholds["Mid"]:
+        message += (
+            "NOT BAD! We found " + str(n_transients) + " "
+            "transients last night. :slightly_smiling_face: "
+            "Let's keep up the good work!"
+        )
 
-        elif n_transients < thresholds["High"]:
-            message += (
-                "IMPRESSIVE! We found " +
-                str(n_transients) +
-                " transients last night. :grin: That's exciting! Good "
-                "luck to anyone trying to check all of those by hand..."
-            )
+    elif n_transients < thresholds["High"]:
+        message += (
+            "IMPRESSIVE! We found "
+            + str(n_transients)
+            + " transients last night. :grin: That's exciting! Good "
+            "luck to anyone trying to check all of those by hand..."
+        )
 
-        else:
-            message += (
-                "WOW!!! We found " +
-                str(n_transients) +
-                " transients last night. :tada: That's loads! Now we "
-                "just need to figure out what to do with all of them..."
-            )
+    else:
+        message += (
+            "WOW!!! We found "
+            + str(n_transients)
+            + " transients last night. :tada: That's loads! Now we "
+            "just need to figure out what to do with all of them..."
+        )
 
-        message += "\n The results are summarised below. "
+    message += "\n The results are summarised below. "
 
     return message
 
 
-def flat_dict(d, prefix=""):
+def flat_dict(d: Mapping[Any, Any], prefix: str = "") -> dict[str, Any]:
     """
     Loop through dictionary d
     Append any key, val pairs to the return list ret
     Add the prefix to any key param
     Recurse if encountered value is a nested dictionary.
     """
 
     if not isinstance(d, Mapping):
         return d
 
-    ret = {}
+    ret: dict[str, Any] = {}
 
     for key, val in d.items():
         if isinstance(val, Mapping):
             ret = {**ret, **flat_dict(val, prefix=prefix + str(key) + "_")}
         else:
             ret[prefix + str(key)] = val
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TNSMirrorUpdater.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSMirrorUpdater.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import asyncio
 import datetime
 from typing import Any
 
 from pymongo import MongoClient
 
 from ampel.abstract.AbsOpsUnit import AbsOpsUnit
-from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
 from ampel.contrib.hu.t3.tns.TNSClient import TNSClient
 from ampel.contrib.hu.t3.tns.TNSMirrorDB import TNSMirrorDB
+from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
 from ampel.secret.NamedSecret import NamedSecret
 
 
 class TNSMirrorUpdater(AbsOpsUnit):
     """
     Sync a local mirror of the TNS database
     """
@@ -28,16 +28,15 @@
     extcats_auth: NamedSecret[dict] = NamedSecret(label="extcats/writer")
     api_key: NamedSecret[dict]
     timeout: float = 60.0
     max_parallel_requests: int = 8
     dry_run: bool = False
 
     def run(self, beacon: None | dict[str, Any] = None) -> None | dict[str, Any]:
-
-        now = datetime.datetime.utcnow()
+        now = datetime.datetime.now(tz=datetime.timezone.utc)
         last_run = beacon["updated"] if beacon else now - datetime.timedelta(days=7)
 
         async def fetch():
             tns = TNSClient(
                 TNSToken(**self.api_key.get()),
                 self.timeout,
                 self.max_parallel_requests,
@@ -46,13 +45,13 @@
             return [item async for item in tns.search(public_timestamp=str(last_run))]
 
         if not self.dry_run:
             new_reports = asyncio.get_event_loop().run_until_complete(fetch())
             TNSMirrorDB(
                 MongoClient(
                     self.context.config.get("resource.extcats", str, raise_exc=True),
-                    **self.extcats_auth.get()
+                    **self.extcats_auth.get(),
                 ),
                 logger=self.logger,
             ).add_sources(new_reports)
 
         return {"updated": now}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TNSTalker.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSTalker.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                17.11.2018
 # Last Modified Date:  04.09.2019
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 import re
-from itertools import islice
-from typing import Any, TYPE_CHECKING
 from collections.abc import Generator, Iterable
-from ampel.struct.StockAttributes import StockAttributes
-from ampel.types import StockId
+from itertools import islice
+from typing import TYPE_CHECKING, Any
+
 from ampel.abstract.AbsT3ReviewUnit import AbsT3ReviewUnit, T3Send
+from ampel.contrib.hu.t3.ampel_tns import (
+    TNS_BASE_URL_REAL,
+    TNS_BASE_URL_SANDBOX,
+    TNSClient,
+)
+from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
 from ampel.secret.NamedSecret import NamedSecret
 from ampel.struct.JournalAttributes import JournalAttributes
-from ampel.contrib.hu.t3.ampel_tns import TNSClient, TNS_BASE_URL_REAL, TNS_BASE_URL_SANDBOX
-from ampel.view.T3Store import T3Store
+from ampel.struct.StockAttributes import StockAttributes
+from ampel.struct.T3Store import T3Store
+from ampel.types import StockId
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
-from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
 
 if TYPE_CHECKING:
     from ampel.content.JournalRecord import JournalRecord
 
 
 def chunks(l: Iterable, n: int) -> Generator[list, None, None]:
     source = iter(l)
@@ -70,15 +75,15 @@
     # Submit to TNS sandbox only
     sandbox: bool = True
     # weather journal will go to separate collection.
     ext_journal: bool = True
 
     # AT report config
     base_at_dict: dict = {
-        "reporting_group_id": "82",    # Should be ampel
+        "reporting_group_id": "82",  # Should be ampel
         "discovery_data_source_id": "48",
         "reporter": "J. Nordin, V. Brinnel, J. van Santen (HU Berlin), A. Gal-Yam, O. Yaron, S. Schulze (Weizmann) on behalf of ZTF",
         "at_type": "1",
     }
     baseremark: str = "See arXiv:1904.05922 for selection criteria."
 
     slack_token: None | NamedSecret = None
@@ -91,34 +96,39 @@
         super().__init__(**kwargs)
         self.client = TNSClient(
             TNS_BASE_URL_SANDBOX if self.sandbox else TNS_BASE_URL_REAL,
             self.logger,
             TNSToken(**self.tns_api_key.get()),
         )
         # maintain a second client to check the real TNS if in sandbox mode
-        self.reference_client = TNSClient(
-            TNS_BASE_URL_REAL,
-            self.logger,
-            TNSToken(**self.tns_api_key.get()),
-        ) if self.sandbox else self.client
+        self.reference_client = (
+            TNSClient(
+                TNS_BASE_URL_REAL,
+                self.logger,
+                TNSToken(**self.tns_api_key.get()),
+            )
+            if self.sandbox
+            else self.client
+        )
 
     def search_journal_tns(
         self, tran_view: TransientView
     ) -> tuple[None | str, list[str]]:
         """
         Look through the journal for a TNS name.
         Assumes journal entries came from this unit, that the TNS name is saved as "tnsName"
         and internal names as "tnsInternal"
         """
         tns_name, tns_internals = None, []
 
         def select(entry: "JournalRecord") -> bool:
             return bool(
-                (entry["extra"] is not None and ("tnsInternal" in entry["extra"])) and
-                entry["unit"] and entry["unit"] == self.__class__.__name__
+                (entry["extra"] is not None and ("tnsInternal" in entry["extra"]))
+                and entry["unit"]
+                and entry["unit"] == self.__class__.__name__
             )
 
         if jentries := list(tran_view.get_journal_entries(tier=3, filter_func=select)):
             if jentries[-1]["extra"] is not None:
                 tns_name = jentries[-1]["extra"].get("tnsName", None)
             tns_internals = [
                 entry["extra"].get("tnsInternal", None)
@@ -143,43 +153,49 @@
         Assumes journal entries came from this unit, that the TNS name is saved as "tnsName"
         and tnsSender stores the api key used ('tnsSender': self.tns_api_key')
         """
 
         def select(entry: "JournalRecord") -> bool:
             return bool(
                 (
-                    entry["extra"] is not None and
-                    (entry["extra"].get("tnsSender") == self.tns_api_key.get()["name"]) and
-                    "tnsSubmitResult" in entry["extra"]
-                ) and
-                entry["unit"] and entry["unit"] == self.__class__.__name__
+                    entry["extra"] is not None
+                    and (
+                        entry["extra"].get("tnsSender")
+                        == self.tns_api_key.get()["name"]
+                    )
+                    and "tnsSubmitResult" in entry["extra"]
+                )
+                and entry["unit"]
+                and entry["unit"] == self.__class__.__name__
             )
 
         # Find the latest tns name (skipping previous)
         if tran_view.get_journal_entries(
             tier=3,
             filter_func=select,
         ):
-            self.logger.info("TNS submitted", extra={"tnsSender": self.tns_api_key.get()["name"]})
+            self.logger.info(
+                "TNS submitted", extra={"tnsSender": self.tns_api_key.get()["name"]}
+            )
             return True
-        else:
-            self.logger.info("Not TNS submitted", extra={"tnsSender": self.tns_api_key.get()["name"]})
-            return False
+        self.logger.info(
+            "Not TNS submitted", extra={"tnsSender": self.tns_api_key.get()["name"]}
+        )
+        return False
 
-    def _query_tns_names(self, tran_view: TransientView, ra: float, dec: float) -> tuple[None | str, list]:
+    def _query_tns_names(
+        self, tran_view: TransientView, ra: float, dec: float
+    ) -> tuple[None | str, list]:
         """
         query the TNS for names and internals at the position
         of the transient.
         """
         # query the TNS for transient at this position. Note that we check the real TNS for names for compatibility...
 
-        tns_name, tns_internal = self.client.getNames(
-            ra=ra,
-            dec=dec
-        )
+        tns_name, tns_internal = self.client.getNames(ra=ra, dec=dec)
 
         # Skip the AT SN prefix if present
         if tns_name is not None:
             tns_name = re.sub("^AT", "", tns_name)
             tns_name = re.sub("^SN", "", tns_name)
 
         # be nice and then go
@@ -208,27 +224,28 @@
         tns_name, tns_internals = None, []
         names: list[str] = (
             [str(name) for name in (tran_view.stock["name"] or [])]
             if tran_view.stock
             else []
         )
         for tname in names:
-
             if "TNS" in tname and (not self.get_tns_force):
                 self.logger.info(
                     "found TNS name in tran_names.",
                     extra={"TNSname": tname, "TransNames": names},
                 )
                 # as TNS to give you the internal names.
                 # we remove the 'TNS' part of the name, since this has been
                 # added by the TNSMatcher T3, plus we skip the prefix
                 # We here assume that the AT/SN suffix is cut
                 tns_name = tname.replace("TNS", "")
                 # Not using sandbox (only checking wrt to full system).
-                tns_internals, runstatus = self.reference_client.getInternalName(tns_name)
+                tns_internals, runstatus = self.reference_client.getInternalName(
+                    tns_name
+                )
 
         # be nice with the logging
         ztf_name = to_ztf_id(tran_view.id)
         self.logger.info(
             "looked for TNS name in self.tran_names",
             extra={
                 "ZTFname": ztf_name,
@@ -236,15 +253,14 @@
                 "tnsInternals": tns_internals,
                 "TransNames": names,
             },
         )
 
         return tns_name, tns_internals
 
-
     def find_tns_name(
         self, tran_view: TransientView, ra: float, dec: float
     ) -> tuple[None | str, list[str], None | JournalAttributes]:
         """
         extensive search for TNS names in:
         - tran_view.tran_names (if added by TNSMatcher)
         - the journal of tran_view (if added by this T3)
@@ -266,32 +282,29 @@
         if (tns_name is not None) and (not self.get_tns_force):
             return tns_name, tns_internals, None
 
         # second option in case there is no TNS name in the journal: go and look in tran_names
         # and if you don't find any, go and ask TNS again.
         tns_name_new, tns_internals_new = self._find_tns_tran_names(tran_view)
         self.logger.debug(
-            "Find tns names added to the ampel name list: %s internal %s"
-            % (tns_name_new, tns_internals_new)
+            f"Find tns names added to the ampel name list: {tns_name_new} internal {tns_internals_new}"
         )
         if tns_name_new is None:
             tns_name_new, tns_internals_new = self._query_tns_names(tran_view, ra, dec)
             self.logger.debug(
                 "Proper check of tns done, found name %s" % (tns_name_new)
             )
 
-
         # now, it is possible (if you set self.get_tns_force) that the
         # new TNS name is different from the one we had in the journal. We always
         # use the most recent one. In this case we also create a JournalUpdate
         jup = None
         if tns_name_new is not None:
-
             # what happen if you have a new name that is different from the old one?
-            if tns_name is not None and not tns_name == tns_name_new:
+            if tns_name is not None and tns_name != tns_name_new:
                 self.logger.info(
                     "Adding new TNS name",
                     extra={"tnsOld": tns_name, "tnsNew": tns_name_new},
                 )
 
                 # create content of journal entry. Eventually
                 # update the list with the new internal names if any are found
@@ -323,41 +336,43 @@
                 jup = JournalAttributes(extra=jcontent)
                 tns_name = tns_name_new
                 # tns_internals = tns_internals_new
 
         # bye!
         return tns_name, tns_internals, jup
 
-
-
-    def process(self, gen: Generator[TransientView, T3Send, None], t3s: T3Store) -> None:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: T3Store
+    ) -> None:
         """
         Loop through transients and check for TNS names and/or candidates to submit
         """
 
         # Reports to be sent, indexed by the transient view IDs (so that we can check in the replies)
         atreports: dict[StockId, dict[str, Any]] = {}
 
         for tran_view in gen:
-
             ztf_name = to_ztf_id(tran_view.id)
 
             # Obtain atdict start from T2 result
             t2result = tran_view.get_t2_body(unit="T2TNSEval")
             if not isinstance(t2result, dict):
-                raise ValueError("Need to have a TNS atdict started from a suitable T2.")
+                raise ValueError(
+                    "Need to have a TNS atdict started from a suitable T2."
+                )
             # Create the submission dictionary - in case the transient is to be submitted
-            atdict = dict(t2result['atdict'])
+            atdict = dict(t2result["atdict"])
             atdict.update(self.base_at_dict)
             atdict["internal_name"] = ztf_name
 
-            ra, dec = atdict['ra']['value'], atdict['dec']['value']
+            ra, dec = atdict["ra"]["value"], atdict["dec"]["value"]
 
             self.logger.info(
-                "TNS init dict found", extra={"tranId": tran_view.id, "ztfName": ztf_name}
+                "TNS init dict found",
+                extra={"tranId": tran_view.id, "ztfName": ztf_name},
             )
 
             # Three things we can find out:
             # - Did this AMPEL channel submit the transient (according to Journal)
             # - Did anyone submit a transient with this ZTF name?
             # - Did anyone submit a transient at this position?
 
@@ -368,37 +383,34 @@
                     self.logger.info("ztf submitted", extra={"ztfSubmitted": True})
                 else:
                     # add AT report
                     self.logger.info("Add TNS report list", extra={"id": tran_view.id})
                     atreports[tran_view.id] = atdict
                 continue
 
-
             # find the TNS name, either from the journal, from tran_names, or
             # from TNS itself. If new names are found, create a new JournalUpdate
             tns_name, tns_internals, jup = self.find_tns_name(tran_view, ra, dec)
-            self.logger.debug("TNS got %s internals %s" % (tns_name, tns_internals))
+            self.logger.debug(f"TNS got {tns_name} internals {tns_internals}")
 
             if tns_name is not None:
-
                 # Chech whether this ID has been submitted (note that we do not check
                 # whether the same candidate was submitted as different ZTF name) and
                 # depending on what's already on the TNS we can chose to submit or not
                 is_ztfsubmitted = ztf_name in tns_internals
-                if is_ztfsubmitted:
-                    # Already registered under this name. Only submit if we explicitly configured to do this
-                    if not self.resubmit_tns_ztf:
-                        self.logger.info(
-                            "ztf submitted",
-                            extra={
-                                "ztfSubmitted": is_ztfsubmitted,
-                                "tnsInternals": tns_internals,
-                            },
-                        )
-                        continue
+                # Already registered under this name. Only submit if we explicitly configured to do this
+                if is_ztfsubmitted and not self.resubmit_tns_ztf:
+                    self.logger.info(
+                        "ztf submitted",
+                        extra={
+                            "ztfSubmitted": is_ztfsubmitted,
+                            "tnsInternals": tns_internals,
+                        },
+                    )
+                    continue
 
                 # Also allow for the option to not submit if someone (anyone) already did this. Not sure why this would be a good idea.
                 if not is_ztfsubmitted and not self.resubmit_tns_nonztf:
                     self.logger.info(
                         "already in tns, skipping",
                         extra={
                             "ztfSubmitted": is_ztfsubmitted,
@@ -435,47 +447,47 @@
                     for i, report in enumerate(chunk)
                 }
             }
         ]
         tnsreplies = self.client.sendReports(atreportlist)
 
         # Now go and check and create journal updates for the cases where SN was added
-        for tran_id in atreports.keys():
+        for tran_id in atreports:
             ztf_name = to_ztf_id(tran_id)
-            if ztf_name not in tnsreplies.keys():
+            if ztf_name not in tnsreplies:
                 self.logger.info("No TNS add reply", extra={"tranId": tran_id})
                 continue
 
-
             # Create new journal entry assuming we submitted or found a name
-            if "TNSName" in tnsreplies[ztf_name][1].keys():
-                gen.send((
-                    tran_id,
-                    StockAttributes(
-                        journal=JournalAttributes(
-                            extra={
-                                "tnsName": tnsreplies[ztf_name][1]["TNSName"],
-                                "tnsInternal": ztf_name,
-                                "tnsSubmitresult": tnsreplies[ztf_name][0],
-                                "tnsSender": self.tns_api_key.get()["name"],
-                            },
+            if "TNSName" in tnsreplies[ztf_name][1]:
+                gen.send(
+                    (
+                        tran_id,
+                        StockAttributes(
+                            journal=JournalAttributes(
+                                extra={
+                                    "tnsName": tnsreplies[ztf_name][1]["TNSName"],
+                                    "tnsInternal": ztf_name,
+                                    "tnsSubmitresult": tnsreplies[ztf_name][0],
+                                    "tnsSender": self.tns_api_key.get()["name"],
+                                },
+                            ),
+                            tag="TNS_SUBMITTED",
+                            name=tnsreplies[ztf_name][1]["TNSName"],
                         ),
-                        tag="TNS_SUBMITTED",
-                        name=tnsreplies[ztf_name][1]["TNSName"],
                     )
-                ))
-
+                )
 
     def report_to_slack(self, atreports: dict[StockId, dict[str, Any]]) -> None:
         self.logger.info("done running T3")
 
         if not atreports:
             self.logger.info("No atreports collected.")
             return
-        elif self.slack_token is None:
+        if self.slack_token is None:
             return
 
         # TODO: to help debugging and verification, we post the collected atreports
         # to the slack, so that we can compare them with what JNo script is doing
         # ALL THE CONTENT OF THIS METHOD SHOULD GO AWAY AS SOON AS WE TRUST THIS T3
         self.logger.warn(
             "Posting collected ATreports to Slack. I'm still running as a test!"
@@ -487,19 +499,18 @@
 
         from slack_sdk import WebClient
         from slack_sdk.errors import SlackClientError
         from slack_sdk.web import SlackResponse
 
         sc = WebClient(token=self.slack_token.get())
 
-        tstamp = datetime.datetime.today().strftime("%Y-%m-%d-%X")
+        tstamp = datetime.datetime.now(tz=datetime.timezone.utc).strftime("%Y-%m-%d-%X")
         atlist = list(atreports.values())
         last = 0
         for ic, atrep in enumerate(chunks(atlist, self.max_slackmsg_size)):
-
             # add the atreport to a file
             self.logger.info("Posting chunk #%d" % ic)
             filename = "TNSTalker_DEBUG_%s_chunk%d.json" % (tstamp, ic)
             fbuffer = io.StringIO(filename)
             json.dump(atrep, fbuffer, indent=2)
 
             # upload the file with the at reports
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/TransientViewDumper.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientViewDumper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,119 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# File:                ampel/contrib/hu/t3/TransientInfoDumper.py
-# License:             BSD-3-Clause
-# Author:              Jakob van Santen <jakob.van.santen@desy.de>
-# Date:                15.08.2018
-# Last Modified Date:  15.08.2018
-# Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
-
-import uuid, requests
-from requests.auth import HTTPBasicAuth
+# File              : ampel/contrib/hu/t3/TransientInfoDumper.py
+# License           : BSD-3-Clause
+# Author            : Jakob van Santen <jakob.van.santen@desy.de>
+# Date              : 15.08.2018
+# Last Modified Date: 02.05.2023
+# Last Modified By  : Simeon Reusch <simeon.reusch@desy.de>
+import uuid
+from collections.abc import Generator
 from gzip import GzipFile
 from io import BytesIO
-from collections.abc import Generator
 from urllib.parse import ParseResult, urlparse, urlunparse
 from xml.etree import ElementTree
-from ampel.types import UBson, T3Send
-from ampel.abstract.AbsT3ReviewUnit import AbsT3ReviewUnit
+
+import requests
+from requests.auth import HTTPBasicAuth
+
+from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.secret.NamedSecret import NamedSecret
-from ampel.util.json import AmpelEncoder
-from ampel.view.SnapView import SnapView
-from ampel.view.T3Store import T3Store
+from ampel.struct.T3Store import T3Store
 from ampel.struct.UnitResult import UnitResult
+from ampel.types import T3Send, UBson
+from ampel.util.json import AmpelEncoder
+from ampel.view.TransientView import TransientView
 
 
 def strip_auth_from_url(url):
     try:
         auth = requests.utils.get_auth_from_url(url)
         scheme, netloc, path, params, query, fragment = urlparse(url)
-        netloc = netloc[(netloc.index("@") + 1):]
+        netloc = netloc[(netloc.index("@") + 1) :]
         url = urlunparse(ParseResult(scheme, netloc, path, params, query, fragment))
         return url, auth
     except KeyError:
         return url, None
 
 
 def strip_path_from_url(url):
-    scheme, netloc, path, params, query, fragment = urlparse(url)
-    return urlunparse(ParseResult(scheme, netloc, "/", None, None, None))
+    scheme, netloc, *_ = urlparse(url)
+    return urlunparse(ParseResult(scheme, netloc, "/", "", "", ""))
 
 
-class TransientViewDumper(AbsT3ReviewUnit):
+class TransientViewDumper(AbsPhotoT3Unit):
     """"""
 
     version = 0.1
-    resources = ("desycloud",)
+    require = ("desycloud",)
 
+    # If this is passed, files are always saved locally
     outputfile: None | str = None
+
     desycloud_auth: NamedSecret[dict] = NamedSecret(label="desycloud")
+    desycloud_folder: str = "dumps"
+    desycloud_filename: str = str(uuid.uuid1())
 
     def post_init(self) -> None:
         if not self.outputfile:
-            self.outfile = GzipFile(fileobj=BytesIO(), mode="w")
-            self.path = "/AMPEL/dumps/" + str(uuid.uuid1()) + ".json.gz"
+            self.buffer = BytesIO()
+            self.outfile = GzipFile(
+                filename=self.desycloud_filename + ".json",
+                fileobj=self.buffer,
+                mode="w",
+            )
+            self.path = (
+                f"/AMPEL/{self.desycloud_folder}/"
+                + self.desycloud_filename
+                + ".json.gz"
+            )
             self.session = requests.Session()
             assert self.resource
             self.webdav_base = self.resource["desycloud"]
             self.ocs_base = (
-                strip_path_from_url(self.resource["desycloud"]) +
-                "/ocs/v1.php/apps/files_sharing/api/v1"
+                strip_path_from_url(self.resource["desycloud"])
+                + "/ocs/v1.php/apps/files_sharing/api/v1"
             )
         else:
             self.outfile = GzipFile(self.outputfile + ".json.gz", mode="w")
+
         # don't bother preserving immutable types
         self.encoder = AmpelEncoder(lossy=True)
 
-
-    def process(self, transients: Generator[SnapView, T3Send, None], t3s: T3Store) -> UBson | UnitResult:
-
+    def process(
+        self, transients: Generator[TransientView, T3Send, None], t3s: T3Store
+    ) -> UBson | UnitResult:
         count = 0
-        for count, tran_view in enumerate(transients, 1):
+        for count, tran_view in enumerate(transients, 1):  # noqa: B007
+            print("TransientViewDumper:")
+            print(type(tran_view))
             self.outfile.write(self.encoder.encode(tran_view).encode("utf-8"))
             self.outfile.write(b"\n")
-
-        self.outfile.flush()
-        self.logger.info("Total number of transient printed: %i" % count)
+        self.outfile.close()
+        self.logger.info("Total number of transients written: %i" % count)
         if self.outputfile:
-            self.outfile.close()
             self.logger.info(self.outputfile + ".json.gz")
         else:
-            assert isinstance(self.outfile.fileobj, BytesIO)
-            mb = len(self.outfile.fileobj.getvalue()) / 2.0 ** 20
-            self.logger.info("{:.1f} MB of gzipped JSONy goodness".format(mb))
+            assert isinstance(self.buffer, BytesIO)
+            mb = len(self.buffer.getvalue()) / 2.0**20
+            self.logger.info(f"{mb:.1f} MB of gzipped JSONy goodness")
             auth = HTTPBasicAuth(**self.desycloud_auth.get())
+
             self.session.put(
                 self.webdav_base + self.path,
-                data=self.outfile.fileobj.getvalue(),
+                data=self.buffer.getvalue(),
                 auth=auth,
             ).raise_for_status()
             response = self.session.post(
                 self.ocs_base + "/shares",
                 data=dict(path=self.path, shareType=3),
                 auth=auth,
                 headers={"OCS-APIRequest": "true"},  # i'm not a CSRF attack, i swear
             )
-            self.outfile.close()
             if response.ok and (
                 element := ElementTree.fromstring(response.text).find("data/url")
             ):
                 if element.text:
                     self.logger.info(element.text)
             else:
                 response.raise_for_status()
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/VOEventPublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/VOEventPublisher.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,29 @@
 # File:                ampel/contrib/hu/t3/VOEventPublisher.py
 # License:             BSD-3-Clause
 # Author:              jno <jnordin@physik.hu-berlin.de>
 # Date:                26.09.2022
 # Last Modified Date:  26.09.2022
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
-from itertools import islice
-from typing import Iterable, TYPE_CHECKING, Literal, Any, Optional
-from collections.abc import Generator
 import datetime
+from collections.abc import Generator
+from typing import TYPE_CHECKING, Any, Literal
+
+import voeventparse as vp
 from astropy.time import Time
 
-from ampel.types import T3Send
-from ampel.struct.StockAttributes import StockAttributes
-from ampel.struct.JournalAttributes import JournalAttributes
-from ampel.enum.DocumentCode import DocumentCode
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
-from ampel.secret.NamedSecret import NamedSecret
-from ampel.view.TransientView import TransientView
-from ampel.view.T2DocView import T2DocView
-from ampel.view.T3Store import T3Store
+from ampel.struct.T3Store import T3Store
+from ampel.types import T3Send
 from ampel.util.mappings import get_by_path
-
-import voeventparse as vp
-
+from ampel.view.TransientView import TransientView
 
 if TYPE_CHECKING:
-    from ampel.content.JournalRecord import JournalRecord
+    pass
 
 
 class VOEventPublisher(AbsPhotoT3Unit):
     """
 
     Unit for creating a VOEvent pased on T2output and transient LightCurve.
 
@@ -42,53 +35,57 @@
                 'voevent_label_2' : ['other','path']
             },
         } }
 
     """
 
     # Characteristics of the VOEvent
-    voevent_ivorn: str = 'AMPEL/dev'
-    voevent_role: str = 'test'
-    voevent_stream: str = 'myFastDecliners'
+    voevent_ivorn: str = "AMPEL/dev"
+    voevent_role: str = "test"
+    voevent_stream: str = "myFastDecliners"
     vovent_streamid: int = 1
 
     # Selection of fields to output ("WHY?")
-    name_filter: dict[str, str] = {'ZTF name': 'ZTF', 'TNS ID': 'TNS'}
+    name_filter: dict[str, str] = {"ZTF name": "ZTF", "TNS ID": "TNS"}
     # Which datapoints to include in submission?
-    which_photometry: Literal['first','last'] = 'first'    #
+    which_photometry: Literal["first", "last"] = "first"  #
     # Schema for state dependent T2s (one row for each)
     why_schema: dict[str, Any]
     # Temporary file name
-    fname = 'voevent.xml'
+    fname = "voevent.xml"
 
-    def process(self, gen: Generator[TransientView, T3Send, None],
-                t3s: Optional[T3Store] = None) -> None:
+    def process(
+        self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None
+    ) -> None:
         """
         Loop through provided TransientViews and extract data according to the
         configured schema.
         """
 
         for k, tran_view in enumerate(gen, 1):
-
             # Chategorized by stock (internal ampel ID) and channel
             stock = tran_view.id
             print(stock)
             assert tran_view.stock is not None
             channels = tran_view.stock.get("channel")
             assert channels is not None
-            channel = channels[0] if isinstance(channels, (list, tuple)) and len(channels) == 1 else '/'.join([str(c) for c in channels])
+            channel = (
+                channels[0]
+                if isinstance(channels, list | tuple) and len(channels) == 1
+                else "/".join([str(c) for c in channels])
+            )
 
             # Get photometry from first|last visit
             dps = tran_view.get_photopoints()
             assert dps is not None
-            dps = sorted(dps, key=lambda d: d['body']['jd'])
-            if self.which_photometry=='first':
-                dp = dps[0]['body']
-            elif self.which_photometry=='last':
-                dp = dps[-1]['body']
+            dps = sorted(dps, key=lambda d: d["body"]["jd"])
+            if self.which_photometry == "first":
+                dp = dps[0]["body"]
+            elif self.which_photometry == "last":
+                dp = dps[-1]["body"]
 
             # Collect t2 information.
             # Only uses latest state. See TransientTablePublisher for
             # possible extension to state.
             t2dict: dict[str, Any] = {}
             for t2unit, table_entries in self.why_schema.items():
                 for t2res in tran_view.get_t2_views(unit=t2unit):
@@ -97,44 +94,50 @@
                         assert isinstance((body := t2res.body[-1]), dict)
                         if result := get_by_path(body, path):
                             t2dict[label] = result
             if len(t2dict.keys()) == 0:
                 continue
 
             # Generate VOEvent
-            v = vp.Voevent(stream=self.voevent_stream, stream_id=self.vovent_streamid,
-                       role=self.voevent_role)
-            vp.set_who(v, datetime.datetime.utcnow())
-            vp.set_author(v, title="Results from {} channel".format(channel),
-                      contactName="ampel-info@desy.de")
+            v = vp.Voevent(
+                stream=self.voevent_stream,
+                stream_id=self.vovent_streamid,
+                role=self.voevent_role,
+            )
+            vp.set_who(v, datetime.datetime.now(tz=datetime.timezone.utc))
+            vp.set_author(
+                v,
+                title=f"Results from {channel} channel",
+                contactName="ampel-info@desy.de",
+            )
             v.Description = "Generated through https://github.com/AmpelProject/Ampel-HU-astro/ampel/contrib/hu/t3/VOEventPublisher.py"
 
-            v.What.append(vp.Param(name="mag", value=dp['magpsf'], ucd="phot.mag"))
+            v.What.append(vp.Param(name="mag", value=dp["magpsf"], ucd="phot.mag"))
 
-            dt = Time(dp['jd'], format='jd').to_datetime()
+            dt = Time(dp["jd"], format="jd").to_datetime()
             dt = dt.replace(tzinfo=datetime.timezone.utc)
 
-            vp.add_where_when(v,
-                coords=vp.Position2D(ra=dp['ra'], dec=dp['dec'], err=0, units='deg',
-                                                system=vp.definitions.sky_coord_system.utc_fk5_geo),
-                           obs_time=dt,
-                           observatory_location="Palomar P48 / ZTF camera")
+            vp.add_where_when(
+                v,
+                coords=vp.Position2D(
+                    ra=dp["ra"],
+                    dec=dp["dec"],
+                    err=0,
+                    units="deg",
+                    system=vp.definitions.sky_coord_system.utc_fk5_geo,
+                ),
+                obs_time=dt,
+                observatory_location="Palomar P48 / ZTF camera",
+            )
 
             # Add collected results
-            vp.add_how( v, descriptions = [
-                    "{}: {}".format(k,v) for k, v in t2dict.items()
-                ]
-                )
+            vp.add_how(v, descriptions=[f"{k}: {v}" for k, v in t2dict.items()])
             vp.add_why(v)
             v.Why.Description = "Selected based on AMPEL T2s: {}".format(
-                ' '.join(self.why_schema.keys() ) )
+                " ".join(self.why_schema.keys())
+            )
 
-            with open(self.fname, 'wb') as fw:
+            with open(self.fname, "wb") as fw:
                 vp.dump(v, fw)
-            with open(self.fname, 'r') as fr:
+            with open(self.fname) as fr:
                 for l in fr.readlines():
                     print(l.rstrip())
-
-
-
-
-        return None
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/ampel_tns.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ampel_tns.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 import json
 import re
 import time
 from typing import Any
 
 from requests.models import Response
+from requests_toolbelt.sessions import BaseUrlSession
 
 from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
 from ampel.protocol.LoggerProtocol import LoggerProtocol
-from requests_toolbelt.sessions import BaseUrlSession
 
 TNSFILTERID = {1: "110", 2: "111", 3: "112"}
 AT_REPORT_FORM = "bulk-report"
 AT_REPORT_REPLY = "bulk-report-reply"
 TNS_ARCHIVE = {"OTHER": "0", "SDSS": "1", "DSS": "2"}
 TNS_BASE_URL_SANDBOX = "https://sandbox.wis-tns.org/api/"
 TNS_BASE_URL_REAL = "https://www.wis-tns.org/api/"
@@ -36,49 +36,54 @@
     403: "Error 403: Forbidden: The request is understood, but it has been refused. An accompanying error message will explain why",
     404: "Error 404: Not Found: The URI requested is invalid or the resource requested, such as a category, does not exists.",
     500: "Error 500: Internal Server Error: Something is broken.",
     503: "Error 503: Service Unavailable.",
     429: "Error 429: Rate Limit Exceeded.",
 }
 
+
 class TNSSession(BaseUrlSession):
     def __init__(self, token: TNSToken, baseURL: str = TNS_BASE_URL_REAL) -> None:
         self.token = token
         super().__init__(baseURL)
-        self.headers["User-Agent"] = (
-            "tns_marker"
-            + json.dumps(
-                {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
-            )
+        self.headers["User-Agent"] = "tns_marker" + json.dumps(
+            {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
         )
 
-    def post(self, method: str, payload: str | dict[str,Any], payload_key="data", **kwargs) -> Response:
+    def post(
+        self, method: str, payload: str | dict[str, Any], payload_key="data", **kwargs
+    ) -> Response:
         for _ in range(10):
-            if (response := super().post(
-                method,
-                files=[
-                    ("api_key", (None, self.token.api_key)),
-                    (payload_key, (None, json.dumps(payload)))
-                ],
-                **kwargs
-            )).status_code != 429:
+            if (
+                response := super().post(
+                    method,
+                    files=[
+                        ("api_key", (None, self.token.api_key)),
+                        (payload_key, (None, json.dumps(payload))),
+                    ],
+                    **kwargs,
+                )
+            ).status_code != 429:
                 return response
             # back off according to rate-limit headers (see https://www.wis-tns.org/content/tns-newsfeed#comment-wrapper-26286)
-            delay = response.headers["x-cone-rate-limit-reset" if response.url.endswith('search') else "x-rate-limit-reset"]
+            delay = response.headers[
+                "x-cone-rate-limit-reset"
+                if response.url.endswith("search")
+                else "x-rate-limit-reset"
+            ]
             time.sleep(int(delay))
-        else:
-            response.raise_for_status()
-            # unreachable
-            return None # type: ignore[return-value]
+        response.raise_for_status()
+        # unreachable
+        return None  # type: ignore[return-value]
 
 
 class TNSClient:
     """Send Bulk TNS Request."""
 
-    def __init__(self, baseURL, logger: LoggerProtocol, token: TNSToken, options={}):
+    def __init__(self, baseURL, logger: LoggerProtocol, token: TNSToken):
         """
         :param baseURL: Base URL of the TNS API
         :param options: (Default value = {})
         """
 
         self.logger = logger
         self.session = TNSSession(token, baseURL)
@@ -87,15 +92,15 @@
         """
         Send JSON response given requests object. Should be a python dict.
 
         :param r: requests object - the response we got back from the server
         :return d: json response converted to python dict
         """
 
-        d : dict[str, Any] = {}
+        d: dict[str, Any] = {}
         # What response did we get?
         message = None
         status = r.status_code
 
         if status != 200:
             message = httpErrors.get(status, f"Error {status}: Undocumented error")
 
@@ -104,21 +109,20 @@
             return d
 
         # Did we get a JSON object?
         try:
             d = r.json()
         except ValueError as e:
             self.logger.error("TNS bulk submit", exc_info=e)
-            d = {}
-            return d
+            return {}
 
         # If so, what error messages if any did we get?
         self.logger.info(json.dumps(d, indent=4, sort_keys=True))
 
-        if "id_code" in d.keys() and "id_message" in d.keys() and d["id_code"] != 200:
+        if "id_code" in d and "id_message" in d and d["id_code"] != 200:
             self.logger.info(
                 "TNS bulk submit: Bad response: code = %d, error = '%s'"
                 % (d["id_code"], d["id_message"])
             )
         return d
 
     def sendBulkReport(self, options) -> dict:
@@ -129,15 +133,15 @@
         # The requests.post method needs to receive a "files" entry, not "data".  And the "files"
         # entry needs to be a dictionary of tuples.  The first value of the tuple is None.
         self.logger.info("TNS bulk submit: " + "sending request")
         r = self.session.post(AT_REPORT_FORM, options, timeout=300)
         # Construct the JSON response and return it.
         self.logger.info("TNS bulk submit: " + "got response (or timed out)")
         return self.jsonResponse(r)
-    
+
     def addBulkReport(self, report):
         """
         Send the report to the TNS
 
         :return reportId: TNS report ID
 
         """
@@ -152,29 +156,28 @@
                 logger.info("TNS bulk submit: successful with ID %s" % (reportId))
             except ValueError:
                 logger.error("Empty response. Something went wrong. Is the API Key OK?")
             except KeyError:
                 logger.error("Cannot find the data key. Something is wrong.")
 
         return reportId
-    
+
     def sendReports(self, reports: list[dict]):
         """
         Based on a lists of reportlists, send to TNS.
         Return results for journal entries
         """
 
         # Submit to TNS
         MAX_LOOP = 25
         SLEEP = 2
 
         logger = self.logger
         reportresult = {}
         for atreport in reports:
-
             # Submit a report
             for _ in range(MAX_LOOP):
                 reportid = self.addBulkReport(atreport)
                 if reportid:
                     logger.info("TNS report ID %s" % (reportid))
                     break
                 time.sleep(SLEEP)
@@ -193,61 +196,60 @@
                 continue
 
             # Check whether request was bad. In this case TNS looks to return a list with dicts
             # of failed objects which does not correspond to the order of input atdicts.
             # In any case, nothing in the submit is posted.
             # Hence only checking first element
             bad_request = None
-            for key_atprop in ['ra','decl','discovery_datetime']:
-                if key_atprop in response[0].keys():
+            for key_atprop in ["ra", "decl", "discovery_datetime"]:
+                if key_atprop in response[0]:
                     try:
                         bad_request = response[0][key_atprop]["value"]["5"]["message"]
                         break
                     except KeyError:
                         pass
             if bad_request is not None:
-                logger.info( bad_request )
+                logger.info(bad_request)
                 continue
 
-
-
-
             # Parse reply for evaluation
             for k, v in atreport["at_report"].items():
-                if "100" in response[k].keys():
+                if "100" in response[k]:
                     logger.info(
                         "TNS Inserted with name %s" % (response[k]["100"]["objname"])
                     )
                     reportresult[v["internal_name"]] = [
                         "TNS inserted",
                         {"TNSName": response[k]["100"]["objname"]},
                     ]
-                elif "101" in response[k].keys():
+                elif "101" in response[k]:
                     logger.info(
-                        "Already existing with name %s" % (response[k]["101"]["objname"])
+                        "Already existing with name %s"
+                        % (response[k]["101"]["objname"])
                     )
                     reportresult[v["internal_name"]] = [
                         "TNS pre-existing",
                         {"TNSName": response[k]["101"]["objname"]},
                     ]
-                    
 
         return reportresult
 
     def _bulkReportReply(self, report_id: str) -> dict[str, Any]:
         """
         Get the report back from the TNS
 
         :param options: dict containing the report ID
         :return: dict
 
         """
         self.logger.info("TNS bulk submit: " + "looking for reply report")
         # every TNS endpoint wraps its arguments in `data`, except bulk-report-reply
-        r = self.session.post(AT_REPORT_REPLY, report_id, payload_key="report_id", timeout=300)
+        r = self.session.post(
+            AT_REPORT_REPLY, report_id, payload_key="report_id", timeout=300
+        )
         self.logger.info("TNS bulk submit: " + "got report (or timed out)")
         return self.jsonResponse(r)
 
     def getBulkReportReply(self, reportId):
         """
         Get the TNS response for the specified report ID
         :param tnsApiKey: TNS API Key
@@ -256,89 +258,95 @@
         """
 
         logger = self.logger
         reply = self._bulkReportReply(reportId)
 
         response = None
         # reply should be a dict
-        if reply and "id_code" in reply.keys() and reply["id_code"] == 404:
+        if reply and "id_code" in reply and reply["id_code"] == 404:
             logger.warn(
                 f"TNS bulk submit {reportId}: Unknown report. "
                 f"Perhaps the report has not yet been processed."
             )
 
-        if reply and "id_code" in reply.keys() and reply["id_code"] == 200:
+        if reply and "id_code" in reply and reply["id_code"] == 200:
             try:
                 response = reply["data"]["feedback"]["at_report"]
             except KeyError:
-                logger.error("TNS bulk submit: cannot find the response feedback payload.")
+                logger.error(
+                    "TNS bulk submit: cannot find the response feedback payload."
+                )
 
         # This is a bad request. Still propagate the response for analysis.
-        if reply and "id_code" in reply.keys() and reply["id_code"] == 400:
+        if reply and "id_code" in reply and reply["id_code"] == 400:
             try:
                 response = reply["data"]["feedback"]["at_report"]
             except KeyError:
-                logger.error("TNS bulk submit: cannot find the response feedback payload.")
-
+                logger.error(
+                    "TNS bulk submit: cannot find the response feedback payload."
+                )
 
         logger.info(f"TNS bulk submit: got response {response}")
 
         return response
-    
+
     def getInternalName(self, tns_name: str):
         """
         formerly tnsInternal
         """
 
         response = self.session.post(
-            "get/object",
-            {"objname": tns_name, "photometry": 0, "spectra": 0}
+            "get/object", {"objname": tns_name, "photometry": 0, "spectra": 0}
         )
         parsed = self.jsonResponse(response)
 
         if parsed["data"]["reply"]["internal_names"] is None:
             return [], "No internal TNS name"
 
         return parsed["data"]["reply"]["internal_names"], "Got internal name response"
-    
-    def search(self, ra: float, dec: float, matchradius: float=5.) -> tuple[list[str], str]:
+
+    def search(
+        self, ra: float, dec: float, matchradius: float = 5.0
+    ) -> tuple[list[str], str]:
         """
         formerly tnsName
         """
         r = self.session.post(
             "get/search",
-            {"ra": ra, "dec": dec, "radius": matchradius, "units": "arcsec"}
+            {"ra": ra, "dec": dec, "radius": matchradius, "units": "arcsec"},
         )
         parsed = self.jsonResponse(r)
 
         try:
             tnsnames = [v["prefix"] + v["objname"] for v in parsed["data"]["reply"]]
         except KeyError:
             return [], "Error: No TNS names in response"
 
         return tnsnames, "Found TNS name(s)"
-    
-    def getNames(self, ra: float, dec: float, matchradius: float=5.):
+
+    def getNames(self, ra: float, dec: float, matchradius: float = 5.0):
         """
         Get names of the first TNS object at location
 
         formerly get_tnsname
         """
         logger = self.logger
         # Look for TNS name at the coordinate of the transient
         tnsnames, runstatus = self.search(ra, dec, matchradius)
         if re.match("Error", runstatus):
             logger.info("TNS get error", extra={"tns_request": runstatus})
             return None, []
         if len(tnsnames) >= 1:
             tns_name = tnsnames[0]
             if len(tnsnames) > 1:
-                logger.debug("Multipe TNS names, choosing first", extra={"tns_names": tnsnames})
+                logger.debug(
+                    "Multipe TNS names, choosing first", extra={"tns_names": tnsnames}
+                )
         else:
             # No TNS name, then no need to look for internals
             return None, None
         logger.info("TNS get cand id", extra={"tns_name": tns_name})
 
         # Look for internal name (note that we skip the prefix)
         internal_names, *_ = self.getInternalName(tns_name[2:])
-        
+
         return tns_name, internal_names
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # License:             BSD-3-Clause
 # Author:              Jakob van Santen <jakob.van.santen@desy.de>
 # Date:                03.11.2020
 # Date:                03.11.2020
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 
-from functools import cached_property
-from typing import Any, Tuple
 from collections.abc import Iterable
+from functools import cached_property
+from typing import Any
 
 from pymongo import MongoClient
 
+from ampel.abstract.AbsBufferComplement import AbsBufferComplement
 from ampel.base.decorator import abstractmethod
-from ampel.base.AmpelBaseModel import AmpelBaseModel
-from ampel.struct.AmpelBuffer import AmpelBuffer
 from ampel.secret.NamedSecret import NamedSecret
-from ampel.abstract.AbsBufferComplement import AbsBufferComplement
-from ampel.view.T3Store import T3Store
+from ampel.struct.AmpelBuffer import AmpelBuffer
+from ampel.struct.T3Store import T3Store
 
 
 class BaseCatalogRecordComplementer(AbsBufferComplement, abstract=True):
     """
     Add entries from an extcats catalog to transients, matched by canonical
     name. This is distinct from, and much cheaper than, general catalog
     matching, where entries are matched by cone search, and can be used for
@@ -31,15 +30,15 @@
     """
 
     auth: NamedSecret[dict] = NamedSecret(label="extcats/reader")
 
     @cached_property
     def mongo_client(self):
         return MongoClient(
-            self.context.config.get(f"resource.extcats", str), **self.auth.get()
+            self.context.config.get("resource.extcats", str), **self.auth.get()
         )
 
     @abstractmethod
     def get_catalog_item(self, names: tuple[str, ...]) -> None | dict[str, Any]:
         """Get catalog entry associated with the stock name"""
         ...
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSClient.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 import asyncio
 import json
 import sys
 import traceback
 from functools import partial
-from typing import Dict
 
 import aiohttp
 import backoff
-from aiohttp import ClientSession, ClientTimeout
+from aiohttp import ClientSession
 from aiohttp.client_exceptions import (
     ClientConnectionError,
     ClientConnectorError,
     ClientResponseError,
     ServerDisconnectedError,
 )
 
@@ -58,16 +57,15 @@
                         else 0,
                         int(resp.headers.get("x-rate-limit-reset", 0)),
                         1,
                     )
                 )
                 await asyncio.sleep(wait)
                 continue
-            else:
-                break
+            break
         resp.raise_for_status()
         return await resp.json()
 
 
 class TNSClient:
     def __init__(self, token: TNSToken, timeout, maxParallelRequests, logger):
         self.token = token
@@ -88,35 +86,40 @@
             on_giveup=self._on_giveup,
             on_backoff=self._on_backoff,
             max_time=timeout,
         )(tns_post)
 
     def _on_backoff(self, details):
         exc_typ, exc, _ = sys.exc_info()
-        if exc is not None:
-            exc = traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+        err = (
+            traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+            if exc
+            else None
+        )
         self.logger.warn(
             "backoff",
-            extra={"exc": exc, "wait": details["wait"], "tries": details["tries"]},
+            extra={"exc": err, "wait": details["wait"], "tries": details["tries"]},
         )
 
     def _on_giveup(self, details):
         exc_typ, exc, _ = sys.exc_info()
-        if exc is not None:
-            exc = traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
-        self.logger.warn("gave up", extra={"exc": exc, "tries": details["tries"]})
+        err = (
+            traceback.format_exception_only(exc_typ, exc)[-1].rstrip("\n")
+            if exc
+            else None
+        )
+        self.logger.warn("gave up", extra={"exc": err, "tries": details["tries"]})
 
     @staticmethod
     def is_permanent_error(exc):
         if isinstance(exc, ClientResponseError):
             return exc.code not in {500, 429}
-        else:
-            return False
+        return False
 
-    async def search(self, exclude=set(), **params):
+    async def search(self, *, exclude: None | set[str] = None, **params):
         semaphore = asyncio.Semaphore(self.maxParallelRequests)
         async with ClientSession(
             headers={
                 "User-Agent": "tns_marker"
                 + json.dumps(
                     {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
                 )
@@ -138,9 +141,9 @@
             )
             for fut in asyncio.as_completed(tasks):
                 item = await fut
                 yield item["data"]["reply"]
 
     async def get(self, session, semaphore, objname):
         return await self.tns_post(
-            session, semaphore, "get/object", self.apiKey, {"objname": objname}
+            session, semaphore, "get/object", self.token, {"objname": objname}
         )
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSMirrorDB.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSMirrorDB.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from contextlib import suppress
 
 import numpy
 from astropy.time import Time
 from pymongo import GEOSPHERE, MongoClient, UpdateOne
 from pymongo.errors import BulkWriteError, OperationFailure
 
 from ampel.contrib.hu.t3.tns.TNSName import TNSName
@@ -20,15 +21,15 @@
             "key": "pos",
             "is_indexed": "true",
             "pos_format": "geoJSON",
             "type": "sphere2d",
         }
         try:
             meta.update_one({}, {"$set": entry}, upsert=True)
-            self.collection.ensure_index([("pos", GEOSPHERE)])
+            self.collection.create_index([("pos", GEOSPHERE)])
         except OperationFailure:
             ...
         if logger:
             self.logger = logger
         else:
             self.logger = log
 
@@ -36,29 +37,29 @@
         """
         :param docs: TNS get/object results
         """
         # NB: bulk_write() an empty list raises InvalidOperation
         if not docs:
             return
 
-        ops = []
-        for doc in docs:
-            doc = self.apply_schema(doc)
-            ops.append(UpdateOne({"_id": doc["_id"]}, {"$set": doc}, upsert=True))
+        ops = [
+            UpdateOne({"_id": doc["_id"]}, {"$set": doc}, upsert=True)
+            for doc in map(self.apply_schema, docs)
+        ]
 
         try:
             result = self.collection.bulk_write(ops, ordered=False)
             self.logger.info(
                 "update TNS mirror",
                 extra={
                     "inserted": result.upserted_count,
                     "modified": result.modified_count,
                 },
             )
-        except BulkWriteError as bwe:
+        except BulkWriteError:
             pass
 
     def get_names_for_location(self, ra, dec, radius):
         ra = ra if ra < 180.0 else ra - 360.0
         cursor = self.collection.find(
             {
                 "pos": {
@@ -73,18 +74,16 @@
     @classmethod
     def apply_schema(cls, doc):
         # convert name to integer for more efficient indexing
         doc["_id"] = int(TNSName.from_str(doc["objname"]))
         doc["pos"] = cls.geojson_key(doc.pop("radeg"), doc.pop("decdeg"))
         for k in ["ra", "dec"]:
             del doc[k]
-        try:
+        with suppress(ValueError):
             doc["discoverydate"] = Time(doc["discoverydate"]).datetime
-        except:
-            pass
         return doc
 
     @staticmethod
     def geojson_key(ra, dec):
         # geoJSON needs longitude between -180 and +180
         ra = ra if ra < 180.0 else ra - 360.0
         return {"type": "Point", "coordinates": [ra, dec]}
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/t3/tns/TNSName.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSName.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,53 @@
 # Author:              Jakob van Santen <jakob.van.santen@desy.de>
 # Date:                04.11.2019
 # Last Modified Date:  04.11.2019
 # Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
 
 import math
 
+
 class TNSName:
     """
     TNS objects are numbered with a variable-length, 1-indexed letter code,
     e.g. 2019a represents (2019,1), while 2019aa represents (2019,27)
     """
-    __slots__ = ('year', 'number')
+
+    __slots__ = ("year", "number")
     BASE = 26
-    def __init__(self, year : int, number : int):
+
+    def __init__(self, year: int, number: int):
         self.year = year
         self.number = number
+
     @classmethod
     def from_str(cls, name):
         assert 0 < len(name) - 4 < 11
         year = int(name[:4])
         number = 0
-        for i,c in enumerate(reversed(name[4:])):
-            number += (ord(c.lower())-ord('a')+1) * (cls.BASE**i)
+        for i, c in enumerate(reversed(name[4:])):
+            number += (ord(c.lower()) - ord("a") + 1) * (cls.BASE**i)
         return cls(year, number)
+
     @classmethod
     def from_index(cls, packed):
-        return cls((packed >> 56) + 1970, packed & ((1<<56)-1))
+        return cls((packed >> 56) + 1970, packed & ((1 << 56) - 1))
+
     def __int__(self):
         """
         Pack year into top 8 bits, intra-year number into bottom 56
         """
         return ((self.year - 1970) << 56) + self.number
+
     def __str__(self):
         name = str(self.year)
         if self.number <= 0:
             return name
         # find number of digits to emit
-        digits = int(math.ceil(math.log(self.number)/math.log(self.BASE)))
-        for i in range(digits-1, -1, -1):
+        digits = int(math.ceil(math.log(self.number) / math.log(self.BASE)))
+        for i in range(digits - 1, -1, -1):
             unit = self.BASE**i
-            name += chr(ord('a') + (self.number % (unit*self.BASE))//unit - 1)
+            name += chr(ord("a") + (self.number % (unit * self.BASE)) // unit - 1)
         return name
+
     def __repr__(self):
-        return "TNSName({},{})".format(self.year, self.number)
+        return f"TNSName({self.year},{self.number})"
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_slackpublisher.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_slackpublisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-from ampel.view.T2DocView import T2DocView, TYPE_STATE_T2
-from ampel.view.T3Store import T3Store
+import csv
+from io import StringIO
+
 import pytest
-from ampel.log.AmpelLogger import AmpelLogger
-from ampel.contrib.hu.t3.SlackSummaryPublisher import SlackSummaryPublisher
-from ampel.secret.NamedSecret import NamedSecret
+import requests
+from slack_sdk import WebClient
 
-from ampel.content.StockDocument import StockDocument
 from ampel.content.DataPoint import DataPoint
-from ampel.content.T2Document import T2Document
+from ampel.content.StockDocument import StockDocument
+from ampel.contrib.hu.t3.SlackSummaryPublisher import SlackSummaryPublisher
 from ampel.enum.DocumentCode import DocumentCode
+from ampel.log.AmpelLogger import AmpelLogger
+from ampel.secret.NamedSecret import NamedSecret
+from ampel.struct.T3Store import T3Store
+from ampel.view.T2DocView import TYPE_STATE_T2, T2DocView
 from ampel.view.TransientView import TransientView
 from ampel.ztf.util.ZTFIdMapper import to_ampel_id
 
-import requests
-from slack_sdk import WebClient
-import csv
-from io import StringIO
-
 
-@pytest.fixture
+@pytest.fixture()
 def t3_transient_views() -> list[TransientView]:
     return [
         TransientView(
             id=(stock_id := to_ampel_id(name)),
             stock=StockDocument(
                 {"stock": stock_id, "channel": ["CHANNYCHAN"]},
             ),
-            t0=[DataPoint(id=i, stock=stock_id, body={}, channel=[], meta=[]) for i in range(10)],
+            t0=[
+                DataPoint(id=i, stock=stock_id, body={}, channel=[], meta=[])
+                for i in range(10)
+            ],
             t2=[
                 T2DocView(
                     stock=stock_id,
                     link=0,
                     tag=[],
                     code=DocumentCode.OK,
                     meta=[{"code": DocumentCode.OK, "tier": 2}],
                     t2_type=TYPE_STATE_T2,
                     unit="T2LightCurveSummary",
+                    confid=None,
                     body=[{"len": 10}],
                 ),
                 T2DocView(
                     stock=stock_id,
                     link=0,
                     tag=[],
                     code=DocumentCode.OK,
                     meta=[{"code": DocumentCode.OK, "tier": 2}],
                     t2_type=TYPE_STATE_T2,
                     unit="T2SNCosmo",
+                    confid=None,
                     body=[
                         {
                             "model": "salt2",
                             "sncosmo_info": {"ndof": 42},
                             "fit_results": {"t0": 13480238.2309423},
                         }
                     ],
@@ -61,15 +65,14 @@
             "ZTF20abthfto",
             "ZTF21aabltvh",
         ]
     ]
 
 
 def test_slacksummary(t3_transient_views: list[TransientView], mocker):
-
     unit = SlackSummaryPublisher(
         **{
             "cols": [
                 "ztf_name",
                 "ra",
                 "dec",
                 "magpsf",
@@ -93,27 +96,27 @@
 
     assert len(t3_transient_views) < unit.excitement["Low"], "Small number passed"
 
     # intercept Slack API calls
     mocker.patch("requests.post")
     mocker.patch("slack_sdk.WebClient.api_call")
 
-    unit.process(iter(t3_transient_views), T3Store()) # type: ignore[arg-type]
+    unit.process(iter(t3_transient_views), T3Store())  # type: ignore[arg-type]
 
     api_call = WebClient.api_call
-    api_call.assert_called_once() # type: ignore[attr-defined]
+    api_call.assert_called_once()  # type: ignore[attr-defined]
     assert (
-        "MEH!" in api_call.call_args[1]["json"]["text"] # type: ignore[attr-defined]
+        "MEH!" in api_call.call_args[1]["json"]["text"]  # type: ignore[attr-defined]
     ), "Text matches number of transients selected"
 
-    requests.post.assert_called() # type: ignore[attr-defined]
-    assert len(requests.post.call_args_list) == 2, "2 explicit requests issued" # type: ignore[attr-defined]
+    requests.post.assert_called()  # type: ignore[attr-defined]
+    assert len(requests.post.call_args_list) == 2, "2 explicit requests issued"  # type: ignore[attr-defined]
 
     # Verify summary
-    content = requests.post.call_args_list[0][1]["files"]["file"] # type: ignore[attr-defined]
+    content = requests.post.call_args_list[0][1]["files"]["file"]  # type: ignore[attr-defined]
     with StringIO(content) as f:
         reader = csv.DictReader(f)
         rows = list(reader)
 
     # verify that T2 information is in summary
     t2s = set(t2.unit for tv in t3_transient_views for t2 in (tv.t2 or []))
     assert len(t2s) > 0
@@ -123,13 +126,13 @@
     assert reader.fieldnames
     for key in ["T2-model", "T2-sncosmo_info_ndof", "T2-fit_results_t0"]:
         assert key in reader.fieldnames
 
     assert len(rows) == len(t3_transient_views), "1 row per transient"
 
     # Verify photometry dump
-    content = requests.post.call_args_list[1][1]["files"]["file"] # type: ignore[attr-defined]
+    content = requests.post.call_args_list[1][1]["files"]["file"]  # type: ignore[attr-defined]
     with StringIO(content) as f:
         rows = list(csv.DictReader(f))
-    assert (
-        len(rows) == sum(len(v.t0 or []) for v in t3_transient_views)
+    assert len(rows) == sum(
+        len(v.t0 or []) for v in t3_transient_views
     ), "1 row per photopoint"
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_t2brightsnprob.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_t2brightsnprob.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from os.path import dirname, join
 
 import pytest
 
+from ampel.content.DataPoint import DataPoint
 from ampel.contrib.hu.t2.T2BrightSNProb import T2BrightSNProb
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.view.LightCurve import LightCurve
-from ampel.content.DataPoint import DataPoint
 from ampel.ztf.util.ZTFIdMapper import to_ampel_id
 
 _ampel_flags = {
     0: "ZTF",
 }
 
 _ampel_photo_flags = _ampel_flags | {
@@ -26,19 +26,19 @@
 
 def _to_datapoint(d):
     return DataPoint(
         id=d.pop("_id"),
         body=d,
         tag=[_ampel_photo_flags[f] for f in d.pop("alTags") if f in _ampel_photo_flags],
         channel=[],
-        meta=[]
+        meta=[],
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def lightcurve() -> LightCurve:
     with open(join(dirname(__file__), "lightcurve.ZTF18abmjvpb.json")) as f:
         blob = json.load(f)
         return LightCurve(
             compound_id=0,
             stock_id=to_ampel_id("ZTF18abmjvpb"),
             photopoints=[
@@ -59,15 +59,15 @@
     }
     assert {k: v for k, v in left.items() if v is not None} == pytest.approx(
         {k: v for k, v in right.items() if v is not None}
     )
 
 
 def test_t2brightsnprob(lightcurve):
-    monitor = T2BrightSNProb(logger=AmpelLogger.get_logger())
+    monitor = T2BrightSNProb(logger=AmpelLogger.get_logger())  # type: ignore[call-arg]
     monitor.post_init()
     assert_equivalent(
         monitor.process(lightcurve),
         {
             "cut_pp": 0,
             "jd_det": 2458343.6521875,
             "jd_last": 2458373.62625,
```

### Comparing `ampel_hu_astro-0.8.3a9/ampel/contrib/hu/test/test_tnstalker.py` & `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_tnstalker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from os import environ
 
 import pytest
 
 from ampel.contrib.hu.t3.tns.TNSToken import TNSToken
-from ampel.contrib.hu.t3.TNSTalker import TNSClient, TNS_BASE_URL_SANDBOX
+from ampel.contrib.hu.t3.TNSTalker import TNS_BASE_URL_SANDBOX, TNSClient
 from ampel.log.AmpelLogger import AmpelLogger
 
-@pytest.fixture
+
+@pytest.fixture()
 def tns_token():
     if not (api_key := environ.get("TNS_API_KEY")):
         raise pytest.skip("Test requires env var TNS_API_KEY")
     return TNSToken(
-        **{
-            "id": 59228,
-            "name": "ZTF_AMPEL_COMPLETE",
-            "api_key": api_key,
-        }
+        id=59228,
+        name="ZTF_AMPEL_COMPLETE",
+        api_key=api_key,
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def test_client(tns_token):
-
     return TNSClient(TNS_BASE_URL_SANDBOX, AmpelLogger.get_logger(), tns_token)
 
 
 def test_tnsclient(test_client):
     assert test_client.getInternalName("2018cow") == (
         "ATLAS18qqn, ZTF18abcfcoo, Gaia18bqa",
         "Got internal name response",
@@ -36,34 +34,37 @@
     )
     assert test_client.getNames(244.000917, 22.268031) == (
         "SN2018cow",
         "ATLAS18qqn, ZTF18abcfcoo, Gaia18bqa",
     )
 
 
-def test_tnsclient_backoff(test_client):
+def test_tnsclient_backoff(test_client: TNSClient):
     import logging
 
     logging.basicConfig()
     for _ in range(12):
         assert test_client.search(244.000917, 22.268031) == (
             ["SN2018cow"],
             "Found TNS name(s)",
         )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_tnsclient_backoff_async(tns_token):
-    from ampel.contrib.hu.t3.tns import TNSClient
+    from ampel.contrib.hu.t3.tns.TNSClient import TNSClient as TNSMirrorClient
 
-    client = TNSClient(
+    client = TNSMirrorClient(
         tns_token, timeout=120, maxParallelRequests=1, logger=AmpelLogger.get_logger()
     )
     ra, dec, matchradius = 244.000917, 22.268031, 5.0
     for _ in range(12):
         hits = [
             hit
             async for hit in client.search(
-                **{"ra": ra, "dec": dec, "radius": matchradius, "units": "arcsec"}
+                ra=ra,
+                dec=dec,
+                radius=matchradius,
+                units="arcsec",
             )
         ]
         assert hits
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/alias.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/alias.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_10.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_10.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_GP_10
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_public
 t0_filter:
   unit: DecentFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_16.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_16.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_GP_16
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_public
 t0_filter:
   unit: DecentFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_59.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_59.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_GP_59
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_public
 t0_filter:
   unit: DecentFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_GP_SINGLE
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: false
 template: ztf_uw_public
 t0_filter:
   unit: XShooterFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_NEARBY_CLUSTERS
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: TransientInClusterFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-channel: HU_PARTNER_10
+channel: HU_TNS_PARTNER
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: DecentFilter
   config:
-    max_tspan: 15
-    gaia_rs: 20
+    min_ndet: 2
+    min_tspan: 0
+    max_tspan: 365
+    min_rb: 0.3
     max_fwhm: 5.5
-    min_rb: 0.5
-    min_drb: 0.95
+    min_drb: 0.99
+    max_elong: 1.4
+    max_magdiff: 1
     max_nbad: 2
-    min_tspan: 4
     min_sso_dist: 20
-    ps1_sgveto_th: 0.8
-    min_ndet: 2
-    ps1_sgveto_rad: 1
     min_gal_lat: 14
-    gaia_veto_gmag_max: 20
-    gaia_plx_signif: 3
-    ps1_confusion_rad: 3
+    gaia_rs: 20
     gaia_pm_signif: 3
-    max_magdiff: 1
+    gaia_plx_signif: 3
     gaia_veto_gmag_min: 9
-    max_elong: 1.4
-    ps1_confusion_sg_tol: 0.1
+    gaia_veto_gmag_max: 20
     gaia_excessnoise_sig_max: 999
+    ps1_sgveto_rad: 1
+    ps1_sgveto_th: 0.8
+    ps1_confusion_rad: 3
+    ps1_confusion_sg_tol: 0.1
 t2_compute:
   - unit: T2SNCosmo
     config:
       model: salt2
   - unit: T2CatalogMatch
     config: T2CatalogMatch_cosmo
   - unit: T2BrightSNProb
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-channel: HU_PARTNER_59
+channel: HU_PARTNER_10
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: DecentFilter
   config:
-    max_tspan: 666
-    gaia_rs: 10
+    max_tspan: 15
+    gaia_rs: 20
     max_fwhm: 5.5
-    min_rb: 0.3
+    min_rb: 0.5
     min_drb: 0.95
     max_nbad: 2
-    min_tspan: 8
+    min_tspan: 4
     min_sso_dist: 20
     ps1_sgveto_th: 0.8
-    min_ndet: 4
+    min_ndet: 2
     ps1_sgveto_rad: 1
     min_gal_lat: 14
     gaia_veto_gmag_max: 20
     gaia_plx_signif: 3
     ps1_confusion_rad: 3
     gaia_pm_signif: 3
     max_magdiff: 1
     gaia_veto_gmag_min: 9
     max_elong: 1.4
     ps1_confusion_sg_tol: 0.1
-    gaia_excessnoise_sig_max: 1.7976931348623153e+308
+    gaia_excessnoise_sig_max: 999
 t2_compute:
   - unit: T2SNCosmo
     config:
       model: salt2
   - unit: T2CatalogMatch
     config: T2CatalogMatch_cosmo
   - unit: T2BrightSNProb
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_RAPID_INFANT
+source: null
 contact: ampel@desy.de
 active: true
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: XShooterFilter
   config: HU_RAPID
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_RAPID_LANCASTER
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: false
 template: ztf_uw_public
 t0_filter:
   unit: XShooterFilter
   config: HU_RAPID
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_RAPID_SINGLE
+source: null
 contact: ampel@desy.de
 active: true
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: XShooterFilter
   config: HU_RAPID
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 channel: HU_TNS_MSIP
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_public
 t0_filter:
   unit: DecentFilter
   config:
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-channel: HU_TNS_PARTNER
+channel: HU_PARTNER_59
+source: null
 contact: ampel@desy.de
 active: false
 auto_complete: live
 template: ztf_uw_private
 t0_filter:
   unit: DecentFilter
   config:
-    min_ndet: 2
-    min_tspan: 0
-    max_tspan: 365
-    min_rb: 0.3
+    max_tspan: 666
+    gaia_rs: 10
     max_fwhm: 5.5
-    min_drb: 0.99
-    max_elong: 1.4
-    max_magdiff: 1
+    min_rb: 0.3
+    min_drb: 0.95
     max_nbad: 2
+    min_tspan: 8
     min_sso_dist: 20
+    ps1_sgveto_th: 0.8
+    min_ndet: 4
+    ps1_sgveto_rad: 1
     min_gal_lat: 14
-    gaia_rs: 20
-    gaia_pm_signif: 3
-    gaia_plx_signif: 3
-    gaia_veto_gmag_min: 9
     gaia_veto_gmag_max: 20
-    gaia_excessnoise_sig_max: 999
-    ps1_sgveto_rad: 1
-    ps1_sgveto_th: 0.8
+    gaia_plx_signif: 3
     ps1_confusion_rad: 3
+    gaia_pm_signif: 3
+    max_magdiff: 1
+    gaia_veto_gmag_min: 9
+    max_elong: 1.4
     ps1_confusion_sg_tol: 0.1
+    gaia_excessnoise_sig_max: 1.7976931348623153e+308
 t2_compute:
   - unit: T2SNCosmo
     config:
       model: salt2
   - unit: T2CatalogMatch
     config: T2CatalogMatch_cosmo
   - unit: T2BrightSNProb
```

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/AmpelAutoLco.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/AmpelAutoLco.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/ChannelSummary.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ChannelSummary.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/CosmologySummary.yaml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/CosmologySummary.yaml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/RapidReact.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidReact.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/process/TNSSubmitNew.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/TNSSubmitNew.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.3a9/conf/ampel-hu-astro/unit.yml` & `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/unit.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 - ampel.contrib.hu.t0.SimpleDecentFilter
 - ampel.contrib.hu.t0.XShooterFilter
+- ampel.contrib.hu.t0.PredetectionFilter
 - ampel.contrib.hu.t0.TransientInClusterFilter
 - ampel.contrib.hu.t0.LensedTransientFilter
 - ampel.contrib.hu.t0.RandFilter
 - ampel.contrib.hu.t0.RcfFilter
 - ampel.contrib.hu.t0.RedshiftCatalogFilter
 - ampel.contrib.hu.t2.T2PanStarrThumbPrint
 - ampel.contrib.hu.t2.T2PhaseLimit
@@ -13,14 +14,17 @@
 - ampel.contrib.hu.t2.T2LCQuality
 - ampel.contrib.hu.t2.T2BrightSNProb
 - ampel.contrib.hu.t2.T2TNSEval
 - ampel.contrib.hu.t2.T2InfantCatalogEval
 - ampel.contrib.hu.t2.T2RunSncosmo
 - ampel.contrib.hu.t2.T2CatalogMatchLocal
 - ampel.contrib.hu.t2.T2DigestRedshifts
+- ampel.contrib.hu.t2.T2LoadRedshift
+- ampel.contrib.hu.t2.T2BayesianBlocks
+- ampel.contrib.hu.t2.T2DustEchoEval
 - ampel.contrib.hu.t2.T2RunPossis
 - ampel.contrib.hu.t2.T2RunTDE
 - ampel.contrib.hu.t2.T2RunParsnip
 - ampel.contrib.hu.t2.T2RunSnoopy
 - ampel.contrib.hu.t2.T2MatchBTS
 - ampel.contrib.hu.t2.T2NedTap
 - ampel.contrib.hu.t2.T2NedSNCosmo
@@ -29,14 +33,17 @@
 - ampel.contrib.hu.t2.T2LSPhotoZTap
 - ampel.contrib.hu.t2.T2ElasticcRedshiftSampler
 - ampel.contrib.hu.t2.T2TabulatorRiseDecline
 - ampel.contrib.hu.t2.T2XgbClassifier
 - ampel.contrib.hu.t2.T2MultiXgbClassifier
 - ampel.contrib.hu.t2.T2ElasticcReport
 - ampel.contrib.hu.t2.T2FastDecliner
+- ampel.contrib.hu.t2.T2HealpixProb
+- ampel.contrib.hu.t2.T2KilonovaEval
+- ampel.contrib.hu.t2.T2MatchGRB
 - ampel.contrib.hu.t3.TransientInfoPrinter
 - ampel.contrib.hu.t3.TransientViewDumper
 - ampel.contrib.hu.t3.ChannelSummaryPublisher
 - ampel.contrib.hu.t3.SlackSummaryPublisher
 - ampel.contrib.hu.t3.RapidBase
 - ampel.contrib.hu.t3.RapidSedm
 - ampel.contrib.hu.t3.RapidLco
@@ -44,7 +51,15 @@
 - ampel.contrib.hu.t3.TNSMirrorUpdater
 - ampel.contrib.hu.t3.TransientTablePublisher
 - ampel.contrib.hu.t3.HealpixCorrPlotter
 - ampel.contrib.hu.t3.PlotLightcurveSample
 - ampel.contrib.hu.t3.ElasticcClassPublisher
 - ampel.contrib.hu.t3.VOEventPublisher
 - ampel.contrib.hu.t3.AstroColibriPublisher
+- ampel.contrib.hu.t3.HealpixTokenGenerator
+- ampel.contrib.hu.t3.RandomMapGenerator
+- ampel.contrib.hu.alert.load.WiseFileAlertLoader
+- ampel.contrib.hu.alert.NeoWisePhotometryAlertSupplier
+- ampel.contrib.hu.alert.ResourceDependentConsumer
+- ampel.contrib.hu.alert.DynamicShaperAlertConsumer
+- ampel.contrib.hu.ingest.ZiGWDataPointShaper
+
```

### Comparing `ampel_hu_astro-0.8.3a9/pyproject.toml` & `ampel_hu_astro-0.8.4a0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-hu-astro"
-version = "0.8.3a9"
+version = "0.8.4a0"
 license = "BSD-3-Clause"
 readme = "README.md"
 description = "Astronomy units for the Ampel system from HU-Berlin"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-HU-astro"
 authors = [
     "Valery Brinnel",
@@ -28,60 +28,73 @@
     'conf/*/*.yaml',
     'conf/*/*/*.yaml',
     'conf/*/*.yml',
     'conf/*/*/*.yml',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
-ampel-plot = {version = "^0.8.3", source = "pypi"}
-ampel-ztf = {version = ">=0.8.3a4,<0.8.4", source = "pypi", extras = ["kafka"], optional = true}
-ampel-photometry = {version = ">=0.8.3-alpha.2,<0.8.4", source = "pypi"}
+python = ">=3.10,<3.12"
+ampel-plot = {version = ">=0.8.3-3,<0.9", source = "pypi"}
+ampel-ztf = {version = ">=0.8.13,<0.9", extras = ["kafka"], optional = true}
+ampel-photometry = {version = ">=0.8.3,<0.9", source = "pypi"}
+ampel-interface = {version = ">=0.8.8,<0.9", source = "pypi"}
+ampel-alerts = {version = ">=0.8.5,<0.9", source = "pypi"}
 sncosmo = {version = "^2.5.0", optional = true}
 iminuit = {version = "^2.8.0", optional = true}
-sfdmap = {version = "^0.1.1", optional = true, source = "pypi"} # conda-forge stale at py3.6
+sfdmap2 = {version = "^0.2.0", optional = true}
 numpy = "^1"
-scipy = "^1.4"
+scipy = ">=1.4"
 beautifulsoup4 = "^4.10.0"
 backoff = "^2"
 requests = "^2.26.0"
 astropy = "^5.0"
 # PyPI prohibits direct dependencies in install_requires
 # see: https://github.com/pypa/pip/issues/6301
 # FIXME: restore pymage when it lands on PyPI
 # pymage = {url = "https://github.com/MickaelRigault/pymage/archive/v1.0.tar.gz#sha256=11e99c4ea06b76ca7fb5b42d1d35d64139a4fa6f7f163a2f0f9cc3ea0b3c55eb"}
 # pymage has an undeclared dependency on pandas
-pandas = "^1.3.3"
-seaborn = "^0.11.2"
+pandas = "^2.0.0"
+seaborn = "^0.12.0"
 adjustText = "^0.7.3"
 extcats = {version = "^2.4.2", optional = true, source = "pypi"}
 slack-sdk = {version = "^3", optional = true}
 xgboost = {version = "^1.6.2", optional = true}
-astro-parsnip = {version = ">=1.3.1", optional = true}
+astro-parsnip = {version = "^1.4.1", optional = true}
 timeout-decorator = {version = "^0.5", optional = true}
 jupyter = {version = "^1.0.0", optional = true}
 voevent-parse = {version = "^1.0.3", optional = true}
-ztfquery = "^1.19.1"
+more-itertools = "^9.0.0"
+uncertainties = "^3.1.7"
+scikit-learn = "^1.1.3"
+healpy = {version = "^1.16.2", optional = true}
+light-curve = {version = "^0.7.3", optional = true}
+ampel-lsst = {version = ">=0.8.6,<0.9", optional = true}
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.971"
-pytest = "^6.2.5"
-pytest-cov = "^2.12.1"
-pytest-mock = "^3.6.1"
+mypy = "^1.6.1"
+pytest = "^7.4.3"
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.12.0"
 types-requests = "^2.25.9"
-types-pytz = "^2021.1.2"
+types-pytz = "^2022.1.2"
+# prevent poetry 1.3 from removing setuptools
+setuptools = "*"
 
 [tool.poetry.extras]
-sncosmo = ["sncosmo", "iminuit", "sfdmap"]
+elasticc = ["xgboost", "astro-parsnip", "timeout-decorator", "ampel-lsst", "light-curve"]
 extcats = ["extcats"]
+ligo = ["healpy", "sncosmo", "iminuit", "sfdmap2", "ampel-ztf"]
 slack = ["slack_sdk"]
-elasticc = ["xgboost", "astro-parsnip", "timeout-decorator"]
-ztf = ["ampel-ztf"]
+sncosmo = ["sncosmo", "iminuit", "sfdmap2"]
 notebook = ["jupyter"]
 voevent = ["voevent-parse"]
+ztf = ["ampel-ztf"]
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.1.13"
 
 [tool.conda-lock]
 channels = ["conda-forge"]
 platforms = ["linux-64", "osx-64", "osx-arm64"]
 
 [tool.conda-lock.dependencies]
 python-confluent-kafka = "1.7"
@@ -91,14 +104,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=40.8.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 namespace_packages = true
 show_error_codes = true
+check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
   "numpy.*",
   "scipy.*",
   "pymongo.*",
   "bson.*",
@@ -113,12 +127,53 @@
   "timeout_decorator.*",
   "parsnip.*",
   "sncosmo.*",
   "requests_toolbelt.*",
   "adjustText.*",
   "extcats.*",
   "voeventparse.*",
+  "healpy.*",
+  "light_curve.*",
 ]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--cov=ampel --showlocals -ra"
+
+[tool.black]
+line-length = 88
+
+[tool.ruff]
+target-version = "py310"
+exclude = [
+    "ampel/contrib/hu/xgb_trees.py",
+    "notebooks"
+]
+
+[tool.ruff.lint]
+select = [
+    "E4",
+    "E7",
+    "E9",
+    "F",
+    "I",
+    "UP", # pyupgrade
+    "B", # bugbear
+    "DTZ", # datetimez
+    # "T20", # print statements
+    # "PT", # pytest-style
+    "RET", # return
+    "SLF",
+    "SIM",
+    # "ARG", # sometimes your arguments have to conform to an interface
+    # "ERA", # seems to prohibit all comments, that's bad
+    "PL",
+    "PERF",
+    "RUF",
+]
+ignore = [
+    "E741", # ambiguous variable name
+    "UP009", # UTF-8 encoding declaration is unnecessary
+    "PLR09", # too many (arguments|branches)
+    "PLR2004", # Magic value used in comparison
+    "RUF012", # fine for AmpelUnit, actually (ruff has a special case for pydantic)
+]
```

### Comparing `ampel_hu_astro-0.8.3a9/PKG-INFO` & `ampel_hu_astro-0.8.4a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 Metadata-Version: 2.1
 Name: ampel-hu-astro
-Version: 0.8.3a9
+Version: 0.8.4a0
 Summary: Astronomy units for the Ampel system from HU-Berlin
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Provides-Extra: elasticc
 Provides-Extra: extcats
+Provides-Extra: ligo
 Provides-Extra: notebook
 Provides-Extra: slack
 Provides-Extra: sncosmo
 Provides-Extra: voevent
 Provides-Extra: ztf
 Requires-Dist: adjustText (>=0.7.3,<0.8.0)
-Requires-Dist: ampel-photometry (>=0.8.3-alpha.2,<0.8.4)
-Requires-Dist: ampel-plot (>=0.8.3,<0.9.0)
-Requires-Dist: ampel-ztf[kafka] (>=0.8.3a4,<0.8.4) ; extra == "ztf"
-Requires-Dist: astro-parsnip (>=1.3.1) ; extra == "elasticc"
+Requires-Dist: ampel-alerts (>=0.8.5,<0.9)
+Requires-Dist: ampel-interface (>=0.8.8,<0.9)
+Requires-Dist: ampel-lsst (>=0.8.6,<0.9) ; extra == "elasticc"
+Requires-Dist: ampel-photometry (>=0.8.3,<0.9)
+Requires-Dist: ampel-plot (>=0.8.3-3,<0.9)
+Requires-Dist: ampel-ztf[kafka] (>=0.8.13,<0.9) ; extra == "ligo" or extra == "ztf"
+Requires-Dist: astro-parsnip (>=1.4.1,<2.0.0) ; extra == "elasticc"
 Requires-Dist: astropy (>=5.0,<6.0)
 Requires-Dist: backoff (>=2,<3)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: extcats (>=2.4.2,<3.0.0) ; extra == "extcats"
-Requires-Dist: iminuit (>=2.8.0,<3.0.0) ; extra == "sncosmo"
+Requires-Dist: healpy (>=1.16.2,<2.0.0) ; extra == "ligo"
+Requires-Dist: iminuit (>=2.8.0,<3.0.0) ; extra == "ligo" or extra == "sncosmo"
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "notebook"
+Requires-Dist: light-curve (>=0.7.3,<0.8.0) ; extra == "elasticc"
+Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: numpy (>=1,<2)
-Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: scipy (>=1.4,<2.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Requires-Dist: sfdmap (>=0.1.1,<0.2.0) ; extra == "sncosmo"
+Requires-Dist: scikit-learn (>=1.1.3,<2.0.0)
+Requires-Dist: scipy (>=1.4)
+Requires-Dist: seaborn (>=0.12.0,<0.13.0)
+Requires-Dist: sfdmap2 (>=0.2.0,<0.3.0) ; extra == "ligo" or extra == "sncosmo"
 Requires-Dist: slack-sdk (>=3,<4) ; extra == "slack"
-Requires-Dist: sncosmo (>=2.5.0,<3.0.0) ; extra == "sncosmo"
+Requires-Dist: sncosmo (>=2.5.0,<3.0.0) ; extra == "ligo" or extra == "sncosmo"
 Requires-Dist: timeout-decorator (>=0.5,<0.6) ; extra == "elasticc"
+Requires-Dist: uncertainties (>=3.1.7,<4.0.0)
 Requires-Dist: voevent-parse (>=1.0.3,<2.0.0) ; extra == "voevent"
 Requires-Dist: xgboost (>=1.6.2,<2.0.0) ; extra == "elasticc"
-Requires-Dist: ztfquery (>=1.19.1,<2.0.0)
 Project-URL: Repository, https://github.com/AmpelProject/Ampel-HU-astro
 Description-Content-Type: text/markdown
 
+<img align="left" src="https://user-images.githubusercontent.com/17532220/213287034-0209aa19-f8a1-418f-a325-7472510542cb.png" width="150" height="150"/>
+<br>
+
+# AMPEL-HU-astro
+<br><br>
+
+
 Contributed Ampel units from HU/DESY group
 ==========================================
 
 Demo install instructions:
 ==========================
 
 Create environment with python 3.10+ / poetry. Then run:
```

