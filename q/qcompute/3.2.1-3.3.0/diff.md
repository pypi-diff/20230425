# Comparing `tmp/qcompute-3.2.1.tar.gz` & `tmp/qcompute-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcompute-3.2.1.tar", last modified: Fri Dec 30 13:37:54 2022, max compression
+gzip compressed data, was "qcompute-3.3.0.tar", last modified: Sun Feb 19 07:46:48 2023, max compression
```

## Comparing `qcompute-3.2.1.tar` & `qcompute-3.3.0.tar`

### file list

```diff
@@ -1,156 +1,162 @@
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.677695 qcompute-3.2.1/
--rw-rw-rw-   0        0        0      601 2022-12-30 13:23:36.000000 qcompute-3.2.1/LICENSE
--rw-rw-rw-   0        0        0     4308 2022-12-30 13:37:54.676688 qcompute-3.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.545941 qcompute-3.2.1/QCompute/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.545941 qcompute-3.2.1/QCompute/Calibration/
--rw-rw-rw-   0        0        0     5343 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/Calibration/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.547954 qcompute-3.2.1/QCompute/Define/
--rw-rw-rw-   0        0        0     2854 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Define/Settings.py
--rw-rw-rw-   0        0        0     2811 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/Define/Utils.py
--rw-rw-rw-   0        0        0     3475 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Define/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.548957 qcompute-3.2.1/QCompute/Module/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.548957 qcompute-3.2.1/QCompute/Module/MappingToBaiduQPUQianModule/
--rw-rw-rw-   0        0        0     1682 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.550892 qcompute-3.2.1/QCompute/Module/MappingToIoPCASModule/
--rw-rw-rw-   0        0        0     1658 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/MappingToIoPCASModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.551906 qcompute-3.2.1/QCompute/Module/MappingToIonAPMModule/
--rw-rw-rw-   0        0        0     1635 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/MappingToIonAPMModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.553129 qcompute-3.2.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/
--rw-rw-rw-   0        0        0     2495 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.554139 qcompute-3.2.1/QCompute/Module/UnrollCircuitToIoPCASModule/
--rw-rw-rw-   0        0        0     2453 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.555148 qcompute-3.2.1/QCompute/Module/UnrollCircuitToIonAPMModule/
--rw-rw-rw-   0        0        0     2388 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py
--rw-rw-rw-   0        0        0      713 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/Module/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.555148 qcompute-3.2.1/QCompute/OpenConvertor/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.556210 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToDrawConsole/
--rw-rw-rw-   0        0        0     9351 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.557216 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToInternalStruct/
--rw-rw-rw-   0        0        0     3423 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.558287 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToIonQ/
--rw-rw-rw-   0        0        0     5194 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToIonQ/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.559380 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToJson/
--rw-rw-rw-   0        0        0     1316 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToJson/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.559380 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQasm/
--rw-rw-rw-   0        0        0    17720 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQasm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.560937 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQobj/
--rw-rw-rw-   0        0        0     6611 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQobj/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.561939 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToXanaduSF/
--rw-rw-rw-   0        0        0    16242 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.562941 qcompute-3.2.1/QCompute/OpenConvertor/InternalStructToCircuit/
--rw-rw-rw-   0        0        0     2061 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.563949 qcompute-3.2.1/QCompute/OpenConvertor/IonQToCircuit/
--rw-rw-rw-   0        0        0     7379 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/IonQToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.563949 qcompute-3.2.1/QCompute/OpenConvertor/JsonToCircuit/
--rw-rw-rw-   0        0        0     1211 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/JsonToCircuit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.565012 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.568069 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/
--rw-rw-rw-   0        0        0      692 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.573139 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/
--rw-rw-rw-   0        0        0     9067 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py
--rw-rw-rw-   0        0        0     7554 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py
--rw-rw-rw-   0        0        0    80812 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py
--rw-rw-rw-   0        0        0     4755 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py
--rw-rw-rw-   0        0        0      692 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py
--rw-rw-rw-   0        0        0    51730 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/__init__.py
--rw-rw-rw-   0        0        0      842 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenConvertor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.574504 qcompute-3.2.1/QCompute/OpenModule/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.575546 qcompute-3.2.1/QCompute/OpenModule/CompositeGateModule/
--rw-rw-rw-   0        0        0     5967 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/CompositeGateModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.576755 qcompute-3.2.1/QCompute/OpenModule/CompressGateModule/
--rw-rw-rw-   0        0        0     8690 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/CompressGateModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.576755 qcompute-3.2.1/QCompute/OpenModule/InverseCircuitModule/
--rw-rw-rw-   0        0        0     5061 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/InverseCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.577886 qcompute-3.2.1/QCompute/OpenModule/ReverseCircuitModule/
--rw-rw-rw-   0        0        0     2398 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/ReverseCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.579343 qcompute-3.2.1/QCompute/OpenModule/UnrollCircuitModule/
--rw-rw-rw-   0        0        0    19682 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/UnrollCircuitModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.579343 qcompute-3.2.1/QCompute/OpenModule/UnrollNoiseModule/
--rw-rw-rw-   0        0        0     3780 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/UnrollNoiseModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.580850 qcompute-3.2.1/QCompute/OpenModule/UnrollProcedureModule/
--rw-rw-rw-   0        0        0     4787 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/UnrollProcedureModule/__init__.py
--rw-rw-rw-   0        0        0      950 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenModule/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.580850 qcompute-3.2.1/QCompute/OpenService/
--rw-rw-rw-   0        0        0      713 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.582920 qcompute-3.2.1/QCompute/OpenService/service_ubqc/
--rw-rw-rw-   0        0        0     2093 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.591812 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/
--rw-rw-rw-   0        0        0      692 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/__init__.py
--rw-rw-rw-   0        0        0    40536 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/client.py
--rw-rw-rw-   0        0        0    34117 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/mcalculus.py
--rw-rw-rw-   0        0        0    62675 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/qobject.py
--rw-rw-rw-   0        0        0     2334 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/transpiler.py
--rw-rw-rw-   0        0        0    20703 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.592917 qcompute-3.2.1/QCompute/OpenSimulator/
--rw-rw-rw-   0        0        0     7273 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/OpenSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.599507 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/
--rw-rw-rw-   0        0        0     1539 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/InitState.py
--rw-rw-rw-   0        0        0     7804 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Measure.py
--rw-rw-rw-   0        0        0    59389 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
--rw-rw-rw-   0        0        0     5503 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
--rw-rw-rw-   0        0        0     6316 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.613674 qcompute-3.2.1/QCompute/QPlatform/
--rw-rw-rw-   0        0        0      747 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/BatchID.py
--rw-rw-rw-   0        0        0     9313 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/CircuitTools.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.614676 qcompute-3.2.1/QCompute/QPlatform/Condition/
--rw-rw-rw-   0        0        0     1147 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Condition/__init__.py
--rw-rw-rw-   0        0        0     1584 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Error.py
--rw-rw-rw-   0        0        0    10682 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QPlatform/InteractiveModule.py
--rw-rw-rw-   0        0        0     2001 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/ProcedureParameterPool.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.619232 qcompute-3.2.1/QCompute/QPlatform/Processor/
--rw-rw-rw-   0        0        0     7212 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QPlatform/Processor/ModuleFilter.py
--rw-rw-rw-   0        0        0     3875 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Processor/PostProcessor.py
--rw-rw-rw-   0        0        0     2978 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Processor/PreProcess.py
--rw-rw-rw-   0        0        0      693 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Processor/__init__.py
--rw-rw-rw-   0        0        0    24577 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QPlatform/QEnv.py
--rw-rw-rw-   0        0        0     7560 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QEnvOperation.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.629217 qcompute-3.2.1/QCompute/QPlatform/QNoise/
--rw-rw-rw-   0        0        0     5884 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/AmplitudeDamping.py
--rw-rw-rw-   0        0        0     2416 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/BitFlip.py
--rw-rw-rw-   0        0        0     2421 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/BitPhaseFlip.py
--rw-rw-rw-   0        0        0     5638 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/CustomizedNoise.py
--rw-rw-rw-   0        0        0     2715 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/Depolarizing.py
--rw-rw-rw-   0        0        0     2889 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/PauliNoise.py
--rw-rw-rw-   0        0        0     2679 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/PhaseDamping.py
--rw-rw-rw-   0        0        0     2417 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/PhaseFlip.py
--rw-rw-rw-   0        0        0     4546 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/ResetNoise.py
--rw-rw-rw-   0        0        0     5958 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/Utilities.py
--rw-rw-rw-   0        0        0     3243 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QNoise/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.637231 qcompute-3.2.1/QCompute/QPlatform/QOperation/
--rw-rw-rw-   0        0        0     1236 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/Barrier.py
--rw-rw-rw-   0        0        0     6787 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/CompositeGate.py
--rw-rw-rw-   0        0        0     1666 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/CustomizedGate.py
--rw-rw-rw-   0        0        0    11825 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/FixedGate.py
--rw-rw-rw-   0        0        0     1968 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/Measure.py
--rw-rw-rw-   0        0        0     3021 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/QProcedure.py
--rw-rw-rw-   0        0        0    11660 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/RotationGate.py
--rw-rw-rw-   0        0        0     8167 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QOperation/__init__.py
--rw-rw-rw-   0        0        0     3569 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QRegPool.py
--rw-rw-rw-   0        0        0     2524 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/QStatus.py
--rw-rw-rw-   0        0        0    16091 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QPlatform/QTask.py
--rw-rw-rw-   0        0        0     6718 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QPlatform/Utilities.py
--rw-rw-rw-   0        0        0     7356 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.639230 qcompute-3.2.1/QCompute/QProtobuf/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.646237 qcompute-3.2.1/QCompute/QProtobuf/Library/
--rw-rw-rw-   0        0        0     1164 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/Complex_pb2.py
--rw-rw-rw-   0        0        0     3423 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/PlatformStruct_pb2.py
--rw-rw-rw-   0        0        0     3422 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/QNoise_pb2.py
--rw-rw-rw-   0        0        0     1691 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/QObj_pb2.py
--rw-rw-rw-   0        0        0     2412 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/QOperation_pb2.py
--rw-rw-rw-   0        0        0     1488 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py
--rw-rw-rw-   0        0        0      692 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/QProtobuf/Library/__init__.py
--rw-rw-rw-   0        0        0     1595 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/QProtobuf/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.647703 qcompute-3.2.1/QCompute/Utilize/
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.648702 qcompute-3.2.1/QCompute/Utilize/ControlledCircuit/
--rw-rw-rw-   0        0        0    16522 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/Utilize/ControlledCircuit/__init__.py
--rw-rw-rw-   0        0        0      714 2022-12-30 13:23:36.000000 qcompute-3.2.1/QCompute/Utilize/__init__.py
--rw-rw-rw-   0        0        0     4395 2022-12-30 13:32:28.000000 qcompute-3.2.1/QCompute/__init__.py
--rw-rw-rw-   0        0        0     3730 2022-12-30 13:23:36.000000 qcompute-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-30 13:37:54.673188 qcompute-3.2.1/qcompute.egg-info/
--rw-rw-rw-   0        0        0     4308 2022-12-30 13:37:54.000000 qcompute-3.2.1/qcompute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4598 2022-12-30 13:37:54.000000 qcompute-3.2.1/qcompute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-30 13:37:54.000000 qcompute-3.2.1/qcompute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2022-12-30 13:37:54.000000 qcompute-3.2.1/qcompute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-30 13:37:54.000000 qcompute-3.2.1/qcompute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-30 13:37:54.677695 qcompute-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2141 2022-12-30 13:32:28.000000 qcompute-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.493297 qcompute-3.3.0/
+-rw-rw-rw-   0        0        0      601 2023-02-19 07:44:27.000000 qcompute-3.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4473 2023-02-19 07:46:48.492297 qcompute-3.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.288503 qcompute-3.3.0/QCompute/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.290504 qcompute-3.3.0/QCompute/Calibration/
+-rw-rw-rw-   0        0        0     5343 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Calibration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.294504 qcompute-3.3.0/QCompute/Define/
+-rw-rw-rw-   0        0        0     2881 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Define/Settings.py
+-rw-rw-rw-   0        0        0     2811 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Define/Utils.py
+-rw-rw-rw-   0        0        0     3475 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Define/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.296507 qcompute-3.3.0/QCompute/Module/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.297508 qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/
+-rw-rw-rw-   0        0        0     1686 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.299510 qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/
+-rw-rw-rw-   0        0        0     1662 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.301509 qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/
+-rw-rw-rw-   0        0        0     1635 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.303509 qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/
+-rw-rw-rw-   0        0        0     2499 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.305510 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/
+-rw-rw-rw-   0        0        0     2455 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.307510 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/
+-rw-rw-rw-   0        0        0     2392 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/Module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.308510 qcompute-3.3.0/QCompute/OpenConvertor/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.310015 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/
+-rw-rw-rw-   0        0        0     9315 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.312019 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/
+-rw-rw-rw-   0        0        0     3423 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.314019 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/
+-rw-rw-rw-   0        0        0     5194 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.316020 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/
+-rw-rw-rw-   0        0        0     1316 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.318020 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/
+-rw-rw-rw-   0        0        0    17698 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.320021 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/
+-rw-rw-rw-   0        0        0     6611 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.321021 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/
+-rw-rw-rw-   0        0        0    16194 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.323021 qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/
+-rw-rw-rw-   0        0        0     2061 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.324022 qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/
+-rw-rw-rw-   0        0        0     7379 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.326022 qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/
+-rw-rw-rw-   0        0        0     1211 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.328022 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.330022 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/
+-rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.339024 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/
+-rw-rw-rw-   0        0        0     9067 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py
+-rw-rw-rw-   0        0        0     7554 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py
+-rw-rw-rw-   0        0        0    80812 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py
+-rw-rw-rw-   0        0        0     4755 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py
+-rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py
+-rw-rw-rw-   0        0        0    51411 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenConvertor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.341025 qcompute-3.3.0/QCompute/OpenModule/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.342026 qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/
+-rw-rw-rw-   0        0        0     5967 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.344026 qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/
+-rw-rw-rw-   0        0        0     8690 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.346027 qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/
+-rw-rw-rw-   0        0        0     5061 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.347027 qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/
+-rw-rw-rw-   0        0        0     2398 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.349027 qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/
+-rw-rw-rw-   0        0        0    19632 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.351028 qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/
+-rw-rw-rw-   0        0        0     3756 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.353028 qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/
+-rw-rw-rw-   0        0        0     4762 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/__init__.py
+-rw-rw-rw-   0        0        0      950 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenModule/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.354028 qcompute-3.3.0/QCompute/OpenService/
+-rw-rw-rw-   0        0        0      713 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.356029 qcompute-3.3.0/QCompute/OpenService/service_ubqc/
+-rw-rw-rw-   0        0        0     2093 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.366031 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/
+-rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/__init__.py
+-rw-rw-rw-   0        0        0    40419 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/client.py
+-rw-rw-rw-   0        0        0    34117 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/mcalculus.py
+-rw-rw-rw-   0        0        0    62675 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/qobject.py
+-rw-rw-rw-   0        0        0     2334 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/transpiler.py
+-rw-rw-rw-   0        0        0    20703 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/utils.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.368031 qcompute-3.3.0/QCompute/OpenSimulator/
+-rw-rw-rw-   0        0        0     7160 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.377034 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/
+-rw-rw-rw-   0        0        0     1499 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/InitState.py
+-rw-rw-rw-   0        0        0     7788 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Measure.py
+-rw-rw-rw-   0        0        0    59134 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
+-rw-rw-rw-   0        0        0     5511 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
+-rw-rw-rw-   0        0        0     6316 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.385038 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/
+-rw-rw-rw-   0        0        0     1838 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/CheckEnv.py
+-rw-rw-rw-   0        0        0     3622 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/DistEinsum.py
+-rw-rw-rw-   0        0        0     6575 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Kernel.py
+-rw-rw-rw-   0        0        0     9045 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/Simulator.py
+-rw-rw-rw-   0        0        0     8271 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/OpenSimulator/local_cuquantum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.404042 qcompute-3.3.0/QCompute/QPlatform/
+-rw-rw-rw-   0        0        0      747 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/BatchID.py
+-rw-rw-rw-   0        0        0     9313 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/CircuitTools.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.406043 qcompute-3.3.0/QCompute/QPlatform/Condition/
+-rw-rw-rw-   0        0        0     1147 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Condition/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Error.py
+-rw-rw-rw-   0        0        0    10657 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/InteractiveModule.py
+-rw-rw-rw-   0        0        0     2001 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/ProcedureParameterPool.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.412553 qcompute-3.3.0/QCompute/QPlatform/Processor/
+-rw-rw-rw-   0        0        0     7195 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/ModuleFilter.py
+-rw-rw-rw-   0        0        0     3875 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/PostProcessor.py
+-rw-rw-rw-   0        0        0     2978 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/PreProcess.py
+-rw-rw-rw-   0        0        0      693 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Processor/__init__.py
+-rw-rw-rw-   0        0        0    26808 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/QEnv.py
+-rw-rw-rw-   0        0        0     7560 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QEnvOperation.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.430557 qcompute-3.3.0/QCompute/QPlatform/QNoise/
+-rw-rw-rw-   0        0        0     5870 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/AmplitudeDamping.py
+-rw-rw-rw-   0        0        0     2416 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/BitFlip.py
+-rw-rw-rw-   0        0        0     2421 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/BitPhaseFlip.py
+-rw-rw-rw-   0        0        0     5632 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/CustomizedNoise.py
+-rw-rw-rw-   0        0        0     2704 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/Depolarizing.py
+-rw-rw-rw-   0        0        0     2889 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PauliNoise.py
+-rw-rw-rw-   0        0        0     2666 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseDamping.py
+-rw-rw-rw-   0        0        0     2415 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseFlip.py
+-rw-rw-rw-   0        0        0     4516 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/ResetNoise.py
+-rw-rw-rw-   0        0        0     5958 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/Utilities.py
+-rw-rw-rw-   0        0        0     3243 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QNoise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.444560 qcompute-3.3.0/QCompute/QPlatform/QOperation/
+-rw-rw-rw-   0        0        0     1236 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/Barrier.py
+-rw-rw-rw-   0        0        0     6724 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/CompositeGate.py
+-rw-rw-rw-   0        0        0     1666 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/CustomizedGate.py
+-rw-rw-rw-   0        0        0    11825 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/FixedGate.py
+-rw-rw-rw-   0        0        0     1968 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/Measure.py
+-rw-rw-rw-   0        0        0     3021 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/QProcedure.py
+-rw-rw-rw-   0        0        0    11615 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/RotationGate.py
+-rw-rw-rw-   0        0        0     8156 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QOperation/__init__.py
+-rw-rw-rw-   0        0        0     3569 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QRegPool.py
+-rw-rw-rw-   0        0        0     2524 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/QStatus.py
+-rw-rw-rw-   0        0        0    16075 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/QTask.py
+-rw-rw-rw-   0        0        0     6731 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QPlatform/Utilities.py
+-rw-rw-rw-   0        0        0     7607 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.446561 qcompute-3.3.0/QCompute/QProtobuf/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.458286 qcompute-3.3.0/QCompute/QProtobuf/Library/
+-rw-rw-rw-   0        0        0     1164 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/Complex_pb2.py
+-rw-rw-rw-   0        0        0     3423 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/PlatformStruct_pb2.py
+-rw-rw-rw-   0        0        0     3422 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QNoise_pb2.py
+-rw-rw-rw-   0        0        0     1691 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QObj_pb2.py
+-rw-rw-rw-   0        0        0     2412 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/QOperation_pb2.py
+-rw-rw-rw-   0        0        0     1488 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py
+-rw-rw-rw-   0        0        0      692 2023-02-19 07:44:27.000000 qcompute-3.3.0/QCompute/QProtobuf/Library/__init__.py
+-rw-rw-rw-   0        0        0     1595 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/QProtobuf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.460290 qcompute-3.3.0/QCompute/Utilize/
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.462290 qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/
+-rw-rw-rw-   0        0        0    17017 2023-02-19 07:44:28.000000 qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-02-19 07:44:28.000000 qcompute-3.3.0/QCompute/Utilize/__init__.py
+-rw-rw-rw-   0        0        0     4451 2023-02-19 07:45:34.000000 qcompute-3.3.0/QCompute/__init__.py
+-rw-rw-rw-   0        0        0     3891 2023-02-19 07:44:28.000000 qcompute-3.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-02-19 07:46:48.491297 qcompute-3.3.0/qcompute.egg-info/
+-rw-rw-rw-   0        0        0     4473 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4854 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-02-19 07:46:48.000000 qcompute-3.3.0/qcompute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-19 07:46:48.494298 qcompute-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2141 2023-02-19 07:45:34.000000 qcompute-3.3.0/setup.py
```

### Comparing `qcompute-3.2.1/LICENSE` & `qcompute-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/PKG-INFO` & `qcompute-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qcompute
-Version: 3.2.1
+Version: 3.3.0
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
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.2.1-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -75,14 +75,18 @@
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2Fqrcode.png)
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
+## Integrations
+
+The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/baidu/QCompute/blob/master/LICENSE) file for details.
```

### Comparing `qcompute-3.2.1/QCompute/Calibration/__init__.py` & `qcompute-3.3.0/QCompute/Calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/Define/Settings.py` & `qcompute-3.3.0/QCompute/Define/Settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,27 +66,29 @@
 inProcessSimulator = True
 """
 Run simulator in or out process.
 
 The 'inProcessSimulator' option can significantly accelerate the calculation of simulator while 
 the outProcessSimulator can enhance the stability of simulator.  
 
-Supporting local_baidu_sim2
-
+Supporting local_baidu_sim2, local_cuquantum
 
 Values: True, False
 """
 
 
 @unique
 class NoiseMethod(IntEnum):
     """
     # different methods
+
     # mixed unitary noise
+
     # general noise
+    
     # low noise circuit, speed up
     """
     MixedUnitaryNoise = 0
     GeneralNoise = MixedUnitaryNoise + 1
     LowNoiseCircuit = GeneralNoise + 1
 
 noiseMethod = NoiseMethod.LowNoiseCircuit
