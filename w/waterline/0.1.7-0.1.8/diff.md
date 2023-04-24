# Comparing `tmp/waterline-0.1.7-py3-none-any.whl.zip` & `tmp/waterline-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,24 @@
-Zip file size: 6216442 bytes, number of entries: 66
--rw-rw-r--  2.0 unx      223 b- defN 23-Apr-09 20:46 waterline/__init__.py
+Zip file size: 6217392 bytes, number of entries: 68
+-rw-rw-r--  2.0 unx      260 b- defN 23-Apr-24 22:11 waterline/__init__.py
+-rw-rw-r--  2.0 unx      129 b- defN 23-Apr-24 21:56 waterline/compiler.py
 -rw-rw-r--  2.0 unx     1805 b- defN 23-Apr-07 00:51 waterline/jobs.py
--rw-rw-r--  2.0 unx     2609 b- defN 23-Apr-10 05:15 waterline/pipeline.py
--rw-rw-r--  2.0 unx     1156 b- defN 23-Apr-11 21:24 waterline/run.py
--rw-rw-r--  2.0 unx     3407 b- defN 23-Apr-11 21:22 waterline/suite.py
+-rw-rw-r--  2.0 unx      619 b- defN 23-Apr-24 22:20 waterline/linker.py
+-rw-rw-r--  2.0 unx     2884 b- defN 23-Apr-24 22:15 waterline/pipeline.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-24 22:09 waterline/run.py
+-rw-rw-r--  2.0 unx     3474 b- defN 23-Apr-24 22:09 waterline/suite.py
 -rw-rw-r--  2.0 unx     7123 b- defN 23-Apr-06 17:01 waterline/suites.py
 -rw-rw-r--  2.0 unx      641 b- defN 23-Apr-10 05:20 waterline/utils.py
 -rw-rw-r--  2.0 unx     6323 b- defN 23-Apr-10 04:50 waterline/workspace.py
 -rw-rw-r--  2.0 unx      135 b- defN 23-Apr-07 15:59 waterline/suites/__init__.py
--rw-rw-r--  2.0 unx     1593 b- defN 23-Apr-10 04:52 waterline/suites/gap.py
--rw-rw-r--  2.0 unx     9004 b- defN 23-Apr-10 19:44 waterline/suites/mibench.py
--rw-rw-r--  2.0 unx     2546 b- defN 23-Apr-09 19:39 waterline/suites/nas.py
--rw-rw-r--  2.0 unx     3416 b- defN 23-Apr-10 15:08 waterline/suites/polybench.py
--rw-rw-r--  2.0 unx     2079 b- defN 23-Apr-07 20:36 waterline/suites/spec2017.py
+-rw-rw-r--  2.0 unx     1644 b- defN 23-Apr-24 22:12 waterline/suites/gap.py
+-rw-rw-r--  2.0 unx     9012 b- defN 23-Apr-24 22:12 waterline/suites/mibench.py
+-rw-rw-r--  2.0 unx     2614 b- defN 23-Apr-24 22:14 waterline/suites/nas.py
+-rw-rw-r--  2.0 unx     3463 b- defN 23-Apr-24 22:11 waterline/suites/polybench.py
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Apr-24 22:12 waterline/suites/spec2017.py
 -rw-rw-r--  2.0 unx     1297 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/Makefile
 -rw-rw-r--  2.0 unx     2959 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/README
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-07 16:10 waterline/suites/SPEC2017/test.txt
 -rwxrwxr-x  2.0 unx  4511744 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s
 -rw-rw-r--  2.0 unx  5067012 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s.bc
 -rwxrwxr-x  2.0 unx 12596976 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/xalancbmk_s/xalancbmk_s
 -rw-rw-r--  2.0 unx      446 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/Makefile
@@ -56,13 +58,13 @@
 -rwxrwxr-x  2.0 unx     2024 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/collect_output.sh
 -rwxrwxr-x  2.0 unx      426 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/compile.sh
 -rwxrwxr-x  2.0 unx      582 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/install.sh
 -rwxrwxr-x  2.0 unx     1410 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/optimization.sh
 -rwxrwxr-x  2.0 unx     2626 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/run.sh
 -rwxrwxr-x  2.0 unx     2757 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/setup.sh
 -rwxrwxr-x  2.0 unx      267 b- defN 23-Apr-09 20:58 waterline/suites/SPEC2017/scripts/uninstall.sh
--rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx      246 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6388 b- defN 23-Apr-11 21:24 waterline-0.1.7.dist-info/RECORD
-66 files, 22293787 bytes uncompressed, 6205982 bytes compressed:  72.2%
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-24 22:24 waterline-0.1.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      246 b- defN 23-Apr-24 22:24 waterline-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 22:24 waterline-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-24 22:24 waterline-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6540 b- defN 23-Apr-24 22:24 waterline-0.1.8.dist-info/RECORD
+68 files, 22295289 bytes uncompressed, 6206700 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
 Filename: waterline/__init__.py
 Comment: 
 
+Filename: waterline/compiler.py
+Comment: 
+
 Filename: waterline/jobs.py
 Comment: 
 
+Filename: waterline/linker.py
+Comment: 
+
 Filename: waterline/pipeline.py
 Comment: 
 
 Filename: waterline/run.py
 Comment: 
 
 Filename: waterline/suite.py
@@ -177,23 +183,23 @@
 
 Filename: waterline/suites/SPEC2017/scripts/setup.sh
 Comment: 
 
 Filename: waterline/suites/SPEC2017/scripts/uninstall.sh
 Comment: 
 
-Filename: waterline-0.1.7.dist-info/LICENSE
+Filename: waterline-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: waterline-0.1.7.dist-info/METADATA
+Filename: waterline-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: waterline-0.1.7.dist-info/WHEEL
+Filename: waterline-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: waterline-0.1.7.dist-info/top_level.txt
+Filename: waterline-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: waterline-0.1.7.dist-info/RECORD
+Filename: waterline-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## waterline/__init__.py

```diff
@@ -1,6 +1,7 @@
 from __future__ import annotations
 from .workspace import Workspace
 from .suite import Suite, Benchmark
 from .run import RunConfiguration, Runner
+from .linker import Linker
 
-__all__ = ["Workspace", "Suite", "Benchmark", "RunConfiguration", "Runner"]
+__all__ = ["Workspace", "Suite", "Benchmark", "RunConfiguration", "Runner", "Linker"]
```

## waterline/pipeline.py

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 import shutil
 from .utils import shell
 from .suite import Benchmark
+from .linker import Linker
 from . import jobs
 from typing import Tuple, List
 
-
 def _should_run(input: Path, output: Path) -> bool:
     """Given an input and an output, check if the input is newer than the output"""
     return not output.exists() or output.stat().st_mtime < input.stat().st_mtime
 
 
 class Stage:
     def run(self, input: Path, output: Path):
@@ -40,46 +40,58 @@
         self.out_bc = output
 
     def run(self):
         self.stage.run(self.in_bc, self.out_bc)
 
 
 class LinkJob(jobs.Job):
-    def __init__(self, name: str, bench: Benchmark, input: Path, output: Path):
+    def __init__(self, name: str, bench: Benchmark, input: Path, output: Path, linker):
         super().__init__(name)
         self.bench = bench
         self.input = input
         self.output = output
+        self.linker = linker
 
     def run(self):
         if _should_run(self.input, self.output):
-            self.bench.link_bitcode(self.input, self.output)
+            self.bench.link_bitcode(self.input, self.output, self.linker)
 
 
 class Pipeline:
     def __init__(self, name: str):
         self.name = name
         self.stages: List[Tuple[Stage, str]] = []
+        self.linker = None
+
+
+    def set_linker(self, linker):
+        self.linker = linker
 
     def add_stage(self, stage: Stage, name=None):
         self.stages.append((stage, name))
 
     def jobs(self, input_bc: Path, output_bc: Path, bench: Benchmark) -> List[Stage]:
         io = []
         for i, (stage, name) in enumerate(self.stages):
             input = input_bc.parent / f"{self.name}-stage{i - 1}.bc"
             output = input_bc.parent / f"{self.name}-stage{i}.bc"
             if i == 0:
                 input = input_bc
             if i == len(self.stages) - 1:
                 output = output_bc
             io.append((input, output))
+
+        linker = self.linker
+        if linker is None:
+            linker = Linker()
+
         for i, ((inp, outp), (stage, name)) in enumerate(zip(io, self.stages)):
             yield StageJob(f"stage {i+1}: {name}", stage, inp, outp)
 
         # Create a link job
         yield LinkJob(
             f"link {bench.suite.name}/{bench.name}",
             bench,
             output_bc,
             bench.suite.bin / bench.name / self.name,
+            linker
         )
