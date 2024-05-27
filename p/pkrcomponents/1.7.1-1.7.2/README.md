# Comparing `tmp/pkrcomponents-1.7.1.tar.gz` & `tmp/pkrcomponents-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.7.1.tar", last modified: Mon May 27 17:13:29 2024, max compression
+gzip compressed data, was "pkrcomponents-1.7.2.tar", last modified: Mon May 27 20:41:03 2024, max compression
```

## Comparing `pkrcomponents-1.7.1.tar` & `pkrcomponents-1.7.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.519946 pkrcomponents-1.7.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:28.841163 pkrcomponents-1.7.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 17:13:29.510715 pkrcomponents-1.7.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.1/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/README.rst
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1400 2024-05-27 17:11:19.000000 pkrcomponents-1.7.1/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.224331 pkrcomponents-1.7.1/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.7.1/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.1/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.1/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      628 2024-05-27 15:52:21.000000 pkrcomponents-1.7.1/pkrcomponents/buy_in.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.1/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      790 2024-05-27 15:24:49.000000 pkrcomponents-1.7.1/pkrcomponents/level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.7.1/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.254996 pkrcomponents-1.7.1/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.340250 pkrcomponents-1.7.1/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.1/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.431150 pkrcomponents-1.7.1/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.450161 pkrcomponents-1.7.1/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.1/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2246 2024-05-27 16:04:03.000000 pkrcomponents-1.7.1/pkrcomponents/payout.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.1/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1039 2024-05-27 14:58:43.000000 pkrcomponents-1.7.1/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16718 2024-05-27 11:48:40.000000 pkrcomponents-1.7.1/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12484 2024-05-27 09:29:53.000000 pkrcomponents-1.7.1/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2717 2024-05-27 17:10:53.000000 pkrcomponents-1.7.1/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.485081 pkrcomponents-1.7.1/pkrcomponents/utils/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.1/pkrcomponents/utils/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      365 2024-05-27 17:06:53.000000 pkrcomponents-1.7.1/pkrcomponents/utils/validators.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.500214 pkrcomponents-1.7.1/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      934 2024-05-27 17:13:27.000000 pkrcomponents-1.7.1/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 17:13:29.519946 pkrcomponents-1.7.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.7.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.884316 pkrcomponents-1.7.2/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:02.718520 pkrcomponents-1.7.2/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.2/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.2/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.2/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 20:41:03.884316 pkrcomponents-1.7.2/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.2/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/README.rst
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1456 2024-05-27 20:38:17.000000 pkrcomponents-1.7.2/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.271327 pkrcomponents-1.7.2/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      612 2024-05-27 17:41:46.000000 pkrcomponents-1.7.2/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.2/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.2/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      628 2024-05-27 15:52:21.000000 pkrcomponents-1.7.2/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.2/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.7.2/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.7.2/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      790 2024-05-27 15:24:49.000000 pkrcomponents-1.7.2/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.7.2/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.317924 pkrcomponents-1.7.2/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.502129 pkrcomponents-1.7.2/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.2/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.2/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.2/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.2/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.666610 pkrcomponents-1.7.2/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.2/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.2/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.2/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.717822 pkrcomponents-1.7.2/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.2/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2246 2024-05-27 16:04:03.000000 pkrcomponents-1.7.2/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.2/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1039 2024-05-27 14:58:43.000000 pkrcomponents-1.7.2/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16733 2024-05-27 20:36:01.000000 pkrcomponents-1.7.2/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10491 2024-05-27 20:24:06.000000 pkrcomponents-1.7.2/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2717 2024-05-27 17:10:53.000000 pkrcomponents-1.7.2/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.820506 pkrcomponents-1.7.2/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.2/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.7.2/pkrcomponents/utils/converters.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.7.2/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 20:41:03.867220 pkrcomponents-1.7.2/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      968 2024-05-27 20:41:00.000000 pkrcomponents-1.7.2/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.2/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 20:41:03.884316 pkrcomponents-1.7.2/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.7.2/setup.py
```

### Comparing `pkrcomponents-1.7.1/LICENSE.txt` & `pkrcomponents-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/MANIFEST.in` & `pkrcomponents-1.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/PKG-INFO` & `pkrcomponents-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.7.1/coverage.txt` & `pkrcomponents-1.7.2/coverage.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Name                                Stmts   Miss  Cover
 -------------------------------------------------------
 pkrcomponents/__init__.py               0      0   100%
 pkrcomponents/_common.py               48      0   100%
-pkrcomponents/action.py                32      0   100%
+pkrcomponents/action.py                11      0   100%
 pkrcomponents/bitcard.py               68      0   100%
 pkrcomponents/board.py                 81      0   100%
 pkrcomponents/buy_in.py                14      0   100%
 pkrcomponents/card.py                 112      1    99%
 pkrcomponents/constants.py             71      0   100%
 pkrcomponents/evaluator.py             28      0   100%
-pkrcomponents/hand.py                 226      0   100%
+pkrcomponents/hand.py                 228      0   100%
 pkrcomponents/level.py                 17      0   100%
 pkrcomponents/listings.py              16      0   100%
 pkrcomponents/lookup_table.py         112      0   100%
 pkrcomponents/payout.py                39      0   100%
 pkrcomponents/players.py               96      0   100%
 pkrcomponents/pot.py                   13      0   100%