@@ -101,14 +103,15 @@
 noiseMultiprocessingSimulator = True
 """
 Run noise simulator in multiprocessing.
 
 Values: True, False
 
 For default noiseMethod, turn on noiseMultiprocessingSimulator
+
     for case 1) if circuit depth :math:`\geq 30` and qubits  :math:`\leq 10`;
 
     or case 2) if qubits > 10.
 """
 
 autoClearOutputDirAfterFetchMeasure = False
 """
```

### Comparing `qcompute-3.2.1/QCompute/Define/Utils.py` & `qcompute-3.3.0/QCompute/Define/Utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,23 +82,23 @@
     if moduleSpec is None:
         return None
     module = importlib.util.module_from_spec(moduleSpec)
     moduleSpec.loader.exec_module(module)
     return module
 
 
-def matchSdkVersion(tagretVersion: str):
+def matchSdkVersion(targetVersion: str):
     """
     Match sdk version.
     """
-    if QCompute.Define.sdkVersion != tagretVersion:
+    if QCompute.Define.sdkVersion != targetVersion:
         import warnings
 
         warnings.warn(
-            f'This example({tagretVersion}) '
+            f'This example({targetVersion}) '
             f'does not match the correct sdk version({QCompute.Define.sdkVersion}). '
             'Please update the sdk.',
             FutureWarning)
 
 
 def clearOutputDir():
     """
```

### Comparing `qcompute-3.2.1/QCompute/Define/__init__.py` & `qcompute-3.3.0/QCompute/Define/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # service address for production
     quantumHubAddr = 'https://quantum-hub.baidu.com/api'
     quantumBucket = 'quantum-task'
     blindCompAddr = 'wss://blindcomp.baidu.com'
 else:
     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
 
-sdkVersion = 'Python 3.2.1'
+sdkVersion = 'Python 3.3.0'
 """
 SDK Version
 
 Do not modify by user.
 
 Used for task submission.
 """
```

### Comparing `qcompute-3.2.1/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/MappingToBaiduQPUQianModule/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Mapping To BaiduQPUQian
 """
-from QCompute.OpenModule import ModuleImplement
 from typing import Dict, List, Optional
+
+from QCompute.OpenModule import ModuleImplement
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBMeasure
 
 
+
 FileErrorCode = 8
 
 
 class MappingToBaiduQPUQianModule(ModuleImplement):
     """
     Mapping Procedure
```

### Comparing `qcompute-3.2.1/QCompute/Module/MappingToIoPCASModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/MappingToIoPCASModule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Mapping To IOPCAS
 """
-from QCompute.OpenModule import ModuleImplement
 from typing import Dict, List, Optional
+
+from QCompute.OpenModule import ModuleImplement
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBMeasure
 
 
+
 FileErrorCode = 2
 
 
 class MappingToIoPCASModule(ModuleImplement):
     """
     Mapping Procedure
```

### Comparing `qcompute-3.2.1/QCompute/Module/MappingToIonAPMModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/MappingToIonAPMModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/UnrollCircuitToBaiduQPUQianModule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Unroll Circuit To BaiduQPUQian
 """
-from QCompute.OpenModule import ModuleImplement
 from typing import List, Dict, Optional, Union
+
+from QCompute.OpenModule import ModuleImplement
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate
 
 
+
 FileErrorCode = 7
 
 
 class UnrollCircuitToBaiduQPUQianModule(ModuleImplement):
     """
     Unroll supported gates to Ry, Rz, barrier, measure
```

### Comparing `qcompute-3.2.1/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/UnrollCircuitToIoPCASModule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Unroll Circuit To IOPCAS
 """
 from QCompute.OpenModule import ModuleImplement
 from typing import List, Dict, Optional, Union
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate
 
 
+
 FileErrorCode = 1
 
 
 class UnrollCircuitToIoPCASModule(ModuleImplement):
     """
     Unroll supported gates to Ry, Rz, barrier, measure
```

### Comparing `qcompute-3.2.1/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py` & `qcompute-3.3.0/QCompute/Module/UnrollCircuitToIonAPMModule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Unroll Circuit To IonAPM
 """
-from QCompute.OpenModule import ModuleImplement
 from typing import List, Dict, Optional, Union
+
+from QCompute.OpenModule import ModuleImplement
 from QCompute.QProtobuf import PBProgram, PBCircuitLine, PBFixedGate, PBRotationGate
 
 
+
 FileErrorCode = 11
 
 
 class UnrollCircuitToIonAPMModule(ModuleImplement):
     """
     Unroll supported gates to X, Y, RX, RY, barrier, measure
```

### Comparing `qcompute-3.2.1/QCompute/Module/__init__.py` & `qcompute-3.3.0/QCompute/Module/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToDrawConsole/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class CircuitToDrawConsole(ConvertorImplement):
     """
     Circuit to draw console
     """
 
     def __init__(self):
-        self.stringIO = None  # typing: StringIO
+        self.stringIO: StringIO = None
 
     def convert(self, pbProgram: PBProgram) -> str:
         """
         Convert the circuit to drawing in terminal.
 
         Example:
 
@@ -71,15 +71,15 @@
         for pbCircuitLine in pbCircuitLineList:
             qRegSet.update(pbCircuitLine.qRegList)
         qRegCount = max(qRegSet) + 1
 
         if qRegCount <= 0:
             return 'Enpty circuit.'
 
-        circuitArray = []  # typing: List[List[str]]
+        circuitArray: List[List[str]] = []
 
         maxQRegNameLen = len(str(qRegCount - 1)) + 1
         for i in range(qRegCount):
             qRegName = f'Q{i}'
             if len(qRegName) < maxQRegNameLen:
                 qRegName += ' ' * (maxQRegNameLen - len(qRegName))
             circuitArray.append([f'Q{i}'])
@@ -120,15 +120,15 @@
                         else:
                             argumentList.append(f'P{argumentId}')
                 else:
                     for argument in pbCircuitLine.argumentValueList:
                         argumentList.append(f'{argument}')
                 self._draw(qRegCount, f'|{gateName}|', pbCircuitLine.qRegList, circuitArray)
             elif op == 'customizedGate':
-                customizedGate = pbCircuitLine.customizedGate  # type: PBCustomizedGate
+                customizedGate: PBCustomizedGate = pbCircuitLine.customizedGate
                 matrixBytes = protobufMatrixToNumpyMatrix(customizedGate.matrix).tobytes()
                 hash = blake2b(matrixBytes, digest_size=Settings.drawCircuitCustomizedGateHashLength)
                 gateName = f'Custom[{hash.hexdigest()}]'
                 gateName = self._appendNoise(gateName, pbCircuitLine)
                 self._draw(qRegCount, f'|{gateName}]|', pbCircuitLine.qRegList, circuitArray)
             elif op == 'procedureName':
                 gateName = pbCircuitLine.procedureName
@@ -141,15 +141,15 @@
                             argumentList.append(f'P{argumentId}')
                 else:
                     for argument in pbCircuitLine.argumentValueList:
                         argumentList.append(f'{argument}')
                 self._draw(qRegCount, f'|{gateName}|', pbCircuitLine.qRegList, circuitArray)
             elif op == 'measure':
                 for qReg in pbCircuitLine.qRegList:
-                    measure = pbCircuitLine.measure  # type: PBMeasure
+                    measure: PBMeasure = pbCircuitLine.measure
                     typeName = PBMeasure.Type.Name(measure.type)
                     self._draw(qRegCount, f'|M[{typeName.lower()}]|', [qReg], circuitArray)
             elif op == 'barrier':
                 for qReg in pbCircuitLine.qRegList:
                     self._draw(qRegCount, '|', [qReg], circuitArray)
             else:
                 raise Error.ArgumentError(f'DrawConsole Unsupported operation {op}!', ModuleErrorCode, FileErrorCode, 1)
```

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToInternalStruct/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToIonQ/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToIonQ/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToJson/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToJson/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQasm/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQasm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,28 +294,27 @@
         return command
 
     def getCircuitsCode(self, circuit: List, regName: str, usingIndex: bool = True) -> Tuple[str, Set[str]]:
         """
         Convert Circuits to qasm code. 
 
         :param circuit: type: List. List of gate operations.
