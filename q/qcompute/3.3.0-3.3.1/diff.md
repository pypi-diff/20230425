# Comparing `tmp/qcompute-3.3.0.tar.gz` & `tmp/qcompute-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcompute-3.3.0.tar", last modified: Sun Feb 19 07:46:48 2023, max compression
+gzip compressed data, was "qcompute-3.3.1.tar", last modified: Tue Apr 25 08:51:51 2023, max compression
```

## Comparing `qcompute-3.3.0.tar` & `qcompute-3.3.1.tar`

### file list

```diff
@@ -1,162 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.493297 qcompute-3.3.0/
--rw-rw-rw-   0        0        0      601 2023-02-19 07:44:27.000000 qcompute-3.3.0/LICENSE
--rw-rw-rw-   0        0        0     4473 2023-02-19 07:46:48.492297 qcompute-3.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.288503 qcompute-3.3.0/QCompute/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.290504 qcompute-3.3.0/QCompute/Calibration/
--rw-rw-rw-   0        0        0     5343 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Calibration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.294504 qcompute-3.3.0/QCompute/Define/
--rw-rw-rw-   0        0        0     2881 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Define/Settings.py
--rw-rw-rw-   0        0        0     2811 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Define/Utils.py
--rw-rw-rw-   0        0        0     3475 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Define/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.296507 qcompute-3.3.0/QCompute/Module/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.297508 qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/
--rw-rw-rw-   0        0        0     1686 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.299510 qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/
--rw-rw-rw-   0        0        0     1662 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.301509 qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/
--rw-rw-rw-   0        0        0     1635 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.303509 qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/
--rw-rw-rw-   0        0        0     2499 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.305510 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/
--rw-rw-rw-   0        0        0     2455 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.307510 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/
--rw-rw-rw-   0        0        0     2392 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py
--rw-rw-rw-   0        0        0      713 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.308510 qcompute-3.3.0/QCompute/OpenConvertor/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.310015 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/
--rw-rw-rw-   0        0        0     9315 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.312019 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/
--rw-rw-rw-   0        0        0     3423 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.314019 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/
--rw-rw-rw-   0        0        0     5194 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.316020 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/
--rw-rw-rw-   0        0        0     1316 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.318020 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/
--rw-rw-rw-   0        0        0    17698 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.320021 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/
--rw-rw-rw-   0        0        0     6611 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.321021 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/
--rw-rw-rw-   0        0        0    16194 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.323021 qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/
--rw-rw-rw-   0        0        0     2061 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.324022 qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/
--rw-rw-rw-   0        0        0     7379 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.326022 qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/
--rw-rw-rw-   0        0        0     1211 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.328022 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.330022 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/
--rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.339024 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/
--rw-rw-rw-   0        0        0     9067 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py
--rw-rw-rw-   0        0        0     7554 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py
--rw-rw-rw-   0        0        0    80812 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py
--rw-rw-rw-   0        0        0     4755 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py
--rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py
--rw-rw-rw-   0        0        0    51411 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/__init__.py
--rw-rw-rw-   0        0        0      842 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.341025 qcompute-3.3.0/QCompute/OpenModule/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.342026 qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/
--rw-rw-rw-   0        0        0     5967 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.344026 qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/
--rw-rw-rw-   0        0        0     8690 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.346027 qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/
--rw-rw-rw-   0        0        0     5061 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.347027 qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/
--rw-rw-rw-   0        0        0     2398 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.349027 qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/
--rw-rw-rw-   0        0        0    19632 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.351028 qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/
--rw-rw-rw-   0        0        0     3756 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.353028 qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/
--rw-rw-rw-   0        0        0     4762 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/__init__.py
--rw-rw-rw-   0        0        0      950 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.354028 qcompute-3.3.0/QCompute/OpenService/
--rw-rw-rw-   0        0        0      713 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.356029 qcompute-3.3.0/QCompute/OpenService/service_ubqc/
--rw-rw-rw-   0        0        0     2093 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.366031 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/
--rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/__init__.py
--rw-rw-rw-   0        0        0    40419 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/client.py
--rw-rw-rw-   0        0        0    34117 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/mcalculus.py
--rw-rw-rw-   0        0        0    62675 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/qobject.py
--rw-rw-rw-   0        0        0     2334 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/transpiler.py
--rw-rw-rw-   0        0        0    20703 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.368031 qcompute-3.3.0/QCompute/OpenSimulator/
--rw-rw-rw-   0        0        0     7160 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.377034 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/
--rw-rw-rw-   0        0        0     1499 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/InitState.py
--rw-rw-rw-   0        0        0     7788 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Measure.py
--rw-rw-rw-   0        0        0    59134 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
--rw-rw-rw-   0        0        0     5511 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
--rw-rw-rw-   0        0        0     6316 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.385038 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/
--rw-rw-rw-   0        0        0     1838 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/CheckEnv.py
--rw-rw-rw-   0        0        0     3622 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/DistEinsum.py
--rw-rw-rw-   0        0        0     6575 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Kernel.py
--rw-rw-rw-   0        0        0     9045 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Simulator.py
--rw-rw-rw-   0        0        0     8271 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.404042 qcompute-3.3.0/QCompute/QPlatform/
--rw-rw-rw-   0        0        0      747 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/BatchID.py
--rw-rw-rw-   0        0        0     9313 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/CircuitTools.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.406043 qcompute-3.3.0/QCompute/QPlatform/Condition/
--rw-rw-rw-   0        0        0     1147 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Condition/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Error.py
--rw-rw-rw-   0        0        0    10657 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/InteractiveModule.py
--rw-rw-rw-   0        0        0     2001 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/ProcedureParameterPool.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.412553 qcompute-3.3.0/QCompute/QPlatform/Processor/
--rw-rw-rw-   0        0        0     7195 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/ModuleFilter.py
--rw-rw-rw-   0        0        0     3875 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/PostProcessor.py
--rw-rw-rw-   0        0        0     2978 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/PreProcess.py
--rw-rw-rw-   0        0        0      693 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/__init__.py
--rw-rw-rw-   0        0        0    26808 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/QEnv.py
--rw-rw-rw-   0        0        0     7560 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QEnvOperation.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.430557 qcompute-3.3.0/QCompute/QPlatform/QNoise/
--rw-rw-rw-   0        0        0     5870 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/AmplitudeDamping.py
--rw-rw-rw-   0        0        0     2416 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/BitFlip.py
--rw-rw-rw-   0        0        0     2421 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/BitPhaseFlip.py
--rw-rw-rw-   0        0        0     5632 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/CustomizedNoise.py
--rw-rw-rw-   0        0        0     2704 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/Depolarizing.py
--rw-rw-rw-   0        0        0     2889 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PauliNoise.py
--rw-rw-rw-   0        0        0     2666 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseDamping.py
--rw-rw-rw-   0        0        0     2415 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseFlip.py
--rw-rw-rw-   0        0        0     4516 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/ResetNoise.py
--rw-rw-rw-   0        0        0     5958 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/Utilities.py
--rw-rw-rw-   0        0        0     3243 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.444560 qcompute-3.3.0/QCompute/QPlatform/QOperation/
--rw-rw-rw-   0        0        0     1236 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/Barrier.py
--rw-rw-rw-   0        0        0     6724 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/CompositeGate.py
--rw-rw-rw-   0        0        0     1666 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/CustomizedGate.py
--rw-rw-rw-   0        0        0    11825 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/FixedGate.py
--rw-rw-rw-   0        0        0     1968 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/Measure.py
--rw-rw-rw-   0        0        0     3021 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/QProcedure.py
--rw-rw-rw-   0        0        0    11615 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/RotationGate.py
--rw-rw-rw-   0        0        0     8156 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/__init__.py
--rw-rw-rw-   0        0        0     3569 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QRegPool.py
--rw-rw-rw-   0        0        0     2524 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QStatus.py
--rw-rw-rw-   0        0        0    16075 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/QTask.py
--rw-rw-rw-   0        0        0     6731 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Utilities.py
--rw-rw-rw-   0        0        0     7607 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.446561 qcompute-3.3.0/QCompute/QProtobuf/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.458286 qcompute-3.3.0/QCompute/QProtobuf/Library/
--rw-rw-rw-   0        0        0     1164 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/Complex_pb2.py
--rw-rw-rw-   0        0        0     3423 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/PlatformStruct_pb2.py
--rw-rw-rw-   0        0        0     3422 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QNoise_pb2.py
--rw-rw-rw-   0        0        0     1691 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QObj_pb2.py
--rw-rw-rw-   0        0        0     2412 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QOperation_pb2.py
--rw-rw-rw-   0        0        0     1488 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py
--rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/__init__.py
--rw-rw-rw-   0        0        0     1595 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QProtobuf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.460290 qcompute-3.3.0/QCompute/Utilize/
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.462290 qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/
--rw-rw-rw-   0        0        0    17017 2023-02-19 07:44:28.000000 qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/__init__.py
--rw-rw-rw-   0        0        0      714 2023-02-19 07:44:28.000000 qcompute-3.3.0/QCompute/Utilize/__init__.py
--rw-rw-rw-   0        0        0     4451 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/__init__.py
--rw-rw-rw-   0        0        0     3891 2023-02-19 07:44:28.000000 qcompute-3.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.491297 qcompute-3.3.0/qcompute.egg-info/
--rw-rw-rw-   0        0        0     4473 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4854 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 07:46:48.494298 qcompute-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2141 2023-02-19 07:45:34.000000 qcompute-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.312621 qcompute-3.3.1/
+-rw-rw-rw-   0        0        0      601 2023-04-25 08:44:12.000000 qcompute-3.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4455 2023-04-25 08:51:51.311621 qcompute-3.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.980999 qcompute-3.3.1/QCompute/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.983999 qcompute-3.3.1/QCompute/Calibration/
+-rw-rw-rw-   0        0        0     5343 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/Calibration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.991002 qcompute-3.3.1/QCompute/Define/
+-rw-rw-rw-   0        0        0     2881 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Define/Settings.py
+-rw-rw-rw-   0        0        0     2811 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/Define/Utils.py
+-rw-rw-rw-   0        0        0     3562 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Define/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.993001 qcompute-3.3.1/QCompute/Module/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.995000 qcompute-3.3.1/QCompute/Module/MappingToBaiduQPUQianModule/
+-rw-rw-rw-   0        0        0     1686 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:50.997002 qcompute-3.3.1/QCompute/Module/MappingToIoPCASModule/
+-rw-rw-rw-   0        0        0     1662 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/MappingToIoPCASModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.000003 qcompute-3.3.1/QCompute/Module/MappingToIonAPMModule/
+-rw-rw-rw-   0        0        0     1635 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/MappingToIonAPMModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.002002 qcompute-3.3.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/
+-rw-rw-rw-   0        0        0     2499 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.004004 qcompute-3.3.1/QCompute/Module/UnrollCircuitToIoPCASModule/
+-rw-rw-rw-   0        0        0     2455 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.007004 qcompute-3.3.1/QCompute/Module/UnrollCircuitToIonAPMModule/
+-rw-rw-rw-   0        0        0     2392 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/Module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.009005 qcompute-3.3.1/QCompute/OpenConvertor/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.012007 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToDrawConsole/
+-rw-rw-rw-   0        0        0    11764 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.014006 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToInternalStruct/
+-rw-rw-rw-   0        0        0     3423 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.017006 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToIonQ/
+-rw-rw-rw-   0        0        0     5194 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToIonQ/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.019006 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToJson/
+-rw-rw-rw-   0        0        0     1316 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToJson/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.021006 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQasm/
+-rw-rw-rw-   0        0        0    17725 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQasm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.024008 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQobj/
+-rw-rw-rw-   0        0        0     6611 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQobj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.026008 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToXanaduSF/
+-rw-rw-rw-   0        0        0    16194 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.028008 qcompute-3.3.1/QCompute/OpenConvertor/InternalStructToCircuit/
+-rw-rw-rw-   0        0        0     2061 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.031009 qcompute-3.3.1/QCompute/OpenConvertor/IonQToCircuit/
+-rw-rw-rw-   0        0        0     7379 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/IonQToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.033010 qcompute-3.3.1/QCompute/OpenConvertor/JsonToCircuit/
+-rw-rw-rw-   0        0        0     1211 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/JsonToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.036009 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.038012 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/
+-rw-rw-rw-   0        0        0      692 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.051013 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/
+-rw-rw-rw-   0        0        0     9067 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py
+-rw-rw-rw-   0        0        0     7554 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py
+-rw-rw-rw-   0        0        0    80812 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py
+-rw-rw-rw-   0        0        0     4755 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py
+-rw-rw-rw-   0        0        0      692 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py
+-rw-rw-rw-   0        0        0    51411 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenConvertor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.053019 qcompute-3.3.1/QCompute/OpenModule/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.055019 qcompute-3.3.1/QCompute/OpenModule/CompositeGateModule/
+-rw-rw-rw-   0        0        0     5967 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/CompositeGateModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.058021 qcompute-3.3.1/QCompute/OpenModule/CompressGateModule/
+-rw-rw-rw-   0        0        0     8690 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/CompressGateModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.060020 qcompute-3.3.1/QCompute/OpenModule/CompressNoiseModule/
+-rw-rw-rw-   0        0        0    16571 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/CompressNoiseModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.063022 qcompute-3.3.1/QCompute/OpenModule/InverseCircuitModule/
+-rw-rw-rw-   0        0        0     5061 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/InverseCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.065023 qcompute-3.3.1/QCompute/OpenModule/ReverseCircuitModule/
+-rw-rw-rw-   0        0        0     2398 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/ReverseCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.067530 qcompute-3.3.1/QCompute/OpenModule/UnrollCircuitModule/
+-rw-rw-rw-   0        0        0    19632 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/UnrollCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.070538 qcompute-3.3.1/QCompute/OpenModule/UnrollNoiseModule/
+-rw-rw-rw-   0        0        0     3756 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/UnrollNoiseModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.072538 qcompute-3.3.1/QCompute/OpenModule/UnrollProcedureModule/
+-rw-rw-rw-   0        0        0     4762 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/UnrollProcedureModule/__init__.py
+-rw-rw-rw-   0        0        0      950 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.075539 qcompute-3.3.1/QCompute/OpenService/
+-rw-rw-rw-   0        0        0      713 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.077540 qcompute-3.3.1/QCompute/OpenService/service_ubqc/
+-rw-rw-rw-   0        0        0     2093 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.091542 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/
+-rw-rw-rw-   0        0        0      692 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/__init__.py
+-rw-rw-rw-   0        0        0    40419 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/client.py
+-rw-rw-rw-   0        0        0    34117 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/mcalculus.py
+-rw-rw-rw-   0        0        0    62675 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/qobject.py
+-rw-rw-rw-   0        0        0     2334 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/transpiler.py
+-rw-rw-rw-   0        0        0    20703 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.093542 qcompute-3.3.1/QCompute/OpenSimulator/
+-rw-rw-rw-   0        0        0     7813 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.114548 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/
+-rw-rw-rw-   0        0        0     8357 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/BaseSimulator.py
+-rw-rw-rw-   0        0        0    10353 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/GeneralNoiseSimulator.py
+-rw-rw-rw-   0        0        0     2120 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/InitState.py
+-rw-rw-rw-   0        0        0    17564 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/LowNoiseCircuitSimulator.py
+-rw-rw-rw-   0        0        0     7788 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/Measure.py
+-rw-rw-rw-   0        0        0    12614 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/MixedUnitaryNoiseSimulator.py
+-rw-rw-rw-   0        0        0     7679 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/NoNoiseSimulator.py
+-rw-rw-rw-   0        0        0     5640 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
+-rw-rw-rw-   0        0        0     5511 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
+-rw-rw-rw-   0        0        0     6344 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.148555 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/
+-rw-rw-rw-   0        0        0     2316 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/FockAddPhotons.py
+-rw-rw-rw-   0        0        0     3511 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/FockAuxiliaryCalculation.py
+-rw-rw-rw-   0        0        0     3392 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/FockCalculateInterferometer.py
+-rw-rw-rw-   0        0        0     6045 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/FockCombination.py
+-rw-rw-rw-   0        0        0     4832 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/FockPhotonCountMeasure.py
+-rw-rw-rw-   0        0        0    12213 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/GaussAuxiliaryCalculation.py
+-rw-rw-rw-   0        0        0     4900 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/GaussHeteroMea.py
+-rw-rw-rw-   0        0        0     4345 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/GaussHomoMea.py
+-rw-rw-rw-   0        0        0     4346 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/GaussPhotonCountMea.py
+-rw-rw-rw-   0        0        0     4986 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/GaussTransfer.py
+-rw-rw-rw-   0        0        0     1379 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/InitFockState.py
+-rw-rw-rw-   0        0        0     1664 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/InitGaussState.py
+-rw-rw-rw-   0        0        0    15923 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/Simulator.py
+-rw-rw-rw-   0        0        0     5283 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim_photonic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.160563 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/
+-rw-rw-rw-   0        0        0     1838 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/CheckEnv.py
+-rw-rw-rw-   0        0        0     3622 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/DistEinsum.py
+-rw-rw-rw-   0        0        0     6841 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/Kernel.py
+-rw-rw-rw-   0        0        0     9045 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/Simulator.py
+-rw-rw-rw-   0        0        0     8271 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.189078 qcompute-3.3.1/QCompute/QPlatform/
+-rw-rw-rw-   0        0        0      747 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/BatchID.py
+-rw-rw-rw-   0        0        0    11158 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/CircuitTools.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.191079 qcompute-3.3.1/QCompute/QPlatform/Condition/
+-rw-rw-rw-   0        0        0     1147 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Condition/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Error.py
+-rw-rw-rw-   0        0        0    10727 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QPlatform/InteractiveModule.py
+-rw-rw-rw-   0        0        0     2001 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/ProcedureParameterPool.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.201079 qcompute-3.3.1/QCompute/QPlatform/Processor/
+-rw-rw-rw-   0        0        0     8905 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QPlatform/Processor/ModuleFilter.py
+-rw-rw-rw-   0        0        0     3875 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Processor/PostProcessor.py
+-rw-rw-rw-   0        0        0     3003 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Processor/PreProcess.py
+-rw-rw-rw-   0        0        0      693 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Processor/__init__.py
+-rw-rw-rw-   0        0        0    29292 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QPlatform/QEnv.py
+-rw-rw-rw-   0        0        0     7560 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QEnvOperation.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.228086 qcompute-3.3.1/QCompute/QPlatform/QNoise/
+-rw-rw-rw-   0        0        0     5870 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/AmplitudeDamping.py
+-rw-rw-rw-   0        0        0     2416 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/BitFlip.py
+-rw-rw-rw-   0        0        0     2421 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/BitPhaseFlip.py
+-rw-rw-rw-   0        0        0     5632 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/CustomizedNoise.py
+-rw-rw-rw-   0        0        0     2704 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/Depolarizing.py
+-rw-rw-rw-   0        0        0     2889 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/PauliNoise.py
+-rw-rw-rw-   0        0        0     2666 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/PhaseDamping.py
+-rw-rw-rw-   0        0        0     2415 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/PhaseFlip.py
+-rw-rw-rw-   0        0        0     4516 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/ResetNoise.py
+-rw-rw-rw-   0        0        0     5958 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/Utilities.py
+-rw-rw-rw-   0        0        0     3243 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QNoise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.247090 qcompute-3.3.1/QCompute/QPlatform/QOperation/
+-rw-rw-rw-   0        0        0     1236 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/Barrier.py
+-rw-rw-rw-   0        0        0     6724 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/CompositeGate.py
+-rw-rw-rw-   0        0        0     1666 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/CustomizedGate.py
+-rw-rw-rw-   0        0        0    11825 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/FixedGate.py
+-rw-rw-rw-   0        0        0     1968 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/Measure.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/QProcedure.py
+-rw-rw-rw-   0        0        0    11607 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/RotationGate.py
+-rw-rw-rw-   0        0        0     9131 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QOperation/__init__.py
+-rw-rw-rw-   0        0        0     3569 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QRegPool.py
+-rw-rw-rw-   0        0        0     2524 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/QStatus.py
+-rw-rw-rw-   0        0        0    16079 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QPlatform/QTask.py
+-rw-rw-rw-   0        0        0    15230 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QPlatform/Utilities.py
+-rw-rw-rw-   0        0        0     7955 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.249090 qcompute-3.3.1/QCompute/QProtobuf/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.270614 qcompute-3.3.1/QCompute/QProtobuf/Library/
+-rw-rw-rw-   0        0        0     1164 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/Complex_pb2.py
+-rw-rw-rw-   0        0        0     3879 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/PlatformStruct_pb2.py
+-rw-rw-rw-   0        0        0     3422 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/QNoise_pb2.py
+-rw-rw-rw-   0        0        0     1691 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/QObj_pb2.py
+-rw-rw-rw-   0        0        0     2412 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/QOperation_pb2.py
+-rw-rw-rw-   0        0        0     2850 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/QPhotonicOperation_pb2.py
+-rw-rw-rw-   0        0        0     1488 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py
+-rw-rw-rw-   0        0        0      692 2023-04-25 08:44:12.000000 qcompute-3.3.1/QCompute/QProtobuf/Library/__init__.py
+-rw-rw-rw-   0        0        0     1859 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/QProtobuf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.272613 qcompute-3.3.1/QCompute/Utilize/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.275617 qcompute-3.3.1/QCompute/Utilize/ControlledCircuit/
+-rw-rw-rw-   0        0        0    17017 2023-04-25 08:44:14.000000 qcompute-3.3.1/QCompute/Utilize/ControlledCircuit/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-04-25 08:44:14.000000 qcompute-3.3.1/QCompute/Utilize/__init__.py
+-rw-rw-rw-   0        0        0     5529 2023-04-25 08:49:42.000000 qcompute-3.3.1/QCompute/__init__.py
+-rw-rw-rw-   0        0        0     3873 2023-04-25 08:44:18.000000 qcompute-3.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:51:51.309620 qcompute-3.3.1/qcompute.egg-info/
+-rw-rw-rw-   0        0        0     4455 2023-04-25 08:51:50.000000 qcompute-3.3.1/qcompute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6236 2023-04-25 08:51:50.000000 qcompute-3.3.1/qcompute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:51:50.000000 qcompute-3.3.1/qcompute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-04-25 08:51:50.000000 qcompute-3.3.1/qcompute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 08:51:50.000000 qcompute-3.3.1/qcompute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:51:51.313622 qcompute-3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2141 2023-04-25 08:49:42.000000 qcompute-3.3.1/setup.py
```

### Comparing `qcompute-3.3.0/LICENSE` & `qcompute-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/PKG-INFO` & `qcompute-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qcompute
-Version: 3.3.0
+Version: 3.3.1
 Summary: QCompute is a Python-based quantum software development kit (SDK). It provides a full-stack programming experience for advanced users via hybrid quantum programming language features and a high-performance simulator.
 Home-page: https://quantum.baidu.com
 Author: Baidu Quantum
 Author-email: quantum@baidu.com
 License: Apache License 2.0
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # QCompute
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2F%E9%87%8F%E6%98%93%E4%BC%8F%E5%9B%BE%E6%A0%87.png)
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.1-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -77,15 +77,15 @@
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
 ## Integrations
 
