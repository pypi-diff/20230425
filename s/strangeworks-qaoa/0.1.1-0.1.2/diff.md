# Comparing `tmp/strangeworks_qaoa-0.1.1.tar.gz` & `tmp/strangeworks_qaoa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.1.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.2.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.1.tar` & `strangeworks_qaoa-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/LICENSE
--rw-r--r--   0        0        0      576 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/README.md
--rw-r--r--   0        0        0      792 2023-04-18 11:14:10.737308 strangeworks_qaoa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      128 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    15787 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    10780 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 11:25:54.241258 strangeworks_qaoa-0.1.2/LICENSE
+-rw-r--r--   0        0        0      576 2023-04-25 11:25:54.241258 strangeworks_qaoa-0.1.2/README.md
+-rw-r--r--   0        0        0      792 2023-04-25 11:26:08.277460 strangeworks_qaoa-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    16286 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    10892 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.2/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.1/LICENSE` & `strangeworks_qaoa-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.1/README.md` & `strangeworks_qaoa-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.1/pyproject.toml` & `strangeworks_qaoa-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_qaoa-0.1.1/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.2/strangeworks_qaoa/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Optional
 
 import dimod
 import networkx as nx
 import numpy as np
 import qiskit
 import strangeworks
@@ -139,14 +140,17 @@
                                 simulation with classical outputs
                 theta0 (array): Optional, initial vector of parameters.
                 optimizer (str): Optional, string specifying classical optimizer,
                                 default='SPSA'.
                 ansatz (str or QuantumCircuit): Optional, Variational circuit
                                                 parametrized with coefficients to
                                                 optimise for the energy
+                ising (bool): Optional, If True then the input problem is treated as
+                                    an Ising problem. If False or unspecified, then the
+                                    input problem is treated as a QUBO problem.
                 problem_type (str): Optional, If the problem is a quantum encoding of a
                 classical problem (i.e. the solution is one of the basis states)
                                     then we can make some simplifications and employ
                                     some tricks to make the algorithm potentially more
                                     optimal.
                 optimization_level: IBM only. How much optimization to perform on the
                                     circuits.
@@ -212,15 +216,16 @@
                 ibm = True
                 channel = "ibm_quantum"
                 backend_id = self.backend_list["IBM_Sim"][nn]["backend_name"]
 
         if ibm is False and aws is False:
             raise StrangeworksError("Unable to Find Backend")
 
-        # Check which format the problem is specified in and convert to the form which our QUBO solver can accept.
+        # Check which format the problem is specified in and convert to the form which
+        # our QUBO solver can accept.
         if type(problem) == nx.classes.graph.Graph:
             H = utils.get_Ham_from_graph(problem)
         elif type(problem) == qiskit.opflow.primitive_ops.pauli_sum_op.PauliSumOp:
             H = utils.get_Ham_from_PauliSumOp(problem)
         elif type(problem) == np.ndarray:
             H = utils.get_Ham_from_QUBO(problem)
         elif (
@@ -237,14 +242,19 @@
             raise StrangeworksError("Problem not in currently supported format")
 
         problem_params["H"] = serializer.pickle_serializer(H, "json")
         problem_params["nqubits"] = str(len(H[0][1]))
         problem_params["theta0"] = (
             str(problem_params.get("theta0")) if problem_params.get("theta0") else None
         )
+        problem_params["ising"] = (
+            json.dumps(problem_params["ising"])
+            if problem_params.get("ising")
+            else json.dumps(False)
+        )
 
         if aws is True:
             input_params = {
                 "provider": "aws",
                 "dev_str": backend_id,
                 "hyperparams": problem_params,
             }
@@ -312,16 +322,19 @@
                 self.rsc, {"payload": {"job_slug": job_slug}}, "get_inputs_url"
             )
             inputs = strangeworks.download_job_files([inputs_url])[0]
 
             H = serializer.pickle_deserializer(inputs["H"], "json")
 
             try:
-                # En_exact = utils.get_exact_en(utils.get_PauliSumOp_from_Ham(H), len(H[0][1]))
-                En_exact = utils.get_exact_en(utils.get_graph_from_Ham(H), len(H[0][1]))
+                En_exact = utils.get_exact_en(
+                    utils.get_graph_from_Ham(H),
+                    len(H[0][1]),
+                    ising=json.loads(inputs["ising"]) if inputs.get("ising") else False,
+                )
             except:
                 En_exact = "!!problem too big for exact solution!!"
             result_file["En_exact"] = En_exact
         else:
             result_file["En_exact"] = None
 
         if display_results:
```

### Comparing `strangeworks_qaoa-0.1.1/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.2/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.1/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.2/strangeworks_qaoa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,15 @@
             Ham = H[nn][0] * temp
         else:
             Ham = Ham + H[nn][0] * temp
 
     return Ham
 
 
-def get_exact_en(G, nodes):
+def get_exact_en(G, nodes, ising=False):
 
     if nodes > 24:
         Egs_exact = "!!problem too big for exact solution!!"
     else:
 
         edges = np.zeros((len(G.edges()), 2), dtype=int)
         we = np.zeros(len(G.edges()), dtype=float)
@@ -415,15 +415,18 @@
 
             out = np.kron(A[0], A[1])
             for oo in range(2, len(A)):
                 out = np.kron(out, A[oo])
 
             return out
 
-        sz = [[1.0, 0.0], [0.0, 0.0]]
+        if ising is True:
+            sz = [[1.0 / 2.0, 0.0], [0.0, -1.0 / 2.0]]
+        else:
+            sz = [[1.0, 0.0], [0.0, 0.0]]
 
         A0 = []
         for n in range(0, nodes):
             A0.append(np.eye(2))
 
         Ham = np.zeros((np.power(2, nodes), np.power(2, nodes)), dtype=float)
         for p in range(0, nodes):
```

### Comparing `strangeworks_qaoa-0.1.1/PKG-INFO` & `strangeworks_qaoa-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