-        :param regName: type: str. Name of register. The name of register \
-            used in the procedure is different from that in external program.
+        :param regName: type: str. Name of register. The name of register used in the procedure is different from that in external program.
         :param usingIndex: type: bool. If True, adds braket [] for register index. Default: True.
 
         :return qasmCode: type: str. Qasm code of circuit.
         :return depends: type: str. Dependencies of called procedures.
         """
 
         # Process circuits recurrently.
         qasmCode = ''
         # If op == 'measure', adds measure code to the end of command code. 
         measureCode = ''
         # Dependency of procedures.
-        depends = set()  # type: Set[str]
+        depends: Set[str] = set()
         for gate in circuit:
             # Type of gate operation.
             op = gate.WhichOneof('op')
             if op == 'fixedGate':
                 qasmCode += self.getFixedCommandCode(gate.fixedGate, gate.qRegList, regName, usingIndex)
             elif op == 'rotationGate':
                 qasmCode += self.getRotationCommandCode(gate.rotationGate, gate.qRegList, regName, usingIndex,
```

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToQobj/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToQobj/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/CircuitToXanaduSF/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,31 +172,31 @@
     kerrRotationGateMapping(TwoQubitsGate.quarter, pbRotationGate, argumentValueList, qRegList, qRegMap, ret)
 
 
 twoQubitsSet = set()
 
 
 def thirdConvert(pbProgram: 'PBProgram', ret: StringIO):
-    qRegMap = {}  # type: Dict[int, int]
+    qRegMap: Dict[int, int] = {}
     for qReg in pbProgram.head.usingQRegList:
         sfQReg = len(qRegMap)
         qRegMap[qReg] = sfQReg
         ret.write(f'Fock(1) | {sfQReg * 2}\n')
         ret.write(f'Fock(0) | {sfQReg * 2 + 1}\n')
     global ancillaQRegIndex
     ancillaQRegIndex = len(qRegMap)
     twoQubitsSet.clear()
 
     for pbCircuitLine in pbProgram.body.circuit:
         op = pbCircuitLine.WhichOneof('op')
         if op == 'fixedGate':
-            fixedGate = pbCircuitLine.fixedGate  # type: PBFixedGate
+            fixedGate: PBFixedGate = pbCircuitLine.fixedGate
             thirdFixedGateMapping(fixedGate, pbCircuitLine.qRegList, qRegMap, ret)
         elif op == 'rotationGate':
-            rotationGate = pbCircuitLine.rotationGate  # type: PBRotationGate
+            rotationGate: PBRotationGate = pbCircuitLine.rotationGate
             thirdRotationGateMapping(rotationGate, pbCircuitLine.argumentValueList, pbCircuitLine.qRegList, qRegMap,
                                      ret)
         elif op == 'measure':
             continue
         else:
             raise Error.ArgumentError(f'Unsupported operation {op} at XanaduSF third!', ModuleErrorCode, FileErrorCode,
                                       2)
@@ -257,28 +257,28 @@
 
 def thirdRotationGateMapping(pbRotationGate: PBRotationGate, argumentValueList: List[float], qRegList: List[int],
                              qRegMap: Dict[int, int], ret: StringIO):
     kerrRotationGateMapping(TwoQubitsGate.third, pbRotationGate, argumentValueList, qRegList, qRegMap, ret)
 
 
 def kerrConvert(pbProgram: 'PBProgram', ret: StringIO):
-    qRegMap = {}  # type: Dict[int, int]
+    qRegMap: Dict[int, int] = {}
     for qReg in pbProgram.head.usingQRegList:
         sfQReg = len(qRegMap)
         qRegMap[qReg] = sfQReg
         ret.write(f'Fock(1) | {sfQReg * 2}\n')
         ret.write(f'Fock(0) | {sfQReg * 2 + 1}\n')
 
     for pbCircuitLine in pbProgram.body.circuit:
         op = pbCircuitLine.WhichOneof('op')
         if op == 'fixedGate':
-            fixedGate = pbCircuitLine.fixedGate  # type: PBFixedGate
+            fixedGate: PBFixedGate = pbCircuitLine.fixedGate
             kerrFixedGateMapping(TwoQubitsGate.kerr, fixedGate, pbCircuitLine.qRegList, qRegMap, ret)
         elif op == 'rotationGate':
-            rotationGate = pbCircuitLine.rotationGate  # type: PBRotationGate
+            rotationGate: PBRotationGate = pbCircuitLine.rotationGate
             kerrRotationGateMapping(TwoQubitsGate.kerr, rotationGate, pbCircuitLine.argumentValueList,
                                     pbCircuitLine.qRegList, qRegMap, ret)
         elif op == 'measure':
             continue
         else:
             raise Error.ArgumentError(f'Unsupported operation {op} at XanaduSF kerr!', ModuleErrorCode, FileErrorCode,
                                       5)
```

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/InternalStructToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/IonQToCircuit/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/IonQToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/JsonToCircuit/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/JsonToCircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMLexer.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMListener.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMParser.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/QASMVisitor.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/BNF_Antlr4/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/QasmToCircuit/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/QasmToCircuit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         Convert arguments to float.
 
         :param arguments: type: str. Arguments.
 
         :return: type: List[float]. List of arguments (floating point data type).
         """
         argumentList = arguments.split(',')
-        return [float(argument) for argument in argumentList]  # type: List[float]
+        return [float(argument) for argument in argumentList]
 
     
     def prepareArguments(self, arguments: str) -> List[str]:
         argumentList = arguments.split(',')
         return argumentList
 
     
@@ -177,15 +177,15 @@
         The argumentExprList, argumentIdList and argumentValueList in the current scope are cleaned at last.
 
         :param ctx: type: object. QASMParser.UopContext.
 
         :return: type: Tuple[str, List[int]]. Converted arguments and list of argument ids.
         """
         arguments = ''
-        argumentIdList = []  # type: List[int]
+        argumentIdList: List[int] = []
         
         explist = ctx.explist()
         if explist:
             arguments = self.visitExplist(explist)
             scopeData = self.getScopeData()
             argumentIdList = scopeData.argumentIdList
             self.cleanArgumentExprList()
@@ -201,15 +201,15 @@
         :param procArguments: type: str. Procedure arguments.
         :param pendingArgumentList: type: List[str]. List of pending arguments.
         :param argumentMap: type: object. Argument map of procedure.
         
         :return realArgumentList: type: List[float]. List of real values of arguments.
         """
         argumentArray = procArguments.split(',')
-        realArgumentList = []  # type: List[float]
+        realArgumentList: List[float] = []
         if pendingArgumentList:
             for argument in pendingArgumentList:
                 realVal = argument
                 try:
                     reVal = float(realVal)
                     realArgumentList.append(reVal)
                     continue
@@ -409,15 +409,15 @@
         
         :param idArgumentList: type: List. List of argument ids.
         :param line: type: int. Row.
         :param position: type: int. Column.
 
         :return: type: bool. True. If the same register is used, throws exception.
         """
-        checkIds = []  # type: List[str]
+        checkIds: List[str] = []
         for id in idArgumentList:
             rId = id.getText()
             # Check if quantum register is defined.
             self.checkQregVar(rId, line, position)
             if rId in checkIds:
                 raise Error.ArgumentError(f'Illegal operation on same register. line: {line}, position: {position}.',
                                           ModuleErrorCode, FileErrorCode, 12)
@@ -481,15 +481,15 @@
         :param argumentCount: type: int. The count of argument(s).
         :param line: type: int. Row.
         :param position: type: int. Column.
 
         :return: bool. True. If the count of arguments is different from operation, throws exception.
         """
         checkOp = opId.upper()
-        error = False  # type: bool
+        error = False
         if checkOp in self.oneArgumentOp:
             if argumentCount != 1:
                 error = True
         elif checkOp in self.twoArgumentsOp and argumentCount != 2:
             if argumentCount != 2:
                 error = True
         elif checkOp in self.threeArgumentsOp and argumentCount != 3:
@@ -563,15 +563,15 @@
         """
         if self.containMeasure:
             raise Error.ArgumentError(
                 f'Illegal operation in code. The measurement instruction must be the last instruction. line: {line}, position: {position}.',
                 ModuleErrorCode, FileErrorCode, 18)
 
     def genSequenceArray(self, size: int):
-        return [i for i in range(size)]  # type: List[int]
+        return [i for i in range(size)]
 
 
     def getProcCircuitList(self, procName: str, procArguments: str, regIdList: List[int]):
         """
         Recursively get circuits of procedures. 
         # NOTE: Use shallowCopy to get values of objects. Objects can not be modified. 
         Each pending argument is calculated by the currently used arguments.
@@ -587,24 +587,24 @@
 
         :param procName: type: str. The name of procedure. 
         :param procArguments: type: str. The arguments of procedure.
         :param regIdList: type: List[int]. List of register ids. 
         
         :return: List[CircuitLine]. The circuits of procedures.
         """
-        circuitList = []  # type: List[CircuitLine]
+        circuitList: List[CircuitLine] = []
         procedureCircuitList = self.procedureMap[procName].circuitList
         
         argumentMap = self.procedureArgumentMap[procName]
 
         for circuit in procedureCircuitList:
             procedureName = circuit.pbCircuitLine.procedureName
             pendingArgumentList = circuit.pendingArgumentList
             
-            newQRegList = []  # type: List[int]
+            newQRegList: List[int] = []
             for i in circuit.pbCircuitLine.qRegList:
                 q = regIdList[i]
                 newQRegList.append(q)
 
             realArgumentList = self.getRealArgumentList(procArguments, pendingArgumentList, argumentMap)
             if procedureName:
                 gateName = circuit.pbCircuitLine.procedureName
@@ -706,18 +706,18 @@
         """
         Check quantum registers. 
         Declaring multiple variables is temporarily not support.
         Check the same variables declared in classic registers.
 
         :param ctx: type: object. QASMParser.QRegContext
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
-        id = ctx.ID().getText()  # type: str
+        id: str = ctx.ID().getText()
         self.checkQregLimit(id, line, position)
         regSize = int(ctx.INT().getText())
         # create sequence number list for array
         regList = self.genSequenceArray(regSize)
         self.qRegVarMap[id] = regSize
         self.usingQRegList = regList
 
@@ -731,18 +731,18 @@
         """
         Check classic registers. 
         Declaring multiple variables is temporarily not support.
         Check the same variables declared in quantum registers.
 
         :param ctx: type: object. QASMParser.CRegContext
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
-        id = ctx.ID().getText()  # type: str
+        id: str = ctx.ID().getText()
         self.checkCregLimit(id, line, position)
         regSize = int(ctx.INT().getText())
         # create sequence number list for array
         regList = self.genSequenceArray(regSize)
         self.cRegVarMap[id] = regSize
         self.usingCRegList = regList
 
@@ -756,21 +756,21 @@
     def getOpName(self, ctx) -> str:
         """
         Get the name of operation instruction.
 
         :param ctx: type: object. QASMParser.UopContext
         """
         # line number
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
-        opCmd = ctx.ID()  # type: str
+        opCmd = ctx.ID()
 
         if opCmd:
-            opId = opCmd.getText()
+            opId: str = opCmd.getText()
         else:
             raise Error.ArgumentError(f'Illegal operation on gate. line: {line}, position: {position}.',
                                       ModuleErrorCode, FileErrorCode, 21)
 
         return opId
 
 
@@ -779,16 +779,16 @@
         Get the type of gate operation.
 
         :param ctx: type: object. QASMParser.UopContext
         :param opId: type: str. The name of operation. For example, 'ID', 'CX', and 'CSWAP'.
 
         :return: type: Tuple[str, Union[str,int], bool]. (gateType, gateName, argumentIdField)
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
         argumentIdField = False
         state = self.getScopeData().state
         if state == QasmParseState.Procedure:
             argumentIdField = True
 
         gateIdCheck = opId.upper()
         gateF = FixedGateIdMap.get(gateIdCheck)
@@ -835,35 +835,35 @@
 
         :param ctx: type: object. QASMParser.UopContext.
         :param opId: type: str. The name of operation. For example, 'ID', 'CX', and 'CSWAP'.
         :param idList: type: object. List of ids.
         :param circuitList: type: List[CircuitLine]. List of circuitLines.
         """
         # line number
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
         gateType, gateName, argumentIdField = self.getGateNameType(ctx, opId)
         arguments, argumentIdList = self.getArguments(ctx)
 
         idArguments = idList.ID()
         self.checkUOpArgumentIdList(idArguments, line, position)
         # Check variable declaration. Only one id argument uses.
-        argument = idArguments[0].getText()  # type: str
+        argument: str = idArguments[0].getText()
         scopeData = self.getScopeData()
         state = scopeData.state
         qReg = scopeData.qReg
         regMap = scopeData.regMap
         procName = scopeData.procName
 
         # Check the number of used registers. Only one register can be expanded so far. 
         idLens = len(idArguments)
         if idLens > 1:
             # command of procedure. Call registers declared in multiple procedures. 
             # Get list of registers according to their positions.
-            regList = [regMap[id.getText()] for id in idArguments]  # type: List[int]
+            regList: List[int] = [regMap[id.getText()] for id in idArguments]
             
             if gateType == 'procedureName':
                 self.checkProcName(procName, gateName, line, position)
                 self.checkProcArgumentsCount(gateName, arguments, line, position)
             
             self.createProcCircuit(circuitList, arguments, argumentIdList, argumentIdField, gateType, gateName, regList)
         else:
@@ -884,16 +884,16 @@
         Operation registers with index, such as h q[1];
 
         :param ctx: type: object. QASMParser.UopContext
         :param opId: type: str. Operation name such as u, cx
         :param mixList: type: object. QASMParser.MixedlistContext
         :param circuitList: type: List[CircuitLine]. List of circuitLines.
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
         gateType, gateName, argumentIdField = self.getGateNameType(ctx, opId)
         arguments, argumentIdList = self.getArguments(ctx)
         scopeData = self.getScopeData()
         state = scopeData.state
 
         mixId = mixList.ID()
         mixArgument = mixList.INT()
@@ -902,15 +902,15 @@
             raise Error.ArgumentError(
                 f'Illegal operation on gate. line: {line}, position: {position}.', ModuleErrorCode, FileErrorCode, 23)
 
         # Check number of arguments.
         self.checkArgumentsCount(opId, len(mixId), line, position)
 
         # Check validity of variables.
-        regName = None  # type: str
+        regName: str = None
         for m in mixId:
             mid = m.getText()
             if not regName:
                 regName = mid
             self.checkQregVar(mid, line, position)
         # Check out-of-bounds access.
         usageIds = []
@@ -954,16 +954,16 @@
         Regular check:
             Valid command. 
             Valid variable. 
             Out-of-bounds cccess. 
         """
 
         # line number
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
         # Check the current state. If procedure is being processed, 
         # turns to process the circuitList of procedureMap.
         circuitList = self.getCurrentCircuitsContainer()
 
         # Operation command, such as u, cx, swap, ry, etc.
         opId = self.getOpName(ctx)
@@ -992,23 +992,23 @@
         :param ctx: type: object. ctx is QASMParser.MeasureOpContext.
 
         Format: measure q -> c;
         # NOTE: the size of q is not greater than c.
 
         measure q[0] -> c[0];
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
         argument = ctx.argument()
         qReg = argument[0]
         cReg = argument[1]
 
-        qRegId = qReg.ID().getText()
-        cRegId = cReg.ID().getText()
+        qRegId: str = qReg.ID().getText()
+        cRegId: str = cReg.ID().getText()
 
         self.checkQregVar(qRegId, line, position)
         self.checkCregVar(cRegId, line, position)
 
         qRegInt = qReg.INT()
         cRegInt = cReg.INT()
 
@@ -1082,15 +1082,15 @@
             mixId = mixList.ID()
             mixArgument = mixList.INT()
             if len(mixId) != len(mixArgument):
                 raise Error.ArgumentError(f'Illegal operation on gate. line: {line}, position: {position}.',
                                           ModuleErrorCode, FileErrorCode, 25)
 
             # Check validity of variables.
-            regName = None  # type: str
+            regName: str = None
             for m in mixId:
                 mid = m.getText()
                 if not regName:
                     regName = mid
                 self.checkQregVar(mid, line, position)
             # Check out-of-bounds access.
             usageIds = []
@@ -1106,16 +1106,16 @@
         """
         Visit expression list.
         
         :param ctx: type: object. QASMParser.UopContext.
 
         :return: expression. 
         """
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
         scopeData = self.getScopeData()
         argumentIdList = scopeData.argumentIdList
         argumentValueList = scopeData.argumentValueList
         argumentMap = scopeData.argumentMap
         argumentExprList = scopeData.argumentExprList
 
         expList = []
@@ -1171,26 +1171,26 @@
                 'flag': -1,
                 'text': calcText,
                 'val': str(reVal),
                 'expr': exprList
             }
         """
 
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
         exprList = []
 
         calcList = []
 
         count = ctx.getChildCount()
         
         calcArgumentList = []
         
-        checkItem = []  # type: List[bool]
+        checkItem: List[bool] = []
         for i in range(count):
             item = ctx.getChild(i)
             itemText = item.getText()
             # check if argument has been declared.
             checkFlag = self.checkArgumentDeclared(itemText)
             checkItem.append(checkFlag)
             if checkFlag:
@@ -1250,18 +1250,18 @@
         """
         Declaration of procedure.
         Current scope is stacked into procStack.
 
         :param ctx: type: object. QASMParser.GatedeclContext
         """
         # line number
-        line = ctx.start.line  # type: int
-        position = ctx.start.column  # type: int
+        line: int = ctx.start.line
+        position: int = ctx.start.column
 
-        gateId = ctx.ID().getText()
+        gateId: str = ctx.ID().getText()
         # Check duplication of procedure names.
         if gateId in self.procedureVarSet:
             # Duplication
             raise Error.ArgumentError(
                 f'Duplicated procedure name ${gateId}, line: ${line}, position: ${position}.', ModuleErrorCode,
                 FileErrorCode, 27)
