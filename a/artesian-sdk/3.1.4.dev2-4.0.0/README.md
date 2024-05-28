# Comparing `tmp/artesian_sdk-3.1.4.dev2.tar.gz` & `tmp/artesian_sdk-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artesian_sdk-3.1.4.dev2.tar", last modified: Thu Apr 18 16:37:56 2024, max compression
+gzip compressed data, was "artesian_sdk-4.0.0.tar", last modified: Tue May 28 12:51:24 2024, max compression
```

## Comparing `artesian_sdk-3.1.4.dev2.tar` & `artesian_sdk-4.0.0.tar`

### file list

```diff
@@ -1,121 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/workflows/dependency-review.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21348 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestAuction.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestGMEOffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestSearchFacet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryAuction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryMas.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/src/Artesian/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianPolicyConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/BaType.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Market.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Zone.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Granularity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/MarketDataService.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/PagedResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/UpsertData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/AggregationRule.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/ArtesianMetadataFacetType.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/MarketDataType.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/Query/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/ActualQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/AuctionQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/BidAskQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/DefaultPartitionStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/MasQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/QueryService.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/RelativeInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/VersionedQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_Query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/QueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/RequestExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestClientErrorHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestGMEPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMarketDataUpsertData.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.733412 artesian_sdk-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.713412 artesian_sdk-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.713412 artesian_sdk-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.github/workflows/dependency-review.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.713412 artesian_sdk-4.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26744 2024-05-28 12:51:24.733412 artesian_sdk-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24282 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.717412 artesian_sdk-4.0.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestAuction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestGMEOffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestSearchFacet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndDeleteActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndDeleteAuction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndDeleteBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndDeleteMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndDeleteVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndQueryActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndQueryAuction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndQueryBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/samples/TestWriteDataAndQueryMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:51:24.733412 artesian_sdk-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.713412 artesian_sdk-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.717412 artesian_sdk-4.0.0/src/Artesian/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/ArtesianConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/ArtesianPolicyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.717412 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.721412 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/BaType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/Market.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/Scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/Zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Granularity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.721412 artesian_sdk-4.0.0/src/Artesian/MarketData/
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/MarketDataService.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.721412 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/DeleteData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/PagedResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/UpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.725412 artesian_sdk-4.0.0/src/Artesian/MarketData/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Enum/AggregationRule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Enum/ArtesianMetadataFacetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Enum/MarketDataType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/MarketData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.725412 artesian_sdk-4.0.0/src/Artesian/Query/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/ActualQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/AuctionQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/BidAskQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/DefaultPartitionStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/MasQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/QueryService.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/RelativeInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/VersionedQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_Query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.729412 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/QueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/Query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.729412 artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/RequestExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/src/Artesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/Artesian/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.729412 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26744 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:51:24.000000 artesian_sdk-4.0.0/src/artesian_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:24.729412 artesian_sdk-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestClientErrorHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestGMEPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestMarketDataDeleteData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestMarketDataUpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-28 12:51:14.000000 artesian_sdk-4.0.0/tests/helpers.py
```

### Comparing `artesian_sdk-3.1.4.dev2/.github/workflows/python-tests.yml` & `artesian_sdk-4.0.0/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/.gitignore` & `artesian_sdk-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/.vscode/launch.json` & `artesian_sdk-4.0.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/LICENSE` & `artesian_sdk-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/PKG-INFO` & `artesian_sdk-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.1.4.dev2
+Version: 4.0.0
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
         
@@ -415,14 +415,56 @@
 
 Latest Value to propagate the latest value, not older than a certain threshold even if there's no value at the end.
 
 ```python
  .withFillLatestValue("P5D", "True")
 ```
 
+### Query written Versions or Products
+
+Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+```
+
+### Search the MarketData collection with faceted results
+
+Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+searchText = "Riconsegnato_"
+filters = {"ProviderName": ["SNAM", "France"]}
+sorts=["MarketDataId asc"]
+doNotLoadAdditionalInfo=True
+res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+```
+
 ## GME Public Offer
 
 Artesian support Query over GME Public Offers which comes in a custom and dedicated format.
 
 ### Extract GME Public Offer
 
 ```Python
@@ -795,14 +837,19 @@
   )
 
   mkservice.upsertData(auctionRows)
 
 
 ```
 
