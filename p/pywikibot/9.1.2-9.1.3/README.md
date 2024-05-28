# Comparing `tmp/pywikibot-9.1.2.tar.gz` & `tmp/pywikibot-9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-9.1.2.tar", last modified: Fri May  3 06:01:55 2024, max compression
+gzip compressed data, was "pywikibot-9.1.3.tar", last modified: Tue May 28 13:52:37 2024, max compression
```

## Comparing `pywikibot-9.1.2.tar` & `pywikibot-9.1.3.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.801658 pywikibot-9.1.2/
--rw-rw-rw-   0        0        0     4207 2024-05-02 14:46:17.000000 pywikibot-9.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0      177 2024-04-20 14:45:29.000000 pywikibot-9.1.2/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1086 2024-04-20 14:45:29.000000 pywikibot-9.1.2/LICENSE
--rw-rw-rw-   0        0        0       90 2024-04-20 14:45:29.000000 pywikibot-9.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    17474 2024-05-03 06:01:55.800200 pywikibot-9.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5484 2024-04-20 14:45:29.000000 pywikibot-9.1.2/README.rst
--rw-rw-rw-   0        0        0     5939 2024-05-03 06:00:19.000000 pywikibot-9.1.2/ROADMAP.rst
--rw-rw-rw-   0        0        0     4617 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.363586 pywikibot-9.1.2/pywikibot/
--rw-rw-rw-   0        0        0    14027 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      363 2024-05-03 06:00:19.000000 pywikibot-9.1.2/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0    43977 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     6897 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/backports.py
--rw-rw-rw-   0        0        0    87385 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/bot.py
--rw-rw-rw-   0        0        0    27855 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.438739 pywikibot-9.1.2/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15778 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    20032 2024-05-02 11:42:30.000000 pywikibot-9.1.2/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    45908 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/config.py
--rw-rw-rw-   0        0        0    46627 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2096 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.450699 pywikibot-9.1.2/pywikibot/data/
--rw-rw-rw-   0        0        0     1990 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.467657 pywikibot-9.1.2/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3212 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41998 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7556 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    16895 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53137 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14075 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2599 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     9737 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     4104 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    97086 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/date.py
--rw-rw-rw-   0        0        0    24621 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/diff.py
--rw-rw-rw-   0        0        0     1937 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/echo.py
--rw-rw-rw-   0        0        0     8033 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/editor.py
--rw-rw-rw-   0        0        0    20732 2024-05-02 15:55:46.000000 pywikibot-9.1.2/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.528648 pywikibot-9.1.2/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     1792 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      481 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      376 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      393 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      621 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      439 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      629 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      407 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      399 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0     1169 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2444 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0      996 2024-04-23 14:22:19.000000 pywikibot-9.1.2/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0      403 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikifunctions_family.py
--rw-rw-rw-   0        0        0     1669 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1047 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      813 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1856 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    11124 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2919 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5373 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      469 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      463 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1176 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1053 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     4166 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2452 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    43417 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/family.py
--rw-rw-rw-   0        0        0    33229 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20614 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/flow.py
--rw-rw-rw-   0        0        0    29937 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     7896 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13048 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12576 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22774 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.552548 pywikibot-9.1.2/pywikibot/page/
--rw-rw-rw-   0        0        0     1289 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    88531 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19031 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2175 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    19962 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29468 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8551 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     3035 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4055 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16532 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    90813 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.562727 pywikibot-9.1.2/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29759 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    41066 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    18463 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    46417 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3955 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/plural.py
--rw-rw-rw-   0        0        0    49322 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.578806 pywikibot-9.1.2/pywikibot/scripts/
--rw-rw-rw-   0        0        0      921 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    12328 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20040 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.592440 pywikibot-9.1.2/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      349 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.679358 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sdh.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/skr.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6095 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3449 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     2045 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3501 2024-05-03 06:00:19.000000 pywikibot-9.1.2/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18718 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.719192 pywikibot-9.1.2/pywikibot/site/
--rw-rw-rw-   0        0        0     1051 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   116994 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    16617 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38399 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4105 2024-05-02 14:46:17.000000 pywikibot-9.1.2/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    29727 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    98105 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3004 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    15079 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1586 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    12928 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4844 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25238 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11158 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.730212 pywikibot-9.1.2/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      409 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3142 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20865 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    87673 2024-04-30 12:33:22.000000 pywikibot-9.1.2/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12246 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    20620 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/time.py
--rw-rw-rw-   0        0        0     3259 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.759332 pywikibot-9.1.2/pywikibot/tools/
--rw-rw-rw-   0        0        0    27110 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25676 2024-05-02 14:46:17.000000 pywikibot-9.1.2/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22245 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     4456 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0    10286 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    10984 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4060 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     8988 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7248 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.782296 pywikibot-9.1.2/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      910 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1885 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2713 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22357 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      495 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    25232 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2152 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2048 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90667 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    15031 2024-05-03 04:36:59.000000 pywikibot-9.1.2/pywikibot/version.py
--rw-rw-rw-   0        0        0    11113 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.787212 pywikibot-9.1.2/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    17474 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10561 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      982 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 06:01:55.801658 pywikibot-9.1.2/setup.cfg
--rw-rw-rw-   0        0        0     8130 2024-04-28 12:23:49.000000 pywikibot-9.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.785244 pywikibot-9.1.2/tests/
--rw-rw-rw-   0        0        0     2832 2024-04-20 14:45:29.000000 pywikibot-9.1.2/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.544335 pywikibot-9.1.3/
+-rw-rw-rw-   0        0        0     4207 2024-05-20 11:42:47.000000 pywikibot-9.1.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0      177 2024-05-20 11:14:51.000000 pywikibot-9.1.3/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1086 2024-05-20 11:42:47.000000 pywikibot-9.1.3/LICENSE
+-rw-rw-rw-   0        0        0       90 2024-05-20 11:42:47.000000 pywikibot-9.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    17526 2024-05-28 13:52:37.540346 pywikibot-9.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5484 2024-05-20 11:42:47.000000 pywikibot-9.1.3/README.rst
+-rw-rw-rw-   0        0        0     5837 2024-05-28 13:49:22.000000 pywikibot-9.1.3/ROADMAP.rst
+-rw-rw-rw-   0        0        0     4617 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:34.990059 pywikibot-9.1.3/pywikibot/
+-rw-rw-rw-   0        0        0    14027 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0    43977 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     6897 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    87385 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    27855 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.073838 pywikibot-9.1.3/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2024-04-20 14:45:29.000000 pywikibot-9.1.3/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15778 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    20032 2024-05-25 15:32:38.000000 pywikibot-9.1.3/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    45908 2024-05-26 11:55:34.000000 pywikibot-9.1.3/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46627 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2096 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.132682 pywikibot-9.1.3/pywikibot/data/
+-rw-rw-rw-   0        0        0     1990 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.144650 pywikibot-9.1.3/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3212 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41998 2024-05-25 16:55:56.000000 pywikibot-9.1.3/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7556 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    16895 2024-05-25 13:04:25.000000 pywikibot-9.1.3/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53137 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14075 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2599 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     9737 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     4104 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    97086 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24621 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     1937 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     8033 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    20732 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.644337 pywikibot-9.1.3/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2024-04-20 14:45:29.000000 pywikibot-9.1.3/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     1792 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      481 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      376 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      393 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      621 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      439 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      629 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1243 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      407 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      399 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0     1169 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2444 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0      996 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0      403 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikifunctions_family.py
+-rw-rw-rw-   0        0        0     1669 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1047 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      813 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1856 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    11131 2024-05-28 13:35:44.000000 pywikibot-9.1.3/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2919 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5373 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      469 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      463 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1176 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1053 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     4166 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2452 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    43417 2024-05-25 16:19:47.000000 pywikibot-9.1.3/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33229 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20614 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    29937 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     7896 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13048 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12576 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22774 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.679245 pywikibot-9.1.3/pywikibot/page/
+-rw-rw-rw-   0        0        0     1289 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    88531 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19031 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2175 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    19962 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29468 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8551 2024-05-25 16:19:47.000000 pywikibot-9.1.3/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     3035 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4055 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16532 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    90813 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.774992 pywikibot-9.1.3/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29759 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    41066 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    18463 2024-05-20 11:42:47.000000 pywikibot-9.1.3/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    46417 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3955 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    49322 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.943548 pywikibot-9.1.3/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      921 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12328 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20040 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:35.962499 pywikibot-9.1.3/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      349 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.152365 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sdh.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/skr.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6095 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3449 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     2045 2024-05-21 13:34:55.000000 pywikibot-9.1.3/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3501 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18718 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.196249 pywikibot-9.1.3/pywikibot/site/
+-rw-rw-rw-   0        0        0     1051 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   116994 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    16617 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38399 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4105 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    29727 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    98105 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3004 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    15079 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1586 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    12928 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4844 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25238 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11158 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.271052 pywikibot-9.1.3/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      409 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3142 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20865 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    87673 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12246 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    20620 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3259 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.353836 pywikibot-9.1.3/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27110 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25676 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1243 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22245 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4456 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0    10286 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    10984 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4060 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     8988 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7248 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.477509 pywikibot-9.1.3/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      910 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1885 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2713 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22357 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      495 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    25232 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2152 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2048 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90667 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    15031 2024-05-28 13:49:23.000000 pywikibot-9.1.3/pywikibot/version.py
+-rw-rw-rw-   0        0        0    11113 2024-05-20 11:42:48.000000 pywikibot-9.1.3/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.514413 pywikibot-9.1.3/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    17526 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10561 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1104 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 13:52:34.000000 pywikibot-9.1.3/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:52:37.545331 pywikibot-9.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     8237 2024-05-28 13:35:44.000000 pywikibot-9.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:52:37.510426 pywikibot-9.1.3/tests/
+-rw-rw-rw-   0        0        0     2832 2024-05-20 11:42:48.000000 pywikibot-9.1.3/tests/tests_tests.py
```

### Comparing `pywikibot-9.1.2/AUTHORS.rst` & `pywikibot-9.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/LICENSE` & `pywikibot-9.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/PKG-INFO` & `pywikibot-9.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.1.2
+Version: 9.1.3
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -111,15 +111,15 @@
 Provides-Extra: memento
 Requires-Dist: memento_client==0.6.1; extra == "memento"
 Provides-Extra: wikitextparser
 Requires-Dist: wikitextparser>=0.47.0; extra == "wikitextparser"
 Provides-Extra: mysql
 Requires-Dist: PyMySQL>=1.0.0; extra == "mysql"
 Provides-Extra: tkinter