```

### Comparing `qcompute-3.2.1/QCompute/OpenConvertor/__init__.py` & `qcompute-3.3.0/QCompute/OpenConvertor/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenModule/CompositeGateModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/CompositeGateModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenModule/CompressGateModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/CompressGateModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenModule/InverseCircuitModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/InverseCircuitModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenModule/ReverseCircuitModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/ReverseCircuitModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenModule/UnrollCircuitModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/UnrollCircuitModule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
                         # U3: gate u3(theta,phi,lamda) a { U(theta,phi,lamda) a; }
                         # U2: gate u2(theta,phi) a { U(pi/2,theta,phi) a; }
                         # U1: gate u1(theta) a { U(0,0,theta) a; }
                         circuitOut.append(
                             gateToProtobuf(U(*_expandAnglesInUGate(list(circuitLine.argumentValueList))), [a]))
                         return
                     else:
-                        ret = deepcopy(circuitLine)  # type: 'PBCircuitLine'
+                        ret = deepcopy(circuitLine)
                         circuitOut.append(ret)
                         return
                 elif rotationGate == PBRotationGate.RX:
                     # RX: gate rx(theta) a { u3(theta, -pi/2,pi/2) a; }
                     self._unrollRecursively(gateToProtobuf(U(theta, -np.pi / 2.0, np.pi / 2.0), [a]), circuitOut)
                     return
                 elif rotationGate == PBRotationGate.RY:
@@ -382,15 +382,15 @@
 
         # Unsupported gate
         if self.errorOnUnsupported:
             # error
             raise Error.ArgumentError(f'Unsupported operation {circuitLine}!', ModuleErrorCode, FileErrorCode, 4)
         else:
             # ignore
-            ret = deepcopy(circuitLine)  # type: 'PBCircuitLine'
+            ret = deepcopy(circuitLine)
             circuitOut.append(ret)
 
     def _decompose(self, circuitOut: List['PBCircuitLine'], circuitIn: List['PBCircuitLine']):
         """
         Unroll the gates
 
         :param circuitOut: input circuit
```

### Comparing `qcompute-3.2.1/QCompute/OpenModule/UnrollNoiseModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/UnrollNoiseModule/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,22 +62,22 @@
 
         ret.body.noiseMap.clear()
 
         return ret
 
     def _findGate(self, pbCircuit: List[PBCircuitLine], gateName: str, qRegList: List[int],
                   positionList: Optional[List[int]]) -> List[PBCircuitLine]:
-        gateList = []  # type: List[PBCircuitLine]
+        gateList: List[PBCircuitLine] = []
         for pbCircuitLine in pbCircuit:
             op = pbCircuitLine.WhichOneof('op')
             if op == 'fixedGate':
-                fixedGate = pbCircuitLine.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = pbCircuitLine.fixedGate
                 opName = PBFixedGate.Name(fixedGate)
             elif op == 'rotationGate':
-                rotationGate = pbCircuitLine.rotationGate  # type: PBRotationGate
+                rotationGate: PBRotationGate = pbCircuitLine.rotationGate
                 opName = PBRotationGate.Name(rotationGate)
             else:
                 continue
             if opName != gateName:
                 continue
 
             if not qRegList or set(pbCircuitLine.qRegList) == set(qRegList):
```

### Comparing `qcompute-3.2.1/QCompute/OpenModule/UnrollProcedureModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/UnrollProcedureModule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def _unrollProcedure(self, circuit: List['PBCircuitLine'], qRegMap: Dict[int, int],
                          argumentValueList: Optional[List[float]]) -> None:
         # Fill in the circuit
         for circuitLine in circuit:
             op = circuitLine.WhichOneof('op')
             if op in ['fixedGate', 'rotationGate', 'compositeGate', 'measure', 'barrier']:
-                ret = deepcopy(circuitLine)  # type: 'PBCircuitLine'
+                ret = deepcopy(circuitLine)
                 if len(ret.argumentIdList) > 0:
                     if len(ret.argumentValueList) == 0:
                         ret.argumentValueList[:] = [0.0] * len(ret.argumentIdList)
                     for index, argumentId in enumerate(ret.argumentIdList):
                         if argumentId >= 0:
                             ret.argumentValueList[index] = argumentValueList[argumentId]
                     del ret.argumentIdList[:]
```

### Comparing `qcompute-3.2.1/QCompute/OpenModule/__init__.py` & `qcompute-3.3.0/QCompute/OpenModule/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/__init__.py` & `qcompute-3.3.0/QCompute/OpenService/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/__init__.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/__init__.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/client.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,16 @@
         self.__shot_inboxes = [Queue() for _ in range(self.__shots)]
 
         self.__bar = None
         self.__ws_conn = None
 
         # Queue is thread-safe so that it can be shared
         self.shot_outbox = Queue()
-        self.ret = {}  # type: Dict[str,int]
-        self.shot_threadings = {}  # type: Dict[int, threading.Thread]
+        self.ret: Dict[str,int] = {}
+        self.shot_threadings: Dict[int, threading.Thread] = {}
         self.program = program
         self.phase_auth = True  # whether or not in the testing process
         self.entry = None
         self.secret = None
         self.failed = True
 
         width, depth = self.__extract_graph_shape()
@@ -502,20 +502,20 @@
             inbox (Queue): inbox queue
             outbox (Queue): outbox queue
             program (PBProgram): program of quantum circuit to be executed
         """
         self.__circuit = None  # circuit
         self.__client_knowledge = {}  # client knowledge
         self.__bw_pattern = None  # brickwork pattern
-        self.__width = None  # type: int # width
-        self.__depth = None  # type: int # depth
-        self.__shots = shots  # type: int # shot
+        self.__width: int = None  # width
+        self.__depth: int = None  # depth
+        self.__shots: int = shots # shot
         self.__states = None
-        self.inbox = inbox  # type: Queue
-        self.outbox = outbox  # type: Queue
+        self.inbox: Queue = inbox
+        self.outbox: Queue = outbox
         self.program = program
         super().__init__()
 
     def send_back(self, action, payload):
         r"""Send back the action and payload messages.
 
         Args:
@@ -573,15 +573,15 @@
         _init_.width = self.__width
         _init_.depth = self.__depth
 
         for vec in self.__states:
             vec_buf = numpyMatrixToProtobufMatrix(vec)
             _init_.vector.append(vec_buf)
 
-        init_stateBuf = _init_.SerializeToString()  # type: bytes
+        init_stateBuf: bytes = _init_.SerializeToString()
 
         self.send_back(
             'remote',
             self.__wrap_shot_message(
                 'setInitState',
                 {'state': b64encode(init_stateBuf).decode()}
             )
@@ -616,15 +616,15 @@
 
         # Establish a request to send the messages to the server
         req = PBEncryptedMeasureReq()
         for angle in angles:
             req.angles.append(angle)
 
         # Encode the message by serialization
-        reqBuf = req.SerializeToString()  # type: bytes
+        reqBuf: bytes = req.SerializeToString()
 
         self.send_back(
             'remote',
             self.__wrap_shot_message(
                 'setAngleBulk',
                 {'angle': b64encode(reqBuf).decode()},
             )
@@ -728,19 +728,19 @@
 
         # Warning: In the circuit model, the quantum states are initialized with |0>.
         # While in MBQC model, the quantum states are initialized with |+>.
         # Therefore, each qubit in the MBQC circuit should be operated by a ``Hadamard`` gate in the front.
         for i in range(width):
             circuit.h(i)
 
-        for PBGate in pbCircuit:  # type: PBCircuitLine
+        for PBGate in pbCircuit:
             op = PBGate.WhichOneof('op')
             # Map ``fixedGate`` (including 'H', 'CX', 'X', 'Y', 'Z', 'S', 'T', 'CZ') to the methods in ``Circuit``
             if op == 'fixedGate':
-                fixedGate = PBGate.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = PBGate.fixedGate
                 gateName = PBFixedGate.Name(fixedGate)
                 bit_idx = PBGate.qRegList
                 if gateName == 'H':
                     circuit.h(bit_idx[0])
                 elif gateName == 'CX':
                     circuit.cnot(bit_idx)
                 elif gateName == 'X':
@@ -762,15 +762,15 @@
                     raise Error.ArgumentError(f"Invalid gate: ({gateName})!\n"
                                               "Only 'H', 'CX', 'X', 'Y', 'Z', 'S', 'T', 'CZ' are supported as the "
                                               "fixed gates in UBQC in this version.", ModuleErrorCode,
                                               FileErrorCode, 8)
 
             # Map ``rotationGate`` (including 'RX', 'RY', 'RZ', 'U') to the methods in ``Circuit``
             elif op == 'rotationGate':
-                rotationGate = PBGate.rotationGate  # type: PBRotationGate
+                rotationGate: PBRotationGate = PBGate.rotationGate
                 gateName = PBRotationGate.Name(rotationGate)
                 bit_idx = PBGate.qRegList
 
                 if gateName == 'RX':
                     circuit.rx(PBGate.argumentValueList[0], bit_idx[0])
                 elif gateName == 'RY':
                     circuit.ry(PBGate.argumentValueList[0], bit_idx[0])
@@ -818,15 +818,15 @@
                 if measurement_qubits != set(range(width)):
                     raise Error.ArgumentError(f"Invalid measurement qubits: ({measurement_qubits})!\n"
                                               "All qubits must be measured in UBQC in this version.",
                                               ModuleErrorCode,
                                               FileErrorCode, 10)
 
                 for qReg in PBGate.qRegList:
-                    typeName = PBMeasure.Type.Name(PBGate.measure.type)  # type: PBMeasure
+                    typeName: PBMeasure = PBMeasure.Type.Name(PBGate.measure.type)
                     if typeName == 'Z':
                         circuit.measure(qReg)
                     else:
                         raise Error.ArgumentError(f"Invalid measurement type: ({typeName})!\n"
                                                   "Only 'Z measurement' is supported as the measurement type "
                                                   "in UBQC in this version.",
                                                   ModuleErrorCode,
```

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/mcalculus.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/mcalculus.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/qobject.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/qobject.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/transpiler.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/transpiler.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenService/service_ubqc/client/utils.py` & `qcompute-3.3.0/QCompute/OpenService/service_ubqc/client/utils.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/__init__.py` & `qcompute-3.3.0/QCompute/OpenSimulator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,30 +33,30 @@
 
 
 class SimulatorVersion:
     """
     The version of quantum simulator.
     """
 
-    gitHash = None  # type: str
+    gitHash: str = None
     """
     Git Hash
     """
 
-    gitTime = None  # type: str
+    gitTime: str = None
     """
     Git Time
     """
 
-    fileHash = None  # type: str
+    fileHash: str = None
     """
     File Hash
     """
 
-    compileTime = None  # type: str
+    compileTime: str = None
     """
     Compile Time
     """
 
     def __init__(self):
         self.gitHash = None
         self.gitTime = None
@@ -64,30 +64,30 @@
         self.compileTime = None
 
 
 class Ancilla:
     """
     Ancilla
     """
-    usedQRegList = None  # type: List[int]
+    usedQRegList: List[int] = None
     """
     used qReg list
     """
 
-    usedCRegList = None  # type: List[int]
+    usedCRegList: List[int] = None
     """
     used cReg list
     """
 
-    compactedQRegDict = None  # type: Dict[int, int]
+    compactedQRegDict: Dict[int, int] = None
     """
     computed qReg list
     """
 
-    compactedCRegDict = None  # type: Dict[int, int]
+    compactedCRegDict: Dict[int, int] = None
     """
     measured qReg list
     """
 
     def __init__(self):
         self.usedQRegList = None
         self.usedCRegList = None
@@ -101,15 +101,15 @@
     """
 
     sdkVersion = Define.sdkVersion
     """
     SDK Version from Define.sdkVersion
     """
 
-    simulatorVersion = None  # type: SimulatorVersion
+    simulatorVersion: SimulatorVersion = None
     """
     The version of quantum simulator
     """
 
     code = 0
     """
     error code
@@ -126,35 +126,35 @@
     """
 
     log = ''
     """
     output results
     """
 
-    ancilla = Ancilla()  # type: Ancilla
+    ancilla: Ancilla = Ancilla()
     """
     ancilla
     """
 
-    moduleList = None  # type:Dict[str,Any]
+    moduleList:Dict[str,Any] = None
     """
     moduleList
     """
 
     shots = 0
     """
     number of shots
     """
 
-    counts = None  # type: Union[Dict[str, int], Dict[str, float]]
+    counts: Union[Dict[str, int], Dict[str, float]] = None
     """
     counts for results
     """
 
-    state = None  # type: numpy.ndarray
+    state: numpy.ndarray = None
     """
     counts for results
     """
 
     seed = 0
     """
     random seed
@@ -260,15 +260,15 @@
 class QImplement:
     """
     Implement params for quantum execution.
 
     Send to the simulator when submitting a task.
     """
 
-    program = None  # type:
+    program = None
     """
     Protobuf format of the circuit
     """
 
     shots = 0
     """
     Number of shots
```

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/InitState.py` & `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/InitState.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 from enum import unique, IntEnum
 from typing import Union
 
 import numpy
 
 
 
-from QCompute.QPlatform import Error
-
 
 @unique
 class MatrixType(IntEnum):
     """
     
     DEFINE the matrix type here.
     """
```

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Measure.py` & `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Measure.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
     def _measureBySingleAccumulation(self, state: numpy.ndarray, shots: int) -> Dict[str, int]:
         """
         Measure by accumulation, one shot at a time
         """
 
         # print("Measure method Single Accu")
-        result = {}  # type: Dict[str, int]
+        result: Dict[str, int] = {}
         for i in range(shots):
             outs = self._measureAll(state)
             if outs not in result:
                 result[outs] = 0
             result[outs] += 1
         return result
 
