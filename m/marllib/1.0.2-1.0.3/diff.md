# Comparing `tmp/marllib-1.0.2.tar.gz` & `tmp/marllib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marllib-1.0.2.tar", last modified: Tue Mar 21 10:22:53 2023, max compression
+gzip compressed data, was "dist/marllib-1.0.3.tar", last modified: Tue Apr 25 03:15:18 2023, max compression
```

## Comparing `marllib-1.0.2.tar` & `marllib-1.0.3.tar`

### file list

```diff
@@ -1,284 +1,289 @@
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.050332 marllib-1.0.2/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1072 2023-02-16 05:45:14.000000 marllib-1.0.2/LICENSE
--rw-rw-r--   0 hsy       (1000) hsy       (1000)       79 2023-02-18 05:47:38.000000 marllib-1.0.2/MANIFEST.in
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    20851 2023-03-21 10:22:53.050332 marllib-1.0.2/PKG-INFO
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    20318 2023-03-21 04:59:08.000000 marllib-1.0.2/README.md
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    15543 2023-03-06 04:21:33.000000 marllib-1.0.2/README.rst
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.026332 marllib-1.0.2/marllib/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/envs/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/envs/base_env/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2765 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/envs/base_env/config/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/config/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1465 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/football.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1341 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/hanabi.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1337 2023-03-17 01:55:36.000000 marllib-1.0.2/marllib/envs/base_env/config/lbf.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1304 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/magent.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1383 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/mamujoco.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1342 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/metadrive.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1302 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/mpe.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1640 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/pommerman.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1438 2023-03-16 23:20:12.000000 marllib-1.0.2/marllib/envs/base_env/config/rware.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1431 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/envs/base_env/config/smac.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4001 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/football.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3450 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/hanabi.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/envs/base_env/install/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/install/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3645 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/lbf.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5559 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/magent.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     6704 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/mamujoco.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     6412 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/metadrive.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5622 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/mpe.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    26674 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/pommerman.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4070 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/rware.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4393 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/base_env/smac.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/envs/global_reward_env/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2713 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1754 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/football_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1930 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/lbf_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2265 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/magent_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1188 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/mamujoco_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1951 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/mpe_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2999 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/pommerman_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1927 2023-03-16 22:19:26.000000 marllib-1.0.2/marllib/envs/global_reward_env/rware_fcoop.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1176 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/envs/global_reward_env/smac_fcoop.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/marl/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    13653 2023-03-14 06:02:38.000000 marllib-1.0.2/marllib/marl/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/marl/algos/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1189 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib/marl/algos/core/
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/core/CC/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/core/CC/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5602 2023-03-13 11:18:59.000000 marllib-1.0.2/marllib/marl/algos/core/CC/coma.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     8458 2023-03-13 11:18:58.000000 marllib-1.0.2/marllib/marl/algos/core/CC/happo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     8821 2023-03-13 11:18:59.000000 marllib-1.0.2/marllib/marl/algos/core/CC/hatrpo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3565 2023-03-13 11:18:58.000000 marllib-1.0.2/marllib/marl/algos/core/CC/maa2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    16505 2023-03-13 11:13:52.000000 marllib-1.0.2/marllib/marl/algos/core/CC/maddpg.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3784 2023-03-14 06:20:19.000000 marllib-1.0.2/marllib/marl/algos/core/CC/mappo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     7307 2023-03-14 06:20:19.000000 marllib-1.0.2/marllib/marl/algos/core/CC/matrpo.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/core/IL/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/core/IL/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1660 2023-03-13 23:45:13.000000 marllib-1.0.2/marllib/marl/algos/core/IL/a2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    24620 2023-03-13 23:45:13.000000 marllib-1.0.2/marllib/marl/algos/core/IL/ddpg.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1668 2023-03-13 23:45:14.000000 marllib-1.0.2/marllib/marl/algos/core/IL/ppo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     7062 2023-03-13 23:48:59.000000 marllib-1.0.2/marllib/marl/algos/core/IL/trpo.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/core/VD/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/core/VD/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    15917 2023-03-13 11:13:52.000000 marllib-1.0.2/marllib/marl/algos/core/VD/facmac.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    22246 2023-03-13 05:59:48.000000 marllib-1.0.2/marllib/marl/algos/core/VD/iql_vdn_qmix.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4643 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/core/VD/vda2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     6824 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/core/VD/vdppo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2144 2023-03-14 06:20:19.000000 marllib-1.0.2/marllib/marl/algos/core/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/hyperparams/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/hyperparams/common/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/coma.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1558 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/facmac.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1444 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/happo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/hatrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/ia2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1526 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/iddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1447 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/ippo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/iql.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1435 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/itrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/maa2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1528 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/maddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1450 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/mappo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/matrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/qmix.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/vda2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/vdn.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1478 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/common/vdppo.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.034332 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1559 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/facmac.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1445 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/happo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/hatrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/ia2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1525 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/iddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1448 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/ippo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1434 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/itrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/maa2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1529 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/maddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1451 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/mappo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/matrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/vda2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1479 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/vdppo.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.038332 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/coma.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1561 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/facmac.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1447 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/happo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/hatrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/ia2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1529 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/iddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1449 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/ippo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/iql.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1435 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/itrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1376 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/maa2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1534 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/maddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1452 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/mappo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/matrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1364 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/qmix.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1398 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vda2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vdn.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1480 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vdppo.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.038332 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/coma.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1431 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/happo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/hatrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/ia2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1448 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/ippo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/iql.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/itrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/maa2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1451 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/mappo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/matrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/qmix.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vda2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vdn.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1479 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vdppo.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/algos/hyperparams/test/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/coma.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1555 2023-03-14 02:44:54.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/facmac.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1443 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/happo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/hatrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1372 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/ia2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1523 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/iddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1446 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/ippo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1359 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/iql.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1434 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/itrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/maa2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1525 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/maddpg.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1449 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/mappo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/matrpo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1360 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/qmix.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1396 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/vda2c.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1359 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/vdn.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1477 2023-03-14 02:44:55.000000 marllib-1.0.2/marllib/marl/algos/hyperparams/test/vdppo.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     6327 2023-03-17 01:25:01.000000 marllib-1.0.2/marllib/marl/algos/run_cc.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5695 2023-03-14 01:06:37.000000 marllib-1.0.2/marllib/marl/algos/run_il.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     8199 2023-03-14 01:33:02.000000 marllib-1.0.2/marllib/marl/algos/run_vd.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/algos/scripts/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1992 2023-03-14 05:11:18.000000 marllib-1.0.2/marllib/marl/algos/scripts/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4587 2023-03-14 03:51:00.000000 marllib-1.0.2/marllib/marl/algos/scripts/coma.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5048 2023-03-14 02:32:33.000000 marllib-1.0.2/marllib/marl/algos/scripts/facmac.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5948 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/happo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5628 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/hatrpo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4572 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/ia2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5040 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/iddpg.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5178 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/ippo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5639 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/itrpo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4605 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/maa2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5045 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/maddpg.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5301 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/mappo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5559 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/matrpo.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4616 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/vda2c.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5493 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/vdn_qmix_iql.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5224 2023-03-14 02:44:30.000000 marllib-1.0.2/marllib/marl/algos/scripts/vdppo.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/algos/utils/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    11178 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/centralized_Q.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     8038 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/centralized_critic.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    15364 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/centralized_critic_hetero.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3930 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/episode_execution_plan.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3168 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/episode_replay_buffer.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     7165 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/heterogeneous_updateing.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1294 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/log_dir_util.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1889 2023-03-14 04:48:03.000000 marllib-1.0.2/marllib/marl/algos/utils/manipulate_tensor.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    12179 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/mixing_Q.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     6880 2023-03-14 04:46:08.000000 marllib-1.0.2/marllib/marl/algos/utils/mixing_critic.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4213 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/popart.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3668 2023-03-14 04:51:40.000000 marllib-1.0.2/marllib/marl/algos/utils/setup_utils.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     7837 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/algos/utils/trust_regions.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4397 2023-03-14 04:51:40.000000 marllib-1.0.2/marllib/marl/algos/utils/valuenorm.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3618 2023-03-14 05:14:34.000000 marllib-1.0.2/marllib/marl/common.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/models/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1127 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/models/configs/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/configs/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1550 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/models/configs/cnn_encoder.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1252 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/models/configs/fc_encoder.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1203 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/models/configs/mixer.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1188 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/models/configs/mlp.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1202 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/models/configs/rnn.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/models/zoo/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1167 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/zoo/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.042332 marllib-1.0.2/marllib/marl/models/zoo/encoder/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/zoo/encoder/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4954 2023-03-13 05:48:44.000000 marllib-1.0.2/marllib/marl/models/zoo/encoder/base_encoder.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5432 2023-03-13 05:49:12.000000 marllib-1.0.2/marllib/marl/models/zoo/encoder/cc_encoder.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/marl/models/zoo/mixer/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1176 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/zoo/mixer/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5638 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/zoo/mixer/monotonic_mixer.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1387 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/models/zoo/mixer/sum_mixer.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/marl/models/zoo/mlp/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1284 2023-03-13 06:03:44.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     4791 2023-03-13 05:49:33.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/base_mlp.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     9174 2023-03-14 04:41:07.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/cc_mlp.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    10418 2023-03-13 05:51:53.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/ddpg_mlp.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3921 2023-03-13 05:52:03.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/jointQ_mlp.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2529 2023-03-13 05:53:07.000000 marllib-1.0.2/marllib/marl/models/zoo/mlp/vd_mlp.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/marl/models/zoo/rnn/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1284 2023-03-13 06:04:45.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     8033 2023-03-13 05:53:27.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/base_rnn.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     9332 2023-03-14 04:41:07.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/cc_rnn.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    13169 2023-03-13 05:59:06.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/ddpg_rnn.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3865 2023-03-13 05:59:48.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/jointQ_rnn.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2528 2023-03-13 06:02:11.000000 marllib-1.0.2/marllib/marl/models/zoo/rnn/vd_rnn.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/marl/ray/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/marl/ray/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1959 2023-03-16 23:20:03.000000 marllib-1.0.2/marllib/marl/ray/ray.yaml
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1921 2023-03-12 07:29:37.000000 marllib-1.0.2/marllib/marl/ray/ray_beta.yaml
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/__init__.py
--rwxrwxr-x   0 hsy       (1000) hsy       (1000)     5038 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/add_patch.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/hanabi/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    38355 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/hanabi/Hanabi_Env.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1683 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/hanabi/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    33258 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/hanabi/pyhanabi.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/pommerman_patch/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     2529 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/pommerman_patch/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    31360 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/pommerman_patch/forward_model.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    18502 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/pommerman_patch/graphics.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    14809 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/pommerman_patch/v0.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/rllib/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/rllib/execution/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/execution/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    23953 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/execution/replay_buffer.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    17856 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/execution/train_ops.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    20069 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/execution/train_ops_new_sgd_batch.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/rllib/models/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/models/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    15153 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/models/preprocessors.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/marllib/patch/rllib/policy/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/policy/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    18728 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/policy/rnn_sequencing.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    49976 2023-03-12 07:29:54.000000 marllib-1.0.2/marllib/patch/rllib/policy/torch_policy.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.030332 marllib-1.0.2/marllib.egg-info/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    20851 2023-03-21 10:22:52.000000 marllib-1.0.2/marllib.egg-info/PKG-INFO
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    10339 2023-03-21 10:22:53.000000 marllib-1.0.2/marllib.egg-info/SOURCES.txt
--rw-rw-r--   0 hsy       (1000) hsy       (1000)        1 2023-03-21 10:22:52.000000 marllib-1.0.2/marllib.egg-info/dependency_links.txt
--rw-rw-r--   0 hsy       (1000) hsy       (1000)      188 2023-03-21 10:22:52.000000 marllib-1.0.2/marllib.egg-info/requires.txt
--rw-rw-r--   0 hsy       (1000) hsy       (1000)       26 2023-03-21 10:22:52.000000 marllib-1.0.2/marllib.egg-info/top_level.txt
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/multiagent_mujoco/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3511 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/__init__.py
-drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-03-21 10:22:53.046332 marllib-1.0.2/multiagent_mujoco/assets/
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     3326 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/assets/__init__.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     5160 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/coupled_half_cheetah.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     9117 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/manyagent_ant.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     7061 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/manyagent_swimmer.py
--rwxrwxr-x   0 hsy       (1000) hsy       (1000)    12044 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/mujoco_multi.py
--rwxrwxr-x   0 hsy       (1000) hsy       (1000)     5737 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/multiagentenv.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)    26220 2023-03-12 07:29:54.000000 marllib-1.0.2/multiagent_mujoco/obsk.py
--rw-rw-r--   0 hsy       (1000) hsy       (1000)      187 2023-02-18 05:47:38.000000 marllib-1.0.2/requirements.txt
--rw-rw-r--   0 hsy       (1000) hsy       (1000)       38 2023-03-21 10:22:53.050332 marllib-1.0.2/setup.cfg
--rw-rw-r--   0 hsy       (1000) hsy       (1000)     1288 2023-03-21 10:22:36.000000 marllib-1.0.2/setup.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)       38 2023-04-25 03:15:18.000000 marllib-1.0.3/setup.cfg
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/multiagent_mujoco/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3511 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/__init__.py
+-rwxrwxr-x   0 hsy       (1000) hsy       (1000)    12044 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/mujoco_multi.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/multiagent_mujoco/assets/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3326 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/assets/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5160 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/coupled_half_cheetah.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    26220 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/obsk.py
+-rwxrwxr-x   0 hsy       (1000) hsy       (1000)     5737 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/multiagentenv.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     9117 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/manyagent_ant.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7061 2023-03-12 07:29:54.000000 marllib-1.0.3/multiagent_mujoco/manyagent_swimmer.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/
+-rwxrwxr-x   0 hsy       (1000) hsy       (1000)     5038 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/add_patch.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/rllib/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/rllib/policy/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    49976 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/policy/torch_policy.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/policy/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    18728 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/policy/rnn_sequencing.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/rllib/execution/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/execution/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    23953 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/execution/replay_buffer.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    20069 2023-03-12 07:29:54.000000 marllib-1.0.3/marllib/patch/rllib/execution/train_ops_new_sgd_batch.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    17856 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/execution/train_ops.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/rllib/models/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    15153 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/models/preprocessors.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/rllib/models/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2173 2023-04-17 22:56:43.000000 marllib-1.0.3/marllib/patch/test.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/pommerman_patch/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2529 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/pommerman_patch/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    31360 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/pommerman_patch/forward_model.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    14809 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/pommerman_patch/v0.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    18502 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/pommerman_patch/graphics.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/patch/hanabi/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1683 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/hanabi/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    38355 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/hanabi/Hanabi_Env.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    33258 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/patch/hanabi/pyhanabi.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3618 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/common.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    13588 2023-04-17 06:26:10.000000 marllib-1.0.3/marllib/marl/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/matrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/maa2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1446 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/ippo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1359 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/iql.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/hatrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1372 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/ia2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1525 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/maddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1555 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/facmac.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1396 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/vda2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1434 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/itrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1359 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/vdn.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/coma.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1360 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/qmix.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1523 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/iddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1443 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/happo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1477 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/vdppo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1449 2023-04-25 01:32:32.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/test/mappo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-04-25 01:31:12.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/matrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-04-25 01:31:12.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/maa2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1447 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/ippo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/iql.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/hatrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/ia2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1528 2023-04-25 01:31:12.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/maddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1558 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/facmac.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/vda2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1435 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/itrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/vdn.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/coma.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/qmix.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1526 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/iddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1444 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/happo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1478 2023-04-25 01:52:27.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/vdppo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1450 2023-04-25 01:18:49.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/common/mappo.yaml
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1436 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/matrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/maa2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1448 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/ippo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/hatrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/ia2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1529 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/maddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1559 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/facmac.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/vda2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1434 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/itrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1525 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/iddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1445 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/happo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1479 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/vdppo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1451 2023-04-25 01:53:08.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/mappo.yaml
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/matrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1376 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/maa2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1449 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/ippo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/iql.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1437 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/hatrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/ia2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1534 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/maddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1561 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/facmac.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1398 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vda2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1435 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/itrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vdn.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/coma.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1364 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/qmix.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1529 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/iddpg.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1447 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/happo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1480 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vdppo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1452 2023-04-25 01:53:20.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/mappo.yaml
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/matrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1375 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/maa2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1448 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/ippo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/iql.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/hatrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1373 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/ia2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1397 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vda2c.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1413 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/itrpo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1362 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vdn.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1374 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/coma.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1363 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/qmix.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1431 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/happo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1479 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vdppo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1451 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/mappo.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1189 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     6327 2023-04-17 11:33:02.000000 marllib-1.0.3/marllib/marl/algos/run_cc.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7702 2023-04-17 23:13:38.000000 marllib-1.0.3/marllib/marl/algos/run_il.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4616 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/vda2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5559 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/matrpo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5045 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/maddpg.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1992 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5948 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/happo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5639 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/itrpo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4605 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/maa2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5178 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/ippo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5040 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/iddpg.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5224 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/vdppo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5628 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/hatrpo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5048 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/facmac.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4572 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/ia2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4587 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/coma.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5301 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/mappo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5493 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/scripts/vdn_qmix_iql.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/utils/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7165 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/heterogeneous_updateing.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1889 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/manipulate_tensor.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4397 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/valuenorm.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3930 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/episode_execution_plan.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1294 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/log_dir_util.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    12179 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/mixing_Q.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     6880 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/mixing_critic.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    11178 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/centralized_Q.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    15364 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/centralized_critic_hetero.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3668 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/setup_utils.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8038 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/centralized_critic.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4213 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/popart.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3168 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/episode_replay_buffer.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7837 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/algos/utils/trust_regions.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8221 2023-04-17 11:21:31.000000 marllib-1.0.3/marllib/marl/algos/run_vd.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/core/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2144 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/core/VD/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4643 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/VD/vda2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/VD/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     6824 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/VD/vdppo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    15917 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/VD/facmac.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    22246 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/VD/iql_vdn_qmix.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/core/IL/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/IL/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1660 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/IL/a2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    24620 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/IL/ddpg.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1668 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/IL/ppo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7062 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/marl/algos/core/IL/trpo.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/algos/core/CC/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7307 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/matrpo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    16505 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/maddpg.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8458 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/happo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3565 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/maa2c.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8821 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/marl/algos/core/CC/hatrpo.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5602 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/coma.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3784 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/marl/algos/core/CC/mappo.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/ray/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/ray/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1921 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/ray/ray_beta.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1957 2023-04-25 01:09:47.000000 marllib-1.0.3/marllib/marl/ray/ray.yaml
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1127 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/zoo/
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     9332 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/cc_rnn.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8033 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/base_rnn.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1284 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2528 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/vd_rnn.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3865 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/jointQ_rnn.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    10932 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/rnn/ddpg_rnn.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1167 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mixer/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1176 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mixer/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1387 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mixer/sum_mixer.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5638 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mixer/monotonic_mixer.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/zoo/encoder/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/encoder/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5432 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/encoder/cc_encoder.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4954 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/encoder/base_encoder.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1284 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     8233 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/ddpg_mlp.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3921 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/jointQ_mlp.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     9174 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/cc_mlp.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4791 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/base_mlp.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2529 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/zoo/mlp/vd_mlp.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/marl/models/configs/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1188 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/mlp.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1252 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/fc_encoder.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1202 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/rnn.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1550 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/cnn_encoder.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1203 2023-04-04 04:25:18.000000 marllib-1.0.3/marllib/marl/models/configs/mixer.yaml
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/envs/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/__init__.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/envs/base_env/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3450 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/hanabi.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5559 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/magent.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7291 2023-04-25 01:04:50.000000 marllib-1.0.3/marllib/envs/base_env/gobigger.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/envs/base_env/config/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1342 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/metadrive.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1341 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/hanabi.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1334 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/lbf.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1640 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/pommerman.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1465 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/football.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1383 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/mamujoco.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1302 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/mpe.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1304 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/magent.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1438 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/rware.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1431 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/config/smac.yaml
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3091 2023-04-24 04:12:32.000000 marllib-1.0.3/marllib/envs/base_env/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     6704 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/mamujoco.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4393 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/smac.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/envs/base_env/install/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1109 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/base_env/install/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4070 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/rware.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3645 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/lbf.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4964 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/mate.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    26674 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/pommerman.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     6412 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/metadrive.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     5622 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/mpe.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     4001 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/base_env/football.py
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib/envs/global_reward_env/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     7298 2023-04-25 01:04:50.000000 marllib-1.0.3/marllib/envs/global_reward_env/gobigger_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1930 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/lbf_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3134 2023-04-24 13:06:20.000000 marllib-1.0.3/marllib/envs/global_reward_env/__init__.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1858 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/rware_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1754 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/football_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1188 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/mamujoco_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2999 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/pommerman_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     2265 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/magent_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1951 2023-04-18 00:45:19.000000 marllib-1.0.3/marllib/envs/global_reward_env/mpe_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     3784 2023-04-18 00:47:58.000000 marllib-1.0.3/marllib/envs/global_reward_env/mate_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1176 2023-04-04 04:25:17.000000 marllib-1.0.3/marllib/envs/global_reward_env/smac_fcoop.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    25761 2023-04-25 03:15:18.000000 marllib-1.0.3/PKG-INFO
+drwxrwxr-x   0 hsy       (1000) hsy       (1000)        0 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)       26 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/top_level.txt
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    25761 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/PKG-INFO
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    10519 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/SOURCES.txt
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)      176 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/requires.txt
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)        1 2023-04-25 03:15:18.000000 marllib-1.0.3/marllib.egg-info/dependency_links.txt
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1288 2023-04-25 03:14:13.000000 marllib-1.0.3/setup.py
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    22303 2023-04-25 03:00:17.000000 marllib-1.0.3/README.md
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)     1072 2023-02-16 05:45:14.000000 marllib-1.0.3/LICENSE
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)      175 2023-04-18 01:56:17.000000 marllib-1.0.3/requirements.txt
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)       79 2023-04-04 04:25:17.000000 marllib-1.0.3/MANIFEST.in
+-rw-rw-r--   0 hsy       (1000) hsy       (1000)    15543 2023-04-18 00:45:19.000000 marllib-1.0.3/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `marllib-1.0.2/LICENSE` & `marllib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/PKG-INFO` & `marllib-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-Metadata-Version: 2.1
-Name: marllib
-Version: 1.0.2
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[comment]: <> (<div align="center">)
 
-<div align="center">
-<img src=docs/source/images/logo1.png width=65% />
-</div>
+[comment]: <> (<img src=docs/source/images/logo1.png width=65% />)
 
-<h1 align="center"> MARLlib: An Extensive Multi-agent Reinforcement Learning Library </h1>
+[comment]: <> (</div>)
 
+<h1 align="center"> MARLlib: A Scalable and Efficient Multi-agent Reinforcement Learning Library </h1>
 
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]()
 ![test](https://github.com/Replicable-MARL/MARLlib/workflows/test/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/)
 [![GitHub issues](https://img.shields.io/github/issues/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib/issues)
 [![PyPI version](https://badge.fury.io/py/marllib.svg)](https://badge.fury.io/py/marllib)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
+[![Organization](https://img.shields.io/badge/Organization-ReLER_RL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
+[![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
 [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
 
-**Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** based
-on [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It provides the MARL research community a unified
-platform for building, training, and evaluating MARL algorithms on almost all diverse tasks and environments.
+> __News__:
+> We are excited to announce that a major update has just been released. For detailed version information, please refer to the [version info](https://github.com/Replicable-MARL/MARLlib/releases/tag/1.0.2).
+
+
+**Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** that utilizes [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It offers a comprehensive platform for developing, training, and testing MARL algorithms across various tasks and environments. 
 
-A simple case of MARLlib usage:
+Here's an example of how MARLlib can be used:
 
 ```py
 from marllib import marl
 
 # prepare env
 env = marl.make_env(environment_name="mpe", map_name="simple_spread")
 