+
+## Delete Data in Artesian
+
+Using the MarketDataService is possible to delete MarketData and its curves.
+
 ### Delete MarketData in Artesian
 
 Using the MarketDataService is possible to delete MarketData and its curves.
 
 ```Python
 
 from Artesian import ArtesianConfig
@@ -811,54 +858,128 @@
 cfg = ArtesianConfg()
 mkservice = MarketDataService(cfg)
 
 mkservice.deleteMarketData(100042422)
 
 ```
 
-### Query written Versions or Products
+Depending on the Type of the MarketData, the DeletData should be composed as per example below.
 
-Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+### Delete Data in an Actual Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
 
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Versioned Time Series
 
 ```Python
-page = 1
-pageSize = 100
-res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 7, 0),
+    version=datetime(2020, 1, 1, 0)
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-### Search the MarketData collection with faceted results
+### Delte Data in a Market Assessment Time Series
 
-Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+```Python
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
+```
+
+### Delte Data in a Bid Ask Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
 
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Auction Time Series
 
 ```Python
-page = 1
-pageSize = 100
-searchText = "Riconsegnato_"
-filters = {"ProviderName": ["SNAM", "France"]}
-sorts=["MarketDataId asc"]
-doNotLoadAdditionalInfo=True
-res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
 ## Jupyter Support
 
 Artesian SDK uses asyncio internally, this causes a conflict with Jupyter. You can work around this issue by add the following at the beginning of the notebook.
 
 ```python
```

### Comparing `artesian_sdk-3.1.4.dev2/README.md` & `artesian_sdk-4.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -361,14 +361,56 @@
 
 Latest Value to propagate the latest value, not older than a certain threshold even if there's no value at the end.
 
 ```python
  .withFillLatestValue("P5D", "True")
 ```
 
+### Query written Versions or Products
+
+Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+```
+
+### Search the MarketData collection with faceted results
+
+Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+searchText = "Riconsegnato_"
+filters = {"ProviderName": ["SNAM", "France"]}
+sorts=["MarketDataId asc"]
+doNotLoadAdditionalInfo=True
+res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+```
+
 ## GME Public Offer
 
 Artesian support Query over GME Public Offers which comes in a custom and dedicated format.
 
 ### Extract GME Public Offer
 
 ```Python
@@ -741,14 +783,19 @@
   )
 
   mkservice.upsertData(auctionRows)
 
 
 ```
 
+
+## Delete Data in Artesian
+
+Using the MarketDataService is possible to delete MarketData and its curves.
+
 ### Delete MarketData in Artesian
 
 Using the MarketDataService is possible to delete MarketData and its curves.
 
 ```Python
 
 from Artesian import ArtesianConfig
@@ -757,54 +804,128 @@
 cfg = ArtesianConfg()
 mkservice = MarketDataService(cfg)
 
 mkservice.deleteMarketData(100042422)
 
 ```
 
-### Query written Versions or Products
+Depending on the Type of the MarketData, the DeletData should be composed as per example below.
 
-Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+### Delete Data in an Actual Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
 
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Versioned Time Series
 
 ```Python
-page = 1
-pageSize = 100
-res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 7, 0),
+    version=datetime(2020, 1, 1, 0)
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-### Search the MarketData collection with faceted results
+### Delte Data in a Market Assessment Time Series
 
-Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+```Python
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
+```
+
+### Delte Data in a Bid Ask Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
 
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Auction Time Series
 
 ```Python
-page = 1
-pageSize = 100
-searchText = "Riconsegnato_"
-filters = {"ProviderName": ["SNAM", "France"]}
-sorts=["MarketDataId asc"]
-doNotLoadAdditionalInfo=True
-res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
 ## Jupyter Support
 
 Artesian SDK uses asyncio internally, this causes a conflict with Jupyter. You can work around this issue by add the following at the beginning of the notebook.
 
 ```python
```