```

## waterline/run.py

```diff
@@ -33,10 +33,10 @@
                 [binary, *config.args],
                 stdout=subprocess.DEVNULL,
                 # stderr=subprocess.DEVNULL,
                 env=config.env,
                 cwd=cwd,
             )
             res = proc.wait()
-            print(res)
+            # print(res)
             end = time.time()
         return end - start
```

## waterline/suite.py

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 from typing import List
 from .run import RunConfiguration
+from .linker import Linker
 from . import jobs
 
 
 class JobRunner:
     pass
 
 
@@ -91,26 +92,26 @@
 
     def compile(self, output: Path):
         """
         Compile this benchmark to a certain output file
         """
         pass
 
-    def link(self, object: Path, destination: Path):
+    def link(self, object: Path, destination: Path, linker: Linker):
         """
         Link an object file of this benchmark into a complete executable.
         """
         print(f"link {object} to {destination} not implemented")
 
-    def link_bitcode(self, bitcode: Path, destination: Path):
+    def link_bitcode(self, bitcode: Path, destination: Path, linker: Linker):
         """
         Compile a bitcode file to an object file, then link the object file to the destination
         using `self.link()`
         """
         object = bitcode.parent / (bitcode.stem + ".o")
         self.shell("llc", "-relocation-model=pic", "-O3", bitcode, "--filetype=obj", "-o", object)
 
-        self.link(object, destination)
+        self.link(object, destination, linker)
         pass
 
     def shell(self, *args):
         self.suite.workspace.shell(*args)
```

## waterline/suites/gap.py

```diff
@@ -1,8 +1,8 @@
-from waterline import Suite, Benchmark, Workspace, RunConfiguration
+from waterline import Suite, Benchmark, Workspace, RunConfiguration, Linker
 from waterline.utils import run_command
 from pathlib import Path
 
 
 class GAPBenchmark(Benchmark):
     def compile(self, output: Path):
         source_file = self.suite.src / "src" / (self.name + ".cc")
@@ -13,15 +13,16 @@
             "-std=c++11",
             "-O1",
             "-Wall",
             "-o",
             output,
         )
 
-    def link(self, object: Path, output: Path):
+    def link(self, object: Path, output: Path, linker: Linker):
+        # todo: use linker
         self.shell(
             "clang++",
             object,
             "-fopenmp",
             "-std=c++11",
             "-Wall",
             "-o",
```

## waterline/suites/mibench.py

```diff
@@ -1,8 +1,8 @@
-from waterline import Suite, Benchmark, Workspace, RunConfiguration
+from waterline import Suite, Benchmark, Workspace, RunConfiguration, Linker
 from waterline.utils import run_command
 from pathlib import Path
 import shutil
 from typing import List
 
 
 class MiBenchSimple(Benchmark):
```

## waterline/suites/nas.py

```diff
@@ -1,8 +1,8 @@
-from waterline import Suite, Benchmark, Workspace, RunConfiguration
+from waterline import Suite, Benchmark, Workspace, RunConfiguration, Linker
 from waterline.utils import run_command
 from pathlib import Path
 import waterline.utils
 import shutil
 from typing import Tuple
 
 
@@ -23,16 +23,17 @@
         self.shell(
             "make", "-C", self.suite.src, self.name, f"CLASS={self.suite.suite_class}"
         )
         # if that compiled, copy the binary to the right location
         compiled = self.suite.src / "bin" / (self.name + "." + self.suite.suite_class)
         shutil.copy(compiled, output)
 
-    def link(self, object: Path, dest: Path):
-        self.shell("clang", "-fPIC", "-lm", "-fopenmp", object, "-o", dest)
+    def link(self, object: Path, dest: Path, linker: Linker):
+        # todo: use linker
+        linker.link(self.suite.workspace, [object], dest, args=["-fPIC", "-lm", "-fopenmp"])
 
 
 class NAS(Suite):
     name = "NAS"
 
     def configure(self, enable_openmp: bool = True, suite_class: str = "B"):
         self.enable_openmp = enable_openmp
```

## waterline/suites/polybench.py

```diff
@@ -1,8 +1,8 @@
-from waterline import Suite, Benchmark, Workspace
+from waterline import Suite, Benchmark, Workspace, Linker
 from waterline.utils import run_command
 from pathlib import Path
 import waterline.utils
 import shutil
 from typing import Tuple
 
 
@@ -67,15 +67,16 @@
             source_file,
             "-lm",
             "-Wno-implicit-function-declaration",
             "-o",
             output,
         )
 
-    def link(self, object: Path, output: Path):
+    def link(self, object: Path, output: Path, linker: Linker):
+        # todo: linker
         self.shell("clang", object, "-lm", "-o", output)
 
 
 class PolyBench(Suite):
     name = "PolyBench"
 
     def configure(self, size="LARGE"):
```

