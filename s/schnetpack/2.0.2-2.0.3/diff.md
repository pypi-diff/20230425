# Comparing `tmp/schnetpack-2.0.2.tar.gz` & `tmp/schnetpack-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schnetpack-2.0.2.tar", last modified: Mon Apr 24 09:40:30 2023, max compression
+gzip compressed data, was "schnetpack-2.0.3.tar", last modified: Tue Apr 25 11:23:56 2023, max compression
```

## Comparing `schnetpack-2.0.2.tar` & `schnetpack-2.0.3.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 09:40:20.000000 schnetpack-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:40:20.000000 schnetpack-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 09:40:30.381232 schnetpack-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-04-24 09:40:20.000000 schnetpack-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:40:30.381232 schnetpack-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 09:40:20.000000 schnetpack-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/atomistic/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/atomwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/external_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/nuclear_repulsion.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/configs/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/checkpoint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/earlystopping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/ema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/lrmonitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/data/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/ani1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/custom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/iso17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/materials_project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/md17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/md22.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/omdb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/qm9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/rmd17.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/md17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_atomwise.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_dipole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/response.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/globals/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/globals/default_globals.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/aim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/csv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/tensorboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/nnp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/field_schnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/painn.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/bessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/schnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/so3net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/predict.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/run/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/run/default_run.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/default_task.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/adabelief.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/train.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/ddp_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/ddp_trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/debug_trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/default_trainer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/data/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/ani1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/iso17.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/md17.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/md22.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/qm9.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/rmd17.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/ase_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    28296 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/batchwise_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/calculators/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/base_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/ensemble_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/lj_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/orca_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/schnetpack_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/data/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/lj.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/ase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/matscipy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/torch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/orca.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/spk.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/spk_ensemble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/checkpoint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/hdf5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/tensorboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/nhc_aniso.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/nhc_iso.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/pile_rpmd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/md.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/rpmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/berendsen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/gle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/langevin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/nhc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_gle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/piglet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pile_global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pile_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/trpmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/maxwell_boltzmann.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/uniform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/neighborlist_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/parsers/orca_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats_rpmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/callback_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats.py
--rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/md_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/normal_model_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/thermostat_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/model/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/equivariant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/nn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/so3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/radial.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/so3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/representation/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/field_schnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/painn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/schnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/so3net.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/train/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/neighborlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/utils/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkconvert
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkdeploy
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkmd
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkpredict
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spktrain
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.186491 schnetpack-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-25 11:23:40.000000 schnetpack-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 11:23:40.000000 schnetpack-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 11:23:56.182491 schnetpack-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-04-25 11:23:40.000000 schnetpack-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:23:56.186491 schnetpack-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-25 11:23:40.000000 schnetpack-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.154491 schnetpack-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.158491 schnetpack-2.0.3/src/schnetpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.158491 schnetpack-2.0.3/src/schnetpack/atomistic/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/atomwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/external_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/nuclear_repulsion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/atomistic/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.158491 schnetpack-2.0.3/src/schnetpack/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.158491 schnetpack-2.0.3/src/schnetpack/configs/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/callbacks/checkpoint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/callbacks/earlystopping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/callbacks/ema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/callbacks/lrmonitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/ani1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/iso17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/materials_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/md17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/md22.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/omdb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/qm9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/data/rmd17.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/experiment/md17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/experiment/qm9_atomwise.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/experiment/qm9_dipole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/experiment/response.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/globals/default_globals.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/logger/aim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/logger/csv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/logger/tensorboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/nnp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/model/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/field_schnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/painn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/model/representation/radial_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/radial_basis/bessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/radial_basis/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/schnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/model/representation/so3net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/predict.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/run/default_run.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/task/default_task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.162491 schnetpack-2.0.3/src/schnetpack/configs/task/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/task/optimizer/adabelief.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/task/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/task/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.166491 schnetpack-2.0.3/src/schnetpack/configs/task/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/task/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/train.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.166491 schnetpack-2.0.3/src/schnetpack/configs/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/trainer/ddp_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/trainer/ddp_trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/trainer/debug_trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/configs/trainer/default_trainer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.166491 schnetpack-2.0.3/src/schnetpack/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/data/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.166491 schnetpack-2.0.3/src/schnetpack/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/ani1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/iso17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/md17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/md22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/qm9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/datasets/rmd17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.166491 schnetpack-2.0.3/src/schnetpack/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/interfaces/ase_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28296 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/interfaces/batchwise_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/base_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/ensemble_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/lj_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/orca_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/calculators/schnetpack_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/data/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/data/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/md_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/lj.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.170491 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/neighbor_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/neighbor_list/ase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/neighbor_list/matscipy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/neighbor_list/torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/orca.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/spk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/calculator/spk_ensemble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/callbacks/checkpoint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/callbacks/hdf5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/callbacks/tensorboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/barostat/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/barostat/nhc_aniso.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/barostat/nhc_iso.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/barostat/pile_rpmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/integrator/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/integrator/md.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/integrator/rpmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/berendsen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/gle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/langevin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/nhc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/pi_gle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/piglet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/pile_global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/pile_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/dynamics/thermostat/trpmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.174491 schnetpack-2.0.3/src/schnetpack/md/md_configs/system/initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/system/initializer/maxwell_boltzmann.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/system/initializer/uniform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/md_configs/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/neighborlist_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.178491 schnetpack-2.0.3/src/schnetpack/md/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/parsers/orca_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.178491 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/barostats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/barostats_rpmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/callback_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/thermostats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.178491 schnetpack-2.0.3/src/schnetpack/md/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/utils/md_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/utils/normal_model_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/md/utils/thermostat_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.178491 schnetpack-2.0.3/src/schnetpack/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.178491 schnetpack-2.0.3/src/schnetpack/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/equivariant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/schnetpack/nn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/ops/so3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/radial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/so3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/schnetpack/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/representation/field_schnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/representation/painn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/representation/schnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/representation/so3net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/schnetpack/train/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/train/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/train/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/train/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/schnetpack/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/neighborlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/transform/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/schnetpack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/schnetpack/utils/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.158491 schnetpack-2.0.3/src/schnetpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 11:23:56.000000 schnetpack-2.0.3/src/schnetpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-25 11:23:56.000000 schnetpack-2.0.3/src/schnetpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:23:56.000000 schnetpack-2.0.3/src/schnetpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 11:23:56.000000 schnetpack-2.0.3/src/schnetpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 11:23:56.000000 schnetpack-2.0.3/src/schnetpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:23:56.182491 schnetpack-2.0.3/src/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/scripts/spkconvert
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/scripts/spkdeploy
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/scripts/spkmd
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/scripts/spkpredict
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 11:23:40.000000 schnetpack-2.0.3/src/scripts/spktrain
```

### Comparing `schnetpack-2.0.2/LICENSE` & `schnetpack-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/PKG-INFO` & `schnetpack-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schnetpack
-Version: 2.0.2
+Version: 2.0.3
 Summary: SchNetPack - Deep Neural Networks for Atomistic Systems
 Home-page: https://github.com/atomistic-machine-learning/schnetpack
 Author: Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer
 License: MIT
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `schnetpack-2.0.2/README.md` & `schnetpack-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/setup.py` & `schnetpack-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with io.open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="schnetpack",
-    version="2.0.2",
+    version="2.0.3",
     author="Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer",
     url="https://github.com/atomistic-machine-learning/schnetpack",
     packages=find_packages("src"),
     scripts=[
         "src/scripts/spkconvert",
         "src/scripts/spktrain",
         "src/scripts/spkpredict",
```

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/aggregation.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/aggregation.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/atomwise.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/atomwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,18 @@
             n_layers: number of layers.
             aggregation_mode: one of {sum, avg} (default: sum)
             output_key: the key under which the result will be stored
             per_atom_output_key: If not None, the key under which the per-atom result will be stored
         """
         super(Atomwise, self).__init__()
         self.output_key = output_key
-        self.model_outputs = [output_key, per_atom_output_key]
+        self.model_outputs = [output_key]
         self.per_atom_output_key = per_atom_output_key
+        if self.per_atom_output_key is not None:
+            self.model_outputs.append(self.per_atom_output_key)
         self.n_out = n_out
 
         if aggregation_mode is None and self.per_atom_output_key is None:
             raise ValueError(
                 "If `aggregation_mode` is None, `per_atom_output_key` needs to be set,"
                 + " since no accumulated output will be returned!"
             )
```

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/distances.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/distances.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/electrostatic.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/electrostatic.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/external_fields.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/external_fields.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/nuclear_repulsion.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/nuclear_repulsion.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/atomistic/response.py` & `schnetpack-2.0.3/src/schnetpack/atomistic/response.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/cli.py` & `schnetpack-2.0.3/src/schnetpack/cli.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/experiment/md17.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/experiment/md17.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_atomwise.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/experiment/qm9_atomwise.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_dipole.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/experiment/qm9_dipole.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/experiment/response.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/experiment/response.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/predict.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/predict.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/configs/train.yaml` & `schnetpack-2.0.3/src/schnetpack/configs/train.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/data/atoms.py` & `schnetpack-2.0.3/src/schnetpack/data/atoms.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/data/datamodule.py` & `schnetpack-2.0.3/src/schnetpack/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/data/loader.py` & `schnetpack-2.0.3/src/schnetpack/data/loader.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/data/splitting.py` & `schnetpack-2.0.3/src/schnetpack/data/splitting.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/data/stats.py` & `schnetpack-2.0.3/src/schnetpack/data/stats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/ani1.py` & `schnetpack-2.0.3/src/schnetpack/datasets/ani1.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/iso17.py` & `schnetpack-2.0.3/src/schnetpack/datasets/iso17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/materials_project.py` & `schnetpack-2.0.3/src/schnetpack/datasets/materials_project.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/md17.py` & `schnetpack-2.0.3/src/schnetpack/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/md22.py` & `schnetpack-2.0.3/src/schnetpack/datasets/md22.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/omdb.py` & `schnetpack-2.0.3/src/schnetpack/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/qm9.py` & `schnetpack-2.0.3/src/schnetpack/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/datasets/rmd17.py` & `schnetpack-2.0.3/src/schnetpack/datasets/rmd17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/interfaces/ase_interface.py` & `schnetpack-2.0.3/src/schnetpack/interfaces/ase_interface.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/interfaces/batchwise_optimization.py` & `schnetpack-2.0.3/src/schnetpack/interfaces/batchwise_optimization.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/calculators/base_calculator.py` & `schnetpack-2.0.3/src/schnetpack/md/calculators/base_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/calculators/ensemble_calculator.py` & `schnetpack-2.0.3/src/schnetpack/md/calculators/ensemble_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/calculators/lj_calculator.py` & `schnetpack-2.0.3/src/schnetpack/md/calculators/lj_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/calculators/orca_calculator.py` & `schnetpack-2.0.3/src/schnetpack/md/calculators/orca_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/calculators/schnetpack_calculator.py` & `schnetpack-2.0.3/src/schnetpack/md/calculators/schnetpack_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/cli.py` & `schnetpack-2.0.3/src/schnetpack/md/cli.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/data/hdf5_data.py` & `schnetpack-2.0.3/src/schnetpack/md/data/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/data/spectra.py` & `schnetpack-2.0.3/src/schnetpack/md/data/spectra.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/initial_conditions.py` & `schnetpack-2.0.3/src/schnetpack/md/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/integrators.py` & `schnetpack-2.0.3/src/schnetpack/md/integrators.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/neighborlist_md.py` & `schnetpack-2.0.3/src/schnetpack/md/neighborlist_md.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/parsers/orca_parser.py` & `schnetpack-2.0.3/src/schnetpack/md/parsers/orca_parser.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/barostats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats_rpmd.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/barostats_rpmd.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/basic_hooks.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/basic_hooks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/callback_hooks.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/callback_hooks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/thermostats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py` & `schnetpack-2.0.3/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/simulator.py` & `schnetpack-2.0.3/src/schnetpack/md/simulator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/system.py` & `schnetpack-2.0.3/src/schnetpack/md/system.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/utils/__init__.py` & `schnetpack-2.0.3/src/schnetpack/md/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/utils/md_config.py` & `schnetpack-2.0.3/src/schnetpack/md/utils/md_config.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/utils/normal_model_transformation.py` & `schnetpack-2.0.3/src/schnetpack/md/utils/normal_model_transformation.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/md/utils/thermostat_utils.py` & `schnetpack-2.0.3/src/schnetpack/md/utils/thermostat_utils.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/model/base.py` & `schnetpack-2.0.3/src/schnetpack/model/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/activations.py` & `schnetpack-2.0.3/src/schnetpack/nn/activations.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/base.py` & `schnetpack-2.0.3/src/schnetpack/nn/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/blocks.py` & `schnetpack-2.0.3/src/schnetpack/nn/blocks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/cutoff.py` & `schnetpack-2.0.3/src/schnetpack/nn/cutoff.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/equivariant.py` & `schnetpack-2.0.3/src/schnetpack/nn/equivariant.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/ops/so3.py` & `schnetpack-2.0.3/src/schnetpack/nn/ops/so3.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/radial.py` & `schnetpack-2.0.3/src/schnetpack/nn/radial.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/scatter.py` & `schnetpack-2.0.3/src/schnetpack/nn/scatter.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/so3.py` & `schnetpack-2.0.3/src/schnetpack/nn/so3.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/nn/utils.py` & `schnetpack-2.0.3/src/schnetpack/nn/utils.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/properties.py` & `schnetpack-2.0.3/src/schnetpack/properties.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/representation/field_schnet.py` & `schnetpack-2.0.3/src/schnetpack/representation/field_schnet.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/representation/painn.py` & `schnetpack-2.0.3/src/schnetpack/representation/painn.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/representation/schnet.py` & `schnetpack-2.0.3/src/schnetpack/representation/schnet.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/representation/so3net.py` & `schnetpack-2.0.3/src/schnetpack/representation/so3net.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/task.py` & `schnetpack-2.0.3/src/schnetpack/task.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/train/callbacks.py` & `schnetpack-2.0.3/src/schnetpack/train/callbacks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/train/lr_scheduler.py` & `schnetpack-2.0.3/src/schnetpack/train/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/train/metrics.py` & `schnetpack-2.0.3/src/schnetpack/train/metrics.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/__init__.py` & `schnetpack-2.0.3/src/schnetpack/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/atomistic.py` & `schnetpack-2.0.3/src/schnetpack/transform/atomistic.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/base.py` & `schnetpack-2.0.3/src/schnetpack/transform/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/casting.py` & `schnetpack-2.0.3/src/schnetpack/transform/casting.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/neighborlist.py` & `schnetpack-2.0.3/src/schnetpack/transform/neighborlist.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/transform/response.py` & `schnetpack-2.0.3/src/schnetpack/transform/response.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/units.py` & `schnetpack-2.0.3/src/schnetpack/units.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/utils/__init__.py` & `schnetpack-2.0.3/src/schnetpack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack/utils/script.py` & `schnetpack-2.0.3/src/schnetpack/utils/script.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/schnetpack.egg-info/PKG-INFO` & `schnetpack-2.0.3/src/schnetpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schnetpack
-Version: 2.0.2
+Version: 2.0.3
 Summary: SchNetPack - Deep Neural Networks for Atomistic Systems
 Home-page: https://github.com/atomistic-machine-learning/schnetpack
 Author: Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer
 License: MIT
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `schnetpack-2.0.2/src/schnetpack.egg-info/SOURCES.txt` & `schnetpack-2.0.3/src/schnetpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/scripts/spkconvert` & `schnetpack-2.0.3/src/scripts/spkconvert`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.2/src/scripts/spkdeploy` & `schnetpack-2.0.3/src/scripts/spkdeploy`

 * *Files identical despite different names*

