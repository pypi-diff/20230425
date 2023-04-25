# Comparing `tmp/fal_serverless-0.6.28.tar.gz` & `tmp/fal_serverless-0.6.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.28.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.29.tar", max compression
```

## Comparing `fal_serverless-0.6.28.tar` & `fal_serverless-0.6.29.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/README.md
--rw-r--r--   0        0        0      956 2023-04-13 08:34:59.200602 fal_serverless-0.6.28/pyproject.toml
--rw-r--r--   0        0        0      335 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    14760 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2390 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5292 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    11503 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-04-13 08:34:51.100543 fal_serverless-0.6.28/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     1127 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    14988 2023-04-13 08:34:34.792433 fal_serverless-0.6.28/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     3300 2023-04-13 08:34:34.792433 fal_serverless-0.6.28/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 fal_serverless-0.6.28/setup.py
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 fal_serverless-0.6.28/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/README.md
+-rw-r--r--   0        0        0      975 2023-04-25 05:36:34.715945 fal_serverless-0.6.29/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17406 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2390 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5292 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    11653 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      158 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0      992 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    15210 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     3520 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 fal_serverless-0.6.29/setup.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fal_serverless-0.6.29/PKG-INFO
```

### Comparing `fal_serverless-0.6.28/pyproject.toml` & `fal_serverless-0.6.29/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.28"
+version = "0.6.29"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
-isolate = {version = "0.11.1", extras = ["build"]}
+isolate = {version = "0.12.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "^0.0.26"
+isolate-proto = "0.0.27"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "^2.9.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
 colorama = "^0.4.6"
 portalocker = "^2.7.0"
 rich = "^13.3.2"
 
 # For 3.10 and later, importlib-metadata's newer versions are included in the standard library.
 importlib-metadata = { version = ">=4.4", python = "<3.10" }
+packaging = "^23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fal-serverless = "fal_serverless.cli:cli"
```

### Comparing `fal_serverless-0.6.28/src/fal_serverless/api.py` & `fal_serverless-0.6.29/src/fal_serverless/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import inspect
 import os
 import time
+from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
 from dataclasses import dataclass, field, replace
 from functools import partial, wraps
-from typing import Any, Callable, ClassVar, Dict, Generic, TypeVar, cast
+from typing import Any, Callable, ClassVar, Dict, Generic, Iterator, TypeVar, cast
 
 import dill
+import dill.detect
 import grpc
 import isolate
 import yaml
 from fal_serverless.flags import bool_envvar
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.sdk import (
     FAL_SERVERLESS_DEFAULT_KEEP_ALIVE,
@@ -23,14 +25,16 @@
     MachineRequirements,
     _get_agent_credentials,
     get_default_credentials,
 )
 from isolate.backends.common import active_python
 from isolate.backends.settings import DEFAULT_SETTINGS
 from isolate.connections import PythonIPC
+from packaging.requirements import Requirement
+from packaging.utils import canonicalize_name
 
 dill.settings["recurse"] = True
 
 ReturnT = TypeVar("ReturnT")
 BasicConfig = Dict[str, Any]
 _UNSET = object()
 
@@ -42,14 +46,19 @@
 
 @dataclass
 class InternalFalServerlessError(Exception):
     ...
 
 
 @dataclass
+class FalMissingDependencyError(FalServerlessError):
+    ...
+
+
+@dataclass
 class Host:
     """The physical environment where the isolated code
     is executed."""
 
     _SUPPORTED_KEYS: ClassVar[frozenset[str]] = frozenset()
 
     @classmethod
@@ -200,22 +209,63 @@
                             )
                     elif e.details().endswith("died with <Signals.SIGKILL: 9>.`."):
                         raise FalServerlessError(
                             "Isolated function crashed. "
                             "This is likely due to resource overflow. "
                             "You can try again by setting a bigger `machine_type`"
                         )
