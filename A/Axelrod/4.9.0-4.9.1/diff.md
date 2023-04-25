# Comparing `tmp/Axelrod-4.9.0.tar.gz` & `tmp/Axelrod-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Axelrod-4.9.0.tar", last modified: Tue Apr  7 18:46:34 2020, max compression
+gzip compressed data, was "dist/Axelrod-4.9.1.tar", last modified: Wed Apr  8 11:37:30 2020, max compression
```

## Comparing `Axelrod-4.9.0.tar` & `Axelrod-4.9.1.tar`

### file list

```diff
@@ -1,174 +1,175 @@
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/
--rw-r--r--   0 vince      (501) staff       (20)     7183 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/PKG-INFO
--rw-r--r--   0 vince      (501) staff       (20)     5438 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/SOURCES.txt
--rw-r--r--   0 vince      (501) staff       (20)        1 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/dependency_links.txt
--rw-r--r--   0 vince      (501) staff       (20)      180 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/requires.txt
--rw-r--r--   0 vince      (501) staff       (20)        8 2020-04-07 18:46:34.000000 Axelrod-4.9.0/Axelrod.egg-info/top_level.txt
--rw-r--r--   0 vince      (501) staff       (20)     1178 2019-04-03 18:23:13.000000 Axelrod-4.9.0/LICENSE.txt
--rw-r--r--   0 vince      (501) staff       (20)       80 2019-04-03 18:23:13.000000 Axelrod-4.9.0/MANIFEST.in
--rw-r--r--   0 vince      (501) staff       (20)     7183 2020-04-07 18:46:34.000000 Axelrod-4.9.0/PKG-INFO
--rw-r--r--   0 vince      (501) staff       (20)     5503 2020-04-07 15:56:13.000000 Axelrod-4.9.0/README.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/axelrod/
--rw-r--r--   0 vince      (501) staff       (20)     1001 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/__init__.py
--rw-r--r--   0 vince      (501) staff       (20)     5351 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/_strategy_utils.py
--rw-r--r--   0 vince      (501) staff       (20)     2300 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/action.py
--rw-r--r--   0 vince      (501) staff       (20)     8494 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/classifier.py
--rw-r--r--   0 vince      (501) staff       (20)    10056 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/compute_finite_state_machine_memory.py
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/axelrod/data/
--rw-r--r--   0 vince      (501) staff       (20)     7820 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/data/ann_weights.csv
--rw-r--r--   0 vince      (501) staff       (20)     1440 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/data/pso_gambler.csv
--rw-r--r--   0 vince      (501) staff       (20)     5117 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/deterministic_cache.py
--rw-r--r--   0 vince      (501) staff       (20)     4557 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/ecosystem.py
--rw-r--r--   0 vince      (501) staff       (20)     2452 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/eigen.py
--rw-r--r--   0 vince      (501) staff       (20)     3016 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/evolvable_player.py
--rw-r--r--   0 vince      (501) staff       (20)    20397 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/fingerprint.py
--rw-r--r--   0 vince      (501) staff       (20)     1972 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/game.py
--rw-r--r--   0 vince      (501) staff       (20)     4941 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/graph.py
--rw-r--r--   0 vince      (501) staff       (20)     4135 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/history.py
--rw-r--r--   0 vince      (501) staff       (20)     8600 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/interaction_utils.py
--rw-r--r--   0 vince      (501) staff       (20)     1909 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/load_data_.py
--rw-r--r--   0 vince      (501) staff       (20)     8011 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/match.py
--rw-r--r--   0 vince      (501) staff       (20)     3789 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/match_generator.py
--rw-r--r--   0 vince      (501) staff       (20)      766 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/mock_player.py
--rw-r--r--   0 vince      (501) staff       (20)    18807 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/moran.py
--rw-r--r--   0 vince      (501) staff       (20)     6719 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/player.py
--rw-r--r--   0 vince      (501) staff       (20)    10656 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/plot.py
--rw-r--r--   0 vince      (501) staff       (20)     2141 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/random_.py
--rw-r--r--   0 vince      (501) staff       (20)    26674 2020-04-06 12:09:42.000000 Axelrod-4.9.0/axelrod/result_set.py
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/axelrod/strategies/
--rw-r--r--   0 vince      (501) staff       (20)     3323 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/strategies/__init__.py
--rw-r--r--   0 vince      (501) staff       (20)     6509 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/strategies/_filters.py
--rw-r--r--   0 vince      (501) staff       (20)     9592 2020-04-06 12:09:42.000000 Axelrod-4.9.0/axelrod/strategies/_strategies.py
--rw-r--r--   0 vince      (501) staff       (20)     1697 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/adaptive.py
--rw-r--r--   0 vince      (501) staff       (20)     2534 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/adaptor.py
--rw-r--r--   0 vince      (501) staff       (20)      744 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/alternator.py
--rw-r--r--   0 vince      (501) staff       (20)    11632 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/ann.py
--rw-r--r--   0 vince      (501) staff       (20)     4005 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/apavlov.py
--rw-r--r--   0 vince      (501) staff       (20)     1012 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/appeaser.py
--rw-r--r--   0 vince      (501) staff       (20)     1659 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/averagecopier.py
--rw-r--r--   0 vince      (501) staff       (20)    37651 2020-03-13 16:46:19.000000 Axelrod-4.9.0/axelrod/strategies/axelrod_first.py
--rw-r--r--   0 vince      (501) staff       (20)    74993 2019-12-11 10:14:15.000000 Axelrod-4.9.0/axelrod/strategies/axelrod_second.py
--rw-r--r--   0 vince      (501) staff       (20)     3121 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/backstabber.py
--rw-r--r--   0 vince      (501) staff       (20)      856 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/better_and_better.py
--rw-r--r--   0 vince      (501) staff       (20)     4290 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/bush_mosteller.py
--rw-r--r--   0 vince      (501) staff       (20)     1527 2019-12-11 10:14:15.000000 Axelrod-4.9.0/axelrod/strategies/calculator.py
--rw-r--r--   0 vince      (501) staff       (20)     2053 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/cooperator.py
--rw-r--r--   0 vince      (501) staff       (20)     7234 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/cycler.py
--rw-r--r--   0 vince      (501) staff       (20)     3216 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/darwin.py
--rw-r--r--   0 vince      (501) staff       (20)    18073 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/dbs.py
--rw-r--r--   0 vince      (501) staff       (20)     1495 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/defector.py
--rw-r--r--   0 vince      (501) staff       (20)      866 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/doubler.py
--rw-r--r--   0 vince      (501) staff       (20)    27448 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/finite_state_machines.py
--rw-r--r--   0 vince      (501) staff       (20)     1897 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/forgiver.py
--rw-r--r--   0 vince      (501) staff       (20)     6370 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/gambler.py
--rw-r--r--   0 vince      (501) staff       (20)     3570 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/geller.py
--rw-r--r--   0 vince      (501) staff       (20)     6511 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/gobymajority.py
--rw-r--r--   0 vince      (501) staff       (20)     1076 2020-03-24 17:17:40.000000 Axelrod-4.9.0/axelrod/strategies/gradualkiller.py
--rw-r--r--   0 vince      (501) staff       (20)     8779 2019-11-18 19:16:01.000000 Axelrod-4.9.0/axelrod/strategies/grudger.py
--rw-r--r--   0 vince      (501) staff       (20)     2131 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/grumpy.py
--rw-r--r--   0 vince      (501) staff       (20)     1267 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/handshake.py
--rw-r--r--   0 vince      (501) staff       (20)    14197 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/hmm.py
--rw-r--r--   0 vince      (501) staff       (20)     5694 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/human.py
--rw-r--r--   0 vince      (501) staff       (20)     7306 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/hunter.py
--rw-r--r--   0 vince      (501) staff       (20)     1238 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/inverse.py
--rw-r--r--   0 vince      (501) staff       (20)    20583 2019-10-23 17:10:13.000000 Axelrod-4.9.0/axelrod/strategies/lookerup.py
--rw-r--r--   0 vince      (501) staff       (20)     1855 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/mathematicalconstants.py
--rw-r--r--   0 vince      (501) staff       (20)     9636 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/memoryone.py
--rw-r--r--   0 vince      (501) staff       (20)     8676 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/memorytwo.py
--rw-r--r--   0 vince      (501) staff       (20)    19766 2020-04-07 15:56:17.000000 Axelrod-4.9.0/axelrod/strategies/meta.py
--rw-r--r--   0 vince      (501) staff       (20)     2345 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/mindcontrol.py
--rw-r--r--   0 vince      (501) staff       (20)     3273 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/mindreader.py
--rw-r--r--   0 vince      (501) staff       (20)     2014 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/mutual.py
--rw-r--r--   0 vince      (501) staff       (20)      881 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/negation.py
--rw-r--r--   0 vince      (501) staff       (20)     3379 2019-11-18 19:16:01.000000 Axelrod-4.9.0/axelrod/strategies/oncebitten.py
--rw-r--r--   0 vince      (501) staff       (20)    10648 2019-11-18 19:16:01.000000 Axelrod-4.9.0/axelrod/strategies/prober.py
--rw-r--r--   0 vince      (501) staff       (20)     5225 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/punisher.py
--rw-r--r--   0 vince      (501) staff       (20)     5014 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/qlearner.py
--rw-r--r--   0 vince      (501) staff       (20)     1177 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/rand.py
--rw-r--r--   0 vince      (501) staff       (20)     1976 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/resurrection.py
--rw-r--r--   0 vince      (501) staff       (20)     5672 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/retaliate.py
--rw-r--r--   0 vince      (501) staff       (20)     2135 2019-12-11 10:14:15.000000 Axelrod-4.9.0/axelrod/strategies/revised_downing.py
--rw-r--r--   0 vince      (501) staff       (20)     1583 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/selfsteem.py
--rw-r--r--   0 vince      (501) staff       (20)     3144 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/sequence_player.py
--rw-r--r--   0 vince      (501) staff       (20)     1303 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategies/shortmem.py
--rw-r--r--   0 vince      (501) staff       (20)     2461 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/stalker.py
--rw-r--r--   0 vince      (501) staff       (20)    25523 2020-04-06 12:09:42.000000 Axelrod-4.9.0/axelrod/strategies/titfortat.py
--rw-r--r--   0 vince      (501) staff       (20)     1344 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/verybad.py
--rw-r--r--   0 vince      (501) staff       (20)     3572 2019-04-03 18:23:13.000000 Axelrod-4.9.0/axelrod/strategies/worse_and_worse.py
--rw-r--r--   0 vince      (501) staff       (20)     6169 2020-04-06 12:09:42.000000 Axelrod-4.9.0/axelrod/strategies/zero_determinant.py
--rw-r--r--   0 vince      (501) staff       (20)    22296 2019-04-09 11:48:49.000000 Axelrod-4.9.0/axelrod/strategy_transformers.py
--rw-r--r--   0 vince      (501) staff       (20)    16386 2020-04-06 18:26:52.000000 Axelrod-4.9.0/axelrod/tournament.py
--rw-r--r--   0 vince      (501) staff       (20)       22 2020-04-07 18:39:35.000000 Axelrod-4.9.0/axelrod/version.py
--rw-r--r--   0 vince      (501) staff       (20)     1497 2020-03-25 15:21:32.000000 Axelrod-4.9.0/cache.txt
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/
--rw-r--r--   0 vince      (501) staff       (20)      333 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/citing_the_library.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/community/
--rw-r--r--   0 vince      (501) staff       (20)     3182 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/community/coc.rst
--rw-r--r--   0 vince      (501) staff       (20)      698 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/community/communication.rst
--rw-r--r--   0 vince      (501) staff       (20)      122 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/community/index.rst
--rw-r--r--   0 vince      (501) staff       (20)     1157 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/community/team.rst
--rw-r--r--   0 vince      (501) staff       (20)     3389 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/index.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/reference/
--rw-r--r--   0 vince      (501) staff       (20)     3390 2020-04-06 20:27:20.000000 Axelrod-4.9.0/docs/reference/all_strategies.rst
--rw-r--r--   0 vince      (501) staff       (20)    10842 2020-04-06 12:09:42.000000 Axelrod-4.9.0/docs/reference/bibliography.rst
--rw-r--r--   0 vince      (501) staff       (20)     2720 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/reference/description.rst
--rw-r--r--   0 vince      (501) staff       (20)     6340 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/reference/fortan_keys.rst
--rw-r--r--   0 vince      (501) staff       (20)     2745 2019-04-09 11:48:49.000000 Axelrod-4.9.0/docs/reference/glossary.rst
--rw-r--r--   0 vince      (501) staff       (20)      270 2020-04-06 15:23:13.000000 Axelrod-4.9.0/docs/reference/index.rst
--rw-r--r--   0 vince      (501) staff       (20)    21512 2020-04-06 12:09:42.000000 Axelrod-4.9.0/docs/reference/overview_of_strategies.rst
--rw-r--r--   0 vince      (501) staff       (20)     1286 2020-04-06 15:35:51.000000 Axelrod-4.9.0/docs/reference/play_contexts.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/advanced/
--rw-r--r--   0 vince      (501) staff       (20)     4094 2020-04-07 15:56:17.000000 Axelrod-4.9.0/docs/tutorials/advanced/classification_of_strategies.rst
--rw-r--r--   0 vince      (501) staff       (20)     1527 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/games.rst
--rw-r--r--   0 vince      (501) staff       (20)      473 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/index.rst
--rw-r--r--   0 vince      (501) staff       (20)      472 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/parallel_processing.rst
--rw-r--r--   0 vince      (501) staff       (20)      657 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/player_equality.rst
--rw-r--r--   0 vince      (501) staff       (20)     1150 2019-12-11 10:14:15.000000 Axelrod-4.9.0/docs/tutorials/advanced/player_information.rst
--rw-r--r--   0 vince      (501) staff       (20)     8761 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/reading_and_writing_interactions.rst
--rw-r--r--   0 vince      (501) staff       (20)     1027 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/setting_a_seed.rst
--rw-r--r--   0 vince      (501) staff       (20)     1377 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/strategies.rst
--rw-r--r--   0 vince      (501) staff       (20)     9569 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/strategy_transformers.rst
--rw-r--r--   0 vince      (501) staff       (20)    12506 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/tournament_results.rst
--rw-r--r--   0 vince      (501) staff       (20)     2780 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/advanced/using_the_cache.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/contributing/
--rw-r--r--   0 vince      (501) staff       (20)     1806 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/guidelines.rst
--rw-r--r--   0 vince      (501) staff       (20)      244 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/index.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/contributing/library/
--rw-r--r--   0 vince      (501) staff       (20)      413 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/library/index.rst
--rw-r--r--   0 vince      (501) staff       (20)     2610 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/running_tests.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/
--rw-r--r--   0 vince      (501) staff       (20)     1252 2020-04-07 15:56:17.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/adding_the_new_strategy.rst
--rw-r--r--   0 vince      (501) staff       (20)     2229 2020-04-07 15:56:17.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/classifying_the_new_strategy.rst
--rw-r--r--   0 vince      (501) staff       (20)     1511 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/docstrings.rst
--rw-r--r--   0 vince      (501) staff       (20)      377 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/index.rst
--rw-r--r--   0 vince      (501) staff       (20)     1745 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/instructions.rst
--rw-r--r--   0 vince      (501) staff       (20)     5772 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/writing_test_for_the_new_strategy.rst
--rw-r--r--   0 vince      (501) staff       (20)     5117 2019-04-03 18:23:13.000000 Axelrod-4.9.0/docs/tutorials/contributing/strategy/writing_the_new_strategy.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/further_topics/
--rw-r--r--   0 vince      (501) staff       (20)     1527 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/approximate_moran_processes.rst
--rw-r--r--   0 vince      (501) staff       (20)     1094 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/ecological_variant.rst
--rw-r--r--   0 vince      (501) staff       (20)     1893 2019-11-18 19:16:01.000000 Axelrod-4.9.0/docs/tutorials/further_topics/evolvable_players.rst
--rw-r--r--   0 vince      (501) staff       (20)     4160 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/fingerprinting.rst
--rw-r--r--   0 vince      (501) staff       (20)      460 2019-10-23 17:10:13.000000 Axelrod-4.9.0/docs/tutorials/further_topics/index.rst
--rw-r--r--   0 vince      (501) staff       (20)     3066 2019-04-09 11:48:49.000000 Axelrod-4.9.0/docs/tutorials/further_topics/meta_strategies.rst
--rw-r--r--   0 vince      (501) staff       (20)     1822 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/morality_metrics.rst
--rw-r--r--   0 vince      (501) staff       (20)     1967 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/moran_processes_on_graphs.rst
--rw-r--r--   0 vince      (501) staff       (20)     1496 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/noisy_tournaments.rst
--rw-r--r--   0 vince      (501) staff       (20)     1743 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/probabilistict_end_tournaments.rst
--rw-r--r--   0 vince      (501) staff       (20)     2414 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/further_topics/spatial_tournaments.rst
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-07 18:46:34.000000 Axelrod-4.9.0/docs/tutorials/getting_started/
--rw-r--r--   0 vince      (501) staff       (20)      741 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/getting_started/human_interaction.rst
--rw-r--r--   0 vince      (501) staff       (20)      401 2019-12-11 10:14:15.000000 Axelrod-4.9.0/docs/tutorials/getting_started/index.rst
--rw-r--r--   0 vince      (501) staff       (20)      362 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/getting_started/installation.rst
--rw-r--r--   0 vince      (501) staff       (20)     3646 2020-04-06 18:51:15.000000 Axelrod-4.9.0/docs/tutorials/getting_started/match.rst
--rw-r--r--   0 vince      (501) staff       (20)     4840 2019-10-23 17:10:13.000000 Axelrod-4.9.0/docs/tutorials/getting_started/moran.rst
--rw-r--r--   0 vince      (501) staff       (20)     6739 2019-12-11 10:14:15.000000 Axelrod-4.9.0/docs/tutorials/getting_started/running_axelrods_first_tournament.rst
--rw-r--r--   0 vince      (501) staff       (20)     2212 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/getting_started/summarising_tournaments.rst
--rw-r--r--   0 vince      (501) staff       (20)     1081 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/getting_started/tournament.rst
--rw-r--r--   0 vince      (501) staff       (20)     2193 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/getting_started/visualising_results.rst
--rw-r--r--   0 vince      (501) staff       (20)      261 2019-04-03 18:23:14.000000 Axelrod-4.9.0/docs/tutorials/index.rst
--rw-r--r--   0 vince      (501) staff       (20)      196 2020-04-07 15:56:17.000000 Axelrod-4.9.0/requirements.txt
--rw-r--r--   0 vince      (501) staff       (20)       67 2020-04-07 18:46:34.000000 Axelrod-4.9.0/setup.cfg
--rw-r--r--   0 vince      (501) staff       (20)     1253 2020-04-07 15:56:13.000000 Axelrod-4.9.0/setup.py
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/
+-rw-r--r--   0 vince      (501) staff       (20)     7183 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/PKG-INFO
+-rw-r--r--   0 vince      (501) staff       (20)     5471 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/SOURCES.txt
+-rw-r--r--   0 vince      (501) staff       (20)        1 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/dependency_links.txt
+-rw-r--r--   0 vince      (501) staff       (20)      180 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/requires.txt
+-rw-r--r--   0 vince      (501) staff       (20)        8 2020-04-08 11:37:29.000000 Axelrod-4.9.1/Axelrod.egg-info/top_level.txt
+-rw-r--r--   0 vince      (501) staff       (20)     1178 2019-04-03 18:23:13.000000 Axelrod-4.9.1/LICENSE.txt
+-rw-r--r--   0 vince      (501) staff       (20)       76 2020-04-08 11:31:13.000000 Axelrod-4.9.1/MANIFEST.in
+-rw-r--r--   0 vince      (501) staff       (20)     7183 2020-04-08 11:37:30.000000 Axelrod-4.9.1/PKG-INFO
+-rw-r--r--   0 vince      (501) staff       (20)     5503 2020-04-08 11:31:09.000000 Axelrod-4.9.1/README.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/axelrod/
+-rw-r--r--   0 vince      (501) staff       (20)     1001 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/__init__.py
+-rw-r--r--   0 vince      (501) staff       (20)     5351 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/_strategy_utils.py
+-rw-r--r--   0 vince      (501) staff       (20)     2300 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/action.py
+-rw-r--r--   0 vince      (501) staff       (20)     8494 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/classifier.py
+-rw-r--r--   0 vince      (501) staff       (20)    10056 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/compute_finite_state_machine_memory.py
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/axelrod/data/
+-rw-r--r--   0 vince      (501) staff       (20)    45345 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/data/all_classifiers.yml
+-rw-r--r--   0 vince      (501) staff       (20)     7820 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/data/ann_weights.csv
+-rw-r--r--   0 vince      (501) staff       (20)     1440 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/data/pso_gambler.csv
+-rw-r--r--   0 vince      (501) staff       (20)     5117 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/deterministic_cache.py
+-rw-r--r--   0 vince      (501) staff       (20)     4557 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/ecosystem.py
+-rw-r--r--   0 vince      (501) staff       (20)     2452 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/eigen.py
+-rw-r--r--   0 vince      (501) staff       (20)     3016 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/evolvable_player.py
+-rw-r--r--   0 vince      (501) staff       (20)    20397 2019-10-23 17:10:13.000000 Axelrod-4.9.1/axelrod/fingerprint.py
+-rw-r--r--   0 vince      (501) staff       (20)     1972 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/game.py
+-rw-r--r--   0 vince      (501) staff       (20)     4941 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/graph.py
+-rw-r--r--   0 vince      (501) staff       (20)     4135 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/history.py
+-rw-r--r--   0 vince      (501) staff       (20)     8600 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/interaction_utils.py
+-rw-r--r--   0 vince      (501) staff       (20)     1909 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/load_data_.py
+-rw-r--r--   0 vince      (501) staff       (20)     8011 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/match.py
+-rw-r--r--   0 vince      (501) staff       (20)     3789 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/match_generator.py
+-rw-r--r--   0 vince      (501) staff       (20)      766 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/mock_player.py
+-rw-r--r--   0 vince      (501) staff       (20)    18807 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/moran.py
+-rw-r--r--   0 vince      (501) staff       (20)     6719 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/player.py
+-rw-r--r--   0 vince      (501) staff       (20)    10656 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/plot.py
+-rw-r--r--   0 vince      (501) staff       (20)     2141 2019-10-23 17:10:13.000000 Axelrod-4.9.1/axelrod/random_.py
+-rw-r--r--   0 vince      (501) staff       (20)    26674 2020-04-06 12:09:42.000000 Axelrod-4.9.1/axelrod/result_set.py
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/axelrod/strategies/
+-rw-r--r--   0 vince      (501) staff       (20)     3323 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/strategies/__init__.py
+-rw-r--r--   0 vince      (501) staff       (20)     6509 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/strategies/_filters.py
+-rw-r--r--   0 vince      (501) staff       (20)     9592 2020-04-06 12:09:42.000000 Axelrod-4.9.1/axelrod/strategies/_strategies.py
+-rw-r--r--   0 vince      (501) staff       (20)     1697 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/adaptive.py
+-rw-r--r--   0 vince      (501) staff       (20)     2534 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/adaptor.py
+-rw-r--r--   0 vince      (501) staff       (20)      744 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/alternator.py
+-rw-r--r--   0 vince      (501) staff       (20)    11632 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/ann.py
+-rw-r--r--   0 vince      (501) staff       (20)     4005 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/apavlov.py
+-rw-r--r--   0 vince      (501) staff       (20)     1012 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/appeaser.py
+-rw-r--r--   0 vince      (501) staff       (20)     1659 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/averagecopier.py
+-rw-r--r--   0 vince      (501) staff       (20)    37651 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/axelrod_first.py
+-rw-r--r--   0 vince      (501) staff       (20)    74993 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/axelrod_second.py
+-rw-r--r--   0 vince      (501) staff       (20)     3121 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/backstabber.py
+-rw-r--r--   0 vince      (501) staff       (20)      856 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/better_and_better.py
+-rw-r--r--   0 vince      (501) staff       (20)     4290 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/bush_mosteller.py
+-rw-r--r--   0 vince      (501) staff       (20)     1527 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/calculator.py
+-rw-r--r--   0 vince      (501) staff       (20)     2053 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/cooperator.py
+-rw-r--r--   0 vince      (501) staff       (20)     7234 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/cycler.py
+-rw-r--r--   0 vince      (501) staff       (20)     3216 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/darwin.py
+-rw-r--r--   0 vince      (501) staff       (20)    18073 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/dbs.py
+-rw-r--r--   0 vince      (501) staff       (20)     1495 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/defector.py
+-rw-r--r--   0 vince      (501) staff       (20)      866 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/doubler.py
+-rw-r--r--   0 vince      (501) staff       (20)    27448 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/finite_state_machines.py
+-rw-r--r--   0 vince      (501) staff       (20)     1897 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/forgiver.py
+-rw-r--r--   0 vince      (501) staff       (20)     6370 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/gambler.py
+-rw-r--r--   0 vince      (501) staff       (20)     3570 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/geller.py
+-rw-r--r--   0 vince      (501) staff       (20)     6511 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/gobymajority.py
+-rw-r--r--   0 vince      (501) staff       (20)     1076 2020-03-24 17:17:40.000000 Axelrod-4.9.1/axelrod/strategies/gradualkiller.py
+-rw-r--r--   0 vince      (501) staff       (20)     8779 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/grudger.py
+-rw-r--r--   0 vince      (501) staff       (20)     2131 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/grumpy.py
+-rw-r--r--   0 vince      (501) staff       (20)     1267 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/handshake.py
+-rw-r--r--   0 vince      (501) staff       (20)    14197 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/hmm.py
+-rw-r--r--   0 vince      (501) staff       (20)     5694 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/human.py
+-rw-r--r--   0 vince      (501) staff       (20)     7306 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/hunter.py
+-rw-r--r--   0 vince      (501) staff       (20)     1238 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/inverse.py
+-rw-r--r--   0 vince      (501) staff       (20)    20583 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/lookerup.py
+-rw-r--r--   0 vince      (501) staff       (20)     1855 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/mathematicalconstants.py
+-rw-r--r--   0 vince      (501) staff       (20)     9636 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/memoryone.py
+-rw-r--r--   0 vince      (501) staff       (20)     8676 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/memorytwo.py
+-rw-r--r--   0 vince      (501) staff       (20)    19766 2020-04-08 10:25:34.000000 Axelrod-4.9.1/axelrod/strategies/meta.py
+-rw-r--r--   0 vince      (501) staff       (20)     2345 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/mindcontrol.py
+-rw-r--r--   0 vince      (501) staff       (20)     3273 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/mindreader.py
+-rw-r--r--   0 vince      (501) staff       (20)     2014 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/mutual.py
+-rw-r--r--   0 vince      (501) staff       (20)      881 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/negation.py
+-rw-r--r--   0 vince      (501) staff       (20)     3379 2019-11-18 19:16:01.000000 Axelrod-4.9.1/axelrod/strategies/oncebitten.py
+-rw-r--r--   0 vince      (501) staff       (20)    10648 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/prober.py
+-rw-r--r--   0 vince      (501) staff       (20)     5225 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/punisher.py
+-rw-r--r--   0 vince      (501) staff       (20)     5014 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/qlearner.py
+-rw-r--r--   0 vince      (501) staff       (20)     1177 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/rand.py
+-rw-r--r--   0 vince      (501) staff       (20)     1976 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/resurrection.py
+-rw-r--r--   0 vince      (501) staff       (20)     5672 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/retaliate.py
+-rw-r--r--   0 vince      (501) staff       (20)     2135 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/revised_downing.py
+-rw-r--r--   0 vince      (501) staff       (20)     1583 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/selfsteem.py
+-rw-r--r--   0 vince      (501) staff       (20)     3144 2019-04-09 11:48:49.000000 Axelrod-4.9.1/axelrod/strategies/sequence_player.py
+-rw-r--r--   0 vince      (501) staff       (20)     1303 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategies/shortmem.py
+-rw-r--r--   0 vince      (501) staff       (20)     2461 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/stalker.py
+-rw-r--r--   0 vince      (501) staff       (20)    25523 2020-04-06 12:09:42.000000 Axelrod-4.9.1/axelrod/strategies/titfortat.py
+-rw-r--r--   0 vince      (501) staff       (20)     1344 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/verybad.py
+-rw-r--r--   0 vince      (501) staff       (20)     3572 2019-04-03 18:23:13.000000 Axelrod-4.9.1/axelrod/strategies/worse_and_worse.py
+-rw-r--r--   0 vince      (501) staff       (20)     6169 2020-04-06 12:09:42.000000 Axelrod-4.9.1/axelrod/strategies/zero_determinant.py
+-rw-r--r--   0 vince      (501) staff       (20)    22296 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/strategy_transformers.py
+-rw-r--r--   0 vince      (501) staff       (20)    16386 2020-04-08 08:38:49.000000 Axelrod-4.9.1/axelrod/tournament.py
+-rw-r--r--   0 vince      (501) staff       (20)       22 2020-04-08 11:34:39.000000 Axelrod-4.9.1/axelrod/version.py
+-rw-r--r--   0 vince      (501) staff       (20)     1497 2020-03-25 15:21:32.000000 Axelrod-4.9.1/cache.txt
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/
+-rw-r--r--   0 vince      (501) staff       (20)      333 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/citing_the_library.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/community/
+-rw-r--r--   0 vince      (501) staff       (20)     3182 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/community/coc.rst
+-rw-r--r--   0 vince      (501) staff       (20)      698 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/community/communication.rst
+-rw-r--r--   0 vince      (501) staff       (20)      122 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/community/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1157 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/community/team.rst
+-rw-r--r--   0 vince      (501) staff       (20)     3389 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/index.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/reference/
+-rw-r--r--   0 vince      (501) staff       (20)     3390 2020-04-06 20:27:20.000000 Axelrod-4.9.1/docs/reference/all_strategies.rst
+-rw-r--r--   0 vince      (501) staff       (20)    10842 2020-04-06 12:09:42.000000 Axelrod-4.9.1/docs/reference/bibliography.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2720 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/reference/description.rst
+-rw-r--r--   0 vince      (501) staff       (20)     6340 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/reference/fortan_keys.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2745 2019-04-09 11:48:49.000000 Axelrod-4.9.1/docs/reference/glossary.rst
+-rw-r--r--   0 vince      (501) staff       (20)      270 2020-04-06 15:23:13.000000 Axelrod-4.9.1/docs/reference/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)    21512 2020-04-06 12:09:42.000000 Axelrod-4.9.1/docs/reference/overview_of_strategies.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1286 2020-04-06 15:35:51.000000 Axelrod-4.9.1/docs/reference/play_contexts.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/advanced/
+-rw-r--r--   0 vince      (501) staff       (20)     4094 2020-04-08 10:25:34.000000 Axelrod-4.9.1/docs/tutorials/advanced/classification_of_strategies.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1527 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/games.rst
+-rw-r--r--   0 vince      (501) staff       (20)      473 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)      472 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/parallel_processing.rst
+-rw-r--r--   0 vince      (501) staff       (20)      657 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/player_equality.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1150 2019-12-11 10:14:15.000000 Axelrod-4.9.1/docs/tutorials/advanced/player_information.rst
+-rw-r--r--   0 vince      (501) staff       (20)     8761 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/reading_and_writing_interactions.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1027 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/setting_a_seed.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1377 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/strategies.rst
+-rw-r--r--   0 vince      (501) staff       (20)     9569 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/strategy_transformers.rst
+-rw-r--r--   0 vince      (501) staff       (20)    12506 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/tournament_results.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2780 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/advanced/using_the_cache.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/contributing/
+-rw-r--r--   0 vince      (501) staff       (20)     1806 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/guidelines.rst
+-rw-r--r--   0 vince      (501) staff       (20)      244 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/index.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/contributing/library/
+-rw-r--r--   0 vince      (501) staff       (20)      413 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/library/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2610 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/running_tests.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/
+-rw-r--r--   0 vince      (501) staff       (20)     1252 2020-04-08 10:25:34.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/adding_the_new_strategy.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2229 2020-04-08 10:25:34.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/classifying_the_new_strategy.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1511 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/docstrings.rst
+-rw-r--r--   0 vince      (501) staff       (20)      377 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1745 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/instructions.rst
+-rw-r--r--   0 vince      (501) staff       (20)     5772 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/writing_test_for_the_new_strategy.rst
+-rw-r--r--   0 vince      (501) staff       (20)     5117 2019-04-03 18:23:13.000000 Axelrod-4.9.1/docs/tutorials/contributing/strategy/writing_the_new_strategy.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/further_topics/
+-rw-r--r--   0 vince      (501) staff       (20)     1527 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/approximate_moran_processes.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1094 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/ecological_variant.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1893 2019-11-18 19:16:01.000000 Axelrod-4.9.1/docs/tutorials/further_topics/evolvable_players.rst
+-rw-r--r--   0 vince      (501) staff       (20)     4160 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/fingerprinting.rst
+-rw-r--r--   0 vince      (501) staff       (20)      460 2019-10-23 17:10:13.000000 Axelrod-4.9.1/docs/tutorials/further_topics/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)     3066 2019-04-09 11:48:49.000000 Axelrod-4.9.1/docs/tutorials/further_topics/meta_strategies.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1822 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/morality_metrics.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1967 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/moran_processes_on_graphs.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1496 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/noisy_tournaments.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1743 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/probabilistict_end_tournaments.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2414 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/further_topics/spatial_tournaments.rst
+drwxr-xr-x   0 vince      (501) staff       (20)        0 2020-04-08 11:37:30.000000 Axelrod-4.9.1/docs/tutorials/getting_started/
+-rw-r--r--   0 vince      (501) staff       (20)      741 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/getting_started/human_interaction.rst
+-rw-r--r--   0 vince      (501) staff       (20)      401 2019-12-11 10:14:15.000000 Axelrod-4.9.1/docs/tutorials/getting_started/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)      362 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/getting_started/installation.rst
+-rw-r--r--   0 vince      (501) staff       (20)     3646 2020-04-06 18:51:15.000000 Axelrod-4.9.1/docs/tutorials/getting_started/match.rst
+-rw-r--r--   0 vince      (501) staff       (20)     4840 2019-10-23 17:10:13.000000 Axelrod-4.9.1/docs/tutorials/getting_started/moran.rst
+-rw-r--r--   0 vince      (501) staff       (20)     6739 2019-12-11 10:14:15.000000 Axelrod-4.9.1/docs/tutorials/getting_started/running_axelrods_first_tournament.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2212 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/getting_started/summarising_tournaments.rst
+-rw-r--r--   0 vince      (501) staff       (20)     1081 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/getting_started/tournament.rst
+-rw-r--r--   0 vince      (501) staff       (20)     2193 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/getting_started/visualising_results.rst
+-rw-r--r--   0 vince      (501) staff       (20)      261 2019-04-03 18:23:14.000000 Axelrod-4.9.1/docs/tutorials/index.rst
+-rw-r--r--   0 vince      (501) staff       (20)      196 2020-04-08 11:31:09.000000 Axelrod-4.9.1/requirements.txt
+-rw-r--r--   0 vince      (501) staff       (20)       67 2020-04-08 11:37:30.000000 Axelrod-4.9.1/setup.cfg
+-rw-r--r--   0 vince      (501) staff       (20)     1249 2020-04-08 11:31:13.000000 Axelrod-4.9.1/setup.py
```

### Comparing `Axelrod-4.9.0/Axelrod.egg-info/PKG-INFO` & `Axelrod-4.9.1/Axelrod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Axelrod
-Version: 4.9.0
+Version: 4.9.1
 Summary: Reproduce the Axelrod iterated prisoners dilemma tournament
 Home-page: http://axelrod.readthedocs.org/
 Author: Vince Knight, Owen Campbell, Karol Langner, Marc Harper
 Author-email: axelrod-python@googlegroups.com
 License: The MIT License (MIT)
 Description: .. image:: https://coveralls.io/repos/github/Axelrod-Python/Axelrod/badge.svg?branch=master
             :target: https://coveralls.io/github/Axelrod-Python/Axelrod?branch=master