## waterline/suites/spec2017.py

```diff
@@ -1,8 +1,8 @@
-from waterline import Suite, Benchmark
+from waterline import Suite, Benchmark, Linker
 from pathlib import Path
 import shutil
 
 
 class SpecBenchmark(Benchmark):
     def __init__(self, suite, name, bin):
         super().__init__(suite, name)
@@ -15,15 +15,16 @@
         shutil.copy(
             self.suite.src
             / f"SPEC2017/benchspec/CPU/{self.name}/build/build_peak_gclang.0000/"
             / self.bin,
             output,
         )
 
-    def link(self, object: Path, output: Path):
+    def link(self, object: Path, output: Path, linker: Linker):
+        # todo: linker
         self.shell("clang++", object, "-lm", "-lstdc++", "-lpthread", "-o", output)
 
 
 default_benchmarks = [
     # Integer
     ("600.perlbench_s", "perlbench_s"),
     ("602.gcc_s", "sgcc"),
```

## Comparing `waterline-0.1.7.dist-info/LICENSE` & `waterline-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `waterline-0.1.7.dist-info/RECORD` & `waterline-0.1.8.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-waterline/__init__.py,sha256=4UwrTIE53TLXgBtiS8bm9QI3FH75W1AZM4e9XcpCRfo,223
+waterline/__init__.py,sha256=ygH_PGE0BoLvPCSVt8JtMETGpCg0h--iq-DgSiP3tUQ,260
+waterline/compiler.py,sha256=AF_7cjjaELsFKN-iVReJzEtmdRcTqW62tFI1utytqQ4,129
 waterline/jobs.py,sha256=0yYmMT-BK_TzrGRzBbZBmLIjwxxHddCSPHVKn8ZUjXU,1805
-waterline/pipeline.py,sha256=A-9hqHRtpKrIGo2iEFfv9Cw0CdNF6NqihuAXhHNM-RU,2609
-waterline/run.py,sha256=5Y8UMl46LKxson_A99hUzgq6JdpGgCRCJlrzkATx6NA,1156
-waterline/suite.py,sha256=S5EO-iOVzjXnOzyMi5DAEvvR3-N15DwHeH4114ZrdyM,3407
+waterline/linker.py,sha256=ljew2Pbvkmf_iHlP5hdr3QGEddytCs2MX3pK2XCC1xc,619
+waterline/pipeline.py,sha256=iftcNQlV-frle2ZALphafASvUdg1iH_9R4Bd6QBe_JQ,2884
+waterline/run.py,sha256=l0Qso8PWkSiiCbMFh2wrY0O-tbGgakrJlqSwSag58Bo,1158
+waterline/suite.py,sha256=P4_fAjQkU3q15ljwb95xYGJSOPKrEQgavCayrRjW1uQ,3474
 waterline/suites.py,sha256=cBJ3KU1Mzzq5LkuCisuvCwcnU9xjPontHEFYYxCtsz0,7123
 waterline/utils.py,sha256=G7a0Bqt8ibml4o7airQ5vL6fkdtFWpnZ8-AocHlk7mA,641
 waterline/workspace.py,sha256=KRIwQEqpmCcHxJgcPWZ_bYKm_1HpMFH7igGUxMJg1UA,6323
 waterline/suites/__init__.py,sha256=ETK4N7n6M9dzDASROaNAthTPdUl97qw2lbW_q5sIgrQ,135