+
+                    elif e.code() == grpc.StatusCode.INVALID_ARGUMENT and (
+                        "The function function could not be deserialized" in e.details()
+                    ):
+                        raise FalMissingDependencyError(e.details())
                     else:
                         raise FalServerlessError(e.details())
 
         return handler
 
     return decorator
 
 
+def find_missing_dependencies(
+    func: Callable[..., Any], env: dict
+) -> Iterator[tuple[str, list[str]]]:
+
+    if env["kind"] != "virtualenv":
+        return
+
+    used_modules = defaultdict(list)
+    scope = {**dill.detect.globalvars(func, recurse=True), **dill.detect.freevars(func)}  # type: ignore
+
+    for name, obj in scope.items():
+        if isinstance(obj, IsolatedFunction):
+            used_modules["fal_serverless"].append(name)
+            continue
+
+        module = inspect.getmodule(obj)
+        possible_package = getattr(module, "__package__", None)
+        if possible_package:
+            pkg_name, *_ = possible_package.split(".")  # type: ignore
+        else:
+            pkg_name = module.__name__  # type: ignore
+
+        used_modules[canonicalize_name(pkg_name)].append(name)  # type: ignore
+
+    raw_requirements = env.get("requirements", [])
+    specified_requirements = set()
+    for raw_requirement in raw_requirements:
+        requirement = Requirement(raw_requirement)
+        specified_requirements.add(canonicalize_name(requirement.name))
+
+    for module_name, used_names in used_modules.items():
+        if module_name in specified_requirements:
+            continue
+        yield module_name, used_names
+
+
 # TODO: Should we build all these in fal/dbt-fal packages instead?
 @dataclass
 class FalServerlessHost(Host):
     _SUPPORTED_KEYS = frozenset({"machine_type", "keep_alive", "setup_function"})
 
     url: str = FAL_SERVERLESS_DEFAULT_URL
     credentials: Credentials = field(default_factory=get_default_credentials)
@@ -421,20 +471,39 @@
             options=self.options,
             args=args,
             kwargs=kwargs,
         )
         return cast(Future[ReturnT], future)
 
     def __call__(self, *args, **kwargs) -> ReturnT:
-        return self.host.run(
-            self.func,
-            self.options,
-            args=args,
-            kwargs=kwargs,
-        )
+        try:
+            return self.host.run(
+                self.func,
+                self.options,
+                args=args,
+                kwargs=kwargs,
+            )
+        except FalMissingDependencyError as e:
+            pairs = list(find_missing_dependencies(self.func, self.options.environment))
+            if not pairs:
+                raise e
+            else:
+                lines = []
+                for used_modules, references in pairs:
+                    lines.append(
+                        f"    - {used_modules} (as referred by {', '.join(references)})"
+                    )
+
+                raise FalServerlessError(
+                    "A deserialization error regarding your function has occurred. \nHint: This might be "
+                    " because the following modules are referenced but not required as part of your environment "
+                    "declaration:\n"
+                    + "\n".join(lines)
+                    + "\ntry adding them to the requirements of your isolated function"
+                )
 
     def on(self, host: Host | None = None, **config: Any) -> IsolatedFunction[ReturnT]:
         host = host or self.host
         if isinstance(host, type(self.host)):
             previous_host_options = self.options.host
         else:
             previous_host_options = {}
```

### Comparing `fal_serverless-0.6.28/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.29/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.29/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.29/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/cli.py` & `fal_serverless-0.6.29/src/fal_serverless/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
+from fal_serverless.logging import get_logger, set_debug_logging
+from fal_serverless.logging.isolate import IsolateLogPrinter
+from fal_serverless.logging.trace import get_tracer
 from rich.table import Table
 
-from .logging import get_logger, set_debug_logging
-from .logging.trace import get_tracer
-
 DEFAULT_HOST = "api.alpha.fal.ai"
 HOST_ENVVAR = "FAL_HOST"
 
 DEFAULT_PORT = "443"
 PORT_ENVVAR = "FAL_PORT"
 
 DEBUG_ENABLED = False