-The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+The new backend "local_cuquantum" is constructed with the NVIDIA cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk).
 
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
```

### Comparing `qcompute-3.3.0/QCompute/Calibration/__init__.py` & `qcompute-3.3.1/QCompute/Calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Define/Settings.py` & `qcompute-3.3.1/QCompute/Define/Settings.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Define/Utils.py` & `qcompute-3.3.1/QCompute/Define/Utils.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Define/__init__.py` & `qcompute-3.3.1/QCompute/Define/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # service address for production
     quantumHubAddr = 'https://quantum-hub.baidu.com/api'
     quantumBucket = 'quantum-task'
     blindCompAddr = 'wss://blindcomp.baidu.com'
 else:
     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
 
-sdkVersion = 'Python 3.3.0'
+sdkVersion = 'Python 3.3.1'
 """
 SDK Version
 
 Do not modify by user.
 
 Used for task submission.
 """
@@ -138,16 +138,18 @@
 Wait Task Retry Delay Seconds
 
 Do not modify by user.
 
 Retry delay for waittask in case network failed.
 """
 
-outputDirPath = Path('Output').absolute()
-
+outputDirPath = os.environ.get('OUTPUTPATH', None)
+if outputDirPath is None:
+    outputDirPath = Path('Output').absolute()
+    
 """
 Output Dir Path
 
 Do not modify by user.
 
 Will be created, when not exist.
 """
```

### Comparing `qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/MappingToIoPCASModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/MappingToIonAPMModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py` & `qcompute-3.3.1/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Module/__init__.py` & `qcompute-3.3.1/QCompute/Module/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from io import StringIO
 from typing import List
 
 from QCompute.Define import Settings
 from QCompute.OpenConvertor import ConvertorImplement, ModuleErrorCode
 from QCompute.QPlatform import Error
 from QCompute.QPlatform.Utilities import protobufMatrixToNumpyMatrix
-from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate, PBCompositeGate, PBMeasure
+from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate, PBCompositeGate, PBMeasure, \
+    PBPhotonicGaussianGate, PBPhotonicGaussianMeasure, PBPhotonicFockGate, PBPhotonicFockMeasure
 
 FileErrorCode = 2
 
 gapNode = '-'
 gap = gapNode * 2
 gapLen = len(gap)
 numPos = gapLen + 1
@@ -147,14 +148,50 @@
                 for qReg in pbCircuitLine.qRegList:
                     measure: PBMeasure = pbCircuitLine.measure
                     typeName = PBMeasure.Type.Name(measure.type)
                     self._draw(qRegCount, f'|M[{typeName.lower()}]|', [qReg], circuitArray)
             elif op == 'barrier':
                 for qReg in pbCircuitLine.qRegList:
                     self._draw(qRegCount, '|', [qReg], circuitArray)
+            elif op == 'photonicGaussianGate':
+                photonicGaussianGate: PBPhotonicGaussianGate = pbCircuitLine.photonicGaussianGate
+                gateName = PBPhotonicGaussianGate.Name(photonicGaussianGate)
+                # argumentList = []
+                # if pbCircuitLine.argumentIdList:
+                #     for index, argumentId in enumerate(pbCircuitLine.argumentIdList):
+                #         if argumentId == -1:
+                #             argumentList.append(f'{pbCircuitLine.argumentValueList[index]}')
+                #         else:
+                #             argumentList.append(f'P{argumentId}')
+                # else:
+                #     for argument in pbCircuitLine.argumentValueList:
+                #         argumentList.append(f'{argument}')
+                self._draw(qRegCount, f'|{gateName}|', pbCircuitLine.qRegList, circuitArray)
+            elif op == 'photonicGaussianMeasure':
+                for qReg in pbCircuitLine.qRegList:
+                    photonicGaussianMeasure: PBPhotonicGaussianMeasure = pbCircuitLine.photonicGaussianMeasure
+                    typeName = PBPhotonicGaussianMeasure.Type.Name(photonicGaussianMeasure.type)
+                    self._draw(qRegCount, f'|M[{typeName.lower()}]|', [qReg], circuitArray)
+            elif op == 'photonicFockGate':
+                photonicFockGate: PBPhotonicFockGate = pbCircuitLine.photonicFockGate
+                gateName = PBPhotonicFockGate.Name(photonicFockGate)
+                # argumentList = []
+                # if pbCircuitLine.argumentIdList:
+                #     for index, argumentId in enumerate(pbCircuitLine.argumentIdList):
+                #         if argumentId == -1:
+                #             argumentList.append(f'{pbCircuitLine.argumentValueList[index]}')
+                #         else:
+                #             argumentList.append(f'P{argumentId}')
+                # else:
+                #     for argument in pbCircuitLine.argumentValueList:
+                #         argumentList.append(f'{argument}')
+                self._draw(qRegCount, f'|{gateName}|', pbCircuitLine.qRegList, circuitArray)
+            elif op == 'photonicFockMeasure':
+                for qReg in pbCircuitLine.qRegList:
+                    self._draw(qRegCount, f'|M[{"PhotonCount".lower()}]|', [qReg], circuitArray)
             else:
                 raise Error.ArgumentError(f'DrawConsole Unsupported operation {op}!', ModuleErrorCode, FileErrorCode, 1)
 
         for array in circuitArray:
             for text in array:
                 self.stringIO.write(text)
             self.stringIO.write('\n')
```

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToIonQ/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToJson/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQasm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         :param regName: type: str. Name of register.
         :param usingIndex: type: bool. If True, adds braket [] for register index. Default: True.
         
         :return: type: str. Command code of fixed gate.
         """
 
         # Get name of gate.
