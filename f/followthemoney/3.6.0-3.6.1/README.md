# Comparing `tmp/followthemoney-3.6.0.tar.gz` & `tmp/followthemoney-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.6.0.tar", last modified: Wed May  8 09:30:56 2024, max compression
+gzip compressed data, was "followthemoney-3.6.1.tar", last modified: Tue May 28 10:27:18 2024, max compression
```

## Comparing `followthemoney-3.6.0.tar` & `followthemoney-3.6.1.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.230000 followthemoney-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-08 09:29:16.000000 followthemoney-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 09:29:16.000000 followthemoney-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 09:30:56.230000 followthemoney-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-08 09:29:16.000000 followthemoney-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Occupancy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Position.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   121331 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    93147 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115533 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    32142 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115183 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   119965 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   106802 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   105130 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    90876 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89847 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    64182 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   139453 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   130621 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89829 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.230000 followthemoney-3.6.0/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:36.000000 followthemoney-3.6.0/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 09:30:56.230000 followthemoney-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 09:29:16.000000 followthemoney-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.456751 followthemoney-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 10:25:44.000000 followthemoney-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 10:25:44.000000 followthemoney-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-28 10:27:18.456751 followthemoney-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-28 10:25:44.000000 followthemoney-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.432751 followthemoney-3.6.1/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.432751 followthemoney-3.6.1/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.436751 followthemoney-3.6.1/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.436751 followthemoney-3.6.1/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Occupancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Position.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   121331 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    93147 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115533 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    32142 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115183 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.448751 followthemoney-3.6.1/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   119965 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   106802 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   105130 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    90876 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89847 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    64182 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   139453 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   130621 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.428751 followthemoney-3.6.1/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.452751 followthemoney-3.6.1/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89829 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.456751 followthemoney-3.6.1/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-28 10:25:44.000000 followthemoney-3.6.1/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:27:18.432751 followthemoney-3.6.1/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:26:59.000000 followthemoney-3.6.1/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 10:27:18.000000 followthemoney-3.6.1/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 10:27:18.456751 followthemoney-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-28 10:25:44.000000 followthemoney-3.6.1/setup.py
```

### Comparing `followthemoney-3.6.0/LICENSE` & `followthemoney-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/PKG-INFO` & `followthemoney-3.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.6.0
+Version: 3.6.1
+Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -84,7 +86,9 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
+
+
```

### Comparing `followthemoney-3.6.0/README.md` & `followthemoney-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/aggregate.py` & `followthemoney-3.6.1/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/cli.py` & `followthemoney-3.6.1/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/exports.py` & `followthemoney-3.6.1/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/mapping.py` & `followthemoney-3.6.1/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/sieve.py` & `followthemoney-3.6.1/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/cli/util.py` & `followthemoney-3.6.1/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/compare.py` & `followthemoney-3.6.1/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/exc.py` & `followthemoney-3.6.1/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/common.py` & `followthemoney-3.6.1/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/csv.py` & `followthemoney-3.6.1/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/excel.py` & `followthemoney-3.6.1/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/graph.py` & `followthemoney-3.6.1/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/neo4j.py` & `followthemoney-3.6.1/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/export/rdf.py` & `followthemoney-3.6.1/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/graph.py` & `followthemoney-3.6.1/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/helpers.py` & `followthemoney-3.6.1/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/csv.py` & `followthemoney-3.6.1/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/entity.py` & `followthemoney-3.6.1/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/property.py` & `followthemoney-3.6.1/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/query.py` & `followthemoney-3.6.1/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/source.py` & `followthemoney-3.6.1/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/mapping/sql.py` & `followthemoney-3.6.1/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/messages.py` & `followthemoney-3.6.1/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/model.py` & `followthemoney-3.6.1/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/namespace.py` & `followthemoney-3.6.1/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/offshore.py` & `followthemoney-3.6.1/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/ontology.py` & `followthemoney-3.6.1/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/property.py` & `followthemoney-3.6.1/followthemoney/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/proxy.py` & `followthemoney-3.6.1/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Address.yaml` & `followthemoney-3.6.1/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Airplane.yaml` & `followthemoney-3.6.1/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.6.1/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Assessment.yaml` & `followthemoney-3.6.1/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Associate.yaml` & `followthemoney-3.6.1/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.6.1/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Call.yaml` & `followthemoney-3.6.1/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.6.1/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Company.yaml` & `followthemoney-3.6.1/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Contract.yaml` & `followthemoney-3.6.1/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.6.1/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.6.1/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.6.1/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.6.1/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Debt.yaml` & `followthemoney-3.6.1/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Directorship.yaml` & `followthemoney-3.6.1/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Document.yaml` & `followthemoney-3.6.1/followthemoney/schema/Document.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Documentation.yml` & `followthemoney-3.6.1/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.6.1/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Email.yaml` & `followthemoney-3.6.1/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Employment.yaml` & `followthemoney-3.6.1/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Event.yaml` & `followthemoney-3.6.1/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Family.yaml` & `followthemoney-3.6.1/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Identification.yaml` & `followthemoney-3.6.1/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Interval.yaml` & `followthemoney-3.6.1/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.6.1/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Membership.yaml` & `followthemoney-3.6.1/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Mention.yaml` & `followthemoney-3.6.1/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Message.yaml` & `followthemoney-3.6.1/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Occupancy.yaml` & `followthemoney-3.6.1/followthemoney/schema/Occupancy.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Ownership.yaml` & `followthemoney-3.6.1/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Page.yaml` & `followthemoney-3.6.1/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Passport.yaml` & `followthemoney-3.6.1/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Payment.yaml` & `followthemoney-3.6.1/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Person.yaml` & `followthemoney-3.6.1/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Position.yaml` & `followthemoney-3.6.1/followthemoney/schema/Position.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Post.yaml` & `followthemoney-3.6.1/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.6.1/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.6.1/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Representation.yaml` & `followthemoney-3.6.1/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Sanction.yaml` & `followthemoney-3.6.1/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Security.yaml` & `followthemoney-3.6.1/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Similar.yaml` & `followthemoney-3.6.1/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Succession.yaml` & `followthemoney-3.6.1/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Table.yaml` & `followthemoney-3.6.1/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.6.1/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Thing.yaml` & `followthemoney-3.6.1/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Trip.yaml` & `followthemoney-3.6.1/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.6.1/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.6.1/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.6.1/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema/Vessel.yaml` & `followthemoney-3.6.1/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/schema.py` & `followthemoney-3.6.1/followthemoney/schema.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/messages.pot` & `followthemoney-3.6.1/followthemoney/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/__init__.py` & `followthemoney-3.6.1/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/address.py` & `followthemoney-3.6.1/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/checksum.py` & `followthemoney-3.6.1/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/common.py` & `followthemoney-3.6.1/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/country.py` & `followthemoney-3.6.1/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/date.py` & `followthemoney-3.6.1/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/email.py` & `followthemoney-3.6.1/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/entity.py` & `followthemoney-3.6.1/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/gender.py` & `followthemoney-3.6.1/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/iban.py` & `followthemoney-3.6.1/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/identifier.py` & `followthemoney-3.6.1/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/ip.py` & `followthemoney-3.6.1/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/json.py` & `followthemoney-3.6.1/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/language.py` & `followthemoney-3.6.1/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/mimetype.py` & `followthemoney-3.6.1/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/name.py` & `followthemoney-3.6.1/followthemoney/types/name.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING, Optional, Sequence
 from rigour.text.distance import levenshtein_similarity
 from rigour.names import pick_name
 from normality import slugify
 from normality.cleaning import collapse_spaces, strip_quotes