@@ -50,79 +39,81 @@
 # start training
 mappo.fit(env, model, stop={'timesteps_total': 1000000}, share_policy='group')
 
 # ready to control
 mappo.render(env, model, share_policy='group', restore_path='path_to_checkpoint')
 ```
 
+
+
 ## Why MARLlib?
 
 Here we provide a table for the comparison of MARLlib and existing work.
 
 |   Library   |  Supported Env | Algorithm | Parameter Sharing  | Model 
 |:-------------:|:-------------:|:-------------:|:--------------:|:----------------:|
 |     [PyMARL](https://github.com/oxwhirl/pymarl) |        1 cooperative       |       5       |         share        |      GRU           | :x:
 |   [PyMARL2](https://github.com/hijkzzz/pymarl2)|        2 cooperative       |     11   |         share        |  MLP + GRU  | :x:
 | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy) |       4 cooperative       |      1     |          share + separate        |          MLP + GRU        |         :x:              |
 | [MAlib](https://github.com/sjtu-marl/malib) |  4 self-play  | 10 | share + group + separate | MLP + LSTM | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest)
 |    [EPyMARL](https://github.com/uoe-agents/epymarl)|        4 cooperative      |    9    |        share + separate       |      GRU             |           :x:            |
-|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       10 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
+|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       12 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
 
 |   Library   | Github Stars  | Documentation | Issues Open | Activity | Last Update
 |:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
 |     [PyMARL](https://github.com/oxwhirl/pymarl) | [![GitHub stars](https://img.shields.io/github/stars/oxwhirl/pymarl)](https://github.com/oxwhirl/pymarl)    |       :x: | ![GitHub opened issue](https://img.shields.io/github/issues/oxwhirl/pymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/oxwhirl/pymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/oxwhirl/pymarl?label=last%20update)  
 |   [PyMARL2](https://github.com/hijkzzz/pymarl2)| [![GitHub stars](https://img.shields.io/github/stars/hijkzzz/pymarl2)](https://github.com/hijkzzz/pymarl2)       |       :x:  | ![GitHub opened issue](https://img.shields.io/github/issues/hijkzzz/pymarl2.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/hijkzzz/pymarl2?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/hijkzzz/pymarl2?label=last%20update)  
 | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy)| [![GitHub stars](https://img.shields.io/github/stars/marlbenchmark/on-policy)](https://github.com/marlbenchmark/on-policy)   |        :x:              | ![GitHub opened issue](https://img.shields.io/github/issues/marlbenchmark/on-policy.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/marlbenchmark/on-policy?label=commit)| ![GitHub last commit](https://img.shields.io/github/last-commit/marlbenchmark/on-policy?label=last%20update)  
-| [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/hijkzzz/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
+| [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
 |    [EPyMARL](https://github.com/uoe-agents/epymarl)| [![GitHub stars](https://img.shields.io/github/stars/uoe-agents/epymarl)](https://github.com/uoe-agents/epymarl)        |           :x:            | ![GitHub opened issue](https://img.shields.io/github/issues/uoe-agents/epymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/uoe-agents/epymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/uoe-agents/epymarl?label=last%20update)  
 |    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |  [![GitHub stars](https://img.shields.io/github/stars/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib)  |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) | ![GitHub opened issue](https://img.shields.io/github/issues/Replicable-MARL/MARLlib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/m/Replicable-MARL/MARLlib/sy_dev?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/Replicable-MARL/MARLlib/sy_dev?label=last%20update)  
 
 
 
 [comment]: <> (<div align="center">)
 
 [comment]: <> (<img src=docs/source/images/overview.png width=100% />)
 
 [comment]: <> (</div>)
 
 ## key features
 
-:beginner: What **MARLlib** brings to MARL community:
+:beginner: MARLlib offers several key features that make it stand out:
 
-- it unifies diverse algorithm pipelines with agent-level distributed dataflow.
-- it supports all task modes: cooperative, collaborative, competitive, and mixed.
-- it unifies multi-agent environment interfaces with a new interface following Gym.
-- it provides flexible and customizable parameter-sharing strategies.
-
-:rocket: With MARLlib, you can exploit the advantages not limited to:
-
-- **zero knowledge of MARL**: out of the box 18 algorithms with intuitive API!
-- **all task modes available**: support almost all multi-agent environment!
-- **customizable model arch**: pick your favorite one from the model zoo!
-- **customizable policy sharing**: grouped by MARLlib or build your own!
-- more than a thousand experiments are conducted and released!
+- MARLlib unifies diverse algorithm pipelines with agent-level distributed dataflow, allowing researchers to develop, test, and evaluate MARL algorithms across different tasks and environments.
+- MARLlib supports all task modes, including cooperative, collaborative, competitive, and mixed. This makes it easier for researchers to train and evaluate MARL algorithms across a wide range of tasks.
+- MARLlib provides a new interface that follows the structure of Gym, making it easier for researchers to work with multi-agent environments.
+- MARLlib provides flexible and customizable parameter-sharing strategies, allowing researchers to optimize their algorithms for different tasks and environments.
+
+:rocket: Using MARLlib, you can take advantage of various benefits, such as:
+
+- **Zero knowledge of MARL**: MARLlib provides 18 pre-built algorithms with an intuitive API, allowing researchers to start experimenting with MARL without prior knowledge of the field.
+- **Support for all task modes**: MARLlib supports almost all multi-agent environments, making it easier for researchers to experiment with different task modes.
+- **Customizable model architecture**: Researchers can choose their preferred model architecture from the model zoo, or build their own.
+- **Customizable policy sharing**: MARLlib provides grouping options for policy sharing, or researchers can create their own.
+- **Access to over a thousand released experiments**: Researchers can access over a thousand released experiments to see how other researchers have used MARLlib.
 
 ## Installation
 
 > __Note__:
-> MARLlib supports Linux only.
+> Currently MARLlib supports Linux only.
 
 ### Step-by-step  (recommended)
 
 - install dependencies
 - install environments
 - install patches
 
 #### 1. install dependencies (basic)
 
 First, install MARLlib dependencies to guarantee basic usage.
 following [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html), finally install patches for RLlib.
 
 ```bash
-$ conda create -n marllib python=3.8
+$ conda create -n marllib python=3.8 # or 3.9
 $ conda activate marllib
 $ git clone https://github.com/Replicable-MARL/MARLlib.git && cd MARLlib
 $ pip install -r requirements.txt
 ```
 
 #### 2. install environments (optional)
 
@@ -187,17 +178,19 @@
 | **[LBF](https://github.com/semitable/lb-foraging)**  | cooperative + collaborative | Both | Discrete | 1D  |
 | **[RWARE](https://github.com/semitable/robotic-warehouse)**  | cooperative | Partial | Discrete | 1D  |
 | **[MPE](https://github.com/openai/multiagent-particle-envs)**  | cooperative + collaborative + mixed | Both | Both | 1D  |
 | **[SMAC](https://github.com/oxwhirl/smac)**  | cooperative | Partial | Discrete | 1D |
 | **[MetaDrive](https://github.com/decisionforce/metadrive)**  | collaborative | Partial | Continuous | 1D |
 | **[MAgent](https://www.pettingzoo.ml/magent)** | collaborative + mixed | Partial | Discrete | 2D |
 | **[Pommerman](https://github.com/MultiAgentLearning/playground)**  | collaborative + competitive + mixed | Both | Discrete | 2D |
-| **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Partial | Continuous | 1D |
+| **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Full | Continuous | 1D |
 | **[GRF](https://github.com/google-research/football)**  | collaborative + mixed | Full | Discrete | 2D |
 | **[Hanabi](https://github.com/deepmind/hanabi-learning-environment)** | cooperative | Partial | Discrete | 1D |
+| **[MATE](https://github.com/XuehaiPan/mate)** | cooperative + mixed | Partial | Both | 1D |
+| **[GoBigger](https://github.com/opendilab/GoBigger)** | cooperative + mixed | Both | Continuous | 1D |
 
 Each environment has a readme file, standing as the instruction for this task, including env settings, installation, and
 important notes.
 </details>
 
 <details>
 <summary><b><big>Initialize the algorithm</big></b></summary>
@@ -323,41 +316,45 @@
 ## Tutorials
 
 Try MPE + MAPPO examples on Google Colaboratory!
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
 
 More tutorial documentations are available [here](https://marllib.readthedocs.io/).
 
+## Awesome List
+
+A collection of research and review papers of multi-agent reinforcement learning (MARL) is available. The papers have been organized based on their publication date and their evaluation of the corresponding environments.
+
+Algorithms: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
+Environments: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/handbook/env.html)
+
+
 ## Community
 
 |  Channel   | Link |
 | :----------- | :----------- |
 | Issues | [GitHub Issues](https://github.com/Replicable-MARL/MARLlib/issues) |
 
+## Roadmap
+
+The roadmap to the future release is available in [ROADMAP.md](https://github.com/Replicable-MARL/MARLlib/blob/main/ROADMAP.md).
 
 ## Contributing
 
 We are a small team on multi-agent reinforcement learning, and we will take all the help we can get! 
 If you would like to get involved, here is information on [contribution guidelines and how to test the code locally](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/CONTRIBUTING.md).
 
 You can contribute in multiple ways, e.g., reporting bugs, writing or translating documentation, reviewing or refactoring code, requesting or implementing new features, etc.
 
-[comment]: <> (## Paper)
-
-[comment]: <> (If you use MARLlib in your research, please cite the [MARLlib paper]&#40;https://arxiv.org/abs/2210.13708&#41;.)
-
-[comment]: <> (```tex)
-
-[comment]: <> (@article{hu2022marllib,)
+## Paper
 
-[comment]: <> (  title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},)
+If you use MARLlib in your research, please cite the [MARLlib paper](https://arxiv.org/abs/2210.13708).
 
-[comment]: <> (  author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},)
-
-[comment]: <> (  journal={arXiv preprint arXiv:2210.13708},)
-
-[comment]: <> (  year={2022})
-
-[comment]: <> (})
-
-[comment]: <> (```)
+```tex
+@article{hu2022marllib,
+  title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},
+  author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},
+  journal={arXiv preprint arXiv:2210.13708},
+  year={2022}
+}
+```
```

