# Comparing `tmp/streamline-1.0.5.tar.gz` & `tmp/streamline-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/streamline-1.0.5.tar", last modified: Sat Feb 29 23:10:22 2020, max compression
+gzip compressed data, was "streamline-1.1.0.tar", last modified: Tue Apr 25 09:17:14 2023, max compression
```

## Comparing `streamline-1.0.5.tar` & `streamline-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-02-29 23:10:22.000000 streamline-1.0.5/
--rw-r--r--   0 kj         (501) staff       (20)    12186 2020-02-29 23:10:22.000000 streamline-1.0.5/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)     9548 2019-11-24 04:49:20.000000 streamline-1.0.5/README.md
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-02-29 23:10:22.000000 streamline-1.0.5/bin/
--rwxr-xr-x   0 kj         (501) staff       (20)      146 2019-11-24 04:49:20.000000 streamline-1.0.5/bin/streamline
--rw-r--r--   0 kj         (501) staff       (20)       38 2020-02-29 23:10:22.000000 streamline-1.0.5/setup.cfg
--rw-r--r--   0 kj         (501) staff       (20)      722 2020-02-29 23:09:35.000000 streamline-1.0.5/setup.py
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-02-29 23:10:22.000000 streamline-1.0.5/streamline/
--rw-r--r--   0 kj         (501) staff       (20)        1 2019-11-24 04:49:20.000000 streamline-1.0.5/streamline/__init__.py
--rw-r--r--   0 kj         (501) staff       (20)    11164 2019-11-24 05:14:44.000000 streamline-1.0.5/streamline/cli.py
--rw-r--r--   0 kj         (501) staff       (20)     5110 2019-11-24 04:49:20.000000 streamline-1.0.5/streamline/consumers.py
--rw-r--r--   0 kj         (501) staff       (20)     1421 2019-11-24 04:49:20.000000 streamline-1.0.5/streamline/core.py
--rw-r--r--   0 kj         (501) staff       (20)     1846 2020-02-29 06:52:51.000000 streamline-1.0.5/streamline/entries.py
--rw-r--r--   0 kj         (501) staff       (20)    16157 2020-02-29 23:06:03.000000 streamline-1.0.5/streamline/executors.py
--rw-r--r--   0 kj         (501) staff       (20)     2256 2019-11-24 04:49:20.000000 streamline-1.0.5/streamline/extractor.py
--rw-r--r--   0 kj         (501) staff       (20)     4404 2019-11-24 04:49:20.000000 streamline-1.0.5/streamline/generators.py
--rw-r--r--   0 kj         (501) staff       (20)    25990 2020-02-29 06:55:22.000000 streamline-1.0.5/streamline/streamers.py
--rw-r--r--   0 kj         (501) staff       (20)     2320 2019-11-24 04:56:05.000000 streamline-1.0.5/streamline/utils.py
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-02-29 23:10:22.000000 streamline-1.0.5/streamline.egg-info/
--rw-r--r--   0 kj         (501) staff       (20)    12186 2020-02-29 23:10:21.000000 streamline-1.0.5/streamline.egg-info/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)      425 2020-02-29 23:10:22.000000 streamline-1.0.5/streamline.egg-info/SOURCES.txt
--rw-r--r--   0 kj         (501) staff       (20)        1 2020-02-29 23:10:21.000000 streamline-1.0.5/streamline.egg-info/dependency_links.txt
--rw-r--r--   0 kj         (501) staff       (20)        7 2020-02-29 23:10:21.000000 streamline-1.0.5/streamline.egg-info/requires.txt
--rw-r--r--   0 kj         (501) staff       (20)       11 2020-02-29 23:10:21.000000 streamline-1.0.5/streamline.egg-info/top_level.txt
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.103753 streamline-1.1.0/
+-rw-r--r--   0 kj         (501) staff       (20)     9975 2023-04-25 09:17:14.103521 streamline-1.1.0/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)     9548 2023-04-25 08:36:21.000000 streamline-1.1.0/README.md
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.101410 streamline-1.1.0/bin/
+-rwxr-xr-x   0 kj         (501) staff       (20)      146 2023-04-25 08:36:21.000000 streamline-1.1.0/bin/streamline
+-rw-r--r--   0 kj         (501) staff       (20)       38 2023-04-25 09:17:14.103804 streamline-1.1.0/setup.cfg
+-rw-r--r--   0 kj         (501) staff       (20)      722 2023-04-25 08:36:31.000000 streamline-1.1.0/setup.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.102640 streamline-1.1.0/streamline/
+-rw-r--r--   0 kj         (501) staff       (20)        1 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/__init__.py
+-rw-r--r--   0 kj         (501) staff       (20)    11164 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/cli.py
+-rw-r--r--   0 kj         (501) staff       (20)     5110 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/consumers.py
+-rw-r--r--   0 kj         (501) staff       (20)     1421 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/core.py
+-rw-r--r--   0 kj         (501) staff       (20)     1846 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/entries.py
+-rw-r--r--   0 kj         (501) staff       (20)    16679 2023-04-25 09:08:43.000000 streamline-1.1.0/streamline/executors.py
+-rw-r--r--   0 kj         (501) staff       (20)     2256 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/extractor.py
+-rw-r--r--   0 kj         (501) staff       (20)     4404 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/generators.py
+-rw-r--r--   0 kj         (501) staff       (20)    25990 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/streamers.py
+-rw-r--r--   0 kj         (501) staff       (20)     2320 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/utils.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.103258 streamline-1.1.0/streamline.egg-info/
+-rw-r--r--   0 kj         (501) staff       (20)     9975 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)      425 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/SOURCES.txt
+-rw-r--r--   0 kj         (501) staff       (20)        1 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/dependency_links.txt
+-rw-r--r--   0 kj         (501) staff       (20)        7 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/requires.txt
+-rw-r--r--   0 kj         (501) staff       (20)       11 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `streamline-1.0.5/PKG-INFO` & `streamline-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,289 +1,291 @@
 Metadata-Version: 2.1
 Name: streamline
-Version: 1.0.5
+Version: 1.1.0
 Summary: CLI tool for doing async tasks and transformations
 Home-page: https://github.com/jdotpy/streamline
 Author: KJ
 Author-email: jdotpy@users.noreply.github.com
 License: UNKNOWN
 Download-URL: https://github.com/jdotpy/streamline/tarball/master
-Description: streamline
-        ============
-        
-        The goal of this project is to make data acessible and actionable on the CLI. Streamline does this by implementing the utility functions necessary for taking an input stream and parallelizing work done on it.
-        
-        The sequence of operations in an invocation:
-        
-        1. The "Generator" object loads entries from a source data stream (usually stdin).
-        2. The "Streamers" selected are sequentially given each input value and are exepcted to filter and make modifications to those values and yield them for the next streamer.
-        3. The "Consumer" object takes the entries yielded from the last streamer and usually outputs them for storage or viewing (usually stdout).
-        
-        ## Installation
-        
-        * Requires Python 3.6+ and pip
-        * `pip install streamline`
-        
-        ## Guide
-        
-        The simplest call specifies no streaming operations it just reads from stdin and writes to stdout exactly what was written:
-        
-        ```bash
-          $ printf "foo\nbar" | streamline
-          foo
-          bar
-        ```
-        
-        By default streamline takes input from stdin and writes to stdout. This is very flexible as it makes the tool composible with other CLI tools. However you can also use the `--input` and `--output` flags to control output. Lets assume that you have a file with the same data you just sent in with printf:
-        
-        ```bash
-          $ streamline --input my_source_file.txt --output my_target_file.txt
-          $ cat my_target_file.txt
-          foo
-          bar
-        ```
-        
-        Now lets do something a little less useless. Lets use the "shell" streamer to execute a shell command for each entry and check if they're listening for https traffic:
-        
-        ```bash
-          $ printf "www.google.com\nslashdot.org" | streamline -s shell -- "nc -zv {value} 443"
-          {"stdout": "", "stderr": "Connection to www.google.com 443 port [tcp/https] succeeded!\n", "exit_code": 0}
-          {"stdout": "", "stderr": "Connection to slashdot.org 443 port [tcp/https] succeeded!\n", "exit_code": 0}
-        ```
-        
-        Streamline modules aim to provide all the useful information in object form as output can then be customized with other streaming modules. For exampe, to take the above output and get just the exit code that tells us whether the port is open we can just add the `headers` streamer to prefix each output with the original input and the `extract` streamer (with its `--selector` option) option to set the value to the `exit_code` property of each result:
-        
-        ```bash
-          $ printf "www.google.com\nslashdot.org" | streamline -s shell extract headers -- "nc -zv {value} 443" --selector exit_code
-          www.google.com: 0
-          slashdot.org: 0
-        ```
-        
-        ## Built-in Modules
-        
-        There are many modules available that do asynchronous jobs and transformations to input.  To see all available modules use the main help option to list them with examples:
-        
-        ```bash
-        $ streamline --help
-        
-        =============== Streamline ===============
-        
-        
-        usage: streamline [--generator GENERATOR] [--consumer CONSUMER]
-                          [-s [STREAMERS [STREAMERS ...]]] [-h]
-        
-        optional arguments:
-          --generator GENERATOR
-                                Entry Generator Module
-          --consumer CONSUMER   Entry Consumer/Writer Module
-          -s [STREAMERS [STREAMERS ...]], --streamers [STREAMERS [STREAMERS ...]]
-                                Additional streamers to apply (-s is optional)
-          -h, --help            Print help
-          -p {buffer,stream-output,streaming}, --progress {buffer,stream-output,streaming}
-                                Print progress to stdout. ("buffer": buffers input and
-                                output, "stream-output" buffers only input, "stream"
-                                for no buffering at all)
-          -w WORKERS, --workers WORKERS
-                                Number of concurrent workers for any one async
-                                execution module to have
-        
-        
-        
-        =============== Streamers ===============
-        
-        ::extract::
-        	Description: Change the value to an attribute of the current value
-        	Example: streamline -s extract -- --selector exit_code
-        
-        ::py::
-        	Description: Translate each value by assigning it to the result of a python expression
-        	Example: streamline -s py -- "value.upper()"
-        
-        ::pyfilter::
-        	Description: Filter out values that dont have a truthy result to a particular python expression
-        	Example: streamline -s pyfilter -- "'foobar' in value"
-        
-        ::truthy::
-        	Description: Filter out values that are not truthy
-        	Example: streamline -s truthy -- 
-        
-        ::noop::
-        	Description: No operation. Just for testing.
-        	Example: streamline -s noop -- 
-        
-        ::split_list::
-        	Description: Take any values that are an array and treat each value of an array as a separate input 
-        	Example: streamline -s split_list -- 
-        
-        ::split::
-        	Description: Take any values that are an array and treat each value of an array as a separate input 
-        	Example: streamline -s split -- 
-        
-        ::breakdown::
-        	Description: Show a report of how many input values ended up with a particular result value
-        	Example: streamline -s breakdown -- 
-        
-        ::headers::
-        	Description: Force each value to a string and prefix each with the original input value
-        	Example: streamline -s headers -- 
-        
-        ::filter_out_errors::
-        	Description: Filter out any entries that have produced an error
-        	Example: streamline -s filter_out_errors -- 
-        
-        ::errors::
-        	Description: Use the latest error on the entry as the value
-        	Example: streamline -s errors -- 
-        
-        ::buffer::
-        	Description: Hold entries in memory until a certain number is reached (give no args to buffer all)
-        	Example: streamline -s buffer -- --buffer 20
-        
-        ::json::
-        	Description: Take json strings and parse them into objects so other streamers can inspect attributes
-        	Example: streamline -s json -- 
-        
-        ::strip::
-        	Description: Strip surrounding whitespace from each string entry, removing entries that are only whitespace
-        	Example: streamline -s strip -- --buffer 20
-        
-        ::head::
-        	Description: Only take the first X entries (Default 1)
-        	Example: streamline -s head -- --count 20
-        
-        ::readfile::
-        	Description: Read the file indicated by the file
-        	Example: streamline -s readfile -- --path ~/dir/{value}.json
-        
-        ::combine::
-        	Description: Combine two previous historical values by setting an attribute
-        	Example: streamline -s combine -- --source "-1" --target "-2"
-        
-        ::http::
-        	Description: Use a template to execute an HTTP request for each value
-        	Example: streamline -s http -- "https://{value}/"
-        
-        ::ssh::
-        	Description: Treat each value as a host to connect to. SSH in and run a command returning the output
-        	Example: streamline -s ssh -- "uptime"
-        
-        ::ssh_exec::
-        	Description: Copy a script to target machine and execute
-        	Example: streamline -s ssh_exec -- ~/dostuff.sh
-        
-        ::shell::
-        	Description: Run a shell command for each value
-        	Example: streamline -s shell -- "nc -zv {value} 22"
-        
-        ::scp::
-        	Description: Treat each value as a host to connect to. Copy a file to or from this host
-        	Example: streamline -s scp -- "/tmp/file.txt" "{value}:/tmp/file.txt"
-        
-        ::sleep::
-        	Description: Sleep for a second (or for {value} seconds) for each entry making no change to its value
-        	Example: streamline -s sleep -- 
-        
-        ::history:push::
-        	Description: Start a new history tree
-        	Example: streamline -s history:push -- 
-        
-        ::history:pop::
-        	Description: Walk back up one level in the history tree
-        	Example: streamline -s history:pop -- 
-        
-        ::history:collapse::
-        	Description: Treat the latest value as the original
-        	Example: streamline -s history:collapse -- 
-        
-        ::history:reset::
-        	Description: Clear all levels of history
-        	Example: streamline -s history:reset -- 
-        
-        ::history:values::
-        	Description: Set the current value to a list of all previous values
-        	Example: streamline -s history:values -- 
-        
-        ```
-        
-        To get available options for a particular module run (substituting "http" for the module you're interested in):
-        
-        ```bash
-        streamline -s http --help
-        ```
-        
-        
-        ## YAML support
-        
-        YAML files defining the streamers and their options is supported. 
-        
-        Given the following yaml file:
-        
-        ```yaml
-        streamers:
-         -
-            name: split
-         -
-            name: http
-            output: code
-            input: value
-            target: status_code
-            options:
-              url: 'https://{value}'`
-        ```
-        
-        It could be used to split a string of domains and get the http code for each one:
-        
-        ```bash
-        $ echo "www.google.com www.slashdot.org" | streamline -y http_codes.yaml
-        {"base": "www.google.com", "status_code": 200}
-        {"base": "www.slashdot.org", "status_code": 200}
-        ```
-        
-        
-        
-        You can also specify the generator and consumer in the same way. Given the below yaml and csv file:
-        ```yaml
-        generator:
-          name: csv
-          options:
-            input: domains.csv
-        consumer:
-          name: csv
-        streamers:
-          -
-             name: http
-             output: code
-             input: domain
-             target: status_code
-             options:
-               url: 'https://{value}'
-        ```
-        
-        ```
-        domain,label
-        www.google.com,The famous big B
-        www.slashdot.org,Mosh pit of opinions
-        ```
-        
-        You can use it the following way:
-        ```bash
-        $ streamline -y http_codes.yaml 
-        domain,label,status_code
-        www.google.com,The famous big B,200
-        www.slashdot.org,Mosh pit of opinions,200
-        ```
-        
-        
-        
-        ## Technical Vocabulary
-        
-        * Entry: A small wrapper around a value being passed along through the stream. Commonly a single line of input.
-        * Generator: An asynchonous generator function that takes no input and yields Entry objects.
-        * Executor:  An asyncronous function that takes a single value and returns a new value. Usually some unit of work is done and the result of that work is returned as the new value.
-        * Streamer: An asynchronous generator function that takes as an argument an asynchronous source iterable that yields Entry objects. Commonly streamers do some manipulation of each Entry it gets from the source iterable and then sets a new value on the entry.
-        * Consumer: An asynchronous function that reads all entries of an asynchronous source iterable. Usually this function writes to some output (such as stdout).
-        
-        
 Keywords: tools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+streamline