-        gateName = PBFixedGate.Name(fixedGate)
+        gateName = PBFixedGate.Name(fixedGate).lower()
         # Convert registers.
         if usingIndex:
             regOp = [f'{regName}[{r}]' for r in regs]
             command = ''
 
         # Index can not be used in the procedure. 
         # Set usingIndex=False to remove braket [].
@@ -176,15 +176,15 @@
         :param paramIds: type: List[int], optional. List of param indices.
         # NOTE: paramValues/paramIds may be None.
 
         :return: type: str. Command code of rotation gate.
         """
 
         # Get name of gate.
-        gateName = PBRotationGate.Name(rotationGate)
+        gateName = PBRotationGate.Name(rotationGate).lower()
 
         # Check if optional arguments paramValues and paramIds are None.
         params = self.getFixedArgumentList(paramValues)
         # Convert params.
         paramCall = self.getArgumentList(params, paramIds)
 
         # Convert registers
@@ -212,20 +212,20 @@
         :param usingIndex: type: bool. If True, adds braket [] for register index. Default: True.
 
         :return: type: str. Command of barrier code.
         """
         # Convert registers.
         if usingIndex:
             regOp = [f'{regName}[{r}]' for r in regs]
-            command = ''
+            command = f'barrier {", ".join(regOp)};\n'
         else:
-            regOp = [f'{regName}{r}' for r in regs]
-            # Indent=2.
-            command = '  '
-        command += f'barrier {", ".join(regOp)};\n'
+            command = ''
+            for r in regs:
+                # Indent=2.
+                command += f'  barrier {regName}{r};\n'
         return command
 
     def getProcCommandCode(self, procedureName: str, regs: List[int], regName: str, usingIndex: bool = True,
                            paramValues: Optional[List[float]] = None, paramIds: Optional = None) -> str:
         """
         Convert procedure to command code.
```

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToQobj/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/IonQToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/JsonToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/QasmToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenConvertor/__init__.py` & `qcompute-3.3.1/QCompute/OpenConvertor/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/CompositeGateModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/CompressGateModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/InverseCircuitModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/ReverseCircuitModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/UnrollCircuitModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/UnrollNoiseModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/UnrollProcedureModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenModule/__init__.py` & `qcompute-3.3.1/QCompute/OpenModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/__init__.py` & `qcompute-3.3.1/QCompute/OpenService/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/__init__.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/__init__.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/client.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/client.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/mcalculus.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/mcalculus.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/qobject.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/qobject.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/transpiler.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/transpiler.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/utils.py` & `qcompute-3.3.1/QCompute/OpenService/service_ubqc/client/utils.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/__init__.py` & `qcompute-3.3.1/QCompute/OpenSimulator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     """
 
     ancilla: Ancilla = Ancilla()
     """
     ancilla
     """
 
-    moduleList:Dict[str,Any] = None
+    moduleList: Dict[str, Any] = None
     """
     moduleList
     """
 
     shots = 0
     """
     number of shots
@@ -181,15 +181,15 @@
         self.shots = 0
         self.counts = None
         self.state = None
         self.seed = 0
         self.startTimeUtc = ''
         self.endTimeUtc = ''
 
-    def fromJson(self, text: str):
+    def fromJson(self, text: str) -> Dict[str, Any]:
         """
         fromJson
         """
         data = json.loads(text)
         if 'sdkVersion' in data:
             self.sdkVersion = data['sdkVersion']  # 否则在模拟器提交前写好
         if 'simulatorVersion' in data:
@@ -200,31 +200,32 @@
             self.simulatorVersion.compileTime = simulatorVersion['compileTime']
         # self.code = data['code']
         # self.output = data['output']
         # self.log = data['log']
         if 'ancilla' in data:
             if 'usedQRegList' in data['ancilla'] and data['ancilla']['usedQRegList'] is not None:
                 self.ancilla.usedQRegList = data['ancilla']['usedQRegList']
-            if 'usedCRegList' in ['ancilla'] and data['ancilla']['usedCRegList'] is not None:
+            if 'usedCRegList' in data['ancilla'] and data['ancilla']['usedCRegList'] is not None:
                 self.ancilla.usedCRegList = data['ancilla']['usedCRegList']
             if 'compactedQRegDict' in data['ancilla'] and data['ancilla']['compactedQRegDict'] is not None:
                 self.ancilla.compactedQRegDict = data['ancilla']['compactedQRegDict']
             if 'compactedCRegDict' in data['ancilla'] and data['ancilla']['compactedCRegDict'] is not None:
                 self.ancilla.compactedCRegDict = data['ancilla']['compactedCRegDict']
         if 'moduleList' in data:
             self.moduleList = data['moduleList']
         self.shots = data['shots']
         self.counts = data['counts']
         if 'state' in data and data['state'] is not None:
             self.state = dictMatrixToNumpyMatrix(data['state'], complex)
         self.seed = data['seed']
         self.startTimeUtc = data['startTimeUtc']
         self.endTimeUtc = data['endTimeUtc']
+        return data
 
-    def toJson(self, inside: bool = None):
+    def toJson(self, inside: bool = None) -> str:
         """
         toJson
         """
         ret = {
             'sdkVersion': self.sdkVersion,
             'ancilla': {
                 'usedQRegList': self.ancilla.usedQRegList,
@@ -253,14 +254,40 @@
                 'fileHash': self.simulatorVersion.fileHash,
                 'compileTime': self.simulatorVersion.compileTime,
             }
             ret['simulatorVersion'] = simulatorVersion
         return json.dumps(ret)
 
 
+class QPhotonicResult(QResult):
+    """
+    The result of photonic experiment.
+
+    For homodyne measure and heterodyne measure.
+    """
+
+    value: Union[Dict[str, int], Dict[str, float]] = None
+    """
+    value for results
+    """
+
+    def __int__(self):
+        self.value = None
+
+    def fromJson(self, text: str):
+        data = super().fromJson(text)
+        self.value = data['value']
+
+    def toJson(self, inside: bool = None):
+        ret = super().toJson(inside)
+        data = json.loads(ret)
+        data['value'] = self.value
+        return json.dumps(data)
+
+
 class QImplement:
     """
     Implement params for quantum execution.
 
     Send to the simulator when submitting a task.
     """
 
@@ -275,15 +302,15 @@
     """
 
     backendArgument = None
     """
     The arguments of backend
     """
 
