# Comparing `tmp/abilian_devtools-0.4.8.tar.gz` & `tmp/abilian_devtools-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abilian_devtools-0.4.8.tar", max compression
+gzip compressed data, was "abilian_devtools-0.4.9.tar", max compression
```

## Comparing `abilian_devtools-0.4.8.tar` & `abilian_devtools-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.4.8/LICENSES/
--rw-r--r--   0        0        0     3131 2023-01-05 08:09:53.677272 abilian_devtools-0.4.8/README.md
--rw-r--r--   0        0        0     3552 2023-02-13 13:43:13.964771 abilian_devtools-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.4.8/src/abilian_devtools/__init__.py
--rw-r--r--   0        0        0      705 2023-02-13 13:46:15.168299 abilian_devtools-0.4.8/src/abilian_devtools/invoke/__init__.py
--rw-r--r--   0        0        0     1346 2023-02-13 13:37:43.794616 abilian_devtools-0.4.8/src/abilian_devtools/invoke/help.py
--rw-r--r--   0        0        0      434 2023-02-13 13:05:06.275836 abilian_devtools-0.4.8/src/abilian_devtools/invoke/subrepos.py
--rw-r--r--   0        0        0     1386 2023-02-13 13:04:39.790057 abilian_devtools-0.4.8/src/abilian_devtools/invoke/versions.py
--rw-r--r--   0        0        0     1790 2023-02-13 13:06:20.879302 abilian_devtools-0.4.8/src/abilian_devtools/main.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 abilian_devtools-0.4.8/setup.py
--rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 abilian_devtools-0.4.8/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.4.9/LICENSES/
+-rw-r--r--   0        0        0     3131 2023-01-05 08:09:53.677272 abilian_devtools-0.4.9/README.md
+-rw-r--r--   0        0        0     3664 2023-02-16 08:35:45.764461 abilian_devtools-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.4.9/src/abilian_devtools/__init__.py
+-rw-r--r--   0        0        0      705 2023-02-13 13:46:15.168299 abilian_devtools-0.4.9/src/abilian_devtools/invoke/__init__.py
+-rw-r--r--   0        0        0     1439 2023-02-13 14:01:32.572788 abilian_devtools-0.4.9/src/abilian_devtools/invoke/help.py
+-rw-r--r--   0        0        0      434 2023-02-13 13:05:06.275836 abilian_devtools-0.4.9/src/abilian_devtools/invoke/subrepos.py
+-rw-r--r--   0        0        0     1386 2023-02-13 13:04:39.790057 abilian_devtools-0.4.9/src/abilian_devtools/invoke/versions.py
+-rw-r--r--   0        0        0     2336 2023-02-16 08:36:24.479478 abilian_devtools-0.4.9/src/abilian_devtools/main.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 abilian_devtools-0.4.9/setup.py
+-rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 abilian_devtools-0.4.9/PKG-INFO
```

### Comparing `abilian_devtools-0.4.8/README.md` & `abilian_devtools-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.4.8/pyproject.toml` & `abilian_devtools-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "abilian-devtools"
-version = "0.4.8"
+version = "0.4.9"
 description = "A curated set of dependencies for quality software development"
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "abilian_devtools", from = "src"}]
+packages = [{ include = "abilian_devtools", from = "src" }]
 repository = "https://github.com/abilian/abilian-devtools"
 keywords = ["qa", "testing", "linting", "typechecking", "security", "supply chain"]
 
 
 [tool.poetry.scripts]
 adt = "abilian_devtools.main:app"
 
@@ -94,15 +94,16 @@
 # Dependencies & supply chain
 deptry = "*"
 pip = "*"
 pip-audit = "*"
 reuse = "*"
 safety = "*"
 vulture = "*"
-# poetryup = "*"
+
+# Invoke
 invoke = "^2.0.0"
 tomlkit = "^0.11.6"
 
 
 [tool.poetry.group.dev.dependencies]
 scriv = "^1.2.0"
 docformatter = "^1.5.1"
@@ -170,18 +171,25 @@
     "vulture",
 ]
 
 [tool.scriv]
 version = "literal: pyproject.toml: tool.poetry.version"
 format = "md"
 categories = [
-  "Removed",
-  "Added",
-  "Changed",
-  "Deprecated",
-  "Fixed",
-  "Security",
-  "Doc",
+    "Removed",
+    "Added",
+    "Changed",
+    "Deprecated",
+    "Fixed",
+    "Security",
+    "Doc",
 ]
 
 
 [tool.pyright]
+
+
+[tool.bandit]
+skips = [
+    "B404", # blacklist
+    "B603", # subprocess_without_shell_equals_true
+]
```

### Comparing `abilian_devtools-0.4.8/src/abilian_devtools/invoke/__init__.py` & `abilian_devtools-0.4.9/src/abilian_devtools/invoke/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.4.8/src/abilian_devtools/invoke/help.py` & `abilian_devtools-0.4.9/src/abilian_devtools/invoke/help.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     """Helper to generate the `make help` message."""
     # TODO: should try harder to find the right file
     with Path("Makefile").open() as f:
         makefile = f.read()
 
     targets = MakefileParser().parse(makefile)
 
+    if not targets:
+        print("No documented targets found in Makefile")
+        return
+
     max_len = max(len(t[0]) for t in targets)
 
     print("Most interesting targets:\n")
     for targets, description in targets:
         print(f"  {targets:<{max_len}}   {description}")
