# Comparing `tmp/tgwrap-0.5.3.tar.gz` & `tmp/tgwrap-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.5.3.tar", max compression
+gzip compressed data, was "tgwrap-0.5.4.tar", max compression
```

## Comparing `tgwrap-0.5.3.tar` & `tgwrap-0.5.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.5.3/LICENSE
--rw-r--r--   0        0        0     5444 2023-03-08 12:07:36.556538 tgwrap-0.5.3/README.md
--rw-r--r--   0        0        0      879 2023-04-05 12:37:42.975493 tgwrap-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.5.3/tgwrap/__init__.py
--rwxr-xr-x   0        0        0    23596 2023-03-28 14:15:39.016474 tgwrap-0.5.3/tgwrap/cli.py
--rwxr-xr-x   0        0        0    44906 2023-04-05 12:18:18.293569 tgwrap-0.5.3/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.5.3/tgwrap/printer.py
--rw-r--r--   0        0        0     4435 2023-01-17 14:04:36.314955 tgwrap-0.5.3/tgwrap/terrasafe.py
--rw-r--r--   0        0        0     6509 1970-01-01 00:00:00.000000 tgwrap-0.5.3/setup.py
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 tgwrap-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.5.4/LICENSE
+-rw-r--r--   0        0        0     5918 2023-04-25 13:13:36.680756 tgwrap-0.5.4/README.md
+-rw-r--r--   0        0        0      879 2023-04-25 13:19:35.269253 tgwrap-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.5.4/tgwrap/__init__.py
+-rwxr-xr-x   0        0        0    24310 2023-04-25 12:36:41.404857 tgwrap-0.5.4/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    45291 2023-04-25 12:53:35.280347 tgwrap-0.5.4/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.5.4/tgwrap/printer.py
+-rw-r--r--   0        0        0     4435 2023-01-17 14:04:36.314955 tgwrap-0.5.4/tgwrap/terrasafe.py
+-rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 tgwrap-0.5.4/setup.py
+-rw-r--r--   0        0        0     6957 1970-01-01 00:00:00.000000 tgwrap-0.5.4/PKG-INFO
```

### Comparing `tgwrap-0.5.3/LICENSE` & `tgwrap-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.3/README.md` & `tgwrap-0.5.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -88,14 +88,27 @@
 tgwrap output -- -json
 ```
 
 > Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:
 
 `tgwrap state mv 'azuread_group.this[\"viewers\"]' 'azuread_group.this[\"readers\"]'`
 
+## A word about escaping inputs
+
+Your shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.
+
+For example:
+
+```console
+# to exclude certain modules from an action (such as analyze):
+tgwrap analyze -E 'integrations/\*/\*'
+
+# to import a resource that has a " in its address:
+tgwrap import -a 'azuread_group.this[\"my_group\"]' -i ${GROUP_ID}
+```
 
 ## Deploy manifests
 
 In order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:
 
 ```yaml
 ---
