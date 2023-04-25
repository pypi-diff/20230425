# Comparing `tmp/psytricks-0.1.0.tar.gz` & `tmp/psytricks-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-0.1.0.tar", max compression
+gzip compressed data, was "psytricks-1.0.0.tar", max compression
```

## Comparing `psytricks-0.1.0.tar` & `psytricks-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-0.1.0/LICENSE
--rw-r--r--   0        0        0      109 2022-12-20 15:40:57.930292 psytricks-0.1.0/README.md
--rw-r--r--   0        0        0      973 2023-04-14 09:23:37.025472 psytricks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-04-14 09:23:37.029473 psytricks-0.1.0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     4664 2023-04-14 09:23:11.163997 psytricks-0.1.0/src/psytricks/cli.py
--rw-r--r--   0        0        0     2247 2023-04-13 12:44:28.211286 psytricks-0.1.0/src/psytricks/decoder.py
--rw-r--r--   0        0        0     1801 2023-04-13 12:44:28.207286 psytricks-0.1.0/src/psytricks/mappings.py
--rw-r--r--   0        0        0     3014 2023-04-13 12:38:57.964112 psytricks-0.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json
--rw-r--r--   0        0        0    18687 2023-04-13 12:44:28.215286 psytricks-0.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json
--rw-r--r--   0        0        0     2967 2023-04-13 12:44:28.215286 psytricks-0.1.0/src/psytricks/ps1scripts/dummydata/GetSessions.json
--rw-r--r--   0        0        0    11721 2023-04-13 12:38:58.096114 psytricks-0.1.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1
--rw-r--r--   0        0        0    11054 2023-04-13 13:25:42.170139 psytricks-0.1.0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 psytricks-0.1.0/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 psytricks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3557 2023-04-25 12:23:05.630073 psytricks-1.0.0/README.md
+-rw-r--r--   0        0        0      973 2023-04-25 12:40:48.831068 psytricks-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-25 12:40:48.831068 psytricks-1.0.0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-25 11:22:59.630911 psytricks-1.0.0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     2247 2023-04-13 12:44:28.211286 psytricks-1.0.0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0     1801 2023-04-13 12:44:28.207286 psytricks-1.0.0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0     3014 2023-04-13 12:38:57.964112 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-04-25 07:07:36.345357 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-04-25 07:59:35.398779 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetSessions.json
+-rw-r--r--   0        0        0    11759 2023-04-25 11:05:43.569742 psytricks-1.0.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0    11067 2023-04-25 11:09:47.919739 psytricks-1.0.0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 psytricks-1.0.0/setup.py
+-rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 psytricks-1.0.0/PKG-INFO
```

### Comparing `psytricks-0.1.0/LICENSE` & `psytricks-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-0.1.0/pyproject.toml` & `psytricks-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "0.1.0"
+version = "1.0.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-0.1.0/src/psytricks/cli.py` & `psytricks-1.0.0/src/psytricks/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Command line interface related functions."""
 
 # pylint: disable-msg=too-many-arguments
 
 import sys
-from pprint import pprint
+from pprint import pprint, pformat
 
 import click
 from loguru import logger as log
 
+from . import __version__
 from .wrapper import PSyTricksWrapper
 
 
 def configure_logging(verbose: int):
     """Configure loguru logging / change log level.
 
     Parameters
@@ -30,19 +31,20 @@
     # set up logging, loguru requires us to remove the default handler and
     # re-add a new one with the desired log-level:
     log.remove()
     log.add(sys.stderr, level=level)
     log.info(f"Set logging level to [{level}] ({verbose}).")
 
 
-@click.command(help="Run the PSyTricks command line interface.")
+@click.command(help="Run the PSyTricks command line interface.", no_args_is_help=True)
+@click.version_option(__version__)
 @click.option(
-    "--config",
-    type=click.Path(exists=True),
-    help="A JSON configuration file.",
+    "--cdc",
+    type=str,
+    help="The address of the Citrix Delivery Controller (CDC) to connect to.",
     required=True,
 )
 @click.option(
     "-v",
     "--verbose",
     count=True,
     help="Increase logging verbosity, may be repeated up to 3 times.",
@@ -104,28 +106,35 @@
     "--disable",
     is_flag=True,
     help=(
         "Flag to indicate a certain property should be disabled / removed. "
         "[applies to: 'maintenance', 'setaccess']"
     ),
 )
-def run_cli(config, verbose, command, machine, group, action, message, users, disable):
+@click.option(
+    "--outfile",
+    type=click.Path(dir_okay=False, writable=True),
+    help="The path to a file to write the output into (default=stdout).",
+)
+def run_cli(
+    cdc, verbose, command, machine, group, action, message, users, disable, outfile
+):
     """Create a wrapper object and call the method requested on the command line.
 
     Parameters
     ----------