```

### Comparing `Axelrod-4.9.0/Axelrod.egg-info/SOURCES.txt` & `Axelrod-4.9.1/Axelrod.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 axelrod/player.py
 axelrod/plot.py
 axelrod/random_.py
 axelrod/result_set.py
 axelrod/strategy_transformers.py
 axelrod/tournament.py
 axelrod/version.py
+axelrod/data/all_classifiers.yml
 axelrod/data/ann_weights.csv
 axelrod/data/pso_gambler.csv
 axelrod/strategies/__init__.py
 axelrod/strategies/_filters.py
 axelrod/strategies/_strategies.py
 axelrod/strategies/adaptive.py
 axelrod/strategies/adaptor.py
```

### Comparing `Axelrod-4.9.0/LICENSE.txt` & `Axelrod-4.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/PKG-INFO` & `Axelrod-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Axelrod
-Version: 4.9.0
+Version: 4.9.1
 Summary: Reproduce the Axelrod iterated prisoners dilemma tournament
 Home-page: http://axelrod.readthedocs.org/
 Author: Vince Knight, Owen Campbell, Karol Langner, Marc Harper
 Author-email: axelrod-python@googlegroups.com
 License: The MIT License (MIT)
 Description: .. image:: https://coveralls.io/repos/github/Axelrod-Python/Axelrod/badge.svg?branch=master
             :target: https://coveralls.io/github/Axelrod-Python/Axelrod?branch=master