### Comparing `artesian_sdk-3.1.4.dev2/pyproject.toml` & `artesian_sdk-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestActual.py` & `artesian_sdk-4.0.0/samples/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestAuction.py` & `artesian_sdk-4.0.0/samples/TestAuction.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestSearchFacet.py` & `artesian_sdk-4.0.0/samples/TestSearchFacet.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestVersioned.py` & `artesian_sdk-4.0.0/samples/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryActual.py` & `artesian_sdk-4.0.0/samples/TestWriteDataAndQueryActual.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryAuction.py` & `artesian_sdk-4.0.0/samples/TestWriteDataAndQueryAuction.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryBidAsk.py` & `artesian_sdk-4.0.0/samples/TestWriteDataAndQueryBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryMas.py` & `artesian_sdk-4.0.0/samples/TestWriteDataAndQueryMas.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianConfig.py` & `artesian_sdk-4.0.0/src/Artesian/ArtesianConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianPolicyConfig.py` & `artesian_sdk-4.0.0/src/Artesian/ArtesianPolicyConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Exceptions.py` & `artesian_sdk-4.0.0/src/Artesian/Exceptions.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py` & `artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py` & `artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/__init__.py` & `artesian_sdk-4.0.0/src/Artesian/GMEPublicOffers/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/MarketDataService.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/MarketDataService.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 from typing import List, Optional, cast, Dict
+
+from Artesian.MarketData._Dto import DeleteData
 from .._ClientsExecutor.RequestExecutor import _RequestExecutor
 from .._ClientsExecutor.Client import _Client
 from ..ArtesianConfig import ArtesianConfig
 from ..ArtesianPolicyConfig import ArtesianPolicyConfig
 from ._Dto.PagedResult import PagedResultCurveRangeEntity
 from ._Dto.ArtesianSearchResults import ArtesianSearchResults
 from ._Dto.MarketDataEntityInput import MarketDataEntityInput
@@ -395,14 +397,23 @@
         with self.__client as c:
             await asyncio.gather(*[self.__executor.exec(c.exec, "POST", url, data)])
             return None
 
     def upsertData(self: MarketDataService, data: UpsertData) -> None:
         return _get_event_loop().run_until_complete(self.upsertDataAsync(data))
 
+    async def deleteDataAsync(self: MarketDataService, data: DeleteData) -> None:
+        url = "/marketdata/deletedata"
+        with self.__client as c:
+            await asyncio.gather(*[self.__executor.exec(c.exec, "POST", url, data)])
+            return None
+
+    def deleteData(self: MarketDataService, data: DeleteData) -> None:
+        return _get_event_loop().run_until_complete(self.deleteDataAsync(data))
+
 
 def _get_event_loop() -> asyncio.AbstractEventLoop:
     """
     Wrapper around asyncio get_event_loop.
     Ensures that there is an event loop available.
     An event loop may not be available if the sdk is not run in the main event loop
     """
```

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/CurveRangeEntity.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/CurveRangeEntity.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/PagedResult.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/PagedResult.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/UpsertData.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/UpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/__init__.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/_Dto/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 from .UpsertData import (
     AuctionBidValue,
     AuctionBids,
     BidAskValue,
     MarketAssessmentValue,
     UpsertData,
 )
+from .DeleteData import DeleteData
 
 __all__ = [
     MarketDataEntityOutput.__name__,
     MarketDataEntityInput.__name__,
     CurveRangeEntity.__name__,
     PagedResultCurveRangeEntity.__name__,
     MarketDataIdentifier.__name__,
     AuctionBidValue.__name__,
     AuctionBids.__name__,
     BidAskValue.__name__,
     MarketAssessmentValue.__name__,
     UpsertData.__name__,
+    DeleteData.__name__,
     ArtesianSearchResults.__name__,
     ArtesianMetadataFacet.__name__,
     ArtesianMetadataFacetCount.__name__,
 ]  # type: ignore
```

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/__init__.py` & `artesian_sdk-4.0.0/src/Artesian/MarketData/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     BidAskValue,
     CurveRangeEntity,
     MarketAssessmentValue,
     MarketDataEntityInput,
     MarketDataEntityOutput,
     MarketDataIdentifier,
     UpsertData,
+    DeleteData,
     PagedResultCurveRangeEntity,
     ArtesianSearchResults,
     ArtesianMetadataFacet,
     ArtesianMetadataFacetCount,
 )
 
 __all__ = [
@@ -31,12 +32,13 @@
     CurveRangeEntity.__name__,
     PagedResultCurveRangeEntity.__name__,
     MarketAssessmentValue.__name__,
     MarketDataEntityInput.__name__,
     MarketDataEntityOutput.__name__,
     MarketDataIdentifier.__name__,
     UpsertData.__name__,
+    DeleteData.__name__,
     ArtesianSearchResults.__name__,
     ArtesianMetadataFacet.__name__,
     ArtesianMetadataFacetCount.__name__,
     ArtesianMetadataFacetType.__name__,
 ]  # type: ignore