-    config : str
-        Path to the JSON config file required by the PowerShell script.
+    cdc : str
+        The address of the Citrix Delivery Controller (CDC) to connect to.
     verbose : int
         The logging verbosity.
     command : str
         The command indicating which wrapper method to call.
     """
     configure_logging(verbose)
-    wrapper = PSyTricksWrapper(conffile=config)
+    wrapper = PSyTricksWrapper(deliverycontroller=cdc)
     call_method = {
         "disconnect": wrapper.disconnect_session,
         "getaccess": wrapper.get_access_users,
         "machines": wrapper.get_machine_status,
         "maintenance": wrapper.set_maintenance,
         "poweraction": wrapper.perform_poweraction,
         "sendmessage": wrapper.send_message,
@@ -154,8 +163,13 @@
     if command in ["maintenance", "poweraction"] and machine is None:
         raise click.UsageError(
             "Commands 'maintenance'/'poweraction' require --machine!"
         )
 
     details = call_method[command](**call_kwargs)
 
-    pprint(details)
+    if outfile:
+        with open(outfile, "a", encoding="utf-8") as fh:
+            fh.writelines(pformat(details))
+        log.success(f"Done writing output into [{outfile}].")
+    else:
+        pprint(details)
```

### Comparing `psytricks-0.1.0/src/psytricks/decoder.py` & `psytricks-1.0.0/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-0.1.0/src/psytricks/mappings.py` & `psytricks-1.0.0/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-0.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json` & `psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-0.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json` & `psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8829365079365076%*

 * *Differences: {'0': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2}",*

 * * '1': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2}",*

 * * '10': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2, 'DesktopGroupName': 'Dinner'}",*

 * * '11': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2, 'DesktopGroupName': 'Dinner'}",*

 * * '12': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2}",*

 * * '13': "{'PowerState': 4, 'RegistrationState': 2, 'SummaryState': 2}",*

 * * '14': "{'PowerState': 4, 'R […]*

```diff
@@ -2,594 +2,599 @@
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d401.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d401",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d402.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d402",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d403.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d403",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.a@example.xy"
         ],
         "DNSName": "ctricks-vm-d404.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d404",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "21.1.0.14",
         "SessionDeviceId": "Ubuntu-2204",
         "SessionStartTime": "/Date(1679653979000)/",
         "SessionStateChangeTime": "/Date(1679656665997)/",
         "SessionUserName": "EXAMPLEDOMAIN\\usera",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d405.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d405",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.b@example.xy"
         ],
         "DNSName": "ctricks-vm-d406.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d406",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "23.01.0.16",
         "SessionDeviceId": "xy-rgxx01-plm01",
         "SessionStartTime": "/Date(1679565112000)/",
         "SessionStateChangeTime": "/Date(1679589645917)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userb",
-        "SummaryState": "disconnected"
+        "SummaryState": 3
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.c@example.xy"
         ],
         "DNSName": "ctricks-vm-d501.vdi.example.xy",
         "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d501",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.3.2000.2105",
         "SessionDeviceId": "xy-rgxx01-pdw01",
         "SessionStartTime": "/Date(1678963753000)/",
         "SessionStateChangeTime": "/Date(1679646240373)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userc",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d502.vdi.example.xy",
+        "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d502",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d503.vdi.example.xy",
+        "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d503",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d504.vdi.example.xy",
+        "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d504",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d505.vdi.example.xy",
+        "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d505",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-d506.vdi.example.xy",
+        "DesktopGroupName": "Dinner",
         "HostedMachineName": "ctricks-vm-d506",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-h401.vdi.example.xy",
         "DesktopGroupName": "Heart",
         "HostedMachineName": "ctricks-vm-h401",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-h402.vdi.example.xy",
         "DesktopGroupName": "Heart",
         "HostedMachineName": "ctricks-vm-h402",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-h501.vdi.example.xy",
         "DesktopGroupName": "Heart",
         "HostedMachineName": "ctricks-vm-h501",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-h502.vdi.example.xy",
         "DesktopGroupName": "Heart",
         "HostedMachineName": "ctricks-vm-h502",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.a@example.xy"
         ],
         "DNSName": "ctricks-vm-n401.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n401",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "21.1.0.14",
         "SessionDeviceId": "Ubuntu-21.34",
         "SessionStartTime": "/Date(1679660327000)/",
         "SessionStateChangeTime": "/Date(1679660327637)/",
         "SessionUserName": "EXAMPLEDOMAIN\\usera",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.b@example.xy"
         ],
         "DNSName": "ctricks-vm-n402.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n402",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "23.01.0.16",
         "SessionDeviceId": "xy-rgxx01-plm01",
         "SessionStartTime": "/Date(1678183269000)/",
         "SessionStateChangeTime": "/Date(1679564956333)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userb",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.c@example.xy"
         ],
         "DNSName": "ctricks-vm-n403.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n403",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.12.0.12",
         "SessionDeviceId": "PinkThad-T490",
         "SessionStartTime": "/Date(1679556708000)/",
         "SessionStateChangeTime": "/Date(1679641780037)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userc",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.d@example.xy"
         ],
         "DNSName": "ctricks-vm-n404.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n404",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.3.2000.2105",
         "SessionDeviceId": "xy-rgxx01-pdw04",
         "SessionStartTime": "/Date(1679562969000)/",
         "SessionStateChangeTime": "/Date(1679601596373)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userd",
-        "SummaryState": "disconnected"
+        "SummaryState": 3
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.e@example.xy"
         ],
         "DNSName": "ctricks-vm-n501.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n501",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.3.2000.2105",
         "SessionDeviceId": "xy-rgxx01-pdw17",
         "SessionStartTime": "/Date(1679662071000)/",
         "SessionStateChangeTime": "/Date(1679662071997)/",
         "SessionUserName": "EXAMPLEDOMAIN\\usere",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.f@example.xy"
         ],
         "DNSName": "ctricks-vm-n502.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n502",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.2.0.4525",
         "SessionDeviceId": "EVO-OVIS",
         "SessionStartTime": "/Date(1679402296000)/",
         "SessionStateChangeTime": "/Date(1679658862193)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userf",
-        "SummaryState": "disconnected"
+        "SummaryState": 3
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.g@example.xy"
         ],
         "DNSName": "ctricks-vm-n503.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n503",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "23.01.0.16",
         "SessionDeviceId": "xy-rgxx01-pdl12",
         "SessionStartTime": "/Date(1679596191000)/",
         "SessionStateChangeTime": "/Date(1679596288500)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userg",
-        "SummaryState": "disconnected"
+        "SummaryState": 3
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [
             "user.h@example.xy"
         ],
         "DNSName": "ctricks-vm-n504.vdi.example.xy",
         "DesktopGroupName": "Night",
         "HostedMachineName": "ctricks-vm-n504",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": "22.3.2000.2105",
         "SessionDeviceId": "xy-rgxx01-pdw14",
         "SessionStartTime": "/Date(1679652800000)/",
         "SessionStateChangeTime": "/Date(1679652800450)/",
         "SessionUserName": "EXAMPLEDOMAIN\\userh",
-        "SummaryState": "inuse"
+        "SummaryState": 4
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t401.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t401",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t402.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t402",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t403.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t403",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t404.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t404",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t405.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t405",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t406.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t406",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t501.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t501",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t502.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t502",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t503.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t503",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t504.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t504",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t505.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t505",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     },
     {
         "AgentVersion": "2203.0.2000.2076",
         "AssociatedUserUPNs": [],
         "DNSName": "ctricks-vm-t506.vdi.example.xy",
         "DesktopGroupName": "Tree",
         "HostedMachineName": "ctricks-vm-t506",
         "InMaintenanceMode": false,
-        "PowerState": "on",
-        "RegistrationState": "registered",
+        "PowerState": 4,
+        "RegistrationState": 2,
         "SessionClientVersion": null,
         "SessionDeviceId": null,
         "SessionStartTime": null,
         "SessionStateChangeTime": null,
         "SessionUserName": null,
-        "SummaryState": "available"
+        "SummaryState": 2
     }
 ]
```

### Comparing `psytricks-0.1.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1` & `psytricks-1.0.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [CmdletBinding()]
 param (
-    # the JSON config file to use
+    # the delivery controller address to connect to
     [Parameter(Mandatory = $true)]
     [string]
-    $JsonConfig,
+    $AdminAddress,
 
     # the command defining the action to be performed by the wrapper
     [Parameter(Mandatory = $true)]
     [ValidateSet(
         "DisconnectSession",
         "GetAccessUsers",
         "GetMachineStatus",
@@ -104,14 +104,20 @@
     "SessionStartTime",
     "SessionStateChangeTime",
     "SessionUserName",
     "SummaryState"
 )
 
 $SessionProperties = @(
+    "ClientAddress",
+    "ClientName",
+    "ClientPlatform",
+    "ClientProductId",
+    "ClientVersion",
+    "ConnectedViaHostName",
     "DesktopGroupName",
     "DNSName",
     "MachineSummaryState",
     "Protocol",
     "SessionState",
     "SessionStateChangeTime",
     "StartTime",
@@ -119,80 +125,73 @@
     "UserName",
     "UserUPN"
 )
 
 #endregion properties-selectors
 
 
-#region config-setup
-
-try {
-    $Config = Get-Content $JsonConfig | ConvertFrom-Json -EA Stop
-} catch {
-    throw "Error reading JSON configuration file: [$JsonConfig]"
-}
-$AdmAddr = $Config.CitrixDC
+#region snapin
 
 if ($NoSnapIn) {
     Write-Debug "NOT loading Citrix Broker Snap-In, can only work on 'dummy' data!"
 } else {
     Add-PSSnapin Citrix.Broker.Admin.V2 -EA Stop
 }
 
-#endregion config-setup
+#endregion snapin
 
 
 #region functions
 
 function Get-MachineStatus {
-    $Data = Get-BrokerMachine -AdminAddress $AdmAddr | `
+    $Data = Get-BrokerMachine -AdminAddress $AdminAddress | `
         Select-Object -Property $MachineProperties
     return $Data
 }
 
 function Get-Sessions {
-    $Data = Get-BrokerSession -AdminAddress $AdmAddr | `
+    $Data = Get-BrokerSession -AdminAddress $AdminAddress | `
         Select-Object -Property $SessionProperties
     return $Data
 }
 
 function Disconnect-Session {
     param (
         # the FQDN of the machine to disconnect the session on
         [Parameter()]
         [string]
         $DNSName
     )
-    $Session = Get-BrokerSession -AdminAddress $AdmAddr -DNSName $DNSName
+    $Session = Get-BrokerSession -AdminAddress $AdminAddress -DNSName $DNSName
     if ($null -eq $Session) {
         return $null
     }
     if ($Session.SessionState -eq "Disconnected") {
         Write-Verbose "Session already disconnected, not disconnecting again!"
         return Select-Object -InputObject $Session -Property $SessionProperties
     }
-    Disconnect-BrokerSession -AdminAddress $AdmAddr -InputObject $Session
+    Disconnect-BrokerSession -AdminAddress $AdminAddress -InputObject $Session
 
     # wait a bit until the status update is reflected by Citrix:
     Start-Sleep -Seconds 0.7
 
-    $Data = Get-BrokerSession -AdminAddress $AdmAddr -DNSName $DNSName | `
+    $Data = Get-BrokerSession -AdminAddress $AdminAddress -DNSName $DNSName | `
         Select-Object -Property $SessionProperties
     return $Data
 }
 
 function Get-AccessUsers {
     param (
         # the name of the Delivery Group to get users with access for
         [Parameter()]
         [string]
         $Group
     )
     $Data = Get-BrokerAccessPolicyRule `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -DesktopGroupName $Group | `
         Select-Object -ExpandProperty IncludedUsers
     return $Data
 }
 
 function Set-AccessUsers {
     param (
@@ -208,31 +207,31 @@
 
         # list of usernames to add / remove access to the given group
         [Parameter()]
         [string[]]
         $UserNames
     )
     $Policy = Get-BrokerAccessPolicyRule `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -DesktopGroupName $Group
 
     if ($null -eq $Policy) {
         throw "Error fetching permissions for Delivery Group [$Group]!"
     }
 
     if ($RemoveAccess) {
         $Data = Set-BrokerAccessPolicyRule `
-            -AdminAddress $AdmAddr `
+            -AdminAddress $AdminAddress `
             -InputObject $Policy `
             -RemoveIncludedUsers $UserNames `
             -PassThru | `
             Select-Object -ExpandProperty IncludedUsers
     } else {
         $Data = Set-BrokerAccessPolicyRule `
-            -AdminAddress $AdmAddr `
+            -AdminAddress $AdminAddress `
             -InputObject $Policy `
             -AddIncludedUsers $UserNames `
             -PassThru | `
             Select-Object -ExpandProperty IncludedUsers
     }
     return $Data
 }
@@ -248,28 +247,28 @@
         [Parameter()]
         [switch]
         $Disable
     )
     $DesiredMode = (-not $Disable)
 
     $Machine = Get-BrokerMachine `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -DNSName $DNSName
 
     if ($null -eq $Machine) {
         throw "Error fetching machine object for [$DNSName]!"
     }
 
     Set-BrokerMachineMaintenanceMode `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -InputObject $Machine `
         -MaintenanceMode $DesiredMode
 
     $Data = Get-BrokerMachine `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -DNSName $DNSName | `
         Select-Object -Property $MachineProperties
 
     return $Data
 }
 
 function Invoke-PowerAction {
@@ -290,15 +289,15 @@
             "turnoff",
             "turnon"
         )]
         [string]
         $Action
     )
     $Data = New-BrokerHostingPowerAction `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -MachineName $DNSName `
         -Action $Action
 
     return $Data
 }
 
 function Send-SessionMessage {
@@ -326,24 +325,24 @@
             "Critical",
             "Question"
         )]
         [string]
         $MessageStyle = "Information"
     )
     $Session = Get-BrokerSession `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -DNSName $DNSName
 
     if ($null -eq $Session) {
         throw "Error fetching session object for [$DNSName]!"
     }
 
     Send-BrokerSessionMessage `
         -InputObject $Session `
-        -AdminAddress $AdmAddr `
+        -AdminAddress $AdminAddress `
         -MessageStyle $MessageStyle `
         -Title $Title `
         -Text $Text
 }
 
 #endregion functions
```

### Comparing `psytricks-0.1.0/src/psytricks/wrapper.py` & `psytricks-1.0.0/src/psytricks/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,22 @@
         symbol "€") or in case parsing it via `json.loads()` failed.
     """
 
     pswrapper = (
         Path(abspath(dirname(__file__))) / "ps1scripts" / "psytricks-wrapper.ps1"
     )
 
