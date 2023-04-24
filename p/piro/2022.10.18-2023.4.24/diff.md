# Comparing `tmp/piro-2022.10.18.tar.gz` & `tmp/piro-2023.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piro-2022.10.18.tar", last modified: Wed Oct 19 02:00:40 2022, max compression
+gzip compressed data, was "piro-2023.4.24.tar", last modified: Mon Apr 24 22:38:14 2023, max compression
```

## Comparing `piro-2022.10.18.tar` & `piro-2023.4.24.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2022-10-19 02:00:40.934074 piro-2022.10.18/
--rw-r--r--   0 josephmontoya   (503) staff       (20)    10743 2022-10-11 21:51:50.000000 piro-2022.10.18/LICENSE
--rw-r--r--   0 josephmontoya   (503) staff       (20)      855 2022-10-19 02:00:40.934200 piro-2022.10.18/PKG-INFO
--rw-r--r--   0 josephmontoya   (503) staff       (20)     3607 2022-10-11 21:51:50.000000 piro-2022.10.18/README.md
-drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2022-10-19 02:00:40.932122 piro-2022.10.18/piro/
--rw-r--r--   0 josephmontoya   (503) staff       (20)       27 2022-10-19 02:00:40.000000 piro-2022.10.18/piro/__init__.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)     3243 2022-10-11 21:51:50.000000 piro-2022.10.18/piro/data.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)     2379 2022-10-19 01:42:40.000000 piro-2022.10.18/piro/mprester.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)    15580 2022-10-11 21:51:50.000000 piro-2022.10.18/piro/reactions.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)    24534 2022-10-19 01:42:40.000000 piro-2022.10.18/piro/route.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)     1095 2022-10-11 21:51:50.000000 piro-2022.10.18/piro/settings.py
--rw-r--r--   0 josephmontoya   (503) staff       (20)     8831 2022-10-13 04:45:32.000000 piro-2022.10.18/piro/utils.py
-drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2022-10-19 02:00:40.933817 piro-2022.10.18/piro.egg-info/
--rw-r--r--   0 josephmontoya   (503) staff       (20)      855 2022-10-19 02:00:40.000000 piro-2022.10.18/piro.egg-info/PKG-INFO
--rw-r--r--   0 josephmontoya   (503) staff       (20)      285 2022-10-19 02:00:40.000000 piro-2022.10.18/piro.egg-info/SOURCES.txt
--rw-r--r--   0 josephmontoya   (503) staff       (20)        1 2022-10-19 02:00:40.000000 piro-2022.10.18/piro.egg-info/dependency_links.txt
--rw-r--r--   0 josephmontoya   (503) staff       (20)       82 2022-10-19 02:00:40.000000 piro-2022.10.18/piro.egg-info/requires.txt
--rw-r--r--   0 josephmontoya   (503) staff       (20)        5 2022-10-19 02:00:40.000000 piro-2022.10.18/piro.egg-info/top_level.txt
--rw-r--r--   0 josephmontoya   (503) staff       (20)     2468 2022-10-19 02:00:40.935577 piro-2022.10.18/setup.cfg
--rw-r--r--   0 josephmontoya   (503) staff       (20)     1522 2022-10-19 02:00:40.000000 piro-2022.10.18/setup.py
+drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2023-04-24 22:38:14.740046 piro-2023.4.24/
+-rw-r--r--   0 josephmontoya   (503) staff       (20)    10743 2023-04-24 19:08:26.000000 piro-2023.4.24/LICENSE
+-rw-r--r--   0 josephmontoya   (503) staff       (20)      877 2023-04-24 22:38:14.740343 piro-2023.4.24/PKG-INFO
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     3607 2023-04-24 19:08:26.000000 piro-2023.4.24/README.md
+drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2023-04-24 22:38:14.737228 piro-2023.4.24/piro/
+-rw-r--r--   0 josephmontoya   (503) staff       (20)       26 2023-04-24 22:21:14.000000 piro-2023.4.24/piro/__init__.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     7162 2023-04-24 19:08:26.000000 piro-2023.4.24/piro/custom_entry.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     3243 2023-04-24 19:08:26.000000 piro-2023.4.24/piro/data.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     2379 2023-04-24 19:08:26.000000 piro-2023.4.24/piro/mprester.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)    15580 2023-04-24 19:08:26.000000 piro-2023.4.24/piro/reactions.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)    24930 2023-04-24 21:24:53.000000 piro-2023.4.24/piro/route.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     1270 2023-04-24 20:24:20.000000 piro-2023.4.24/piro/settings.py
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     9054 2023-04-24 21:38:20.000000 piro-2023.4.24/piro/utils.py
+drwxr-xr-x   0 josephmontoya   (503) staff       (20)        0 2023-04-24 22:38:14.739709 piro-2023.4.24/piro.egg-info/
+-rw-r--r--   0 josephmontoya   (503) staff       (20)      877 2023-04-24 22:38:14.000000 piro-2023.4.24/piro.egg-info/PKG-INFO
+-rw-r--r--   0 josephmontoya   (503) staff       (20)      306 2023-04-24 22:38:14.000000 piro-2023.4.24/piro.egg-info/SOURCES.txt
+-rw-r--r--   0 josephmontoya   (503) staff       (20)        1 2023-04-24 22:38:14.000000 piro-2023.4.24/piro.egg-info/dependency_links.txt
+-rw-r--r--   0 josephmontoya   (503) staff       (20)      108 2023-04-24 22:38:14.000000 piro-2023.4.24/piro.egg-info/requires.txt
+-rw-r--r--   0 josephmontoya   (503) staff       (20)        5 2023-04-24 22:38:14.000000 piro-2023.4.24/piro.egg-info/top_level.txt
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     2468 2023-04-24 22:38:14.742055 piro-2023.4.24/setup.cfg
+-rw-r--r--   0 josephmontoya   (503) staff       (20)     1560 2023-04-24 22:21:04.000000 piro-2023.4.24/setup.py
```

### Comparing `piro-2022.10.18/LICENSE` & `piro-2023.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/PKG-INFO` & `piro-2023.4.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: piro
-Version: 2022.10.18
+Version: 2023.4.24
 Summary: piro is software designed to assist in planning of synthesis pathways for inorganics
 Author: AMDD - Toyota Research Institute
 Author-email: murat.aykol@tri.global
 Maintainer: Joseph Montoya
 Maintainer-email: joseph.montoya@tri.global
 Keywords: materials,battery,chemistry,science,density functional theory,energy,AI,artificial intelligence,sequential learning,active learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: m3gnet
 License-File: LICENSE
 
 
 The piro software package enables prediction and planning of synthesis pathways
 and determination of pareto-optimal frontiers for synthesis of
 specific inorganic materials.