@@ -188,15 +188,15 @@
         # print("The sum prob is ", sum(prob_values))
 
         samples = numpy.random.choice(len(prob_key), shots, p=prob_values)
         """
 
         samples = numpy.random.choice(range(2 ** n), shots, p=prob_array)
         count_samples = Counter(samples)
-        result = {}  # type: Dict[str, int]
+        result: Dict[str, int] = {}
         for idex in count_samples:
             """
             result[prob_key[idex]] = count_samples[idex]
             """
             result[numToBinStr(idex, n)] = count_samples[idex]
         return result
```

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py` & `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from datetime import datetime
 from pathlib import Path
 from typing import List, Union, Dict, Optional
 
 import multiprocess
 import numpy
 from google.protobuf.json_format import MessageToDict, ParseDict
+
 from QCompute import Define
 from QCompute.Define import Settings
 from QCompute.Define.Settings import NoiseMethod
 from QCompute.OpenConvertor.JsonToCircuit import JsonToCircuit
 from QCompute.OpenSimulator import QResult, ModuleErrorCode, withNoise
 from QCompute.OpenSimulator.local_baidu_sim2.InitState import MatrixType, initState_1_0
 from QCompute.OpenSimulator.local_baidu_sim2.Measure import MeasureMethod, Measurer
@@ -149,15 +150,15 @@
                     if Settings.noiseMultiprocessingSimulator:
                         self.programDict = MessageToDict(self.program)
                         self.program = None
                         noise_rng_array = []
                         for i in range(len(noise_rngList[0])):
                             array = []
                             for j in range(len(noise_rngList)):
-                                 array.append(noise_rngList[j][i])
+                                array.append(noise_rngList[j][i])
                             noise_rng_array.append(array)
                         countsList = list(pool.map(self.core_once_mixed_unitary_noise, noise_rng_array))
                     else:
                         countsList = list(map(self.core_once_mixed_unitary_noise, *noise_rngList))
 
                     # counts accumulate
                     for element in countsList:
@@ -377,48 +378,48 @@
                 pointer += 1
 
         measured = False
         pointer = 0
         for circuitLine in program.body.circuit:  # Traverse the circuit
             op = circuitLine.WhichOneof('op')
 
-            qRegList = [qRegMap[_] for _ in circuitLine.qRegList]  # type List[int]
+            qRegList: List[int] = [qRegMap[_] for _ in circuitLine.qRegList]
 
             if op == 'fixedGate':  # fixed gate
-                fixedGate = circuitLine.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = circuitLine.fixedGate
                 matrix = operationDict.get(fixedGate)
                 if matrix is None:
                     raise Error.ArgumentError(f'Unsupported operation {PBFixedGate.Name(fixedGate)}!', ModuleErrorCode,
                                               FileErrorCode, 10)
                 state = transfer(state, matrix, qRegList)
                 transfer_noise_matrix(noise_rng)
 
             elif op == 'rotationGate':  # rotation gate
-                uGate = getRotationGate(circuitLine)  # type RotationGateOp
+                uGate: RotationGateOP = getRotationGate(circuitLine)
 
                 if matrixType == MatrixType.Dense:
                     matrix = uGate.getMatrix()
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 state = transfer(state, matrix, qRegList)
                 transfer_noise_matrix(noise_rng)
             elif op == 'customizedGate':  # customized gate
-                customizedGate = circuitLine.customizedGate  # type: PBCustomizedGate
+                customizedGate: PBCustomizedGate = circuitLine.customizedGate
                 if matrixType == MatrixType.Dense:
                     matrix = protobufMatrixToNumpyMatrix(customizedGate.matrix)
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 state = transfer(state, matrix, qRegList)
                 transfer_noise_matrix(noise_rng)
             elif op == 'procedureName':  # procedure
                 raise Error.ArgumentError('Unsupported operation procedure, please flatten by UnrollProcedureModule!',
                                           ModuleErrorCode, FileErrorCode, 12)
                 # it is not implemented, flattened by UnrollProcedureModule
             elif op == 'measure':  # measure
-                measure = circuitLine.measure  # type: PBMeasure
+                measure: PBMeasure = circuitLine.measure
                 if measure.type != PBMeasure.Type.Z:  # only Z measure is supported
                     raise Error.ArgumentError(
                         f'Unsupported operation measure {PBMeasure.Type.Name(measure.type)}!', ModuleErrorCode,
                         FileErrorCode, 13)
                 if not measured:
                     counts = measurer(state, shots)
                     measured = True
@@ -492,25 +493,25 @@
 
             return noiseRng
 
         for circuitLine in program.body.circuit:  # Traverse the circuit
             op = circuitLine.WhichOneof('op')
 
             if op == 'fixedGate':  # fixed gate
-                fixedGate = circuitLine.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = circuitLine.fixedGate
                 matrix = operationDict.get(fixedGate)
                 if matrix is None:
                     raise Error.ArgumentError(f'Unsupported operation {PBFixedGate.Name(fixedGate)}!', ModuleErrorCode,
                                               FileErrorCode, 10)
 
                 rngList = transfer_noise_rng(max_run_num)
                 if rngList:
                     batchedNoiseRng.append(rngList)
             elif op == 'rotationGate':  # rotation gate
-                rotationGate = circuitLine.rotationGate  # type: PBRotationGate
+                rotationGate: PBRotationGate = circuitLine.rotationGate
                 if rotationGate - PBRotationGate.U > 7:  # current support 8 rotation gates
                     raise Error.ArgumentError(
                         f'Unsupported operation {PBRotationGate.Name(rotationGate)}!', ModuleErrorCode, FileErrorCode,
                         11)
 
                 rngList = transfer_noise_rng(max_run_num)
                 if rngList:
@@ -619,44 +620,44 @@
                         ModuleErrorCode, FileErrorCode, 8)
                 state = transfer(state, noise_matrix, qRegList)
 
         measured = False
         for circuitLine in program.body.circuit:  # Traverse the circuit
             op = circuitLine.WhichOneof('op')
 
-            qRegList = [qRegMap[_] for _ in circuitLine.qRegList]  # type List[int]
+            qRegList: List[int] = [qRegMap[_] for _ in circuitLine.qRegList]
 
             if op == 'fixedGate':  # fixed gate
-                fixedGate = circuitLine.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = circuitLine.fixedGate
                 matrix = operationDict.get(fixedGate)
                 if matrix is None:
                     raise Error.ArgumentError(f'Unsupported operation {PBFixedGate.Name(fixedGate)}!', ModuleErrorCode,
                                               FileErrorCode, 10)
                 transfer_noise_list()
             elif op == 'rotationGate':  # rotation gate
-                uGate = getRotationGate(circuitLine)  # type RotationGateOp
+                uGate: RotationGateOP = getRotationGate(circuitLine)
 
                 if matrixType == MatrixType.Dense:
                     matrix = uGate.getMatrix()
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 transfer_noise_list()
             elif op == 'customizedGate':  # customized gate
-                customizedGate = circuitLine.customizedGate  # type: PBCustomizedGate
+                customizedGate: PBCustomizedGate = circuitLine.customizedGate
                 if matrixType == MatrixType.Dense:
                     matrix = protobufMatrixToNumpyMatrix(customizedGate.matrix)
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 transfer_noise_list()
             elif op == 'procedureName':  # procedure
                 raise Error.ArgumentError('Unsupported operation procedure, please flatten by UnrollProcedureModule!',
                                           ModuleErrorCode, FileErrorCode, 12)
                 # it is not implemented, flattened by UnrollProcedureModule
             elif op == 'measure':  # measure
-                measure = circuitLine.measure  # type: PBMeasure
+                measure: PBMeasure = circuitLine.measure
                 if measure.type != PBMeasure.Type.Z:  # only Z measure is supported
                     raise Error.ArgumentError(
                         f'Unsupported operation measure {PBMeasure.Type.Name(measure.type)}!', ModuleErrorCode,
                         FileErrorCode, 13)
                 if not measured:
                     counts = measurer(state, shots)
                     measured = True
@@ -903,48 +904,48 @@
             elif measureMethod in [MeasureMethod.OutputState, MeasureMethod.OutputProbability]:
                 pass
 
         measured = False
         for circuitLine in program.body.circuit:  # Traverse the circuit
             op = circuitLine.WhichOneof('op')
 
-            qRegList = [qRegMap[_] for _ in circuitLine.qRegList]  # type List[int]
+            qRegList: List[int] = [qRegMap[_] for _ in circuitLine.qRegList]
 
             if not stateDict:  # Verify the output stateDict is not None
                 return {}
             else:
                 if op == 'fixedGate':  # fixed gate
-                    fixedGate = circuitLine.fixedGate  # type: PBFixedGate
+                    fixedGate: PBFixedGate = circuitLine.fixedGate
                     matrix = operationDict.get(fixedGate)
                     if matrix is None:
                         raise Error.ArgumentError(f'Unsupported operation {PBFixedGate.Name(fixedGate)}!',
                                                   ModuleErrorCode, FileErrorCode, 10)
                     transfer_batch_noisy_gate(matrix, num)
                 elif op == 'rotationGate':  # rotation gate
-                    uGate = getRotationGate(circuitLine)  # type RotationGateOp
+                    uGate: RotationGateOP = getRotationGate(circuitLine)
 
                     if matrixType == MatrixType.Dense:
                         matrix = uGate.getMatrix()
                     else:
                         from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                     transfer_batch_noisy_gate(matrix, num)
                 elif op == 'customizedGate':  # customized gate
-                    customizedGate = circuitLine.customizedGate  # type: PBCustomizedGate
+                    customizedGate: PBCustomizedGate = circuitLine.customizedGate
                     if matrixType == MatrixType.Dense:
                         matrix = protobufMatrixToNumpyMatrix(
                             customizedGate.matrix)
                     else:
                         from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                     transfer_batch_noisy_gate(matrix, num)
                 elif op == 'proceduresName':  # procedure
                     raise Error.ArgumentError('Unsupported operation procedure, please flatten by '
                                               'UnrollProcedureModule!', ModuleErrorCode, FileErrorCode, 12)
                     # it is not implemented, flattened by UnrollProcedureModule
                 elif op == 'measure':  # measure
-                    measure = circuitLine.measure  # type: PBMeasure
+                    measure: PBMeasure = circuitLine.measure
                     if measure.type != PBMeasure.Type.Z:  # only Z measure is supported
                         raise Error.ArgumentError(
                             f'Unsupported operation measure {PBMeasure.Type.Name(measure.type)}!', ModuleErrorCode,
                             FileErrorCode, 13)
                     if not measured:
                         # measure a batch of states
                         counts = batch_measure(stateDict, measurer, shots)
@@ -967,15 +968,15 @@
             else:
                 stateDict = {key: normalizeNdarrayOrderForTranspose(value.todense()) for key, value in
                              stateDict.items()}
             return stateDict
 
     def core_once_without_noise(self) -> Union[Dict[str, int], Dict[str, float], numpy.ndarray]:
         """