-Requires-Dist: Pillow!=10.0,!=10.1,>=8.1.2; extra == "tkinter"
+Requires-Dist: Pillow!=10.0,!=10.1,>=8.1.2; python_version < "3.13" and extra == "tkinter"
 Provides-Extra: mwoauth
 Requires-Dist: mwoauth!=0.3.1,>=0.2.4; extra == "mwoauth"
 Provides-Extra: html
 Requires-Dist: beautifulsoup4>=4.7.1; extra == "html"
 Provides-Extra: http
 Requires-Dist: fake-useragent>=1.4.0; extra == "http"
 Provides-Extra: flake8
@@ -133,15 +133,16 @@
 Requires-Dist: flake8-mock-x2; extra == "flake8"
 Requires-Dist: flake8-print>=5.0.0; extra == "flake8"
 Requires-Dist: flake8-quotes>=3.3.2; extra == "flake8"
 Requires-Dist: flake8-raise; extra == "flake8"
 Requires-Dist: flake8-string-format; extra == "flake8"
 Requires-Dist: flake8-tuple>=0.4.1; extra == "flake8"
 Requires-Dist: flake8-no-u-prefixed-strings>=0.2; extra == "flake8"
-Requires-Dist: pep8-naming>=0.13.3; extra == "flake8"
+Requires-Dist: pep8-naming==0.13.3; python_version < "3.8" and extra == "flake8"
+Requires-Dist: pep8-naming>=0.14.0; python_version >= "3.8" and extra == "flake8"
 Provides-Extra: hacking
 Requires-Dist: hacking; extra == "hacking"
 Requires-Dist: importlib-metadata<5.0.0; python_version < "3.8" and extra == "hacking"
 Provides-Extra: create-isbn-edition-py
 Requires-Dist: isbnlib; extra == "create-isbn-edition-py"
 Requires-Dist: unidecode; extra == "create-isbn-edition-py"
 Provides-Extra: weblinkchecker-py
