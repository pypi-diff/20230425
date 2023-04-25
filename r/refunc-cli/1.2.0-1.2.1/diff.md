# Comparing `tmp/refunc-cli-1.2.0.tar.gz` & `tmp/refunc-cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refunc-cli-1.2.0.tar", last modified: Mon Apr 24 06:56:47 2023, max compression
+gzip compressed data, was "refunc-cli-1.2.1.tar", last modified: Tue Apr 25 06:30:34 2023, max compression
```

## Comparing `refunc-cli-1.2.0.tar` & `refunc-cli-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 06:56:47.024816 refunc-cli-1.2.0/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-23 02:26:55.000000 refunc-cli-1.2.0/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-24 06:56:47.024816 refunc-cli-1.2.0/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-23 09:58:14.000000 refunc-cli-1.2.0/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 06:56:47.020816 refunc-cli-1.2.0/refunc_cli.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-24 06:56:46.000000 refunc-cli-1.2.0/refunc_cli.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-24 06:30:18.000000 refunc-cli-1.2.0/requirements.txt
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 06:56:47.024816 refunc-cli-1.2.0/rfctl/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-23 02:02:22.000000 refunc-cli-1.2.0/rfctl/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-24 02:41:18.000000 refunc-cli-1.2.0/rfctl/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-24 02:58:19.000000 refunc-cli-1.2.0/rfctl/awslocal.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3681 2023-04-23 06:58:17.000000 refunc-cli-1.2.0/rfctl/build.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 06:56:47.024816 refunc-cli-1.2.0/rfctl/client/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-24 06:37:09.000000 refunc-cli-1.2.0/rfctl/client/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1425 2023-04-24 06:31:46.000000 refunc-cli-1.2.0/rfctl/client/client.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      818 2023-04-24 02:57:03.000000 refunc-cli-1.2.0/rfctl/create.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-23 07:21:11.000000 refunc-cli-1.2.0/rfctl/create_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-23 07:14:35.000000 refunc-cli-1.2.0/rfctl/delete.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-23 07:21:59.000000 refunc-cli-1.2.0/rfctl/delete_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-23 07:28:56.000000 refunc-cli-1.2.0/rfctl/get.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-23 07:28:47.000000 refunc-cli-1.2.0/rfctl/get_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-24 06:51:06.000000 refunc-cli-1.2.0/rfctl/init.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      361 2023-04-24 06:43:33.000000 refunc-cli-1.2.0/rfctl/init_source.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-23 03:35:02.000000 refunc-cli-1.2.0/rfctl/schema.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      657 2023-04-24 02:56:46.000000 refunc-cli-1.2.0/rfctl/update_code.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-23 07:17:30.000000 refunc-cli-1.2.0/rfctl/update_config.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-24 06:56:47.024816 refunc-cli-1.2.0/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-24 06:32:20.000000 refunc-cli-1.2.0/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-23 02:26:55.000000 refunc-cli-1.2.1/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-23 09:58:14.000000 refunc-cli-1.2.1/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.556407 refunc-cli-1.2.1/refunc_cli.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-24 06:30:18.000000 refunc-cli-1.2.1/requirements.txt
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/rfctl/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-23 02:02:22.000000 refunc-cli-1.2.1/rfctl/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-24 02:41:18.000000 refunc-cli-1.2.1/rfctl/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-24 02:58:19.000000 refunc-cli-1.2.1/rfctl/awslocal.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-25 06:26:50.000000 refunc-cli-1.2.1/rfctl/build.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/rfctl/client/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-24 06:37:09.000000 refunc-cli-1.2.1/rfctl/client/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1425 2023-04-24 06:31:46.000000 refunc-cli-1.2.1/rfctl/client/client.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      841 2023-04-25 06:27:25.000000 refunc-cli-1.2.1/rfctl/create.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-23 07:21:11.000000 refunc-cli-1.2.1/rfctl/create_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-23 07:14:35.000000 refunc-cli-1.2.1/rfctl/delete.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-23 07:21:59.000000 refunc-cli-1.2.1/rfctl/delete_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-23 07:28:56.000000 refunc-cli-1.2.1/rfctl/get.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-23 07:28:47.000000 refunc-cli-1.2.1/rfctl/get_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-24 06:51:06.000000 refunc-cli-1.2.1/rfctl/init.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-25 06:20:52.000000 refunc-cli-1.2.1/rfctl/init_source.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-23 03:35:02.000000 refunc-cli-1.2.1/rfctl/schema.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-25 06:27:08.000000 refunc-cli-1.2.1/rfctl/update_code.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-23 07:17:30.000000 refunc-cli-1.2.1/rfctl/update_config.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-25 06:21:17.000000 refunc-cli-1.2.1/setup.py
```

### Comparing `refunc-cli-1.2.0/refunc_cli.egg-info/SOURCES.txt` & `refunc-cli-1.2.1/refunc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/__main__.py` & `refunc-cli-1.2.1/rfctl/__main__.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/awslocal.py` & `refunc-cli-1.2.1/rfctl/awslocal.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/build.py` & `refunc-cli-1.2.1/rfctl/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @click.command()
 @click.option('--out', default=os.path.join(os.getcwd(), "lambda.zip"), type=click.Path(exists=False, dir_okay=False, resolve_path=True))
 @click.pass_context
 def build_command(ctx: click.Context, out: str):
     do_build(ctx, out)
 
 