+============
+
+The goal of this project is to make data acessible and actionable on the CLI. Streamline does this by implementing the utility functions necessary for taking an input stream and parallelizing work done on it.
+
+The sequence of operations in an invocation:
+
+1. The "Generator" object loads entries from a source data stream (usually stdin).
+2. The "Streamers" selected are sequentially given each input value and are exepcted to filter and make modifications to those values and yield them for the next streamer.
+3. The "Consumer" object takes the entries yielded from the last streamer and usually outputs them for storage or viewing (usually stdout).
+
+## Installation
+
+* Requires Python 3.6+ and pip
+* `pip install streamline`
+
+## Guide
+
+The simplest call specifies no streaming operations it just reads from stdin and writes to stdout exactly what was written:
+
+```bash
+  $ printf "foo\nbar" | streamline
+  foo
+  bar
+```
+
+By default streamline takes input from stdin and writes to stdout. This is very flexible as it makes the tool composible with other CLI tools. However you can also use the `--input` and `--output` flags to control output. Lets assume that you have a file with the same data you just sent in with printf:
+
+```bash
+  $ streamline --input my_source_file.txt --output my_target_file.txt
+  $ cat my_target_file.txt
+  foo
+  bar
+```
+
+Now lets do something a little less useless. Lets use the "shell" streamer to execute a shell command for each entry and check if they're listening for https traffic:
+
+```bash
+  $ printf "www.google.com\nslashdot.org" | streamline -s shell -- "nc -zv {value} 443"
+  {"stdout": "", "stderr": "Connection to www.google.com 443 port [tcp/https] succeeded!\n", "exit_code": 0}
+  {"stdout": "", "stderr": "Connection to slashdot.org 443 port [tcp/https] succeeded!\n", "exit_code": 0}
+```
+
+Streamline modules aim to provide all the useful information in object form as output can then be customized with other streaming modules. For exampe, to take the above output and get just the exit code that tells us whether the port is open we can just add the `headers` streamer to prefix each output with the original input and the `extract` streamer (with its `--selector` option) option to set the value to the `exit_code` property of each result:
+
+```bash
+  $ printf "www.google.com\nslashdot.org" | streamline -s shell extract headers -- "nc -zv {value} 443" --selector exit_code
+  www.google.com: 0
+  slashdot.org: 0
+```
+
+## Built-in Modules
+
+There are many modules available that do asynchronous jobs and transformations to input.  To see all available modules use the main help option to list them with examples:
+
+```bash
+$ streamline --help
+
+=============== Streamline ===============
+
+
+usage: streamline [--generator GENERATOR] [--consumer CONSUMER]
+                  [-s [STREAMERS [STREAMERS ...]]] [-h]
+
+optional arguments:
+  --generator GENERATOR
+                        Entry Generator Module
+  --consumer CONSUMER   Entry Consumer/Writer Module
+  -s [STREAMERS [STREAMERS ...]], --streamers [STREAMERS [STREAMERS ...]]
+                        Additional streamers to apply (-s is optional)
+  -h, --help            Print help
+  -p {buffer,stream-output,streaming}, --progress {buffer,stream-output,streaming}
+                        Print progress to stdout. ("buffer": buffers input and
+                        output, "stream-output" buffers only input, "stream"
+                        for no buffering at all)
+  -w WORKERS, --workers WORKERS
+                        Number of concurrent workers for any one async
+                        execution module to have
+
+
+
+=============== Streamers ===============
+
+::extract::
+	Description: Change the value to an attribute of the current value
+	Example: streamline -s extract -- --selector exit_code
+
+::py::
+	Description: Translate each value by assigning it to the result of a python expression
+	Example: streamline -s py -- "value.upper()"
+
+::pyfilter::
+	Description: Filter out values that dont have a truthy result to a particular python expression
+	Example: streamline -s pyfilter -- "'foobar' in value"
+
+::truthy::
+	Description: Filter out values that are not truthy
+	Example: streamline -s truthy -- 
+
+::noop::
+	Description: No operation. Just for testing.
+	Example: streamline -s noop -- 
+
+::split_list::
+	Description: Take any values that are an array and treat each value of an array as a separate input 
+	Example: streamline -s split_list -- 
+
+::split::
+	Description: Take any values that are an array and treat each value of an array as a separate input 
+	Example: streamline -s split -- 
+
+::breakdown::
+	Description: Show a report of how many input values ended up with a particular result value
+	Example: streamline -s breakdown -- 
+
+::headers::
+	Description: Force each value to a string and prefix each with the original input value
+	Example: streamline -s headers -- 
+
+::filter_out_errors::
+	Description: Filter out any entries that have produced an error
+	Example: streamline -s filter_out_errors -- 
+
+::errors::
+	Description: Use the latest error on the entry as the value
+	Example: streamline -s errors -- 
+
+::buffer::
+	Description: Hold entries in memory until a certain number is reached (give no args to buffer all)
+	Example: streamline -s buffer -- --buffer 20
+
+::json::
+	Description: Take json strings and parse them into objects so other streamers can inspect attributes
+	Example: streamline -s json -- 
+
+::strip::
+	Description: Strip surrounding whitespace from each string entry, removing entries that are only whitespace
+	Example: streamline -s strip -- --buffer 20
+
+::head::
+	Description: Only take the first X entries (Default 1)
+	Example: streamline -s head -- --count 20
+
+::readfile::
+	Description: Read the file indicated by the file
+	Example: streamline -s readfile -- --path ~/dir/{value}.json
+
+::combine::
+	Description: Combine two previous historical values by setting an attribute
+	Example: streamline -s combine -- --source "-1" --target "-2"
+
+::http::
+	Description: Use a template to execute an HTTP request for each value
+	Example: streamline -s http -- "https://{value}/"
+
+::ssh::
+	Description: Treat each value as a host to connect to. SSH in and run a command returning the output
+	Example: streamline -s ssh -- "uptime"
+
+::ssh_exec::
+	Description: Copy a script to target machine and execute
+	Example: streamline -s ssh_exec -- ~/dostuff.sh
+
+::shell::
+	Description: Run a shell command for each value
+	Example: streamline -s shell -- "nc -zv {value} 22"
+
+::scp::
+	Description: Treat each value as a host to connect to. Copy a file to or from this host
+	Example: streamline -s scp -- "/tmp/file.txt" "{value}:/tmp/file.txt"
+
+::sleep::
+	Description: Sleep for a second (or for {value} seconds) for each entry making no change to its value
+	Example: streamline -s sleep -- 
+
+::history:push::
+	Description: Start a new history tree
+	Example: streamline -s history:push -- 
+
+::history:pop::
+	Description: Walk back up one level in the history tree
+	Example: streamline -s history:pop -- 
+
+::history:collapse::
+	Description: Treat the latest value as the original
+	Example: streamline -s history:collapse -- 
+
+::history:reset::
+	Description: Clear all levels of history
+	Example: streamline -s history:reset -- 
+
+::history:values::
+	Description: Set the current value to a list of all previous values
+	Example: streamline -s history:values -- 
+
+```
+
+To get available options for a particular module run (substituting "http" for the module you're interested in):
+
+```bash
+streamline -s http --help
+```
+
+
+## YAML support
+
+YAML files defining the streamers and their options is supported. 
+
+Given the following yaml file:
+
+```yaml
+streamers:
+ -
+    name: split
+ -
+    name: http
+    output: code
+    input: value
+    target: status_code
+    options:
+      url: 'https://{value}'`
+```
+
+It could be used to split a string of domains and get the http code for each one:
+
+```bash
+$ echo "www.google.com www.slashdot.org" | streamline -y http_codes.yaml
+{"base": "www.google.com", "status_code": 200}
+{"base": "www.slashdot.org", "status_code": 200}
+```
+
+
+
+You can also specify the generator and consumer in the same way. Given the below yaml and csv file:
+```yaml
+generator:
+  name: csv
+  options:
+    input: domains.csv
+consumer:
+  name: csv
+streamers:
+  -
+     name: http
+     output: code
+     input: domain
+     target: status_code
+     options:
+       url: 'https://{value}'
+```
+
+```
+domain,label
+www.google.com,The famous big B
+www.slashdot.org,Mosh pit of opinions
+```
+
+You can use it the following way:
+```bash
+$ streamline -y http_codes.yaml 
+domain,label,status_code
+www.google.com,The famous big B,200
+www.slashdot.org,Mosh pit of opinions,200
+```
+
+
+
+## Technical Vocabulary
+
+* Entry: A small wrapper around a value being passed along through the stream. Commonly a single line of input.
+* Generator: An asynchonous generator function that takes no input and yields Entry objects.
+* Executor:  An asyncronous function that takes a single value and returns a new value. Usually some unit of work is done and the result of that work is returned as the new value.
+* Streamer: An asynchronous generator function that takes as an argument an asynchronous source iterable that yields Entry objects. Commonly streamers do some manipulation of each Entry it gets from the source iterable and then sets a new value on the entry.
+* Consumer: An asynchronous function that reads all entries of an asynchronous source iterable. Usually this function writes to some output (such as stdout).
+
+
+
```

### Comparing `streamline-1.0.5/README.md` & `streamline-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/setup.py` & `streamline-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = 'streamline',
     scripts=['bin/streamline'],
     packages=['streamline'],
-    version = '1.0.5',
+    version = '1.1.0',
     description = 'CLI tool for doing async tasks and transformations',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'KJ',
     author_email = 'jdotpy@users.noreply.github.com',
     url = 'https://github.com/jdotpy/streamline',
     download_url = 'https://github.com/jdotpy/streamline/tarball/master',
```

### Comparing `streamline-1.0.5/streamline/cli.py` & `streamline-1.1.0/streamline/cli.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/consumers.py` & `streamline-1.1.0/streamline/consumers.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/core.py` & `streamline-1.1.0/streamline/core.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/entries.py` & `streamline-1.1.0/streamline/entries.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/executors.py` & `streamline-1.1.0/streamline/executors.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,19 @@
         # Hook for other things
         self.initialize()
 
     def initialize(self):
         pass
 
     async def handle(self, value):
-        async with asyncssh.connect(value.strip(), **self.connection_options) as conn:
+        connection_options = dict(self.connection_options)
+        username = self.options.get('username', None)
+        if username:
+            connection_options['username'] = username
+        async with asyncssh.connect(value.strip(), **connection_options) as conn:
             return await self.handle_connection(conn, value)
 
 @arg_help('Treat each value as a host to connect to. Copy a file to or from this host', example='"/tmp/file.txt" "{value}:/tmp/file.txt"')
 class ScpHandler(BaseAsyncSSHHandler):
     async_handler = True
 
     @classmethod
@@ -175,14 +179,18 @@
             help='Sudo as user'
         )
         parser.add_argument(
             '--stream-output',
             help='Where to stream output to (default is to return stdout)'
         )
         parser.add_argument(
+            '--username',
+            help='Username for SSH connection',
+        )
+        parser.add_argument(
             '--stream-append',
             default=False,
             action='store_true',
             help='Append to streaming output instead of overwriting'
         )
 
     async def handle_connection(self, conn, value):