@@ -270,51 +270,53 @@
 @click.pass_obj
 def list_scheduled(client: api.FalServerlessHost):
     table = Table(title="Cronjobs")
     table.add_column("Cron ID")
     table.add_column("Cron")
     table.add_column("ETA next run")
     table.add_column("State")
-
     for cron in client._connection.list_scheduled_runs():
         state_string = ["Not Active", "Active"][cron.active]
         table.add_row(cron.cron_id, cron.cron_string, str(cron.next_run), state_string)
 
     console.print(table)
 
 
 @crons_cli.command(name="activations")
 @click.argument("cron_id", required=True)
 @click.argument("limit", default=15)
 @click.pass_obj
 def list_activations(client: api.FalServerlessHost, cron_id: str, limit: int = 15):
     table = Table(title="Cron activations")
-    table.add_column("Cron ID")
     table.add_column("Activation ID")
-    table.add_column("Activation Start Date")
-    table.add_column("Activation Finish Date")
+    table.add_column("Start Date")
+    table.add_column("Finish Date")
 
-    for activation in client._connection.list_run_activations(cron_id)[-limit:]:
+    for activation in client._connection.list_run_activations(cron_id)[:limit]:
         table.add_row(
-            cron_id,
             str(activation.activation_id),
             str(activation.started_at),
             str(activation.finished_at),
         )
 
     console.print(table)
 
 
 @crons_cli.command(name="logs")
 @click.argument("cron_id", required=True)
-@click.argument("activation-id", required=True)
+@click.argument("activation_id", required=True)
 @click.pass_obj
 def print_logs(client: api.FalServerlessHost, cron_id: str, activation_id: str):
-    raw_logs = client._connection.get_activation_logs(activation_id)
-    console.print(raw_logs.decode(errors="ignore"), highlight=False)
+    logs = client._connection.get_activation_logs(cron_id, activation_id)
+    if not logs:
+        console.print(f"No logs found for activation {activation_id}")
+        return
+    log_printer = IsolateLogPrinter(debug=True)
+    for log in logs:
+        log_printer.print(log)
 
 
 @crons_cli.command("cancel")
 @click.argument("cron_id", required=True)
 @click.pass_obj
 def cancel_scheduled(client: api.FalServerlessHost, cron_id: str):
     client._connection.cancel_scheduled_run(cron_id)
```

### Comparing `fal_serverless-0.6.28/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.29/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.29/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.29/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.29/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.29/src/fal_serverless/logging/isolate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
 from isolate.logs import Log, LogLevel
 from structlog.dev import ConsoleRenderer
-from structlog.processors import TimeStamper
 from structlog.typing import EventDict
 
 from .style import LEVEL_STYLES
 
 _renderer = ConsoleRenderer(level_styles=LEVEL_STYLES)
 
-_timestamper = TimeStamper(fmt="%Y-%m-%d %H:%M:%S", utc=False)
-
 
 class IsolateLogPrinter:
 
     debug: bool
 
     def __init__(self, debug: bool = False) -> None:
         self.debug = debug
@@ -22,16 +19,15 @@
     def print(self, log: Log):
         if log.level < LogLevel.INFO and not self.debug:
             return
         level = str(log.level)
         event: EventDict = {
             "event": log.message,
             "level": level,
+            "timestamp": log.timestamp.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3],
         }
-        if self.debug:
-            bound_env = log.bound_env.key if log.bound_env is not None else "global"
-            event["bound_env"] = bound_env
+        if self.debug and log.bound_env and log.bound_env.key != "global":
+            event["bound_env"] = log.bound_env.key
 
         # Use structlog processors to get consistent output with local logs
-        event = _timestamper.__call__(logger={}, name=level, event_dict=event)
         message = _renderer.__call__(logger={}, name=level, event_dict=event)
         print(message)
```

### Comparing `fal_serverless-0.6.28/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.29/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.29/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.28/src/fal_serverless/sdk.py` & `fal_serverless-0.6.29/src/fal_serverless/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,16 +458,20 @@
         ]
 
     def cancel_scheduled_run(self, cron_id: str) -> None:
         request = isolate_proto.CancelCronRequest(cron_id=cron_id)
         response: isolate_proto.CancelCronResult = self.stub.CancelCron(request)
         return
 