-waterline/suites/gap.py,sha256=XbLPn0mMb0JxzH1yVT3J98Y-cCJa_06wu55ABmL1_nY,1593
-waterline/suites/mibench.py,sha256=zX0u-rcmYbtEww2n01ElUEICqn-bl-hiWd_M8w0ac7I,9004
-waterline/suites/nas.py,sha256=WLqeP3CPqUFhZt5ECEpjDGYJA61MOSK2-cn7Vx1suzU,2546
-waterline/suites/polybench.py,sha256=sHG-0twmJlp5f3_zi5A_0oekdVR_IuRvF7PDDjM1HLM,3416
-waterline/suites/spec2017.py,sha256=14AcdlXKvtdwbL0RAQ0_LmCdONNJr1e7W4rPnBMi9pc,2079
+waterline/suites/gap.py,sha256=lTedLLlKAPVUd8s7UB4wRUS1bB5J-ItTAWJSxHVd8O8,1644
+waterline/suites/mibench.py,sha256=Dr5NT0VBjeUDN0Ieog6X7kBEfcqj6G9DazoAmSwY6II,9012
+waterline/suites/nas.py,sha256=mC1i5QGpJWZPcaeXDy-FM82RFiEHK2wff-vUkH9sByc,2614
+waterline/suites/polybench.py,sha256=eM6_w38SFwGfzIay_rfec4UXyEjj6HsyUtDfv75PqjE,3463
+waterline/suites/spec2017.py,sha256=ifuAE67ElSJM-Fzey0vJOB6N8wMIutKPTgTC3vH_S1w,2126
 waterline/suites/SPEC2017/Makefile,sha256=kHw3DC6XA1_KnWp0hcoaAhRnsIVugk4J04ZBM2-p7pA,1297
 waterline/suites/SPEC2017/README,sha256=EMM5XiYQ_Dy36WvBw-fIS7bnYpStx2tQms5igraom88,2959
 waterline/suites/SPEC2017/test.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s,sha256=NtLDubIsdpLwv-Cn3ey-D7SE0u2SxejhxJPrSSbPYTE,4511744
 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s.bc,sha256=3cyAGbCI5989qQf2XNdTcb5_HePciJhf05lZYMMLMsU,5067012
 waterline/suites/SPEC2017/benchmarks/xalancbmk_s/xalancbmk_s,sha256=3RXpLkRrIsXlYEwoeGZUAv3x-W7YPA-42wMDoFoQeII,12596976
 waterline/suites/SPEC2017/condor/Makefile,sha256=y-KcPJrUHXGaNs88-DtqtE9PnjDHV1a5U5yNA0A77fQ,446
@@ -55,12 +57,12 @@
 waterline/suites/SPEC2017/scripts/collect_output.sh,sha256=ggAiKroVgHC5rq26J3eVa0fW4FFaeiLsG6BUfWZ2weY,2024
 waterline/suites/SPEC2017/scripts/compile.sh,sha256=9VpgIqHmLgfKjjibS0i4xFkNh6dgEgrWqKyyK-MiceI,426
 waterline/suites/SPEC2017/scripts/install.sh,sha256=3fQeOYVldVYHHfh6WgQLJeKot3J0ijMUQ7nz8YUE1Vw,582
 waterline/suites/SPEC2017/scripts/optimization.sh,sha256=6qHL1B3J-M5M80RJp2E7W9FB_jmNS6grcRYKOgOo5jk,1410
 waterline/suites/SPEC2017/scripts/run.sh,sha256=zWKgeZ_pteRG3Quks7e8KKbkQbz38CWHBBWTVUzOR68,2626
 waterline/suites/SPEC2017/scripts/setup.sh,sha256=FnVDLvabQm6CVwxl0y0rA5g6V5j5VXLm2ZZVIO2xZI8,2757
 waterline/suites/SPEC2017/scripts/uninstall.sh,sha256=0szAcj1MraRZ0QjGdL6aLq8QkxKdFm9qoTAaKdhOeUY,267
-waterline-0.1.7.dist-info/LICENSE,sha256=UveJQplGBXBAOAqKBm_4SQ2XE2VBHPRJDIuVa9829uc,1057
-waterline-0.1.7.dist-info/METADATA,sha256=14ZR-NsgpFiNGeCCLTIDAHnqEDx1p4wQNcb3_4p1wZQ,246
-waterline-0.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-waterline-0.1.7.dist-info/top_level.txt,sha256=ptFfPeDDWWfu4ZroUwKjceRrASyf4j3zXvL1UxLuLTk,10
-waterline-0.1.7.dist-info/RECORD,,
+waterline-0.1.8.dist-info/LICENSE,sha256=UveJQplGBXBAOAqKBm_4SQ2XE2VBHPRJDIuVa9829uc,1057
+waterline-0.1.8.dist-info/METADATA,sha256=JaihEkf7X2rUAmZR5N5zKfAQE3Jy-lnrHSuecoVRWwk,246
+waterline-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+waterline-0.1.8.dist-info/top_level.txt,sha256=ptFfPeDDWWfu4ZroUwKjceRrASyf4j3zXvL1UxLuLTk,10
+waterline-0.1.8.dist-info/RECORD,,
```

