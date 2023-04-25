# Comparing `tmp/hwave-0.2.tar.gz` & `tmp/hwave-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwave-0.2.tar", max compression
+gzip compressed data, was "hwave-1.0.0.tar", max compression
```

## Comparing `hwave-0.2.tar` & `hwave-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-02-17 04:34:29.380231 hwave-0.2/LICENSE
--rw-r--r--   0        0        0     2067 2023-02-17 04:34:29.380231 hwave-0.2/README.md
--rw-r--r--   0        0        0      600 2023-02-17 04:34:29.400231 hwave-0.2/pyproject.toml
--rw-r--r--   0        0        0       20 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/__init__.py
--rw-r--r--   0        0        0     4247 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/qlms.py
--rw-r--r--   0        0        0       52 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/qlmsio/__init__.py
--rw-r--r--   0        0        0     4269 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/qlmsio/read_input.py
--rw-r--r--   0        0        0     5111 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/qlmsio/read_input_k.py
--rw-r--r--   0        0        0     4490 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/qlmsio/wan90.py
--rw-r--r--   0        0        0        1 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/solver/__init__.py
--rw-r--r--   0        0        0     5510 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/solver/base.py
--rw-r--r--   0        0        0     1587 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/solver/perf.py
--rw-r--r--   0        0        0    52751 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/solver/uhfk.py
--rw-r--r--   0        0        0    29242 2023-02-17 04:34:29.400231 hwave-0.2/src/hwave/solver/uhfr.py
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 hwave-0.2/setup.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hwave-0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 08:12:40.035518 hwave-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2327 2023-04-25 08:12:40.035518 hwave-1.0.0/README.md
+-rw-r--r--   0        0        0      631 2023-04-25 08:12:40.063518 hwave-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/__init__.py
+-rw-r--r--   0        0        0     5574 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/dos.py
+-rw-r--r--   0        0        0     5037 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/qlms.py
+-rw-r--r--   0        0        0       52 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/qlmsio/__init__.py
+-rw-r--r--   0        0        0     4269 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/qlmsio/read_input.py
+-rw-r--r--   0        0        0     5121 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/qlmsio/read_input_k.py
+-rw-r--r--   0        0        0     4490 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/qlmsio/wan90.py
+-rw-r--r--   0        0        0        1 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/__init__.py
+-rw-r--r--   0        0        0     7520 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/base.py
+-rw-r--r--   0        0        0     1643 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/perf.py
+-rw-r--r--   0        0        0    55143 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/rpa.py
+-rw-r--r--   0        0        0    57169 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/uhfk.py
+-rw-r--r--   0        0        0    29474 2023-04-25 08:12:40.067519 hwave-1.0.0/src/hwave/solver/uhfr.py
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 hwave-1.0.0/PKG-INFO
```

### Comparing `hwave-0.2/LICENSE` & `hwave-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hwave-0.2/README.md` & `hwave-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # H-wave
 
-H-wave is a program for performing unrestricted Hartree-Fock (UHF) approximation
-for itinerant electron systems.
-The UHF method approximates two-body interaction terms into one-body ones by
-taking account of the fluctuations up to the first order. The wave functions
-and energies are determined self-consistently by an iterative method.
-H-wave treats two types of UHF approximation: one is real-space and the other is
-wavenumber-space UHF methods using translational symmetry. In the wavenumber space
-UHF method, the input file defining the one-body and two-body interactions is
-based on the Wannier90 format, and the program can be smoothly connected to
-the softwares for deriving effective models from first-principles calculations.
+H-wave is a program for performing unrestricted Hartree-Fock (UHF) approximation and random phase approximation (RPA) for itinerant electron systems. UHF and RPA correspond to simple approximations that deal with fluctuations up to first order and enable analyses of electron correlation effects in materials at a low computational cost. The input files describing the one-body and two-body interactions are based on the Wannier90 format[1]. This allows smooth connection for the software packages that derive the effective models from first principles calculations, such as RESPACK[2], to the analyses of the effective model with H-wave.
+
+[1] G. Pizzi et al, J. Phys.: Condens. Matter 32 165902 (2020).
+[2] K. Nakmura, Y. Yoshimoto, Y. Nomura et al., Comp. Phys. Commun. 261, 107781 (2021).
+
 
 ## Methods
 
-Hartree-Fock approximation
+Hartree-Fock and Random Phase approximation
 
 ## Target models
 
 Hubbard model, multi-orbital Hubbard model
 
 ## Available physical quantities
 
-ground-state energy, free energy, etc.
+ground-state energy, free energy, charge and spin susceptibilities, etc.
 
 ## Requirement
 
 Python3 with numpy, scipy, and other library packages
 
 ## Install
 