-    def get_activation_logs(self, activation_id: str) -> bytes:
-        raise NotImplementedError
+    def get_activation_logs(self, cron_id: str, activation_id: str) -> list[Log]:
+        request = isolate_proto.GetActivationLogsRequest(
+            cron_id=cron_id, activation_id=activation_id
+        )
+        response = self.stub.GetActivationLogs(request)
+        return [from_grpc(log) for log in response.logs]
 
     def list_worker_status(self, user_id: str | None = None) -> list[WorkerStatus]:
         request = isolate_proto.WorkerStatusListRequest(user_id=user_id)
         response = self.stub.WorkerStatusList(request)
         return [
             WorkerStatus(
                 ws.worker_id,
```

### Comparing `fal_serverless-0.6.28/src/fal_serverless/sync.py` & `fal_serverless-0.6.29/src/fal_serverless/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,35 +72,41 @@
         for root, _, files in os.walk(dir_path):
             for file in files:
                 file_path = os.path.join(root, file)
                 arcname = file_path[len(dir_path) :]
                 zipf.write(file_path, arcname)
 
 
-def sync_dir(local_dir: str, remote_dir: str, force_upload=False) -> None:
+def sync_dir(local_dir: str, remote_dir: str, force_upload=False) -> str:
+    if not os.path.isabs(remote_dir) or not remote_dir.startswith("/data"):
+        raise ValueError(
+            "'remote_dir' must be an absolute path starting with `/data`, e.g. '/data/sync/my_dir'"
+        )
+
     # Compute the local directory hash
     local_hash = _compute_directory_hash(local_dir)
 
-    full_remote_dir = os.path.join("/data/sync", remote_dir)
-
-    print(f"Syncing {local_dir} with {full_remote_dir}...")
+    print(f"Syncing {local_dir} with {remote_dir}...")
 
-    if _check_hash(full_remote_dir, local_hash) and not force_upload:
+    if _check_hash(remote_dir, local_hash) and not force_upload:
         print(f"{remote_dir} already uploaded and matches {local_dir}")
-        return
+        return remote_dir
 
     with open(os.path.join(local_dir, ".fal_hash"), "w") as f:
         f.write(local_hash)
 
     # Zip the local directory
     zip_path = f"{local_dir}.zip"
 
     _zip_directory(local_dir, zip_path)
 
     # Upload the zipped directory to the serverless environment
     zip_remote_path = os.path.join("/data/sync", os.path.basename(zip_path))
     _upload_file(zip_path, zip_remote_path)
-    _unzip_target_directory(zip_remote_path, full_remote_dir)
+    _unzip_target_directory(zip_remote_path, remote_dir)
 
     # Remove the zipped directory
     os.remove(zip_path)
     print("Done")
+
+    # Return the full path to the remote directory
+    return remote_dir
```

### Comparing `fal_serverless-0.6.28/setup.py` & `fal_serverless-0.6.29/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,34 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client>=2.9.0,<3.0.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.26,<0.0.27',
- 'isolate[build]==0.11.1',
+ 'isolate-proto==0.0.27',
+ 'isolate[build]==0.12.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
+ 'packaging>=23.1,<24.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=13.3.2,<14.0.0',
  'structlog>=22.3.0,<23.0.0',
  'typing-extensions==4.4']
 
 extras_require = \
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.28',
+    'version': '0.6.29',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.28/PKG-INFO` & `fal_serverless-0.6.29/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.28
+Version: 0.6.29
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,18 +15,19 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.26,<0.0.27)
-Requires-Dist: isolate[build] (==0.11.1)
+Requires-Dist: isolate-proto (==0.0.27)
+Requires-Dist: isolate[build] (==0.12.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: typing-extensions (==4.4)
 Description-Content-Type: text/markdown
```