-pkrcomponents/table.py                326      8    98%
-pkrcomponents/table_player.py         253      4    98%
+pkrcomponents/table.py                327      4    99%
+pkrcomponents/table_player.py         183      2    99%
 pkrcomponents/tournament.py            46      0   100%
 pkrcomponents/utils/__init__.py         0      0   100%
-pkrcomponents/utils/validators.py       7      1    86%
+pkrcomponents/utils/converters.py       6      1    83%
+pkrcomponents/utils/validators.py       7      0   100%
 -------------------------------------------------------
-TOTAL                                1605     14    99%
+TOTAL                                1523      8    99%
```

### Comparing `pkrcomponents-1.7.1/pkrcomponents/_common.py` & `pkrcomponents-1.7.2/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/bitcard.py` & `pkrcomponents-1.7.2/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/board.py` & `pkrcomponents-1.7.2/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/buy_in.py` & `pkrcomponents-1.7.2/pkrcomponents/buy_in.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/card.py` & `pkrcomponents-1.7.2/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/constants.py` & `pkrcomponents-1.7.2/pkrcomponents/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 class MoneyType(PokerEnum):
     """Class describing money type"""
     REAL = "Real money", "Real", "real"
     PLAY = "Play money", "Play", "play"
 
 
-class Action(PokerEnum):
+class ActionMove(PokerEnum):
     """Class describing an action done"""
     BET = "BET", "bet", "bets", "BETS", "Bet", "Bets", "R"
     RAISE = "RAISE", "raise", "raises",  "RAISES", "Raise", "Raises", "R"
     CHECK = "CHECK", "check", "checks", "CHECKS", "Check", "Checks", "X"
     FOLD = "FOLD", "fold", "folded", "folds", "FOLDS", "Fold", "Folds", "F"
     CALL = "CALL", "call", "calls", "CALLS", "Call", "Calls", "C"
     RETURN = "RETURN", "return", "returned", "uncalled", "O"
```

### Comparing `pkrcomponents-1.7.1/pkrcomponents/evaluator.py` & `pkrcomponents-1.7.2/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/hand.py` & `pkrcomponents-1.7.2/pkrcomponents/hand.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,16 @@
 
     _shape: Shape
     __slots__ = ("first", "second")
 
     def __new__(cls, combo):
         if isinstance(combo, Combo):
             return combo
-
+        if not combo:
+            return None
         if len(combo) != 4:
             raise ValueError(f"{combo}, should have a length of 4")
         elif combo[0] == combo[2] and combo[1] == combo[3]:
             raise ValueError(f"{combo!r}, Pair can't have the same suit: {combo[1]!r}")
 
         self = super().__new__(cls)
         self._set_cards_in_order(combo[:2], combo[2:])
```

### Comparing `pkrcomponents-1.7.1/pkrcomponents/level.py` & `pkrcomponents-1.7.2/pkrcomponents/level.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/listings.py` & `pkrcomponents-1.7.2/pkrcomponents/listings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from pkrcomponents.constants import Action, Street, Position
+from pkrcomponents.constants import ActionMove, Street, Position
 from pkrcomponents.card import Card
 from pkrcomponents.hand import Hand
 
-all_actions = np.hstack(list(Action))
+all_actions = np.hstack(list(ActionMove))
 all_cards = np.hstack(list(Card))
 all_combos = np.hstack([hand.to_combos() for hand in list(Hand)])
 all_hands = np.hstack(list(Hand))
 all_positions = np.hstack([position for position in list(Position)])
 all_streets = np.hstack(list(Street))
 str_actions = all_actions.astype(str)
 str_positions = all_positions.astype(str)
```

### Comparing `pkrcomponents-1.7.1/pkrcomponents/lookup_table.py` & `pkrcomponents-1.7.2/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.7.2/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.7.2/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/amount.py` & `pkrcomponents-1.7.2/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.7.2/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.7.2/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.7.2/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.7.2/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/payout.py` & `pkrcomponents-1.7.2/pkrcomponents/payout.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/players.py` & `pkrcomponents-1.7.2/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/pot.py` & `pkrcomponents-1.7.2/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents/table.py` & `pkrcomponents-1.7.2/pkrcomponents/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,14 +388,15 @@
         return sum(pl.init_stack for pl in self.players) / self.players.len
 
     @property
     def average_stack_bb(self):
         """Returns the average stack in big blinds"""
         return round(self.average_stack/self.level.bb, 2)
 
+    @property
     def estimated_players_remaining(self):
         """Returns the estimated number of players remaining in the tournament"""
         return self.tournament.estimated_players_remaining(average_stack=self.average_stack)
 
     def advance_seat_playing(self):
         """Advances seat playing to next available player"""
         player = self.current_player
```

### Comparing `pkrcomponents-1.7.1/pkrcomponents/tournament.py` & `pkrcomponents-1.7.2/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.1/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.7.2/pkrcomponents.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 pkrcomponents/models/actions/sequence.py
 pkrcomponents/models/actions/street.py
 pkrcomponents/models/cards/card.py
 pkrcomponents/models/cards/rank.py
 pkrcomponents/models/cards/suit.py
 pkrcomponents/models/pots/pot.py
 pkrcomponents/utils/__init__.py
+pkrcomponents/utils/converters.py
 pkrcomponents/utils/validators.py
```

### Comparing `pkrcomponents-1.7.1/setup.py` & `pkrcomponents-1.7.2/setup.py`

 * *Files identical despite different names*