-        Simulaton process for ideal circuit
+        Simulation process for ideal circuit
         """
 
         if self.program is None:
             program = PBProgram()
             ParseDict(self.programDict, program)
         else:
             program = self.program
@@ -998,48 +999,48 @@
         transfer = TransferProcessor(matrixType, algorithm)
         measurer = Measurer(matrixType, algorithm, measureMethod)
 
         measured = False
         for circuitLine in program.body.circuit:  # Traverse the circuit
             op = circuitLine.WhichOneof('op')
 
-            qRegList = [qRegMap[qReg] for qReg in circuitLine.qRegList]  # type List[int]
+            qRegList: List[int] = [qRegMap[qReg] for qReg in circuitLine.qRegList]
 
             if op == 'fixedGate':  # fixed gate
-                fixedGate = circuitLine.fixedGate  # type: PBFixedGate
+                fixedGate: PBFixedGate = circuitLine.fixedGate
                 matrix = operationDict.get(fixedGate)
                 if matrix is None:
                     raise Error.ArgumentError(f'Unsupported operation {PBFixedGate.Name(fixedGate)}!', ModuleErrorCode,
                                               FileErrorCode, 7)
                 state = transfer(state, matrix, qRegList)
             elif op == 'rotationGate':  # rotation gate
-                rotationGate = circuitLine.rotationGate  # type: PBRotationGate
+                rotationGate: PBRotationGate = circuitLine.rotationGate
                 if rotationGate != PBRotationGate.U:
                     raise Error.ArgumentError(
                         f'Unsupported operation {PBRotationGate.Name(rotationGate)}!', ModuleErrorCode, FileErrorCode,
                         8)
                 uGate = U(*circuitLine.argumentValueList)
                 if matrixType == MatrixType.Dense:
                     matrix = uGate.getMatrix()
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 state = transfer(state, matrix, qRegList)
             elif op == 'customizedGate':  # customized gate
-                customizedGate = circuitLine.customizedGate  # type: PBCustomizedGate
+                customizedGate: PBCustomizedGate = circuitLine.customizedGate
                 if matrixType == MatrixType.Dense:
                     matrix = protobufMatrixToNumpyMatrix(customizedGate.matrix)
                 else:
                     from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
                 state = transfer(state, matrix, qRegList)
             elif op == 'procedureName':  # procedure
                 raise Error.ArgumentError('Unsupported operation procedure, please flatten by UnrollProcedureModule!',
                                           ModuleErrorCode, FileErrorCode, 9)
                 # it is not implemented, flattened by UnrollProcedureModule
             elif op == 'measure':  # measure
-                measure = circuitLine.measure  # type: PBMeasure
+                measure: PBMeasure = circuitLine.measure
                 if measure.type != PBMeasure.Type.Z:  # only Z measure is supported
                     raise Error.ArgumentError(
                         f'Unsupported operation measure {PBMeasure.Type.Name(measure.type)}!', ModuleErrorCode,
                         FileErrorCode, 10)
                 if not measured:
                     counts = measurer(state, shots)
                     measured = True
@@ -1061,15 +1062,15 @@
 
     @staticmethod
     def loadGates(matrixType: 'MatrixType') -> Dict['PBFixedGate', Union[numpy.ndarray, 'COO']]:
         """
         Load the matrix of the gate
         """
         if matrixType == MatrixType.Dense:
-            operationDict = {
+            operationDict: Dict['PBFixedGate', Union[numpy.ndarray, 'COO']] = {
                 PBFixedGate.ID: ID.getMatrix(),
                 PBFixedGate.X: X.getMatrix(),
                 PBFixedGate.Y: Y.getMatrix(),
                 PBFixedGate.Z: Z.getMatrix(),
                 PBFixedGate.H: H.getMatrix(),
                 PBFixedGate.S: S.getMatrix(),
                 PBFixedGate.SDG: SDG.getMatrix(),
@@ -1078,25 +1079,25 @@
                 PBFixedGate.CX: CX.getMatrix().reshape(2, 2, 2, 2),
                 PBFixedGate.CY: CY.getMatrix().reshape(2, 2, 2, 2),
                 PBFixedGate.CZ: CZ.getMatrix().reshape(2, 2, 2, 2),
                 PBFixedGate.CH: CH.getMatrix().reshape(2, 2, 2, 2),
                 PBFixedGate.SWAP: SWAP.getMatrix(),
                 PBFixedGate.CCX: CCX.getMatrix(),
                 PBFixedGate.CSWAP: CSWAP.getMatrix()
-            }  # type: Dict['PBFixedGate', Union[numpy.ndarray, 'COO']]
+            }
         else:
             from QCompute.QPlatform import Error; raise Error.RuntimeError('Not implemented')
         return operationDict
 
 
 def getRotationGate(circuitLine: 'PBCircuitLine') -> 'RotationGateOP':
     """
     Get the rotation gate instance form PBCircuitLine
     """
-    rotationGate = circuitLine.rotationGate  # type: PBRotationGate
+    rotationGate: PBRotationGate = circuitLine.rotationGate
     if rotationGate - PBRotationGate.U == 0:
         ugate = U(*circuitLine.argumentValueList)
     elif rotationGate - PBRotationGate.U == 1:
         ugate = RX(*circuitLine.argumentValueList)
     elif rotationGate - PBRotationGate.U == 2:
         ugate = RY(*circuitLine.argumentValueList)
     elif rotationGate - PBRotationGate.U == 3:
@@ -1173,47 +1174,47 @@
     parser.add_argument('-mm', default='probability', type=str)
 
     parser.add_argument('-s', default=None, type=int)
     parser.add_argument('-shots', default=None, type=int)
     parser.add_argument('-inputFile', default=None, type=str)
 
     args = parser.parse_args(args=args)
-    matrixType = args.mt.lower()  # type: str
-    algorithm = args.a.lower()  # type: str
-    measureMethod = args.mm.lower()  # type: str
-    seed = args.s  # type: int
-    shots = args.shots  # type: int
-    inputFile = args.inputFile  # type: str
+    matrixType: str = args.mt.lower()
+    algorithm: str = args.a.lower()
+    measureMethod: str = args.mm.lower()
+    seed: int = args.s
+    shots: int = args.shots
+    inputFile: str = args.inputFile
 
     if shots < 1 or shots > Define.maxShots:
         raise Error.ArgumentError(f'Invalid shots {shots}, should in [0, {Define.maxShots}]', ModuleErrorCode,
                                   FileErrorCode, 1)
     if seed is not None:
         if seed < 0 or seed > Define.maxSeed:
             raise Error.ArgumentError(f'Invalid seed {seed}, should in [0, {Define.maxSeed}]', ModuleErrorCode,
                                       FileErrorCode, 2)
 
-    matrixTypeValue = None  # type: Optional[MatrixType]
+    matrixTypeValue: Optional[MatrixType] = None
     if matrixType == 'dense':
         matrixTypeValue = MatrixType.Dense
     
     else:
         raise Error.ArgumentError(
             f'Invalid MatrixType {matrixTypeValue}', ModuleErrorCode, FileErrorCode, 2)
 
-    algorithmValue = None  # type: Optional[Algorithm]
+    algorithmValue: Optional[Algorithm] = None
     if algorithm == 'matmul':
         algorithmValue = Algorithm.Matmul
     elif algorithm == 'einsum':
         algorithmValue = Algorithm.Einsum
     else:
         raise Error.ArgumentError(
             f'Invalid Algorithm {algorithmValue}', ModuleErrorCode, FileErrorCode, 4)
 
-    measureMethodValue = None  # type: Optional[MeasureMethod]
+    measureMethodValue: Optional[MeasureMethod] = None
     if measureMethod == 'probability':
         measureMethodValue = MeasureMethod.Probability
     elif measureMethod == 'output_probability':
         measureMethodValue = MeasureMethod.OutputProbability
     elif measureMethod == 'output_state':
         measureMethodValue = MeasureMethod.OutputState
     elif measureMethod == 'accumulation':
```

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py` & `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/Transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if matrixType == MatrixType.Dense and algorithm == Algorithm.Matmul:
             self.proc = self._transferStateDenseMatmul
         elif matrixType == MatrixType.Dense and algorithm == Algorithm.Einsum:
             self.proc = self._transferStateDenseEinsum
         
 
     def __call__(self, state: Union[numpy.ndarray, 'COO'], gate_matrix: Union[numpy.ndarray, 'COO'], bits: List[int]) -> \
-    Union[numpy.ndarray, 'COO']:
+            Union[numpy.ndarray, 'COO']:
         """
         :param state:
         :param gate_matrix:
         :param bits:
         :return:
         """
```

### Comparing `qcompute-3.2.1/QCompute/OpenSimulator/local_baidu_sim2/__init__.py` & `qcompute-3.3.0/QCompute/OpenSimulator/local_baidu_sim2/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/BatchID.py` & `qcompute-3.3.0/QCompute/QPlatform/BatchID.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/CircuitTools.py` & `qcompute-3.3.0/QCompute/QPlatform/CircuitTools.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Condition/__init__.py` & `qcompute-3.3.0/QCompute/QPlatform/Condition/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Error.py` & `qcompute-3.3.0/QCompute/QPlatform/Error.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/InteractiveModule.py` & `qcompute-3.3.0/QCompute/QPlatform/InteractiveModule.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 _AerSimulatorModuleList = [
     [UnrollProcedureModule, CompositeGateModule, UnrollCircuitModule],
     [InverseCircuitModule, ReverseCircuitModule]
 ]
 
 BackendModuleDict = {
     BackendName.LocalBaiduSim2: _SimulatorModuleList,
+    BackendName.LocalCuQuantum: _SimulatorModuleList,
     
     BackendName.CloudBaiduSim2Water: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Earth: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Thunder: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Heaven: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Wind: _SimulatorModuleList,
     BackendName.CloudBaiduSim2Lake: _SimulatorModuleList,
@@ -84,27 +85,27 @@
 
     def __init__(self, env: QEnv):
         self.env = env
         self.circuitToDrawTerminal = CircuitToDrawConsole()
         self.originProgram = PBProgram()
         self.originProgram.sdkVersion = Define.sdkVersion
         QEnvToProtobuf(self.originProgram, env)
-        self.backendName = env.backendName  # type: BackendName
+        self.backendName: BackendName = env.backendName
         self.moduleSetting = BackendModuleDict.get(self.backendName)
 
         if self.moduleSetting is _SimulatorModuleList and len(env.noiseDefineMap) > 0:
             self.moduleSetting = _SimulatorWithNoiseModuleList
 
         if self.moduleSetting:
-            self.moduleDict = {}  # type: Dict[str, Type[ModuleImplement]]
-            self.usingModuleList = []  # type: List[ModuleImplement]
+            self.moduleDict: Dict[str, Type[ModuleImplement]] = {}
+            self.usingModuleList: List[ModuleImplement] = []
             self.necessaryModuleList = self.moduleSetting[0]
             self.optionalModuleList = self.moduleSetting[1]
-            self.necessaryModuleNameList = []  # type: List[str]
-            self.optionalModuleNameList = []  # type: List[str]
+            self.necessaryModuleNameList: List[str] = []
+            self.optionalModuleNameList: List[str] = []
             for module in self.necessaryModuleList:
                 self.necessaryModuleNameList.append(module.__name__)
                 self.moduleDict[module.__name__] = module
             for module in self.optionalModuleList:
                 self.optionalModuleNameList.append(module.__name__)
                 self.moduleDict[module.__name__] = module
         else:
@@ -130,35 +131,35 @@
                 arguments = cmdList[1:] if len(cmdList) >= 2 else None
                 self.do(verb, arguments)
             except Exception as ex:
                 print(ex)
 
     def refurbishStatus(self):
         usingModuleList = filterModule(self.backendName, self.usingModuleList)
-        usingModuleNameList = []  # type: List[str]
-        reorderUsingModuleList = []  # type: List[ModuleImplement]
+        usingModuleNameList: List[str] = []
+        reorderUsingModuleList: List[ModuleImplement] = []
         for module in usingModuleList:
             if module in self.usingModuleList:
                 usingModuleNameList.append(module.__class__.__name__)
                 reorderUsingModuleList.append(module)
         self.usingModuleList = reorderUsingModuleList
 
-        canBeUsedModuleNameList = []  # type: List[str]
+        canBeUsedModuleNameList: List[str] = []
         for moduleName in self.optionalModuleNameList:
             if moduleName not in usingModuleNameList:
                 canBeUsedModuleNameList.append(moduleName)
         for moduleName in self.necessaryModuleNameList:
             if moduleName not in usingModuleNameList:
                 canBeUsedModuleNameList.append(moduleName)
         print(f'Modules can be used: {self._markModuleNameList(canBeUsedModuleNameList)}')
         usingModuleListFormArrow = self._markModuleNameList(usingModuleNameList).replace(',', ' ->')
         print(f'Modules used by order: {usingModuleListFormArrow}')
 
     def _markModuleNameList(self, moduleNameList: List[str]) -> str:
-        nameList = []  # type: List[str]
+        nameList: List[str] = []
         for moduleName in moduleNameList:
             if moduleName in self.necessaryModuleNameList:
                 nameList.append('(*)' + moduleName)
             else:
                 nameList.append(moduleName)
         return json.dumps(nameList).replace('"', '')
 
@@ -251,14 +252,14 @@
 
         self.env.commit(shots)
 
     def _exit(self):
         sys.exit()
 
     def printModuleList(self, moduleList: List[str]) -> None:
-        nameList = []  # type: List[str]
+        nameList: List[str] = []
         for moduleName in moduleList:
             if moduleName in self.necessaryModuleNameList:
                 nameList.append('(*)' + moduleName)
             else:
                 nameList.append(moduleName)
         print('-> ' + ' -> '.join(nameList))
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/ProcedureParameterPool.py` & `qcompute-3.3.0/QCompute/QPlatform/ProcedureParameterPool.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Processor/ModuleFilter.py` & `qcompute-3.3.0/QCompute/QPlatform/Processor/ModuleFilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,35 +16,37 @@
 # limitations under the License.
 
 """
 Module Filter
 """
 from typing import List, Optional
 
-from QCompute.OpenModule.UnrollCircuitModule import UnrollCircuitModule
-from QCompute.OpenModule.CompressGateModule import CompressGateModule
-from QCompute.OpenModule.UnrollProcedureModule import UnrollProcedureModule
+from QCompute.Define import Settings
+from QCompute.OpenModule import ModuleImplement
 from QCompute.OpenModule.CompositeGateModule import CompositeGateModule
+from QCompute.OpenModule.CompressGateModule import CompressGateModule
 from QCompute.OpenModule.InverseCircuitModule import InverseCircuitModule
+from QCompute.OpenModule.UnrollCircuitModule import UnrollCircuitModule
 from QCompute.OpenModule.UnrollNoiseModule import UnrollNoiseModule
-from QCompute.OpenModule import ModuleImplement
+from QCompute.OpenModule.UnrollProcedureModule import UnrollProcedureModule
 from QCompute.QPlatform import BackendName, Error, ModuleErrorCode
-from QCompute.Define import Settings
+
 
 
 FileErrorCode = 15
 
 
 def filterModule(backendName: Optional['BackendName'], moduleList: List['ModuleImplement']) \
         -> List['ModuleImplement']:
     if backendName is None:
         return moduleList
 
     if backendName in [
         BackendName.LocalBaiduSim2,
+        BackendName.LocalCuQuantum,
         
         BackendName.CloudBaiduSim2Water,
         BackendName.CloudBaiduSim2Earth,
         BackendName.CloudBaiduSim2Thunder,
         BackendName.CloudBaiduSim2Heaven,
         BackendName.CloudBaiduSim2Wind,
         BackendName.CloudBaiduSim2Lake,
@@ -53,21 +55,21 @@
         return _filterSimulator(backendName, moduleList)
     
     else:
         return moduleList
 
 
 def _filterSimulator(backendName: BackendName, moduleList: List['ModuleImplement']) -> List['ModuleImplement']:
-    unrollNoiseModule = None  # type: Optional[UnrollNoiseModule]
-    unrollProcedureModule = None  # type: Optional[UnrollProcedureModule]
-    compositeGateModule = None  # type: Optional[CompositeGateModule]
-    inverseCircuitModule = None  # type: Optional[InverseCircuitModule]
-    unrollCircuitModule = None  # type: Optional[UnrollCircuitModule]
-    compressGateModule = None  # type: Optional[CompressGateModule]
-    ret = []  # type: List['ModuleImplement']
+    unrollNoiseModule: Optional[UnrollNoiseModule] = None
+    unrollProcedureModule: Optional[UnrollProcedureModule] = None
+    compositeGateModule: Optional[CompositeGateModule] = None
+    inverseCircuitModule: Optional[InverseCircuitModule] = None
+    unrollCircuitModule: Optional[UnrollCircuitModule] = None
+    compressGateModule: Optional[CompressGateModule] = None
+    ret: List['ModuleImplement'] = []
     for module in moduleList:
         
         if module.__class__.__name__ == 'UnrollNoiseModule':
             unrollNoiseModule = module
         elif module.__class__.__name__ == 'UnrollProcedureModule':
             unrollProcedureModule = module
         elif module.__class__.__name__ == 'CompositeGateModule':
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Processor/PostProcessor.py` & `qcompute-3.3.0/QCompute/QPlatform/Processor/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Processor/PreProcess.py` & `qcompute-3.3.0/QCompute/QPlatform/Processor/PreProcess.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Processor/__init__.py` & `qcompute-3.3.0/QCompute/QPlatform/Processor/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QEnv.py` & `qcompute-3.3.0/QCompute/QPlatform/QEnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Quantum Environment
 """
+import copy
 import json
 import os
 import tempfile
 from copy import deepcopy
 from pathlib import Path
 from typing import Set, List, Dict, TYPE_CHECKING, Union, Optional, Tuple, Any
 
 from QCompute import Define, UnrollProcedureModule
 from QCompute.Define import Settings
 from QCompute.Define.Utils import loadPythonModule, clearOutputDir
 from QCompute.OpenConvertor.CircuitToDrawConsole import CircuitToDrawConsole
 from QCompute.OpenModule import ModuleImplement
 from QCompute.OpenModule.UnrollNoiseModule import UnrollNoiseModule
-from QCompute.OpenSimulator import QResult
+from QCompute.OpenSimulator import QResult, QImplement
 from QCompute.QPlatform import Error, ModuleErrorCode, BackendName, getBackendFromName
 from QCompute.QPlatform.CircuitTools import QEnvToProtobuf
 from QCompute.QPlatform.InteractiveModule import InteractiveModule
 from QCompute.QPlatform.ProcedureParameterPool import ProcedureParameterPool
 from QCompute.QPlatform.Processor.ModuleFilter import filterModule, printModuleListDescription
 from QCompute.QPlatform.Processor.PostProcessor import formatMeasure
 from QCompute.QPlatform.QNoise import QNoise, QNoiseDefine
@@ -72,42 +73,48 @@
     The module function inserts the processing module to the end of module list.
     """
 
     def __init__(self) -> None:
         self.Q = QRegPool(self)
         self.Parameter = ProcedureParameterPool()
 
-        self.measuredQRegSet = set()  # type: Set[int]
-        self.measuredCRegSet = set()  # type: Set[int]
-        self.circuit = []  # type: List['CircuitLine']
-        self.procedureMap = {}  # type: Dict[str, 'QProcedure']
-        self.program = None  # type: Optional['PBProgram']
-
-        self.backendName = None  # type: Optional[BackendName]
-        self.backendArgument = None  # type: Optional[List]
-        self.shots = 0  # type: int
+        self.measuredQRegSet: Set[int] = set()
+        self.measuredCRegSet: Set[int] = set()
+        self.circuit: List['CircuitLine'] = []
+        self.procedureMap: Dict[str, 'QProcedure'] = {}
+        self.program: Optional['PBProgram'] = None
+
+        self.backendName: Optional[BackendName] = None
+        self.backendArgument: Optional[List] = None
+        self.shots = 0
 
-        self.usingModuleList = []  # type: List['ModuleImplement']
-        self.usedServerModuleList = []  # type: List[Tuple[str, Dict]]
+        self.usingModuleList: List['ModuleImplement'] = []
+        self.usedServerModuleList: List[Tuple[str, Dict]] = []
 
-        self.noiseDefineMap = {}  # type: Dict[str, List[QNoiseDefine]]
+        self.noiseDefineMap: Dict[str, List[QNoiseDefine]] = {}
 
     def backend(self, backendName: Union['BackendName', str], *backendArgument: Any) -> None:
         """
         Set backend.
         """
         if type(backendName) is str:
             self.backendName = getBackendFromName(backendName)
         else:
             self.backendName = backendName
         self.backendArgument = list(backendArgument)
 
     def convertToProcedure(self, name: str, env: 'QEnv') -> 'QProcedure':
         if name in env.procedureMap:
             raise Error.ArgumentError(f'Duplicate procedure name: {name}!', ModuleErrorCode, FileErrorCode, 1)
+
+        if len(self.procedureMap) > 0:
+            for subName, subProc in self.procedureMap.items():
+                if subName not in env.procedureMap:
+                    env.procedureMap[subName] = subProc
+
         procedure = QProcedure(name, self.Q, self.Parameter, self.circuit)
         env.procedureMap[name] = procedure
         destoryObject(self)
         return procedure
 
     def inverseProcedure(self, name: str) -> Tuple['QProcedure', str]:
         procedure = self.procedureMap.get(name)
@@ -126,15 +133,15 @@
         inversedProcedure = deepcopy(procedure)
         inversedProcedure.name = inversedProcedureName
         self.procedureMap[inversedProcedureName] = inversedProcedure
         for index, circuitLine in enumerate(reversed(procedure.circuit)):
             newLine = deepcopy(circuitLine)
             if isinstance(newLine.data, QProcedureOP):
                 data, name = self.inverseProcedure(circuitLine.data.name)
-                op = deepcopy(circuitLine.data)  # type: QProcedureOP
+                op: QProcedureOP = deepcopy(circuitLine.data)
                 op.procedureData = data
                 op.name = name
                 newLine.data = op
             else:
                 newLine.data = circuitLine.data.getInversed()
             inversedProcedure.circuit[index] = newLine
         return inversedProcedure, inversedProcedureName
@@ -156,43 +163,43 @@
         reversedProcedure = deepcopy(procedure)
         reversedProcedure.name = reversedProcedureName
         self.procedureMap[reversedProcedureName] = reversedProcedure
         for index, circuitLine in enumerate(reversed(procedure.circuit)):
             newLine = deepcopy(circuitLine)
             if isinstance(newLine.data, QProcedureOP):
                 data, name = self.reverseProcedure(circuitLine.data.name)
-                op = deepcopy(circuitLine.data)  # type: QProcedureOP
+                op: QProcedureOP = deepcopy(circuitLine.data)
                 op.procedureData = data
                 op.name = name
                 newLine.data = op
             reversedProcedure.circuit[index] = newLine
         return reversedProcedure, reversedProcedureName
 
     def inverseCircuit(self) -> 'QEnv':
         inversedEnv = deepcopy(self)
         for index, circuitLine in enumerate(reversed(self.circuit)):
             newLine = deepcopy(circuitLine)
             if isinstance(newLine.data, QProcedureOP):
                 data, name = inversedEnv.inverseProcedure(circuitLine.data.name)
-                op = deepcopy(circuitLine.data)  # type: QProcedureOP
+                op: QProcedureOP = deepcopy(circuitLine.data)
                 op.procedureData = data
                 op.name = name
                 newLine.data = op
             else:
                 newLine.data = circuitLine.data.getInversed()
             inversedEnv.circuit[index] = newLine
         return inversedEnv
 
     def reverseCircuit(self) -> 'QEnv':
         reversedEnv = deepcopy(self)
         for index, circuitLine in enumerate(reversed(self.circuit)):
             newLine = deepcopy(circuitLine)
             if isinstance(newLine.data, QProcedureOP):
                 data, name = self.reverseProcedure(circuitLine.data.name)
-                op = deepcopy(circuitLine.data)  # type: QProcedureOP
+                op: QProcedureOP = deepcopy(circuitLine.data)
                 op.procedureData = data
                 op.name = name
                 newLine.data = op
             reversedEnv.circuit[index] = newLine
         return reversedEnv
 
     def controlProcedure(self, name: str, cuFirst: bool = False) -> Tuple['QProcedure', str]:
@@ -208,15 +215,15 @@
         controlledProcedure = deepcopy(procedure)
         controlledProcedure.name = controlledProcedureName
         controlQRegIndex = max(controlledProcedure.Q.registerMap.keys()) + 1
         controlQReg = controlledProcedure.Q[controlQRegIndex]  # need to create QRegStorage
         controlledProcedure.circuit.clear()
         self.procedureMap[controlledProcedureName] = controlledProcedure
         for circuitLine in procedure.circuit:
-            newCircuitLineList = getControlledCircuit(circuitLine, controlQRegIndex, cuFirst)
+            newCircuitLineList = getControlledCircuit(self, circuitLine, controlQRegIndex, cuFirst)
             controlledProcedure.circuit.extend(newCircuitLineList)
         return controlledProcedure, controlledProcedureName
 
     def publish(self, applyModule=True) -> List['ModuleImplement']:
         """
         To protobuf.
         """
@@ -286,15 +293,15 @@
         {status: 'error', reason: ''}
 
         {status: 'failed', reason: ''}
         """
 
         self.shots = shots
 