@@ -295,16 +296,15 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Remove line endings in version.getversion_nightly(T363943)
-* Provide ``-nouser`` option with pywikibot.scripts.version
+* Add support for dtpwiki (T365232)
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
```

### Comparing `pywikibot-9.1.2/README.rst` & `pywikibot-9.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/ROADMAP.rst` & `pywikibot-9.1.3/ROADMAP.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Current release
 ---------------
 
-* Remove line endings in :func:`version.getversion_nightly` (:phab:`T363943`)
-* Provide ``-nouser`` option with :mod:`pywikibot.scripts.version`
+* Add support for dtpwiki (:phab:`T365232`)
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of :meth:`proofreadpage.IndexPage.page_gen` is deprecated and will be ignored
   (:phab:`T358635`)
```

### Comparing `pywikibot-9.1.2/pyproject.toml` & `pywikibot-9.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/__init__.py` & `pywikibot-9.1.3/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/_wbtypes.py` & `pywikibot-9.1.3/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/backports.py` & `pywikibot-9.1.3/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/bot.py` & `pywikibot-9.1.3/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/bot_choice.py` & `pywikibot-9.1.3/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/comms/eventstreams.py` & `pywikibot-9.1.3/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/comms/http.py` & `pywikibot-9.1.3/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/config.py` & `pywikibot-9.1.3/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/cosmetic_changes.py` & `pywikibot-9.1.3/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/daemonize.py` & `pywikibot-9.1.3/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/__init__.py` & `pywikibot-9.1.3/pywikibot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/api/__init__.py` & `pywikibot-9.1.3/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/api/_generators.py` & `pywikibot-9.1.3/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/api/_optionset.py` & `pywikibot-9.1.3/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/api/_paraminfo.py` & `pywikibot-9.1.3/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/api/_requests.py` & `pywikibot-9.1.3/pywikibot/data/api/_requests.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/memento.py` & `pywikibot-9.1.3/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/mysql.py` & `pywikibot-9.1.3/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/sparql.py` & `pywikibot-9.1.3/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/data/wikistats.py` & `pywikibot-9.1.3/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/date.py` & `pywikibot-9.1.3/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/diff.py` & `pywikibot-9.1.3/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/echo.py` & `pywikibot-9.1.3/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/editor.py` & `pywikibot-9.1.3/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/exceptions.py` & `pywikibot-9.1.3/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/commons_family.py` & `pywikibot-9.1.3/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/lingualibre_family.py` & `pywikibot-9.1.3/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/meta_family.py` & `pywikibot-9.1.3/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/osm_family.py` & `pywikibot-9.1.3/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/vikidia_family.py` & `pywikibot-9.1.3/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikibooks_family.py` & `pywikibot-9.1.3/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikidata_family.py` & `pywikibot-9.1.3/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikihow_family.py` & `pywikibot-9.1.3/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikimania_family.py` & `pywikibot-9.1.3/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikimediachapter_family.py` & `pywikibot-9.1.3/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikinews_family.py` & `pywikibot-9.1.3/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikipedia_family.py` & `pywikibot-9.1.3/pywikibot/families/wikipedia_family.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,40 +30,40 @@
     codes = {
         'ab', 'ace', 'ady', 'af', 'als', 'alt', 'am', 'ami', 'an', 'ang',
         'anp', 'ar', 'arc', 'ary', 'arz', 'as', 'ast', 'atj', 'av', 'avk',
         'awa', 'ay', 'az', 'azb', 'ba', 'ban', 'bar', 'bat-smg', 'bbc', 'bcl',
         'be', 'be-tarask', 'bew', 'bg', 'bh', 'bi', 'bjn', 'blk', 'bm', 'bn',
         'bo', 'bpy', 'br', 'bs', 'bug', 'bxr', 'ca', 'cbk-zam', 'cdo', 'ce',
         'ceb', 'ch', 'chr', 'chy', 'ckb', 'co', 'cr', 'crh', 'cs', 'csb', 'cu',
-        'cv', 'cy', 'da', 'dag', 'de', 'dga', 'din', 'diq', 'dsb', 'dty', 'dv',
-        'dz', 'ee', 'el', 'eml', 'en', 'eo', 'es', 'et', 'eu', 'ext', 'fa',
-        'fat', 'ff', 'fi', 'fiu-vro', 'fj', 'fo', 'fon', 'fr', 'frp', 'frr',
-        'fur', 'fy', 'ga', 'gag', 'gan', 'gcr', 'gd', 'gl', 'glk', 'gn', 'gom',
-        'gor', 'got', 'gpe', 'gu', 'guc', 'gur', 'guw', 'gv', 'ha', 'hak',
-        'haw', 'he', 'hi', 'hif', 'hr', 'hsb', 'ht', 'hu', 'hy', 'hyw', 'ia',
-        'id', 'ie', 'ig', 'igl', 'ik', 'ilo', 'inh', 'io', 'is', 'it', 'iu',
-        'ja', 'jam', 'jbo', 'jv', 'ka', 'kaa', 'kab', 'kbd', 'kbp', 'kcg',
-        'kg', 'ki', 'kk', 'kl', 'km', 'kn', 'ko', 'koi', 'krc', 'ks', 'ksh',
-        'ku', 'kus', 'kv', 'kw', 'ky', 'la', 'lad', 'lb', 'lbe', 'lez', 'lfn',
-        'lg', 'li', 'lij', 'lld', 'lmo', 'ln', 'lo', 'lt', 'ltg', 'lv', 'mad',
-        'mai', 'map-bms', 'mdf', 'mg', 'mhr', 'mi', 'min', 'mk', 'ml', 'mn',
-        'mni', 'mnw', 'mr', 'mrj', 'ms', 'mt', 'mwl', 'my', 'myv', 'mzn',
-        'nah', 'nap', 'nds', 'nds-nl', 'ne', 'new', 'nia', 'nl', 'nn', 'no',
-        'nov', 'nqo', 'nrm', 'nso', 'nv', 'ny', 'oc', 'olo', 'om', 'or', 'os',
-        'pa', 'pag', 'pam', 'pap', 'pcd', 'pcm', 'pdc', 'pfl', 'pi', 'pih',
-        'pl', 'pms', 'pnb', 'pnt', 'ps', 'pt', 'pwn', 'qu', 'rm', 'rmy', 'rn',
-        'ro', 'roa-rup', 'roa-tara', 'ru', 'rue', 'rw', 'sa', 'sah', 'sat',
-        'sc', 'scn', 'sco', 'sd', 'se', 'sg', 'sh', 'shi', 'shn', 'si',
-        'simple', 'sk', 'skr', 'sl', 'sm', 'smn', 'sn', 'so', 'sq', 'sr',
-        'srn', 'ss', 'st', 'stq', 'su', 'sv', 'sw', 'szl', 'szy', 'ta', 'tay',
-        'tcy', 'te', 'tet', 'tg', 'th', 'ti', 'tk', 'tl', 'tly', 'tn', 'to',
-        'tpi', 'tr', 'trv', 'ts', 'tt', 'tum', 'tw', 'ty', 'tyv', 'udm', 'ug',
-        'uk', 'ur', 'uz', 've', 'vec', 'vep', 'vi', 'vls', 'vo', 'wa', 'war',
-        'wo', 'wuu', 'xal', 'xh', 'xmf', 'yi', 'yo', 'za', 'zea', 'zgh', 'zh',
-        'zh-classical', 'zh-min-nan', 'zh-yue', 'zu',
+        'cv', 'cy', 'da', 'dag', 'de', 'dga', 'din', 'diq', 'dsb', 'dtp',
+        'dty', 'dv', 'dz', 'ee', 'el', 'eml', 'en', 'eo', 'es', 'et', 'eu',
+        'ext', 'fa', 'fat', 'ff', 'fi', 'fiu-vro', 'fj', 'fo', 'fon', 'fr',
+        'frp', 'frr', 'fur', 'fy', 'ga', 'gag', 'gan', 'gcr', 'gd', 'gl',
+        'glk', 'gn', 'gom', 'gor', 'got', 'gpe', 'gu', 'guc', 'gur', 'guw',
+        'gv', 'ha', 'hak', 'haw', 'he', 'hi', 'hif', 'hr', 'hsb', 'ht', 'hu',
+        'hy', 'hyw', 'ia', 'id', 'ie', 'ig', 'igl', 'ik', 'ilo', 'inh', 'io',
+        'is', 'it', 'iu', 'ja', 'jam', 'jbo', 'jv', 'ka', 'kaa', 'kab', 'kbd',
+        'kbp', 'kcg', 'kg', 'ki', 'kk', 'kl', 'km', 'kn', 'ko', 'koi', 'krc',
+        'ks', 'ksh', 'ku', 'kus', 'kv', 'kw', 'ky', 'la', 'lad', 'lb', 'lbe',
+        'lez', 'lfn', 'lg', 'li', 'lij', 'lld', 'lmo', 'ln', 'lo', 'lt',
+        'ltg', 'lv', 'mad', 'mai', 'map-bms', 'mdf', 'mg', 'mhr', 'mi', 'min',
+        'mk', 'ml', 'mn', 'mni', 'mnw', 'mr', 'mrj', 'ms', 'mt', 'mwl', 'my',
+        'myv', 'mzn', 'nah', 'nap', 'nds', 'nds-nl', 'ne', 'new', 'nia', 'nl',
+        'nn', 'no', 'nov', 'nqo', 'nrm', 'nso', 'nv', 'ny', 'oc', 'olo', 'om',
+        'or', 'os', 'pa', 'pag', 'pam', 'pap', 'pcd', 'pcm', 'pdc', 'pfl',
+        'pi', 'pih', 'pl', 'pms', 'pnb', 'pnt', 'ps', 'pt', 'pwn', 'qu', 'rm',
+        'rmy', 'rn', 'ro', 'roa-rup', 'roa-tara', 'ru', 'rue', 'rw', 'sa',
+        'sah', 'sat', 'sc', 'scn', 'sco', 'sd', 'se', 'sg', 'sh', 'shi',
+        'shn', 'si', 'simple', 'sk', 'skr', 'sl', 'sm', 'smn', 'sn', 'so',
+        'sq', 'sr', 'srn', 'ss', 'st', 'stq', 'su', 'sv', 'sw', 'szl', 'szy',
+        'ta', 'tay', 'tcy', 'te', 'tet', 'tg', 'th', 'ti', 'tk', 'tl', 'tly',
+        'tn', 'to', 'tpi', 'tr', 'trv', 'ts', 'tt', 'tum', 'tw', 'ty', 'tyv',
+        'udm', 'ug', 'uk', 'ur', 'uz', 've', 'vec', 'vep', 'vi', 'vls', 'vo',
+        'wa', 'war', 'wo', 'wuu', 'xal', 'xh', 'xmf', 'yi', 'yo', 'za', 'zea',
+        'zgh', 'zh', 'zh-classical', 'zh-min-nan', 'zh-yue', 'zu',
     }
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
```

### Comparing `pywikibot-9.1.2/pywikibot/families/wikiquote_family.py` & `pywikibot-9.1.3/pywikibot/families/wikiquote_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikisource_family.py` & `pywikibot-9.1.3/pywikibot/families/wikisource_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikiversity_family.py` & `pywikibot-9.1.3/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wikivoyage_family.py` & `pywikibot-9.1.3/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wiktionary_family.py` & `pywikibot-9.1.3/pywikibot/families/wiktionary_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/families/wowwiki_family.py` & `pywikibot-9.1.3/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/family.py` & `pywikibot-9.1.3/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/fixes.py` & `pywikibot-9.1.3/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/flow.py` & `pywikibot-9.1.3/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/i18n.py` & `pywikibot-9.1.3/pywikibot/i18n.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/interwiki_graph.py` & `pywikibot-9.1.3/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/logentries.py` & `pywikibot-9.1.3/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/logging.py` & `pywikibot-9.1.3/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/login.py` & `pywikibot-9.1.3/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/__init__.py` & `pywikibot-9.1.3/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_basepage.py` & `pywikibot-9.1.3/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_category.py` & `pywikibot-9.1.3/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_collections.py` & `pywikibot-9.1.3/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_decorators.py` & `pywikibot-9.1.3/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_filepage.py` & `pywikibot-9.1.3/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_links.py` & `pywikibot-9.1.3/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_page.py` & `pywikibot-9.1.3/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_revision.py` & `pywikibot-9.1.3/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_toolforge.py` & `pywikibot-9.1.3/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_user.py` & `pywikibot-9.1.3/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/page/_wikibase.py` & `pywikibot-9.1.3/pywikibot/page/_wikibase.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/pagegenerators/__init__.py` & `pywikibot-9.1.3/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/pagegenerators/_factory.py` & `pywikibot-9.1.3/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/pagegenerators/_filters.py` & `pywikibot-9.1.3/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/pagegenerators/_generators.py` & `pywikibot-9.1.3/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/plural.py` & `pywikibot-9.1.3/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/proofreadpage.py` & `pywikibot-9.1.3/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/__init__.py` & `pywikibot-9.1.3/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/generate_family_file.py` & `pywikibot-9.1.3/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/generate_user_files.py` & `pywikibot-9.1.3/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ku.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ku.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-9.1.3/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/login.py` & `pywikibot-9.1.3/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/preload_sites.py` & `pywikibot-9.1.3/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/shell.py` & `pywikibot-9.1.3/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/version.py` & `pywikibot-9.1.3/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/scripts/wrapper.py` & `pywikibot-9.1.3/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/__init__.py` & `pywikibot-9.1.3/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_apisite.py` & `pywikibot-9.1.3/pywikibot/site/_apisite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_basesite.py` & `pywikibot-9.1.3/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_datasite.py` & `pywikibot-9.1.3/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_decorators.py` & `pywikibot-9.1.3/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_extensions.py` & `pywikibot-9.1.3/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_generators.py` & `pywikibot-9.1.3/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_interwikimap.py` & `pywikibot-9.1.3/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_namespace.py` & `pywikibot-9.1.3/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_obsoletesites.py` & `pywikibot-9.1.3/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_siteinfo.py` & `pywikibot-9.1.3/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_tokenwallet.py` & `pywikibot-9.1.3/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site/_upload.py` & `pywikibot-9.1.3/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/site_detect.py` & `pywikibot-9.1.3/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/specialbots/_unlink.py` & `pywikibot-9.1.3/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/specialbots/_upload.py` & `pywikibot-9.1.3/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/textlib.py` & `pywikibot-9.1.3/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/throttle.py` & `pywikibot-9.1.3/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/time.py` & `pywikibot-9.1.3/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/titletranslate.py` & `pywikibot-9.1.3/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/__init__.py` & `pywikibot-9.1.3/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/_deprecate.py` & `pywikibot-9.1.3/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/_logging.py` & `pywikibot-9.1.3/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/_unidata.py` & `pywikibot-9.1.3/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/chars.py` & `pywikibot-9.1.3/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/collections.py` & `pywikibot-9.1.3/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/djvu.py` & `pywikibot-9.1.3/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/formatter.py` & `pywikibot-9.1.3/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/itertools.py` & `pywikibot-9.1.3/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/tools/threading.py` & `pywikibot-9.1.3/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/__init__.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/gui.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/userinterfaces/transliteration.py` & `pywikibot-9.1.3/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/version.py` & `pywikibot-9.1.3/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot/xmlreader.py` & `pywikibot-9.1.3/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot.egg-info/PKG-INFO` & `pywikibot-9.1.3/pywikibot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.1.2
+Version: 9.1.3
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -111,15 +111,15 @@
 Provides-Extra: memento
 Requires-Dist: memento_client==0.6.1; extra == "memento"
 Provides-Extra: wikitextparser
 Requires-Dist: wikitextparser>=0.47.0; extra == "wikitextparser"
 Provides-Extra: mysql
 Requires-Dist: PyMySQL>=1.0.0; extra == "mysql"
 Provides-Extra: tkinter