### Comparing `marllib-1.0.2/README.md` & `marllib-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,347 +1,378 @@
-<div align="center">
-<img src=docs/source/images/logo1.png width=65% />
-</div>
-
-<h1 align="center"> MARLlib: An Extensive Multi-agent Reinforcement Learning Library </h1>
-
-
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]()
-![test](https://github.com/Replicable-MARL/MARLlib/workflows/test/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/)
-[![GitHub issues](https://img.shields.io/github/issues/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib/issues)
-[![PyPI version](https://badge.fury.io/py/marllib.svg)](https://badge.fury.io/py/marllib)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
-[![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
-
-**Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** based
-on [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It provides the MARL research community a unified
-platform for building, training, and evaluating MARL algorithms on almost all diverse tasks and environments.
-
-A simple case of MARLlib usage:
-
-```py
-from marllib import marl
-
-# prepare env
-env = marl.make_env(environment_name="mpe", map_name="simple_spread")
-
-# initialize algorithm with appointed hyper-parameters
-mappo = marl.algos.mappo(hyperparam_source='mpe')
-
-# build agent model based on env + algorithms + user preference
-model = marl.build_model(env, mappo, {"core_arch": "gru", "encode_layer": "128-256"})
-
-# start training
-mappo.fit(env, model, stop={'timesteps_total': 1000000}, share_policy='group')
-
-# ready to control
-mappo.render(env, model, share_policy='group', restore_path='path_to_checkpoint')
-```
-
-## Why MARLlib?
-
-Here we provide a table for the comparison of MARLlib and existing work.
-
-|   Library   |  Supported Env | Algorithm | Parameter Sharing  | Model 
-|:-------------:|:-------------:|:-------------:|:--------------:|:----------------:|
-|     [PyMARL](https://github.com/oxwhirl/pymarl) |        1 cooperative       |       5       |         share        |      GRU           | :x:
-|   [PyMARL2](https://github.com/hijkzzz/pymarl2)|        2 cooperative       |     11   |         share        |  MLP + GRU  | :x:
-| [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy) |       4 cooperative       |      1     |          share + separate        |          MLP + GRU        |         :x:              |
-| [MAlib](https://github.com/sjtu-marl/malib) |  4 self-play  | 10 | share + group + separate | MLP + LSTM | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest)
-|    [EPyMARL](https://github.com/uoe-agents/epymarl)|        4 cooperative      |    9    |        share + separate       |      GRU             |           :x:            |
-|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       10 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
-
-|   Library   | Github Stars  | Documentation | Issues Open | Activity | Last Update
-|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
-|     [PyMARL](https://github.com/oxwhirl/pymarl) | [![GitHub stars](https://img.shields.io/github/stars/oxwhirl/pymarl)](https://github.com/oxwhirl/pymarl)    |       :x: | ![GitHub opened issue](https://img.shields.io/github/issues/oxwhirl/pymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/oxwhirl/pymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/oxwhirl/pymarl?label=last%20update)  
-|   [PyMARL2](https://github.com/hijkzzz/pymarl2)| [![GitHub stars](https://img.shields.io/github/stars/hijkzzz/pymarl2)](https://github.com/hijkzzz/pymarl2)       |       :x:  | ![GitHub opened issue](https://img.shields.io/github/issues/hijkzzz/pymarl2.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/hijkzzz/pymarl2?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/hijkzzz/pymarl2?label=last%20update)  
-| [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy)| [![GitHub stars](https://img.shields.io/github/stars/marlbenchmark/on-policy)](https://github.com/marlbenchmark/on-policy)   |        :x:              | ![GitHub opened issue](https://img.shields.io/github/issues/marlbenchmark/on-policy.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/marlbenchmark/on-policy?label=commit)| ![GitHub last commit](https://img.shields.io/github/last-commit/marlbenchmark/on-policy?label=last%20update)  
-| [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/hijkzzz/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
-|    [EPyMARL](https://github.com/uoe-agents/epymarl)| [![GitHub stars](https://img.shields.io/github/stars/uoe-agents/epymarl)](https://github.com/uoe-agents/epymarl)        |           :x:            | ![GitHub opened issue](https://img.shields.io/github/issues/uoe-agents/epymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/uoe-agents/epymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/uoe-agents/epymarl?label=last%20update)  
-|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |  [![GitHub stars](https://img.shields.io/github/stars/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib)  |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) | ![GitHub opened issue](https://img.shields.io/github/issues/Replicable-MARL/MARLlib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/m/Replicable-MARL/MARLlib/sy_dev?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/Replicable-MARL/MARLlib/sy_dev?label=last%20update)  
-
-
-
-[comment]: <> (<div align="center">)
-
-[comment]: <> (<img src=docs/source/images/overview.png width=100% />)
-
-[comment]: <> (</div>)
-
-## key features
-
-:beginner: What **MARLlib** brings to MARL community:
-
-- it unifies diverse algorithm pipelines with agent-level distributed dataflow.
-- it supports all task modes: cooperative, collaborative, competitive, and mixed.
-- it unifies multi-agent environment interfaces with a new interface following Gym.
-- it provides flexible and customizable parameter-sharing strategies.
-
-:rocket: With MARLlib, you can exploit the advantages not limited to:
-
-- **zero knowledge of MARL**: out of the box 18 algorithms with intuitive API!
-- **all task modes available**: support almost all multi-agent environment!
-- **customizable model arch**: pick your favorite one from the model zoo!
-- **customizable policy sharing**: grouped by MARLlib or build your own!
-- more than a thousand experiments are conducted and released!
-
-## Installation
-
-> __Note__:
-> MARLlib supports Linux only.
-
-### Step-by-step  (recommended)
-
-- install dependencies
-- install environments
-- install patches
-
-#### 1. install dependencies (basic)
-
-First, install MARLlib dependencies to guarantee basic usage.
-following [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html), finally install patches for RLlib.
-
-```bash
-$ conda create -n marllib python=3.8
-$ conda activate marllib
-$ git clone https://github.com/Replicable-MARL/MARLlib.git && cd MARLlib
-$ pip install -r requirements.txt
-```
-
-#### 2. install environments (optional)
-
-Please follow [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html).
-
-#### 3. install patches (basic)
-
-Fix bugs of RLlib using patches by running the following command:
-
-```bash
-$ cd /Path/To/MARLlib/marl/patch
-$ python add_patch.py -y
-```
-
-### PyPI
-
-```bash
-$ pip install --upgrade pip
-$ pip install marllib
-```
-
-## Getting started
-
-<details>
-<summary><b><big>Prepare the configuration</big></b></summary>
-
-There are four parts of configurations that take charge of the whole training process.
-
-- scenario: specify the environment/task settings
-- algorithm: choose the hyperparameters of the algorithm
-- model: customize the model architecture
-- ray/rllib: change the basic training settings
-
-<div align="center">
-<img src=docs/source/images/configurations.png width=100% />
-</div>
-
-Before training, ensure all the parameters are set correctly, especially those you don't want to change.
-> __Note__:
-> You can also modify all the pre-set parameters via MARLLib API.*
-
-</details>
-
-<details>
-<summary><b><big>Register the environment</big></b></summary>
-
-Ensure all the dependencies are installed for the environment you are running with. Otherwise, please refer to
-[MARLlib documentation](https://marllib.readthedocs.io/en/latest/handbook/env.html).
-
-
-|   task mode   | api example |
-| :-----------: | ----------- |
-| cooperative | ```marl.make_env(environment_name="mpe", map_name="simple_spread", force_coop=True)``` |
-| collaborative | ```marl.make_env(environment_name="mpe", map_name="simple_spread")``` |
-| competitive | ```marl.make_env(environment_name="mpe", map_name="simple_adversary")``` |
-| mixed | ```marl.make_env(environment_name="mpe", map_name="simple_crypto")``` |
-
-Most of the popular environments in MARL research are supported by MARLlib:
-
-| Env Name | Learning Mode | Observability | Action Space | Observations |
-| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
-| **[LBF](https://github.com/semitable/lb-foraging)**  | cooperative + collaborative | Both | Discrete | 1D  |
-| **[RWARE](https://github.com/semitable/robotic-warehouse)**  | cooperative | Partial | Discrete | 1D  |
-| **[MPE](https://github.com/openai/multiagent-particle-envs)**  | cooperative + collaborative + mixed | Both | Both | 1D  |
-| **[SMAC](https://github.com/oxwhirl/smac)**  | cooperative | Partial | Discrete | 1D |
-| **[MetaDrive](https://github.com/decisionforce/metadrive)**  | collaborative | Partial | Continuous | 1D |
-| **[MAgent](https://www.pettingzoo.ml/magent)** | collaborative + mixed | Partial | Discrete | 2D |
-| **[Pommerman](https://github.com/MultiAgentLearning/playground)**  | collaborative + competitive + mixed | Both | Discrete | 2D |
-| **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Partial | Continuous | 1D |
-| **[GRF](https://github.com/google-research/football)**  | collaborative + mixed | Full | Discrete | 2D |
-| **[Hanabi](https://github.com/deepmind/hanabi-learning-environment)** | cooperative | Partial | Discrete | 1D |
-
-Each environment has a readme file, standing as the instruction for this task, including env settings, installation, and
-important notes.
-</details>
-
-<details>
-<summary><b><big>Initialize the algorithm</big></b></summary>
-
-
-|  running target   | api example |
-| :-----------: | ----------- |
-| train & finetune  | ```marl.algos.mappo(hyperparam_source=$ENV)``` |
-| develop & debug | ```marl.algos.mappo(hyperparam_source="test")``` |
-| 3rd party env | ```marl.algos.mappo(hyperparam_source="common")``` |
-
-Here is a chart describing the characteristics of each algorithm:
-
-| algorithm                                                    | support task mode | discrete action   | continuous action |  policy type        |
-| :------------------------------------------------------------: | :-----------------: | :----------: | :--------------------: | :----------: | 
-| *IQL**                                                         | all four               | :heavy_check_mark:   |    |  off-policy |
-| *[PG](https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf)* | all four                  | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[A2C](https://arxiv.org/abs/1602.01783)*                      | all four              | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[DDPG](https://arxiv.org/abs/1509.02971)*                     | all four             |  | :heavy_check_mark:   |  off-policy |
-| *[TRPO](http://proceedings.mlr.press/v37/schulman15.pdf)*      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[PPO](https://arxiv.org/abs/1707.06347)*                      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[COMA](https://ojs.aaai.org/index.php/AAAI/article/download/11794/11653)* | all four                           | :heavy_check_mark:       |   |  on-policy  |
-| *[MADDPG](https://arxiv.org/abs/1706.02275)*                   | all four                     |  | :heavy_check_mark:   |  off-policy |
-| *MAA2C**                                                       | all four                        | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *MATRPO**                                                      | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[MAPPO](https://arxiv.org/abs/2103.01955)*                    | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[HATRPO](https://arxiv.org/abs/2109.11251)*                   | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[HAPPO](https://arxiv.org/abs/2109.11251)*                    | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[VDN](https://arxiv.org/abs/1706.05296)*                      | cooperative         | :heavy_check_mark:   |    |  off-policy |
-| *[QMIX](https://arxiv.org/abs/1803.11485)*                     | cooperative                    | :heavy_check_mark:   |   |  off-policy |
-| *[FACMAC](https://arxiv.org/abs/2003.06709)*                   | cooperative                    |  | :heavy_check_mark:   |  off-policy |
-| *[VDAC](https://arxiv.org/abs/2007.12306)*                    | cooperative                    | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *VDPPO**                                                      | cooperative                | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-
-***all four**: cooperative collaborative competitive mixed
-
-*IQL* is the multi-agent version of Q learning.
-*MAA2C* and *MATRPO* are the centralized version of A2C and TRPO.
-*VDPPO* is the value decomposition version of PPO.
-
-</details>
-
-<details>
-<summary><b><big>Build the agent model</big></b></summary>
-
-An agent model consists of two parts, `encoder` and `core arch`. 
-`encoder` will be constructed by MARLlib according to the observation space.
-Choose `mlp`, `gru`, or `lstm` as you like to build the complete model.
-
-|  model arch   | api example |
-| :-----------: | ----------- |
-| MLP  | ```marl.build_model(env, algo, {"core_arch": "mlp")``` |
-| GRU | ```marl.build_model(env, algo, {"core_arch": "gru"})```  |
-| LSTM | ```marl.build_model(env, algo, {"core_arch": "lstm"})```  |
-| Encoder Arch | ```marl.build_model(env, algo, {"core_arch": "gru", "encode_layer": "128-256"})```  |
-
-
-</details>
-
-<details>
-<summary><b><big>Kick off the training</big></b></summary>
-
-|  setting   | api example |
-| :-----------: | ----------- |
-| train  | ```algo.fit(env, model)``` |
-| debug  | ```algo.fit(env, model, local_mode=True)``` |
-| stop condition | ```algo.fit(env, model, stop={'episode_reward_mean': 2000, 'timesteps_total': 10000000})```  |
-| policy sharing | ```algo.fit(env, model, share_policy='all') # or 'group' / 'individual'```  |
-| save model | ```algo.fit(env, model, checkpoint_freq=100, checkpoint_end=True)```  |
-| GPU accelerate  | ```algo.fit(env, model, local_mode=False, num_gpus=1)``` |
-| CPU accelerate | ```algo.fit(env, model, local_mode=False, num_workers=5)```  |
-
-</details>
-
-<details>
-<summary><b><big>Training & rendering API</big></b></summary>
-
-```py
-from marllib import marl
-
-# prepare env
-env = marl.make_env(environment_name="mpe", map_name="simple_spread")
-# initialize algorithm with appointed hyper-parameters
-mappo = marl.algos.mappo(hyperparam_source="mpe")
-# build agent model based on env + algorithms + user preference
-model = marl.build_model(env, mappo, {"core_arch": "mlp", "encode_layer": "128-256"})
-# start training
-mappo.fit(
-  env, model, 
-  stop={"timesteps_total": 1000000}, 
-  checkpoint_freq=100, 
-  share_policy="group"
-)
-# rendering
-mappo.render(
-  env, model, 
-  local_mode=True, 
-  restore_path={'params_path': "checkpoint_000010/params.json",
-                'model_path': "checkpoint_000010/checkpoint-10"}
-)
-```
-</details>
-
-## Benchmark results
-
-All results are listed [here](https://github.com/Replicable-MARL/MARLlib/tree/main/results).
-
-## Quick examples
-
-MARLlib provides some practical examples for you to refer to.
-
-- [Detailed API usage](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/api_basic_usage.py): show how to use MARLlib api in
-  detail, e.g. cmd + api combined running.
-- [Policy sharing cutomization](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/customize_policy_sharing.py):
-  define your group policy-sharing strategy as you like based on current tasks.
-- [Loading model and rendering](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/load_and_render_model.py):
-  render the environment based on the pre-trained model.
-- [Incorporating new environment](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_env.py):
-  add your new environment following MARLlib's env-agent interaction interface.
-- [Incorporating new algorithm](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_algorithm.py):
-  add your new algorithm following MARLlib learning pipeline.
-
-## Tutorials
-
-Try MPE + MAPPO examples on Google Colaboratory!
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
-
-More tutorial documentations are available [here](https://marllib.readthedocs.io/).
-
-## Community
-
-|  Channel   | Link |
-| :----------- | :----------- |
-| Issues | [GitHub Issues](https://github.com/Replicable-MARL/MARLlib/issues) |
-
-
-## Contributing
-
-We are a small team on multi-agent reinforcement learning, and we will take all the help we can get! 
-If you would like to get involved, here is information on [contribution guidelines and how to test the code locally](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/CONTRIBUTING.md).
-
-You can contribute in multiple ways, e.g., reporting bugs, writing or translating documentation, reviewing or refactoring code, requesting or implementing new features, etc.
-
-[comment]: <> (## Paper)
-
-[comment]: <> (If you use MARLlib in your research, please cite the [MARLlib paper]&#40;https://arxiv.org/abs/2210.13708&#41;.)
-
-[comment]: <> (```tex)
-
-[comment]: <> (@article{hu2022marllib,)
-
-[comment]: <> (  title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},)
-
-[comment]: <> (  author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},)
-
-[comment]: <> (  journal={arXiv preprint arXiv:2210.13708},)
-
-[comment]: <> (  year={2022})
-
-[comment]: <> (})
-
-[comment]: <> (```)
-
+Metadata-Version: 2.1
+Name: marllib
+Version: 1.0.3
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: MIT
+Description: [comment]: <> (<div align="center">)
+        
+        [comment]: <> (<img src=docs/source/images/logo1.png width=65% />)
+        
+        [comment]: <> (</div>)
+        
+        <h1 align="center"> MARLlib: A Scalable and Efficient Multi-agent Reinforcement Learning Library </h1>
+        
+        [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]()
+        ![test](https://github.com/Replicable-MARL/MARLlib/workflows/test/badge.svg)
+        [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/)
+        [![GitHub issues](https://img.shields.io/github/issues/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib/issues)
+        [![PyPI version](https://badge.fury.io/py/marllib.svg)](https://badge.fury.io/py/marllib)
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
+        [![Organization](https://img.shields.io/badge/Organization-ReLER_RL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
+        [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
+        [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
+        
+        > __News__:
+        > We are excited to announce that a major update has just been released. For detailed version information, please refer to the [version info](https://github.com/Replicable-MARL/MARLlib/releases/tag/1.0.2).
+        
+        
+        **Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** that utilizes [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It offers a comprehensive platform for developing, training, and testing MARL algorithms across various tasks and environments. 
+        
+        Here's an example of how MARLlib can be used:
+        
+        ```py
+        from marllib import marl
+        
+        # prepare env
+        env = marl.make_env(environment_name="mpe", map_name="simple_spread")
+        
+        # initialize algorithm with appointed hyper-parameters
+        mappo = marl.algos.mappo(hyperparam_source='mpe')
+        
+        # build agent model based on env + algorithms + user preference
+        model = marl.build_model(env, mappo, {"core_arch": "gru", "encode_layer": "128-256"})
+        
+        # start training
+        mappo.fit(env, model, stop={'timesteps_total': 1000000}, share_policy='group')
+        
+        # ready to control
+        mappo.render(env, model, share_policy='group', restore_path='path_to_checkpoint')
+        ```
+        
+        
+        
+        ## Why MARLlib?
+        
+        Here we provide a table for the comparison of MARLlib and existing work.
+        
+        |   Library   |  Supported Env | Algorithm | Parameter Sharing  | Model 
+        |:-------------:|:-------------:|:-------------:|:--------------:|:----------------:|
+        |     [PyMARL](https://github.com/oxwhirl/pymarl) |        1 cooperative       |       5       |         share        |      GRU           | :x:
+        |   [PyMARL2](https://github.com/hijkzzz/pymarl2)|        2 cooperative       |     11   |         share        |  MLP + GRU  | :x:
+        | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy) |       4 cooperative       |      1     |          share + separate        |          MLP + GRU        |         :x:              |
+        | [MAlib](https://github.com/sjtu-marl/malib) |  4 self-play  | 10 | share + group + separate | MLP + LSTM | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest)
+        |    [EPyMARL](https://github.com/uoe-agents/epymarl)|        4 cooperative      |    9    |        share + separate       |      GRU             |           :x:            |
+        |    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       12 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
+        
+        |   Library   | Github Stars  | Documentation | Issues Open | Activity | Last Update
+        |:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
+        |     [PyMARL](https://github.com/oxwhirl/pymarl) | [![GitHub stars](https://img.shields.io/github/stars/oxwhirl/pymarl)](https://github.com/oxwhirl/pymarl)    |       :x: | ![GitHub opened issue](https://img.shields.io/github/issues/oxwhirl/pymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/oxwhirl/pymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/oxwhirl/pymarl?label=last%20update)  
+        |   [PyMARL2](https://github.com/hijkzzz/pymarl2)| [![GitHub stars](https://img.shields.io/github/stars/hijkzzz/pymarl2)](https://github.com/hijkzzz/pymarl2)       |       :x:  | ![GitHub opened issue](https://img.shields.io/github/issues/hijkzzz/pymarl2.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/hijkzzz/pymarl2?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/hijkzzz/pymarl2?label=last%20update)  
+        | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy)| [![GitHub stars](https://img.shields.io/github/stars/marlbenchmark/on-policy)](https://github.com/marlbenchmark/on-policy)   |        :x:              | ![GitHub opened issue](https://img.shields.io/github/issues/marlbenchmark/on-policy.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/marlbenchmark/on-policy?label=commit)| ![GitHub last commit](https://img.shields.io/github/last-commit/marlbenchmark/on-policy?label=last%20update)  
+        | [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
+        |    [EPyMARL](https://github.com/uoe-agents/epymarl)| [![GitHub stars](https://img.shields.io/github/stars/uoe-agents/epymarl)](https://github.com/uoe-agents/epymarl)        |           :x:            | ![GitHub opened issue](https://img.shields.io/github/issues/uoe-agents/epymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/uoe-agents/epymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/uoe-agents/epymarl?label=last%20update)  
+        |    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |  [![GitHub stars](https://img.shields.io/github/stars/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib)  |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) | ![GitHub opened issue](https://img.shields.io/github/issues/Replicable-MARL/MARLlib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/m/Replicable-MARL/MARLlib/sy_dev?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/Replicable-MARL/MARLlib/sy_dev?label=last%20update)  
+        
+        
+        
+        [comment]: <> (<div align="center">)
+        
+        [comment]: <> (<img src=docs/source/images/overview.png width=100% />)
+        
+        [comment]: <> (</div>)
+        
+        ## key features
+        
+        :beginner: MARLlib offers several key features that make it stand out:
+        
+        - MARLlib unifies diverse algorithm pipelines with agent-level distributed dataflow, allowing researchers to develop, test, and evaluate MARL algorithms across different tasks and environments.
+        - MARLlib supports all task modes, including cooperative, collaborative, competitive, and mixed. This makes it easier for researchers to train and evaluate MARL algorithms across a wide range of tasks.
+        - MARLlib provides a new interface that follows the structure of Gym, making it easier for researchers to work with multi-agent environments.
+        - MARLlib provides flexible and customizable parameter-sharing strategies, allowing researchers to optimize their algorithms for different tasks and environments.
+        
+        :rocket: Using MARLlib, you can take advantage of various benefits, such as:
+        
+        - **Zero knowledge of MARL**: MARLlib provides 18 pre-built algorithms with an intuitive API, allowing researchers to start experimenting with MARL without prior knowledge of the field.
+        - **Support for all task modes**: MARLlib supports almost all multi-agent environments, making it easier for researchers to experiment with different task modes.
+        - **Customizable model architecture**: Researchers can choose their preferred model architecture from the model zoo, or build their own.
+        - **Customizable policy sharing**: MARLlib provides grouping options for policy sharing, or researchers can create their own.
+        - **Access to over a thousand released experiments**: Researchers can access over a thousand released experiments to see how other researchers have used MARLlib.
+        
+        ## Installation
+        
+        > __Note__:
+        > Currently MARLlib supports Linux only.
+        
+        ### Step-by-step  (recommended)
+        
+        - install dependencies
+        - install environments
+        - install patches
+        
+        #### 1. install dependencies (basic)
+        
+        First, install MARLlib dependencies to guarantee basic usage.
+        following [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html), finally install patches for RLlib.
+        
+        ```bash
+        $ conda create -n marllib python=3.8 # or 3.9
+        $ conda activate marllib
+        $ git clone https://github.com/Replicable-MARL/MARLlib.git && cd MARLlib
+        $ pip install -r requirements.txt
+        ```
+        
+        #### 2. install environments (optional)
+        
+        Please follow [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html).
+        
+        #### 3. install patches (basic)
+        
+        Fix bugs of RLlib using patches by running the following command:
+        
+        ```bash
+        $ cd /Path/To/MARLlib/marl/patch
+        $ python add_patch.py -y
+        ```
+        
+        ### PyPI
+        
+        ```bash
+        $ pip install --upgrade pip
+        $ pip install marllib
+        ```
+        
+        ## Getting started
+        
+        <details>
+        <summary><b><big>Prepare the configuration</big></b></summary>
+        
+        There are four parts of configurations that take charge of the whole training process.
+        
+        - scenario: specify the environment/task settings
+        - algorithm: choose the hyperparameters of the algorithm
+        - model: customize the model architecture
+        - ray/rllib: change the basic training settings
+        
+        <div align="center">
+        <img src=docs/source/images/configurations.png width=100% />
+        </div>
+        
+        Before training, ensure all the parameters are set correctly, especially those you don't want to change.
+        > __Note__:
+        > You can also modify all the pre-set parameters via MARLLib API.*
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Register the environment</big></b></summary>
+        
+        Ensure all the dependencies are installed for the environment you are running with. Otherwise, please refer to
+        [MARLlib documentation](https://marllib.readthedocs.io/en/latest/handbook/env.html).
+        
+        
+        |   task mode   | api example |
+        | :-----------: | ----------- |
+        | cooperative | ```marl.make_env(environment_name="mpe", map_name="simple_spread", force_coop=True)``` |
+        | collaborative | ```marl.make_env(environment_name="mpe", map_name="simple_spread")``` |
+        | competitive | ```marl.make_env(environment_name="mpe", map_name="simple_adversary")``` |
+        | mixed | ```marl.make_env(environment_name="mpe", map_name="simple_crypto")``` |
+        
+        Most of the popular environments in MARL research are supported by MARLlib:
+        
+        | Env Name | Learning Mode | Observability | Action Space | Observations |
+        | :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
+        | **[LBF](https://github.com/semitable/lb-foraging)**  | cooperative + collaborative | Both | Discrete | 1D  |
+        | **[RWARE](https://github.com/semitable/robotic-warehouse)**  | cooperative | Partial | Discrete | 1D  |
+        | **[MPE](https://github.com/openai/multiagent-particle-envs)**  | cooperative + collaborative + mixed | Both | Both | 1D  |
+        | **[SMAC](https://github.com/oxwhirl/smac)**  | cooperative | Partial | Discrete | 1D |
+        | **[MetaDrive](https://github.com/decisionforce/metadrive)**  | collaborative | Partial | Continuous | 1D |
+        | **[MAgent](https://www.pettingzoo.ml/magent)** | collaborative + mixed | Partial | Discrete | 2D |
+        | **[Pommerman](https://github.com/MultiAgentLearning/playground)**  | collaborative + competitive + mixed | Both | Discrete | 2D |
+        | **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Full | Continuous | 1D |
+        | **[GRF](https://github.com/google-research/football)**  | collaborative + mixed | Full | Discrete | 2D |
+        | **[Hanabi](https://github.com/deepmind/hanabi-learning-environment)** | cooperative | Partial | Discrete | 1D |
+        | **[MATE](https://github.com/XuehaiPan/mate)** | cooperative + mixed | Partial | Both | 1D |
+        | **[GoBigger](https://github.com/opendilab/GoBigger)** | cooperative + mixed | Both | Continuous | 1D |
+        
+        Each environment has a readme file, standing as the instruction for this task, including env settings, installation, and
+        important notes.
+        </details>
+        
+        <details>
+        <summary><b><big>Initialize the algorithm</big></b></summary>
+        
+        
+        |  running target   | api example |
+        | :-----------: | ----------- |
+        | train & finetune  | ```marl.algos.mappo(hyperparam_source=$ENV)``` |
+        | develop & debug | ```marl.algos.mappo(hyperparam_source="test")``` |
+        | 3rd party env | ```marl.algos.mappo(hyperparam_source="common")``` |
+        
+        Here is a chart describing the characteristics of each algorithm:
+        
+        | algorithm                                                    | support task mode | discrete action   | continuous action |  policy type        |
+        | :------------------------------------------------------------: | :-----------------: | :----------: | :--------------------: | :----------: | 
+        | *IQL**                                                         | all four               | :heavy_check_mark:   |    |  off-policy |
+        | *[PG](https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf)* | all four                  | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[A2C](https://arxiv.org/abs/1602.01783)*                      | all four              | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[DDPG](https://arxiv.org/abs/1509.02971)*                     | all four             |  | :heavy_check_mark:   |  off-policy |
+        | *[TRPO](http://proceedings.mlr.press/v37/schulman15.pdf)*      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[PPO](https://arxiv.org/abs/1707.06347)*                      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[COMA](https://ojs.aaai.org/index.php/AAAI/article/download/11794/11653)* | all four                           | :heavy_check_mark:       |   |  on-policy  |
+        | *[MADDPG](https://arxiv.org/abs/1706.02275)*                   | all four                     |  | :heavy_check_mark:   |  off-policy |
+        | *MAA2C**                                                       | all four                        | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *MATRPO**                                                      | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[MAPPO](https://arxiv.org/abs/2103.01955)*                    | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[HATRPO](https://arxiv.org/abs/2109.11251)*                   | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[HAPPO](https://arxiv.org/abs/2109.11251)*                    | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[VDN](https://arxiv.org/abs/1706.05296)*                      | cooperative         | :heavy_check_mark:   |    |  off-policy |
+        | *[QMIX](https://arxiv.org/abs/1803.11485)*                     | cooperative                    | :heavy_check_mark:   |   |  off-policy |
+        | *[FACMAC](https://arxiv.org/abs/2003.06709)*                   | cooperative                    |  | :heavy_check_mark:   |  off-policy |
+        | *[VDAC](https://arxiv.org/abs/2007.12306)*                    | cooperative                    | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *VDPPO**                                                      | cooperative                | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        
+        ***all four**: cooperative collaborative competitive mixed
+        
+        *IQL* is the multi-agent version of Q learning.
+        *MAA2C* and *MATRPO* are the centralized version of A2C and TRPO.
+        *VDPPO* is the value decomposition version of PPO.
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Build the agent model</big></b></summary>
+        
+        An agent model consists of two parts, `encoder` and `core arch`. 
+        `encoder` will be constructed by MARLlib according to the observation space.
+        Choose `mlp`, `gru`, or `lstm` as you like to build the complete model.
+        
+        |  model arch   | api example |
+        | :-----------: | ----------- |
+        | MLP  | ```marl.build_model(env, algo, {"core_arch": "mlp")``` |
+        | GRU | ```marl.build_model(env, algo, {"core_arch": "gru"})```  |
+        | LSTM | ```marl.build_model(env, algo, {"core_arch": "lstm"})```  |
+        | Encoder Arch | ```marl.build_model(env, algo, {"core_arch": "gru", "encode_layer": "128-256"})```  |
+        
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Kick off the training</big></b></summary>
+        
+        |  setting   | api example |
+        | :-----------: | ----------- |
+        | train  | ```algo.fit(env, model)``` |
+        | debug  | ```algo.fit(env, model, local_mode=True)``` |
+        | stop condition | ```algo.fit(env, model, stop={'episode_reward_mean': 2000, 'timesteps_total': 10000000})```  |
+        | policy sharing | ```algo.fit(env, model, share_policy='all') # or 'group' / 'individual'```  |
+        | save model | ```algo.fit(env, model, checkpoint_freq=100, checkpoint_end=True)```  |
+        | GPU accelerate  | ```algo.fit(env, model, local_mode=False, num_gpus=1)``` |
+        | CPU accelerate | ```algo.fit(env, model, local_mode=False, num_workers=5)```  |
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Training & rendering API</big></b></summary>
+        
+        ```py
+        from marllib import marl
+        
+        # prepare env
+        env = marl.make_env(environment_name="mpe", map_name="simple_spread")
+        # initialize algorithm with appointed hyper-parameters
+        mappo = marl.algos.mappo(hyperparam_source="mpe")
+        # build agent model based on env + algorithms + user preference
+        model = marl.build_model(env, mappo, {"core_arch": "mlp", "encode_layer": "128-256"})
+        # start training
+        mappo.fit(
+          env, model, 
+          stop={"timesteps_total": 1000000}, 
+          checkpoint_freq=100, 
+          share_policy="group"
+        )
+        # rendering
+        mappo.render(
+          env, model, 
+          local_mode=True, 
+          restore_path={'params_path': "checkpoint_000010/params.json",
+                        'model_path': "checkpoint_000010/checkpoint-10"}
+        )
+        ```
+        </details>
+        
+        ## Benchmark results
+        
+        All results are listed [here](https://github.com/Replicable-MARL/MARLlib/tree/main/results).
+        
+        ## Quick examples
+        
+        MARLlib provides some practical examples for you to refer to.
+        
+        - [Detailed API usage](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/api_basic_usage.py): show how to use MARLlib api in
+          detail, e.g. cmd + api combined running.
+        - [Policy sharing cutomization](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/customize_policy_sharing.py):
+          define your group policy-sharing strategy as you like based on current tasks.
+        - [Loading model and rendering](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/load_and_render_model.py):
+          render the environment based on the pre-trained model.
+        - [Incorporating new environment](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_env.py):
+          add your new environment following MARLlib's env-agent interaction interface.
+        - [Incorporating new algorithm](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_algorithm.py):
+          add your new algorithm following MARLlib learning pipeline.
+        
+        ## Tutorials
+        
+        Try MPE + MAPPO examples on Google Colaboratory!
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
+        
+        More tutorial documentations are available [here](https://marllib.readthedocs.io/).
+        
+        ## Awesome List
+        
+        A collection of research and review papers of multi-agent reinforcement learning (MARL) is available. The papers have been organized based on their publication date and their evaluation of the corresponding environments.
+        
+        Algorithms: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
+        Environments: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/handbook/env.html)
+        
+        
+        ## Community
+        
+        |  Channel   | Link |
+        | :----------- | :----------- |
+        | Issues | [GitHub Issues](https://github.com/Replicable-MARL/MARLlib/issues) |
+        
+        ## Roadmap
+        
+        The roadmap to the future release is available in [ROADMAP.md](https://github.com/Replicable-MARL/MARLlib/blob/main/ROADMAP.md).
+        
+        ## Contributing
+        
+        We are a small team on multi-agent reinforcement learning, and we will take all the help we can get! 
+        If you would like to get involved, here is information on [contribution guidelines and how to test the code locally](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/CONTRIBUTING.md).
+        
+        You can contribute in multiple ways, e.g., reporting bugs, writing or translating documentation, reviewing or refactoring code, requesting or implementing new features, etc.
+        
+        ## Paper
+        
+        If you use MARLlib in your research, please cite the [MARLlib paper](https://arxiv.org/abs/2210.13708).
+        
+        ```tex
+        @article{hu2022marllib,
+          title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},
+          author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},
+          journal={arXiv preprint arXiv:2210.13708},
+          year={2022}
+        }
+        ```
+        
+        
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `marllib-1.0.2/README.rst` & `marllib-1.0.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         :target: https://github.com/Replicable-MARL/MARLlib/stargazers
         :alt: GitHub stars
      
      - any task with **no task mode restriction**
      - 18
      - share + group + separate + customizable
      - MLP / CNN / GRU / LSTM
-     - Ray/Rllib
+     - Ray/RLlib
 
 
 What **MARLlib** brings to MARL community:
 
 
 * MARLlib unifies diverse algorithm pipeline with agent-level distributed dataflow.
 * MARLlib supports all task modes: cooperative, collaborative, competitive, and mixed.
```

### Comparing `marllib-1.0.2/marllib/__init__.py` & `marllib-1.0.3/marllib/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/__init__.py` & `marllib-1.0.3/marllib/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/__init__.py` & `marllib-1.0.3/marllib/envs/base_env/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,66 +19,78 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 ENV_REGISTRY = {}
 
 try:
-    from marllib.envs.base_env.mpe import RllibMPE
-    ENV_REGISTRY["mpe"] = RllibMPE
+    from marllib.envs.base_env.mpe import RLlibMPE
+    ENV_REGISTRY["mpe"] = RLlibMPE
 except Exception as e:
     ENV_REGISTRY["mpe"] = str(e)
 
 try:
-    from marllib.envs.base_env.mamujoco import RllibMAMujoco
-    ENV_REGISTRY["mamujoco"] = RllibMAMujoco
+    from marllib.envs.base_env.mamujoco import RLlibMAMujoco
+    ENV_REGISTRY["mamujoco"] = RLlibMAMujoco
 except Exception as e:
     ENV_REGISTRY["mamujoco"] = str(e)
 
 try:
     from marllib.envs.base_env.smac import RLlibSMAC
     ENV_REGISTRY["smac"] = RLlibSMAC
 except Exception as e:
     ENV_REGISTRY["smac"] = str(e)
 
 try:
-    from marllib.envs.base_env.football import RllibGFootball
-    ENV_REGISTRY["football"] = RllibGFootball
+    from marllib.envs.base_env.football import RLlibGFootball
+    ENV_REGISTRY["football"] = RLlibGFootball
 except Exception as e:
     ENV_REGISTRY["football"] = str(e)
 
 try:
-    from marllib.envs.base_env.magent import RllibMAgent
-    ENV_REGISTRY["magent"] = RllibMAgent
+    from marllib.envs.base_env.magent import RLlibMAgent
+    ENV_REGISTRY["magent"] = RLlibMAgent
 except Exception as e:
     ENV_REGISTRY["magent"] = str(e)
 
 try:
-    from marllib.envs.base_env.rware import RllibRWARE
-    ENV_REGISTRY["rware"] = RllibRWARE
+    from marllib.envs.base_env.rware import RLlibRWARE
+    ENV_REGISTRY["rware"] = RLlibRWARE
 except Exception as e:
     ENV_REGISTRY["rware"] = str(e)
 
 try:
-    from marllib.envs.base_env.lbf import RllibLBF
-    ENV_REGISTRY["lbf"] = RllibLBF
+    from marllib.envs.base_env.lbf import RLlibLBF
+    ENV_REGISTRY["lbf"] = RLlibLBF
 except Exception as e:
     ENV_REGISTRY["lbf"] = str(e)
 
 try:
-    from marllib.envs.base_env.pommerman import RllibPommerman
-    ENV_REGISTRY["pommerman"] = RllibPommerman
+    from marllib.envs.base_env.pommerman import RLlibPommerman
+    ENV_REGISTRY["pommerman"] = RLlibPommerman
 except Exception as e:
     ENV_REGISTRY["pommerman"] = str(e)
 
 try:
     from marllib.envs.base_env.hanabi import RLlibHanabi
     ENV_REGISTRY["hanabi"] = RLlibHanabi
 except Exception as e:
     ENV_REGISTRY["hanabi"] = str(e)
 
 try:
-    from marllib.envs.base_env.metadrive import RllibMetaDrive
-    ENV_REGISTRY["metadrive"] = RllibMetaDrive
+    from marllib.envs.base_env.metadrive import RLlibMetaDrive
+    ENV_REGISTRY["metadrive"] = RLlibMetaDrive
 except Exception as e:
     ENV_REGISTRY["metadrive"] = str(e)
 
+try:
+    from marllib.envs.base_env.mate import RLlibMATE
+    ENV_REGISTRY["mate"] = RLlibMATE
+except Exception as e:
+    ENV_REGISTRY["mate"] = str(e)
+
+try:
+    from marllib.envs.base_env.gobigger import RLlibGoBigger
+    ENV_REGISTRY["gobigger"] = RLlibGoBigger
+except Exception as e:
+    ENV_REGISTRY["gobigger"] = str(e)
+
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/__init__.py` & `marllib-1.0.3/marllib/patch/rllib/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/football.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/football.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/hanabi.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/hanabi.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/lbf.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/lbf.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 env: lbf
 
 env_args:
   players: 4
-  field_size_x: 15
-  field_size_y: 15
-  max_food: 3
-  sight: 15
+  field_size_x: 8
+  field_size_y: 8
+  max_food: 2
+  sight: 3
   force_coop: False
   max_episode_steps: 50
   max_player_level: 3
 
 mask_flag: False
 global_state_flag: False
 opp_action_in_cc: True
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/magent.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/magent.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/mamujoco.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/mamujoco.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/metadrive.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/metadrive.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/mpe.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/mpe.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/pommerman.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/pommerman.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/rware.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/rware.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,12 +27,12 @@
   map_size: "tiny" # "tiny", "small", "medium", "large"
   difficulty: "medium" # "easy", "medium", "hard"
   column_height: 1
   max_inactivity_steps: null
   max_steps: 500
   fast_obs: True
   msg_bits: 0
-  sensor_range: 2
+  sensor_range: 1
 
 mask_flag: False
 global_state_flag: False
 opp_action_in_cc: True
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/config/smac.yaml` & `marllib-1.0.3/marllib/envs/base_env/config/smac.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/football.py` & `marllib-1.0.3/marllib/envs/base_env/football.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         "description": "football all scenarios",
         "team_prefix": ("agent_",),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
-class RllibGFootball(MultiAgentEnv):
+class RLlibGFootball(MultiAgentEnv):
     """An example of a wrapper for GFootball to make it compatible with rllib."""
 
     def __init__(self, env_config):
         env_config["env_name"] = env_config.pop("map_name")
         self.env_config = env_config
         self.num_agents = ally_num_dict[self.env_config["env_name"]]
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/hanabi.py` & `marllib-1.0.3/marllib/envs/base_env/hanabi.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/install/__init__.py` & `marllib-1.0.3/marllib/patch/rllib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/base_env/lbf.py` & `marllib-1.0.3/marllib/envs/base_env/lbf.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "description": "lbf all scenarios",
         "team_prefix": ("agent_",),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
-class RllibLBF(MultiAgentEnv):
+class RLlibLBF(MultiAgentEnv):
 
     def __init__(self, env_config):
         map_name = env_config["map_name"]
         env_config.pop("map_name", None)
         field_size_y = env_config.pop("field_size_y", None)
         field_size_x = env_config.pop("field_size_x", None)
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/magent.py` & `marllib-1.0.3/marllib/envs/base_env/magent.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         "team_prefix": ("tiger_", "deer_"),
         "all_agents_one_policy": False,
         "one_agent_one_policy": False,
     },
 }
 
 
-class RllibMAgent(MultiAgentEnv):
+class RLlibMAgent(MultiAgentEnv):
 
     def __init__(self, env_config):
         map = env_config.pop("map_name", None)
 
         env = REGISTRY[map](**env_config)
 
         # keep obs and action dim same across agents
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/mamujoco.py` & `marllib-1.0.3/marllib/envs/base_env/mamujoco.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         "team_prefix": ("agent_",),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
 
-class RllibMAMujoco(MultiAgentEnv):
+class RLlibMAMujoco(MultiAgentEnv):
 
     def __init__(self, env_config):
         self.env_config = env_args_dict[env_config["map_name"]]
         self.env = MujocoMulti(env_args=self.env_config)
         self.action_space = self.env.action_space[0]
         self.state_dim = self.env.wrapped_env.observation_space.shape[0]
         self.observation_space = GymDict({
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/metadrive.py` & `marllib-1.0.3/marllib/envs/base_env/metadrive.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
 
 def dynamic_inheritance(super_class):
-    class RllibMetaDrive_Scenario(super_class):
+    class RLlibMetaDrive_Scenario(super_class):
 
         def __init__(self, config):
             map = config["map_name"]
             config.pop("map_name", None)
             super(super_class, self).__init__(config)
             self.__name__ = map
             self.__qualname__ = map
@@ -59,18 +59,18 @@
             self.distance_map = defaultdict(lambda: defaultdict(lambda: float("inf")))
 
         def step(self, actions):
             obs, reward, done, info = super(super_class, self).step(actions)
             update_neighbours_map(self.distance_map, self.vehicles, reward, info, self.config)
             return obs, reward, done, info
 
-    return RllibMetaDrive_Scenario
+    return RLlibMetaDrive_Scenario
 
 
-class RllibMetaDrive(MultiAgentEnv):
+class RLlibMetaDrive(MultiAgentEnv):
 
     def __init__(self, env_config):
         map = env_config["map_name"]
         super_class = SUPER_REGISTRY[map]
         env_class = dynamic_inheritance(super_class)
         self.env = env_class(env_config)
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/mpe.py` & `marllib-1.0.3/marllib/envs/base_env/mpe.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         "team_prefix": ("speaker_", "listener_"),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
 
-class RllibMPE(MultiAgentEnv):
+class RLlibMPE(MultiAgentEnv):
 
     def __init__(self, env_config):
         map = env_config["map_name"]
         env_config.pop("map_name", None)
         env = REGISTRY[map](**env_config)
 
         # keep obs and action dim same across agents
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/pommerman.py` & `marllib-1.0.3/marllib/envs/base_env/pommerman.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "description": "pommerman all scenarios",
         "team_prefix": ("agent_",),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
-class RllibPommerman(MultiAgentEnv):
+class RLlibPommerman(MultiAgentEnv):
 
     def __init__(self, env_config):
         agent_position = env_config["agent_position"]
         map = env_config["map_name"]
         builtin_ai_type = env_config["builtin_ai_type"]
 
         if "One" in map:
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/rware.py` & `marllib-1.0.3/marllib/envs/base_env/rware.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         "team_prefix": ("agent_",),
         "all_agents_one_policy": True,
         "one_agent_one_policy": True,
     },
 }
 
 
-class RllibRWARE(MultiAgentEnv):
+class RLlibRWARE(MultiAgentEnv):
 
     def __init__(self, env_config):
 
         map_name = env_config["map_name"]
         map_size = env_config["map_size"]
         difficulty = env_config["difficulty"]
```

### Comparing `marllib-1.0.2/marllib/envs/base_env/smac.py` & `marllib-1.0.3/marllib/envs/base_env/smac.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/__init__.py` & `marllib-1.0.3/marllib/envs/global_reward_env/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,54 +19,75 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 COOP_ENV_REGISTRY = {}
 
 try:
-    from marllib.envs.global_reward_env.mpe_fcoop import RllibMPE_FCOOP
-    COOP_ENV_REGISTRY["mpe"] = RllibMPE_FCOOP
+    from marllib.envs.global_reward_env.mpe_fcoop import RLlibMPE_FCOOP
+
+    COOP_ENV_REGISTRY["mpe"] = RLlibMPE_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["mpe"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.magent_fcoop import RllibMAgent_FCOOP
-    COOP_ENV_REGISTRY["magent"] = RllibMAgent_FCOOP
+    from marllib.envs.global_reward_env.magent_fcoop import RLlibMAgent_FCOOP
+
+    COOP_ENV_REGISTRY["magent"] = RLlibMAgent_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["magent"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.mamujoco_fcoop import RllibMAMujoco_FCOOP
-    COOP_ENV_REGISTRY["mamujoco"] = RllibMAMujoco_FCOOP
+    from marllib.envs.global_reward_env.mamujoco_fcoop import RLlibMAMujoco_FCOOP
+
+    COOP_ENV_REGISTRY["mamujoco"] = RLlibMAMujoco_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["mamujoco"] = str(e)
 
 try:
     from marllib.envs.global_reward_env.smac_fcoop import RLlibSMAC_FCOOP
+
     COOP_ENV_REGISTRY["smac"] = RLlibSMAC_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["smac"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.football_fcoop import RllibGFootball_FCOOP
-    COOP_ENV_REGISTRY["football"] = RllibGFootball_FCOOP
+    from marllib.envs.global_reward_env.football_fcoop import RLlibGFootball_FCOOP
+
+    COOP_ENV_REGISTRY["football"] = RLlibGFootball_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["football"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.rware_fcoop import RllibRWARE_FCOOP
-    COOP_ENV_REGISTRY["rware"] = RllibRWARE_FCOOP
+    from marllib.envs.global_reward_env.rware_fcoop import RLlibRWARE_FCOOP
+
+    COOP_ENV_REGISTRY["rware"] = RLlibRWARE_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["rware"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.lbf_fcoop import RllibLBF_FCOOP
-    COOP_ENV_REGISTRY["lbf"] = RllibLBF_FCOOP
+    from marllib.envs.global_reward_env.lbf_fcoop import RLlibLBF_FCOOP
+
+    COOP_ENV_REGISTRY["lbf"] = RLlibLBF_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["lbf"] = str(e)
 
 try:
-    from marllib.envs.global_reward_env.pommerman_fcoop import RllibPommerman
-    COOP_ENV_REGISTRY["pommerman"] = RllibPommerman
+    from marllib.envs.global_reward_env.pommerman_fcoop import RLlibPommerman_FCOOP
+
+    COOP_ENV_REGISTRY["pommerman"] = RLlibPommerman_FCOOP
 except Exception as e:
     COOP_ENV_REGISTRY["pommerman"] = str(e)
 
+try:
+    from marllib.envs.global_reward_env.mate_fcoop import RLlibMATE_FCOOP
+
+    COOP_ENV_REGISTRY["mate"] = RLlibMATE_FCOOP
+except Exception as e:
+    COOP_ENV_REGISTRY["mate"] = str(e)
+
+try:
+    from marllib.envs.global_reward_env.gobigger_fcoop import RLlibGoBigger_FCOOP
+
+    COOP_ENV_REGISTRY["gobigger"] = RLlibGoBigger_FCOOP
+except Exception as e:
+    COOP_ENV_REGISTRY["gobigger"] = str(e)
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/football_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/football_fcoop.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.football import RllibGFootball
+from marllib.envs.base_env.football import RLlibGFootball
 
 
-class RllibGFootball_FCOOP(RllibGFootball):
+class RLlibGFootball_FCOOP(RLlibGFootball):
 
     def step(self, action_dict):
         actions = []
         for key, value in sorted(action_dict.items()):
             actions.append(value)
         o, r, d, i = self.env.step(actions)
         r = sum(r)
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/lbf_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/lbf_fcoop.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.lbf import RllibLBF
+from marllib.envs.base_env.lbf import RLlibLBF
 
 
-class RllibLBF_FCOOP(RllibLBF):
+class RLlibLBF_FCOOP(RLlibLBF):
 
     def __init__(self, env_config):
         env_config["force_coop"] = True
         super().__init__(env_config)
 
     def step(self, action_dict):
         actions = []
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/magent_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/magent_fcoop.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.magent import RllibMAgent
+from marllib.envs.base_env.magent import RLlibMAgent
 
 legal_scenarios = ["gather"]
 
 
-class RllibMAgent_FCOOP(RllibMAgent):
+class RLlibMAgent_FCOOP(RLlibMAgent):
 
     def __init__(self, env_config):
         if env_config["map_name"] not in legal_scenarios:
             raise ValueError("must in: 1.gather")
         super().__init__(env_config)
 
     def reset(self):
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/mamujoco_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/mamujoco_fcoop.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.mamujoco import RllibMAMujoco as RllibMAMujoco_FCOOP
+from marllib.envs.base_env.mamujoco import RLlibMAMujoco as RLlibMAMujoco_FCOOP
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/mpe_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/mpe_fcoop.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.mpe import RllibMPE
+from marllib.envs.base_env.mpe import RLlibMPE
 
 legal_scenarios = ["simple_spread", "simple_reference", "simple_speaker_listener"]
 
 
-class RllibMPE_FCOOP(RllibMPE):
+class RLlibMPE_FCOOP(RLlibMPE):
 
     def __init__(self, env_config):
         if env_config["map_name"] not in legal_scenarios:
             raise ValueError("must in: 1.simple_spread, 2.simple_reference, 3.simple_speaker_listener")
         super().__init__(env_config)
 
     def step(self, action_dict):
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/pommerman_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/pommerman_fcoop.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
-from marllib.envs.base_env.pommerman import RllibPommerman, get_obs_dict
+from marllib.envs.base_env.pommerman import RLlibPommerman, get_obs_dict
 
 
 """
 "OneVsOne-v0",
 "PommeFFACompetition-v0",
 "PommeTeamCompetition-v0",
 """
 
 
-class RllibPommerman_FCOOP(RllibPommerman):
+class RLlibPommerman_FCOOP(RLlibPommerman):
 
     def step(self, action_dict):
         # fake action
         if self.map == "OneVsOne-v0":  # 2 agents map
             actions = [-1, -1, ]
         else:
             actions = [-1, -1, -1, -1]
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/rware_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/rware_fcoop.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from marllib.envs.base_env.rware import RllibRWARE
+from marllib.envs.base_env.rware import RLlibRWARE
 
 
-class RllibRWARE_FCOOP(RllibRWARE):
+class RLlibRWARE_FCOOP(RLlibRWARE):
 
     def step(self, action_dict):
         actions = []
         for key, value in sorted(action_dict.items()):
             actions.append(value)
-        try:
-            o, r, d, i = self.env.step(actions)
-        except Exception as e:
-            print(e)
+        o, r, d, i = self.env.step(actions)
         # cooperative need global reward
         r = sum(r)
         rewards = {}
         obs = {}
         infos = {}
         done_flag = False
         for pos, key in enumerate(sorted(action_dict.keys())):
```

### Comparing `marllib-1.0.2/marllib/envs/global_reward_env/smac_fcoop.py` & `marllib-1.0.3/marllib/envs/global_reward_env/smac_fcoop.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/__init__.py` & `marllib-1.0.3/marllib/marl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,16 @@
         model_config = get_model_config("rnn")
     elif model_preference["core_arch"] in ["mlp"]:
         model_config = get_model_config("mlp")
     else:
         raise NotImplementedError("{} not supported agent model arch".format(model_preference["core_arch"]))
 
     if len(environment[0].observation_space.spaces["obs"].shape) == 1:
-        print("use fc encoder")
         encoder = "fc_encoder"
     else:
-        print("use cnn encoder")
         encoder = "cnn_encoder"
 
     # encoder config
     encoder_arch_config = get_model_config(encoder)
     model_config = recursive_dict_update(model_config, encoder_arch_config)
     model_config = recursive_dict_update(model_config, {"model_arch_args": model_preference})
```

### Comparing `marllib-1.0.2/marllib/marl/algos/__init__.py` & `marllib-1.0.3/marllib/marl/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/__init__.py` & `marllib-1.0.3/marllib/patch/rllib/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/coma.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/coma.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/happo.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/happo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/hatrpo.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/hatrpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Implement TRPO and HATRPO in Ray Rllib
+Implement TRPO and HATRPO in Ray RLlib
 __author__: minquan
 __data__: May-15
 """
 
 import logging
 from typing import List, Type, Union
 from ray.rllib.models.torch.torch_action_dist import TorchDistributionWrapper
```

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/maa2c.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/maa2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/maddpg.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/maddpg.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/mappo.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/mappo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/CC/matrpo.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/matrpo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/IL/__init__.py` & `marllib-1.0.3/marllib/patch/rllib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/IL/a2c.py` & `marllib-1.0.3/marllib/marl/algos/core/IL/a2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/IL/ddpg.py` & `marllib-1.0.3/marllib/marl/algos/core/IL/ddpg.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/IL/ppo.py` & `marllib-1.0.3/marllib/marl/algos/core/IL/ppo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/IL/trpo.py` & `marllib-1.0.3/marllib/marl/algos/core/IL/trpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Implement TRPO and HATRPO in Ray Rllib
+Implement TRPO and HATRPO in Ray RLlib
 __author__: minquan
 __data__: May-15
 """
 
 import logging
 from typing import List, Type, Union
 from ray.rllib.models.torch.torch_action_dist import TorchDistributionWrapper
```

### Comparing `marllib-1.0.2/marllib/marl/algos/core/VD/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/VD/facmac.py` & `marllib-1.0.3/marllib/marl/algos/core/VD/facmac.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/VD/iql_vdn_qmix.py` & `marllib-1.0.3/marllib/marl/algos/core/VD/iql_vdn_qmix.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/VD/vda2c.py` & `marllib-1.0.3/marllib/marl/algos/core/VD/vda2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/VD/vdppo.py` & `marllib-1.0.3/marllib/marl/algos/core/VD/vdppo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/core/__init__.py` & `marllib-1.0.3/marllib/marl/algos/core/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/coma.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/coma.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/facmac.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/maddpg.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# FACMAC parameters
+# MADDPG parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
   batch_episode:  8
   learning_starts_episode: 16
   twin_q: False
@@ -32,10 +32,9 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
-  mixer: "qmix" # qmix or vdn
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/happo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/happo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
   critic_lr: 0.0005
   vf_loss_coeff: 1.0
   lr: 0.0000005
   gain: 0.01
   entropy_coeff: 0.01
   vf_clip_param: 10.0
   min_lr_schedule: 1e-11
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/hatrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/hatrpo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,11 +30,11 @@
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/ia2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/ia2c.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/iddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/iddpg.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 # DDPG parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
   batch_episode:  8
-  learning_starts_episode: 16
+  learning_starts_episode: 8
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/ippo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/ippo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
-  batch_episode: 10
+  batch_episode: 2
   num_sgd_iter: 5
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/iql.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/iql.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/itrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/matrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# TRPO parameters
+# MATRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
   batch_episode: 10
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/maa2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/maa2c.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/maddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/iddpg.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MADDPG parameters
+# DDPG parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
   batch_episode:  8
   learning_starts_episode: 16
   twin_q: False
@@ -32,9 +32,9 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/mappo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/mappo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
   batch_episode: 10
-  num_sgd_iter: 5
+  num_sgd_iter: 10
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/matrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/happo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MATRPO parameters
+# HAPPO parameters
 
 algo_args:
   use_gae: True
-  lambda: 1.0
   gamma: 0.99
-  batch_episode: 10
+  lambda: 1.0
+  batch_episode: 2
   kl_coeff: 0.2
-  num_sgd_iter: 1
+  num_sgd_iter: 5
   grad_clip: 10
+  gain: 0.01
   clip_param: 0.3
+  critic_lr: 0.0005
   vf_loss_coeff: 1.0
+  lr: 0.0000005
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-  kl_threshold: 0.00001
-  accept_ratio: 0.5
-  critic_lr: 0.00005
+  min_lr_schedule: 1e-11
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/qmix.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/qmix.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/vda2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vda2c.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/vdn.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/vdn.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/common/vdppo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vdppo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -28,12 +28,12 @@
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
   batch_episode: 10
   num_sgd_iter: 5
   vf_loss_coeff: 1.0
   lr: 0.0005
-  entropy_coeff: 0.01
+  entropy_coeff: 0.001
   clip_param: 0.3
-  vf_clip_param: 10.0
+  vf_clip_param: 20.0
   batch_mode: "complete_episodes"
   mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/facmac.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/maddpg.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# FACMAC parameters
+# MADDPG parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
-  batch_episode:  10
-  learning_starts_episode: 10
+  batch_episode:  128
+  learning_starts_episode: 128
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
-  critic_lr: 0.0005
-  actor_lr: 0.0005
-  buffer_size_episode: 1000
+  critic_lr: 0.00005
+  actor_lr: 0.00005
+  buffer_size_episode: 10000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
-  mixer: "qmix" # qmix or vdn
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/happo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/happo.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,10 @@
   grad_clip: 10
   clip_param: 0.3
   critic_lr: 0.000001
   vf_loss_coeff: 1.0
   lr: 0.0001
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   min_lr_schedule: 1e-11
   gain: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/hatrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/hatrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,12 +30,12 @@
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/ia2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/vdppo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# A2C parameters
+# VDPPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 10
+  num_sgd_iter: 5
   vf_loss_coeff: 1.0
-  batch_episode:  10
-  batch_mode: "complete_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
+  clip_param: 0.3
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+  mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/iddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/iddpg.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 # SOFTWARE.
 
 # DDPG parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
-  batch_episode:  8
-  learning_starts_episode: 8
+  batch_episode:  128
+  learning_starts_episode: 128
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/ippo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/coma.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# PPO parameters
+# COMA parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
-  kl_coeff: 0.2
-  batch_episode: 10
-  num_sgd_iter: 10
   vf_loss_coeff: 1.0
+  batch_episode:  2
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
-  clip_param: 0.3
-  vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/itrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/happo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# TRPO parameters
-
+# HAPPO parameters
 algo_args:
   use_gae: True
   lambda: 1.0
-  gamma: 0.99
   batch_episode: 10
   kl_coeff: 0.2
-  num_sgd_iter: 1
+  num_sgd_iter: 5
   grad_clip: 10
   clip_param: 0.3
+  critic_lr: 0.00005
   vf_loss_coeff: 1.0
+  lr: 0.00005
+  gamma: 0.99
   entropy_coeff: 0.01
-  vf_clip_param: 10.0
+  vf_clip_param: 20.0
+  min_lr_schedule: 1e-11
   batch_mode: "complete_episodes"
-  kl_threshold: 0.00001
-  accept_ratio: 0.5
-  critic_lr: 0.0005
+
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/maa2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/vdppo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MAA2C parameters
+# VDPPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 2
+  num_sgd_iter: 5
   vf_loss_coeff: 1.0
-  batch_episode:  10
-  batch_mode: "complete_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
+  clip_param: 0.3
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+  mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/maddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/maddpg.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/mappo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/mappo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
   batch_episode: 10
-  num_sgd_iter: 10
+  num_sgd_iter: 5
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/matrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/matrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/vda2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/vda2c.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
   batch_episode:  10
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
   mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mamujoco/vdppo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/vda2c.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDPPO parameters
+# VDA2C parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
-  kl_coeff: 0.2
-  batch_episode: 10
-  num_sgd_iter: 10
   vf_loss_coeff: 1.0
+  batch_episode:  10
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
-  clip_param: 0.3
-  vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-  mixer: "qmix" # qmix or vdn
+  mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/coma.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/ia2c.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# COMA parameters
+# A2C parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
-  batch_episode:  128
-  batch_mode: "complete_episodes"
+  batch_episode:  10
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/facmac.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/facmac.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -32,10 +32,10 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/happo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/happo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
   critic_lr: 0.0005
   vf_loss_coeff: 1.0
   lr: 0.0000005
   gain: 0.01
   entropy_coeff: 0.01
   vf_clip_param: 10.0
   min_lr_schedule: 1e-11
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/hatrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/itrpo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# HATRPO parameters
+# TRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
   batch_episode: 128
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/ia2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/mappo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# A2C parameters
+# MAPPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 2
+  num_sgd_iter: 2
   vf_loss_coeff: 1.0
-  batch_episode:  10
-  batch_mode: "complete_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
+  clip_param: 0.3
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+
+
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/iddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/facmac.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# DDPG parameters
+# FACMAC parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
-  batch_episode:  128
-  learning_starts_episode: 128
+  batch_episode:  8
+  learning_starts_episode: 16
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
+  mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/ippo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/ippo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
   batch_episode: 128
   num_sgd_iter: 10
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 20.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/iql.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/iql.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/itrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/itrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 # TRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
-  batch_episode: 128
+  batch_episode: 2
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
-  critic_lr: 0.0005
+  critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/maa2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/maa2c.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
-  batch_episode:  128
-  batch_mode: "complete_episodes"
+  batch_episode:  10
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/maddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/facmac.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MADDPG parameters
+# FACMAC parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
-  batch_episode:  128
-  learning_starts_episode: 128
+  batch_episode:  2
+  learning_starts_episode: 2
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
-  critic_lr: 0.00005
-  actor_lr: 0.00005
-  buffer_size_episode: 10000
+  critic_lr: 0.0005
+  actor_lr: 0.0005
+  buffer_size_episode: 10
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
+  mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/mappo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/mappo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,10 @@
   batch_episode: 128
   num_sgd_iter: 10
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 20.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/matrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/hatrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MATRPO parameters
+# HATRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
-  batch_episode: 128
+  batch_episode: 2
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
-  critic_lr: 0.0005
+  critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/qmix.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/qmix.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vda2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/ia2c.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDA2C parameters
+# A2C parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
-  batch_episode:  128
-  batch_mode: "complete_episodes"
+  batch_episode:  10
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
-  mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vdn.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vdn.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/mpe/vdppo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vdppo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -31,9 +31,9 @@
   batch_episode: 128
   num_sgd_iter: 10
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.01
   clip_param: 0.3
   vf_clip_param: 20.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/coma.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/coma.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
   batch_episode:  10
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/happo.yaml` & `marllib-1.0.3/marllib/marl/models/configs/mixer.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,25 +16,13 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# HAPPO parameters
-algo_args:
-  use_gae: True
-  lambda: 1.0
-  batch_episode: 10
-  kl_coeff: 0.2
-  num_sgd_iter: 5
-  grad_clip: 10
-  clip_param: 0.3
-  critic_lr: 0.00005
-  vf_loss_coeff: 1.0
-  lr: 0.00005
-  gamma: 0.99
-  entropy_coeff: 0.01
-  vf_clip_param: 20.0
-  min_lr_schedule: 1e-11
-  batch_mode: "complete_episodes"
+# rnn parameters
+
+model_arch_args:
+  mixer_embedding: 256
+  mixer_arch: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/hatrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/matrpo.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/ia2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/ippo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# A2C parameters
+# PPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 10
+  num_sgd_iter: 5
   vf_loss_coeff: 1.0
-  batch_episode:  10
-  batch_mode: "complete_episodes"
   lr: 0.0005
-  entropy_coeff: 0.01
+  entropy_coeff: 0.001
+  clip_param: 0.3
+  vf_clip_param: 20.0
+  batch_mode: "complete_episodes"
+
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/ippo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/mappo.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# PPO parameters
+# MAPPO parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
@@ -33,7 +33,8 @@
   vf_loss_coeff: 1.0
   lr: 0.0005
   entropy_coeff: 0.001
   clip_param: 0.3
   vf_clip_param: 20.0
   batch_mode: "complete_episodes"
 
+
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/iql.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/iql.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/itrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/hatrpo.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/maa2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/ippo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MAA2C parameters
+# PPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 10
+  num_sgd_iter: 5
   vf_loss_coeff: 1.0
-  batch_episode:  10
-  batch_mode: "complete_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
+  clip_param: 0.3
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/mappo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/ippo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MAPPO parameters
+# PPO parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   kl_coeff: 0.2
   batch_episode: 10
-  num_sgd_iter: 5
+  num_sgd_iter: 10
   vf_loss_coeff: 1.0
   lr: 0.0005
-  entropy_coeff: 0.001
+  entropy_coeff: 0.01
   clip_param: 0.3
-  vf_clip_param: 20.0
-  batch_mode: "complete_episodes"
-
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/matrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/itrpo.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/qmix.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/qmix.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vda2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/ia2c.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDA2C parameters
+# A2C parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
   batch_episode:  10
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
-  mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vdn.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/smac/vdn.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/finetuned/smac/vdppo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/maa2c.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDPPO parameters
+# MAA2C parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
-  kl_coeff: 0.2
-  batch_episode: 10
-  num_sgd_iter: 5
   vf_loss_coeff: 1.0
+  batch_episode:  10
+  batch_mode: "truncate_episodes"
   lr: 0.0005
-  entropy_coeff: 0.001
-  clip_param: 0.3
-  vf_clip_param: 20.0
-  batch_mode: "complete_episodes"
-  mixer: "qmix" # qmix or vdn
+  entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/__init__.py` & `marllib-1.0.3/marllib/marl/algos/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/coma.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/coma.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
   vf_loss_coeff: 1.0
-  batch_episode:  2
-  batch_mode: "complete_episodes"
+  batch_episode:  128
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/facmac.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/facmac.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 # SOFTWARE.
 
 # FACMAC parameters
 
 # Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ddpg/iddpg.py
 
 algo_args:
-  batch_episode:  2
-  learning_starts_episode: 2
+  batch_episode:  10
+  learning_starts_episode: 10
   twin_q: False
   prioritized_replay: False
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
-  buffer_size_episode: 10
+  buffer_size_episode: 1000
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/happo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/common/itrpo.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# HAPPO parameters
+# TRPO parameters
 
 algo_args:
   use_gae: True
-  gamma: 0.99
   lambda: 1.0
-  batch_episode: 2
+  gamma: 0.99
+  batch_episode: 10
   kl_coeff: 0.2
-  num_sgd_iter: 5
+  num_sgd_iter: 1
   grad_clip: 10
-  gain: 0.01
   clip_param: 0.3
-  critic_lr: 0.0005
   vf_loss_coeff: 1.0
-  lr: 0.0000005
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  min_lr_schedule: 1e-11
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
+  kl_threshold: 0.00001
+  accept_ratio: 0.5
+  critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/hatrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/matrpo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# HATRPO parameters
+# MATRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
   batch_episode: 2
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
   critic_lr: 0.00005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/ia2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/vdppo.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# A2C parameters
+# VDPPO parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  kl_coeff: 0.2
+  batch_episode: 10
+  num_sgd_iter: 10
   vf_loss_coeff: 1.0
-  batch_episode:  2
-  batch_mode: "complete_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
+  clip_param: 0.3
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+  mixer: "qmix" # qmix or vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/iddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/iddpg.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,9 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 10
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/ippo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/vda2c.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# PPO parameters
+# VDA2C parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
 
 algo_args:
   use_gae: True
   lambda: 1.0
-  kl_coeff: 0.2
-  batch_episode: 2
-  num_sgd_iter: 5
   vf_loss_coeff: 1.0
+  batch_episode:  2
+  batch_mode: "truncate_episodes"
   lr: 0.0005
   entropy_coeff: 0.01
-  clip_param: 0.3
-  vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-
+  mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/iql.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/iql.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/itrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mamujoco/itrpo.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 # TRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
   gamma: 0.99
-  batch_episode: 2
+  batch_episode: 10
   kl_coeff: 0.2
   num_sgd_iter: 1
   grad_clip: 10
   clip_param: 0.3
   vf_loss_coeff: 1.0
   entropy_coeff: 0.01
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
   kl_threshold: 0.00001
   accept_ratio: 0.5
-  critic_lr: 0.00005
+  critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/maa2c.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/matrpo.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MAA2C parameters
-
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+# MATRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  gamma: 0.99
+  batch_episode: 128
+  kl_coeff: 0.2
+  num_sgd_iter: 1
+  grad_clip: 10
+  clip_param: 0.3
   vf_loss_coeff: 1.0
-  batch_episode:  2
-  batch_mode: "complete_episodes"
-  lr: 0.0005
   entropy_coeff: 0.01
+  vf_clip_param: 10.0
+  batch_mode: "truncate_episodes"
+  kl_threshold: 0.00001
+  accept_ratio: 0.5
+  critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/maddpg.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/maddpg.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
   smooth_target_policy: False
   n_step: 1
   critic_lr: 0.0005
   actor_lr: 0.0005
   buffer_size_episode: 10
   target_network_update_freq_episode: 1
   tau: 0.002
-  batch_mode: "complete_episodes"
+  batch_mode: "truncate_episodes"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/mappo.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/hatrpo.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MAPPO parameters
-
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
+# HATRPO parameters
 
 algo_args:
   use_gae: True
   lambda: 1.0
+  gamma: 0.99
+  batch_episode: 128
   kl_coeff: 0.2
-  batch_episode: 2
-  num_sgd_iter: 2
+  num_sgd_iter: 1
+  grad_clip: 10
+  clip_param: 0.3
   vf_loss_coeff: 1.0
-  lr: 0.0005
   entropy_coeff: 0.01
-  clip_param: 0.3
   vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-
-
+  batch_mode: "truncate_episodes"
+  kl_threshold: 0.00001
+  accept_ratio: 0.5
+  critic_lr: 0.0005
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/matrpo.yaml` & `marllib-1.0.3/marllib/marl/algos/utils/log_dir_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,25 +16,13 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# MATRPO parameters
+import shutil
+import os
 
-algo_args:
-  use_gae: True
-  lambda: 1.0
-  gamma: 0.99
-  batch_episode: 2
-  kl_coeff: 0.2
-  num_sgd_iter: 1
-  grad_clip: 10
-  clip_param: 0.3
-  vf_loss_coeff: 1.0
-  entropy_coeff: 0.01
-  vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-  kl_threshold: 0.00001
-  accept_ratio: 0.5
-  critic_lr: 0.00005
+__total, __used, __free = shutil.disk_usage(".")
+
+available_local_dir = '{}/exp_results'.format(os.getcwd()) if __used / __total <= 0.95 else '/mnt/exp_results'
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/qmix.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/qmix.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/vda2c.yaml` & `marllib-1.0.3/marllib/marl/models/zoo/mixer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDA2C parameters
-
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
-
-algo_args:
-  use_gae: True
-  lambda: 1.0
-  vf_loss_coeff: 1.0
-  batch_episode:  2
-  batch_mode: "complete_episodes"
-  lr: 0.0005
-  entropy_coeff: 0.01
-  mixer: "qmix" # vdn
+from .monotonic_mixer import QMixer
+from .sum_mixer import VDNMixer
```

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/vdn.yaml` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/vdn.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/hyperparams/test/vdppo.yaml` & `marllib-1.0.3/marllib/marl/models/configs/mlp.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# VDPPO parameters
+# mlp parameters
 
-# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/ppo/ippo.py
-
-algo_args:
-  use_gae: True
-  lambda: 1.0
-  kl_coeff: 0.2
-  batch_episode: 2
-  num_sgd_iter: 5
-  vf_loss_coeff: 1.0
-  lr: 0.0005
-  entropy_coeff: 0.01
-  clip_param: 0.3
-  vf_clip_param: 10.0
-  batch_mode: "complete_episodes"
-  mixer: "qmix" # qmix or vdn
+model_arch_args:
+  hidden_state_size: 256
+  core_arch: "mlp"
```

### Comparing `marllib-1.0.2/marllib/marl/algos/run_cc.py` & `marllib-1.0.3/marllib/marl/algos/run_cc.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/run_il.py` & `marllib-1.0.3/marllib/marl/algos/run_vd.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import ray
+from gym.spaces import Dict as GymDict, Discrete, Tuple
+from ray.tune import register_env
 from ray import tune
 from ray.rllib.utils.framework import try_import_tf, try_import_torch
 from marllib.marl.algos.scripts import POlICY_REGISTRY
+from marllib.envs.global_reward_env import COOP_ENV_REGISTRY as ENV_REGISTRY
 from marllib.marl.common import recursive_dict_update, dict_update
 
 tf1, tf, tfv = try_import_tf()
 torch, nn = try_import_torch()
 
 
-def run_il(exp_info, env, model, stop=None):
+def run_vd(exp_info, env, model, stop=None):
     ray.init(local_mode=exp_info["local_mode"])
 
     ########################
     ### environment info ###
     ########################
 
     env_info = env.get_env_info()
@@ -43,70 +46,115 @@
     env_info["agent_name_ls"] = agent_name_ls
     env.close()
 
     ######################
     ### policy sharing ###
     ######################
 
+    # grab the policy mapping info here to use in grouping environment
     policy_mapping_info = env_info["policy_mapping_info"]
 
     if "all_scenario" in policy_mapping_info:
         policy_mapping_info = policy_mapping_info["all_scenario"]
     else:
         policy_mapping_info = policy_mapping_info[map_name]
 
-    if exp_info["share_policy"] == "all":
-        if not policy_mapping_info["all_agents_one_policy"]:
-            raise ValueError("in {}, policy can not be shared".format(map_name))
-
-        policies = {"av"}
-        policy_mapping_fn = (
-            lambda agent_id, episode, **kwargs: "av")
+    if exp_info["algorithm"] in ["qmix", "vdn", "iql"]:
+        space_obs = env_info["space_obs"].spaces
+        space_act = env_info["space_act"]
+        # check the action space condition:
+        if not isinstance(space_act, Discrete):
+            raise ValueError("illegal action space")
+
+        n_agents = env_info["num_agents"]
+
+        if exp_info["share_policy"] == "all":
+            obs_space = Tuple([GymDict(space_obs)] * n_agents)
+            act_space = Tuple([space_act] * n_agents)
+            if not policy_mapping_info["all_agents_one_policy"]:
+                raise ValueError("in {}, policy can not be shared".format(map_name))
+            grouping = {"group_all_": agent_name_ls}
+
+        elif exp_info["share_policy"] == "group":
+            groups = policy_mapping_info["team_prefix"]
+            if len(groups) == 1:
+                obs_space = Tuple([GymDict(space_obs)] * n_agents)
+                act_space = Tuple([space_act] * n_agents)
+                if not policy_mapping_info["all_agents_one_policy"]:
+                    raise ValueError("in {}, policy can not be shared".format(map_name))
+                grouping = {"group_all_": agent_name_ls}
+            else:
+                raise ValueError("joint Q learning does not support group function")
+        elif exp_info["share_policy"] == "individual":
+            raise ValueError("joint Q learning does not support individual function")
+        else:
+            raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
 
-    elif exp_info["share_policy"] == "group":
-        groups = policy_mapping_info["team_prefix"]
+        env_reg_name = "grouped_" + exp_info["env"] + "_" + exp_info["env_args"]["map_name"]
+        register_env(env_reg_name,
+                     lambda _: ENV_REGISTRY[exp_info["env"]](exp_info["env_args"]).with_agent_groups(
+                         grouping, obs_space=obs_space, act_space=act_space))
+    else:
+        env_reg_name = exp_info["env"] + "_" + exp_info["env_args"]["map_name"]
+        register_env(env_reg_name,
+                     lambda _: ENV_REGISTRY[exp_info["env"]](exp_info["env_args"]))
+
+    if exp_info["algorithm"] in ["qmix", "vdn", "iql"]:
+        policies = None
+        policy_mapping_fn = None
 
-        if len(groups) == 1:
+    else:
+        if exp_info["share_policy"] == "all":
             if not policy_mapping_info["all_agents_one_policy"]:
-                raise ValueError(
-                    "in {}, policy can not be shared, change it to 1. group 2. individual".format(map_name))
+                raise ValueError("in {}, policy can not be shared".format(map_name))
+
             policies = {"shared_policy"}
             policy_mapping_fn = (
                 lambda agent_id, episode, **kwargs: "shared_policy")
-        else:
+
+        elif exp_info["share_policy"] == "group":
+            groups = policy_mapping_info["team_prefix"]
+            if len(groups) == 1:
+                if not policy_mapping_info["all_agents_one_policy"]:
+                    raise ValueError(
+                        "in {}, policy can not be shared, change it to 1. group 2. individual".format(map_name))
+                policies = {"shared_policy"}
+                policy_mapping_fn = (
+                    lambda agent_id, episode, **kwargs: "shared_policy")
+            else:
+                policies = {
+                    "policy_{}".format(i): (None, env_info["space_obs"], env_info["space_act"], {}) for i in
+                    groups
+                }
+                policy_ids = list(policies.keys())
+                policy_mapping_fn = tune.function(
+                    lambda agent_id: "policy_{}_".format(agent_id.split("_")[0]))
+
+        elif exp_info["share_policy"] == "individual":
+            if not policy_mapping_info["one_agent_one_policy"]:
+                raise ValueError("in {}, agent number too large, we disable no sharing function".format(map_name))
+
             policies = {
                 "policy_{}".format(i): (None, env_info["space_obs"], env_info["space_act"], {}) for i in
-                groups
+                range(env_info["num_agents"])
             }
             policy_ids = list(policies.keys())
             policy_mapping_fn = tune.function(
-                lambda agent_id: "policy_{}_".format(agent_id.split("_")[0]))
-
-    elif exp_info["share_policy"] == "individual":
-        if not policy_mapping_info["one_agent_one_policy"]:
-            raise ValueError("in {}, agent number too large, we disable no sharing function".format(map_name))
-
-        policies = {
-            "policy_{}".format(i): (None, env_info["space_obs"], env_info["space_act"], {}) for i in
-            range(env_info["num_agents"])
-        }
-        policy_ids = list(policies.keys())
-        policy_mapping_fn = tune.function(
-            lambda agent_id: policy_ids[agent_name_ls.index(agent_id)])
+                lambda agent_id: policy_ids[agent_name_ls.index(agent_id)])
 
-    else:
-        raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
+        else:
+            raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
 
     #########################
     ### experiment config ###
     #########################
 
     run_config = {
         "seed": int(exp_info["seed"]),
-        "env": exp_info["env"] + "_" + exp_info["env_args"]["map_name"],
+        "env": env_reg_name,
         "num_gpus_per_worker": exp_info["num_gpus_per_worker"],
         "num_gpus": exp_info["num_gpus"],
         "num_workers": exp_info["num_workers"],
         "multiagent": {
             "policies": policies,
             "policy_mapping_fn": policy_mapping_fn
         },
@@ -143,12 +191,12 @@
             "training_iteration": 1,
         }
 
         stop_config = recursive_dict_update(stop_config, render_stop_config)
 
     ##################
     ### run script ###
-    ##################
+    ###################
 
     results = POlICY_REGISTRY[exp_info["algorithm"]](model, exp_info, run_config, env_info, stop_config,
                                                      restore_config)
     ray.shutdown()
```

### Comparing `marllib-1.0.2/marllib/marl/algos/run_vd.py` & `marllib-1.0.3/marllib/marl/algos/run_il.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,27 +17,25 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import ray
-from gym.spaces import Dict as GymDict, Discrete, Tuple
-from ray.tune import register_env
 from ray import tune
 from ray.rllib.utils.framework import try_import_tf, try_import_torch
+from ray.rllib.policy.policy import PolicySpec
 from marllib.marl.algos.scripts import POlICY_REGISTRY
-from marllib.envs.global_reward_env import COOP_ENV_REGISTRY as ENV_REGISTRY
 from marllib.marl.common import recursive_dict_update, dict_update
 
 tf1, tf, tfv = try_import_tf()
 torch, nn = try_import_torch()
 
 
-def run_vd(exp_info, env, model, stop=None):
+def run_il(exp_info, env, model, stop=None):
     ray.init(local_mode=exp_info["local_mode"])
 
     ########################
     ### environment info ###
     ########################
 
     env_info = env.get_env_info()
@@ -46,115 +44,112 @@
     env_info["agent_name_ls"] = agent_name_ls
     env.close()
 
     ######################
     ### policy sharing ###
     ######################
 
-    # grab the policy mapping info here to use in grouping environment
     policy_mapping_info = env_info["policy_mapping_info"]
 
     if "all_scenario" in policy_mapping_info:
         policy_mapping_info = policy_mapping_info["all_scenario"]
     else:
         policy_mapping_info = policy_mapping_info[map_name]
 
-    if exp_info["algorithm"] in ["qmix", "vdn", "iql"]:
-        space_obs = env_info["space_obs"].spaces
-        space_act = env_info["space_act"]
-        # check the action space condition:
-        if not isinstance(space_act, Discrete):
-            raise ValueError("illegal action space")
-
-        n_agents = env_info["num_agents"]
-
-        if exp_info["share_policy"] == "all":
-            obs_space = Tuple([GymDict(space_obs)] * n_agents)
-            act_space = Tuple([space_act] * n_agents)
-            if not policy_mapping_info["all_agents_one_policy"]:
-                raise ValueError("in {}, policy can not be shared".format(map_name))
-            grouping = {"group_all_": agent_name_ls}
+    if exp_info["share_policy"] == "all":
+        if not policy_mapping_info["all_agents_one_policy"]:
+            raise ValueError("in {}, policy can not be shared".format(map_name))
+
+        policies = {"shared_policy"}
+        policy_mapping_fn = (
+            lambda agent_id, episode, **kwargs: "shared_policy")
 
-        elif exp_info["share_policy"] == "group":
-            groups = policy_mapping_info["team_prefix"]
-            if len(groups) == 1:
-                obs_space = Tuple([GymDict(space_obs)] * n_agents)
-                act_space = Tuple([space_act] * n_agents)
-                if not policy_mapping_info["all_agents_one_policy"]:
-                    raise ValueError("in {}, policy can not be shared".format(map_name))
-                grouping = {"group_all_": agent_name_ls}
-            else:
-                raise ValueError("joint Q learning does not support group function")
-        elif exp_info["share_policy"] == "individual":
-            raise ValueError("joint Q learning does not support individual function")
-        else:
-            raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
-
-        env_reg_name = "grouped_" + exp_info["env"] + "_" + exp_info["env_args"]["map_name"]
-        register_env(env_reg_name,
-                     lambda _: ENV_REGISTRY[exp_info["env"]](exp_info["env_args"]).with_agent_groups(
-                         grouping, obs_space=obs_space, act_space=act_space))
-    else:
-        env_reg_name = exp_info["env"] + "_" + exp_info["env_args"]["map_name"]
-        register_env(env_reg_name,
-                     lambda _: ENV_REGISTRY[exp_info["env"]](exp_info["env_args"]))
-
-    if exp_info["algorithm"] in ["qmix", "vdn", "iql"]:
-        policies = None
-        policy_mapping_fn = None
+    elif exp_info["share_policy"] == "group":
+        groups = policy_mapping_info["team_prefix"]
 
-    else:
-        if exp_info["share_policy"] == "all":
+        if len(groups) == 1:
             if not policy_mapping_info["all_agents_one_policy"]:
-                raise ValueError("in {}, policy can not be shared".format(map_name))
-
-            policies = {"av"}
+                raise ValueError(
+                    "in {}, policy can not be shared, change it to 1. group 2. individual".format(map_name))
+            policies = {"shared_policy"}
             policy_mapping_fn = (
-                lambda agent_id, episode, **kwargs: "av")
-
-        elif exp_info["share_policy"] == "group":
-            groups = policy_mapping_info["team_prefix"]
-            if len(groups) == 1:
-                if not policy_mapping_info["all_agents_one_policy"]:
-                    raise ValueError(
-                        "in {}, policy can not be shared, change it to 1. group 2. individual".format(map_name))
-                policies = {"shared_policy"}
-                policy_mapping_fn = (
-                    lambda agent_id, episode, **kwargs: "shared_policy")
-            else:
+                lambda agent_id, episode, **kwargs: "shared_policy")
+        else:
+            if "space_obs" in env_info:
+                print("homogeneous action space")
                 policies = {
                     "policy_{}".format(i): (None, env_info["space_obs"], env_info["space_act"], {}) for i in
                     groups
                 }
                 policy_ids = list(policies.keys())
                 policy_mapping_fn = tune.function(
                     lambda agent_id: "policy_{}_".format(agent_id.split("_")[0]))
+            else:
+                print("heterogeneous action space")
+                action_spec_dict = {}
+                obs_spec_dict = {}
+                for key in env_info.keys():
+                    if "space_obs" in key:
+                        g_name = key.split("space_obs")[1]
+                        obs_spec_dict[g_name] = env_info[key]
+                    if "space_act" in key:
+                        g_name = key.split("space_act")[1]
+                        action_spec_dict[g_name] = env_info[key]
+
+                policies = {}
+                for g_name in action_spec_dict.keys():
+                    policies["policy" + g_name + "_"] = PolicySpec(None, obs_spec_dict[g_name], action_spec_dict[g_name], {})
 
-        elif exp_info["share_policy"] == "individual":
-            if not policy_mapping_info["one_agent_one_policy"]:
-                raise ValueError("in {}, agent number too large, we disable no sharing function".format(map_name))
+                policy_mapping_fn = tune.function(
+                    lambda agent_id: "policy_{}_".format(agent_id.split("_")[0]))
 
+    elif exp_info["share_policy"] == "individual":
+        if not policy_mapping_info["one_agent_one_policy"]:
+            raise ValueError("in {}, agent number too large, we disable no sharing function".format(map_name))
+        if "space_obs" in env_info:
+            print("homogeneous action space")
             policies = {
                 "policy_{}".format(i): (None, env_info["space_obs"], env_info["space_act"], {}) for i in
                 range(env_info["num_agents"])
             }
             policy_ids = list(policies.keys())
             policy_mapping_fn = tune.function(
                 lambda agent_id: policy_ids[agent_name_ls.index(agent_id)])
-
         else:
-            raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
+            print("heterogeneous action space")
+            action_spec_dict = {}
+            obs_spec_dict = {}
+            for key in env_info.keys():
+                if "space_obs" in key:
+                    g_name = key.split("space_obs_")[1]
+                    obs_spec_dict[g_name] = env_info[key]
+                if "space_act" in key:
+                    g_name = key.split("space_act_")[1]
+                    action_spec_dict[g_name] = env_info[key]
+
+            policies = {}
+
+            for agent in env_info["agents"]:
+                for g_name in action_spec_dict.keys():
+                    if g_name in agent:
+                        policies[agent] = PolicySpec(None, obs_spec_dict[g_name], action_spec_dict[g_name], {})
+
+            policy_mapping_fn = tune.function(
+                lambda agent_id: agent_id)
+
+    else:
+        raise ValueError("wrong share_policy {}".format(exp_info["share_policy"]))
 
     #########################
     ### experiment config ###
     #########################
 
     run_config = {
         "seed": int(exp_info["seed"]),
-        "env": env_reg_name,
+        "env": exp_info["env"] + "_" + exp_info["env_args"]["map_name"],
         "num_gpus_per_worker": exp_info["num_gpus_per_worker"],
         "num_gpus": exp_info["num_gpus"],
         "num_workers": exp_info["num_workers"],
         "multiagent": {
             "policies": policies,
             "policy_mapping_fn": policy_mapping_fn
         },
@@ -191,12 +186,12 @@
             "training_iteration": 1,
         }
 
         stop_config = recursive_dict_update(stop_config, render_stop_config)
 
     ##################
     ### run script ###
-    ###################
+    ##################
 
     results = POlICY_REGISTRY[exp_info["algorithm"]](model, exp_info, run_config, env_info, stop_config,
                                                      restore_config)
     ray.shutdown()
```

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/__init__.py` & `marllib-1.0.3/marllib/marl/algos/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/coma.py` & `marllib-1.0.3/marllib/marl/algos/scripts/coma.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/facmac.py` & `marllib-1.0.3/marllib/marl/algos/scripts/facmac.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/happo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/happo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/hatrpo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/hatrpo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/ia2c.py` & `marllib-1.0.3/marllib/marl/algos/scripts/ia2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/iddpg.py` & `marllib-1.0.3/marllib/marl/algos/scripts/iddpg.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/ippo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/ippo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/itrpo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/itrpo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/maa2c.py` & `marllib-1.0.3/marllib/marl/algos/scripts/maa2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/maddpg.py` & `marllib-1.0.3/marllib/marl/algos/scripts/maddpg.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/mappo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/mappo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/matrpo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/matrpo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/vda2c.py` & `marllib-1.0.3/marllib/marl/algos/scripts/vda2c.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/vdn_qmix_iql.py` & `marllib-1.0.3/marllib/marl/algos/scripts/vdn_qmix_iql.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/scripts/vdppo.py` & `marllib-1.0.3/marllib/marl/algos/scripts/vdppo.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/__init__.py` & `marllib-1.0.3/marllib/marl/algos/core/VD/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/centralized_Q.py` & `marllib-1.0.3/marllib/marl/algos/utils/centralized_Q.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/centralized_critic.py` & `marllib-1.0.3/marllib/marl/algos/utils/centralized_critic.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/centralized_critic_hetero.py` & `marllib-1.0.3/marllib/marl/algos/utils/centralized_critic_hetero.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/episode_execution_plan.py` & `marllib-1.0.3/marllib/marl/algos/utils/episode_execution_plan.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/episode_replay_buffer.py` & `marllib-1.0.3/marllib/marl/algos/utils/episode_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/heterogeneous_updateing.py` & `marllib-1.0.3/marllib/marl/algos/utils/heterogeneous_updateing.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/log_dir_util.py` & `marllib-1.0.3/marllib/marl/algos/core/IL/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,13 +16,7 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import shutil
-import os
-
-__total, __used, __free = shutil.disk_usage(".")
-
-available_local_dir = '{}/exp_results'.format(os.getcwd()) if __used / __total <= 0.95 else '/mnt/exp_results'
```

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/manipulate_tensor.py` & `marllib-1.0.3/marllib/marl/algos/utils/manipulate_tensor.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/mixing_Q.py` & `marllib-1.0.3/marllib/marl/algos/utils/mixing_Q.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/mixing_critic.py` & `marllib-1.0.3/marllib/marl/algos/utils/mixing_critic.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/popart.py` & `marllib-1.0.3/marllib/marl/algos/utils/popart.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/setup_utils.py` & `marllib-1.0.3/marllib/marl/algos/utils/setup_utils.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/trust_regions.py` & `marllib-1.0.3/marllib/marl/algos/utils/trust_regions.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/algos/utils/valuenorm.py` & `marllib-1.0.3/marllib/marl/algos/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/common.py` & `marllib-1.0.3/marllib/marl/common.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/__init__.py` & `marllib-1.0.3/marllib/marl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/configs/__init__.py` & `marllib-1.0.3/marllib/marl/algos/core/CC/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/configs/cnn_encoder.yaml` & `marllib-1.0.3/marllib/marl/models/configs/cnn_encoder.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/configs/fc_encoder.yaml` & `marllib-1.0.3/marllib/marl/models/configs/fc_encoder.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/configs/mixer.yaml` & `marllib-1.0.3/marllib/marl/models/configs/rnn.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -19,10 +19,9 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # rnn parameters
 
 model_arch_args:
-  mixer_embedding: 256
-  mixer_arch: "qmix" # qmix or vdn
-
+  hidden_state_size: 256
+  core_arch: "gru" # gru or lstm
```

### Comparing `marllib-1.0.2/marllib/marl/models/configs/mlp.yaml` & `marllib-1.0.3/marllib/marl/ray/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,12 +16,7 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# mlp parameters
-
-model_arch_args:
-  hidden_state_size: 256
-  core_arch: "mlp"
```

### Comparing `marllib-1.0.2/marllib/marl/models/configs/rnn.yaml` & `marllib-1.0.3/marllib/marl/models/zoo/encoder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,12 +16,7 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# rnn parameters
-
-model_arch_args:
-  hidden_state_size: 256
-  core_arch: "gru" # gru or lstm
```

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/__init__.py` & `marllib-1.0.3/marllib/marl/models/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/encoder/__init__.py` & `marllib-1.0.3/marllib/marl/models/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/encoder/base_encoder.py` & `marllib-1.0.3/marllib/marl/models/zoo/encoder/base_encoder.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/encoder/cc_encoder.py` & `marllib-1.0.3/marllib/marl/models/zoo/encoder/cc_encoder.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mixer/__init__.py` & `marllib-1.0.3/marllib/envs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,9 +16,7 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .monotonic_mixer import QMixer
-from .sum_mixer import VDNMixer
```

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mixer/monotonic_mixer.py` & `marllib-1.0.3/marllib/marl/models/zoo/mixer/monotonic_mixer.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mixer/sum_mixer.py` & `marllib-1.0.3/marllib/marl/models/zoo/mixer/sum_mixer.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/__init__.py` & `marllib-1.0.3/marllib/marl/models/zoo/mlp/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/base_mlp.py` & `marllib-1.0.3/marllib/marl/models/zoo/mlp/base_mlp.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/cc_mlp.py` & `marllib-1.0.3/marllib/marl/models/zoo/mlp/cc_mlp.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/ddpg_mlp.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/ddpg_rnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,33 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import numpy as np
 from typing import Dict, List
 from ray.rllib.models.modelv2 import ModelV2
-from ray.rllib.models.torch.torch_modelv2 import TorchModelV2
+from ray.rllib.models.torch.recurrent_net import RecurrentNetwork as TorchRNN
 from ray.rllib.utils.annotations import override
 from ray.rllib.utils.framework import try_import_tf, try_import_torch, \
     TensorType
-from ray.rllib.models.torch.misc import SlimFC, SlimConv2d, normc_initializer
+from ray.rllib.policy.rnn_sequencing import add_time_dimension
+from ray.rllib.models.torch.misc import SlimFC, normc_initializer
 from marllib.marl.models.zoo.mixer import QMixer, VDNMixer
+from marllib.marl.models.zoo.encoder.base_encoder import BaseEncoder
 
 tf1, tf, tfv = try_import_tf()
 torch, nn = try_import_torch()
 
 
-class DDPGSeriesMLP(TorchModelV2, nn.Module):
+class DDPGSeriesRNN(TorchRNN, nn.Module):
     """
-    DDOG/MADDPG/FACMAC agent arch in one model
+    IDDPG/MADDPG/FACMAC agent rnn arch in one model
     """
 
     def __init__(
             self,
             obs_space,
             action_space,
             num_outputs,
@@ -47,96 +50,58 @@
             name,
             **kwargs,
     ):
         nn.Module.__init__(self)
         super().__init__(obs_space, action_space, num_outputs, model_config,
                          name)
 
-        # judge the model arch
         self.custom_config = model_config["custom_model_config"]
         self.full_obs_space = getattr(obs_space, "original_space", obs_space)
         self.n_agents = self.custom_config["num_agents"]
         self.activation = model_config.get("fcnet_activation")
 
-        if self.custom_config["model_arch_args"]["core_arch"] != "mlp":
-            raise ValueError()
         # encoder
-        layers = []
-        if "fc_layer" in self.custom_config["model_arch_args"]:
-            if "encode_layer" in self.custom_config["model_arch_args"]:
-                encode_layer = self.custom_config["model_arch_args"]["encode_layer"]
-                encoder_layer_dim = encode_layer.split("-")
-                encoder_layer_dim = [int(i) for i in encoder_layer_dim]
-            else:  # default config
-                encoder_layer_dim = []
-                for i in range(self.custom_config["model_arch_args"]["fc_layer"]):
-                    out_dim = self.custom_config["model_arch_args"]["out_dim_fc_{}".format(i)]
-                    encoder_layer_dim.append(out_dim)
-
-            self.encoder_layer_dim = encoder_layer_dim
-            self.obs_size = self.full_obs_space["obs"].shape[0]
-            input_dim = self.obs_size
-            for out_dim in self.encoder_layer_dim:
-                layers.append(
-                    SlimFC(in_size=input_dim,
-                           out_size=out_dim,
-                           initializer=normc_initializer(1.0),
-                           activation_fn=self.activation))
-                input_dim = out_dim
-        elif "conv_layer" in self.custom_config["model_arch_args"]:
-            self.obs_size = self.full_obs_space['obs'].shape
-            input_dim = self.obs_size[2]
-            for i in range(self.custom_config["model_arch_args"]["conv_layer"]):
-                layers.append(
-                    SlimConv2d(
-                        in_channels=input_dim,
-                        out_channels=self.custom_config["model_arch_args"]["out_channel_layer_{}".format(i)],
-                        kernel=self.custom_config["model_arch_args"]["kernel_size_layer_{}".format(i)],
-                        stride=self.custom_config["model_arch_args"]["stride_layer_{}".format(i)],
-                        padding=self.custom_config["model_arch_args"]["padding_layer_{}".format(i)],
-                        activation_fn=self.activation
-                    )
-                )
-                pool_f = nn.MaxPool2d(
-                    kernel_size=self.custom_config["model_arch_args"]["pool_size_layer_{}".format(i)])
-                layers.append(pool_f)
-
-                input_dim = self.custom_config["model_arch_args"]["out_channel_layer_{}".format(i)]
-
-        else:
-            raise ValueError()
-
-        self.encoder = nn.Sequential(
-            *layers
-        )
+        self.encoder = BaseEncoder(model_config, self.full_obs_space)
 
         if self.custom_config["algorithm"] in ["maddpg"]:
             all_action_dim = self.custom_config["space_act"].shape[0] * self.custom_config["num_agents"]
             if self.custom_config["global_state_flag"]:
                 self.state_encoder = nn.Linear(self.full_obs_space["state"].shape[0],
-                                               input_dim)
+                                               self.encoder.output_dim)
             if "q" in name:
                 if self.custom_config["global_state_flag"]:
-                    input_dim = input_dim * 2 + all_action_dim
+                    input_dim = self.encoder.output_dim * 2 + all_action_dim
                 else:
-                    input_dim = input_dim * self.custom_config["num_agents"] + all_action_dim
+                    input_dim = self.encoder.output_dim * self.custom_config["num_agents"] + all_action_dim
+            else:
+                input_dim = self.encoder.output_dim
 
-        else:  # no centralized critic -> iddpg
+        else:  # no centralized critic -> iddpg, facmac
             if "q" in name:
-                input_dim = input_dim + self.custom_config["space_act"].shape[0]
+                input_dim = self.encoder.output_dim + self.custom_config["space_act"].shape[0]
+            else:
+                input_dim = self.encoder.output_dim
 
         # core rnn
         self.hidden_state_size = self.custom_config["model_arch_args"]["hidden_state_size"]
         self.input_dim = input_dim
 
-        self.mlp = nn.Linear(input_dim, self.hidden_state_size)
+        if self.custom_config["model_arch_args"]["core_arch"] == "gru":
+            self.rnn = nn.GRU(self.input_dim, self.hidden_state_size, batch_first=True)
+        elif self.custom_config["model_arch_args"]["core_arch"] == "lstm":
+            self.rnn = nn.LSTM(self.input_dim, self.hidden_state_size, batch_first=True)
+        else:
+            raise ValueError()
 
         # action branch and value branch
-        self.action_branch = nn.Linear(self.hidden_state_size, num_outputs)
-        self.value_branch = nn.Linear(self.hidden_state_size, 1)
+        self.out_branch = SlimFC(
+            in_size=self.hidden_state_size,
+            out_size=num_outputs,
+            initializer=normc_initializer(0.01),
+            activation_fn=None)
 
         if self.custom_config["algorithm"] in ["facmac"]:
             # mixer:
             if self.custom_config["global_state_flag"]:
                 state_dim = self.custom_config["space_obs"]["state"].shape
             else:
                 state_dim = self.custom_config["space_obs"]["obs"].shape + (self.custom_config["num_agents"],)
@@ -152,90 +117,141 @@
 
         # record the custom config
         self.n_agents = self.custom_config["num_agents"]
         self.q_flag = False
 
     @override(ModelV2)
     def get_initial_state(self):
-        # Place hidden states on same device as model.
-        return self.value_branch.weight.new(1, self.hidden_state_size).zero_().squeeze(0),
+        if self.custom_config["model_arch_args"]["core_arch"] == "gru":
+            hidden_state = [
+                self.out_branch._model._modules["0"].weight.new(1, self.hidden_state_size).zero_().squeeze(0),
+            ]
+        else:  # lstm
+            hidden_state = [
+                self.out_branch._model._modules["0"].weight.new(1, self.hidden_state_size).zero_().squeeze(0),
+                self.out_branch._model._modules["0"].weight.new(1, self.hidden_state_size).zero_().squeeze(0)
+            ]
+        return hidden_state
 
     @override(ModelV2)
     def forward(self, input_dict: Dict[str, TensorType],
                 state: List[TensorType],
                 seq_lens: TensorType) -> (TensorType, List[TensorType]):
         """
         Adds time dimension to batch before sending inputs to forward_rnn()
         """
 
         obs_inputs = input_dict["obs"]["obs"].float()
+        if isinstance(seq_lens, np.ndarray):
+            seq_lens = torch.Tensor(seq_lens).int()
+        max_seq_len = obs_inputs.shape[0] // seq_lens.shape[0]
+
+        self.time_major = self.model_config.get("_time_major", False)
+
+        obs_inputs = add_time_dimension(
+            obs_inputs,
+            max_seq_len=max_seq_len,
+            framework="torch",
+            time_major=self.time_major,
+        )
 
         if "state" in input_dict:
             state_inputs = input_dict["state"].float()
+            state_inputs = add_time_dimension(
+                state_inputs,
+                max_seq_len=max_seq_len,
+                framework="torch",
+                time_major=self.time_major,
+            )
         else:
             state_inputs = None
 
         if "opponent_actions" in input_dict:
             opp_action_inputs = input_dict["opponent_actions"].float()
+            opp_action_inputs = add_time_dimension(
+                opp_action_inputs,
+                max_seq_len=max_seq_len,
+                framework="torch",
+                time_major=self.time_major,
+            )
         else:
             opp_action_inputs = None
 
         if "actions" in input_dict:
             action_inputs = input_dict["actions"].float()
+            action_inputs = add_time_dimension(
+                action_inputs,
+                max_seq_len=max_seq_len,
+                framework="torch",
+                time_major=self.time_major,
+            )
         else:
             action_inputs = None
 
-        output, new_state = self.forward_mlp(obs_inputs, action_inputs, state_inputs, opp_action_inputs, state,
+        output, new_state = self.forward_rnn(obs_inputs, action_inputs, state_inputs, opp_action_inputs, state,
                                              seq_lens)
         output = torch.reshape(output, [-1, self.num_outputs])
 
         return output, new_state
 
-    def forward_mlp(self, obs_inputs, action_inputs, state_inputs, opp_action_inputs, state, seq_lens):
+    @override(TorchRNN)
+    def forward_rnn(self, obs_inputs, action_inputs, state_inputs, opp_action_inputs, hidden_state, seq_lens):
         # Extract the available actions tensor from the observation.
         # Compute the unmasked logits.
         if self.custom_config["algorithm"] in ["maddpg"]:
-            # CNN not support in MADDPG
+            # currently we do not support CNN in MADDPG
             if action_inputs is not None:
                 B = obs_inputs.shape[0]
+                L = obs_inputs.shape[1]
                 obs_x = self.encoder(obs_inputs)
                 if self.custom_config["global_state_flag"]:
                     state_x = self.state_encoder(state_inputs)
-                    x = torch.cat((obs_x, state_x, action_inputs, opp_action_inputs.reshape(B, -1)), -1)
+                    x = torch.cat((obs_x, state_x, action_inputs, opp_action_inputs.reshape(B, L, -1)), -1)
                 else:
                     state_x_ls = []
                     for i in range(self.n_agents):
-                        state_x = self.encoder(state_inputs[:, i])
+                        state_x = self.encoder(state_inputs[:, :, i])
                         state_x_ls.append(state_x)
                     state_x = torch.cat(state_x_ls, -1)
-                    x = torch.cat((state_x, action_inputs, opp_action_inputs.reshape(B, -1)), -1)
+                    x = torch.cat((state_x, action_inputs, opp_action_inputs.reshape(B, L, -1)), -1)
 
             else:
                 x = self.encoder(obs_inputs)
 
         else:
             if "conv_layer" in self.custom_config["model_arch_args"]:
                 x = obs_inputs.reshape(-1, obs_inputs.shape[2], obs_inputs.shape[3], obs_inputs.shape[4]).permute(0, 3,
+                                                                                                                  1,
                                                                                                                   2)
                 x = self.encoder(x)
                 x = torch.mean(x, (2, 3))
                 x = x.reshape(obs_inputs.shape[0], obs_inputs.shape[1], -1)
             else:
                 x = self.encoder(obs_inputs)
 
             if action_inputs is not None:
                 x = torch.cat((x, action_inputs), -1)
 
         x = nn.functional.relu(x)
 
-        self._features = self.mlp(x)
-        logits = self.action_branch(self._features)
+        if self.custom_config["model_arch_args"]["core_arch"] == "gru":
+            self._features, h = self.rnn(x, torch.unsqueeze(hidden_state[0], 0))
+            logits = self.out_branch(self._features)
+            return logits, [torch.squeeze(h, 0)]
+
+        elif self.custom_config["model_arch_args"]["core_arch"] == "lstm":
+            self._features, [h, c] = self.rnn(
+                x, [torch.unsqueeze(hidden_state[0], 0),
+                    torch.unsqueeze(hidden_state[1], 0)])
+            logits = self.out_branch(self._features)
+            return logits, [torch.squeeze(h, 0), torch.squeeze(c, 0)]
 
-        return logits, state
+        else:
+            raise ValueError("rnn core_arch wrong: {}".format(self.custom_config["model_arch_args"]["core_arch"]))
 
     def mixing_value(self, all_agents_q, state):
         # compatiable with rllib qmix mixer
         all_agents_q = all_agents_q.view(-1, 1, self.n_agents)
         q_tot = self.mixer(all_agents_q, state)
 
         # shape to [B]
-        return q_tot.flatten(start_dim=0)
+        return q_tot.flatten(start_dim=0)
```

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/jointQ_mlp.py` & `marllib-1.0.3/marllib/marl/models/zoo/mlp/jointQ_mlp.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/mlp/vd_mlp.py` & `marllib-1.0.3/marllib/marl/models/zoo/mlp/vd_mlp.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/rnn/__init__.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/rnn/base_rnn.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/base_rnn.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/rnn/cc_rnn.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/cc_rnn.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/rnn/jointQ_rnn.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/jointQ_rnn.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/models/zoo/rnn/vd_rnn.py` & `marllib-1.0.3/marllib/marl/models/zoo/rnn/vd_rnn.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/ray/__init__.py` & `marllib-1.0.3/marllib/envs/base_env/config/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/marl/ray/ray.yaml` & `marllib-1.0.3/marllib/marl/ray/ray.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ray/rllib config
 
 local_mode: False # True for debug mode only
 share_policy: "group" #  individual(separate) / group(division) / all(share)
-evaluation_interval: 1000 # evaluate model every 10 training iterations
+evaluation_interval: 50 # evaluate model every 10 training iterations
 framework: "torch"
 num_workers: 1 # thread number
 num_gpus: 1 # gpu to use
 num_cpus_per_worker: 1 # cpu allocate to each worker
 num_gpus_per_worker: 0 # gpu allocate to each worker
 checkpoint_freq: 100 # save model every 100 training iterations
 checkpoint_end: True # save model at the end of the exp
```

### Comparing `marllib-1.0.2/marllib/marl/ray/ray_beta.yaml` & `marllib-1.0.3/marllib/marl/ray/ray_beta.yaml`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/__init__.py` & `marllib-1.0.3/marllib/envs/base_env/install/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/add_patch.py` & `marllib-1.0.3/marllib/patch/add_patch.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/hanabi/Hanabi_Env.py` & `marllib-1.0.3/marllib/patch/hanabi/Hanabi_Env.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/hanabi/__init__.py` & `marllib-1.0.3/marllib/patch/hanabi/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/hanabi/pyhanabi.py` & `marllib-1.0.3/marllib/patch/hanabi/pyhanabi.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/pommerman_patch/__init__.py` & `marllib-1.0.3/marllib/patch/pommerman_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/pommerman_patch/forward_model.py` & `marllib-1.0.3/marllib/patch/pommerman_patch/forward_model.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/pommerman_patch/graphics.py` & `marllib-1.0.3/marllib/patch/pommerman_patch/graphics.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/pommerman_patch/v0.py` & `marllib-1.0.3/marllib/patch/pommerman_patch/v0.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/__init__.py` & `marllib-1.0.3/multiagent_mujoco/assets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,7 +16,50 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# MIT License
+
+# Copyright (c) 2023 Replicable-MARL
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# MIT License
+
+# Copyright (c) 2023 Replicable-MARL
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
```

### Comparing `marllib-1.0.2/marllib/patch/rllib/execution/__init__.py` & `marllib-1.0.3/multiagent_mujoco/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,7 +16,54 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# MIT License
+
+# Copyright (c) 2023 Replicable-MARL
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# MIT License
+
+# Copyright (c) 2023 Replicable-MARL
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+from .mujoco_multi import MujocoMulti
+from .coupled_half_cheetah import CoupledHalfCheetah
+from .manyagent_swimmer import ManyAgentSwimmerEnv
+from .manyagent_ant import ManyAgentAntEnv
```

### Comparing `marllib-1.0.2/marllib/patch/rllib/execution/replay_buffer.py` & `marllib-1.0.3/marllib/patch/rllib/execution/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/execution/train_ops.py` & `marllib-1.0.3/marllib/patch/rllib/execution/train_ops.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/execution/train_ops_new_sgd_batch.py` & `marllib-1.0.3/marllib/patch/rllib/execution/train_ops_new_sgd_batch.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/models/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/finetuned/mpe/vda2c.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -16,7 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# VDA2C parameters
+
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+
+algo_args:
+  use_gae: True
+  lambda: 1.0
+  vf_loss_coeff: 1.0
+  batch_episode:  128
+  batch_mode: "truncate_episodes"
+  lr: 0.0005
+  entropy_coeff: 0.01
+  mixer: "qmix" # vdn
```

### Comparing `marllib-1.0.2/marllib/patch/rllib/models/preprocessors.py` & `marllib-1.0.3/marllib/patch/rllib/models/preprocessors.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/policy/__init__.py` & `marllib-1.0.3/marllib/marl/algos/hyperparams/test/ia2c.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -16,7 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# A2C parameters
+
+# Detailed explanation for each hyper parameter can be found in ray/rllib/agents/a3c/ia2c.py
+
+algo_args:
+  use_gae: True
+  lambda: 1.0
+  vf_loss_coeff: 1.0
+  batch_episode:  2
+  batch_mode: "truncate_episodes"
+  lr: 0.0005
+  entropy_coeff: 0.01
```

### Comparing `marllib-1.0.2/marllib/patch/rllib/policy/rnn_sequencing.py` & `marllib-1.0.3/marllib/patch/rllib/policy/rnn_sequencing.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib/patch/rllib/policy/torch_policy.py` & `marllib-1.0.3/marllib/patch/rllib/policy/torch_policy.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/marllib.egg-info/PKG-INFO` & `marllib-1.0.3/marllib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,378 @@
 Metadata-Version: 2.1
 Name: marllib
-Version: 1.0.2
+Version: 1.0.3
+Summary: UNKNOWN
+Home-page: UNKNOWN
 License: MIT
+Description: [comment]: <> (<div align="center">)
+        
+        [comment]: <> (<img src=docs/source/images/logo1.png width=65% />)
+        
+        [comment]: <> (</div>)
+        
+        <h1 align="center"> MARLlib: A Scalable and Efficient Multi-agent Reinforcement Learning Library </h1>
+        
+        [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]()
+        ![test](https://github.com/Replicable-MARL/MARLlib/workflows/test/badge.svg)
+        [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/)
+        [![GitHub issues](https://img.shields.io/github/issues/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib/issues)
+        [![PyPI version](https://badge.fury.io/py/marllib.svg)](https://badge.fury.io/py/marllib)
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
+        [![Organization](https://img.shields.io/badge/Organization-ReLER_RL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
+        [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/Replicable-MARL/MARLlib)
+        [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
+        
+        > __News__:
+        > We are excited to announce that a major update has just been released. For detailed version information, please refer to the [version info](https://github.com/Replicable-MARL/MARLlib/releases/tag/1.0.2).
+        
+        
+        **Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** that utilizes [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It offers a comprehensive platform for developing, training, and testing MARL algorithms across various tasks and environments. 
+        
+        Here's an example of how MARLlib can be used:
+        
+        ```py
+        from marllib import marl
+        
+        # prepare env
+        env = marl.make_env(environment_name="mpe", map_name="simple_spread")
+        
+        # initialize algorithm with appointed hyper-parameters
+        mappo = marl.algos.mappo(hyperparam_source='mpe')
+        
+        # build agent model based on env + algorithms + user preference
+        model = marl.build_model(env, mappo, {"core_arch": "gru", "encode_layer": "128-256"})
+        
+        # start training
+        mappo.fit(env, model, stop={'timesteps_total': 1000000}, share_policy='group')
+        
+        # ready to control
+        mappo.render(env, model, share_policy='group', restore_path='path_to_checkpoint')
+        ```
+        
+        
+        
+        ## Why MARLlib?
+        
+        Here we provide a table for the comparison of MARLlib and existing work.
+        
+        |   Library   |  Supported Env | Algorithm | Parameter Sharing  | Model 
+        |:-------------:|:-------------:|:-------------:|:--------------:|:----------------:|
+        |     [PyMARL](https://github.com/oxwhirl/pymarl) |        1 cooperative       |       5       |         share        |      GRU           | :x:
+        |   [PyMARL2](https://github.com/hijkzzz/pymarl2)|        2 cooperative       |     11   |         share        |  MLP + GRU  | :x:
+        | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy) |       4 cooperative       |      1     |          share + separate        |          MLP + GRU        |         :x:              |
+        | [MAlib](https://github.com/sjtu-marl/malib) |  4 self-play  | 10 | share + group + separate | MLP + LSTM | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest)
+        |    [EPyMARL](https://github.com/uoe-agents/epymarl)|        4 cooperative      |    9    |        share + separate       |      GRU             |           :x:            |
+        |    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       12 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
+        
+        |   Library   | Github Stars  | Documentation | Issues Open | Activity | Last Update
+        |:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
+        |     [PyMARL](https://github.com/oxwhirl/pymarl) | [![GitHub stars](https://img.shields.io/github/stars/oxwhirl/pymarl)](https://github.com/oxwhirl/pymarl)    |       :x: | ![GitHub opened issue](https://img.shields.io/github/issues/oxwhirl/pymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/oxwhirl/pymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/oxwhirl/pymarl?label=last%20update)  
+        |   [PyMARL2](https://github.com/hijkzzz/pymarl2)| [![GitHub stars](https://img.shields.io/github/stars/hijkzzz/pymarl2)](https://github.com/hijkzzz/pymarl2)       |       :x:  | ![GitHub opened issue](https://img.shields.io/github/issues/hijkzzz/pymarl2.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/hijkzzz/pymarl2?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/hijkzzz/pymarl2?label=last%20update)  
+        | [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy)| [![GitHub stars](https://img.shields.io/github/stars/marlbenchmark/on-policy)](https://github.com/marlbenchmark/on-policy)   |        :x:              | ![GitHub opened issue](https://img.shields.io/github/issues/marlbenchmark/on-policy.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/marlbenchmark/on-policy?label=commit)| ![GitHub last commit](https://img.shields.io/github/last-commit/marlbenchmark/on-policy?label=last%20update)  
+        | [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
+        |    [EPyMARL](https://github.com/uoe-agents/epymarl)| [![GitHub stars](https://img.shields.io/github/stars/uoe-agents/epymarl)](https://github.com/uoe-agents/epymarl)        |           :x:            | ![GitHub opened issue](https://img.shields.io/github/issues/uoe-agents/epymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/uoe-agents/epymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/uoe-agents/epymarl?label=last%20update)  
+        |    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |  [![GitHub stars](https://img.shields.io/github/stars/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib)  |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) | ![GitHub opened issue](https://img.shields.io/github/issues/Replicable-MARL/MARLlib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/m/Replicable-MARL/MARLlib/sy_dev?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/Replicable-MARL/MARLlib/sy_dev?label=last%20update)  
+        
+        
+        
+        [comment]: <> (<div align="center">)
+        
+        [comment]: <> (<img src=docs/source/images/overview.png width=100% />)
+        
+        [comment]: <> (</div>)
+        
+        ## key features
+        
+        :beginner: MARLlib offers several key features that make it stand out:
+        
+        - MARLlib unifies diverse algorithm pipelines with agent-level distributed dataflow, allowing researchers to develop, test, and evaluate MARL algorithms across different tasks and environments.
+        - MARLlib supports all task modes, including cooperative, collaborative, competitive, and mixed. This makes it easier for researchers to train and evaluate MARL algorithms across a wide range of tasks.
+        - MARLlib provides a new interface that follows the structure of Gym, making it easier for researchers to work with multi-agent environments.
+        - MARLlib provides flexible and customizable parameter-sharing strategies, allowing researchers to optimize their algorithms for different tasks and environments.
+        
+        :rocket: Using MARLlib, you can take advantage of various benefits, such as:
+        
+        - **Zero knowledge of MARL**: MARLlib provides 18 pre-built algorithms with an intuitive API, allowing researchers to start experimenting with MARL without prior knowledge of the field.
+        - **Support for all task modes**: MARLlib supports almost all multi-agent environments, making it easier for researchers to experiment with different task modes.
+        - **Customizable model architecture**: Researchers can choose their preferred model architecture from the model zoo, or build their own.
+        - **Customizable policy sharing**: MARLlib provides grouping options for policy sharing, or researchers can create their own.
+        - **Access to over a thousand released experiments**: Researchers can access over a thousand released experiments to see how other researchers have used MARLlib.
+        
+        ## Installation
+        
+        > __Note__:
+        > Currently MARLlib supports Linux only.
+        
+        ### Step-by-step  (recommended)
+        
+        - install dependencies
+        - install environments
+        - install patches
+        
+        #### 1. install dependencies (basic)
+        
+        First, install MARLlib dependencies to guarantee basic usage.
+        following [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html), finally install patches for RLlib.
+        
+        ```bash
+        $ conda create -n marllib python=3.8 # or 3.9
+        $ conda activate marllib
+        $ git clone https://github.com/Replicable-MARL/MARLlib.git && cd MARLlib
+        $ pip install -r requirements.txt
+        ```
+        
+        #### 2. install environments (optional)
+        
+        Please follow [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html).
+        
+        #### 3. install patches (basic)
+        
+        Fix bugs of RLlib using patches by running the following command:
+        
+        ```bash
+        $ cd /Path/To/MARLlib/marl/patch
+        $ python add_patch.py -y
+        ```
+        
+        ### PyPI
+        
+        ```bash
+        $ pip install --upgrade pip
+        $ pip install marllib
+        ```
+        
+        ## Getting started
+        
+        <details>
+        <summary><b><big>Prepare the configuration</big></b></summary>
+        
+        There are four parts of configurations that take charge of the whole training process.
+        
+        - scenario: specify the environment/task settings
+        - algorithm: choose the hyperparameters of the algorithm
+        - model: customize the model architecture
+        - ray/rllib: change the basic training settings
+        
+        <div align="center">
+        <img src=docs/source/images/configurations.png width=100% />
+        </div>
+        
+        Before training, ensure all the parameters are set correctly, especially those you don't want to change.
+        > __Note__:
+        > You can also modify all the pre-set parameters via MARLLib API.*
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Register the environment</big></b></summary>
+        
+        Ensure all the dependencies are installed for the environment you are running with. Otherwise, please refer to
+        [MARLlib documentation](https://marllib.readthedocs.io/en/latest/handbook/env.html).
+        
+        
+        |   task mode   | api example |
+        | :-----------: | ----------- |
+        | cooperative | ```marl.make_env(environment_name="mpe", map_name="simple_spread", force_coop=True)``` |
+        | collaborative | ```marl.make_env(environment_name="mpe", map_name="simple_spread")``` |
+        | competitive | ```marl.make_env(environment_name="mpe", map_name="simple_adversary")``` |
+        | mixed | ```marl.make_env(environment_name="mpe", map_name="simple_crypto")``` |
+        
+        Most of the popular environments in MARL research are supported by MARLlib:
+        
+        | Env Name | Learning Mode | Observability | Action Space | Observations |
+        | :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
+        | **[LBF](https://github.com/semitable/lb-foraging)**  | cooperative + collaborative | Both | Discrete | 1D  |
+        | **[RWARE](https://github.com/semitable/robotic-warehouse)**  | cooperative | Partial | Discrete | 1D  |
+        | **[MPE](https://github.com/openai/multiagent-particle-envs)**  | cooperative + collaborative + mixed | Both | Both | 1D  |
+        | **[SMAC](https://github.com/oxwhirl/smac)**  | cooperative | Partial | Discrete | 1D |
+        | **[MetaDrive](https://github.com/decisionforce/metadrive)**  | collaborative | Partial | Continuous | 1D |
+        | **[MAgent](https://www.pettingzoo.ml/magent)** | collaborative + mixed | Partial | Discrete | 2D |
+        | **[Pommerman](https://github.com/MultiAgentLearning/playground)**  | collaborative + competitive + mixed | Both | Discrete | 2D |
+        | **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Full | Continuous | 1D |
+        | **[GRF](https://github.com/google-research/football)**  | collaborative + mixed | Full | Discrete | 2D |
+        | **[Hanabi](https://github.com/deepmind/hanabi-learning-environment)** | cooperative | Partial | Discrete | 1D |
+        | **[MATE](https://github.com/XuehaiPan/mate)** | cooperative + mixed | Partial | Both | 1D |
+        | **[GoBigger](https://github.com/opendilab/GoBigger)** | cooperative + mixed | Both | Continuous | 1D |
+        
+        Each environment has a readme file, standing as the instruction for this task, including env settings, installation, and
+        important notes.
+        </details>
+        
+        <details>
+        <summary><b><big>Initialize the algorithm</big></b></summary>
+        
+        
+        |  running target   | api example |
+        | :-----------: | ----------- |
+        | train & finetune  | ```marl.algos.mappo(hyperparam_source=$ENV)``` |
+        | develop & debug | ```marl.algos.mappo(hyperparam_source="test")``` |
+        | 3rd party env | ```marl.algos.mappo(hyperparam_source="common")``` |
+        
+        Here is a chart describing the characteristics of each algorithm:
+        
+        | algorithm                                                    | support task mode | discrete action   | continuous action |  policy type        |
+        | :------------------------------------------------------------: | :-----------------: | :----------: | :--------------------: | :----------: | 
+        | *IQL**                                                         | all four               | :heavy_check_mark:   |    |  off-policy |
+        | *[PG](https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf)* | all four                  | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[A2C](https://arxiv.org/abs/1602.01783)*                      | all four              | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[DDPG](https://arxiv.org/abs/1509.02971)*                     | all four             |  | :heavy_check_mark:   |  off-policy |
+        | *[TRPO](http://proceedings.mlr.press/v37/schulman15.pdf)*      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[PPO](https://arxiv.org/abs/1707.06347)*                      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[COMA](https://ojs.aaai.org/index.php/AAAI/article/download/11794/11653)* | all four                           | :heavy_check_mark:       |   |  on-policy  |
+        | *[MADDPG](https://arxiv.org/abs/1706.02275)*                   | all four                     |  | :heavy_check_mark:   |  off-policy |
+        | *MAA2C**                                                       | all four                        | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *MATRPO**                                                      | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[MAPPO](https://arxiv.org/abs/2103.01955)*                    | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[HATRPO](https://arxiv.org/abs/2109.11251)*                   | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[HAPPO](https://arxiv.org/abs/2109.11251)*                    | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *[VDN](https://arxiv.org/abs/1706.05296)*                      | cooperative         | :heavy_check_mark:   |    |  off-policy |
+        | *[QMIX](https://arxiv.org/abs/1803.11485)*                     | cooperative                    | :heavy_check_mark:   |   |  off-policy |
+        | *[FACMAC](https://arxiv.org/abs/2003.06709)*                   | cooperative                    |  | :heavy_check_mark:   |  off-policy |
+        | *[VDAC](https://arxiv.org/abs/2007.12306)*                    | cooperative                    | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        | *VDPPO**                                                      | cooperative                | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
+        
+        ***all four**: cooperative collaborative competitive mixed
+        
+        *IQL* is the multi-agent version of Q learning.
+        *MAA2C* and *MATRPO* are the centralized version of A2C and TRPO.
+        *VDPPO* is the value decomposition version of PPO.
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Build the agent model</big></b></summary>
+        
+        An agent model consists of two parts, `encoder` and `core arch`. 
+        `encoder` will be constructed by MARLlib according to the observation space.
+        Choose `mlp`, `gru`, or `lstm` as you like to build the complete model.
+        
+        |  model arch   | api example |
+        | :-----------: | ----------- |
+        | MLP  | ```marl.build_model(env, algo, {"core_arch": "mlp")``` |
+        | GRU | ```marl.build_model(env, algo, {"core_arch": "gru"})```  |
+        | LSTM | ```marl.build_model(env, algo, {"core_arch": "lstm"})```  |
+        | Encoder Arch | ```marl.build_model(env, algo, {"core_arch": "gru", "encode_layer": "128-256"})```  |
+        
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Kick off the training</big></b></summary>
+        
+        |  setting   | api example |
+        | :-----------: | ----------- |
+        | train  | ```algo.fit(env, model)``` |
+        | debug  | ```algo.fit(env, model, local_mode=True)``` |
+        | stop condition | ```algo.fit(env, model, stop={'episode_reward_mean': 2000, 'timesteps_total': 10000000})```  |
+        | policy sharing | ```algo.fit(env, model, share_policy='all') # or 'group' / 'individual'```  |
+        | save model | ```algo.fit(env, model, checkpoint_freq=100, checkpoint_end=True)```  |
+        | GPU accelerate  | ```algo.fit(env, model, local_mode=False, num_gpus=1)``` |
+        | CPU accelerate | ```algo.fit(env, model, local_mode=False, num_workers=5)```  |
+        
+        </details>
+        
+        <details>
+        <summary><b><big>Training & rendering API</big></b></summary>
+        
+        ```py
+        from marllib import marl
+        
+        # prepare env
+        env = marl.make_env(environment_name="mpe", map_name="simple_spread")
+        # initialize algorithm with appointed hyper-parameters
+        mappo = marl.algos.mappo(hyperparam_source="mpe")
+        # build agent model based on env + algorithms + user preference
+        model = marl.build_model(env, mappo, {"core_arch": "mlp", "encode_layer": "128-256"})
+        # start training
+        mappo.fit(
+          env, model, 
+          stop={"timesteps_total": 1000000}, 
+          checkpoint_freq=100, 
+          share_policy="group"
+        )
+        # rendering
+        mappo.render(
+          env, model, 
+          local_mode=True, 
+          restore_path={'params_path': "checkpoint_000010/params.json",
+                        'model_path': "checkpoint_000010/checkpoint-10"}
+        )
+        ```
+        </details>
+        
+        ## Benchmark results
+        
+        All results are listed [here](https://github.com/Replicable-MARL/MARLlib/tree/main/results).
+        
+        ## Quick examples
+        
+        MARLlib provides some practical examples for you to refer to.
+        
+        - [Detailed API usage](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/api_basic_usage.py): show how to use MARLlib api in
+          detail, e.g. cmd + api combined running.
+        - [Policy sharing cutomization](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/customize_policy_sharing.py):
+          define your group policy-sharing strategy as you like based on current tasks.
+        - [Loading model and rendering](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/load_and_render_model.py):
+          render the environment based on the pre-trained model.
+        - [Incorporating new environment](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_env.py):
+          add your new environment following MARLlib's env-agent interaction interface.
+        - [Incorporating new algorithm](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_algorithm.py):
+          add your new algorithm following MARLlib learning pipeline.
+        
+        ## Tutorials
+        
+        Try MPE + MAPPO examples on Google Colaboratory!
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
+        
+        More tutorial documentations are available [here](https://marllib.readthedocs.io/).
+        
+        ## Awesome List
+        
+        A collection of research and review papers of multi-agent reinforcement learning (MARL) is available. The papers have been organized based on their publication date and their evaluation of the corresponding environments.
+        
+        Algorithms: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
+        Environments: [![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/handbook/env.html)
+        
+        
+        ## Community
+        
+        |  Channel   | Link |
+        | :----------- | :----------- |
+        | Issues | [GitHub Issues](https://github.com/Replicable-MARL/MARLlib/issues) |
+        
+        ## Roadmap
+        
+        The roadmap to the future release is available in [ROADMAP.md](https://github.com/Replicable-MARL/MARLlib/blob/main/ROADMAP.md).
+        
+        ## Contributing
+        
+        We are a small team on multi-agent reinforcement learning, and we will take all the help we can get! 
+        If you would like to get involved, here is information on [contribution guidelines and how to test the code locally](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/CONTRIBUTING.md).
+        
+        You can contribute in multiple ways, e.g., reporting bugs, writing or translating documentation, reviewing or refactoring code, requesting or implementing new features, etc.
+        
+        ## Paper
+        
+        If you use MARLlib in your research, please cite the [MARLlib paper](https://arxiv.org/abs/2210.13708).
+        
+        ```tex
+        @article{hu2022marllib,
+          title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},
+          author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},
+          journal={arXiv preprint arXiv:2210.13708},
+          year={2022}
+        }
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-<img src=docs/source/images/logo1.png width=65% />
-</div>
-
-<h1 align="center"> MARLlib: An Extensive Multi-agent Reinforcement Learning Library </h1>
-
-
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]()
-![test](https://github.com/Replicable-MARL/MARLlib/workflows/test/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/)
-[![GitHub issues](https://img.shields.io/github/issues/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib/issues)
-[![PyPI version](https://badge.fury.io/py/marllib.svg)](https://badge.fury.io/py/marllib)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
-[![Awesome](https://awesome.re/badge.svg)](https://marllib.readthedocs.io/en/latest/resources/awesome.html)
-
-**Multi-agent Reinforcement Learning Library ([MARLlib](https://arxiv.org/abs/2210.13708))** is ***a MARL library*** based
-on [**Ray**](https://github.com/ray-project/ray) and one of its toolkits [**RLlib**](https://github.com/ray-project/ray/tree/master/rllib). It provides the MARL research community a unified
-platform for building, training, and evaluating MARL algorithms on almost all diverse tasks and environments.
-
-A simple case of MARLlib usage:
-
-```py
-from marllib import marl
-
-# prepare env
-env = marl.make_env(environment_name="mpe", map_name="simple_spread")
-
-# initialize algorithm with appointed hyper-parameters
-mappo = marl.algos.mappo(hyperparam_source='mpe')
-
-# build agent model based on env + algorithms + user preference
-model = marl.build_model(env, mappo, {"core_arch": "gru", "encode_layer": "128-256"})
-
-# start training
-mappo.fit(env, model, stop={'timesteps_total': 1000000}, share_policy='group')
-
-# ready to control
-mappo.render(env, model, share_policy='group', restore_path='path_to_checkpoint')
-```
-
-## Why MARLlib?
-
-Here we provide a table for the comparison of MARLlib and existing work.
-
-|   Library   |  Supported Env | Algorithm | Parameter Sharing  | Model 
-|:-------------:|:-------------:|:-------------:|:--------------:|:----------------:|
-|     [PyMARL](https://github.com/oxwhirl/pymarl) |        1 cooperative       |       5       |         share        |      GRU           | :x:
-|   [PyMARL2](https://github.com/hijkzzz/pymarl2)|        2 cooperative       |     11   |         share        |  MLP + GRU  | :x:
-| [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy) |       4 cooperative       |      1     |          share + separate        |          MLP + GRU        |         :x:              |
-| [MAlib](https://github.com/sjtu-marl/malib) |  4 self-play  | 10 | share + group + separate | MLP + LSTM | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest)
-|    [EPyMARL](https://github.com/uoe-agents/epymarl)|        4 cooperative      |    9    |        share + separate       |      GRU             |           :x:            |
-|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |       10 **no task mode restriction**     |    18     |   share + group + separate + **customizable**         |         MLP + CNN + GRU + LSTM          |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) |
-
-|   Library   | Github Stars  | Documentation | Issues Open | Activity | Last Update
-|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
-|     [PyMARL](https://github.com/oxwhirl/pymarl) | [![GitHub stars](https://img.shields.io/github/stars/oxwhirl/pymarl)](https://github.com/oxwhirl/pymarl)    |       :x: | ![GitHub opened issue](https://img.shields.io/github/issues/oxwhirl/pymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/oxwhirl/pymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/oxwhirl/pymarl?label=last%20update)  
-|   [PyMARL2](https://github.com/hijkzzz/pymarl2)| [![GitHub stars](https://img.shields.io/github/stars/hijkzzz/pymarl2)](https://github.com/hijkzzz/pymarl2)       |       :x:  | ![GitHub opened issue](https://img.shields.io/github/issues/hijkzzz/pymarl2.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/hijkzzz/pymarl2?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/hijkzzz/pymarl2?label=last%20update)  
-| [MAPPO Benchmark](https://github.com/marlbenchmark/on-policy)| [![GitHub stars](https://img.shields.io/github/stars/marlbenchmark/on-policy)](https://github.com/marlbenchmark/on-policy)   |        :x:              | ![GitHub opened issue](https://img.shields.io/github/issues/marlbenchmark/on-policy.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/marlbenchmark/on-policy?label=commit)| ![GitHub last commit](https://img.shields.io/github/last-commit/marlbenchmark/on-policy?label=last%20update)  
-| [MAlib](https://github.com/sjtu-marl/malib) | [![GitHub stars](https://img.shields.io/github/stars/sjtu-marl/malib)](https://github.com/hijkzzz/sjtu-marl/malib) | [![Documentation Status](https://readthedocs.org/projects/malib/badge/?version=latest)](https://malib.readthedocs.io/en/latest/?badge=latest) | ![GitHub opened issue](https://img.shields.io/github/issues/sjtu-marl/malib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/sjtu-marl/malib?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/sjtu-marl/malib?label=last%20update)  
-|    [EPyMARL](https://github.com/uoe-agents/epymarl)| [![GitHub stars](https://img.shields.io/github/stars/uoe-agents/epymarl)](https://github.com/uoe-agents/epymarl)        |           :x:            | ![GitHub opened issue](https://img.shields.io/github/issues/uoe-agents/epymarl.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/y/uoe-agents/epymarl?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/uoe-agents/epymarl?label=last%20update)  
-|    **[MARLlib](https://github.com/Replicable-MARL/MARLlib)** |  [![GitHub stars](https://img.shields.io/github/stars/Replicable-MARL/MARLlib)](https://github.com/Replicable-MARL/MARLlib)  |           [![Documentation Status](https://readthedocs.org/projects/marllib/badge/?version=latest)](https://marllib.readthedocs.io/en/latest/) | ![GitHub opened issue](https://img.shields.io/github/issues/Replicable-MARL/MARLlib.svg) | ![GitHub commit-activity](https://img.shields.io/github/commit-activity/m/Replicable-MARL/MARLlib/sy_dev?label=commit) | ![GitHub last commit](https://img.shields.io/github/last-commit/Replicable-MARL/MARLlib/sy_dev?label=last%20update)  
-
-
-
-[comment]: <> (<div align="center">)
-
-[comment]: <> (<img src=docs/source/images/overview.png width=100% />)
-
-[comment]: <> (</div>)
-
-## key features
-
-:beginner: What **MARLlib** brings to MARL community:
-
-- it unifies diverse algorithm pipelines with agent-level distributed dataflow.
-- it supports all task modes: cooperative, collaborative, competitive, and mixed.
-- it unifies multi-agent environment interfaces with a new interface following Gym.
-- it provides flexible and customizable parameter-sharing strategies.
-
-:rocket: With MARLlib, you can exploit the advantages not limited to:
-
-- **zero knowledge of MARL**: out of the box 18 algorithms with intuitive API!
-- **all task modes available**: support almost all multi-agent environment!
-- **customizable model arch**: pick your favorite one from the model zoo!
-- **customizable policy sharing**: grouped by MARLlib or build your own!
-- more than a thousand experiments are conducted and released!
-
-## Installation
-
-> __Note__:
-> MARLlib supports Linux only.
-
-### Step-by-step  (recommended)
-
-- install dependencies
-- install environments
-- install patches
-
-#### 1. install dependencies (basic)
-
-First, install MARLlib dependencies to guarantee basic usage.
-following [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html), finally install patches for RLlib.
-
-```bash
-$ conda create -n marllib python=3.8
-$ conda activate marllib
-$ git clone https://github.com/Replicable-MARL/MARLlib.git && cd MARLlib
-$ pip install -r requirements.txt
-```
-
-#### 2. install environments (optional)
-
-Please follow [this guide](https://marllib.readthedocs.io/en/latest/handbook/env.html).
-
-#### 3. install patches (basic)
-
-Fix bugs of RLlib using patches by running the following command:
-
-```bash
-$ cd /Path/To/MARLlib/marl/patch
-$ python add_patch.py -y
-```
-
-### PyPI
-
-```bash
-$ pip install --upgrade pip
-$ pip install marllib
-```
-
-## Getting started
-
-<details>
-<summary><b><big>Prepare the configuration</big></b></summary>
-
-There are four parts of configurations that take charge of the whole training process.
-
-- scenario: specify the environment/task settings
-- algorithm: choose the hyperparameters of the algorithm
-- model: customize the model architecture
-- ray/rllib: change the basic training settings
-
-<div align="center">
-<img src=docs/source/images/configurations.png width=100% />
-</div>
-
-Before training, ensure all the parameters are set correctly, especially those you don't want to change.
-> __Note__:
-> You can also modify all the pre-set parameters via MARLLib API.*
-
-</details>
-
-<details>
-<summary><b><big>Register the environment</big></b></summary>
-
-Ensure all the dependencies are installed for the environment you are running with. Otherwise, please refer to
-[MARLlib documentation](https://marllib.readthedocs.io/en/latest/handbook/env.html).
-
-
-|   task mode   | api example |
-| :-----------: | ----------- |
-| cooperative | ```marl.make_env(environment_name="mpe", map_name="simple_spread", force_coop=True)``` |
-| collaborative | ```marl.make_env(environment_name="mpe", map_name="simple_spread")``` |
-| competitive | ```marl.make_env(environment_name="mpe", map_name="simple_adversary")``` |
-| mixed | ```marl.make_env(environment_name="mpe", map_name="simple_crypto")``` |
-
-Most of the popular environments in MARL research are supported by MARLlib:
-
-| Env Name | Learning Mode | Observability | Action Space | Observations |
-| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
-| **[LBF](https://github.com/semitable/lb-foraging)**  | cooperative + collaborative | Both | Discrete | 1D  |
-| **[RWARE](https://github.com/semitable/robotic-warehouse)**  | cooperative | Partial | Discrete | 1D  |
-| **[MPE](https://github.com/openai/multiagent-particle-envs)**  | cooperative + collaborative + mixed | Both | Both | 1D  |
-| **[SMAC](https://github.com/oxwhirl/smac)**  | cooperative | Partial | Discrete | 1D |
-| **[MetaDrive](https://github.com/decisionforce/metadrive)**  | collaborative | Partial | Continuous | 1D |
-| **[MAgent](https://www.pettingzoo.ml/magent)** | collaborative + mixed | Partial | Discrete | 2D |
-| **[Pommerman](https://github.com/MultiAgentLearning/playground)**  | collaborative + competitive + mixed | Both | Discrete | 2D |
-| **[MAMuJoCo](https://github.com/schroederdewitt/multiagent_mujoco)**  | cooperative | Partial | Continuous | 1D |
-| **[GRF](https://github.com/google-research/football)**  | collaborative + mixed | Full | Discrete | 2D |
-| **[Hanabi](https://github.com/deepmind/hanabi-learning-environment)** | cooperative | Partial | Discrete | 1D |
-
-Each environment has a readme file, standing as the instruction for this task, including env settings, installation, and
-important notes.
-</details>
-
-<details>
-<summary><b><big>Initialize the algorithm</big></b></summary>
-
-
-|  running target   | api example |
-| :-----------: | ----------- |
-| train & finetune  | ```marl.algos.mappo(hyperparam_source=$ENV)``` |
-| develop & debug | ```marl.algos.mappo(hyperparam_source="test")``` |
-| 3rd party env | ```marl.algos.mappo(hyperparam_source="common")``` |
-
-Here is a chart describing the characteristics of each algorithm:
-
-| algorithm                                                    | support task mode | discrete action   | continuous action |  policy type        |
-| :------------------------------------------------------------: | :-----------------: | :----------: | :--------------------: | :----------: | 
-| *IQL**                                                         | all four               | :heavy_check_mark:   |    |  off-policy |
-| *[PG](https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf)* | all four                  | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[A2C](https://arxiv.org/abs/1602.01783)*                      | all four              | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[DDPG](https://arxiv.org/abs/1509.02971)*                     | all four             |  | :heavy_check_mark:   |  off-policy |
-| *[TRPO](http://proceedings.mlr.press/v37/schulman15.pdf)*      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[PPO](https://arxiv.org/abs/1707.06347)*                      | all four            | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[COMA](https://ojs.aaai.org/index.php/AAAI/article/download/11794/11653)* | all four                           | :heavy_check_mark:       |   |  on-policy  |
-| *[MADDPG](https://arxiv.org/abs/1706.02275)*                   | all four                     |  | :heavy_check_mark:   |  off-policy |
-| *MAA2C**                                                       | all four                        | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *MATRPO**                                                      | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[MAPPO](https://arxiv.org/abs/2103.01955)*                    | all four                         | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[HATRPO](https://arxiv.org/abs/2109.11251)*                   | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[HAPPO](https://arxiv.org/abs/2109.11251)*                    | cooperative                     | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *[VDN](https://arxiv.org/abs/1706.05296)*                      | cooperative         | :heavy_check_mark:   |    |  off-policy |
-| *[QMIX](https://arxiv.org/abs/1803.11485)*                     | cooperative                    | :heavy_check_mark:   |   |  off-policy |
-| *[FACMAC](https://arxiv.org/abs/2003.06709)*                   | cooperative                    |  | :heavy_check_mark:   |  off-policy |
-| *[VDAC](https://arxiv.org/abs/2007.12306)*                    | cooperative                    | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-| *VDPPO**                                                      | cooperative                | :heavy_check_mark:       | :heavy_check_mark:   |  on-policy  |
-
-***all four**: cooperative collaborative competitive mixed
-
-*IQL* is the multi-agent version of Q learning.
-*MAA2C* and *MATRPO* are the centralized version of A2C and TRPO.
-*VDPPO* is the value decomposition version of PPO.
-
-</details>
-
-<details>
-<summary><b><big>Build the agent model</big></b></summary>
-
-An agent model consists of two parts, `encoder` and `core arch`. 
-`encoder` will be constructed by MARLlib according to the observation space.
-Choose `mlp`, `gru`, or `lstm` as you like to build the complete model.
-
-|  model arch   | api example |
-| :-----------: | ----------- |
-| MLP  | ```marl.build_model(env, algo, {"core_arch": "mlp")``` |
-| GRU | ```marl.build_model(env, algo, {"core_arch": "gru"})```  |
-| LSTM | ```marl.build_model(env, algo, {"core_arch": "lstm"})```  |
-| Encoder Arch | ```marl.build_model(env, algo, {"core_arch": "gru", "encode_layer": "128-256"})```  |
-
-
-</details>
-
-<details>
-<summary><b><big>Kick off the training</big></b></summary>
-
-|  setting   | api example |
-| :-----------: | ----------- |
-| train  | ```algo.fit(env, model)``` |
-| debug  | ```algo.fit(env, model, local_mode=True)``` |
-| stop condition | ```algo.fit(env, model, stop={'episode_reward_mean': 2000, 'timesteps_total': 10000000})```  |
-| policy sharing | ```algo.fit(env, model, share_policy='all') # or 'group' / 'individual'```  |
-| save model | ```algo.fit(env, model, checkpoint_freq=100, checkpoint_end=True)```  |
-| GPU accelerate  | ```algo.fit(env, model, local_mode=False, num_gpus=1)``` |
-| CPU accelerate | ```algo.fit(env, model, local_mode=False, num_workers=5)```  |
-
-</details>
-
-<details>
-<summary><b><big>Training & rendering API</big></b></summary>
-
-```py
-from marllib import marl
-
-# prepare env
-env = marl.make_env(environment_name="mpe", map_name="simple_spread")
-# initialize algorithm with appointed hyper-parameters
-mappo = marl.algos.mappo(hyperparam_source="mpe")
-# build agent model based on env + algorithms + user preference
-model = marl.build_model(env, mappo, {"core_arch": "mlp", "encode_layer": "128-256"})
-# start training
-mappo.fit(
-  env, model, 
-  stop={"timesteps_total": 1000000}, 
-  checkpoint_freq=100, 
-  share_policy="group"
-)
-# rendering
-mappo.render(
-  env, model, 
-  local_mode=True, 
-  restore_path={'params_path': "checkpoint_000010/params.json",
-                'model_path': "checkpoint_000010/checkpoint-10"}
-)
-```
-</details>
-
-## Benchmark results
-
-All results are listed [here](https://github.com/Replicable-MARL/MARLlib/tree/main/results).
-
-## Quick examples
-
-MARLlib provides some practical examples for you to refer to.
-
-- [Detailed API usage](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/api_basic_usage.py): show how to use MARLlib api in
-  detail, e.g. cmd + api combined running.
-- [Policy sharing cutomization](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/customize_policy_sharing.py):
-  define your group policy-sharing strategy as you like based on current tasks.
-- [Loading model and rendering](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/load_and_render_model.py):
-  render the environment based on the pre-trained model.
-- [Incorporating new environment](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_env.py):
-  add your new environment following MARLlib's env-agent interaction interface.
-- [Incorporating new algorithm](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/examples/add_new_algorithm.py):
-  add your new algorithm following MARLlib learning pipeline.
-
-## Tutorials
-
-Try MPE + MAPPO examples on Google Colaboratory!
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Replicable-MARL/MARLlib/blob/sy_dev/marllib.ipynb)
-
-More tutorial documentations are available [here](https://marllib.readthedocs.io/).
-
-## Community
-
-|  Channel   | Link |
-| :----------- | :----------- |
-| Issues | [GitHub Issues](https://github.com/Replicable-MARL/MARLlib/issues) |
-
-
-## Contributing
-
-We are a small team on multi-agent reinforcement learning, and we will take all the help we can get! 
-If you would like to get involved, here is information on [contribution guidelines and how to test the code locally](https://github.com/Replicable-MARL/MARLlib/blob/sy_dev/CONTRIBUTING.md).
-
-You can contribute in multiple ways, e.g., reporting bugs, writing or translating documentation, reviewing or refactoring code, requesting or implementing new features, etc.
-
-[comment]: <> (## Paper)
-
-[comment]: <> (If you use MARLlib in your research, please cite the [MARLlib paper]&#40;https://arxiv.org/abs/2210.13708&#41;.)
-
-[comment]: <> (```tex)
-
-[comment]: <> (@article{hu2022marllib,)
-
-[comment]: <> (  title={MARLlib: Extending RLlib for Multi-agent Reinforcement Learning},)
-
-[comment]: <> (  author={Hu, Siyi and Zhong, Yifan and Gao, Minquan and Wang, Weixun and Dong, Hao and Li, Zhihui and Liang, Xiaodan and Chang, Xiaojun and Yang, Yaodong},)
-
-[comment]: <> (  journal={arXiv preprint arXiv:2210.13708},)
-
-[comment]: <> (  year={2022})
-
-[comment]: <> (})
-
-[comment]: <> (```)
-
```

### Comparing `marllib-1.0.2/marllib.egg-info/SOURCES.txt` & `marllib-1.0.3/marllib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 marllib.egg-info/SOURCES.txt
 marllib.egg-info/dependency_links.txt
 marllib.egg-info/requires.txt
 marllib.egg-info/top_level.txt
 marllib/envs/__init__.py
 marllib/envs/base_env/__init__.py
 marllib/envs/base_env/football.py
+marllib/envs/base_env/gobigger.py
 marllib/envs/base_env/hanabi.py
 marllib/envs/base_env/lbf.py
 marllib/envs/base_env/magent.py
 marllib/envs/base_env/mamujoco.py
+marllib/envs/base_env/mate.py
 marllib/envs/base_env/metadrive.py
 marllib/envs/base_env/mpe.py
 marllib/envs/base_env/pommerman.py
 marllib/envs/base_env/rware.py
 marllib/envs/base_env/smac.py
 marllib/envs/base_env/config/__init__.py
 marllib/envs/base_env/config/football.yaml
@@ -32,17 +34,19 @@
 marllib/envs/base_env/config/mpe.yaml
 marllib/envs/base_env/config/pommerman.yaml
 marllib/envs/base_env/config/rware.yaml
 marllib/envs/base_env/config/smac.yaml
 marllib/envs/base_env/install/__init__.py
 marllib/envs/global_reward_env/__init__.py
 marllib/envs/global_reward_env/football_fcoop.py
+marllib/envs/global_reward_env/gobigger_fcoop.py
 marllib/envs/global_reward_env/lbf_fcoop.py
 marllib/envs/global_reward_env/magent_fcoop.py
 marllib/envs/global_reward_env/mamujoco_fcoop.py
+marllib/envs/global_reward_env/mate_fcoop.py
 marllib/envs/global_reward_env/mpe_fcoop.py
 marllib/envs/global_reward_env/pommerman_fcoop.py
 marllib/envs/global_reward_env/rware_fcoop.py
 marllib/envs/global_reward_env/smac_fcoop.py
 marllib/marl/__init__.py
 marllib/marl/common.py
 marllib/marl/algos/__init__.py
@@ -211,14 +215,15 @@
 marllib/marl/models/zoo/rnn/jointQ_rnn.py
 marllib/marl/models/zoo/rnn/vd_rnn.py
 marllib/marl/ray/__init__.py
 marllib/marl/ray/ray.yaml
 marllib/marl/ray/ray_beta.yaml
 marllib/patch/__init__.py
 marllib/patch/add_patch.py
+marllib/patch/test.py
 marllib/patch/hanabi/Hanabi_Env.py
 marllib/patch/hanabi/__init__.py
 marllib/patch/hanabi/pyhanabi.py
 marllib/patch/pommerman_patch/__init__.py
 marllib/patch/pommerman_patch/forward_model.py
 marllib/patch/pommerman_patch/graphics.py
 marllib/patch/pommerman_patch/v0.py
```

### Comparing `marllib-1.0.2/multiagent_mujoco/coupled_half_cheetah.py` & `marllib-1.0.3/multiagent_mujoco/coupled_half_cheetah.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/multiagent_mujoco/manyagent_ant.py` & `marllib-1.0.3/multiagent_mujoco/manyagent_ant.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/multiagent_mujoco/manyagent_swimmer.py` & `marllib-1.0.3/multiagent_mujoco/manyagent_swimmer.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/multiagent_mujoco/mujoco_multi.py` & `marllib-1.0.3/multiagent_mujoco/mujoco_multi.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/multiagent_mujoco/multiagentenv.py` & `marllib-1.0.3/multiagent_mujoco/multiagentenv.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/multiagent_mujoco/obsk.py` & `marllib-1.0.3/multiagent_mujoco/obsk.py`

 * *Files identical despite different names*

### Comparing `marllib-1.0.2/setup.py` & `marllib-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="marllib",
-    version="1.0.2",
+    version="1.0.3",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["examples", "docs", "tests"]),
     license="MIT",
     python_requires=">=3.8",
     package_data={'': ['*.yaml']},
     include_package_data=True,
```