-        ret = None  # type: Dict[str, Union[str, Dict[str, int]]]
+        ret: Dict[str, Union[str, Dict[str, int]]] = None
         if self.backendName.value.startswith('local_'):
             if len(self.noiseDefineMap) > 0:
                 self.usingModuleList.clear()
                 self.module(UnrollProcedureModule())
                 self.module(UnrollNoiseModule())
             usedModuleList = self.publish()  # circuit in Protobuf format
             moduleList = [{
@@ -319,15 +326,15 @@
                 'arguments': module.arguments
             } for module in usedModuleList]
             ret = self._serviceCommit(fetchMeasure, moduleList)
         else:
             raise Error.ArgumentError(f"Invalid backendName => {self.backendName.value}", ModuleErrorCode,
                                       FileErrorCode, 5)
         if Settings.outputInfo and 'moduleList' in ret:
-            moduleList = [moduleSetting['module'] for moduleSetting in ret['moduleList']]  # type: List[str]
+            moduleList: List[str] = [moduleSetting['module'] for moduleSetting in ret['moduleList']]
             interactiveModule = InteractiveModule(self)
             print('Modules called sequentially')
             interactiveModule.printModuleList(moduleList)
             printModuleListDescription(moduleList)
 
         if Settings.autoClearOutputDirAfterFetchMeasure:
             clearOutputDir()
@@ -351,15 +358,15 @@
             module = loadPythonModule(f'QCompute.Simulator.{self.backendName.value}')
         if module is None:
             raise Error.ArgumentError(f"Invalid local backend => {self.backendName.value}!", ModuleErrorCode,
                                       FileErrorCode, 7)
         backendClass = getattr(module, 'Backend')
 
         # configure the parameters
-        backend = backendClass()  # type: 'QImplement'
+        backend: QImplement = backendClass()
         backend.program = self.program
         backend.shots = self.shots
         backend.backendArgument = self.backendArgument
         # execution
         backend.commit()
 
         # wrap taskResult
@@ -431,15 +438,15 @@
         """
         Cloud Commitment
 
         :return: task result
         """
 
         # the sequential bytes of the circuit which is already in PB
-        programBuf = self.program.SerializeToString()  # type: bytes
+        programBuf: bytes = self.program.SerializeToString()
 
         if not Settings.cloudTaskDoNotWriteFile:
             circuitPackageFd, circuitPackageFn = tempfile.mkstemp(prefix="circuit.", suffix=".pb",
                                                                   dir=Define.outputDirPath)
             with os.fdopen(circuitPackageFd, "wb") as file:
                 file.write(programBuf)
             if Settings.outputInfo:
@@ -483,15 +490,15 @@
         #     module = loadPythonModule(f'QCompute.Service.{self.backendName.value}')
         if module is None:
             raise Error.ArgumentError(f"Invalid service backend => {self.backendName.value}!", ModuleErrorCode,
                                       FileErrorCode, 8)
         backendClass = getattr(module, 'Backend')
 
         # configure the parameters
-        backend = backendClass()  # type: 'QImplement'
+        backend: QImplement = backendClass()
         backend.program = self.program
         backend.shots = self.shots
         backend.backendArgument = self.backendArgument
         # execution
         backend.commit()
 
         taskResult = {'status': 'success'}
@@ -549,7 +556,56 @@
                                               ModuleErrorCode, FileErrorCode, 10)
             noiseDefine = QNoiseDefine(noiseList, qRegList, positionList)
             defineList = self.noiseDefineMap.get(gateName)
             if defineList is None:
                 defineList = []
                 self.noiseDefineMap[gateName] = defineList
             defineList.append(noiseDefine)
+
+    def join(self, env: 'QEnv', startQRegIndex: int = 0) -> None:
+        """
+        Join quantum environment
+
+        :param env: a target quantum environment, which is joined in the current environment.
+        :param startQRegIndex: a index of QRegister is used to indicate which qubit the connection starts from.
+        """
+
+        if len(env.noiseDefineMap) > 0:
+            raise Error.ArgumentError(f"Unsupported noise in QEnv.join and concatEnv!",
+                                      ModuleErrorCode, FileErrorCode, 11)
+        env = copy.deepcopy(env)
+        nameMap: Dict[str, str] = {}
+        for procedureName, procedure in env.procedureMap.items():
+            newProcedureName = procedureName + '_joined'
+            num = 0
+            while newProcedureName + str(num) in self.procedureMap:
+                num += 1
+            nameMap[procedureName] = newProcedureName + str(num)
+        for procedureName, procedure in env.procedureMap.items():
+            for circuitLine in procedure.circuit:
+                if isinstance(circuitLine.data, QProcedureOP):
+                    circuitLine.data.name = nameMap[circuitLine.data.name]
+                    circuitLine.data.procedureData.name = circuitLine.data.name
+            self.procedureMap[nameMap[procedureName]] = procedure
+        for circuitLine in env.circuit:
+            self.circuit.append(circuitLine)
+            for index, qreg in enumerate(circuitLine.qRegList):
+                qreg += startQRegIndex
+                circuitLine.qRegList[index] = qreg
+                self.Q(qreg)
+            if isinstance(circuitLine.data, QProcedureOP):
+                circuitLine.data.name = nameMap[circuitLine.data.name]
+                circuitLine.data.procedureData.name = circuitLine.data.name
+
+
+def concatQEnv(*envList: QEnv) -> QEnv:
+    """
+    Concatenate quantum environments
+
+    :param envList: a list of quantum environments
+    :return: a new quantum environment with all environments concatenated
+    """
+
+    ret = copy.deepcopy(envList[0])
+    for env in envList[1:]:
+        ret.join(env)
+    return ret
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QEnvOperation.py` & `qcompute-3.3.0/QCompute/QPlatform/QEnvOperation.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/AmplitudeDamping.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/AmplitudeDamping.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 class AmplitudeDamping(QNoise):
     r"""
     Amplitude damping class.
 
     The Kraus operators of such noise are as follows:
 
-    :math:`E_0 = \begin{bmatrix} 1.0 & 0.0 \\ 0.0 & \sqrt{1 - p} \end{bmatrix}`
+    :math:`E_0 = \begin{bmatrix} 1 & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix}`
 
-    :math:`E_1 = \begin{bmatrix} 0.0 &  \sqrt{p}\\ 0.0 & 0.0 \end{bmatrix}`
+    :math:`E_1 = \begin{bmatrix} 0 &  \sqrt{p}\\ 0 & 0 \end{bmatrix}`
 
     Here, :math:`p` is the strength of noise.
     """
 
     def __init__(self, probability: float) -> None:
         super().__init__(1)
         self.probability = probability
@@ -59,15 +59,15 @@
         """
 
         if np.isclose(0.0, self.probability):
             return 'mixed_unitary_noise'
         else:
             return 'non_mixed_unitary_noise'
 
-    def calc_batched_noise_rng(self, num: int) -> List[float]:
+    def calc_batched_noise_rng(self, num: int) -> List[int]:
         """
         Generate a batch of sampled random numbers for mixed-unitary noise.
 
         :param num: int, the number of sampled random numbers
         :return: List[int], a set of random numbers
         """
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/BitFlip.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/BitFlip.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/BitPhaseFlip.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/BitPhaseFlip.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/CustomizedNoise.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/CustomizedNoise.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from QCompute.OpenSimulator.local_baidu_sim2.Transfer import TransferProcessor
 
 
 class CustomizedNoise(QNoise):
     """
     Customized noise class.
 
-    Generate a noise defined by customers which is described by Kraus operator summation representation.
+    Generate a noise defined by customers which is described by Kraus operator-sum representation.
 
     Available for Kraus operators of numpy formation.
     """
 
     def __init__(self, krauses: List[np.ndarray]) -> None:
         bits = int(math.log2(math.sqrt(krauses[0].size)) + 0.5)
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/Depolarizing.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/Depolarizing.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 
 class Depolarizing(QNoise):
     r"""
     Depolarizing noise class.
 
     The Kraus operators of one qubit depolarizing noise are as follows:
 
-    :math:`E_0 = \sqrt{1 - 3.0  p / 4.0} \ ID`
+    :math:`E_0 = \sqrt{1 - 3 p / 4} \ ID`
 
-    :math:`E_1 = \sqrt{p / 4.0} \ X`
+    :math:`E_1 = \sqrt{p / 4} \ X`
 
-    :math:`E_2 = \sqrt{p / 4.0} \ Y`
+    :math:`E_2 = \sqrt{p / 4} \ Y`
 
-    :math:`E_3 = \sqrt{p / 4.0} \ Z`
+    :math:`E_3 = \sqrt{p / 4} \ Z`
 
     Here, :math:`p` is the strength of noise.
 
     Example:
 
     Depolarizing(bits=2, probability=0.1)
     """
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/PauliNoise.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/PauliNoise.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/PhaseDamping.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseDamping.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 class PhaseDamping(QNoise):
     r"""
     Phase damping class.
 
     The Kraus operators of such noise are as follows:  
 
-    :math:`E_0 = \begin{bmatrix} 1.0 & 0.0 \\ 0.0 & \sqrt{1 - p} \end{bmatrix}`
+    :math:`E_0 = \begin{bmatrix} 1 & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix}`
 
-    :math:`E_1 = \begin{bmatrix} 0.0 & 0.0\\ 0.0 & \sqrt{p} \end{bmatrix}`  
+    :math:`E_1 = \begin{bmatrix} 0 & 0 \\ 0 & \sqrt{p} \end{bmatrix}`  
 
     Here, :math:`p` is the strength of noise.
 
     Phase damping noise is equivalent to a phase flip noise with probability as follows,
 
-    :math:`p_{pf} = (1 - \sqrt{1.0 - p}) / 2`
+    :math:`p_{pf} = (1 - \sqrt{1 - p}) / 2`
     """
 
     def __init__(self, probability: float) -> None:
         super().__init__(1)
         self.probability = (1 - np.sqrt(1.0 - probability)) / 2
 
         self.krauses = [sigma(0), sigma(3)]
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/PhaseFlip.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/PhaseFlip.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 class PhaseFlip(QNoise):
     r"""
     Phase flip class.
 
     The Kraus operators of such noise are as follows:
 
-    :math:`E_0 = \sqrt{1.0 - p} \ ID`
+    :math:`E_0 = \sqrt{1 - p} \ ID`
     
     :math:`E_1 = \sqrt{p} \ Z`
 
     Here, :math:`p` is the strength of noise.
     """
 
     def __init__(self, probability: float) -> None:
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/ResetNoise.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/ResetNoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 class ResetNoise(QNoise):
     r"""
     Reset noise class.
 
     The Kraus operators of such noise are as follows:
     
-    :math:`E_0 = \sqrt{1 - p_1 - p_2 - p_3} \ ID`
+    :math:`E_0 = \sqrt{1 - p_1 - p_2} \ ID`
 
-    :math:`E_1 = \begin{bmatrix} \sqrt{p_1} & 0.0 \\ 0.0 & 0.0 \end{bmatrix}`
+    :math:`E_1 = \begin{bmatrix} \sqrt{p_1} & 0 \\ 0 & 0 \end{bmatrix}`
 
-    :math:`E_2 = \begin{bmatrix} 0.0 & \sqrt{p_1} \\ 0.0 & 0.0 \end{bmatrix}`
+    :math:`E_2 = \begin{bmatrix} 0 & \sqrt{p_1} \\ 0 & 0 \end{bmatrix}`
 
-    :math:`E_3 = \begin{bmatrix} 0.0 & 0.0 \\ \sqrt{p_2} & 0.0 \end{bmatrix}`
+    :math:`E_3 = \begin{bmatrix} 0 & 0 \\ \sqrt{p_2} & 0 \end{bmatrix}`
 
-    :math:`E_4 = \begin{bmatrix} 0.0 & 0.0 \\ 0.0 & \sqrt{p_2} \end{bmatrix}`
+    :math:`E_4 = \begin{bmatrix} 0 & 0 \\ 0 & \sqrt{p_2} \end{bmatrix}`
 
     Here, :math:`p` is the strength of noise.
     """
 
     def __init__(self, probability1: float, probability2: float) -> None:
         super().__init__(1)
         self.probability1 = probability1
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/Utilities.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/Utilities.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QNoise/__init__.py` & `qcompute-3.3.0/QCompute/QPlatform/QNoise/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/Barrier.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/Barrier.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/CompositeGate.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/CompositeGate.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,19 +64,19 @@
                 raise Error.ArgumentError(f'Can not inverse argument id. angles id: {argument.index}!', ModuleErrorCode,
                                           FileErrorCode, 2)
 
         nAngles = len(self.argumentList)
         if nAngles == 0:
             pass
         elif nAngles == 1:
-            [theta] = self.argumentList  # type: List[float]
+            [theta] = self.argumentList
         elif nAngles == 2:
-            [theta, phi] = self.argumentList  # type: List[float]
+            [theta, phi] = self.argumentList
         elif nAngles == 3:
-            [theta, phi, lamda] = self.argumentList  # type: List[float]
+            [theta, phi, lamda] = self.argumentList
         else:
             raise Error.ArgumentError(f'Wrong angles count. angles value: {self.argumentList}!', ModuleErrorCode,
                                       FileErrorCode, 3)
 
         if self.name == 'MS':
             if nAngles == 0:
                 return CompositeGateOP('MS', 2, MSOpAllowArgumentCounts, [-math.pi / 2])
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/CustomizedGate.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/CustomizedGate.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/FixedGate.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/FixedGate.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/Measure.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/Measure.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/QProcedure.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/QProcedure.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/RotationGate.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/RotationGate.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,19 +137,19 @@
         for argument in self.argumentList:
             if isinstance(argument, ProcedureParameterStorage):
                 raise Error.ArgumentError(f'Can not inverse argument id. angles id: {argument.index}!', ModuleErrorCode,
                                           FileErrorCode, 2)
 
         nAngles = len(self.argumentList)
         if nAngles == 1:
-            [theta] = self.argumentList  # type: float
+            [theta] = self.argumentList
         elif nAngles == 2:
-            [theta, phi] = self.argumentList  # type: float
+            [theta, phi] = self.argumentList
         elif nAngles == 3:
-            [theta, phi, lamda] = self.argumentList  # type: float
+            [theta, phi, lamda] = self.argumentList
         else:
             raise Error.ArgumentError(f'Wrong angles count. angles value: {self.argumentList}!', ModuleErrorCode,
                                       FileErrorCode, 3)
 
         if self.name == 'RX':
             return RX(-theta)
         elif self.name == 'RY':
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QOperation/__init__.py` & `qcompute-3.3.0/QCompute/QPlatform/QOperation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         :param data: a Quanlse.QOperation.Operation instance,
                     the quantum gate to be applied
         :param qRegList: a list of qubit indices.
                     If `gate` is a single-qubit
                     gate, then `qubits` still be a List of the form `[i]`
         :param cRegList: a list of classical bit indices
         """