-Requires-Dist: Pillow!=10.0,!=10.1,>=8.1.2; extra == "tkinter"
+Requires-Dist: Pillow!=10.0,!=10.1,>=8.1.2; python_version < "3.13" and extra == "tkinter"
 Provides-Extra: mwoauth
 Requires-Dist: mwoauth!=0.3.1,>=0.2.4; extra == "mwoauth"
 Provides-Extra: html
 Requires-Dist: beautifulsoup4>=4.7.1; extra == "html"
 Provides-Extra: http
 Requires-Dist: fake-useragent>=1.4.0; extra == "http"
 Provides-Extra: flake8
@@ -133,15 +133,16 @@
 Requires-Dist: flake8-mock-x2; extra == "flake8"
 Requires-Dist: flake8-print>=5.0.0; extra == "flake8"
 Requires-Dist: flake8-quotes>=3.3.2; extra == "flake8"
 Requires-Dist: flake8-raise; extra == "flake8"
 Requires-Dist: flake8-string-format; extra == "flake8"
 Requires-Dist: flake8-tuple>=0.4.1; extra == "flake8"
 Requires-Dist: flake8-no-u-prefixed-strings>=0.2; extra == "flake8"
-Requires-Dist: pep8-naming>=0.13.3; extra == "flake8"
+Requires-Dist: pep8-naming==0.13.3; python_version < "3.8" and extra == "flake8"
+Requires-Dist: pep8-naming>=0.14.0; python_version >= "3.8" and extra == "flake8"
 Provides-Extra: hacking
 Requires-Dist: hacking; extra == "hacking"
 Requires-Dist: importlib-metadata<5.0.0; python_version < "3.8" and extra == "hacking"
 Provides-Extra: create-isbn-edition-py
 Requires-Dist: isbnlib; extra == "create-isbn-edition-py"
 Requires-Dist: unidecode; extra == "create-isbn-edition-py"
 Provides-Extra: weblinkchecker-py