```

### Comparing `abilian_devtools-0.4.8/src/abilian_devtools/invoke/versions.py` & `abilian_devtools-0.4.9/src/abilian_devtools/invoke/versions.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.4.8/src/abilian_devtools/main.py` & `abilian_devtools-0.4.9/src/abilian_devtools/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import typer
 
 app = typer.Typer()
 
 
 def run(cmd):
-    typer.secho(cmd, fg=typer.colors.GREEN)
+    typer.secho("> " + cmd, fg=typer.colors.GREEN)
     args = shlex.split(cmd)
     p = subprocess.Popen(args)
     p.wait()
     if p.returncode:
         typer.secho(f"failed with error code {p.returncode}", fg="red")
         # typer.secho(p.stderr)
         sys.exit()
@@ -42,21 +42,33 @@
     run("pyright")
     run(f"vulture --min-confidence 80 {args_str}")
     # TODO: currently broken
     # run("deptry .")
 
 
 @app.command("security-check")
-def security_check():
-    """Run security checks."""
-    run("pip-audit")
-    run("safety check")
+def security_check(ctx: typer.Context):
+    """Run security checks (deprecated, use 'audit' instead)."""
+    typer.secho(
+        "WARNING: 'security-check' is deprecated, use 'audit' instead.",
+        fg=typer.colors.RED,
+    )
+    ctx.invoke(audit)
+
 
+@app.command()
+def audit():
+    """Run security audit."""
+    run("pip-audit")
     # TODO: don't assume source dir is src
-    # run("bandit -r src")
+    run("bandit -q -c pyproject.toml -r src")
+    # TODO: suppress output on success
+    run("reuse lint")
+    # TODO: Don't run safety check for now, it's too noisy
+    # run("safety check")
 
 
 @app.command()
 def test():
     """Run tests."""
     run("pytest")
 
@@ -72,15 +84,19 @@
 def clean():
     """Cleanup cruft."""
     typer.echo("Removing cache directories")
     for cache_dir in glob.glob("**/__pycache__", recursive=True):
         shutil.rmtree(cache_dir)
 
 
-@app.callback()
-def main():
-    """Abilian Dev Tools command-line runner."""
-    # Nothing here yet
+@app.callback(invoke_without_command=True)
+def main(ctx: typer.Context):
+    """Abilian Dev Tools command-line runner.
+
+    Helps keeping your project clean and healthy.
+    """
+    if ctx.invoked_subcommand is None:
+        ctx.get_help()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `abilian_devtools-0.4.8/setup.py` & `abilian_devtools-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
  'vulture']
 
 entry_points = \
 {'console_scripts': ['adt = abilian_devtools.main:app']}
 
 setup_kwargs = {
     'name': 'abilian-devtools',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'A curated set of dependencies for quality software development',
     'long_description': "Abilian Development Tools\n=========================\n\nWhat this is?\n-------------\n\nThis is a curated, and opiniated, collection of best-of-breed Python development tools:\n\n- Formatters (`black`, `isort`, `docformatter`)\n- Testing frameworks (`pytest` and friends, `nox`)\n- Style checkers (`ruff`, `flake8` and friends)\n- Type checkers (`mypy`, `pyright`)\n- Supply chain audit (`pip-audit`, `safety`, `reuse`, `vulture`, `deptry`)\n- And more.\n\nUsage\n-----\n\nInstead of having to track all the 40+ projects and plugins we have curated, you just need to add `abilian-devtools = '*'` in your project's `requirements.in` or `pyproject.toml`.\n\nYou still need to properly configure and call them in your own projects.\n\nFor example configuration, see, for instance, <https://github.com/abilian/nua> (`Makefile`, `pyproject.toml`, `setup.cfg`).\n\nAs a bonus, we're providing a CLI called `adt` which can help you get started:\n\n```\n$ adt --help\nUsage: adt [OPTIONS] COMMAND [ARGS]...\n\nAbilian Dev Tool command-line runner.\n\n╭─ Options ────────────────────────────────────────────────────────────────────╮\n│ --install-completion        [bash|zsh|fish|powershe  Install completion for  │\n│                             ll|pwsh]                 the specified shell.    │\n│                                                      [default: None]         │\n│ --show-completion           [bash|zsh|fish|powershe  Show completion for the │\n│                             ll|pwsh]                 specified shell, to     │\n│                                                      copy it or customize    │\n│                                                      the installation.       │\n│                                                      [default: None]         │\n│ --help                                               Show this message and   │\n│                                                      exit.                   │\n╰──────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ───────────────────────────────────────────────────────────────────╮\n│ all               Run everything.                                            │\n│ check             Run checker/linters on specified files or directories.     │\n│ security-check    Run security checks.                                       │\n│ test              Run tests.                                                 │\n╰──────────────────────────────────────────────────────────────────────────────╯\n```\n",
     'author': 'Stefane Fermigier',
     'author_email': 'sf@abilian.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/abilian/abilian-devtools',
```

### Comparing `abilian_devtools-0.4.8/PKG-INFO` & `abilian_devtools-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abilian-devtools
-Version: 0.4.8
+Version: 0.4.9
 Summary: A curated set of dependencies for quality software development
 Home-page: https://github.com/abilian/abilian-devtools
 License: MIT
 Keywords: qa,testing,linting,typechecking,security,supply chain
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
```