@@ -247,14 +255,18 @@
             '--sudo',
             nargs='?',
             default=cls.NO_SUDO,
             dest='as_user',
             help='Sudo as user'
         )
         parser.add_argument(
+            '--username',
+            help='Username for SSH connection',
+        )
+        parser.add_argument(
             '--var',
             action='append',
             dest='var',
             help='Environment variables to set for the session (e.g. KEY=VALUE or KEY to pass from current env)'
         )
         parser.add_argument(
             '--command',
@@ -347,14 +359,18 @@
             '--sudo',
             nargs='?',
             default=cls.NO_SUDO,
             dest='as_user',
             help='Sudo as user'
         )
         parser.add_argument(
+            '--username',
+            help='Username for SSH connection',
+        )
+        parser.add_argument(
             '--var',
             action='append',
             dest='var',
             help='Environment variables to set for the session (e.g. KEY=VALUE or KEY to pass from current env)'
         )
         parser.add_argument(
             '--stream-output',
```

### Comparing `streamline-1.0.5/streamline/extractor.py` & `streamline-1.1.0/streamline/extractor.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/generators.py` & `streamline-1.1.0/streamline/generators.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/streamers.py` & `streamline-1.1.0/streamline/streamers.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline/utils.py` & `streamline-1.1.0/streamline/utils.py`

 * *Files identical despite different names*

### Comparing `streamline-1.0.5/streamline.egg-info/PKG-INFO` & `streamline-1.1.0/streamline.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,289 +1,291 @@
 Metadata-Version: 2.1
 Name: streamline
-Version: 1.0.5
+Version: 1.1.0
 Summary: CLI tool for doing async tasks and transformations
 Home-page: https://github.com/jdotpy/streamline
 Author: KJ
 Author-email: jdotpy@users.noreply.github.com
 License: UNKNOWN
 Download-URL: https://github.com/jdotpy/streamline/tarball/master
-Description: streamline
-        ============
-        
-        The goal of this project is to make data acessible and actionable on the CLI. Streamline does this by implementing the utility functions necessary for taking an input stream and parallelizing work done on it.
-        
-        The sequence of operations in an invocation:
-        
-        1. The "Generator" object loads entries from a source data stream (usually stdin).
-        2. The "Streamers" selected are sequentially given each input value and are exepcted to filter and make modifications to those values and yield them for the next streamer.
-        3. The "Consumer" object takes the entries yielded from the last streamer and usually outputs them for storage or viewing (usually stdout).
-        
-        ## Installation
-        
-        * Requires Python 3.6+ and pip
-        * `pip install streamline`
-        
-        ## Guide
-        
-        The simplest call specifies no streaming operations it just reads from stdin and writes to stdout exactly what was written:
-        
-        ```bash
-          $ printf "foo\nbar" | streamline
-          foo
-          bar
-        ```
-        
-        By default streamline takes input from stdin and writes to stdout. This is very flexible as it makes the tool composible with other CLI tools. However you can also use the `--input` and `--output` flags to control output. Lets assume that you have a file with the same data you just sent in with printf:
-        
-        ```bash
-          $ streamline --input my_source_file.txt --output my_target_file.txt
-          $ cat my_target_file.txt
-          foo
-          bar
-        ```
-        
-        Now lets do something a little less useless. Lets use the "shell" streamer to execute a shell command for each entry and check if they're listening for https traffic:
-        
-        ```bash
-          $ printf "www.google.com\nslashdot.org" | streamline -s shell -- "nc -zv {value} 443"
-          {"stdout": "", "stderr": "Connection to www.google.com 443 port [tcp/https] succeeded!\n", "exit_code": 0}
-          {"stdout": "", "stderr": "Connection to slashdot.org 443 port [tcp/https] succeeded!\n", "exit_code": 0}
-        ```
-        
-        Streamline modules aim to provide all the useful information in object form as output can then be customized with other streaming modules. For exampe, to take the above output and get just the exit code that tells us whether the port is open we can just add the `headers` streamer to prefix each output with the original input and the `extract` streamer (with its `--selector` option) option to set the value to the `exit_code` property of each result:
-        
-        ```bash
-          $ printf "www.google.com\nslashdot.org" | streamline -s shell extract headers -- "nc -zv {value} 443" --selector exit_code
-          www.google.com: 0
-          slashdot.org: 0
-        ```
-        
-        ## Built-in Modules
-        
-        There are many modules available that do asynchronous jobs and transformations to input.  To see all available modules use the main help option to list them with examples:
-        
-        ```bash
-        $ streamline --help
-        
-        =============== Streamline ===============
-        
-        
-        usage: streamline [--generator GENERATOR] [--consumer CONSUMER]
-                          [-s [STREAMERS [STREAMERS ...]]] [-h]
-        
-        optional arguments:
-          --generator GENERATOR
-                                Entry Generator Module
-          --consumer CONSUMER   Entry Consumer/Writer Module
-          -s [STREAMERS [STREAMERS ...]], --streamers [STREAMERS [STREAMERS ...]]
-                                Additional streamers to apply (-s is optional)
-          -h, --help            Print help
-          -p {buffer,stream-output,streaming}, --progress {buffer,stream-output,streaming}
-                                Print progress to stdout. ("buffer": buffers input and
-                                output, "stream-output" buffers only input, "stream"
-                                for no buffering at all)
-          -w WORKERS, --workers WORKERS
-                                Number of concurrent workers for any one async
-                                execution module to have
-        
-        
-        
-        =============== Streamers ===============
-        
-        ::extract::
-        	Description: Change the value to an attribute of the current value
-        	Example: streamline -s extract -- --selector exit_code
-        
-        ::py::
-        	Description: Translate each value by assigning it to the result of a python expression
-        	Example: streamline -s py -- "value.upper()"
-        
-        ::pyfilter::
-        	Description: Filter out values that dont have a truthy result to a particular python expression
-        	Example: streamline -s pyfilter -- "'foobar' in value"
-        
-        ::truthy::
-        	Description: Filter out values that are not truthy
-        	Example: streamline -s truthy -- 
-        
-        ::noop::
-        	Description: No operation. Just for testing.
-        	Example: streamline -s noop -- 
-        
-        ::split_list::
-        	Description: Take any values that are an array and treat each value of an array as a separate input 
-        	Example: streamline -s split_list -- 
-        
-        ::split::
-        	Description: Take any values that are an array and treat each value of an array as a separate input 
-        	Example: streamline -s split -- 
-        
-        ::breakdown::
-        	Description: Show a report of how many input values ended up with a particular result value
-        	Example: streamline -s breakdown -- 
-        
-        ::headers::
-        	Description: Force each value to a string and prefix each with the original input value
-        	Example: streamline -s headers -- 
-        
-        ::filter_out_errors::
-        	Description: Filter out any entries that have produced an error
-        	Example: streamline -s filter_out_errors -- 
-        
-        ::errors::
-        	Description: Use the latest error on the entry as the value
-        	Example: streamline -s errors -- 
-        
-        ::buffer::
-        	Description: Hold entries in memory until a certain number is reached (give no args to buffer all)
-        	Example: streamline -s buffer -- --buffer 20
-        
-        ::json::
-        	Description: Take json strings and parse them into objects so other streamers can inspect attributes
-        	Example: streamline -s json -- 
-        
-        ::strip::
-        	Description: Strip surrounding whitespace from each string entry, removing entries that are only whitespace
-        	Example: streamline -s strip -- --buffer 20
-        
-        ::head::
-        	Description: Only take the first X entries (Default 1)
-        	Example: streamline -s head -- --count 20
-        
-        ::readfile::
-        	Description: Read the file indicated by the file
-        	Example: streamline -s readfile -- --path ~/dir/{value}.json
-        
-        ::combine::
-        	Description: Combine two previous historical values by setting an attribute
-        	Example: streamline -s combine -- --source "-1" --target "-2"
-        
-        ::http::
-        	Description: Use a template to execute an HTTP request for each value
-        	Example: streamline -s http -- "https://{value}/"
-        
-        ::ssh::
-        	Description: Treat each value as a host to connect to. SSH in and run a command returning the output
-        	Example: streamline -s ssh -- "uptime"
-        
-        ::ssh_exec::
-        	Description: Copy a script to target machine and execute
-        	Example: streamline -s ssh_exec -- ~/dostuff.sh
-        
-        ::shell::
-        	Description: Run a shell command for each value
-        	Example: streamline -s shell -- "nc -zv {value} 22"
-        
-        ::scp::
-        	Description: Treat each value as a host to connect to. Copy a file to or from this host
-        	Example: streamline -s scp -- "/tmp/file.txt" "{value}:/tmp/file.txt"
-        
-        ::sleep::
-        	Description: Sleep for a second (or for {value} seconds) for each entry making no change to its value
-        	Example: streamline -s sleep -- 
-        
-        ::history:push::
-        	Description: Start a new history tree
-        	Example: streamline -s history:push -- 
-        
-        ::history:pop::
-        	Description: Walk back up one level in the history tree
-        	Example: streamline -s history:pop -- 
-        
-        ::history:collapse::
-        	Description: Treat the latest value as the original
-        	Example: streamline -s history:collapse -- 
-        
-        ::history:reset::
-        	Description: Clear all levels of history
-        	Example: streamline -s history:reset -- 
-        
-        ::history:values::
-        	Description: Set the current value to a list of all previous values
-        	Example: streamline -s history:values -- 
-        
-        ```
-        
-        To get available options for a particular module run (substituting "http" for the module you're interested in):
-        
-        ```bash
-        streamline -s http --help
-        ```
-        
-        
-        ## YAML support
-        
-        YAML files defining the streamers and their options is supported. 
-        
-        Given the following yaml file:
-        
-        ```yaml
-        streamers:
-         -
-            name: split
-         -
-            name: http
-            output: code
-            input: value
-            target: status_code
-            options:
-              url: 'https://{value}'`
-        ```
-        
-        It could be used to split a string of domains and get the http code for each one:
-        
-        ```bash
-        $ echo "www.google.com www.slashdot.org" | streamline -y http_codes.yaml
-        {"base": "www.google.com", "status_code": 200}
-        {"base": "www.slashdot.org", "status_code": 200}
-        ```
-        
-        
-        
-        You can also specify the generator and consumer in the same way. Given the below yaml and csv file:
-        ```yaml
-        generator:
-          name: csv
-          options:
-            input: domains.csv
-        consumer:
-          name: csv
-        streamers:
-          -
-             name: http
-             output: code
-             input: domain
-             target: status_code
-             options:
-               url: 'https://{value}'
-        ```
-        
-        ```
-        domain,label
-        www.google.com,The famous big B
-        www.slashdot.org,Mosh pit of opinions
-        ```
-        
-        You can use it the following way:
-        ```bash
-        $ streamline -y http_codes.yaml 
-        domain,label,status_code
-        www.google.com,The famous big B,200
-        www.slashdot.org,Mosh pit of opinions,200
-        ```
-        
-        
-        
-        ## Technical Vocabulary
-        
-        * Entry: A small wrapper around a value being passed along through the stream. Commonly a single line of input.
-        * Generator: An asynchonous generator function that takes no input and yields Entry objects.
-        * Executor:  An asyncronous function that takes a single value and returns a new value. Usually some unit of work is done and the result of that work is returned as the new value.
-        * Streamer: An asynchronous generator function that takes as an argument an asynchronous source iterable that yields Entry objects. Commonly streamers do some manipulation of each Entry it gets from the source iterable and then sets a new value on the entry.
-        * Consumer: An asynchronous function that reads all entries of an asynchronous source iterable. Usually this function writes to some output (such as stdout).
-        
-        
 Keywords: tools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+streamline
+============
+
+The goal of this project is to make data acessible and actionable on the CLI. Streamline does this by implementing the utility functions necessary for taking an input stream and parallelizing work done on it.
+
+The sequence of operations in an invocation:
+
+1. The "Generator" object loads entries from a source data stream (usually stdin).
+2. The "Streamers" selected are sequentially given each input value and are exepcted to filter and make modifications to those values and yield them for the next streamer.
+3. The "Consumer" object takes the entries yielded from the last streamer and usually outputs them for storage or viewing (usually stdout).
+
+## Installation
+
+* Requires Python 3.6+ and pip
+* `pip install streamline`
+
+## Guide
+
+The simplest call specifies no streaming operations it just reads from stdin and writes to stdout exactly what was written:
+
+```bash
+  $ printf "foo\nbar" | streamline
+  foo
+  bar
+```
+
+By default streamline takes input from stdin and writes to stdout. This is very flexible as it makes the tool composible with other CLI tools. However you can also use the `--input` and `--output` flags to control output. Lets assume that you have a file with the same data you just sent in with printf:
+
+```bash
+  $ streamline --input my_source_file.txt --output my_target_file.txt
+  $ cat my_target_file.txt
+  foo
+  bar
+```
+
+Now lets do something a little less useless. Lets use the "shell" streamer to execute a shell command for each entry and check if they're listening for https traffic:
+
+```bash
+  $ printf "www.google.com\nslashdot.org" | streamline -s shell -- "nc -zv {value} 443"
+  {"stdout": "", "stderr": "Connection to www.google.com 443 port [tcp/https] succeeded!\n", "exit_code": 0}
+  {"stdout": "", "stderr": "Connection to slashdot.org 443 port [tcp/https] succeeded!\n", "exit_code": 0}
+```
+
+Streamline modules aim to provide all the useful information in object form as output can then be customized with other streaming modules. For exampe, to take the above output and get just the exit code that tells us whether the port is open we can just add the `headers` streamer to prefix each output with the original input and the `extract` streamer (with its `--selector` option) option to set the value to the `exit_code` property of each result:
+
+```bash
+  $ printf "www.google.com\nslashdot.org" | streamline -s shell extract headers -- "nc -zv {value} 443" --selector exit_code
+  www.google.com: 0
+  slashdot.org: 0
+```
+
+## Built-in Modules
+
+There are many modules available that do asynchronous jobs and transformations to input.  To see all available modules use the main help option to list them with examples:
+
+```bash
+$ streamline --help
+
+=============== Streamline ===============
+
+
+usage: streamline [--generator GENERATOR] [--consumer CONSUMER]
+                  [-s [STREAMERS [STREAMERS ...]]] [-h]
+
+optional arguments:
+  --generator GENERATOR
+                        Entry Generator Module
+  --consumer CONSUMER   Entry Consumer/Writer Module
+  -s [STREAMERS [STREAMERS ...]], --streamers [STREAMERS [STREAMERS ...]]
+                        Additional streamers to apply (-s is optional)
+  -h, --help            Print help
+  -p {buffer,stream-output,streaming}, --progress {buffer,stream-output,streaming}
+                        Print progress to stdout. ("buffer": buffers input and
+                        output, "stream-output" buffers only input, "stream"
+                        for no buffering at all)
+  -w WORKERS, --workers WORKERS
+                        Number of concurrent workers for any one async
+                        execution module to have
+
+
+
+=============== Streamers ===============
+
+::extract::
+	Description: Change the value to an attribute of the current value
+	Example: streamline -s extract -- --selector exit_code
+
+::py::
+	Description: Translate each value by assigning it to the result of a python expression
+	Example: streamline -s py -- "value.upper()"
+
+::pyfilter::
+	Description: Filter out values that dont have a truthy result to a particular python expression
+	Example: streamline -s pyfilter -- "'foobar' in value"
+
+::truthy::
+	Description: Filter out values that are not truthy
+	Example: streamline -s truthy -- 
+
+::noop::
+	Description: No operation. Just for testing.
+	Example: streamline -s noop -- 
+
+::split_list::
+	Description: Take any values that are an array and treat each value of an array as a separate input 
+	Example: streamline -s split_list -- 
+
+::split::
+	Description: Take any values that are an array and treat each value of an array as a separate input 
+	Example: streamline -s split -- 
+
+::breakdown::
+	Description: Show a report of how many input values ended up with a particular result value
+	Example: streamline -s breakdown -- 
+
+::headers::
+	Description: Force each value to a string and prefix each with the original input value
+	Example: streamline -s headers -- 
+
+::filter_out_errors::
+	Description: Filter out any entries that have produced an error
+	Example: streamline -s filter_out_errors -- 
+
+::errors::
+	Description: Use the latest error on the entry as the value
+	Example: streamline -s errors -- 
+
+::buffer::
+	Description: Hold entries in memory until a certain number is reached (give no args to buffer all)
+	Example: streamline -s buffer -- --buffer 20
+
+::json::
+	Description: Take json strings and parse them into objects so other streamers can inspect attributes
+	Example: streamline -s json -- 
+
+::strip::
+	Description: Strip surrounding whitespace from each string entry, removing entries that are only whitespace
+	Example: streamline -s strip -- --buffer 20
+
+::head::
+	Description: Only take the first X entries (Default 1)
+	Example: streamline -s head -- --count 20
+
+::readfile::
+	Description: Read the file indicated by the file
+	Example: streamline -s readfile -- --path ~/dir/{value}.json
+
+::combine::
+	Description: Combine two previous historical values by setting an attribute
+	Example: streamline -s combine -- --source "-1" --target "-2"
+
+::http::
+	Description: Use a template to execute an HTTP request for each value
+	Example: streamline -s http -- "https://{value}/"
+
+::ssh::
+	Description: Treat each value as a host to connect to. SSH in and run a command returning the output
+	Example: streamline -s ssh -- "uptime"
+
+::ssh_exec::
+	Description: Copy a script to target machine and execute
+	Example: streamline -s ssh_exec -- ~/dostuff.sh
+
+::shell::
+	Description: Run a shell command for each value
+	Example: streamline -s shell -- "nc -zv {value} 22"
+
+::scp::
+	Description: Treat each value as a host to connect to. Copy a file to or from this host
+	Example: streamline -s scp -- "/tmp/file.txt" "{value}:/tmp/file.txt"
+
+::sleep::
+	Description: Sleep for a second (or for {value} seconds) for each entry making no change to its value
+	Example: streamline -s sleep -- 
+
+::history:push::
+	Description: Start a new history tree
+	Example: streamline -s history:push -- 
+
+::history:pop::
+	Description: Walk back up one level in the history tree
+	Example: streamline -s history:pop -- 
+
+::history:collapse::
+	Description: Treat the latest value as the original
+	Example: streamline -s history:collapse -- 
+
+::history:reset::
+	Description: Clear all levels of history
+	Example: streamline -s history:reset -- 
+
+::history:values::
+	Description: Set the current value to a list of all previous values
+	Example: streamline -s history:values -- 
+
+```
+
+To get available options for a particular module run (substituting "http" for the module you're interested in):
+
+```bash
+streamline -s http --help
+```
+
+
+## YAML support
+
+YAML files defining the streamers and their options is supported. 
+
+Given the following yaml file:
+
+```yaml
+streamers:
+ -
+    name: split
+ -
+    name: http
+    output: code
+    input: value
+    target: status_code
+    options:
+      url: 'https://{value}'`
+```
+
+It could be used to split a string of domains and get the http code for each one:
+
+```bash
+$ echo "www.google.com www.slashdot.org" | streamline -y http_codes.yaml
+{"base": "www.google.com", "status_code": 200}
+{"base": "www.slashdot.org", "status_code": 200}
+```
+
+
+
+You can also specify the generator and consumer in the same way. Given the below yaml and csv file:
+```yaml
+generator:
+  name: csv
+  options:
+    input: domains.csv
+consumer:
+  name: csv
+streamers:
+  -
+     name: http
+     output: code
+     input: domain
+     target: status_code
+     options:
+       url: 'https://{value}'
+```
+
+```
+domain,label
+www.google.com,The famous big B
+www.slashdot.org,Mosh pit of opinions
+```
+
+You can use it the following way:
+```bash
+$ streamline -y http_codes.yaml 
+domain,label,status_code
+www.google.com,The famous big B,200
+www.slashdot.org,Mosh pit of opinions,200
+```
+
+
+
+## Technical Vocabulary
+
+* Entry: A small wrapper around a value being passed along through the stream. Commonly a single line of input.
+* Generator: An asynchonous generator function that takes no input and yields Entry objects.
+* Executor:  An asyncronous function that takes a single value and returns a new value. Usually some unit of work is done and the result of that work is returned as the new value.
+* Streamer: An asynchronous generator function that takes as an argument an asynchronous source iterable that yields Entry objects. Commonly streamers do some manipulation of each Entry it gets from the source iterable and then sets a new value on the entry.
+* Consumer: An asynchronous function that reads all entries of an asynchronous source iterable. Usually this function writes to some output (such as stdout).
+
+
+
```