@@ -295,16 +296,15 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Remove line endings in version.getversion_nightly(T363943)
-* Provide ``-nouser`` option with pywikibot.scripts.version
+* Add support for dtpwiki (T365232)
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
```

### Comparing `pywikibot-9.1.2/pywikibot.egg-info/SOURCES.txt` & `pywikibot-9.1.3/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.2/pywikibot.egg-info/requires.txt` & `pywikibot-9.1.3/pywikibot.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 [Google]
 google>=1.7
 
 [Graphviz]
 pydot>=1.4.1
 
 [Tkinter]
+
+[Tkinter:python_version < "3.13"]
 Pillow!=10.0,!=10.1,>=8.1.2
 
 [create_isbn_edition.py]
 isbnlib
 unidecode
 
 [eventstreams]
@@ -32,15 +34,20 @@
 flake8-mock-x2
 flake8-print>=5.0.0
 flake8-quotes>=3.3.2
 flake8-raise
 flake8-string-format
 flake8-tuple>=0.4.1
 flake8-no-u-prefixed-strings>=0.2
-pep8-naming>=0.13.3
+
+[flake8:python_version < "3.8"]
+pep8-naming==0.13.3
+
+[flake8:python_version >= "3.8"]
+pep8-naming>=0.14.0
 
 [hacking]
 hacking
 
 [hacking:python_version < "3.8"]
 importlib-metadata<5.0.0