```

### Comparing `tgwrap-0.5.3/pyproject.toml` & `tgwrap-0.5.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.5.3"
+version = "0.5.4"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.5.3/tgwrap/cli.py` & `tgwrap-0.5.4/tgwrap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,21 +211,21 @@
     help='When running in step-by-step mode, start processing at the given step number',
     )
 @click.option('--limit-parallelism', '-l', type=int, default=None,
     help='Limit the parallelism to the given number, unlimitted if omitted',
     )
 @click.option('--include-dir', '-I',
     multiple=True, default=[],
-    help='A glob of a directory that needs to be included, this option can be used multiple times',
+    help='A glob of a directory that needs to be included, this option can be used multiple times. For example: -I "integrations/\*/\*"',
     show_default=True
     )
 @click.option('--exclude-dir', '-E',
     multiple=True, default=[],
-    help='A glob of a directory that needs to be excluded, this option can be used multiple times',
-    show_default=True
+    help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
+    show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run_all(command, verbose, debug, dry_run, no_lock, update, exclude_external_dependencies,
     step_by_step, planfile, auto_approve, working_dir, start_at_step,
     limit_parallelism, include_dir, exclude_dir, terragrunt_args):
     """ Executes a terragrunt command across multiple projects """
@@ -327,31 +327,43 @@
 @click.option('--terrasafe-config', '-T', default=None,
     help='Name of the terrasafe config file (or set the TERRASAFE_CONFIG environment variable)',
     envvar='TERRASAFE_CONFIG', type=click.Path(),
     )
 @click.option('--parallel-execution', '-p', is_flag=True, default=False,
     help='Whether or not to use parallel execution',
     )
+@click.option('--include-dir', '-I',
+    multiple=True, default=[],
+    help='A glob of a directory that needs to be included, this option can be used multiple times. For example: -I "integrations/\*/\*"',
+    show_default=True
+    )
+@click.option('--exclude-dir', '-E',
+    multiple=True, default=[],
+    help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
+    show_default=True,
+    )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
-def analyze(verbose, dry_run, exclude_external_dependencies, working_dir, 
-    start_at_step, out, parallel_execution, terrasafe_config, terragrunt_args):
+def analyze(verbose, dry_run, exclude_external_dependencies, working_dir, start_at_step,
+    out, terrasafe_config, parallel_execution, include_dir, exclude_dir, terragrunt_args):
     """ Analyzes the plan files """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.analyze(
         dry_run=dry_run,
         exclude_external_dependencies=exclude_external_dependencies,
         working_dir=working_dir,
         start_at_step=start_at_step,
         out=out,
-        parallel_execution=parallel_execution,
         terrasafe_config=terrasafe_config,
+        parallel_execution=parallel_execution,
+        include_dir=include_dir,
+        exclude_dir=exclude_dir,
         terragrunt_args=terragrunt_args,
     )
 
 @main.command(
     name="lock",
     context_settings=dict(
         ignore_unknown_options=True,
@@ -625,21 +637,21 @@
 @click.option('--exclude-external-dependencies/--include-external-dependencies', '-x/-i',
     is_flag=True, default=True,
     help='Whether or not external dependencies must be ignored',
     show_default=True
     )
 @click.option('--include-dir', '-I',
     multiple=True, default=[],
-    help='A glob of a directory that needs to be included, this option can be used multiple times',
+    help='A glob of a directory that needs to be included, this option can be used multiple times. For example: -I "integrations/\*/\*"',
     show_default=True
     )
 @click.option('--exclude-dir', '-E',
     multiple=True, default=[],
-    help='A glob of a directory that needs to be excluded, this option can be used multiple times',
-    show_default=True
+    help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
+    show_default=True,
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def show_graph(verbose, backwards, exclude_external_dependencies, working_dir, include_dir, exclude_dir, terragrunt_args):
```

### Comparing `tgwrap-0.5.3/tgwrap/main.py` & `tgwrap-0.5.4/tgwrap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
     def _prepare_groups(self, graph, exclude_external_dependencies, working_dir,
                         exclude_dir=[], include_dir=[]):
         """ Prepare the list of groups that will be executed """
 
         working_dir = os.path.abspath(working_dir) if working_dir else os.getcwd()
         self.printer.verbose(f"Check for working dir: {working_dir}")
 
-        print(include_dir, exclude_dir)
+        self.printer.verbose(f"Include dirs: {'; '.join(include_dir)}")
+        self.printer.verbose(f"Exclude dirs: {'; '.join(exclude_dir)}")
+
         groups = []
         for group in nx.topological_generations(graph):
             try:
                 group.remove("\\n") # terragrunt is adding this in some groups for whatever reason
             except ValueError:
                 pass
 
@@ -441,15 +443,15 @@
                         dry_run=dry_run,
                         progress=progress,
                     )
 
                     if stop_processing:
                         self.printer.warning(f"Processing needs to be stopped at step {step_nbr}.")
                         self.printer.normal(
-                            f"After you've fixed the problem, you can continue where you were left by adding '--start-at-step {step_nbr}'."
+                            f"After you've fixed the problem, you can continue where you left off by adding '--start-at-step {step_nbr}'."
                             )
                         sys.exit(1)
 
         if parallel_execution:
             # now wait until the threads are done and collect the output
             # todo: how to implement something as stop_processing like in regular execution?
             total_counter = counter
@@ -651,16 +653,16 @@
             # tgwrap import 'azuread_group.this["viewers"]' '123e4567-e89b-12d3-a456-426655440000'
             rc = subprocess.run(
                 shlex.split(cmd, posix=False),
                 env=env,
             )
             self.printer.verbose(rc)
 
-    def analyze(self, dry_run, exclude_external_dependencies, working_dir,
-        start_at_step, out, parallel_execution, terrasafe_config, terragrunt_args):
+    def analyze(self, dry_run, exclude_external_dependencies, working_dir, start_at_step,
+        out, terrasafe_config, parallel_execution, include_dir, exclude_dir, terragrunt_args):
         """ Analyzes the plan files """
 
         self.printer.verbose("Attempting to 'analyze'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
         # first run a 'show' and write output to file
@@ -695,14 +697,16 @@
                     command=cmd,
                     exclude_external_dependencies=exclude_external_dependencies,
                     dry_run=dry_run,
                     collect_output_file=f,
                     working_dir=working_dir,
                     start_at_step=start_at_step,
                     ask_for_confirmation=False,
+                    include_dir=include_dir,
+                    exclude_dir=exclude_dir,
                     parallel_execution=parallel_execution,
                 )
 
             with open(f.name, 'r') as f:
                 for line in f:
                     split_line = line.split(self.SEPARATOR)
                     module = split_line[0]
@@ -902,15 +906,15 @@
                     stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
                     )
                 self.printer.verbose(rc)
 
             # collect all the base paths of the substacks as you don't want
             # to include them in regular syncs
             substacks = []
-            for ss, substack in manifest['sub_stacks'].items():
+            for ss, substack in manifest.get('sub_stacks', {}).items():
                 # get the base directory of the sub stack so that we can ignore it when deploying the regular modules
                 substacks.append(substack['source'].split(os.path.sep)[0])
 
             deploy_actions = {}
             for key, value in manifest['deploy'].items():
                 if target_stage not in value['applies_to_stages']:
                     self.printer.verbose(f'Target stage {target_stage} not applicable for action {key}.')
@@ -934,15 +938,15 @@
                             self.printer.verbose(f'Exclude module {source_module}')
                         else:
                             deploy_actions[module] = {
                                 "source": os.path.join(source_path, source_module, ''),
                                 "target": os.path.join(target_dir, target_module, ''),
                             }
 
-                    for ss, substack in manifest['sub_stacks'].items():
+                    for ss, substack in manifest.get('sub_stacks', {}).items():
                         self.printer.verbose(f'Found substack : {ss}')
 
                         source_path = os.path.join(
                             source_dir, source_stage, substack['source'], ''
                             )
                         target_path = os.path.join(
                             target_dir, substack['target'], ''
@@ -1003,14 +1007,17 @@
     def show_graph(self, backwards, exclude_external_dependencies, working_dir, include_dir, exclude_dir, terragrunt_args):
         """ Shows the dependencies of a project """
 
         self.printer.verbose(f"Attempting to show dependencies")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
+        # self.printer.verbose(f"Include dirs: {'; '.join(include_dir)}")
+        # self.printer.verbose(f"Exclude dirs: {'; '.join(exclude_dir)}")
+
         "Runs the desired command in the directories as defined in the directed graph"
         graph = self._get_di_graph(backwards=backwards, working_dir=working_dir)
 
         # first go through the groups and clean up where needed
         groups = self._prepare_groups(
             graph=graph,
             exclude_external_dependencies=exclude_external_dependencies,
```

### Comparing `tgwrap-0.5.3/tgwrap/printer.py` & `tgwrap-0.5.4/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.3/tgwrap/terrasafe.py` & `tgwrap-0.5.4/tgwrap/terrasafe.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.3/setup.py` & `tgwrap-0.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
-    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
+    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tgwrap-0.5.3/PKG-INFO` & `tgwrap-0.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.5.3
+Version: 0.5.4
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -115,14 +115,27 @@
 tgwrap output -- -json
 ```
 
 > Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:
 
 `tgwrap state mv 'azuread_group.this[\"viewers\"]' 'azuread_group.this[\"readers\"]'`
 
+## A word about escaping inputs
+
+Your shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.
+
+For example:
+
+```console
+# to exclude certain modules from an action (such as analyze):
+tgwrap analyze -E 'integrations/\*/\*'
+
+# to import a resource that has a " in its address:
+tgwrap import -a 'azuread_group.this[\"my_group\"]' -i ${GROUP_ID}
+```
 
 ## Deploy manifests
 
 In order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:
 
 ```yaml
 ---
```