@@ -54,19 +49,19 @@
 of The Institute for Solid State Physics, The University of Tokyo.
 
 ## Official page
 
 - [H-wave project site](https://www.pasums.issp.u-tokyo.ac.jp/h-wave/en)
 - [Software repository](https://github.com/issp-center-dev/H-wave)
 - [User Manual](https://www.pasums.issp.u-tokyo.ac.jp/h-wave/en/doc/manual)
-- [Samples/Tutorials](https://isspns-gitlab.issp.u-tokyo.ac.jp/hwave-dev/hwave-gallery)
+- [Data Repository](https://datarepo.mdcl.issp.u-tokyo.ac.jp/repo/23)
 
 ## Authors
 
-Kazuyoshi Yoshimi,
-Yuichi Motoyama,
-Tatsumi Aoyama,
-Kota Ido,
-Takahiro Misawa,
-Taiki Kawamura
-Akito Kobayashi,
-Takeo Kato
+Kazuyoshi Yoshimi (ISSP, Univ. of Tokyo),
+Yuichi Motoyama (ISSP, Univ. of Tokyo),
+Tatsumi Aoyama (ISSP, Univ. of Tokyo),
+Kota Ido (ISSP, Univ. of Tokyo),
+Takahiro Misawa (ISSP, Univ. of Tokyo),
+Taiki Kawamura (Nagoya Univ.),
+Akito Kobayashi (Nagoya Univ.),
+Takeo Kato (ISSP, Univ. of Tokyo)
```

### Comparing `hwave-0.2/pyproject.toml` & `hwave-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwave"
-version = "0.2"
+version = "1.0.0"
 description = "UHF"
 authors = ["H-Wave developers <hwave-dev@issp.u-tokyo.ac.jp>"]
 license = "GPL-3.0-or-later"
 
 readme = "README.md"
 repository = "https://github.com/issp-center-dev/H-Wave"
 
@@ -21,11 +21,12 @@
 
 [tool.poetry.extras]
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 hwave = "hwave.qlms:main"
+hwave_dos = "hwave.dos:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hwave-0.2/src/hwave/qlms.py` & `hwave-1.0.0/src/hwave/qlms.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import sys
 import os
 # import pprint
 import logging
 
 import tomli
 
+import hwave
 import hwave.qlmsio as qlmsio
 import hwave.solver.uhfr as sol_uhfr
 import hwave.solver.uhfk as sol_uhfk
+import hwave.solver.rpa as sol_rpa
 from requests.structures import CaseInsensitiveDict
 
 def run(*, input_dict: Optional[dict] = None, input_file: Optional[str] = None):
     if input_dict is None:
         if input_file is None:
             raise RuntimeError("Neither input_dict nor input_file are passed")
         with open(input_file, "rb") as f:
@@ -91,25 +93,48 @@
         logger.info("Get Green function information")
         green_info = read_io.get_param("green")
 
         # pprint.pprint(info_mode, width=1)
 
         solver = sol_uhfk.UHFk(ham_info, info_log, info_mode)
 
+    elif mode == "RPA":
+        logger.info("RPA mode")
+
+        logger.info("Read interaction definitions from files")
+        read_io = qlmsio.read_input_k.QLMSkInput(info_inputfile)
+        ham_info = read_io.get_param("ham")
+
+        solver = sol_rpa.RPA(ham_info, info_log, info_mode)
+
+        green_info = read_io.get_param("green")
+        green_info.update( solver.read_init(info_inputfile) )
+
     else:
         logger.warning("mode is incorrect: mode={}.".format(mode))
         exit(0)
 
     logger.info("Start UHF calculation")
     solver.solve(green_info, path_to_output)
     logger.info("Save calculation results.")
     solver.save_results(info_outputfile, green_info)
     logger.info("All procedures are finished.")
 
 
 def main():
-    args = sys.argv
-    if len(args) != 2:
-        print("Usage: python3 qlms.py input.toml")
-        exit(1)
-    run(input_file=args[1])
+    import argparse
+
+    parser = argparse.ArgumentParser(prog='hwave')
+    parser.add_argument('input_toml', nargs='?', default=None, help='input parameter file')
+    parser.add_argument('--version', action='store_true', help='show version')
+
+    args = parser.parse_args()
+
+    if args.version:
+        print('hwave', hwave.__version__)
+        sys.exit(0)
+
+    if args.input_toml is None:
+        parser.print_help()
+        sys.exit(1)
 
+    run(input_file = args.input_toml)
```

### Comparing `hwave-0.2/src/hwave/qlmsio/read_input.py` & `hwave-1.0.0/src/hwave/qlmsio/read_input.py`

 * *Files identical despite different names*

### Comparing `hwave-0.2/src/hwave/qlmsio/read_input_k.py` & `hwave-1.0.0/src/hwave/qlmsio/read_input_k.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from requests.structures import CaseInsensitiveDict
 from . import wan90
 
 logger = logging.getLogger("qlms").getChild("read_input")
 
 
 class QLMSkInput():
-    valid_namelist = [s.lower() for s in ["path_to_input", "Geometry", "Transfer", "CoulombIntra", "CoulombInter", "Hund", "Ising", "PairLift", "Exchange", "PairHop"]]
+    valid_namelist = [s.lower() for s in ["path_to_input", "Geometry", "Transfer", "CoulombIntra", "CoulombInter", "Hund", "Ising", "PairLift", "Exchange", "PairHop", "Extern"]]
 
     def __init__(self, info_inputfile, solver_type="UHFk"):
         logger.debug(">>> QLMSkInput init")
 
         # [file.input]
         #   path_to_input
         #   initial
```

### Comparing `hwave-0.2/src/hwave/qlmsio/wan90.py` & `hwave-1.0.0/src/hwave/qlmsio/wan90.py`

 * *Files identical despite different names*

### Comparing `hwave-0.2/src/hwave/solver/base.py` & `hwave-1.0.0/src/hwave/solver/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import logging
+import sys
 from requests.structures import CaseInsensitiveDict
-
 # from pprint import pprint
 
+import logging
+logger = logging.getLogger("qlms").getChild("solver")
+
 class solver_base():
     def __init__(self, param_ham, info_log, info_mode, param_mod=None):
         logger = logging.getLogger("qlms").getChild(self.name)
 
         self.param_mod = param_mod
         self.param_ham = param_ham
         self.info_log = info_log
@@ -28,15 +30,15 @@
             "ene_cutoff": 1.0e+2,
         })
 
         range_list = {
             "T":     [ 0, None ],
             # "2Sz":   [ -param_mod["Nsite"], param_mod["Nsite"] ],
             # "Nsite": [ 1, None ],
-            "Ncond": [ 1, None ],
+            # "Ncond": [ 1, None ],
             "IterationMax": [ 0, None ],
             "Mix":   [ 0.0, 1.0 ],
             # "print_step": [ 1, None ],
             "EPS":   [ 0, None ],
         }
 
         if param_mod is not None:
@@ -61,34 +63,57 @@
                 self.param_mod[key] = value
 
         # relax parameter checks
         self.relax_checks = self.param_mod.get("trustme_interaction_range", False)
         if self.relax_checks:
             logger.warning("TRUST-ME mode enabled. parameter checks are relaxed")
 
+        # Sz mode
         if "2Sz" in self.param_mod and self.param_mod["2Sz"] == "free":
             self.param_mod["2Sz"] = None
 
+        # Ncond and filling
+        if "Nelec" in self.param_mod:
+            if self.param_mod["Ncond"] > 0:
+                logger.warning("Both Ncond and Nelec are specified: Ncond used")
+            else:
+                self.param_mod["Ncond"] = self.param_mod["Nelec"]
+
+        if "filling" in self.param_mod:
+            if self.param_mod["Ncond"] > 0:
+                logger.error("Both Ncond and filling are specified.")
+                sys.exit(1)
+            else:
+                filling = self.param_mod["filling"]
+                if filling < 0.0 or filling > 1.0:
+                    logger.error("Parameter range check failed for filling")
+                    sys.exit(1)
+        else:
+            if self.param_mod["Ncond"] == 0:
+                logger.error("Neigher Ncond nor filling is specified.")
+                sys.exit(1)
+
+        # checks
         if self._check_info_mode(info_mode) != 0:
             logger.error("Parameter check failed for info_mode.")
-            exit(1)
+            sys.exit(1)
         if self._check_param_range(self.param_mod, range_list) != 0:
             msg = "Parameter range check failed for param_mod."
             if self.relax_checks:
                 logger.warning(msg)
             else:
                 logger.error(msg)
-                exit(1)
+                sys.exit(1)
         if self._check_param_mod(self.param_mod) != 0:
             msg = "Parameter check failed for param_mod."
             if self.relax_checks:
                 logger.warning(msg)
             else:
                 logger.error(msg)
-                exit(1)
+                sys.exit(1)
 
         # canonicalize
         self.param_mod["EPS"] = pow(10, -self.param_mod["EPS"])
 
         # debug
         # pprint(self.param_mod)
 
@@ -136,14 +161,45 @@
                     logger.warning("mode.param.{} must be greater than {}.".format(key, vmin))
                     error_code += 1
                 if vmax is not None and param_mod[key] > vmax:
                     logger.warning("mode.param.{} must be smaller than {}.".format(key, vmax))
                     error_code += 1
         return error_code
 
+    def _round_to_int(self, val, mode):
+        import math
+        mode = mode.lower()  # case-insensitive
+        if   mode == "as-is":
+            ret = val  # not rounding to int
+        elif mode == "round":
+            ret = round(val)
+        elif mode == "round-up":
+            ret = math.ceil(val)
+        elif mode == "round-down":
+            ret = math.floor(val)
+        elif mode == "round-to-zero":
+            ret = int(val)
+        elif mode == "round-off":
+            nn = math.floor(val)
+            rr = val - nn
+            ret = nn if rr < 0.5 else nn+1
+        elif mode == "strict":
+            if val != round(val):
+                logger.error("value not integer")
+                sys.exit(1)
+            ret = round(val)
+        elif mode == "exact":  # "round" with warning
+            if val != round(val):
+                logger.warning("value not integer")
+            ret = round(val)
+        else:
+            logger.error("round_to_int: unknown mode {}".format(mode))
+            sys.exit(1)
+        return ret
+
     def solve(self, path_to_output):
         pass
 
     def get_results(self):
         return (self.physics, self.Green)
 
     def save_results(self, info_outputfile, green_info):
```

### Comparing `hwave-0.2/src/hwave/solver/perf.py` & `hwave-1.0.0/src/hwave/solver/perf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import time
 
 class PerfDB:
     def __init__(self):
         self._db_count = {}
         self._db_value = {}
     def __del__(self):
+        if len(self._db_count) == 0:
+            return
         print("--------------------------------------------------------------------------------")
         print("Statistics")
         print("  function                         :  total elapsed  : average elapsed : ncalls")
         print("--------------------------------------------------------------------------------")
         for item in self._db_count.keys():
             print("  {:32s} : {:10.3f} msec : {:10.3f} msec : {:6d}".format(
                 item,
```

### Comparing `hwave-0.2/src/hwave/solver/uhfk.py` & `hwave-1.0.0/src/hwave/solver/uhfk.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,61 +31,73 @@
             "NCond": 0.0,
             "Sz": 0.0,
             "Rest": 1.0
         }
 
         nvol = self.nvol
         nd = self.nd
-        
+
         self._green_list = {
 #            "eigenvalue":  np.zeros((nvol,nd), dtype=np.complex128),
 #            "eigenvector": np.zeros((nvol,nd,nd), dtype=np.complex128)
         }
 
         #self.Green = np.zeros((nvol,ns,norb,ns,norb), dtype=np.complex128),
 
         # work area
         self.ham = np.zeros((nvol,nd,nd), dtype=np.complex128)
 
     def _init_mode(self, param):
         self.iflag_fock = param.get('flag_fock', True)
+        self.enable_spin_orbital = param.get('enable_spin_orbital', False)
 
     @do_profile
     def _init_param(self):
         # check and store parameters
-        
+
+        # - cell shape
         if not "CellShape" in self.param_mod:
             logger.error("CellShape is missing. abort")
             exit(1)
 
-        if "Ncond" in self.param_mod:
-            ncond = self.param_mod["Ncond"]
-        elif "Nelec" in self.param_mod:
-            ncond = self.param_mod["Nelec"]
-        else:
-            logger.error("Ncond or Nelec is missing. abort")
-            exit(1)
+        # - temperature
+        self.T = self.param_mod.get("T", 0.0)
 
-        # self.Ncond = ncond
+        # - number of electrons
+        if "filling" in self.param_mod:
+            self.filling = self.param_mod["filling"]
+            round_mode = self.param_mod.get("Ncond_round_mode", "strict")
+
+            Lx,Ly,Lz = self.param_mod.get("CellShape")
+            norb = self.param_ham["Geometry"]["norb"]
+            Nstate = Lx*Ly*Lz*norb*2
 
+            ncond = self._round_to_int(Nstate * self.filling, round_mode)
+            self.param_mod["Ncond"] = ncond  # overwrite
+        else:
+            self.filling = None
+            ncond = self.param_mod["Ncond"]
+
+        # - Sz fixed or free
         if self.param_mod["2Sz"] is None:
             self.sz_free = True
             self.Nconds = [ ncond ]
         else:
             self.sz_free = False
             twosz = self.param_mod["2Sz"]
             self.Nconds = [ (ncond + twosz)//2, (ncond - twosz)//2 ]
 
-        self.T = self.param_mod.get("T", 0.0)
+        # - calc condition
         self.ene_cutoff = self.param_mod.get("ene_cutoff", 1e+2)
 
-        # strict hermiticity check
+        # - strict hermiticity check
         self.strict_hermite = self.param_mod.get("strict_hermite", False)
         self.hermite_tolerance = self.param_mod.get("hermite_tolerance", 1.0e-8)
 
+        # - check strictness
         if self.relax_checks:
             self.strict_hermite = False
 
     @do_profile
     def _init_lattice(self):
         Lx,Ly,Lz = self.param_mod.get("CellShape")
         self.cellshape = (Lx,Ly,Lz)
@@ -136,25 +148,29 @@
         logger.info("    Block volume   = {}".format(self.nvol))
         logger.info("    Num orbit      = {}".format(self.norb_orig))
         logger.info("    Num orbit eff  = {}".format(self.norb))
         logger.info("    nspin          = {}".format(self.ns))
         logger.info("    nd             = {}".format(self.nd))
 
         logger.info("    Ncond          = {}".format(self.Nconds))
+        if self.filling is not None:
+            logger.info("    filling        = {}".format(self.filling))
         logger.info("    T              = {}".format(self.T))
         logger.info("    E_cutoff       = {}".format(self.ene_cutoff))
 
         logger.info("    Mix            = {}".format(self.param_mod["Mix"]))
         logger.info("    RndSeed        = {}".format(self.param_mod["RndSeed"]))
         logger.info("    IterationMax   = {}".format(self.param_mod["IterationMax"]))
         logger.info("    EPS            = {}".format(self.param_mod["EPS"]))
         logger.info("    2Sz            = {}".format(self.param_mod["2Sz"]))
         logger.info("    strict_hermite = {}".format(self.strict_hermite))
         logger.info("    hermite_tol    = {}".format(self.hermite_tolerance))
 
+        logger.info("    spin_orbital   = {}".format(self.enable_spin_orbital))
+
     @do_profile
     def _reshape_geometry(self, geom):
         Bx,By,Bz = self.subshape
         bvol = Bx * By * Bz
 
         norb = geom['norb']
 
@@ -172,21 +188,32 @@
                 centerv[k] = cw[i] + np.array([bx, by, bz]) * sc
                 k += 1
         geom_new['center'] = centerv
 
         return geom_new
 
     @do_profile
-    def _reshape_interaction(self, ham):
+    def _reshape_interaction(self, ham, enable_spin_orbital):
         Bx,By,Bz = self.subshape
         nx,ny,nz = self.shape
 
-        def _reshape_orbit(a, x):
+        norb_orig = self.param_ham_orig["Geometry"]["norb"]
+
+        def _reshape_orbit_(a, x):
             return a + self.norb_orig * ( x[0] + Bx * (x[1] + By * (x[2])))
 
+        def _reshape_orbit_spin(a, x):
+            a_, s_ = a%norb_orig, a//norb_orig
+            return a_ + norb_orig * ( x[0] + Bx * (x[1] + By * (x[2] + Bz * s_)))
+
+        if enable_spin_orbital:
+            _reshape_orbit = _reshape_orbit_spin
+        else:
+            _reshape_orbit = _reshape_orbit_
+
         def _round(x, n):
             return x % n if x >= 0 else x % -n
 
         ham_new = {}
         for (irvec,orbvec), v in ham.items():
             rx,ry,rz = irvec
             alpha,beta = orbvec
@@ -208,17 +235,17 @@
                 # find orbital index within supercell
                 aa = _reshape_orbit(alpha,(x0,y0,z0))
                 bb = _reshape_orbit(beta, (xr1,yr1,zr1))
 
                 # check wrap-around: maybe overwritten by duplicate entries
                 ir = (_round(xx1, nx), _round(yy1, ny), _round(zz1, nz))
                 ov = (aa, bb)
-                
+
                 ham_new[(ir, ov)] = v
-        
+
         return ham_new
 
     @do_profile
     def _reshape_green(self, green):
         # convert green function into sublattice
 
         Lx,Ly,Lz = self.cellshape
@@ -243,32 +270,44 @@
         def _unpack_index(x, n):
             _nx, _ny, _nz = n
             _ix = x % _nx
             _iy = (x // _nx) % _ny
             _iz = (x // (_nx * _ny)) % _nz
             return (_ix, _iy, _iz)
 
+        def _pack_site(x, n):
+            _ix, _iy, _iz = x
+            _nx, _ny, _nz = n
+            return _iz + _nz * (_iy + _ny * (_ix))
+
+        def _unpack_site(idx, n):
+            _nx, _ny, _nz = n
+            _iz = idx % _nz
+            _iy = (idx // _nz) % _ny
+            _ix = (idx // (_nz * _ny)) % _nx
+            return (_ix,_iy,_iz)
+
         green_sub = np.zeros((Nvol,ns,norb,ns,norb), dtype=np.complex128)
 
         for isite in range(Nvol):
-            ixx, iyy, izz = _unpack_index(isite, (Nx,Ny,Nz))
+            ixx, iyy, izz = _unpack_site(isite, (Nx,Ny,Nz))
             ix0, iy0, iz0 = ixx * Bx, iyy * By, izz * Bz
 
             for aa, bb in itertools.product(range(norb), range(norb)):
                 a, ri = aa % norb_orig, aa // norb_orig
                 b, rj = bb % norb_orig, bb // norb_orig
 
                 rix, riy, riz = _unpack_index(ri, (Bx,By,Bz))
                 rjx, rjy, rjz = _unpack_index(rj, (Bx,By,Bz))
 
                 ix = (ix0 + rjx - rix) % Lx
                 iy = (iy0 + rjy - riy) % Ly
                 iz = (iz0 + rjz - riz) % Lz
 
-                jsite = _pack_index((ix,iy,iz), (Lx,Ly,Lz))
+                jsite = _pack_site((ix,iy,iz), (Lx,Ly,Lz))
 
                 for s, t in itertools.product(range(ns), range(ns)):
                     green_sub[isite, s, aa, t, bb] = green[jsite, s, a, t, b]
 
         return green_sub
 
     @do_profile
@@ -293,24 +332,36 @@
         def _unpack_index(x, n):
             _nx, _ny, _nz = n
             _ix = x % _nx
             _iy = (x // _nx) % _ny
             _iz = (x // (_nx * _ny)) % _nz
             return (_ix, _iy, _iz)
 
+        def _pack_site(x, n):
+            _ix, _iy, _iz = x
+            _nx, _ny, _nz = n
+            return _iz + _nz * (_iy + _ny * (_ix))
+
+        def _unpack_site(idx, n):
+            _nx, _ny, _nz = n
+            _iz = idx % _nz
+            _iy = (idx // _nz) % _ny
+            _ix = (idx // (_nz * _ny)) % _nx
+            return (_ix,_iy,_iz)
+
         green = np.zeros((Lvol,ns,norb_orig,ns,norb_orig), dtype=np.complex128)
 
         for jsite in range(Lvol):
-            ix, iy, iz = _unpack_index(jsite, (Lx,Ly,Lz))
+            ix, iy, iz = _unpack_site(jsite, (Lx,Ly,Lz))
 
             ixx, irx = ix // Bx, ix % Bx
             iyy, iry = iy // By, iy % By
             izz, irz = iz // Bz, iz % Bz
 
-            isite = _pack_index((ixx,iyy,izz), (Nx,Ny,Nz))
+            isite = _pack_site((ixx,iyy,izz), (Nx,Ny,Nz))
             ir = _pack_index((irx,iry,irz), (Bx,By,Bz))
 
             for a, b in itertools.product(range(norb_orig), range(norb_orig)):
                 aa = a
                 bb = b + norb_orig * ir
                 for s, t in itertools.product(range(ns), range(ns)):
                     green[jsite, s, a, t, b] = green_sub[isite, s, aa, t, bb]
@@ -318,28 +369,29 @@
         return green
 
     @do_profile
     def _init_interaction(self):
         # reinterpret interaction coefficient on sublattice
         if self.has_sublattice:
             # backup
-            self.param_ham_orig = {}
+            import copy
+            self.param_ham_orig = copy.deepcopy(self.param_ham)
 
+            # replace by sublatticed versions
             for type in self.param_ham.keys():
                 if type in ["Initial"]:
                     pass
                 elif type in ["Geometry"]:
-                    self.param_ham_orig[type] = self.param_ham[type]
                     tbl = self._reshape_geometry(self.param_ham[type])
-                    # replace
+                    self.param_ham[type] = tbl
+                elif type in ["Transfer"]:
+                    tbl = self._reshape_interaction(self.param_ham[type], self.enable_spin_orbital)
                     self.param_ham[type] = tbl
                 else:
-                    self.param_ham_orig[type] = self.param_ham[type]
-                    tbl = self._reshape_interaction(self.param_ham[type])
-                    # replace
+                    tbl = self._reshape_interaction(self.param_ham[type], False)
                     self.param_ham[type] = tbl
 
     def _init_wavevec(self):
         # wave vectors on sublatticed geometry
         def _klist(n):
             return np.roll( (np.arange(n)-(n//2)), -(n//2) )
 
@@ -429,23 +481,43 @@
 
     def _check_orbital_index(self):
         norb = self.param_ham["Geometry"]["norb"]
         err = 0
         for k in self.param_ham.keys():
             if k in ["Geometry", "Initial"]:
                 pass
+            elif k == "Transfer":
+                fail = 0
+                for (irvec,orbvec), v in self.param_ham[k].items():
+                    # allow spin-orbital interaction, i.e. twice norb
+                    if not all([ 0 <= orbvec[i] < norb*2 for i in range(2) ]):
+                        fail += 1
+                if fail > 0:
+                    logger.error("orbital index check failed for {}.".format(k))
+                    err += 1
+                else:
+                    logger.debug("orbital index check for {} ok.".format(k))
+            elif k == "CoulombIntra":
+                fail = 0
+                for (irvec,orbvec), v in self.param_ham[k].items():
+                    if not all([ 0 <= orbvec[i] < norb for i in range(2) ]):
+                        fail += 1
+                for (irvec,orbvec), v in self.param_ham[k].items():
+                    if not orbvec[0] == orbvec[1]:
+                        fail += 1
+                if fail > 0:
+                    logger.error("orbital index check failed for {}.".format(k))
+                    err += 1
+                else:
+                    logger.debug("orbital index check for {} ok.".format(k))
             else:
                 fail = 0
                 for (irvec,orbvec), v in self.param_ham[k].items():
                     if not all([ 0 <= orbvec[i] < norb for i in range(2) ]):
                         fail += 1
-                if k == "CoulombIntra":
-                    for (irvec,orbvec), v in self.param_ham[k].items():
-                        if not orbvec[0] == orbvec[1]:
-                            fail += 1
                 if fail > 0:
                     logger.error("orbital index check failed for {}.".format(k))
                     err += 1
                 else:
                     logger.debug("orbital index check for {} ok.".format(k))
         if err > 0:
             logger.error("_check_orbital_index failed. invalid orbital index found in interaction definitions.")
@@ -523,25 +595,25 @@
                                   self.physics["Ene"]["Total"],
                                   self.physics["NCond"],
                                   self.physics["Sz"]))
 
             if self.physics["Rest"] < self.param_mod["eps"]:
                 is_converged = True
                 break
-            
+
         if is_converged:
             logger.info("UHFk calculation succeeded: rest={}, eps={}."
                         .format(self.physics["Rest"], self.param_mod["eps"]))
             logger.info("Total Energy = {}.".format(self.physics["Ene"]["Total"]))
         else:
             logger.info("UHFk calculation failed: rest={}, eps={}."
                         .format(self.physics["Rest"], self.param_mod["eps"]))
         if print_check is not None:
             fch.close()
-            
+
     @do_profile
     def _initial_green(self, green_info):
         logger.debug(">>> _initial_green")
 
         _data = None
         if "initial" in green_info and green_info["initial"] is not None:
             logger.info("load initial green function from file")
@@ -626,36 +698,51 @@
             return self._reshape_green(green_uhf[0])
         else:
             return green_uhf[0]
 
     @do_profile
     def _make_ham_trans(self):
         logger.debug(">>> _make_ham_trans")
-        
+
         nx,ny,nz = self.shape
         nvol     = self.nvol
         norb     = self.norb
         nd       = self.nd
 
-        # data structure of T_ab(r): T(rx,ry,rz,a,b)
-        tab_r = np.zeros((nx,ny,nz,norb,norb), dtype=np.complex128)
+        if self.enable_spin_orbital == True:
+            tab_r = np.zeros((nx,ny,nz,nd,nd), dtype=np.complex128)
 
-        for (irvec,orbvec), v in self.param_ham["Transfer"].items():
-            tab_r[(*irvec, *orbvec)] = v
+            for (irvec,orbvec), v in self.param_ham["Transfer"].items():
+                tab_r[(*irvec, *orbvec)] = v
 
-        # fourier transform
-        tab_k = np.fft.ifftn(tab_r, axes=(0,1,2), norm='forward')
+            # fourier transform
+            tab_k = np.fft.ifftn(tab_r, axes=(0,1,2), norm='forward')
 
-        # 2x2 unit matrix to introduce spin index
-        spin = np.eye(2)
-
-        # T_{a,si,b,sj}(k)
-        ham = np.einsum(
-            'kab, st -> ksatb', tab_k.reshape(nvol,norb,norb), spin
-        ).reshape(nvol,nd,nd)
+            ham = tab_k
+
+        else:
+            # data structure of T_ab(r): T(rx,ry,rz,a,b)
+            tab_r = np.zeros((nx,ny,nz,norb,norb), dtype=np.complex128)
+
+            for (irvec,orbvec), v in self.param_ham["Transfer"].items():
+                if orbvec[0] < norb and orbvec[1] < norb:
+                    tab_r[(*irvec, *orbvec)] = v
+                else:
+                    pass # skip spin dependence
+
+            # fourier transform
+            tab_k = np.fft.ifftn(tab_r, axes=(0,1,2), norm='forward')
+
+            # 2x2 unit matrix to introduce spin index
+            spin = np.eye(2)
+
+            # T_{a,si,b,sj}(k)
+            ham = np.einsum(
+                'kab, st -> ksatb', tab_k.reshape(nvol,norb,norb), spin
+            ).reshape(nvol,nd,nd)
 
         # store
         self.ham_trans = ham
 
     @do_profile
     def _make_ham_inter(self):
         logger.debug(">>> _make_ham_inter")
@@ -666,15 +753,15 @@
         nd       = self.nd
 
         #----------------
         # interaction table
         #----------------
         self.inter_table = {}
         self.spin_table = {}
-        
+
         #----------------
         # Coulomb Intra and Coulomb Inter
         #----------------
         if 'Coulomb' in self.param_ham.keys():
             # assume zvo_ur.dat
             # divide into r=0 (coulomb intra) and r!=0 (coulomb inter)
 
@@ -791,15 +878,15 @@
             self.inter_table["Hund"] = None
 
         #----------------
         # Ising
         #----------------
         if 'Ising' in self.param_ham.keys():
             jab_r = np.zeros((nx,ny,nz,norb,norb), dtype=np.complex128)
-        
+
             for (irvec,orbvec), v in self.param_ham["Ising"].items():
                 jab_r[(*irvec, *orbvec)] = v
 
             # J~ab(r) = Jab(r) + Jba(-r)
             jba = np.conjugate(
                 np.transpose(
                     np.flip(np.roll(jab_r, -1, axis=(0,1,2)), axis=(0,1,2)),
@@ -914,15 +1001,15 @@
 
         # hamiltonian H_{ab,st}(k) : ham(k,(s,a),(t,b))
         ham = np.zeros((nvol,nd,nd), dtype=np.complex128)
 
         # transfer term  T_{ab}(k) (note convention)
         logger.debug("Transfer")
         ham += self.ham_trans
-        
+
         # interaction term: Coulomb type
         for type in ['CoulombIntra', 'CoulombInter', 'Hund', 'Ising', 'PairLift', 'Exchange']:
             if self.inter_table[type] is not None:
                 logger.debug(type)
 
                 # coefficient of interaction term J_{ab}(r)
                 jab_r = self.inter_table[type].reshape(nvol,norb,norb)
@@ -933,15 +1020,15 @@
                 #   sum_r J_{ab}(r) G_{bb,uv}(0) Spin{s,u,v,t}
                 hh0 = np.einsum('uvb, suvt -> stb', gbb, spin)
                 hh1 = np.einsum('rab, stb -> rsta', jab_r, hh0)
                 hh2 = np.einsum('rsta, ab -> rsatb', hh1, np.eye(norb, norb))
                 hh3 = np.sum(hh2, axis=0).reshape(nd,nd)
 
                 ham += np.broadcast_to(hh3, (nvol,nd,nd))
-                
+
                 # cross term
                 #   - sum_r J_{ab}(r) G_{ba,uv}(r) Spin{s,u,t,v} e^{ikr}
                 if self.iflag_fock:
                     hh4 = np.einsum('rab, rubva, sutv -> rsatb', jab_r, gab_r, spin)
 
                     #   fourier transform: sum_r (*) e^{ikr}
                     hh5 = np.fft.ifftn(hh4.reshape(nx,ny,nz,nd,nd), axes=(0,1,2), norm='forward')
@@ -1035,15 +1122,15 @@
             )
 
         # merge spin-diagonal blocks
         gab_k = np.einsum('skab,st->ksatb', np.array(gg), np.eye(ws.shape[0])).reshape(nx,ny,nz,nd,nd)
 
         # G_ab(r) = 1/V sum_k G_ab(k) e^{-ikr}
         gab_r = np.fft.fftn(gab_k, axes=(0,1,2), norm='forward')
-            
+
         # store
         self.Green_prev = self.Green
         self.Green = gab_r.reshape(nvol,ns,norb,ns,norb)
 
     def _find_dist(self, w, v, ncond):
         if self.T == 0:
             return self._find_dist_zero_t(w, v, ncond)
@@ -1185,15 +1272,15 @@
             T = self.T
 
             e_band = 0.0
             for k in range(ws.shape[0]):
                 w = ws[k]
                 v = vs[k]
                 mu = mus[k]
-            
+
                 def _fermi(t, mu, ev):
                     w = (ev - mu) / t
                     mask_ = w < self.ene_cutoff
                     w1 = np.where( mask_, w, 0.0 )
                     v1 = 1.0 / (1.0 + np.exp(w1))
                     v = np.where( mask_, v1, 0.0 )
                     #v = np.where( w > self.ene_cutoff, 0.0, 1.0 / (1.0 + np.exp(w)) )
@@ -1296,39 +1383,47 @@
             np.savez(file_name,
                      eigenvalue  = egg,
                      eigenvector = evv,
                      wavevector_unit = self.kvec,
                      wavevector_index = self.wavenum_table,
                      )
             logger.info("save_results: save eigenvalues and eigenvectors in file {}".format(file_name))
-                
-        if "green" in info_outputfile.keys():
-            file_name = os.path.join(path_to_output, info_outputfile["green"])
+
+        # export green function to "green.npz",
+        # or to a file of the name specified by 'green' keyword.
+        # if the keyword has empty string "", nothing exported.
+        fname = info_outputfile.get("green", "green")
+        if fname != "":
+            file_name = os.path.join(path_to_output, fname)
             self._save_green(file_name)
 
         if "onebodyg" in info_outputfile.keys():
             file_name = os.path.join(path_to_output, info_outputfile["onebodyg"])
             self._save_greenone(file_name, green_info)
 
         if "initial" in info_outputfile.keys():
             logger.warn("save_results: save initial is not supported")
             pass
 
+        if "rpa" in info_outputfile.keys():
+            file_name = os.path.join(path_to_output, info_outputfile["rpa"])
+            self._save_trans_mod(file_name)
+
         if "export_hamiltonian" in info_outputfile.keys():
             self._export_hamiltonian(path_to_output, info_outputfile["export_hamiltonian"])
 
     @do_profile
     def _read_green(self, file_name):
         try:
             v = np.load(file_name)
         except FileNotFoundError:
             logger.info("_read_green: file {} not found".format(file_name))
             return None
         return self._read_green_from_data(v)
-            
+
     def _read_green_from_data(self, ginfo):
         if self.has_sublattice:
             if "green_sublattice" in ginfo.files:
                 logger.debug("_read_green: read green_sublattice")
                 data = ginfo["green_sublattice"]
             elif "green" in ginfo.files:
                 logger.debug("_read_green: read green and reshape")
@@ -1394,14 +1489,39 @@
 
                 fw.write("{:3} {:3} {:3} {:3}  {:.12e} {:.12e}\n".format(
                     i, s, j, t, v.real, v.imag
                 ))
 
         logger.info("save_results: save greenone to file {}".format(file_name))
 
+    def _save_trans_mod(self, file_name):
+        nx,ny,nz = self.shape
+        nvol = self.nvol
+        nd = self.nd
+
+        tab_k = self.ham
+        tab_r = np.fft.fftn(tab_k.reshape(nx,ny,nz,nd,nd), axes=(0,1,2)).reshape(nvol,nd,nd) / nvol
+
+        if self.has_sublattice:
+            # use deflate_green to convert to original lattice
+
+            norb = self.norb
+            ns = self.ns
+
+            tab_r_defl = self._deflate_green(tab_r.reshape(nvol,ns,norb,ns,norb))
+
+            lvol = self.cellvol
+            norb_orig = self.norb_orig
+            nd0 = norb_orig * ns
+
+            np.savez(file_name, trans_mod=tab_r_defl.reshape(lvol,nd0,nd0), trans_mod_sublattice=tab_r)
+        else:
+            np.savez(file_name, trans_mod=tab_r)
+        logger.info("save_results: save trans_mod to file {}".format(file_name))
+
     def _export_geometry(self, file_name):
         geom = self.param_ham["Geometry"]
         with open(file_name, "w") as fw:
             # write unit vector
             rvec = geom["rvec"]
             for k in range(3):
                 fw.write("{:.8f} {:.8f} {:.8f}\n".format(rvec[k][0], rvec[k][1], rvec[k][2]))
```

### Comparing `hwave-0.2/src/hwave/solver/uhfr.py` & `hwave-1.0.0/src/hwave/solver/uhfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,19 @@
         self.T = self.param_mod.get("T", 0)
 
         self.strict_hermite = self.param_mod.get("strict_hermite", False)
         self.hermite_tolerance = self.param_mod.get("hermite_tolerance", 1.0e-8)
 
         # Make a list for generating Hamiltonian
         self.Nsize = self.param_mod["nsite"]
-        self.Ncond = self.param_mod["Ncond"]
+        if "filling" in self.param_mod:
+            round_mode = self.param_mod.get("Ncond_round_mode", "strict")
+            self.Ncond = self._round_to_int(self.param_mod["filling"] * 2 * self.Nsize, round_mode)
+        else:
+            self.Ncond = self.param_mod["Ncond"]
         TwoSz = self.param_mod["2Sz"]
         if TwoSz is None:
             self.green_list = {"sz-free": {"label": [i for i in range(2 * self.Nsize)], "occupied": self.Ncond}}
         else:
             self.green_list = {
                 "spin-up": {"label": [i for i in range(self.Nsize)], "value": 0.5, "occupied": int((self.Ncond + TwoSz) / 2)},
                 "spin-down": {"label": [i for i in range(self.Nsize, 2 * self.Nsize)], "value": -0.5,
```

### Comparing `hwave-0.2/PKG-INFO` & `hwave-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwave
-Version: 0.2
+Version: 1.0.0
 Summary: UHF
 Home-page: https://github.com/issp-center-dev/H-Wave
 License: GPL-3.0-or-later
 Author: H-Wave developers
 Author-email: hwave-dev@issp.u-tokyo.ac.jp
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -19,36 +19,31 @@
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/issp-center-dev/H-Wave
 Description-Content-Type: text/markdown
 
 # H-wave
 
-H-wave is a program for performing unrestricted Hartree-Fock (UHF) approximation
-for itinerant electron systems.
-The UHF method approximates two-body interaction terms into one-body ones by
-taking account of the fluctuations up to the first order. The wave functions
-and energies are determined self-consistently by an iterative method.
-H-wave treats two types of UHF approximation: one is real-space and the other is
-wavenumber-space UHF methods using translational symmetry. In the wavenumber space
-UHF method, the input file defining the one-body and two-body interactions is
-based on the Wannier90 format, and the program can be smoothly connected to
-the softwares for deriving effective models from first-principles calculations.
+H-wave is a program for performing unrestricted Hartree-Fock (UHF) approximation and random phase approximation (RPA) for itinerant electron systems. UHF and RPA correspond to simple approximations that deal with fluctuations up to first order and enable analyses of electron correlation effects in materials at a low computational cost. The input files describing the one-body and two-body interactions are based on the Wannier90 format[1]. This allows smooth connection for the software packages that derive the effective models from first principles calculations, such as RESPACK[2], to the analyses of the effective model with H-wave.
+
+[1] G. Pizzi et al, J. Phys.: Condens. Matter 32 165902 (2020).
+[2] K. Nakmura, Y. Yoshimoto, Y. Nomura et al., Comp. Phys. Commun. 261, 107781 (2021).
+
 
 ## Methods
 
-Hartree-Fock approximation
+Hartree-Fock and Random Phase approximation
 
 ## Target models
 
 Hubbard model, multi-orbital Hubbard model
 
 ## Available physical quantities
 
-ground-state energy, free energy, etc.
+ground-state energy, free energy, charge and spin susceptibilities, etc.
 
 ## Requirement
 
 Python3 with numpy, scipy, and other library packages
 
 ## Install
 
@@ -77,20 +72,20 @@
 of The Institute for Solid State Physics, The University of Tokyo.
 
 ## Official page
 
 - [H-wave project site](https://www.pasums.issp.u-tokyo.ac.jp/h-wave/en)
 - [Software repository](https://github.com/issp-center-dev/H-wave)
 - [User Manual](https://www.pasums.issp.u-tokyo.ac.jp/h-wave/en/doc/manual)
-- [Samples/Tutorials](https://isspns-gitlab.issp.u-tokyo.ac.jp/hwave-dev/hwave-gallery)
+- [Data Repository](https://datarepo.mdcl.issp.u-tokyo.ac.jp/repo/23)
 
 ## Authors
 
-Kazuyoshi Yoshimi,
-Yuichi Motoyama,
-Tatsumi Aoyama,
-Kota Ido,
-Takahiro Misawa,
-Taiki Kawamura
-Akito Kobayashi,
-Takeo Kato
+Kazuyoshi Yoshimi (ISSP, Univ. of Tokyo),
+Yuichi Motoyama (ISSP, Univ. of Tokyo),
+Tatsumi Aoyama (ISSP, Univ. of Tokyo),
+Kota Ido (ISSP, Univ. of Tokyo),
+Takahiro Misawa (ISSP, Univ. of Tokyo),
+Taiki Kawamura (Nagoya Univ.),
+Akito Kobayashi (Nagoya Univ.),
+Takeo Kato (ISSP, Univ. of Tokyo)
```