-        self.data: Operation = data
+        self.data = data
         self.qRegList: List[int] = qRegList
         self.cRegList: List[int] = cRegList
 
     def inverse(self) -> 'CircuitLine':
         """
         Return a `CircuitLine` instance whose `QOperation` data is the inverse of the origin one.
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QRegPool.py` & `qcompute-3.3.0/QCompute/QPlatform/QRegPool.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QStatus.py` & `qcompute-3.3.0/QCompute/QPlatform/QStatus.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QPlatform/QTask.py` & `qcompute-3.3.0/QCompute/QPlatform/QTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,27 @@
 # submit the file id to cloud service, and finally get the results.
 from QCompute.Define import Settings
 from QCompute.QPlatform import Error, ModuleErrorCode
 from QCompute.QPlatform.BatchID import BatchID
 
 FileErrorCode = 7
 
-_bosClient = None  # type: BceClientConfiguration
+_bosClient: BceClientConfiguration = None
 
 
 def _retryWhileNetworkError(func: Callable) -> Callable:
     """
     The decorator for retrying function when network failed
     """
 
     def _func(*args, **kwargs):
         retryCount = 0
         ret = None
         
-        lastError = None  # type: Exception
+        lastError: Exception = None
         while retryCount < Define.waitTaskRetryTimes:
             try:
                 ret = func(*args, **kwargs)
                 lastError = None
                 break
 
             except (Error.NetworkError, requests.RequestException) as e:
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/Utilities.py` & `qcompute-3.3.0/QCompute/QPlatform/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,18 +141,18 @@
     return functools.reduce(
         lambda result, index: numpy.kron(
             result, index), args, numpy.kron(
             AMatrix, BMatrix))
 
 
 def contract1_1(matrixParking: numpy.ndarray, matrixFloating: numpy.ndarray) -> numpy.ndarray:
-    """
+    r"""
     The first indicator of the gate is the output,
     and the latter indicator is the input,
-    just like writing matrix vector multiplication, U{ket0}
+    just like writing matrix vector multiplication, :math:`U |0\rangle`
     """
     if matrixFloating.shape != (2, 2):
         raise Error.ArgumentError("Floating gate not a 1-qubit gate", ModuleErrorCode, FileErrorCode, 3)
     if matrixParking.shape != (2, 2):
         raise Error.ArgumentError("Parking gate not a 1-qubit gate", ModuleErrorCode, FileErrorCode, 4)
     newArray = numpy.einsum('ab,bc->ac', matrixParking,
                             matrixFloating)  # v is a vector, A B is a matrix, we must count ABv, here we count AB
```

### Comparing `qcompute-3.2.1/QCompute/QPlatform/__init__.py` & `qcompute-3.3.0/QCompute/QPlatform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,27 @@
     env.backend(BackendName.LocalBaiduSim2, Sim2Argument.Dense_Matmul_Probability)
 
     or Added shots(must have space in string)
 
     env.backend(BackendName.LocalBaiduSim2, Sim2Argument.Dense_Matmul_Probability.value + ' -s 20210210')
     """
 
+    LocalCuQuantum = 'local_cuquantum'
+    """
+    Local CuQuantum
+    
+    This backend name (LocalCuQuantum) is only available >= v3.3.0
+    
+    Example: 
+    
+    env = QEnv()
+    
+    env.backend(BackendName.LocalCuQuantum)
+    """
+
     LocalBaiduSim2WithNoise = 'local_baidu_sim2'
     """
     Local Baidu Sim2 With Noise
     """
```

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/Complex_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/Complex_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/PlatformStruct_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/PlatformStruct_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/QNoise_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/QNoise_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/QObj_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/QObj_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/QOperation_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/QOperation_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/UniversalBlindQuantumComputing_pb2.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/Library/__init__.py` & `qcompute-3.3.0/QCompute/QProtobuf/Library/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/QProtobuf/__init__.py` & `qcompute-3.3.0/QCompute/QProtobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/Utilize/ControlledCircuit/__init__.py` & `qcompute-3.3.0/QCompute/Utilize/ControlledCircuit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Controlled Circuit
 """
+import copy
 from typing import List
 
 import numpy
 
-from QCompute.QPlatform import Error
+from QCompute.QPlatform import Error, QEnv
 from QCompute.QPlatform.QOperation import CircuitLine
 from QCompute.QPlatform.QOperation.FixedGate import CX, CY, CH, CCX, SDG, S, H, CSWAP, CZ
 from QCompute.QPlatform.QOperation.RotationGate import RotationGateOP, CU, CRX, CRY, CRZ, U
 from QCompute.Utilize import ModuleErrorCode
 
 FileErrorCode = 1
 
 
-def getControlledCircuit(circuitLine: CircuitLine, controlQRegIndex: int, cuFirst: bool) \
+def getControlledCircuit(env: QEnv, circuitLine: CircuitLine, controlQRegIndex: int, cuFirst: bool) \
         -> List[CircuitLine]:
     ret: List['CircuitLine'] = []
 
     op = circuitLine.data
 
     if op.bits == 1:
         q0 = circuitLine.qRegList[0]
@@ -45,26 +46,28 @@
         q1 = circuitLine.qRegList[1]
         q2 = controlQRegIndex
     elif op.bits == 3:
         q0 = circuitLine.qRegList[0]
         q1 = circuitLine.qRegList[1]
         q2 = circuitLine.qRegList[2]
         q3 = controlQRegIndex
+    elif op.__class__.__name__ == 'QProcedureOP':
+        pass
     else:
         raise Error.ArgumentError(f'Wrong bits count. bits value: {op.bits}!', ModuleErrorCode,
                                   FileErrorCode, 1)
 
     if isinstance(op, RotationGateOP):
         nAngles = len(op.argumentList)
         if nAngles == 1:
-            [theta] = op.argumentList  # type: float
+            [theta] = op.argumentList
         elif nAngles == 2:
-            [theta, phi] = op.argumentList  # type: float
+            [theta, phi] = op.argumentList
         elif nAngles == 3:
-            [theta, phi, lamda] = op.argumentList  # type: float
+            [theta, phi, lamda] = op.argumentList
         else:
             raise Error.ArgumentError(f'Wrong angles count. angles value: {op.argumentList}!', ModuleErrorCode,
                                       FileErrorCode, 2)
 
     # 1-qubit, FixedGate
     if op.name == 'ID':
         newCircuitLine = CircuitLine()
@@ -482,14 +485,24 @@
         ret.append(newCircuitLine)
 
         newCircuitLine = CircuitLine()
         newCircuitLine.data = CRZ(-numpy.pi / 2)
         newCircuitLine.qRegList = [q1, q2]
         ret.append(newCircuitLine)
 
+    elif op.__class__.__name__ == 'QProcedureOP':
+        newProcedure, newProcedureName = env.controlProcedure(op.name, cuFirst)
+        env.procedureMap[newProcedureName] = newProcedure
+
+        newCircuitLine = CircuitLine()
+        newCircuitLine.data = newProcedure(*op.argumentList)
+        newCircuitLine.qRegList = copy.copy(circuitLine.qRegList)
+        newCircuitLine.qRegList.append(controlQRegIndex)
+        ret.append(newCircuitLine)
+
     # Unsupported
     else:
         raise Error.ArgumentError(
             f"{op.__class__.__name__} {op.name} can't be controlled in procedure!",
             ModuleErrorCode, FileErrorCode, 3)
 
     return ret
```

### Comparing `qcompute-3.2.1/QCompute/Utilize/__init__.py` & `qcompute-3.3.0/QCompute/Utilize/__init__.py`

 * *Files identical despite different names*

### Comparing `qcompute-3.2.1/QCompute/__init__.py` & `qcompute-3.3.0/QCompute/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,47 +16,45 @@
 # limitations under the License.
 
 """
 Export the entire directory as a library
 """
 
 from QCompute import Define
-
 from QCompute.Define import (
     sdkVersion,
     outputDirPath,
 )
-
 from QCompute.Define.Utils import matchSdkVersion
-
+from QCompute.Module.MappingToBaiduQPUQianModule import MappingToBaiduQPUQianModule
+from QCompute.Module.MappingToIoPCASModule import MappingToIoPCASModule
+from QCompute.Module.MappingToIonAPMModule import MappingToIonAPMModule
+from QCompute.Module.UnrollCircuitToBaiduQPUQianModule import UnrollCircuitToBaiduQPUQianModule
+from QCompute.Module.UnrollCircuitToIoPCASModule import UnrollCircuitToIoPCASModule
+from QCompute.Module.UnrollCircuitToIonAPMModule import UnrollCircuitToIonAPMModule
 from QCompute.OpenModule.CompositeGateModule import CompositeGateModule
 from QCompute.OpenModule.CompressGateModule import CompressGateModule
 from QCompute.OpenModule.InverseCircuitModule import InverseCircuitModule
 from QCompute.OpenModule.ReverseCircuitModule import ReverseCircuitModule
 from QCompute.OpenModule.UnrollCircuitModule import UnrollCircuitModule
 from QCompute.OpenModule.UnrollProcedureModule import UnrollProcedureModule
-from QCompute.Module.MappingToBaiduQPUQianModule import MappingToBaiduQPUQianModule
-from QCompute.Module.UnrollCircuitToBaiduQPUQianModule import UnrollCircuitToBaiduQPUQianModule
-from QCompute.Module.MappingToIoPCASModule import MappingToIoPCASModule
-from QCompute.Module.UnrollCircuitToIoPCASModule import UnrollCircuitToIoPCASModule
-from QCompute.Module.MappingToIonAPMModule import MappingToIonAPMModule
-from QCompute.Module.UnrollCircuitToIonAPMModule import UnrollCircuitToIonAPMModule
+
 
 
 from QCompute.OpenSimulator import (
     QResult,
 )
 
 from QCompute.QPlatform import (
     QTask,
     BackendName,
     Sim2Argument,
     ServerModule,
 )
-from QCompute.QPlatform.QEnv import QEnv
+from QCompute.QPlatform.QEnv import QEnv, concatQEnv
 from QCompute.QPlatform.QEnvOperation import QEnvOperation
 from QCompute.QPlatform.InteractiveModule import InteractiveModule
 
 from QCompute.QPlatform.QOperation.Barrier import Barrier, BarrierOP
 from QCompute.QPlatform.QOperation.CompositeGate import MS, CK
 from QCompute.QPlatform.QOperation.CustomizedGate import CustomizedGateOP
 from QCompute.QPlatform.QOperation.FixedGate import (
@@ -123,18 +121,20 @@
 from QCompute.OpenConvertor.CircuitToXanaduSF import (
     CircuitToXanaduSF, TwoQubitsGate
 )
 from QCompute.QPlatform import QStatus
 from QCompute.QPlatform import Utilities
 from QCompute.Calibration import CalibrationUpdate, CalibrationReadData
 
-
+if True:  # prevent scrambling
+    
+    pass
 
 from QCompute.QPlatform.QNoise.AmplitudeDamping import AmplitudeDamping
 from QCompute.QPlatform.QNoise.BitFlip import BitFlip
 from QCompute.QPlatform.QNoise.BitPhaseFlip import BitPhaseFlip
 from QCompute.QPlatform.QNoise.CustomizedNoise import CustomizedNoise
 from QCompute.QPlatform.QNoise.Depolarizing import Depolarizing
 from QCompute.QPlatform.QNoise.PauliNoise import PauliNoise
 from QCompute.QPlatform.QNoise.PhaseDamping import PhaseDamping
 from QCompute.QPlatform.QNoise.PhaseFlip import PhaseFlip
-from QCompute.QPlatform.QNoise.ResetNoise import ResetNoise
+from QCompute.QPlatform.QNoise.ResetNoise import ResetNoise
```

### Comparing `qcompute-3.2.1/README.md` & `qcompute-3.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # QCompute
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2F%E9%87%8F%E6%98%93%E4%BC%8F%E5%9B%BE%E6%A0%87.png)
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.2.1-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -63,14 +63,18 @@
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2Fqrcode.png)
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
+## Integrations
+
+The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/baidu/QCompute/blob/master/LICENSE) file for details.
```

### Comparing `qcompute-3.2.1/qcompute.egg-info/PKG-INFO` & `qcompute-3.3.0/qcompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qcompute
-Version: 3.2.1
+Version: 3.3.0
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
 
-[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.2.1-blue)
+[![](https://img.shields.io/badge/license-Apache%202.0-green)](./LICENSE) ![](https://img.shields.io/badge/build-passing-green) ![](https://img.shields.io/badge/Python-3.8--3.10-blue) ![](https://img.shields.io/badge/release-v3.3.0-blue)
 
 Quantum Leaf (量易伏) is a Cloud-Native quantum computing platform developed by the Institute for Quantum Computing, Baidu. It is used for programming, simulating and executing quantum computers, aiming at providing the quantum programming environment for Quantum infrastructure as a Service (QaaS).
 
 QCompute is a Python-based open-source SDK. It provides a full-stack programming experience for advanced users via the features of hybrid quantum programming language and a high-performance simulator. Users can use the already-built objects and modules of quantum programming environment, pass parameters to build and execute the quantum circuits on the local simulator or the cloud simulator/hardware.
 
 QCompute provides services for creating and analyzing quantum circuits, and calling quantum backend. The architecture of Quantum Leaf including QCompute is shown in the figure below.
 
@@ -75,14 +75,18 @@
 
 ![](https://release-data.cdn.bcebos.com/github-qleaf%2Fqrcode.png)
 
 ## Maintainers & Authors
 
 Institute for Quantum Computing, Baidu.
 
+## Integrations
+
+The new backend "local_cuquantum" is constructed under cuQuantum SDK (https://developer.nvidia.com/cuquantum-sdk)  and is supported by NVIDIA.
+
 ## Changelog
 
 The changelog of this project can be found in [CHANGELOG.md](https://github.com/baidu/QCompute/blob/master/CHANGELOG.md).
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/baidu/QCompute/blob/master/LICENSE) file for details.
```

### Comparing `qcompute-3.2.1/qcompute.egg-info/SOURCES.txt` & `qcompute-3.3.0/qcompute.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 QCompute/OpenService/service_ubqc/client/utils.py
 QCompute/OpenSimulator/__init__.py
 QCompute/OpenSimulator/local_baidu_sim2/InitState.py
 QCompute/OpenSimulator/local_baidu_sim2/Measure.py
 QCompute/OpenSimulator/local_baidu_sim2/Simulator.py
 QCompute/OpenSimulator/local_baidu_sim2/Transfer.py
 QCompute/OpenSimulator/local_baidu_sim2/__init__.py
+QCompute/OpenSimulator/local_cuquantum/CheckEnv.py
+QCompute/OpenSimulator/local_cuquantum/DistEinsum.py
+QCompute/OpenSimulator/local_cuquantum/Kernel.py
+QCompute/OpenSimulator/local_cuquantum/Simulator.py
+QCompute/OpenSimulator/local_cuquantum/__init__.py
 QCompute/QPlatform/BatchID.py
 QCompute/QPlatform/CircuitTools.py
 QCompute/QPlatform/Error.py
 QCompute/QPlatform/InteractiveModule.py
 QCompute/QPlatform/ProcedureParameterPool.py
 QCompute/QPlatform/QEnv.py
 QCompute/QPlatform/QEnvOperation.py
```

### Comparing `qcompute-3.2.1/setup.py` & `qcompute-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pathlib import Path
 
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
-SDK_VERSION = '3.2.1'
+SDK_VERSION = '3.3.0'
 
 DESC = Path('./README.md').read_text(encoding='utf-8')
 
 setup(
     name='qcompute',
     version=SDK_VERSION,
     install_requires=[
```