```

### Comparing `pywikibot-9.1.2/setup.py` & `pywikibot-9.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - synchronize the local tags with the remote repositoy
 - merge current master branch to stable branch
 - push new stable branch to Gerrit and merge it the stable repository
 - prepare the next master release by increasing the version number in
   ``pywikibot.__metadata__.py`` and adding developmental identifier
 - upload this patchset to Gerrit and merge it.
 
-.. warning: do not upload a development release to pypi.
+.. warning:: do not upload a development release to pypi.
 """
 #
 # (C) Pywikibot team, 2009-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
@@ -41,15 +41,15 @@
     'isbn': ['python-stdnum>=1.19'],
     'Graphviz': ['pydot>=1.4.1'],
     'Google': ['google>=1.7'],
     'memento': ['memento_client==0.6.1'],
     'wikitextparser': ['wikitextparser>=0.47.0'],
     'mysql': ['PyMySQL >= 1.0.0'],
     # vulnerability found in Pillow<8.1.2 but toolforge uses 5.4.1
-    'Tkinter': ['Pillow>=8.1.2, != 10.0, != 10.1'],
+    'Tkinter': ['Pillow>=8.1.2, != 10.0, != 10.1; python_version < "3.13"'],
     'mwoauth': ['mwoauth!=0.3.1,>=0.2.4'],
     'html': ['beautifulsoup4>=4.7.1'],
     'http': ['fake-useragent>=1.4.0'],
     'flake8': [  # Due to incompatibilities between packages the order matters.
         'flake8>=5.0.4',
         'darglint2',
         'pydocstyle>=6.3.0',
@@ -60,15 +60,16 @@
         'flake8-mock-x2',
         'flake8-print>=5.0.0',
         'flake8-quotes>=3.3.2',
         'flake8-raise',
         'flake8-string-format',
         'flake8-tuple>=0.4.1',
         'flake8-no-u-prefixed-strings>=0.2',
-        'pep8-naming>=0.13.3',
+        'pep8-naming==0.13.3; python_version < "3.8"',
+        'pep8-naming>=0.14.0; python_version >= "3.8"',
     ],
     'hacking': [
         'hacking',
         # importlib-metadata module is already installed with hacking 4.1.0
         # used by Python 3.7 but importlib-metadata >= 5 fails, so adjust it
         'importlib-metadata<5.0.0; python_version < "3.8"',
     ],
```

### Comparing `pywikibot-9.1.2/tests/tests_tests.py` & `pywikibot-9.1.3/tests/tests_tests.py`

 * *Files identical despite different names*