```

### Comparing `piro-2022.10.18/README.md` & `piro-2023.4.24/README.md`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/piro/data.py` & `piro-2023.4.24/piro/data.py`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/piro/mprester.py` & `piro-2023.4.24/piro/mprester.py`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/piro/reactions.py` & `piro-2023.4.24/piro/reactions.py`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/piro/route.py` & `piro-2023.4.24/piro/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pymatgen.analysis.phase_diagram import PhaseDiagram
 from pymatgen.util.string import latexify
 from tqdm import tqdm
 
 from piro.data import GASES, GAS_RELEASE, DEFAULT_GAS_PRESSURES
 from piro.mprester import get_mprester
 from piro.reactions import get_reactions
-from piro.settings import settings
+from piro.settings import CacheType, settings
 from piro.utils import get_epitaxies, get_similarities
 
 
 logger = logging.getLogger(__name__)
 
 
 class SynthesisRoutes:
@@ -120,19 +120,25 @@
                 self.elts.extend(add_elements)
             self.get_mp_entries()
         else:
             self.elts = list(self.target_entry.composition.as_dict().keys())
 
         self.get_precursor_library()
         print("Precursor library ready.")
+        cache_type = CacheType.NO_CACHE if self.custom_target_entry else settings.cache_type
+        print("Epitaxy and Similarity cache type: ", cache_type)
         self.epitaxies = epitaxies if epitaxies else get_epitaxies(
-            self.precursor_library, self.target_entry
+            self.precursor_library,
+            self.target_entry,
+            cache_type
         )
         self.similarities = similarities if similarities else get_similarities(
-            self.precursor_library, self.target_entry
+            self.precursor_library,
+            self.target_entry,
+            cache_type
         )
 
         self._reactions_objs = None
 
     @property
     def reactions_objs(self):
         if not self._reactions_objs:
@@ -149,14 +155,17 @@
         with get_mprester() as mpr:
             if len(mpr.api_key) == 32:
                 self.entries = mpr.get_entries_in_chemsys(
                     self.elts,
                     inc_structure="final",
                     property_data=["material_id", "formation_energy_per_atom"],
                 )
+                # Hack to fix MP append
+                for entry in self.entries:
+                    entry.entry_id = entry.entry_id.replace("-GGA", "")
                 mp_ids = [ent.data['material_id'] for ent in self.entries]
                 provs = mpr.provenance.search(mp_ids, fields=['material_id', 'database_IDs', 'theoretical'])
                 from emmet.core.provenance import Database
                 mp_to_icsd = {str(doc.material_id): doc.database_IDs.get(Database.ICSD)
                               for doc in provs if not doc.theoretical}
                 for entry in self.entries:
                     entry.data.update({"icsd_ids": mp_to_icsd.get(entry.data['material_id'])})
```

### Comparing `piro-2022.10.18/piro/settings.py` & `piro-2023.4.24/piro/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,20 @@
         os.path.dirname(os.path.abspath(__file__)),
         'files'
     )
 
     cache_type: CacheType = CacheType.FILE_CACHE
     use_mapi_db: bool = False
 
+    @validator('mapi_key')
+    def update_env_with_mapi_key(cls, v):
+        if v and not os.environ.get('MAPI_KEY'):
+            os.environ['MAPI_KEY'] = v
+        return v
+
     @validator('cache_type')
     def check_cache_type(cls, v, values):
         if v == CacheType.MONGO_CACHE:
             if not values.get('mongodb_uri'):
                 raise ValueError('MONGODB_URI must be provided when using mongo cache.')
         return v
```

### Comparing `piro-2022.10.18/piro/utils.py` & `piro-2023.4.24/piro/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Tuple, List
 
 import pandas as pd
 import os
 import pickle
 import numpy as np
 import json
-from functools import lru_cache, wraps
+from functools import lru_cache
 