-    result = QResult()
+    result: Union[QResult, QPhotonicResult] = None
     """
     The final result
     """
 
     def commit(self):
         """
         Commit task
```

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Measure.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/Measure.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/__init__.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_baidu_sim2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from sys import executable
 from typing import List
 
 from QCompute import Define
 from QCompute.Define import Settings
 from QCompute.Define.Utils import filterConsoleOutput, findUniError
 from QCompute.OpenConvertor.CircuitToJson import CircuitToJson
-from QCompute.OpenSimulator import QImplement, ModuleErrorCode, withNoise
+from QCompute.OpenSimulator import QImplement, ModuleErrorCode, withNoise, QResult
 from QCompute.OpenSimulator.local_baidu_sim2.Simulator import runSimulator
 from QCompute.QPlatform import Error
 
 FileErrorCode = 4
 
 
 class Backend(QImplement):
@@ -131,16 +131,17 @@
             '-inputFile', programFilePath)
         if Settings.outputInfo:
             print(f'{cmd}')
 
         # call the simulator
         completedProcess = subprocess.run(
             # Compatible with Python3.6, in Python3.7 and above, the more understandable alias of 'universal_newlines' is 'text'.
-            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True, encoding='utf-8')
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True, encoding='utf-8')
 
+        self.result = QResult()
         self.result.log = filterConsoleOutput(completedProcess.stdout)
         # collect the result to simulator for the subsequent invoking
         self.result.code = completedProcess.returncode
         if self.result.code != 0:
             self.result.vendor = findUniError(completedProcess.stdout) or \
                                  f'QC.3.{ModuleErrorCode}.{FileErrorCode}.2'
             return
```

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/CheckEnv.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/CheckEnv.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/DistEinsum.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/DistEinsum.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Kernel.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/Kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,20 @@
     CUSV_HANDLE = cusv.create()
 
     # single + half precision
     # NP_DATA_TYPE = np.complex64  # todo: numpy do not support half precision complex. Fix it later.
     # CUDA_DATA_TYPE = cuquantum.cudaDataType.CUDA_C_32F
     # DistEinsum.CUDA_COMPUTE_TYPE = cuquantum.ComputeType.COMPUTE_16F
 
+    # single precision (tensor-float)
+    # NP_DATA_TYPE = np.complex64  # todo: numpy do not support tf32. Fix it later.
+    # CUDA_DATA_TYPE = cuquantum.cudaDataType.CUDA_C_32F
+    # DistEinsum.CUDA_COMPUTE_TYPE = cuquantum.ComputeType.COMPUTE_TF32
 
-    # single precision
+    # single precision (normal float)
     NP_DATA_TYPE = np.complex64
     CUDA_DATA_TYPE = cuquantum.cudaDataType.CUDA_C_32F
     DistEinsum.CUDA_COMPUTE_TYPE = cuquantum.ComputeType.COMPUTE_32F
 
     # double precision
     # NP_DATA_TYPE = np.complex128
     # CUDA_DATA_TYPE = cuquantum.cudaDataType.CUDA_C_64F
```

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Simulator.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/Simulator.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/__init__.py` & `qcompute-3.3.1/QCompute/OpenSimulator/local_cuquantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/BatchID.py` & `qcompute-3.3.1/QCompute/QPlatform/BatchID.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/CircuitTools.py` & `qcompute-3.3.1/QCompute/QPlatform/CircuitTools.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,18 +33,23 @@
 from QCompute.QPlatform.QNoise.PhaseFlip import PhaseFlip
 from QCompute.QPlatform.QNoise.ResetNoise import ResetNoise
 from QCompute.QPlatform.QOperation.Barrier import BarrierOP
 from QCompute.QPlatform.QOperation.CompositeGate import CompositeGateOP
 from QCompute.QPlatform.QOperation.CustomizedGate import CustomizedGateOP
 from QCompute.QPlatform.QOperation.FixedGate import FixedGateOP
 from QCompute.QPlatform.QOperation.Measure import MeasureOP
+from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianGate import PhotonicGaussianGateOP
+from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianMeasure import PhotonicGaussianMeasureOP
+from QCompute.QPlatform.QOperation.Photonic.PhotonicFockGate import PhotonicFockGateOP
+from QCompute.QPlatform.QOperation.Photonic.PhotonicFockMeasure import PhotonicFockMeasureOP
 from QCompute.QPlatform.QOperation.QProcedure import QProcedureOP
 from QCompute.QPlatform.QOperation.RotationGate import RotationGateOP
 from QCompute.QPlatform.Utilities import numpyMatrixToProtobufMatrix
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate, PBCompositeGate, \
+    PBPhotonicGaussianGate, PBPhotonicGaussianMeasure, PBPhotonicFockGate, PBPhotonicFockMeasure, \
     PBMeasure, PBQNoise, PBQNoiseDefine
 
 if TYPE_CHECKING:
     from QCompute.QPlatform.QEnv import QEnv
     from QCompute.QPlatform.QOperation import CircuitLine, QOperation
 
 FileErrorCode = 5
@@ -94,14 +99,32 @@
         pbCircuitLine.argumentIdList[:] = argumentIdList
         pbCircuitLine.argumentValueList[:] = argumentValueList
     elif isinstance(circuitLine.data, MeasureOP):
         pbCircuitLine.measure.type = PBMeasure.Type.Value(circuitLine.data.name)
         pbCircuitLine.measure.cRegList[:] = circuitLine.cRegList
     elif isinstance(circuitLine.data, BarrierOP):
         pbCircuitLine.barrier = True
+    elif isinstance(circuitLine.data, PhotonicGaussianGateOP):
+        pbCircuitLine.photonicGaussianGate = PBPhotonicGaussianGate.Value(circuitLine.data.name)
+        pbCircuitLine.argumentValueList[:] = circuitLine.data.argumentList
+    elif isinstance(circuitLine.data, PhotonicGaussianMeasureOP):
+        pbCircuitLine.photonicGaussianMeasure.type = PBPhotonicGaussianMeasure.Type.Value(circuitLine.data.name)
+        pbCircuitLine.photonicGaussianMeasure.cRegList[:] = circuitLine.cRegList
+        if pbCircuitLine.photonicGaussianMeasure.type == PBPhotonicGaussianMeasure.Type.Heterodyne:
+            for argument in circuitLine.data.heterodyneArgument:
+                arg = pbCircuitLine.photonicGaussianMeasure.heterodyne.add()
+                arg.r = argument[0]
+                arg.phi = argument[1]
+        elif pbCircuitLine.photonicGaussianMeasure.type == PBPhotonicGaussianMeasure.Type.PhotonCount:
+            pbCircuitLine.photonicGaussianMeasure.photonCount.cutoff = circuitLine.data.cutoff
+    elif isinstance(circuitLine.data, PhotonicFockGateOP):
+        pbCircuitLine.photonicFockGate = PBPhotonicFockGate.Value(circuitLine.data.name)
+        pbCircuitLine.argumentValueList[:] = circuitLine.data.argumentList
+    elif isinstance(circuitLine.data, PhotonicFockMeasureOP):
+        pbCircuitLine.photonicFockMeasure.cutoff = circuitLine.data.cutoff
 
     pbCircuitLine.qRegList[:] = circuitLine.qRegList
     return pbCircuitLine
 
 
 def getRotationArgumentList(data: 'QOperation') -> Tuple[List[int], List[float]]:
     if not (isinstance(data, RotationGateOP) or
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Condition/__init__.py` & `qcompute-3.3.1/QCompute/QPlatform/Condition/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Error.py` & `qcompute-3.3.1/QCompute/QPlatform/Error.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/InteractiveModule.py` & `qcompute-3.3.1/QCompute/QPlatform/InteractiveModule.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     [UnrollProcedureModule, CompositeGateModule, UnrollCircuitModule],
     [InverseCircuitModule, ReverseCircuitModule]
 ]
 
 BackendModuleDict = {
     BackendName.LocalBaiduSim2: _SimulatorModuleList,
     BackendName.LocalCuQuantum: _SimulatorModuleList,
+    BackendName.LocalBaiduSimPhotonic: [[], []],
     
     BackendName.CloudBaiduSim2Water: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Earth: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Thunder: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Heaven: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Wind: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Lake: _SimulatorModuleList,
@@ -130,15 +131,15 @@
                 verb = cmdList[0] if len(cmdList) >= 1 else None
                 arguments = cmdList[1:] if len(cmdList) >= 2 else None
                 self.do(verb, arguments)
             except Exception as ex:
                 print(ex)
 
     def refurbishStatus(self):
-        usingModuleList = filterModule(self.backendName, self.usingModuleList)
+        usingModuleList = filterModule(self.originProgram, self.backendName, self.usingModuleList)
         usingModuleNameList: List[str] = []
         reorderUsingModuleList: List[ModuleImplement] = []
         for module in usingModuleList:
             if module in self.usingModuleList:
                 usingModuleNameList.append(module.__class__.__name__)
                 reorderUsingModuleList.append(module)
         self.usingModuleList = reorderUsingModuleList
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/ProcedureParameterPool.py` & `qcompute-3.3.1/QCompute/QPlatform/ProcedureParameterPool.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Processor/ModuleFilter.py` & `qcompute-3.3.1/QCompute/QPlatform/Processor/ModuleFilter.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,78 +17,113 @@
 
 """
 Module Filter
 """
 from typing import List, Optional
 
 from QCompute.Define import Settings
+from QCompute.QProtobuf import PBProgram
 from QCompute.OpenModule import ModuleImplement
 from QCompute.OpenModule.CompositeGateModule import CompositeGateModule
 from QCompute.OpenModule.CompressGateModule import CompressGateModule
 from QCompute.OpenModule.InverseCircuitModule import InverseCircuitModule
 from QCompute.OpenModule.UnrollCircuitModule import UnrollCircuitModule
+from QCompute.OpenModule.CompressNoiseModule import CompressNoiseModule
 from QCompute.OpenModule.UnrollNoiseModule import UnrollNoiseModule
 from QCompute.OpenModule.UnrollProcedureModule import UnrollProcedureModule
 from QCompute.QPlatform import BackendName, Error, ModuleErrorCode
 
 
 
 FileErrorCode = 15
 
 
-def filterModule(backendName: Optional['BackendName'], moduleList: List['ModuleImplement']) \
+def filterModule(programe: PBProgram, backendName: Optional['BackendName'], moduleList: List['ModuleImplement']) \
         -> List['ModuleImplement']:
     if backendName is None:
         return moduleList
 
     if backendName in [
         BackendName.LocalBaiduSim2,
         BackendName.LocalCuQuantum,
+        BackendName.LocalBaiduSimPhotonic,
         
         BackendName.CloudBaiduSim2Water,
         BackendName.CloudBaiduSim2Earth,
         BackendName.CloudBaiduSim2Thunder,
         BackendName.CloudBaiduSim2Heaven,
         BackendName.CloudBaiduSim2Wind,
         BackendName.CloudBaiduSim2Lake,
         BackendName.CloudAerAtBD,
     ]:
-        return _filterSimulator(backendName, moduleList)
+        return _filterSimulator(programe, backendName, moduleList)
     
     else:
         return moduleList
 
 
-def _filterSimulator(backendName: BackendName, moduleList: List['ModuleImplement']) -> List['ModuleImplement']:
+def _filterSimulator(programe: PBProgram, backendName: BackendName, moduleList: List['ModuleImplement']) -> List[
+    'ModuleImplement']:
     unrollNoiseModule: Optional[UnrollNoiseModule] = None
+    compressNoiseModule: Optional[CompressNoiseModule] = None
     unrollProcedureModule: Optional[UnrollProcedureModule] = None
     compositeGateModule: Optional[CompositeGateModule] = None
     inverseCircuitModule: Optional[InverseCircuitModule] = None
     unrollCircuitModule: Optional[UnrollCircuitModule] = None
     compressGateModule: Optional[CompressGateModule] = None
     ret: List['ModuleImplement'] = []
     for module in moduleList:
         
-        if module.__class__.__name__ == 'UnrollNoiseModule':
-            unrollNoiseModule = module
+        if backendName in [
+            
+        ] and module.__class__.__name__ == 'CompressGateModule' \
+                and not module.disable:
+            raise Error.ArgumentError(f'Unsupported {module.__class__.__name__} in {backendName.name}',
+                                      ModuleErrorCode,
+                                      FileErrorCode, 2)
         elif module.__class__.__name__ == 'UnrollProcedureModule':
             unrollProcedureModule = module
         elif module.__class__.__name__ == 'CompositeGateModule':
             compositeGateModule = module
         elif module.__class__.__name__ == 'InverseCircuitModule':
             inverseCircuitModule = module
         elif module.__class__.__name__ == 'UnrollCircuitModule':
             unrollCircuitModule = module
         elif module.__class__.__name__ == 'CompressGateModule':
             compressGateModule = module
+        if module.__class__.__name__ == 'UnrollNoiseModule':
+            unrollNoiseModule = module
+        if module.__class__.__name__ == 'CompressNoiseModule':
+            compressNoiseModule = module
         elif not module.disable:
             ret.append(module)
 
-    if unrollNoiseModule is not None:
-        return moduleList
+    if backendName == BackendName.LocalBaiduSimPhotonic:
+        return []
+
+    if len(programe.body.noiseMap) > 0:
+        if unrollProcedureModule is not None:
+            if not unrollProcedureModule.disable:
+                ret.append(unrollProcedureModule)
+        else:
+            ret.append(UnrollProcedureModule())
+
+        if unrollNoiseModule is not None:
+            if not unrollNoiseModule.disable:
+                ret.append(unrollNoiseModule)
+        else:
+            ret.append(UnrollNoiseModule())
+
+        if compressNoiseModule is not None:
+            if not compressNoiseModule.disable:
+                ret.append(compressNoiseModule)
+        else:
+            ret.append(CompressNoiseModule())
+
+        return ret
 
     if unrollProcedureModule is not None:
         if not unrollProcedureModule.disable:
             ret.append(unrollProcedureModule)
     else:
         ret.append(UnrollProcedureModule())
 
@@ -167,10 +202,14 @@
             print(
                 f'- {moduleName}: The subprocedure decomposition module expands all the subprocedures in the quantum circuit.'
             )
         elif moduleName == 'UnrollNoiseModule':
             print(
                 f'- {moduleName}: The noise unrolling module assigns all noises to the quantum circuit by user-defined rules.'
             )
+        elif moduleName == 'CompressNoiseModule':
+            print(
+                f'- {moduleName}: The compress noise module compress single qubit noiseless gates into two-qubit gates and reorder gates to construct a more dense circuit.'
+            )
     if len(moduleList) > 0:
         print(
             '*Tips: to close the output info, you can insert `QCompute.Define.Settings.outputInfo = False` at the beginning of your code.')
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Processor/PostProcessor.py` & `qcompute-3.3.1/QCompute/QPlatform/Processor/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Processor/PreProcess.py` & `qcompute-3.3.1/QCompute/QPlatform/Processor/PreProcess.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         if rerangeQReg:
             compactedQRegDict[qReg] = index
         else:
             compactedQRegDict[qReg] = qReg
 
     measured = False
     for circuitLine in program.body.circuit:
-        op = circuitLine.WhichOneof('op')
-        if measured and op != 'measure':
+        op: str = circuitLine.WhichOneof('op')
+        if measured and 'measure' not in op.lower():
             raise Error.ArgumentError('Measure must be the last operation!', ModuleErrorCode, FileErrorCode, 1)
 
         circuitLine.qRegList[:] = [compactedQRegDict[qReg] for qReg in circuitLine.qRegList]
 
-        if op == 'measure':
+        if 'measure' in op.lower():
             measured = True
             for index, cReg in enumerate(circuitLine.measure.cRegList):
                 qReg = circuitLine.qRegList[index]
                 if qReg in compactedCRegDict:
                     raise Error.ArgumentError('Measure must be once on a QReg', ModuleErrorCode, FileErrorCode, 2)
                 if cReg in compactedCRegDict.values():
                     raise Error.ArgumentError('Measure must be once on a CReg', ModuleErrorCode, FileErrorCode, 3)
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/Processor/__init__.py` & `qcompute-3.3.1/QCompute/QPlatform/Processor/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QEnv.py` & `qcompute-3.3.1/QCompute/QPlatform/QEnv.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from QCompute import Define, UnrollProcedureModule
 from QCompute.Define import Settings
 from QCompute.Define.Utils import loadPythonModule, clearOutputDir
 from QCompute.OpenConvertor.CircuitToDrawConsole import CircuitToDrawConsole
 from QCompute.OpenModule import ModuleImplement
 from QCompute.OpenModule.UnrollNoiseModule import UnrollNoiseModule
-from QCompute.OpenSimulator import QResult, QImplement
+from QCompute.OpenSimulator import QResult, QImplement, QPhotonicResult
 from QCompute.QPlatform import Error, ModuleErrorCode, BackendName, getBackendFromName
 from QCompute.QPlatform.CircuitTools import QEnvToProtobuf
 from QCompute.QPlatform.InteractiveModule import InteractiveModule
 from QCompute.QPlatform.ProcedureParameterPool import ProcedureParameterPool
 from QCompute.QPlatform.Processor.ModuleFilter import filterModule, printModuleListDescription
 from QCompute.QPlatform.Processor.PostProcessor import formatMeasure
 from QCompute.QPlatform.QNoise import QNoise, QNoiseDefine
@@ -238,15 +238,15 @@
                 Settings.drawCircuitControl is None or moduleStep in Settings.drawCircuitControl):
             asciiPic = circuitToDrawTerminal.convert(self.program)
             print('Origin circuit:')
             print(asciiPic)
 
         if applyModule:
             # filter the circuit by Modules
-            usedModuleList = filterModule(self.backendName, self.usingModuleList)
+            usedModuleList = filterModule(program, self.backendName, self.usingModuleList)
             for module in usedModuleList:
                 moduleStep += 1
                 self.program = module(self.program)
 
                 if Settings.outputInfo and (
                         Settings.drawCircuitControl is None or moduleStep in Settings.drawCircuitControl):
                     asciiPic = circuitToDrawTerminal.convert(self.program)
@@ -295,28 +295,22 @@
         {status: 'failed', reason: ''}
         """
 
         self.shots = shots
 
         ret: Dict[str, Union[str, Dict[str, int]]] = None
         if self.backendName.value.startswith('local_'):