-def do_build(ctx: click.Context, out: str):
+def do_build(ctx: click.Context, out: str) -> bool:
     funcdef = ctx.obj["funcdef"]
     build = funcdef["spec"]["build"]
     capabilities = {
         "language": build["language"],
         "dependency_manager": get_dependency_manager(build["language"])
     }
     with tempfile.TemporaryDirectory() as tmp_dir:
@@ -79,9 +79,11 @@
             with zipfile.ZipFile(out, mode='w') as zip_file:
                 directory = os.path.join(tmp_dir, "lambda")
                 for root, _, files in os.walk(directory):
                     for file in files:
                         file_path = os.path.join(root, file)
                         zip_file.write(file_path, os.path.relpath(file_path, directory))
             ctx.obj["out"] = out
+            return True
         except Exception as ex:
             click.echo("Build error:\n %s" % traceback.format_exc())
+            return False
```

### Comparing `refunc-cli-1.2.0/rfctl/client/client.py` & `refunc-cli-1.2.1/rfctl/client/client.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/create.py` & `refunc-cli-1.2.1/rfctl/create.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 
 @click.command()
 @click.pass_context
 def create_command(ctx: click.Context):
     funcdef = ctx.obj["funcdef"]
     out = os.path.join(ctx.obj["working_dir"], "lambda.zip")
-    do_build(ctx, out)
+    if not do_build(ctx, out):
+        return
     click.echo("Creating function %s/%s" % (funcdef["metadata"]["namespace"], funcdef["metadata"]["name"]))
     lambda_args = ["create-function",
                    "--function-name", funcdef["metadata"]["name"],
                    "--handler", funcdef["spec"]["handler"],
                    "--zip-file", "fileb://{}".format(out),
                    "--runtime", funcdef["spec"]["runtime"],
                    "--timeout", funcdef["spec"]["timeout"]]
```

### Comparing `refunc-cli-1.2.0/rfctl/init.py` & `refunc-cli-1.2.1/rfctl/init.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/schema.py` & `refunc-cli-1.2.1/rfctl/schema.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/rfctl/update_code.py` & `refunc-cli-1.2.1/rfctl/update_code.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 @click.command()
 @click.pass_context
 def update_code_command(ctx: click.Context):
     funcdef = ctx.obj["funcdef"]
     out = os.path.join(ctx.obj["working_dir"], "lambda.zip")
-    do_build(ctx, out)
+    if not do_build(ctx, out):
+        return
     click.echo("Updating code for function %s/%s" % (funcdef["metadata"]["namespace"], funcdef["metadata"]["name"]))
     lambda_args = ["update-function-code",
                    "--function-name", funcdef["metadata"]["name"],
                    "--zip-file", "fileb://{}".format(out)]
     lambda_command(ctx.obj["endpoint"], lambda_args)
     os.remove(out)
```

### Comparing `refunc-cli-1.2.0/rfctl/update_config.py` & `refunc-cli-1.2.1/rfctl/update_config.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.0/setup.py` & `refunc-cli-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='refunc-cli',
-    version='1.2.0',
+    version='1.2.1',
     description='refunc command line tools',
     author='arvin',
     license='MIT',
     url='https://github.com/refunc/refunc-cli',
     author_email='arvintian8@gamil.com',
     packages=find_packages(),
     include_package_data=True,
```