+from fingerprints.cleanup import clean_name_light
 
 from followthemoney.types.common import PropertyType
 from followthemoney.util import dampen
 from followthemoney.util import defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
@@ -44,14 +45,18 @@
 
     def _specificity(self, value: str) -> float:
         # TODO: insert artificial intelligence here.
         return dampen(3, 50, value)
 
     def compare(self, left: str, right: str) -> float:
         """Compare two names for similarity."""
-        return levenshtein_similarity(left, right)
+        left_clean = clean_name_light(left)
+        right_clean = clean_name_light(right)
+        if left_clean is None or right_clean is None:
+            return 0.0
+        return levenshtein_similarity(left_clean, right_clean)
 
     def node_id(self, value: str) -> Optional[str]:
         slug = slugify(value)
         if slug is None:
             return None
         return f"name:{slug}"
```

### Comparing `followthemoney-3.6.0/followthemoney/types/number.py` & `followthemoney-3.6.1/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/phone.py` & `followthemoney-3.6.1/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/registry.py` & `followthemoney-3.6.1/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/string.py` & `followthemoney-3.6.1/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/types/topic.py` & `followthemoney-3.6.1/followthemoney/types/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         "gov.financial": _("Central banking and financial integrity"),
         "fin": _("Financial services"),
         "fin.bank": _("Bank"),
         "fin.fund": _("Fund"),
         "fin.adivsor": _("Financial advisor"),
         "reg.action": _("Regulator action"),
         "reg.warn": _("Regulator warning"),
-        "role.pep": _("Politican"),
+        "role.pep": _("Politician"),
         "role.pol": _("Non-PEP"),
         "role.rca": _("Close Associate"),
         "role.judge": _("Judge"),
         "role.civil": _("Civil servant"),
         "role.diplo": _("Diplomat"),
         "role.lawyer": _("Lawyer"),
         "role.acct": _("Accountant"),
```

### Comparing `followthemoney-3.6.0/followthemoney/types/url.py` & `followthemoney-3.6.1/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney/util.py` & `followthemoney-3.6.1/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.6.1/followthemoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.6.0
+Version: 3.6.1
+Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -84,7 +86,9 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
+
+
```

### Comparing `followthemoney-3.6.0/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.6.1/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.6.1/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
+
```

### Comparing `followthemoney-3.6.0/followthemoney.egg-info/requires.txt` & `followthemoney-3.6.1/followthemoney.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.6.0/setup.py` & `followthemoney-3.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.6.0",
+    version="3.6.1",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