-            if len(self.noiseDefineMap) > 0:
-                self.usingModuleList.clear()
-                self.module(UnrollProcedureModule())
-                self.module(UnrollNoiseModule())
             usedModuleList = self.publish()  # circuit in Protobuf format
             moduleList = [{
                 'module': module.__class__.__name__,
                 'arguments': module.arguments
             } for module in usedModuleList]
             ret = self._localCommit(fetchMeasure, moduleList)
         elif self.backendName.value.startswith('cloud_'):
             self.publish(False)  # circuit in Protobuf format
-
-            
             moduleList = [(module.__class__.__name__, module.arguments) for module in self.usingModuleList]
             moduleList.extend(self.usedServerModuleList)
 
             ret = self._cloudCommit(fetchMeasure, downloadResult, moduleList, notes
                                     
                                     )
         elif self.backendName.value.startswith('service_'):
@@ -373,64 +367,110 @@
         if backend.result.code != 0:
             if backend.result.log != '':
                 logFd, logFn = tempfile.mkstemp(prefix="local.", suffix=".log", dir=Define.outputDirPath)
                 with os.fdopen(logFd, "wt") as file:
                     file.write(backend.result.log)
             return {"status": "error", "reason": backend.result.log}
 
-        if backend.result.counts is not None or backend.result.state is not None:
-            cRegCount = max(self.program.head.usingCRegList) + 1
-
-            if backend.result.counts is not None:
-                backend.result.counts = formatMeasure(backend.result.counts, cRegCount)
-
-            try:
-                ret = QResult()
-                ret.fromJson(backend.result.output)
-                ret.moduleList = moduleList
-                backend.result.output = ret.toJson()
-            except Exception as ex:
-                print(ex)
-
-            originFd, originFn = tempfile.mkstemp(prefix="local.", suffix=".origin.json", dir=Define.outputDirPath)
-            rsplitedFn = originFn.rsplit('.', 4)
-            taskResult = {'taskId': rsplitedFn[-3], 'status': 'success'}
-            if backend.result.output != '':
-                with os.fdopen(originFd, "wt") as fObj:
-                    fObj.write(backend.result.output)
-                taskResult["origin"] = originFn
-            else:
-                os.close(originFd)
+        if 'photonic' not in self.backendName.value:
+            if backend.result.counts is not None or backend.result.state is not None:
+                cRegCount = max(self.program.head.usingCRegList) + 1
+                if backend.result.counts is not None:
+                    backend.result.counts = formatMeasure(backend.result.counts, cRegCount)
+
+                try:
+                    ret = QResult()
+                    ret.fromJson(backend.result.output)
+                    ret.moduleList = moduleList
+                    backend.result.output = ret.toJson()
+                except Exception as ex:
+                    print(ex)
+
+                originFd, originFn = tempfile.mkstemp(prefix="local.", suffix=".origin.json", dir=Define.outputDirPath)
+                rsplitedFn = originFn.rsplit('.', 4)
+                taskResult = {'taskId': rsplitedFn[-3], 'status': 'success'}
+                if backend.result.output != '':
+                    with os.fdopen(originFd, "wt") as fObj:
+                        fObj.write(backend.result.output)
+                    taskResult["origin"] = originFn
+                else:
+                    os.close(originFd)
+
+                if backend.result.counts is not None:
+                    measureFn = Path(originFn[:-12] + '.measure.json')
+                    measureFn.write_text(json.dumps(backend.result.counts), encoding='utf-8')
+                elif backend.result.state is not None:
+                    measureFn = Path(originFn[:-12] + '.measure.txt')
+                    measureFn.write_text(str(backend.result.state), encoding='utf-8')
+                taskResult["measure"] = str(measureFn)
+
+                if backend.result.log != '':
+                    logFn = Path(originFn[:-12] + '.log')
+                    logFn.write_text(backend.result.log, encoding='utf-8')
+                    taskResult["log"] = str(logFn)
+
+                taskResult["moduleList"] = moduleList
+
+                if fetchMeasure:
+                    taskResult['ancilla'] = {}
+                    taskResult['ancilla']['usedQRegList'] = backend.result.ancilla.usedQRegList
+                    taskResult['ancilla']['usedCRegList'] = backend.result.ancilla.usedCRegList
+                    taskResult['ancilla']['compactedQRegDict'] = backend.result.ancilla.compactedQRegDict
+                    taskResult['ancilla']['compactedCRegDict'] = backend.result.ancilla.compactedCRegDict
+                    taskResult['shots'] = backend.result.shots
+                    taskResult['counts'] = backend.result.counts
+                    taskResult['state'] = backend.result.state
 