```

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/ActualQuery.py` & `artesian_sdk-4.0.0/src/Artesian/Query/ActualQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/AuctionQuery.py` & `artesian_sdk-4.0.0/src/Artesian/Query/AuctionQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/BidAskQuery.py` & `artesian_sdk-4.0.0/src/Artesian/Query/BidAskQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/DefaultPartitionStrategy.py` & `artesian_sdk-4.0.0/src/Artesian/Query/DefaultPartitionStrategy.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/MasQuery.py` & `artesian_sdk-4.0.0/src/Artesian/Query/MasQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/QueryService.py` & `artesian_sdk-4.0.0/src/Artesian/Query/QueryService.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/VersionedQuery.py` & `artesian_sdk-4.0.0/src/Artesian/Query/VersionedQuery.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_Query.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_Query.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MasQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/MasQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/QueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/QueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py` & `artesian_sdk-4.0.0/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py` & `artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/Client.py` & `artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/Client.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/RequestExecutor.py` & `artesian_sdk-4.0.0/src/Artesian/_ClientsExecutor/RequestExecutor.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/Artesian/__init__.py` & `artesian_sdk-4.0.0/src/Artesian/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/PKG-INFO` & `artesian_sdk-4.0.0/src/artesian_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.1.4.dev2
+Version: 4.0.0
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
         
@@ -415,14 +415,56 @@
 
 Latest Value to propagate the latest value, not older than a certain threshold even if there's no value at the end.
 
 ```python
  .withFillLatestValue("P5D", "True")
 ```
 
+### Query written Versions or Products
+
+Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+```
+
+### Search the MarketData collection with faceted results
+
+Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+
+```Python
+from Artesian.MarketData import MarketDataService
+
+mds = MarketDataService(cfg)
+
+```
+
+To list MarketData curves
+
+```Python
+page = 1
+pageSize = 100
+searchText = "Riconsegnato_"
+filters = {"ProviderName": ["SNAM", "France"]}
+sorts=["MarketDataId asc"]
+doNotLoadAdditionalInfo=True
+res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+```
+
 ## GME Public Offer
 
 Artesian support Query over GME Public Offers which comes in a custom and dedicated format.
 
 ### Extract GME Public Offer
 
 ```Python
@@ -795,14 +837,19 @@
   )
 
   mkservice.upsertData(auctionRows)
 
 
 ```
 
+
+## Delete Data in Artesian
+
+Using the MarketDataService is possible to delete MarketData and its curves.
+
 ### Delete MarketData in Artesian
 
 Using the MarketDataService is possible to delete MarketData and its curves.
 
 ```Python
 
 from Artesian import ArtesianConfig
@@ -811,54 +858,128 @@
 cfg = ArtesianConfg()
 mkservice = MarketDataService(cfg)
 
 mkservice.deleteMarketData(100042422)
 
 ```
 
-### Query written Versions or Products
+Depending on the Type of the MarketData, the DeletData should be composed as per example below.
 
-Using MarketDataService is possible to query all the Versions and all the Products curves which has been written in a MarketData.
+### Delete Data in an Actual Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
 
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Versioned Time Series
 
 ```Python
-page = 1
-pageSize = 100
-res = mds.readCurveRange(100042422, page, pageSize, versionFrom="2016-12-20" , versionTo="2019-03-12")
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 7, 0),
+    version=datetime(2020, 1, 1, 0)
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-### Search the MarketData collection with faceted results
+### Delte Data in a Market Assessment Time Series
 
-Using MarketDataService is possible to query and search the MarketData collection with faceted results. Supports paging, filtering and free text.
+```Python
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
+```
+
+### Delte Data in a Bid Ask Time Series
 
 ```Python
-from Artesian.MarketData import MarketDataService
+from Artesian import ArtesianConfig, Granularity, MarketData
+from datetime import datetime
+from dateutil import tz
 