-    def __init__(self, conffile: str):
+    def __init__(self, deliverycontroller: str):
         """Constructor for the `PSyTricksWrapper` class.
 
         Parameters
         ----------
-        conffile : str
-            The path to a JSON-formatted configuration file required by the
-            PowerShell script that will be called by the wrapper.
+        deliverycontroller : str
+            The address (IP or FQDN) of the Citrix Delivery Controller to
+            connect to.
         """
         # FIXME: this is a hack while implementing the package, remove for production!
         self.add_flags = []
         if platform.startswith("linux"):
             self.ps_exe = Path("/snap/bin/pwsh")
             self.add_flags = ["-Dummy", "-NoSnapIn"]
         else:
@@ -66,17 +66,17 @@
                 Path(os.environ["SYSTEMROOT"])
                 / "System32"
                 / "WindowsPowerShell"
                 / "v1.0"
                 / "powershell.exe"
             )
 
-        self.conffile = Path(conffile)
+        self.deliverycontroller = deliverycontroller
         log.debug(f"Using PowerShell script [{self.pswrapper}].")
-        log.debug(f"Using configuration file [{self.conffile}].")
+        log.debug(f"Using Delivery Controller [{self.deliverycontroller}].")
 
     def _run_ps1_script(self, request: RequestNames, extra_params: list = None) -> list:
         """Call the PowerShell wrapper to retrieve information from Citrix.
 
         Parameters
         ----------
         request : RequestNames
@@ -108,16 +108,16 @@
             tstart = time.time()
             command = [
                 self.ps_exe,
                 "-NonInteractive",
                 "-NoProfile",
                 "-File",
                 self.pswrapper,
-                "-JsonConfig",
-                self.conffile,
+                "-AdminAddress",
+                self.deliverycontroller,
                 "-CommandName",
                 request,
             ]
             command = command + self.add_flags + extra_params
             log.debug(f"Command for subprocess call: {command}")
             completed = subprocess.run(
                 command,
```