-            if backend.result.counts is not None:
-                measureFn = Path(originFn[:-12] + '.measure.json')
-                measureFn.write_text(json.dumps(backend.result.counts), encoding='utf-8')
-            elif backend.result.state is not None:
-                measureFn = Path(originFn[:-12] + '.measure.txt')
-                measureFn.write_text(str(backend.result.state), encoding='utf-8')
-            taskResult["measure"] = str(measureFn)
-
-            if backend.result.log != '':
-                logFn = Path(originFn[:-12] + '.log')
-                logFn.write_text(backend.result.log, encoding='utf-8')
-                taskResult["log"] = str(logFn)
-
-            taskResult["moduleList"] = moduleList
-
-            if fetchMeasure:
-                taskResult['ancilla'] = {}
-                taskResult['ancilla']['usedQRegList'] = backend.result.ancilla.usedQRegList
-                taskResult['ancilla']['usedCRegList'] = backend.result.ancilla.usedCRegList
-                taskResult['ancilla']['compactedQRegDict'] = backend.result.ancilla.compactedQRegDict
-                taskResult['ancilla']['compactedCRegDict'] = backend.result.ancilla.compactedCRegDict
-                taskResult['shots'] = backend.result.shots
-                taskResult['counts'] = backend.result.counts
-                taskResult['state'] = backend.result.state
+                return taskResult
+        else:
+            if backend.result.value is not None or backend.result.counts is not None:
+                try:
+                    ret = QPhotonicResult()
+                    ret.fromJson(backend.result.output)
+                    ret.moduleList = moduleList
+                    backend.result.output = ret.toJson()
+                except Exception as ex:
+                    print(ex)
+
+                originFd, originFn = tempfile.mkstemp(prefix="local.", suffix=".origin.json", dir=Define.outputDirPath)
+                rsplitedFn = originFn.rsplit('.', 4)
+                taskResult = {'taskId': rsplitedFn[-3], 'status': 'success'}
+                if backend.result.output != '':
+                    with os.fdopen(originFd, "wt") as fObj:
+                        fObj.write(backend.result.output)
+                    taskResult["origin"] = originFn
+                else:
+                    os.close(originFd)
+
+                if backend.result.value is not None:
+                    measureFn = Path(originFn[:-12] + '.measure.json')
+                    measureFn.write_text(json.dumps(backend.result.value), encoding='utf-8')
+                elif backend.result.state is not None:
+                    measureFn = Path(originFn[:-12] + '.measure.txt')
+                    measureFn.write_text(str(backend.result.state), encoding='utf-8')
+                taskResult["measure"] = str(measureFn)
+
+                if backend.result.log != '':
+                    logFn = Path(originFn[:-12] + '.log')
+                    logFn.write_text(backend.result.log, encoding='utf-8')
+                    taskResult["log"] = str(logFn)
+
+                taskResult["moduleList"] = moduleList
+
+                if fetchMeasure:
+                    taskResult['ancilla'] = {}
+                    taskResult['ancilla']['usedQRegList'] = backend.result.ancilla.usedQRegList
+                    taskResult['ancilla']['usedCRegList'] = backend.result.ancilla.usedCRegList
+                    taskResult['ancilla']['compactedQRegDict'] = backend.result.ancilla.compactedQRegDict
+                    taskResult['ancilla']['compactedCRegDict'] = backend.result.ancilla.compactedCRegDict
+                    taskResult['shots'] = backend.result.shots
+                    taskResult['value'] = backend.result.value
+                    taskResult['state'] = backend.result.state
 
-            return taskResult
+                return taskResult
 
         return {"status": "failed", "reason": backend.result.log}
 
     def _cloudCommit(self, fetchMeasure: bool, downloadResult: bool, moduleList: List[Tuple[str, Any]],
                      notes: str
                      
                      ) -> Dict[
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QEnvOperation.py` & `qcompute-3.3.1/QCompute/QPlatform/QEnvOperation.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/AmplitudeDamping.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/AmplitudeDamping.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/BitFlip.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/BitFlip.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/BitPhaseFlip.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/BitPhaseFlip.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/CustomizedNoise.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/CustomizedNoise.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/Depolarizing.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/Depolarizing.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/PauliNoise.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/PauliNoise.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseDamping.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/PhaseDamping.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseFlip.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/PhaseFlip.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/ResetNoise.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/ResetNoise.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/Utilities.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/Utilities.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QNoise/__init__.py` & `qcompute-3.3.1/QCompute/QPlatform/QNoise/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/Barrier.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/Barrier.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/CompositeGate.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/CompositeGate.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/CustomizedGate.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/CustomizedGate.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/FixedGate.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/FixedGate.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/Measure.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/Measure.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/QProcedure.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/QProcedure.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/RotationGate.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/RotationGate.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,60 +272,60 @@
 
     It contains two qubits: the control qubit and the target qubit.
 
     The rotation gate is performed on the target qubit only when the control qubit is taking effect.
     """
     uGateArgumentList = angleList = [theta, phi, lamda]
     gate = RotationGateOP('CU', 2, CUOpAllowArgumentCounts, angleList, uGateArgumentList)
-    gate.generateMatrix = gate._generateCUMatrix()
+    gate.generateMatrix = gate._generateCUMatrix
     return gate
 
 
 CU.type = 'RotationGateOP'
 CU.allowArgumentCounts = CUOpAllowArgumentCounts
 
 
 def CRX(theta: 'RotationArgument') -> 'OperationFunc':
     """
     Controlled-RX gate.
     """
     angleList = [theta]
     uGateArgumentList = [theta, -numpy.math.pi / 2, numpy.math.pi / 2]
     gate = RotationGateOP('CRX', 2, CRXOpAllowArgumentCounts, angleList, uGateArgumentList)
-    gate.generateMatrix = gate._generateCUMatrix()
+    gate.generateMatrix = gate._generateCUMatrix
     return gate
 
 
 CRX.type = 'RotationGateOP'
 CRX.allowArgumentCounts = CRXOpAllowArgumentCounts
 
 
 def CRY(theta: 'RotationArgument') -> 'OperationFunc':
     """
     Controlled-RY Gate.
     """
     angleList = [theta]
     uGateArgumentList = [theta, 0, 0]
     gate = RotationGateOP('CRY', 2, CRYOpAllowArgumentCounts, angleList, uGateArgumentList)
-    gate.generateMatrix = gate._generateCUMatrix()
+    gate.generateMatrix = gate._generateCUMatrix
     return gate
 
 
 CRY.type = 'RotationGateOP'
 CRY.allowArgumentCounts = CRYOpAllowArgumentCounts
 
 
 def CRZ(lamda: 'RotationArgument') -> 'OperationFunc':
     """
     Controlled-RZ Gate.
     """
     angleList = [lamda]
     uGateArgumentList = [0, 0, lamda]
     gate = RotationGateOP('CRZ', 2, CRZOpAllowArgumentCounts, angleList, uGateArgumentList)
-    gate.generateMatrix = gate._generateCUMatrix()
+    gate.generateMatrix = gate._generateCUMatrix
     return gate
 
 
 CRZ.type = 'RotationGateOP'
 CRZ.allowArgumentCounts = CRZOpAllowArgumentCounts
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QOperation/__init__.py` & `qcompute-3.3.1/QCompute/QPlatform/QOperation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Quantum Operation
 """
-from typing import List, Union, Optional, Callable, TYPE_CHECKING
+from typing import List, Union, Optional, Callable, TYPE_CHECKING, Tuple
 
 import numpy
 
 from QCompute.QPlatform import Error, ModuleErrorCode
 from QCompute.QPlatform.ProcedureParameterPool import ProcedureParameterStorage
 
 if TYPE_CHECKING:
@@ -30,14 +30,16 @@
     from QCompute.QPlatform.QOperation.RotationGate import RotationGateOP
     from QCompute.QPlatform.QOperation.CompositeGate import CompositeGateOP
     from QCompute.QPlatform.QOperation.CustomizedGate import CustomizedGateOP
     from QCompute.QPlatform.QOperation.QProcedure import QProcedureOP
     from QCompute.QPlatform.QOperation.Barrier import BarrierOP
     from QCompute.QPlatform.QOperation.Measure import MeasureOP
     from QCompute.QPlatform.QRegPool import QRegStorage
+    from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianGate import PhotonicGaussianGateOP
+    from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianMeasure import PhotonicGaussianMeasureOP
 
 FileErrorCode = 9
 
 OperationFunc = Callable[[*'QRegStorage'], None]
 RotationArgument = Union[int, float, ProcedureParameterStorage]
 
 
@@ -51,48 +53,59 @@
         self.name = name
         self.bits = bits
         self.matrix = matrix
 
     def getMatrix(self) -> numpy.ndarray:
         if self.__class__.__name__ == 'FixedGateOP':
             return self.matrix
-        elif self.__class__.__name__ == 'RotationGateOP':
+        elif self.__class__.__name__ == 'RotationGateOP' or self.__class__.__name__ == 'PhotonicFockGateOP':
             if self.matrix is None:
-                self.generateMatrix()
-            return self.matrix
+                return self.generateMatrix()  # include generate self.matrix
+            else:
+                return self.matrix
         elif self.__class__.__name__ == 'CustomizedGateOP':
             return self.matrix
         else:
             raise Error.ArgumentError(f'{self.__class__.__name__} do not have matrix!', ModuleErrorCode, FileErrorCode,
                                       1)
 
+    def getMatrixAndVector(self) -> Tuple[numpy.ndarray, numpy.ndarray]:
+        if self.__class__.__name__ == 'PhotonicGaussianGateOP':
+            if self.matrix is None:
+                return self.generateMatrixAndVector()  # include generate self.matrix and self.displace_vector
+            else:
+                return self.matrix, self.displace_verctor
+        else:
+            raise Error.ArgumentError(f'{self.__class__.__name__} only support photonic gate!', ModuleErrorCode,
+                                      FileErrorCode, 2)
+
     def getInversed(self) -> 'QOperation':
         return self
 
     def _op(self, qRegList: List['QRegStorage']) -> None:
         """
         Quantum operation base
 
         :param qRegList: quantum register list
         """
         env = qRegList[0].env
         for qReg in qRegList:
             if qReg.env != env:
-                raise Error.ArgumentError('QReg must belong to the same env!', ModuleErrorCode, FileErrorCode, 2)
+                raise Error.ArgumentError('QReg must belong to the same env!', ModuleErrorCode, FileErrorCode, 3)
 
         if env.__class__.__name__ == 'QProcedure':
-            raise Error.ArgumentError('QProcedure should not be operated!', ModuleErrorCode, FileErrorCode, 3)
+            raise Error.ArgumentError('QProcedure should not be operated!', ModuleErrorCode, FileErrorCode, 4)
 
         if self.bits is not None and self.bits != len(
                 qRegList):  # Barrier and QProcedure does not match bits configuration
-            raise Error.ArgumentError('The number of QReg must match the setting!', ModuleErrorCode, FileErrorCode, 4)
+            raise Error.ArgumentError('The number of QReg must match the setting!', ModuleErrorCode, FileErrorCode, 5)
 
         if len(qRegList) != len(set(qReg for qReg in qRegList)):
             raise Error.ArgumentError('QReg of operators in circuit are not repeatable!', ModuleErrorCode,
-                                      FileErrorCode, 5)
+                                      FileErrorCode, 6)
 
         circuitLine = CircuitLine()
         circuitLine.data = self
         circuitLine.qRegList = [qReg.index for qReg in qRegList]
         env.circuit.append(circuitLine)
 
     def _opMeasure(self, qRegList: List['QRegStorage'], cRegList: List[int]) -> None:
@@ -100,57 +113,59 @@
         Measure operation base.
 
         :param qRegList: quantum register list
         :param cRegList: classic register list
         """
         if len(qRegList) != len(cRegList):
             raise Error.ArgumentError('QReg and CReg in measure must have same count!', ModuleErrorCode, FileErrorCode,
-                                      6)
+                                      7)
 
         env = qRegList[0].env
         for qReg in qRegList:
             if qReg.env != env:
-                raise Error.ArgumentError('QReg must belong to the same env!', ModuleErrorCode, FileErrorCode, 7)
+                raise Error.ArgumentError('QReg must belong to the same env!', ModuleErrorCode, FileErrorCode, 8)
 
         if env.__class__.__name__ == 'QProcedure':
-            raise Error.ArgumentError('QProcedure must not be measured!', ModuleErrorCode, FileErrorCode, 8)
+            raise Error.ArgumentError('QProcedure must not be measured!', ModuleErrorCode, FileErrorCode, 9)
 
         if len(qRegList) <= 0:
-            raise Error.ArgumentError('Must have QReg in measure!', ModuleErrorCode, FileErrorCode, 9)
+            raise Error.ArgumentError('Must have QReg in measure!', ModuleErrorCode, FileErrorCode, 10)
 
         if len(qRegList) != len(set(qReg for qReg in qRegList)):
             raise Error.ArgumentError('QReg of measure in circuit are not repeatable!', ModuleErrorCode,
-                                      FileErrorCode, 10)
+                                      FileErrorCode, 11)
 
         for qReg in qRegList:  # Only in QEnv
             if qReg.index in env.measuredQRegSet:
-                raise Error.ArgumentError('Measure must be once on a QReg!', ModuleErrorCode, FileErrorCode, 11)
+                raise Error.ArgumentError('Measure must be once on a QReg!', ModuleErrorCode, FileErrorCode, 12)
             env.measuredQRegSet.add(qReg.index)
 
         if len(cRegList) <= 0:
-            raise Error.ArgumentError('Must have CReg in measure!', ModuleErrorCode, FileErrorCode, 12)
+            raise Error.ArgumentError('Must have CReg in measure!', ModuleErrorCode, FileErrorCode, 13)
 
         if len(cRegList) != len(set(cReg for cReg in cRegList)):
             raise Error.ArgumentError('CReg of measure in circuit are not repeatable!', ModuleErrorCode,
-                                      FileErrorCode, 13)
+                                      FileErrorCode, 14)
 
         for cReg in cRegList:  # Only in QEnv
             if cReg in env.measuredCRegSet:
-                raise Error.ArgumentError('Measure must be once on a CReg!', ModuleErrorCode, FileErrorCode, 14)
+                raise Error.ArgumentError('Measure must be once on a CReg!', ModuleErrorCode, FileErrorCode, 15)
             env.measuredCRegSet.add(cReg)
 
         circuitLine = CircuitLine()
         circuitLine.data = self
         circuitLine.qRegList = [qReg.index for qReg in qRegList]
         circuitLine.cRegList = cRegList
         env.circuit.append(circuitLine)
 
 
 Operation = Union[
-    'FixedGateOP', 'RotationGateOP', 'CompositeGateOP', 'CustomizedGateOP', 'QProcedureOP', 'BarrierOP', 'MeasureOP']
+    'FixedGateOP', 'RotationGateOP', 'CompositeGateOP', 'CustomizedGateOP', 'QProcedureOP', 'BarrierOP', 'MeasureOP',
+    'PhotonicGaussianGateOP', 'PhotonicGaussianMeasureOP', 'PhotonicFockGateOP', 'PhotonicFockMeasureOP'
+]
 
 
 class CircuitLine:
     """
     Circuit Line
     """
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QRegPool.py` & `qcompute-3.3.1/QCompute/QPlatform/QRegPool.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QStatus.py` & `qcompute-3.3.1/QCompute/QPlatform/QStatus.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QPlatform/QTask.py` & `qcompute-3.3.1/QCompute/QPlatform/QTask.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
                             if not Settings.cloudTaskDoNotWriteFile:
                                 result["origin"] = str(self.originFile)
                                 originResult = self._fetchOriginResult()
                             else:
                                 originResult = self.originJson
 
                             result["moduleList"] = originResult["moduleList"]
-                            result["batchID"] = originResult["batchID"]
+                            result["batchID"] = originResult.get("batchID")
 
                             if fetchMeasure:
                                 if not Settings.cloudTaskDoNotWriteFile:
                                     result["counts"] = self._fetchMeasureResult()
                                 else:
                                     result["counts"] = self.measureJson
                             elif not Settings.cloudTaskDoNotWriteFile:
```

### Comparing `qcompute-3.3.0/QCompute/QPlatform/__init__.py` & `qcompute-3.3.1/QCompute/QPlatform/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,34 @@
     Example: 
     
     env = QEnv()
     
     env.backend(BackendName.LocalCuQuantum)
     """
 
+    LocalBaiduSimPhotonic = 'local_baidu_sim_photonic'
+    """
+    Local Baidu Sim Photonic Gaussian And Fock
+
+    Example: 
+
+    env = QEnv()
+
+    env.backend(BackendName.LocalBaiduSimPhotonic)
+    """
+
     LocalBaiduSim2WithNoise = 'local_baidu_sim2'
     """
-    Local Baidu Sim2 With Noise
+    Local Baidu Sim2 With Noise (Deprecated, should use LocalBaiduSim2)
+
+    Example: 
+
+    env = QEnv()
+
+    env.backend(BackendName.LocalBaiduSim2WithNoise)
     """
 
     
 
     CloudBaiduSim2Water = 'cloud_baidu_sim2_water'
     """
     Cloud Baidu Sim2 Water
```

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/Complex_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/Complex_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/PlatformStruct_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/PlatformStruct_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from QCompute.QProtobuf.Library import QOperation_pb2 as QOperation__pb2
+from QCompute.QProtobuf.Library import QPhotonicOperation_pb2 as QPhotonicOperation__pb2
 from QCompute.QProtobuf.Library import QNoise_pb2 as QNoise__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14PlatformStruct.proto\x1a\x10QOperation.proto\x1a\x0cQNoise.proto\"`\n\x07Program\x12\x12\n\nsdkVersion\x18\x01 \x01(\t\x12\x13\n\x04head\x18\x02 \x01(\x0b\x32\x05.Head\x12\x13\n\x04\x62ody\x18\x03 \x01(\x0b\x32\x05.Body\x12\x17\n\x06source\x18\x04 \x01(\x0b\x32\x07.Source\"4\n\x04Head\x12\x15\n\rusingQRegList\x18\x01 \x03(\r\x12\x15\n\rusingCRegList\x18\x02 \x03(\r\"\x81\x02\n\x04\x42ody\x12\x1d\n\x07\x63ircuit\x18\x01 \x03(\x0b\x32\x0c.CircuitLine\x12-\n\x0cprocedureMap\x18\x02 \x03(\x0b\x32\x17.Body.ProcedureMapEntry\x12%\n\x08noiseMap\x18\x03 \x03(\x0b\x32\x13.Body.NoiseMapEntry\x1a@\n\x11ProcedureMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.QProcedure:\x02\x38\x01\x1a\x42\n\rNoiseMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12 \n\x05value\x18\x02 \x01(\x0b\x32\x11.QNoiseDefineList:\x02\x38\x01\"\x16\n\x06Source\x12\x0c\n\x04qasm\x18\x01 \x01(\t\"\xd9\x02\n\x0b\x43ircuitLine\x12\x1f\n\tfixedGate\x18\x01 \x01(\x0e\x32\n.FixedGateH\x00\x12%\n\x0crotationGate\x18\x02 \x01(\x0e\x32\r.RotationGateH\x00\x12)\n\x0e\x63ustomizedGate\x18\x03 \x01(\x0b\x32\x0f.CustomizedGateH\x00\x12\'\n\rcompositeGate\x18\x04 \x01(\x0e\x32\x0e.CompositeGateH\x00\x12\x17\n\rprocedureName\x18\x05 \x01(\tH\x00\x12\x1b\n\x07measure\x18\x06 \x01(\x0b\x32\x08.MeasureH\x00\x12\x11\n\x07\x62\x61rrier\x18\x07 \x01(\x08H\x00\x12\x10\n\x08qRegList\x18\x08 \x03(\r\x12\x19\n\x11\x61rgumentValueList\x18\t \x03(\x01\x12\x16\n\x0e\x61rgumentIdList\x18\n \x03(\x05\x12\x1a\n\tnoiseList\x18\x0b \x03(\x0b\x32\x07.QNoiseB\x04\n\x02op\"Z\n\nQProcedure\x12\x16\n\x0eparameterCount\x18\x01 \x01(\r\x12\x15\n\rusingQRegList\x18\x02 \x03(\r\x12\x1d\n\x07\x63ircuit\x18\x03 \x03(\x0b\x32\x0c.CircuitLineb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14PlatformStruct.proto\x1a\x10QOperation.proto\x1a\x18QPhotonicOperation.proto\x1a\x0cQNoise.proto\"`\n\x07Program\x12\x12\n\nsdkVersion\x18\x01 \x01(\t\x12\x13\n\x04head\x18\x02 \x01(\x0b\x32\x05.Head\x12\x13\n\x04\x62ody\x18\x03 \x01(\x0b\x32\x05.Body\x12\x17\n\x06source\x18\x04 \x01(\x0b\x32\x07.Source\"4\n\x04Head\x12\x15\n\rusingQRegList\x18\x01 \x03(\r\x12\x15\n\rusingCRegList\x18\x02 \x03(\r\"\x81\x02\n\x04\x42ody\x12\x1d\n\x07\x63ircuit\x18\x01 \x03(\x0b\x32\x0c.CircuitLine\x12-\n\x0cprocedureMap\x18\x02 \x03(\x0b\x32\x17.Body.ProcedureMapEntry\x12%\n\x08noiseMap\x18\x03 \x03(\x0b\x32\x13.Body.NoiseMapEntry\x1a@\n\x11ProcedureMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.QProcedure:\x02\x38\x01\x1a\x42\n\rNoiseMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12 \n\x05value\x18\x02 \x01(\x0b\x32\x11.QNoiseDefineList:\x02\x38\x01\"\x16\n\x06Source\x12\x0c\n\x04qasm\x18\x01 \x01(\t\"\xb1\x04\n\x0b\x43ircuitLine\x12\x1f\n\tfixedGate\x18\x01 \x01(\x0e\x32\n.FixedGateH\x00\x12%\n\x0crotationGate\x18\x02 \x01(\x0e\x32\r.RotationGateH\x00\x12)\n\x0e\x63ustomizedGate\x18\x03 \x01(\x0b\x32\x0f.CustomizedGateH\x00\x12\'\n\rcompositeGate\x18\x04 \x01(\x0e\x32\x0e.CompositeGateH\x00\x12\x17\n\rprocedureName\x18\x05 \x01(\tH\x00\x12\x1b\n\x07measure\x18\x06 \x01(\x0b\x32\x08.MeasureH\x00\x12\x11\n\x07\x62\x61rrier\x18\x07 \x01(\x08H\x00\x12\x35\n\x14photonicGaussianGate\x18\x0c \x01(\x0e\x32\x15.PhotonicGaussianGateH\x00\x12;\n\x17photonicGaussianMeasure\x18\r \x01(\x0b\x32\x18.PhotonicGaussianMeasureH\x00\x12-\n\x10photonicFockGate\x18\x0e \x01(\x0e\x32\x11.PhotonicFockGateH\x00\x12\x33\n\x13photonicFockMeasure\x18\x0f \x01(\x0b\x32\x14.PhotonicFockMeasureH\x00\x12\x10\n\x08qRegList\x18\x08 \x03(\r\x12\x19\n\x11\x61rgumentValueList\x18\t \x03(\x01\x12\x16\n\x0e\x61rgumentIdList\x18\n \x03(\x05\x12\x1a\n\tnoiseList\x18\x0b \x03(\x0b\x32\x07.QNoiseB\x04\n\x02op\"Z\n\nQProcedure\x12\x16\n\x0eparameterCount\x18\x01 \x01(\r\x12\x15\n\rusingQRegList\x18\x02 \x03(\r\x12\x1d\n\x07\x63ircuit\x18\x03 \x03(\x0b\x32\x0c.CircuitLineb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'PlatformStruct_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BODY_PROCEDUREMAPENTRY._options = None
   _BODY_PROCEDUREMAPENTRY._serialized_options = b'8\001'
   _BODY_NOISEMAPENTRY._options = None
   _BODY_NOISEMAPENTRY._serialized_options = b'8\001'
-  _PROGRAM._serialized_start=56
-  _PROGRAM._serialized_end=152
-  _HEAD._serialized_start=154
-  _HEAD._serialized_end=206
-  _BODY._serialized_start=209
-  _BODY._serialized_end=466
-  _BODY_PROCEDUREMAPENTRY._serialized_start=334
-  _BODY_PROCEDUREMAPENTRY._serialized_end=398
-  _BODY_NOISEMAPENTRY._serialized_start=400
-  _BODY_NOISEMAPENTRY._serialized_end=466
-  _SOURCE._serialized_start=468
-  _SOURCE._serialized_end=490
-  _CIRCUITLINE._serialized_start=493
-  _CIRCUITLINE._serialized_end=838
-  _QPROCEDURE._serialized_start=840
-  _QPROCEDURE._serialized_end=930
+  _PROGRAM._serialized_start=82
+  _PROGRAM._serialized_end=178
+  _HEAD._serialized_start=180
+  _HEAD._serialized_end=232
+  _BODY._serialized_start=235
+  _BODY._serialized_end=492
+  _BODY_PROCEDUREMAPENTRY._serialized_start=360
+  _BODY_PROCEDUREMAPENTRY._serialized_end=424
+  _BODY_NOISEMAPENTRY._serialized_start=426
+  _BODY_NOISEMAPENTRY._serialized_end=492
+  _SOURCE._serialized_start=494
+  _SOURCE._serialized_end=516
+  _CIRCUITLINE._serialized_start=519
+  _CIRCUITLINE._serialized_end=1080
+  _QPROCEDURE._serialized_start=1082
+  _QPROCEDURE._serialized_end=1172
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/QNoise_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/QNoise_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/QObj_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/QObj_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/QOperation_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/QOperation_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/Library/__init__.py` & `qcompute-3.3.1/QCompute/QProtobuf/Library/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/QProtobuf/__init__.py` & `qcompute-3.3.1/QCompute/QProtobuf/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,13 +20,16 @@
 """
 
 from QCompute.QProtobuf.Library.Complex_pb2 import Matrix as PBMatrix
 from QCompute.QProtobuf.Library.PlatformStruct_pb2 import Program as PBProgram, CircuitLine as PBCircuitLine, \
     QProcedure as PBQProcedure
 from QCompute.QProtobuf.Library.QOperation_pb2 import FixedGate as PBFixedGate, RotationGate as PBRotationGate, \
     CustomizedGate as PBCustomizedGate, CompositeGate as PBCompositeGate, Measure as PBMeasure