-mds = MarketDataService(cfg)
+cfg = ArtesianConfg()
+mkservice = MarketData.MarketDataService(cfg)
 
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID= mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 0),
+    rangeEnd=datetime(2020, 1, 3, 0),
+    product=["Feb-20"]
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
-To list MarketData curves
+### Delete Data in an Auction Time Series
 
 ```Python
-page = 1
-pageSize = 100
-searchText = "Riconsegnato_"
-filters = {"ProviderName": ["SNAM", "France"]}
-sorts=["MarketDataId asc"]
-doNotLoadAdditionalInfo=True
-res = mds.searchFacet(page, pageSize, searchText, filters, sorts, doNotLoadAdditionalInfo)
+from Artesian import ArtesianConfig, Granularity, MarketData
+from Artesian.MarketData import AggregationRule
+from datetime import datetime
+from dateutil import tz
+
+cfg = ArtesianConfg()
+
+mkservice = MarketData.MarketDataService(cfg)
+
+mkdid = MarketData.MarketDataIdentifier('PROVIDER', 'MARKETDATANAME')
+deleteData = MarketData.DeleteData(
+    ID=mkdid,
+    timezone='CET',
+    rangeStart=datetime(2020, 1, 1, 6),
+    rangeEnd=datetime(2020, 1, 1, 18),
+)
+
+mkdservice.deleteData(deleteData)
 ```
 
 ## Jupyter Support
 
 Artesian SDK uses asyncio internally, this causes a conflict with Jupyter. You can work around this issue by add the following at the beginning of the notebook.
 
 ```python
```

### Comparing `artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/SOURCES.txt` & `artesian_sdk-4.0.0/src/artesian_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 samples/TestAuction.py
 samples/TestBidAsk.py
 samples/TestGMEOffers.py
 samples/TestMarketDataService.py
 samples/TestMas.py
 samples/TestSearchFacet.py
 samples/TestVersioned.py
+samples/TestWriteDataAndDeleteActual.py
+samples/TestWriteDataAndDeleteAuction.py
+samples/TestWriteDataAndDeleteBidAsk.py
+samples/TestWriteDataAndDeleteMas.py
+samples/TestWriteDataAndDeleteVersioned.py
 samples/TestWriteDataAndQueryActual.py
 samples/TestWriteDataAndQueryAuction.py
 samples/TestWriteDataAndQueryBidAsk.py
 samples/TestWriteDataAndQueryMas.py
 src/Artesian/.gitignore
 src/Artesian/ArtesianConfig.py
 src/Artesian/ArtesianPolicyConfig.py
@@ -44,14 +49,15 @@
 src/Artesian/GMEPublicOffers/_Enum/Zone.py
 src/Artesian/GMEPublicOffers/_Enum/__init__.py
 src/Artesian/MarketData/MarketDataService.py
 src/Artesian/MarketData/__init__.py
 src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py
 src/Artesian/MarketData/_Dto/ArtesianSearchResults.py
 src/Artesian/MarketData/_Dto/CurveRangeEntity.py
+src/Artesian/MarketData/_Dto/DeleteData.py
 src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
 src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
 src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
 src/Artesian/MarketData/_Dto/PagedResult.py
 src/Artesian/MarketData/_Dto/UpsertData.py
 src/Artesian/MarketData/_Dto/__init__.py
 src/Artesian/MarketData/_Enum/AggregationRule.py
@@ -90,13 +96,14 @@
 src/artesian_sdk.egg-info/dependency_links.txt
 src/artesian_sdk.egg-info/requires.txt
 src/artesian_sdk.egg-info/top_level.txt
 tests/TestActual.py
 tests/TestBidAsk.py
 tests/TestClientErrorHandling.py
 tests/TestGMEPO.py
+tests/TestMarketDataDeleteData.py
 tests/TestMarketDataService.py
 tests/TestMarketDataUpsertData.py
 tests/TestMas.py
 tests/TestVersioned.py
 tests/__init__.py
 tests/helpers.py
```

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestActual.py` & `artesian_sdk-4.0.0/tests/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestBidAsk.py` & `artesian_sdk-4.0.0/tests/TestBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestClientErrorHandling.py` & `artesian_sdk-4.0.0/tests/TestClientErrorHandling.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestGMEPO.py` & `artesian_sdk-4.0.0/tests/TestGMEPO.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestMarketDataService.py` & `artesian_sdk-4.0.0/tests/TestMarketDataService.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestMarketDataUpsertData.py` & `artesian_sdk-4.0.0/tests/TestMarketDataUpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestMas.py` & `artesian_sdk-4.0.0/tests/TestMas.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/TestVersioned.py` & `artesian_sdk-4.0.0/tests/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian_sdk-3.1.4.dev2/tests/helpers.py` & `artesian_sdk-4.0.0/tests/helpers.py`

 * *Files identical despite different names*

