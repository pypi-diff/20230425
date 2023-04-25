# Comparing `tmp/qcodes_contrib_drivers-0.9.0.tar.gz` & `tmp/qcodes_contrib_drivers-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcodes_contrib_drivers-0.9.0.tar", last modified: Thu May 20 06:10:00 2021, max compression
+gzip compressed data, was "dist/qcodes_contrib_drivers-0.9.1.tar", last modified: Thu May 20 09:13:53 2021, max compression
```

## Comparing `qcodes_contrib_drivers-0.9.0.tar` & `qcodes_contrib_drivers-0.9.1.tar`

### file list

```diff
@@ -1,176 +1,177 @@
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/
--rw-r--r--   0 vsts      (1001) docker     (118)     1063 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (118)    18092 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/LICENSE_TEKTRONIX_AWG520_KEITHLEY_2700
--rw-r--r--   0 vsts      (1001) docker     (118)       65 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (118)      966 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/
--rw-r--r--   0 vsts      (1001) docker     (118)       93 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      497 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Advantech/
--rw-r--r--   0 vsts      (1001) docker     (118)    11372 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Advantech/PCIE_1751.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Advantech/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Agilent/
--rw-r--r--   0 vsts      (1001) docker     (118)     3865 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Agilent/Agilent_N9000A.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Agilent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/AimTTi/
--rw-r--r--   0 vsts      (1001) docker     (118)     2625 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/AimTTi/EL320P.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/AimTTi/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Andor/
--rw-r--r--   0 vsts      (1001) docker     (118)    18514 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Andor/DU401.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Andor/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/
--rw-r--r--   0 vsts      (1001) docker     (118)    23856 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC300.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7706 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC300sim.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20181 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/
--rw-r--r--   0 vsts      (1001) docker     (118)      667 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5594 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/interface.py
--rw-r--r--   0 vsts      (1001) docker     (118)    44064 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v3.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7615 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v4.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Aviosys/
--rw-r--r--   0 vsts      (1001) docker     (118)     3385 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Aviosys/IP_Power_9258S.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Aviosys/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Bilt/
--rw-r--r--   0 vsts      (1001) docker     (118)    15405 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Bilt/ITest.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Bilt/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/BlueFors/
--rw-r--r--   0 vsts      (1001) docker     (118)     8595 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/BlueFors/BlueFors.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/BlueFors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/CopperMountain/
--rw-r--r--   0 vsts      (1001) docker     (118)    21574 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/CopperMountain/M5180.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/CopperMountain/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryocon/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryocon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6638 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryocon/cryocon_26.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryogenic/
--rw-r--r--   0 vsts      (1001) docker     (118)    21863 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryogenic/CryogenicSMS120C.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryogenic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Gentec/
--rw-r--r--   0 vsts      (1001) docker     (118)     2119 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Gentec/Gentec_Maestro.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Gentec/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/
--rw-r--r--   0 vsts      (1001) docker     (118)     3099 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_E36313A.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9671 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_E8267D.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1330 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_J7211.py
--rw-r--r--   0 vsts      (1001) docker     (118)      626 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3201A.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2031 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3300A.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1504 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/M3202A.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/
--rw-r--r--   0 vsts      (1001) docker     (118)    43101 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18139 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG_Async.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29191 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_DIG.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16346 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_Module.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6234 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/memory_manager.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/
--rw-r--r--   0 vsts      (1001) docker     (118)     3967 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/Model_331.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18098 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/Model_625.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/
--rw-r--r--   0 vsts      (1001) docker     (118)     7571 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/DAQ.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2253 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_2597.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1477 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_5654.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9296 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/RFSG.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6389 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/Switch.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11449 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/dll_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2582 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/ni_dll_instrument.py
--rw-r--r--   0 vsts      (1001) docker     (118)      326 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/visa_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Newport/
--rw-r--r--   0 vsts      (1001) docker     (118)    13722 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Newport/AG_UC8.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Newport/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/
--rw-r--r--   0 vsts      (1001) docker     (118)     9780 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/ILM200.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28906 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/IPS120.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8296 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/Triton.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17771 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/kelvinox.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/
--rw-r--r--   0 vsts      (1001) docker     (118)     1755 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/D4.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5401 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/D5a.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2867 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/F1d.py
--rw-r--r--   0 vsts      (1001) docker     (118)    27765 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/IVVI.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2703 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/M2j.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3393 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/S5i.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/
--rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8041.py
--rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8042.py
--rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8043.py
--rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP2020.py
--rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP2030.py
--rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP4030.py
--rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP4040.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9498 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMR40.py
--rw-r--r--   0 vsts      (1001) docker     (118)   121277 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200A.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7792 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200Asim.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/
--rw-r--r--   0 vsts      (1001) docker     (118)     4185 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMC804x.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4846 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMP.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Shamrock/
--rw-r--r--   0 vsts      (1001) docker     (118)    12502 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Shamrock/SR750.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Shamrock/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/SingleQuantum/
--rw-r--r--   0 vsts      (1001) docker     (118)    15758 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/SingleQuantum/SingleQuantum.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/SingleQuantum/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/
--rw-r--r--   0 vsts      (1001) docker     (118)    56158 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/M4i.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5960 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/h2py.py
--rw-r--r--   0 vsts      (1001) docker     (118)    64337 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/regs.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1913 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/spcerr.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7543 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/pyspcm.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Standa/
--rw-r--r--   0 vsts      (1001) docker     (118)     7537 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Standa/Standa_10MWA168.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Standa/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/
--rw-r--r--   0 vsts      (1001) docker     (118)     9118 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/DG645.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15062 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/SIM928.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/
--rw-r--r--   0 vsts      (1001) docker     (118)    24674 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/AFG3000.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23016 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/AWG520.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2543 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2000_Scan.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12154 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2700.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18205 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6430.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6155 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6500.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/
--rw-r--r--   0 vsts      (1001) docker     (118)    15397 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/APT.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10488 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/K10CR1.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1711 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/MFF10x.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1661 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/PRM1Z8.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Vaunix/
--rw-r--r--   0 vsts      (1001) docker     (118)    11690 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Vaunix/LDA.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Vaunix/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/
--rw-r--r--   0 vsts      (1001) docker     (118)     9922 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/HF2LI.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14493 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/ZIHDAWG8.py
--rw-r--r--   0 vsts      (1001) docker     (118)       22 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    21098 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_Keysight_M3201A.py
--rw-r--r--   0 vsts      (1001) docker     (118)      763 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_Spectrum_M4i.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1921 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_m2j.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6445 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_ni_pxie_2597.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1431 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_rohdeschwarz_HMC804x.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10149 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_zihdawg8.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (118)      966 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)     7202 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-20 06:04:38.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (118)       14 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       23 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (118)     1604 2021-05-20 06:10:00.000000 qcodes_contrib_drivers-0.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (118)      138 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/setup.py
--rw-r--r--   0 vsts      (1001) docker     (118)    68611 2021-05-20 05:53:01.000000 qcodes_contrib_drivers-0.9.0/versioneer.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1063 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (118)    18092 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/LICENSE_TEKTRONIX_AWG520_KEITHLEY_2700
+-rw-r--r--   0 vsts      (1001) docker     (118)       65 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (118)     3154 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     1811 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/
+-rw-r--r--   0 vsts      (1001) docker     (118)       93 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      497 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Advantech/
+-rw-r--r--   0 vsts      (1001) docker     (118)    11372 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Advantech/PCIE_1751.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Advantech/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Agilent/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3865 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Agilent/Agilent_N9000A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Agilent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/AimTTi/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2625 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/AimTTi/EL320P.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/AimTTi/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Andor/
+-rw-r--r--   0 vsts      (1001) docker     (118)    18514 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Andor/DU401.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Andor/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/
+-rw-r--r--   0 vsts      (1001) docker     (118)    23856 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC300.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7706 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC300sim.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    20181 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/
+-rw-r--r--   0 vsts      (1001) docker     (118)      667 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5594 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    44064 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v3.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7615 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v4.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Aviosys/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3385 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Aviosys/IP_Power_9258S.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Aviosys/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Bilt/
+-rw-r--r--   0 vsts      (1001) docker     (118)    15405 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Bilt/ITest.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Bilt/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/BlueFors/
+-rw-r--r--   0 vsts      (1001) docker     (118)     8595 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/BlueFors/BlueFors.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/BlueFors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/CopperMountain/
+-rw-r--r--   0 vsts      (1001) docker     (118)    21574 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/CopperMountain/M5180.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/CopperMountain/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryocon/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryocon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6638 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryocon/cryocon_26.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryogenic/
+-rw-r--r--   0 vsts      (1001) docker     (118)    21863 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryogenic/CryogenicSMS120C.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryogenic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Gentec/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2119 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Gentec/Gentec_Maestro.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Gentec/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3099 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_E36313A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9671 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_E8267D.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1330 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_J7211.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      626 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3201A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2031 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3300A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1504 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/M3202A.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/
+-rw-r--r--   0 vsts      (1001) docker     (118)    43101 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18139 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG_Async.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29191 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_DIG.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16346 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_Module.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6234 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/memory_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3967 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/Model_331.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18098 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/Model_625.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/
+-rw-r--r--   0 vsts      (1001) docker     (118)     7571 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/DAQ.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2253 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_2597.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1477 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_5654.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9296 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/RFSG.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6389 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/Switch.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11449 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/dll_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2582 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/ni_dll_instrument.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      326 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/visa_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Newport/
+-rw-r--r--   0 vsts      (1001) docker     (118)    13722 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Newport/AG_UC8.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Newport/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/
+-rw-r--r--   0 vsts      (1001) docker     (118)     9780 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/ILM200.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28906 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/IPS120.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8296 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/Triton.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17771 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/kelvinox.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1755 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/D4.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5401 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/D5a.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2867 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/F1d.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    27765 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/IVVI.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2703 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/M2j.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3393 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/S5i.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/
+-rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8041.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8042.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      306 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMC8043.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP2020.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP2030.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP4030.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      293 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/HMP4040.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9498 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMR40.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   121277 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7792 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200Asim.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/
+-rw-r--r--   0 vsts      (1001) docker     (118)     4185 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMC804x.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4846 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMP.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Shamrock/
+-rw-r--r--   0 vsts      (1001) docker     (118)    12502 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Shamrock/SR750.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Shamrock/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/SingleQuantum/
+-rw-r--r--   0 vsts      (1001) docker     (118)    15758 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/SingleQuantum/SingleQuantum.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/SingleQuantum/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/
+-rw-r--r--   0 vsts      (1001) docker     (118)    56158 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/M4i.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5960 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/h2py.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    64337 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/regs.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1913 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/spcerr.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7543 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/pyspcm.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Standa/
+-rw-r--r--   0 vsts      (1001) docker     (118)     7537 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Standa/Standa_10MWA168.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Standa/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/
+-rw-r--r--   0 vsts      (1001) docker     (118)     9118 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/DG645.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15062 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/SIM928.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/
+-rw-r--r--   0 vsts      (1001) docker     (118)    24674 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/AFG3000.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23016 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/AWG520.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2543 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2000_Scan.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12154 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2700.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18205 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6430.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6155 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6500.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/
+-rw-r--r--   0 vsts      (1001) docker     (118)    15397 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/APT.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10488 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/K10CR1.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1711 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/MFF10x.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1661 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/PRM1Z8.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Vaunix/
+-rw-r--r--   0 vsts      (1001) docker     (118)    11690 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Vaunix/LDA.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Vaunix/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/
+-rw-r--r--   0 vsts      (1001) docker     (118)     9922 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/HF2LI.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14493 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/ZIHDAWG8.py
+-rw-r--r--   0 vsts      (1001) docker     (118)       22 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    21098 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_Keysight_M3201A.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      763 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_Spectrum_M4i.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1921 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_m2j.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6445 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_ni_pxie_2597.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1431 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_rohdeschwarz_HMC804x.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10149 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_zihdawg8.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3154 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     7213 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-20 09:09:58.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (118)       14 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       23 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)     1604 2021-05-20 09:13:53.000000 qcodes_contrib_drivers-0.9.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (118)      138 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    68611 2021-05-20 09:00:07.000000 qcodes_contrib_drivers-0.9.1/versioneer.py
```

### Comparing `qcodes_contrib_drivers-0.9.0/LICENSE` & `qcodes_contrib_drivers-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/LICENSE_TEKTRONIX_AWG520_KEITHLEY_2700` & `qcodes_contrib_drivers-0.9.1/LICENSE_TEKTRONIX_AWG520_KEITHLEY_2700`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Advantech/PCIE_1751.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Advantech/PCIE_1751.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Agilent/Agilent_N9000A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Agilent/Agilent_N9000A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/AimTTi/EL320P.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/AimTTi/EL320P.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Andor/DU401.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Andor/DU401.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC300.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC300.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC300sim.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC300sim.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/__init__.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/interface.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/interface.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v3.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v3.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v4.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Attocube/ANC350Lib/v4.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Aviosys/IP_Power_9258S.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Aviosys/IP_Power_9258S.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Bilt/ITest.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Bilt/ITest.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/BlueFors/BlueFors.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/BlueFors/BlueFors.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/CopperMountain/M5180.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/CopperMountain/M5180.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryocon/cryocon_26.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryocon/cryocon_26.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Cryogenic/CryogenicSMS120C.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Cryogenic/CryogenicSMS120C.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Gentec/Gentec_Maestro.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Gentec/Gentec_Maestro.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_E36313A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_E36313A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_E8267D.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_E8267D.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_J7211.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_J7211.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3201A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3201A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3300A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/Keysight_M3300A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/M3202A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/M3202A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG_Async.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_AWG_Async.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_DIG.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_DIG.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_Module.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/SD_Module.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Keysight/SD_common/memory_manager.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Keysight/SD_common/memory_manager.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/Model_331.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/Model_331.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Lakeshore/Model_625.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Lakeshore/Model_625.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/DAQ.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/DAQ.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_2597.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_2597.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_5654.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/PXIe_5654.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/RFSG.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/RFSG.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/Switch.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/Switch.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/dll_wrapper.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/dll_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/NationalInstruments/ni_dll_instrument.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/NationalInstruments/ni_dll_instrument.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Newport/AG_UC8.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Newport/AG_UC8.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/ILM200.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/ILM200.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/IPS120.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/IPS120.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/Triton.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/Triton.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Oxford/kelvinox.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Oxford/kelvinox.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/D4.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/D4.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/D5a.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/D5a.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/F1d.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/F1d.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/IVVI.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/IVVI.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/M2j.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/M2j.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/QuTech/S5i.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/QuTech/S5i.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMR40.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMR40.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200Asim.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/SMW200Asim.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMC804x.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMC804x.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMP.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/RohdeSchwarz/private/HMP.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Shamrock/SR750.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Shamrock/SR750.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/SingleQuantum/SingleQuantum.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/SingleQuantum/SingleQuantum.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/M4i.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/M4i.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/h2py.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/h2py.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/regs.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/regs.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/py_header/spcerr.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/py_header/spcerr.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Spectrum/pyspcm.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Spectrum/pyspcm.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Standa/Standa_10MWA168.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Standa/Standa_10MWA168.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/DG645.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/DG645.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/StanfordResearchSystems/SIM928.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/StanfordResearchSystems/SIM928.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/AFG3000.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/AFG3000.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/AWG520.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/AWG520.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2000_Scan.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2000_Scan.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2700.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_2700.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6430.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6430.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6500.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Tektronix/Keithley_6500.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/APT.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/APT.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/K10CR1.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/K10CR1.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/MFF10x.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/MFF10x.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Thorlabs/PRM1Z8.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Thorlabs/PRM1Z8.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/Vaunix/LDA.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/Vaunix/LDA.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/HF2LI.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/HF2LI.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/drivers/ZurichInstruments/ZIHDAWG8.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/drivers/ZurichInstruments/ZIHDAWG8.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_Keysight_M3201A.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_Keysight_M3201A.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_Spectrum_M4i.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_Spectrum_M4i.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_m2j.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_m2j.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_ni_pxie_2597.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_ni_pxie_2597.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_rohdeschwarz_HMC804x.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_rohdeschwarz_HMC804x.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers/tests/test_zihdawg8.py` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers/tests/test_zihdawg8.py`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/qcodes_contrib_drivers.egg-info/SOURCES.txt` & `qcodes_contrib_drivers-0.9.1/qcodes_contrib_drivers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 LICENSE_TEKTRONIX_AWG520_KEITHLEY_2700
 MANIFEST.in
+README.rst
 setup.cfg
 setup.py
 versioneer.py
 qcodes_contrib_drivers/__init__.py
 qcodes_contrib_drivers/_version.py
 qcodes_contrib_drivers.egg-info/PKG-INFO
 qcodes_contrib_drivers.egg-info/SOURCES.txt
```

### Comparing `qcodes_contrib_drivers-0.9.0/setup.cfg` & `qcodes_contrib_drivers-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `qcodes_contrib_drivers-0.9.0/versioneer.py` & `qcodes_contrib_drivers-0.9.1/versioneer.py`

 * *Files identical despite different names*