+from QCompute.QProtobuf.Library.QPhotonicOperation_pb2 import \
+    PhotonicGaussianGate as PBPhotonicGaussianGate, PhotonicGaussianMeasure as PBPhotonicGaussianMeasure, \
+    PhotonicFockGate as PBPhotonicFockGate, PhotonicFockMeasure as PBPhotonicFockMeasure
 from QCompute.QProtobuf.Library.QNoise_pb2 import QNoise as PBQNoise, QNoiseDefine as PBQNoiseDefine
 from QCompute.QProtobuf.Library.QObj_pb2 import QObject as PBQObject, Experiment as PBExperiment, \
     Instruction as PBInstruction
 from QCompute.QProtobuf.Library.UniversalBlindQuantumComputing_pb2 import InitState as PBUbpcInitState, \
     EncryptedMeasureReq as PBEncryptedMeasureReq, EncryptedMeasureRes as PBEncryptedMeasureRes
```

### Comparing `qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/__init__.py` & `qcompute-3.3.1/QCompute/Utilize/ControlledCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/Utilize/__init__.py` & `qcompute-3.3.1/QCompute/Utilize/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.3.0/QCompute/__init__.py` & `qcompute-3.3.1/QCompute/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from QCompute.Module.UnrollCircuitToIonAPMModule import UnrollCircuitToIonAPMModule
 from QCompute.OpenModule.CompositeGateModule import CompositeGateModule
 from QCompute.OpenModule.CompressGateModule import CompressGateModule
 from QCompute.OpenModule.InverseCircuitModule import InverseCircuitModule
 from QCompute.OpenModule.ReverseCircuitModule import ReverseCircuitModule
 from QCompute.OpenModule.UnrollCircuitModule import UnrollCircuitModule
 from QCompute.OpenModule.UnrollProcedureModule import UnrollProcedureModule
+from QCompute.OpenModule.UnrollNoiseModule import UnrollNoiseModule
+from QCompute.OpenModule.CompressNoiseModule import CompressNoiseModule
 
 
 
 from QCompute.OpenSimulator import (
     QResult,
 )
 
@@ -84,14 +86,40 @@
     RY,
     RZ,
     CU,
     CRX,
     CRY,
     CRZ,
 )
+from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianGate import (
+    PhotonicDX as GaussianDX,
+    PhotonicDP as GaussianDP,
+    PhotonicPHA as GaussianPHA,
+    PhotonicBS as GaussianBS,
+    PhotonicCZ as GaussianCZ,
+    PhotonicCX as GaussianCX,
+    PhotonicDIS as GaussianDIS,
+    PhotonicSQU as GaussianSQU,
+    PhotonicTSQU as GaussianTSQU,
+    PhotonicMZ as GaussianMZ,  # CompositeGate
+)
+from QCompute.QPlatform.QOperation.Photonic.PhotonicGaussianMeasure import (
+    MeasureHomodyne as GaussianMeasureHomodyne,
+    MeasureHeterodyne as GaussianMeasureHeterodyne,
+    MeasurePhotonCount as GaussianMeasurePhotonCount,
+)
+from QCompute.QPlatform.QOperation.Photonic.PhotonicFockGate import (
+    PhotonicAP as FockAP,
+    PhotonicPHA as FockPHA,
+    PhotonicBS as FockBS,
+    PhotonicMZ as FockMZ,  # CompositeGate
+)
+from QCompute.QPlatform.QOperation.Photonic.PhotonicFockMeasure import (
+    MeasurePhotonCount as FockMeasurePhotonCount,
+)
 from QCompute.OpenConvertor.CircuitToDrawConsole import (
     CircuitToDrawConsole
 )
 from QCompute.OpenConvertor.CircuitToJson import (
     CircuitToJson
 )
 from QCompute.OpenConvertor.JsonToCircuit import (
@@ -121,17 +149,15 @@
 from QCompute.OpenConvertor.CircuitToXanaduSF import (
     CircuitToXanaduSF, TwoQubitsGate
 )
 from QCompute.QPlatform import QStatus
 from QCompute.QPlatform import Utilities
 from QCompute.Calibration import CalibrationUpdate, CalibrationReadData
 
-if True:  # prevent scrambling
-    
-    pass
+
 
 from QCompute.QPlatform.QNoise.AmplitudeDamping import AmplitudeDamping
 from QCompute.QPlatform.QNoise.BitFlip import BitFlip
 from QCompute.QPlatform.QNoise.BitPhaseFlip import BitPhaseFlip
 from QCompute.QPlatform.QNoise.CustomizedNoise import CustomizedNoise
 from QCompute.QPlatform.QNoise.Depolarizing import Depolarizing
 from QCompute.QPlatform.QNoise.PauliNoise import PauliNoise
```

### Comparing `qcompute-3.3.0/README.md` & `qcompute-3.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # QCompute
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2F%E9%87%8F%E6%98%93%E4%BC%8F%E5%9B%BE%E6%A0%87.png)
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.1-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -65,15 +65,15 @@
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
 ## Integrations
 
-The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+The new backend "local_cuquantum" is constructed with the NVIDIA cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk).
 
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
```

### Comparing `qcompute-3.3.0/qcompute.egg-info/PKG-INFO` & `qcompute-3.3.1/qcompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qcompute
-Version: 3.3.0
+Version: 3.3.1
 Summary: QCompute is a Python-based quantum software development kit (SDK). It provides a full-stack programming experience for advanced users via hybrid quantum programming language features and a high-performance simulator.
 Home-page: https://quantum.baidu.com
 Author: Baidu Quantum
 Author-email: quantum@baidu.com
 License: Apache License 2.0
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # QCompute
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2F%E9%87%8F%E6%98%93%E4%BC%8F%E5%9B%BE%E6%A0%87.png)
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.1-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -77,15 +77,15 @@
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
 ## Integrations
 
-The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+The new backend "local_cuquantum" is constructed with the NVIDIA cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk).
 
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
```

### Comparing `qcompute-3.3.0/qcompute.egg-info/SOURCES.txt` & `qcompute-3.3.1/qcompute.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -30,33 +30,53 @@
 QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py
 QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py
 QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py
 QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py
 QCompute/OpenModule/__init__.py
 QCompute/OpenModule/CompositeGateModule/__init__.py
 QCompute/OpenModule/CompressGateModule/__init__.py
+QCompute/OpenModule/CompressNoiseModule/__init__.py
 QCompute/OpenModule/InverseCircuitModule/__init__.py
 QCompute/OpenModule/ReverseCircuitModule/__init__.py
 QCompute/OpenModule/UnrollCircuitModule/__init__.py
 QCompute/OpenModule/UnrollNoiseModule/__init__.py
 QCompute/OpenModule/UnrollProcedureModule/__init__.py
 QCompute/OpenService/__init__.py
 QCompute/OpenService/service_ubqc/__init__.py
 QCompute/OpenService/service_ubqc/client/__init__.py
 QCompute/OpenService/service_ubqc/client/client.py
 QCompute/OpenService/service_ubqc/client/mcalculus.py
 QCompute/OpenService/service_ubqc/client/qobject.py
 QCompute/OpenService/service_ubqc/client/transpiler.py
 QCompute/OpenService/service_ubqc/client/utils.py
 QCompute/OpenSimulator/__init__.py
+QCompute/OpenSimulator/local_baidu_sim2/BaseSimulator.py
+QCompute/OpenSimulator/local_baidu_sim2/GeneralNoiseSimulator.py
 QCompute/OpenSimulator/local_baidu_sim2/InitState.py
+QCompute/OpenSimulator/local_baidu_sim2/LowNoiseCircuitSimulator.py
 QCompute/OpenSimulator/local_baidu_sim2/Measure.py
+QCompute/OpenSimulator/local_baidu_sim2/MixedUnitaryNoiseSimulator.py
+QCompute/OpenSimulator/local_baidu_sim2/NoNoiseSimulator.py
 QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
 QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
 QCompute/OpenSimulator/local_baidu_sim2/__init__.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/FockAddPhotons.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/FockAuxiliaryCalculation.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/FockCalculateInterferometer.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/FockCombination.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/FockPhotonCountMeasure.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/GaussAuxiliaryCalculation.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/GaussHeteroMea.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/GaussHomoMea.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/GaussPhotonCountMea.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/GaussTransfer.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/InitFockState.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/InitGaussState.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/Simulator.py
+QCompute/OpenSimulator/local_baidu_sim_photonic/__init__.py
 QCompute/OpenSimulator/local_cuquantum/CheckEnv.py
 QCompute/OpenSimulator/local_cuquantum/DistEinsum.py
 QCompute/OpenSimulator/local_cuquantum/Kernel.py
 QCompute/OpenSimulator/local_cuquantum/Simulator.py
 QCompute/OpenSimulator/local_cuquantum/__init__.py
 QCompute/QPlatform/BatchID.py
 QCompute/QPlatform/CircuitTools.py
@@ -96,14 +116,15 @@
 QCompute/QPlatform/QOperation/__init__.py
 QCompute/QProtobuf/__init__.py
 QCompute/QProtobuf/Library/Complex_pb2.py
 QCompute/QProtobuf/Library/PlatformStruct_pb2.py
 QCompute/QProtobuf/Library/QNoise_pb2.py
 QCompute/QProtobuf/Library/QObj_pb2.py
 QCompute/QProtobuf/Library/QOperation_pb2.py
+QCompute/QProtobuf/Library/QPhotonicOperation_pb2.py
 QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py
 QCompute/QProtobuf/Library/__init__.py
 QCompute/Utilize/__init__.py
 QCompute/Utilize/ControlledCircuit/__init__.py
 qcompute.egg-info/PKG-INFO
 qcompute.egg-info/SOURCES.txt
 qcompute.egg-info/dependency_links.txt
```

### Comparing `qcompute-3.3.0/setup.py` & `qcompute-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pathlib import Path
 
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
-SDK_VERSION = '3.3.0'
+SDK_VERSION = '3.3.1'
 
 DESC = Path('./README.md').read_text(encoding='utf-8')
 
 setup(
     name='qcompute',
     version=SDK_VERSION,
     install_requires=[
```