```

### Comparing `Axelrod-4.9.0/README.rst` & `Axelrod-4.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/__init__.py` & `Axelrod-4.9.1/axelrod/__init__.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/_strategy_utils.py` & `Axelrod-4.9.1/axelrod/_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/action.py` & `Axelrod-4.9.1/axelrod/action.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/classifier.py` & `Axelrod-4.9.1/axelrod/classifier.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/compute_finite_state_machine_memory.py` & `Axelrod-4.9.1/axelrod/compute_finite_state_machine_memory.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/data/ann_weights.csv` & `Axelrod-4.9.1/axelrod/data/ann_weights.csv`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/data/pso_gambler.csv` & `Axelrod-4.9.1/axelrod/data/pso_gambler.csv`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/deterministic_cache.py` & `Axelrod-4.9.1/axelrod/deterministic_cache.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/ecosystem.py` & `Axelrod-4.9.1/axelrod/ecosystem.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/eigen.py` & `Axelrod-4.9.1/axelrod/eigen.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/evolvable_player.py` & `Axelrod-4.9.1/axelrod/evolvable_player.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/fingerprint.py` & `Axelrod-4.9.1/axelrod/fingerprint.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/game.py` & `Axelrod-4.9.1/axelrod/game.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/graph.py` & `Axelrod-4.9.1/axelrod/graph.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/history.py` & `Axelrod-4.9.1/axelrod/history.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/interaction_utils.py` & `Axelrod-4.9.1/axelrod/interaction_utils.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/load_data_.py` & `Axelrod-4.9.1/axelrod/load_data_.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/match.py` & `Axelrod-4.9.1/axelrod/match.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/match_generator.py` & `Axelrod-4.9.1/axelrod/match_generator.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/mock_player.py` & `Axelrod-4.9.1/axelrod/mock_player.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/moran.py` & `Axelrod-4.9.1/axelrod/moran.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/player.py` & `Axelrod-4.9.1/axelrod/player.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/plot.py` & `Axelrod-4.9.1/axelrod/plot.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/random_.py` & `Axelrod-4.9.1/axelrod/random_.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/result_set.py` & `Axelrod-4.9.1/axelrod/result_set.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/__init__.py` & `Axelrod-4.9.1/axelrod/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/_filters.py` & `Axelrod-4.9.1/axelrod/strategies/_filters.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/_strategies.py` & `Axelrod-4.9.1/axelrod/strategies/_strategies.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/adaptive.py` & `Axelrod-4.9.1/axelrod/strategies/adaptive.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/adaptor.py` & `Axelrod-4.9.1/axelrod/strategies/adaptor.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/alternator.py` & `Axelrod-4.9.1/axelrod/strategies/alternator.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/ann.py` & `Axelrod-4.9.1/axelrod/strategies/ann.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/apavlov.py` & `Axelrod-4.9.1/axelrod/strategies/apavlov.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/appeaser.py` & `Axelrod-4.9.1/axelrod/strategies/appeaser.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/averagecopier.py` & `Axelrod-4.9.1/axelrod/strategies/averagecopier.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/axelrod_first.py` & `Axelrod-4.9.1/axelrod/strategies/axelrod_first.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/axelrod_second.py` & `Axelrod-4.9.1/axelrod/strategies/axelrod_second.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/backstabber.py` & `Axelrod-4.9.1/axelrod/strategies/backstabber.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/better_and_better.py` & `Axelrod-4.9.1/axelrod/strategies/better_and_better.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/bush_mosteller.py` & `Axelrod-4.9.1/axelrod/strategies/bush_mosteller.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/calculator.py` & `Axelrod-4.9.1/axelrod/strategies/calculator.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/cooperator.py` & `Axelrod-4.9.1/axelrod/strategies/cooperator.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/cycler.py` & `Axelrod-4.9.1/axelrod/strategies/cycler.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/darwin.py` & `Axelrod-4.9.1/axelrod/strategies/darwin.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/dbs.py` & `Axelrod-4.9.1/axelrod/strategies/dbs.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/defector.py` & `Axelrod-4.9.1/axelrod/strategies/defector.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/doubler.py` & `Axelrod-4.9.1/axelrod/strategies/doubler.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/finite_state_machines.py` & `Axelrod-4.9.1/axelrod/strategies/finite_state_machines.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/forgiver.py` & `Axelrod-4.9.1/axelrod/strategies/forgiver.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/gambler.py` & `Axelrod-4.9.1/axelrod/strategies/gambler.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/geller.py` & `Axelrod-4.9.1/axelrod/strategies/geller.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/gobymajority.py` & `Axelrod-4.9.1/axelrod/strategies/gobymajority.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/gradualkiller.py` & `Axelrod-4.9.1/axelrod/strategies/gradualkiller.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/grudger.py` & `Axelrod-4.9.1/axelrod/strategies/grudger.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/grumpy.py` & `Axelrod-4.9.1/axelrod/strategies/grumpy.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/handshake.py` & `Axelrod-4.9.1/axelrod/strategies/handshake.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/hmm.py` & `Axelrod-4.9.1/axelrod/strategies/hmm.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/human.py` & `Axelrod-4.9.1/axelrod/strategies/human.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/hunter.py` & `Axelrod-4.9.1/axelrod/strategies/hunter.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/inverse.py` & `Axelrod-4.9.1/axelrod/strategies/inverse.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/lookerup.py` & `Axelrod-4.9.1/axelrod/strategies/lookerup.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/mathematicalconstants.py` & `Axelrod-4.9.1/axelrod/strategies/mathematicalconstants.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/memoryone.py` & `Axelrod-4.9.1/axelrod/strategies/memoryone.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/memorytwo.py` & `Axelrod-4.9.1/axelrod/strategies/memorytwo.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/meta.py` & `Axelrod-4.9.1/axelrod/strategies/meta.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/mindcontrol.py` & `Axelrod-4.9.1/axelrod/strategies/mindcontrol.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/mindreader.py` & `Axelrod-4.9.1/axelrod/strategies/mindreader.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/mutual.py` & `Axelrod-4.9.1/axelrod/strategies/mutual.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/negation.py` & `Axelrod-4.9.1/axelrod/strategies/negation.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/oncebitten.py` & `Axelrod-4.9.1/axelrod/strategies/oncebitten.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/prober.py` & `Axelrod-4.9.1/axelrod/strategies/prober.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/punisher.py` & `Axelrod-4.9.1/axelrod/strategies/punisher.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/qlearner.py` & `Axelrod-4.9.1/axelrod/strategies/qlearner.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/rand.py` & `Axelrod-4.9.1/axelrod/strategies/rand.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/resurrection.py` & `Axelrod-4.9.1/axelrod/strategies/resurrection.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/retaliate.py` & `Axelrod-4.9.1/axelrod/strategies/retaliate.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/revised_downing.py` & `Axelrod-4.9.1/axelrod/strategies/revised_downing.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/selfsteem.py` & `Axelrod-4.9.1/axelrod/strategies/selfsteem.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/sequence_player.py` & `Axelrod-4.9.1/axelrod/strategies/sequence_player.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/shortmem.py` & `Axelrod-4.9.1/axelrod/strategies/shortmem.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/stalker.py` & `Axelrod-4.9.1/axelrod/strategies/stalker.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/titfortat.py` & `Axelrod-4.9.1/axelrod/strategies/titfortat.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/verybad.py` & `Axelrod-4.9.1/axelrod/strategies/verybad.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/worse_and_worse.py` & `Axelrod-4.9.1/axelrod/strategies/worse_and_worse.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategies/zero_determinant.py` & `Axelrod-4.9.1/axelrod/strategies/zero_determinant.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/strategy_transformers.py` & `Axelrod-4.9.1/axelrod/strategy_transformers.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/axelrod/tournament.py` & `Axelrod-4.9.1/axelrod/tournament.py`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/cache.txt` & `Axelrod-4.9.1/cache.txt`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/community/coc.rst` & `Axelrod-4.9.1/docs/community/coc.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/community/communication.rst` & `Axelrod-4.9.1/docs/community/communication.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/community/team.rst` & `Axelrod-4.9.1/docs/community/team.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/index.rst` & `Axelrod-4.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/all_strategies.rst` & `Axelrod-4.9.1/docs/reference/all_strategies.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/bibliography.rst` & `Axelrod-4.9.1/docs/reference/bibliography.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/description.rst` & `Axelrod-4.9.1/docs/reference/description.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/fortan_keys.rst` & `Axelrod-4.9.1/docs/reference/fortan_keys.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/glossary.rst` & `Axelrod-4.9.1/docs/reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/overview_of_strategies.rst` & `Axelrod-4.9.1/docs/reference/overview_of_strategies.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/reference/play_contexts.rst` & `Axelrod-4.9.1/docs/reference/play_contexts.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/classification_of_strategies.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/classification_of_strategies.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/games.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/games.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/player_equality.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/player_equality.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/player_information.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/player_information.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/reading_and_writing_interactions.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/reading_and_writing_interactions.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/setting_a_seed.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/setting_a_seed.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/strategies.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/strategies.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/strategy_transformers.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/strategy_transformers.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/tournament_results.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/tournament_results.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/advanced/using_the_cache.rst` & `Axelrod-4.9.1/docs/tutorials/advanced/using_the_cache.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/guidelines.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/guidelines.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/running_tests.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/running_tests.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/adding_the_new_strategy.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/adding_the_new_strategy.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/classifying_the_new_strategy.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/classifying_the_new_strategy.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/docstrings.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/docstrings.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/instructions.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/instructions.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/writing_test_for_the_new_strategy.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/writing_test_for_the_new_strategy.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/contributing/strategy/writing_the_new_strategy.rst` & `Axelrod-4.9.1/docs/tutorials/contributing/strategy/writing_the_new_strategy.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/approximate_moran_processes.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/approximate_moran_processes.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/ecological_variant.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/ecological_variant.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/evolvable_players.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/evolvable_players.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/fingerprinting.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/fingerprinting.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/meta_strategies.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/meta_strategies.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/morality_metrics.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/morality_metrics.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/moran_processes_on_graphs.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/moran_processes_on_graphs.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/noisy_tournaments.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/noisy_tournaments.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/probabilistict_end_tournaments.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/probabilistict_end_tournaments.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/further_topics/spatial_tournaments.rst` & `Axelrod-4.9.1/docs/tutorials/further_topics/spatial_tournaments.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/human_interaction.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/human_interaction.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/match.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/match.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/moran.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/moran.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/running_axelrods_first_tournament.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/running_axelrods_first_tournament.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/summarising_tournaments.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/summarising_tournaments.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/tournament.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/tournament.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/docs/tutorials/getting_started/visualising_results.rst` & `Axelrod-4.9.1/docs/tutorials/getting_started/visualising_results.rst`

 * *Files identical despite different names*

### Comparing `Axelrod-4.9.0/setup.py` & `Axelrod-4.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     packages=["axelrod", "axelrod.strategies", "axelrod.data"],
     url="http://axelrod.readthedocs.org/",
     license="The MIT License (MIT)",
     description="Reproduce the Axelrod iterated prisoners dilemma tournament",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     include_package_data=True,
-    package_data={"": ["axelrod/data/*.csv"]},
+    package_data={"": ["axelrod/data/*"]},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3 :: Only",
     ],
     python_requires=">=3.5",
 )
```