+from pymatgen.core import Structure
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymongo import MongoClient
 from scipy.interpolate import interp1d
 from pymatgen.core.composition import Composition
 from pymatgen.analysis.substrate_analyzer import SubstrateAnalyzer
 from matminer.featurizers.base import MultipleFeaturizer
 from matminer.featurizers.composition import (
@@ -36,91 +37,97 @@
 from piro.settings import settings, CacheType
 
 
 def get_v(composition_as_dict: dict, elts: Tuple[str]) -> np.array:
     return np.array([composition_as_dict[el] for el in elts])
 
 
-def get_epitaxies(precursor_library: List[ComputedStructureEntry], target: ComputedStructureEntry):
-    if settings.cache_type == CacheType.MONGO_CACHE:
+def get_epitaxies(
+    precursor_library: List[ComputedStructureEntry],
+    target: ComputedStructureEntry,
+    cache_type: CacheType
+):
+    if cache_type == CacheType.MONGO_CACHE:
         precursor_set = set([s.entry_id for s in precursor_library])
         epitaxies = {}
         for e in mongo_results_generator(target, 'epitaxies'):
             for material_id in e["material_ids"]:
                 if material_id in precursor_set:
                     # If "min_epitaxy" is not in the cached entry, most likely the epitaxy calculation failed.
                     # Assign the high value so they will get discounted.
                     epitaxies[material_id] = float(e.get("min_epitaxy", 1000000.0))
 
     else:
         precursor_structures = [s.structure for s in precursor_library]
         target_structure = target.structure
-        results = epitaxy(precursor_structures, target_structure)
+        if cache_type == CacheType.FILE_CACHE:
+            results = through_cache(precursor_structures, target_structure, epitaxy)
+        else:
+            results = epitaxy(precursor_structures, target_structure)
         epitaxies = dict(
             zip([i.entry_id for i in precursor_library], results)
         )
         print("Epitaxies ready")
 
     return epitaxies
 
 
-def get_similarities(precursor_library: List[ComputedStructureEntry], target: ComputedStructureEntry):
+def get_similarities(
+    precursor_library: List[ComputedStructureEntry],
+    target: ComputedStructureEntry,
+    cache_type: CacheType
+ ):
     if settings.cache_type == CacheType.MONGO_CACHE:
         precursor_set = set([s.entry_id for s in precursor_library])
         similarities = {}
         for s in mongo_results_generator(target, 'similarity'):
             if "similarity" not in s.keys():
                 print(f"Missing 'similarity' at:\n {s}")
                 continue
             for material_id in s["material_ids"]:
                 if material_id in precursor_set:
                     similarities[material_id] = s["similarity"]
 
     else:
         precursor_structures = [s.structure for s in precursor_library]
         target_structure = target.structure
-        results = similarity(precursor_structures, target_structure)
+        if cache_type == CacheType.FILE_CACHE:
+            results = through_cache(precursor_structures, target_structure, similarity)
+        else:
+            results = similarity(precursor_structures, target_structure)
+
         similarities = dict(zip([i.entry_id for i in precursor_library], results))
         print("similarity matrix ready")
 
     return similarities
 
 
 def mongo_results_generator(target: ComputedStructureEntry, collection_name: str):
     with MongoClient(settings.mongodb_uri) as mongo_client:
         for result in mongo_client.piro[collection_name].find({"material_ids": target.entry_id}):
             yield result
 
 
-def through_cache_if_enabled(func):
-    @wraps(func)
-    def wrapper(_parents, target):
-        if settings.cache_type == CacheType.FILE_CACHE:
-            return through_cache(_parents, target, func)
-        else:
-            return func(_parents, target)
-    return wrapper
-
-
-def through_cache(_parents, target, func):
+def through_cache(_parents: List[Structure], target: Structure, func):
 
     if not os.path.exists(settings.rxn_files):
         os.mkdir(settings.rxn_files)
 
     cache_path = os.path.join(settings.rxn_files, "_" + func.__name__ + "_cache.json")
     if os.path.isfile(cache_path):
         with open(cache_path, "r") as f:
             db = json.load(f)
     else:
         db = {}
     ordered_pairs = ["_".join(sorted([target.entry_id, i.entry_id])) for i in _parents]
     indices_compt = [i for i in range(len(ordered_pairs)) if ordered_pairs[i] not in db]
 
     if indices_compt:
-        _res = func(np.array(_parents)[indices_compt].tolist(), target)
+        # Don't use numpy here because structures is iterable
+        _res = func([_parents[i] for i in indices_compt], target)
     else:
         _res = []
     results = []
     for i in ordered_pairs:
         if i in db:
             results.append(db[i])
         else:
@@ -128,31 +135,29 @@
             db[i] = _res[indices_compt.index(ordered_pairs.index(i))]
 
     with open(cache_path, "w") as f:
         json.dump(db, f)
     return results
 
 
-@through_cache_if_enabled
-def epitaxy(_parents, target):
+def epitaxy(_parents: List[Structure], target: Structure):
     def _func(s, target):
         sa = SubstrateAnalyzer(film_max_miller=2, substrate_max_miller=2)
         gen = [g for g in sa.calculate(s, target) if g]
         if gen:
             return min([e.match_area for e in gen])
         else:
             return 1000000.0
 
     # Uncomment to debug SA issues
-    return [_func(s, target) for s in _parents]
-    # return Parallel(n_jobs=-1, verbose=1)(delayed(_func)(s, target) for s in _parents)
+    # return [_func(s, target) for s in _parents]
+    return Parallel(n_jobs=-1, verbose=1)(delayed(_func)(s, target) for s in _parents)
 
 
-@through_cache_if_enabled
-def similarity(_parents, target):
+def similarity(_parents: List[Structure], target: Structure):
     featurizer = MultipleFeaturizer(
         [
             SiteStatsFingerprint.from_preset("CoordinationNumber_ward-prb-2017"),
             StructuralHeterogeneity(),
             ChemicalOrdering(),
             MaximumPackingEfficiency(),
             SiteStatsFingerprint.from_preset("LocalPropertyDifference_ward-prb-2017"),
@@ -185,15 +190,15 @@
     x_parent = x_parent.reindex(sorted(x_parent.columns), axis=1)
 
     with open(os.path.join(settings.rxn_files, "scaler2.pickle"), "rb") as f:
         scaler = pickle.load(f)
     with open(os.path.join(settings.rxn_files, "quantiles.pickle"), "rb") as f:
         quantiles = pickle.load(f)
 
-    X = scaler.transform(x_parent.append(x_target))
+    X = scaler.transform(pd.concat([x_parent, x_target], axis=0))
 
     D = [pairwise_distances(np.array([row, X[-1]]))[0, 1] for row in X[:-1]]
 
     _res = []
     for d in D:
         _res.append(np.linspace(0, 1, 101)[np.abs(quantiles - d).argmin()])
     _res = np.array(_res)
```

### Comparing `piro-2022.10.18/piro.egg-info/PKG-INFO` & `piro-2023.4.24/piro.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: piro
-Version: 2022.10.18
+Version: 2023.4.24
 Summary: piro is software designed to assist in planning of synthesis pathways for inorganics
 Author: AMDD - Toyota Research Institute
 Author-email: murat.aykol@tri.global
 Maintainer: Joseph Montoya
 Maintainer-email: joseph.montoya@tri.global
 Keywords: materials,battery,chemistry,science,density functional theory,energy,AI,artificial intelligence,sequential learning,active learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: m3gnet
 License-File: LICENSE
 
 
 The piro software package enables prediction and planning of synthesis pathways
 and determination of pareto-optimal frontiers for synthesis of
 specific inorganic materials.
```

### Comparing `piro-2022.10.18/setup.cfg` & `piro-2023.4.24/setup.cfg`

 * *Files identical despite different names*

### Comparing `piro-2022.10.18/setup.py` & `piro-2023.4.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 The piro software package enables prediction and planning of synthesis pathways
 and determination of pareto-optimal frontiers for synthesis of
 specific inorganic materials.
 """
 
 setup(
     name="piro",
-    version="2022.10.18",
+    version="2023.4.24",
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    install_requires=["matminer==0.7.8",
-                      "plotly==5.6.0",
-                      "pymongo==4.1.1",
+    install_requires=["matminer==0.8.0",
+                      "plotly==5.11.0",
+                      "pymongo==3.12.0",
                       ],
     classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
     ],
     extras_require={
         "tests": ["pytest",
                   "pytest-cov",
                   "coveralls"
-                  ]
+                  ],
+        "m3gnet": ["m3gnet==0.2.4"]
     },
     package_data={
         "piro": ["*.pickle", "*.json"]
     },
     include_package_data=True,
     author="AMDD - Toyota Research Institute",
     author_email="murat.aykol@tri.global",
```

