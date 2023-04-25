# Comparing `tmp/promptimize-0.1.0.tar.gz` & `tmp/promptimize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptimize-0.1.0.tar", last modified: Fri Apr  7 00:03:12 2023, max compression
+gzip compressed data, was "promptimize-0.2.0.tar", last modified: Tue Apr 25 01:42:55 2023, max compression
```

## Comparing `promptimize-0.1.0.tar` & `promptimize-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,41 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-07 00:03:12.963074 promptimize-0.1.0/
--rw-r--r--   0 max        (501) staff       (20)    11585 2023-04-07 00:03:12.962359 promptimize-0.1.0/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     9253 2023-04-06 23:58:32.000000 promptimize-0.1.0/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-07 00:03:12.958802 promptimize-0.1.0/promptimize/
--rw-r--r--   0 max        (501) staff       (20)       32 2023-04-06 19:36:35.000000 promptimize-0.1.0/promptimize/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     1383 2023-04-06 22:55:12.000000 promptimize-0.1.0/promptimize/cli.py
--rw-r--r--   0 max        (501) staff       (20)     1832 2023-04-05 07:16:13.000000 promptimize-0.1.0/promptimize/crawler.py
--rw-r--r--   0 max        (501) staff       (20)     4182 2023-04-06 19:55:12.000000 promptimize-0.1.0/promptimize/evals.py
--rw-r--r--   0 max        (501) staff       (20)      264 2023-04-06 01:28:03.000000 promptimize-0.1.0/promptimize/openai_api.py
--rw-r--r--   0 max        (501) staff       (20)     4820 2023-04-06 17:00:29.000000 promptimize-0.1.0/promptimize/prompt.py
--rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.1.0/promptimize/simple_jinja.py
--rw-r--r--   0 max        (501) staff       (20)     1623 2023-04-06 19:55:12.000000 promptimize-0.1.0/promptimize/suite.py
--rw-r--r--   0 max        (501) staff       (20)     5196 2023-04-06 00:56:16.000000 promptimize-0.1.0/promptimize/utils.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-07 00:03:12.961785 promptimize-0.1.0/promptimize.egg-info/
--rw-r--r--   0 max        (501) staff       (20)    11585 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      435 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       71 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       42 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       12 2023-04-07 00:03:12.000000 promptimize-0.1.0/promptimize.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-04-07 00:03:12.963195 promptimize-0.1.0/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      830 2023-04-07 00:02:22.000000 promptimize-0.1.0/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.583011 promptimize-0.2.0/
+-rw-r--r--   0 max        (501) staff       (20)       56 2023-04-07 20:39:22.000000 promptimize-0.2.0/.gitignore
+-rw-r--r--   0 max        (501) staff       (20)       57 2023-04-08 19:15:24.000000 promptimize-0.2.0/.mypy.ini
+-rw-r--r--   0 max        (501) staff       (20)     2058 2023-04-25 01:37:21.000000 promptimize-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 max        (501) staff       (20)    11358 2023-04-08 19:28:50.000000 promptimize-0.2.0/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)    10422 2023-04-25 01:42:55.581957 promptimize-0.2.0/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     8480 2023-04-25 01:33:15.000000 promptimize-0.2.0/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.540409 promptimize-0.2.0/docs/
+-rw-r--r--   0 max        (501) staff       (20)      685 2023-04-08 20:12:24.000000 promptimize-0.2.0/docs/Makefile
+-rwxr-xr-x   0 max        (501) staff       (20)      565 2023-04-25 01:09:25.000000 promptimize-0.2.0/docs/publish.sh
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.541629 promptimize-0.2.0/docs/source/
+-rw-r--r--   0 max        (501) staff       (20)     8144 2023-04-20 19:39:26.000000 promptimize-0.2.0/docs/source/README.md
+-rw-r--r--   0 max        (501) staff       (20)     1268 2023-04-20 01:56:57.000000 promptimize-0.2.0/docs/source/conf.py
+-rw-r--r--   0 max        (501) staff       (20)      111 2023-04-20 02:07:39.000000 promptimize-0.2.0/docs/source/index.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.542423 promptimize-0.2.0/examples/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.542949 promptimize-0.2.0/examples/__pycache__/
+-rw-r--r--   0 max        (501) staff       (20)     2557 2023-04-05 07:54:58.000000 promptimize-0.2.0/examples/__pycache__/use_cases.cpython-38.pyc
+-rw-r--r--   0 max        (501) staff       (20)     2937 2023-04-25 00:36:26.000000 promptimize-0.2.0/examples/readme_examples.py
+-rw-r--r--   0 max        (501) staff       (20)      892 2023-04-20 19:54:23.000000 promptimize-0.2.0/examples/readme_hello_world.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.576401 promptimize-0.2.0/promptimize/
+-rw-r--r--   0 max        (501) staff       (20)       40 2023-04-25 01:13:35.000000 promptimize-0.2.0/promptimize/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     3556 2023-04-25 01:15:16.000000 promptimize-0.2.0/promptimize/cli.py
+-rw-r--r--   0 max        (501) staff       (20)     1843 2023-04-25 01:16:34.000000 promptimize-0.2.0/promptimize/crawler.py
+-rw-r--r--   0 max        (501) staff       (20)     4192 2023-04-25 01:20:03.000000 promptimize-0.2.0/promptimize/evals.py
+-rw-r--r--   0 max        (501) staff       (20)     7634 2023-04-25 01:23:40.000000 promptimize-0.2.0/promptimize/prompt_cases.py
+-rw-r--r--   0 max        (501) staff       (20)     3495 2023-04-25 01:26:15.000000 promptimize-0.2.0/promptimize/reports.py
+-rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.2.0/promptimize/simple_jinja.py
+-rw-r--r--   0 max        (501) staff       (20)     5910 2023-04-25 01:25:06.000000 promptimize-0.2.0/promptimize/suite.py
+-rw-r--r--   0 max        (501) staff       (20)     9068 2023-04-25 01:25:49.000000 promptimize-0.2.0/promptimize/utils.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 01:42:55.581043 promptimize-0.2.0/promptimize.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)    10422 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      743 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       71 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       65 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       12 2023-04-25 01:42:55.000000 promptimize-0.2.0/promptimize.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       31 2023-04-25 01:19:56.000000 promptimize-0.2.0/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       97 2023-04-25 01:11:21.000000 promptimize-0.2.0/requirements-dev.txt
+-rw-r--r--   0 max        (501) staff       (20)       65 2023-04-19 00:07:38.000000 promptimize-0.2.0/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-04-25 01:42:55.583616 promptimize-0.2.0/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      899 2023-04-25 01:37:29.000000 promptimize-0.2.0/setup.py
```

### Comparing `promptimize-0.1.0/PKG-INFO` & `promptimize-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,78 @@
 Metadata-Version: 2.1
 Name: promptimize
-Version: 0.1.0
-Summary: A python framework to generate and evaluate prompts for GPT at scale
+Version: 0.2.0
+Summary: A python toolkit to generate and evaluate prompts for GPT at scale
 Home-page: UNKNOWN
 Author: Maxime Beauchemin
 Author-email: maximebeauchemin@gmail.com
-License: UNKNOWN
+License: Apache License, Version 2.0
 Description: # 💡 ¡promptimize! 💡
+        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+        [![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
+        
         <img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
         
-        **Promptimize** is a framework that accelerates prompt engineering,
-        crafting, and evaluation.
+        Promptimize is a prompt engineering evaluation and testing toolkit.
         
-        Use `promptimize` to
-        - define your prompts as code and tie them to evaluation functions
-        - generate prompt variations dynamically
-        - execute and rank across different engines
-        - get reporting on how your prompts perform
-        
-        In short, `promptimize` offers a programmatic way to define and tune
-        your prompt and evaluation functions in Python in a way that allows
-        you to iterate quickly and confidently.
+        It accelerates and provides structure around prompt engineering at scale
+        with confidence, brigning some of the ideas behind test-driven
+        developmet (TDD) to engineering prompts.
+        
+        With promptimize, you can:
+        
+        - Define your "prompt cases" (think "test cases" but specific to evaluating
+          prompts) as code and associate them with evaluation functions
+        - Generate prompt variations dynamically
+        - Execute and rank prompts test suites across different
+          engines/models/temperature/settings and compare results, brining
+          the hyperparameter tuning mindset to prompt engineering
+        - Get reports on your prompts' performance as you iterate. Answer question
+          around how different prompt suites are performing against one-another.
+          Which individual cases or categories of cases improved? regressed?
+        - Minimize API calls! only re-assess what changed as you change it
+        - Perform human if and where needed, introspected failed cases, overriding
+          false negatives
+        
+        In essence, promptimize provides a programmatic way to execute and fine-tune
+        your prompts and evaluation functions in Python, allowing you to iterate
+        quickly and with confidence.
         
         ## Hello world - the simplest prompt examples
-        [more examples on GitHub](https://github.com/preset-io/promptimize/tree/master/examples)
+        [more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
         ```python
         # Brining some "prompt generator" classes - note that you can derive and extend those
-        from promptimize.prompt import SimplePrompt
+        from promptimize.prompts import SimplePrompt
         
         # Bringing some useful eval function that help evaluating and scoring responses
         # eval functions have a handle on the prompt object and are expected
         # to return a score between 0 and 1
         from promptimize import evals
         
         # Promptimize will scan the target folder and find all Prompt objects
         # and derivatives that are in the python modules
         simple_prompts = [
         
             # Prompting "hello there" and making sure there's "hi" or "hello"
             # somewhere in the answer
-            SimplePrompt("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-            SimplePrompt(
+            PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
+            PromptCase(
                 "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
             ),
         ]
         ```
         
         ### The CLI
         ```bash
-        $ promptimize examples/readme_hello_world.py
-        💡 ¡promptimize! 💡
-        # ----------------------------------------
-        # Prompt prompt-c6950959
-        # ----------------------------------------
-        key: prompt-c6950959
-        input: hello there!
-        response_text: Hi there! How are you?
-        test_results_avg: 1.0
-        
-        # ----------------------------------------
-        # Prompt prompt-7bfe4487
-        # ----------------------------------------
-        key: prompt-7bfe4487
-        input: name the top 50 guitar players!
-        response_text: |-
-          1. Jimi Hendrix
-          2. Eric Clapton
-          3. Jimmy Page
-          {...}
-          50. Jerry Garcia
-        test_results_avg: 0.0
-        
-        # ----------------------------------------
-        # Suite summary
-        # ----------------------------------------
-        suite_score: 0.5
-        completion_create_kwargs:
-          engine: text-davinci-003
-          max_tokens: 1000
-          temperature: 0.5
+        $ promptimize run my_prompts.py --output ./results.yaml
+        
+        $ promptimize --help
         ```
         
+        
         ## Problem + POV
         
         Thousands of product builders are currently trying to figure out how to
         bring the power of AI into the products and experiences they are building.
         The probabilistic (often semi-random, sometimes hectic) nature of LLMs
         makes this a challenge.
         
@@ -93,34 +81,67 @@
         model tuning.
         
         We believe product builders need to tame AI through proper, rigorous
         **prompt engineering**. This allows making the probabilistic nature of
         AI more deterministic, or somewhat predictable, and allows builders to apply
         a hyperparameter tuning-type mindset and approach to prompt engineering.
         
-        In short, Promptimize allows you to generate and test prompts at industrial scale,
+        Any prompt-generator logic that's going to be let loose in the wild inside
+        a product should be thoroughly tested and evaluated with "prompt cases" that
+        cover the breath of what people may do in a product.
+        
+        In short, Promptimize allows you to test prompts at industrial scale,
         so that you can confidently use them in the products you are building.
         
         ## Information Architecture
         
         - **Prompt:** A Prompt instance is a certain test case, a single prompt
           with an associated set of evaluation functions to rate its success.
-        - **Eval:** An evaluation function that reads the response and returns
+        - **Evaluation:** An evaluation function that reads the response and returns
           a success rate between `0` and `1`.
         - **Suite:** A Suite is a collection of Prompt; it's able to run things,
           accumulate results, and print reports about its collection of use cases.
+        - **Report**: a report is the compiled results of running a certain prompt
+          `Suite` or set of suites. Reports can be consumed, compared, and expanded.
         
         ## Principles
         
-        - **Configuration as code:** All use cases, suites, and evaluations are defined as code,
-          which makes it easy to dynamically generate all sorts of use cases and suites.
+        - **Configuration as code:** All prompt cases, suites, and evaluations are
+          defined as code, which makes it easy to dynamically generate all sorts
+          of use cases and suites.
+        - **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
+          the actually prompt creation logic lives in the derivative class of `PromptCase`,
+          so that we can have clean, dense files that contain nice `Suite`s
         - **Support the iteration mindset:** making it easy for people to try things,
           get suggestions from the AI, adapt, compare, and push forward
-        - **Extensibility:** the framework is designed to be extremely hackable and
+        - **Extensibility:** the toolkit is designed to be extremely hackable and
           extensible. Hooks, extensions, high API surface.
+        - **AI-powered:** the framework offers ways to expand your suites based
+          on the examples that exists. Use AI to generate more prompt cases!
+        
+        
+        ## Interesting features / facts
+        
+        Listing out a few features you should know about that you can start using as your
+        suites of prompts become larger / more complex
+        
+        * evaluation functions are assumed to return a value between 0 and 1.
+          contrarily to unit tests, prompt cases aren't boolean
+        * prompts can be assigned a `weight` (default 1) this enables you to define
+          which prompts are more important than others for reporting purposes and suite evaluation
+        * prompts can be assigned a `category`, this can be used in the reporting.
+          That helps understanding which categories are performing better than
+          others, or are most affected by iterations
+        * The `Prompt` class `pre_run` and `post_run` hooks if you want to do
+          post-processing for instance. An example of that would be if you do a prompt
+          that expects GPT to generate code, and you'd like actually say run that code
+          and test it. In our SQL implementation, we run the SQL against the database
+          for instance and get a pandas dataframe back, and allow doing assertions
+          on the dataframe itself
+        
         
         ## Setup
         
         To install the Promptimize package, use the following command:
         ```bash
         pip install promptimize
         ```
@@ -128,117 +149,41 @@
         ## Getting started
         
         First you'll need an openai API key, let's set it as an env var
         ```bash
         export OPENAI_API_KEY=sk-{REDACTED}
         ```
         
-        Find the examples bellow [here](https://github.com/preset-io/promptimize/blob/master/examples/readme_examples.py)
+        Find the examples bellow [here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
         
         ```python
-        # Brining some "prompt generator" classes
-        from promptimize.prompt import SimplePrompt, TemplatedPrompt
-        
-        # Bringing some useful eval function that help evaluating and scoring responses
-        # eval functions have a handle on the prompt object and are expected
-        # to return a score between 0 and 1
-        from promptimize import evals
-        
-        # Promptimize will scan the target folder and find all Prompt objects
-        # and derivatives that are in the python modules
-        simple_prompts = [
-        
-            # Prompting "hello there" and making sure there's "hi" or "hello"
-            # somewhere in the answer
-            SimplePrompt("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-        
-            # Making sure 3 specific guitar players are in the top 50
-            # the score here is a percentage of the words found
-            SimplePrompt(
-                "who are the top 50 best guitar players of all time?",
-                lambda x: evals.percentage_of_words(
-                    x, ["frank zappa", "david gilmore", "carlos santana"]
-                ),
-            ),
-            # GPT-ing myself and making sure the response mentions Superset and Airflow
-            SimplePrompt(
-                "who is Maxime Beauchemin, (the data guy...)?",
-                lambda x: evals.percentage_of_words(x, ["superset", "airflow"], case_sensitive=False),
-            ),
-        ]
-        
-        # deriving TemplatedPrompt to generate prompts that ask GPT to generate SQL
-        # based on table schemas. The point here is you can derive the `Prompt`
-        # class to create more specialized Prompt generators
-        # For instance, the SqlPropt class defined bellow could be extended to fetch
-        # schema definitions dynamically, acutally run the SQL, and allow
-        # doing evals against the resultset.
-        
-        class SqlPrompt(TemplatedPrompt):
-            # the TemplatedPrompt expects a dict of defaults that can be overriden in the constructor
-            template_defaults = {"dialect": "Postgres"}
-            # The actual Jinja2 template
-            prompt_template = """\
-            given these SQL table schemas:
-                CREATE TABLE world_population (
-                    country_name STRING,
-                    year DATE,
-                    population_total INT,
-                );
-        
-            So, can you write a SQL query for {{ dialect }} that answers this user prompt:
-            {{ input }}
-            """
-        
-        # Generating a few SQL prompts
-        sql_prompts = [
-            SqlPrompt(
-                # the user input that'll be added in place of {{ input }} in the template above
-                "give me the top 10 countries with the highest net increase of population over the past 25 years?",
-                # the dialect template parameter, overriding the default set above
-                dialect="BigQuery",
-                # a simple validation function making sure the SQL starts with SELECT
-                evaluators=[lambda x: x.trim().startswith("SELECT")],
-            ),
-        ]
-        
         ```
-        
         ```bash
         # NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
         
         # First let's run some of the examples
         p9e ./examples
         
         # Now the same but with verbose output
         p9e ./examples --verbose
         
         ```
+        ## Langchain?
         
-        Now take a look at the definitions of what you just ran here ->
-        [Promptimize examples on GitHub](https://github.com/preset-io/promptimize/tree/master/examples)
+        How does promptimize relate to `langchain`?
         
-        ## The CLI
-        ```bash
-        $ promptimize --help
-        Usage: promptimize [OPTIONS] PATH
+        We think langchain is amazing and promptimize uses langchain under the
+        hood to interact with openai, and has integration with langchain
+        (see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
+        and `LangchainAgntPromptCase`)
+        While you don't have to use
+        langchain, and could use promptimize on top of any python prompt generation
+        whether it'd be another library or some home grown thing.
         
         
-        Options:
-          -v, --verbose             Trigger more verbose output
-          -s, --style [json|yaml]   json or yaml formatting
-          -m, --max-tokens INTEGER  max_tokens passed to the model
-          -t, --temperature FLOAT   max_tokens passed to the model
-          -e, --engine TEXT         model as accepted by the openai API
-          --help                    Show this message and exit.
-        ```
-        
-        ## Resources
-        * [GPT interactive playground](https://platform.openai.com/playground/p/default-adv-tweet-classifier)
-        
         ## Context
         
         <img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
         
         Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
         founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
         (data exploration,
@@ -246,19 +191,23 @@
         complex SQL based on natural language, and to suggest charts to users. We
         derive the `SimpleQuery` class to make it fitted to our specific use
         cases in our own prompt engineering repo. Not my first open source project
         as the creator of
         [Apache Superset](https://github.com/apache/superset/) and
         [Apache Airflow](https://github.com/apache/airflow/)
         
-        ## Disclaimer
         
-        "Publish early, publish often!" This project is pretty much at `0.1.0`
-        and the creator is a busy man
-        (running www.preset.io), and actually extending and using this framework
-        to work on bringing AI to BI. Contributions, contributors and maintainers
-        are more than welcomed! Looking forward to engage directly with all
-        contributors! To get involved, open an GitHub issue detailing how you'd
-        like to get involved, or just open a PR!
+        ## Contribute
+        
+        This project is in its super early stages as of `0.1.0`, and contributions,
+        contributors, and maintainers are highly encouraged. While it's a great time
+        to onboard and influence the direction of the project, things are still
+        evolving quickly. To get involved, open a GitHub issue
+        or submit a pull request!
+        
+        ## Links
+        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/)
+        * [Preset Blog](https://preset.io/blog/)
+        * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `promptimize-0.1.0/README.md` & `promptimize-0.2.0/promptimize.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,253 +1,213 @@
-# 💡 ¡promptimize! 💡
-<img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
-
-**Promptimize** is a framework that accelerates prompt engineering,
-crafting, and evaluation.
-
-Use `promptimize` to
-- define your prompts as code and tie them to evaluation functions
-- generate prompt variations dynamically
-- execute and rank across different engines
-- get reporting on how your prompts perform
-
-In short, `promptimize` offers a programmatic way to define and tune
-your prompt and evaluation functions in Python in a way that allows
-you to iterate quickly and confidently.
-
-## Hello world - the simplest prompt examples
-[more examples on GitHub](https://github.com/preset-io/promptimize/tree/master/examples)
-```python
-# Brining some "prompt generator" classes - note that you can derive and extend those
-from promptimize.prompt import SimplePrompt
-
-# Bringing some useful eval function that help evaluating and scoring responses
-# eval functions have a handle on the prompt object and are expected
-# to return a score between 0 and 1
-from promptimize import evals
-
-# Promptimize will scan the target folder and find all Prompt objects
-# and derivatives that are in the python modules
-simple_prompts = [
-
-    # Prompting "hello there" and making sure there's "hi" or "hello"
-    # somewhere in the answer
-    SimplePrompt("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-    SimplePrompt(
-        "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
-    ),
-]
-```
-
-### The CLI
-```bash
-$ promptimize examples/readme_hello_world.py
-💡 ¡promptimize! 💡
-# ----------------------------------------
-# Prompt prompt-c6950959
-# ----------------------------------------
-key: prompt-c6950959
-input: hello there!
-response_text: Hi there! How are you?
-test_results_avg: 1.0
-
-# ----------------------------------------
-# Prompt prompt-7bfe4487
-# ----------------------------------------
-key: prompt-7bfe4487
-input: name the top 50 guitar players!
-response_text: |-
-  1. Jimi Hendrix
-  2. Eric Clapton
-  3. Jimmy Page
-  {...}
-  50. Jerry Garcia
-test_results_avg: 0.0
-
-# ----------------------------------------
-# Suite summary
-# ----------------------------------------
-suite_score: 0.5
-completion_create_kwargs:
-  engine: text-davinci-003
-  max_tokens: 1000
-  temperature: 0.5
-```
-
-## Problem + POV
-
-Thousands of product builders are currently trying to figure out how to
-bring the power of AI into the products and experiences they are building.
-The probabilistic (often semi-random, sometimes hectic) nature of LLMs
-makes this a challenge.
-
-Prompt engineering is a huge piece of the puzzle in terms of how to do this
-right, especially given the complexity, risks, and drawbacks around
-model tuning.
-
-We believe product builders need to tame AI through proper, rigorous
-**prompt engineering**. This allows making the probabilistic nature of
-AI more deterministic, or somewhat predictable, and allows builders to apply
-a hyperparameter tuning-type mindset and approach to prompt engineering.
-
-In short, Promptimize allows you to generate and test prompts at industrial scale,
-so that you can confidently use them in the products you are building.
-
-## Information Architecture
-
-- **Prompt:** A Prompt instance is a certain test case, a single prompt
-  with an associated set of evaluation functions to rate its success.
-- **Eval:** An evaluation function that reads the response and returns
-  a success rate between `0` and `1`.
-- **Suite:** A Suite is a collection of Prompt; it's able to run things,
-  accumulate results, and print reports about its collection of use cases.
-
-## Principles
-
-- **Configuration as code:** All use cases, suites, and evaluations are defined as code,
-  which makes it easy to dynamically generate all sorts of use cases and suites.
-- **Support the iteration mindset:** making it easy for people to try things,
-  get suggestions from the AI, adapt, compare, and push forward
-- **Extensibility:** the framework is designed to be extremely hackable and
-  extensible. Hooks, extensions, high API surface.
-
-## Setup
-
-To install the Promptimize package, use the following command:
-```bash
-pip install promptimize
-```
-
-## Getting started
-
-First you'll need an openai API key, let's set it as an env var
-```bash
-export OPENAI_API_KEY=sk-{REDACTED}
-```
-
-Find the examples bellow [here](https://github.com/preset-io/promptimize/blob/master/examples/readme_examples.py)
-
-```python
-# Brining some "prompt generator" classes
-from promptimize.prompt import SimplePrompt, TemplatedPrompt
-
-# Bringing some useful eval function that help evaluating and scoring responses
-# eval functions have a handle on the prompt object and are expected
-# to return a score between 0 and 1
-from promptimize import evals
-
-# Promptimize will scan the target folder and find all Prompt objects
-# and derivatives that are in the python modules
-simple_prompts = [
-
-    # Prompting "hello there" and making sure there's "hi" or "hello"
-    # somewhere in the answer
-    SimplePrompt("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-
-    # Making sure 3 specific guitar players are in the top 50
-    # the score here is a percentage of the words found
-    SimplePrompt(
-        "who are the top 50 best guitar players of all time?",
-        lambda x: evals.percentage_of_words(
-            x, ["frank zappa", "david gilmore", "carlos santana"]
-        ),
-    ),
-    # GPT-ing myself and making sure the response mentions Superset and Airflow
-    SimplePrompt(
-        "who is Maxime Beauchemin, (the data guy...)?",
-        lambda x: evals.percentage_of_words(x, ["superset", "airflow"], case_sensitive=False),
-    ),
-]
-
-# deriving TemplatedPrompt to generate prompts that ask GPT to generate SQL
-# based on table schemas. The point here is you can derive the `Prompt`
-# class to create more specialized Prompt generators
-# For instance, the SqlPropt class defined bellow could be extended to fetch
-# schema definitions dynamically, acutally run the SQL, and allow
-# doing evals against the resultset.
-
-class SqlPrompt(TemplatedPrompt):
-    # the TemplatedPrompt expects a dict of defaults that can be overriden in the constructor
-    template_defaults = {"dialect": "Postgres"}
-    # The actual Jinja2 template
-    prompt_template = """\
-    given these SQL table schemas:
-        CREATE TABLE world_population (
-            country_name STRING,
-            year DATE,
-            population_total INT,
-        );
-
-    So, can you write a SQL query for {{ dialect }} that answers this user prompt:
-    {{ input }}
-    """
-
-# Generating a few SQL prompts
-sql_prompts = [
-    SqlPrompt(
-        # the user input that'll be added in place of {{ input }} in the template above
-        "give me the top 10 countries with the highest net increase of population over the past 25 years?",
-        # the dialect template parameter, overriding the default set above
-        dialect="BigQuery",
-        # a simple validation function making sure the SQL starts with SELECT
-        evaluators=[lambda x: x.trim().startswith("SELECT")],
-    ),
-]
-
-```
-
-```bash
-# NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
-
-# First let's run some of the examples
-p9e ./examples
-
-# Now the same but with verbose output
-p9e ./examples --verbose
-
-```
-
-Now take a look at the definitions of what you just ran here ->
-[Promptimize examples on GitHub](https://github.com/preset-io/promptimize/tree/master/examples)
-
-## The CLI
-```bash
-$ promptimize --help
-Usage: promptimize [OPTIONS] PATH
-
-
-Options:
-  -v, --verbose             Trigger more verbose output
-  -s, --style [json|yaml]   json or yaml formatting
-  -m, --max-tokens INTEGER  max_tokens passed to the model
-  -t, --temperature FLOAT   max_tokens passed to the model
-  -e, --engine TEXT         model as accepted by the openai API
-  --help                    Show this message and exit.
-```
-
-## Resources
-* [GPT interactive playground](https://platform.openai.com/playground/p/default-adv-tweet-classifier)
-
-## Context
-
-<img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
-
-Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
-founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
-(data exploration,
-and visualization). At Preset, we use `promptimize` to generate
-complex SQL based on natural language, and to suggest charts to users. We
-derive the `SimpleQuery` class to make it fitted to our specific use
-cases in our own prompt engineering repo. Not my first open source project
-as the creator of
-[Apache Superset](https://github.com/apache/superset/) and
-[Apache Airflow](https://github.com/apache/airflow/)
-
-## Disclaimer
-
-"Publish early, publish often!" This project is pretty much at `0.1.0`
-and the creator is a busy man
-(running www.preset.io), and actually extending and using this framework
-to work on bringing AI to BI. Contributions, contributors and maintainers
-are more than welcomed! Looking forward to engage directly with all
-contributors! To get involved, open an GitHub issue detailing how you'd
-like to get involved, or just open a PR!
+Metadata-Version: 2.1
+Name: promptimize
+Version: 0.2.0
+Summary: A python toolkit to generate and evaluate prompts for GPT at scale
+Home-page: UNKNOWN
+Author: Maxime Beauchemin
+Author-email: maximebeauchemin@gmail.com
+License: Apache License, Version 2.0
+Description: # 💡 ¡promptimize! 💡
+        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+        [![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
+        
+        <img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
+        
+        Promptimize is a prompt engineering evaluation and testing toolkit.
+        
+        It accelerates and provides structure around prompt engineering at scale
+        with confidence, brigning some of the ideas behind test-driven
+        developmet (TDD) to engineering prompts.
+        
+        With promptimize, you can:
+        
+        - Define your "prompt cases" (think "test cases" but specific to evaluating
+          prompts) as code and associate them with evaluation functions
+        - Generate prompt variations dynamically
+        - Execute and rank prompts test suites across different
+          engines/models/temperature/settings and compare results, brining
+          the hyperparameter tuning mindset to prompt engineering
+        - Get reports on your prompts' performance as you iterate. Answer question
+          around how different prompt suites are performing against one-another.
+          Which individual cases or categories of cases improved? regressed?
+        - Minimize API calls! only re-assess what changed as you change it
+        - Perform human if and where needed, introspected failed cases, overriding
+          false negatives
+        
+        In essence, promptimize provides a programmatic way to execute and fine-tune
+        your prompts and evaluation functions in Python, allowing you to iterate
+        quickly and with confidence.
+        
+        ## Hello world - the simplest prompt examples
+        [more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
+        ```python
+        # Brining some "prompt generator" classes - note that you can derive and extend those
+        from promptimize.prompts import SimplePrompt
+        
+        # Bringing some useful eval function that help evaluating and scoring responses
+        # eval functions have a handle on the prompt object and are expected
+        # to return a score between 0 and 1
+        from promptimize import evals
+        
+        # Promptimize will scan the target folder and find all Prompt objects
+        # and derivatives that are in the python modules
+        simple_prompts = [
+        
+            # Prompting "hello there" and making sure there's "hi" or "hello"
+            # somewhere in the answer
+            PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
+            PromptCase(
+                "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
+            ),
+        ]
+        ```
+        
+        ### The CLI
+        ```bash
+        $ promptimize run my_prompts.py --output ./results.yaml
+        
+        $ promptimize --help
+        ```
+        
+        
+        ## Problem + POV
+        
+        Thousands of product builders are currently trying to figure out how to
+        bring the power of AI into the products and experiences they are building.
+        The probabilistic (often semi-random, sometimes hectic) nature of LLMs
+        makes this a challenge.
+        
+        Prompt engineering is a huge piece of the puzzle in terms of how to do this
+        right, especially given the complexity, risks, and drawbacks around
+        model tuning.
+        
+        We believe product builders need to tame AI through proper, rigorous
+        **prompt engineering**. This allows making the probabilistic nature of
+        AI more deterministic, or somewhat predictable, and allows builders to apply
+        a hyperparameter tuning-type mindset and approach to prompt engineering.
+        
+        Any prompt-generator logic that's going to be let loose in the wild inside
+        a product should be thoroughly tested and evaluated with "prompt cases" that
+        cover the breath of what people may do in a product.
+        
+        In short, Promptimize allows you to test prompts at industrial scale,
+        so that you can confidently use them in the products you are building.
+        
+        ## Information Architecture
+        
+        - **Prompt:** A Prompt instance is a certain test case, a single prompt
+          with an associated set of evaluation functions to rate its success.
+        - **Evaluation:** An evaluation function that reads the response and returns
+          a success rate between `0` and `1`.
+        - **Suite:** A Suite is a collection of Prompt; it's able to run things,
+          accumulate results, and print reports about its collection of use cases.
+        - **Report**: a report is the compiled results of running a certain prompt
+          `Suite` or set of suites. Reports can be consumed, compared, and expanded.
+        
+        ## Principles
+        
+        - **Configuration as code:** All prompt cases, suites, and evaluations are
+          defined as code, which makes it easy to dynamically generate all sorts
+          of use cases and suites.
+        - **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
+          the actually prompt creation logic lives in the derivative class of `PromptCase`,
+          so that we can have clean, dense files that contain nice `Suite`s
+        - **Support the iteration mindset:** making it easy for people to try things,
+          get suggestions from the AI, adapt, compare, and push forward
+        - **Extensibility:** the toolkit is designed to be extremely hackable and
+          extensible. Hooks, extensions, high API surface.
+        - **AI-powered:** the framework offers ways to expand your suites based
+          on the examples that exists. Use AI to generate more prompt cases!
+        
+        
+        ## Interesting features / facts
+        
+        Listing out a few features you should know about that you can start using as your
+        suites of prompts become larger / more complex
+        
+        * evaluation functions are assumed to return a value between 0 and 1.
+          contrarily to unit tests, prompt cases aren't boolean
+        * prompts can be assigned a `weight` (default 1) this enables you to define
+          which prompts are more important than others for reporting purposes and suite evaluation
+        * prompts can be assigned a `category`, this can be used in the reporting.
+          That helps understanding which categories are performing better than
+          others, or are most affected by iterations
+        * The `Prompt` class `pre_run` and `post_run` hooks if you want to do
+          post-processing for instance. An example of that would be if you do a prompt
+          that expects GPT to generate code, and you'd like actually say run that code
+          and test it. In our SQL implementation, we run the SQL against the database
+          for instance and get a pandas dataframe back, and allow doing assertions
+          on the dataframe itself
+        
+        
+        ## Setup
+        
+        To install the Promptimize package, use the following command:
+        ```bash
+        pip install promptimize
+        ```
+        
+        ## Getting started
+        
+        First you'll need an openai API key, let's set it as an env var
+        ```bash
+        export OPENAI_API_KEY=sk-{REDACTED}
+        ```
+        
+        Find the examples bellow [here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
+        
+        ```python
+        ```
+        ```bash
+        # NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
+        
+        # First let's run some of the examples
+        p9e ./examples
+        
+        # Now the same but with verbose output
+        p9e ./examples --verbose
+        
+        ```
+        ## Langchain?
+        
+        How does promptimize relate to `langchain`?
+        
+        We think langchain is amazing and promptimize uses langchain under the
+        hood to interact with openai, and has integration with langchain
+        (see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
+        and `LangchainAgntPromptCase`)
+        While you don't have to use
+        langchain, and could use promptimize on top of any python prompt generation
+        whether it'd be another library or some home grown thing.
+        
+        
+        ## Context
+        
+        <img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
+        
+        Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
+        founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
+        (data exploration,
+        and visualization). At Preset, we use `promptimize` to generate
+        complex SQL based on natural language, and to suggest charts to users. We
+        derive the `SimpleQuery` class to make it fitted to our specific use
+        cases in our own prompt engineering repo. Not my first open source project
+        as the creator of
+        [Apache Superset](https://github.com/apache/superset/) and
+        [Apache Airflow](https://github.com/apache/airflow/)
+        
+        
+        ## Contribute
+        
+        This project is in its super early stages as of `0.1.0`, and contributions,
+        contributors, and maintainers are highly encouraged. While it's a great time
+        to onboard and influence the direction of the project, things are still
+        evolving quickly. To get involved, open a GitHub issue
+        or submit a pull request!
+        
+        ## Links
+        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/)
+        * [Preset Blog](https://preset.io/blog/)
+        * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `promptimize-0.1.0/promptimize/crawler.py` & `promptimize-0.2.0/promptimize/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import os, sys
+import sys
 import importlib
 import pkgutil
 from pathlib import Path
-from typing import List, Type, Any, Union
+from typing import List, Type, Any
 
 
 def is_instance_or_derivative(obj: Any, object_type: Type) -> bool:
     return isinstance(obj, object_type)
 
 
-def discover_objects(path: str, object_type: Type) -> List[Any]:
+def discover_objects(path: str, object_type: Type) -> List[Any]:  # noqa
     objects = []
     folder_path = Path(path).resolve()
 
     def process_module(module):
         # Iterate over the objects in the module
         for name, obj in module.__dict__.items():
             # Check if the object is an instance or derivative of the specified type
             if is_instance_or_derivative(obj, object_type):
                 objects.append(obj)
-            # Check if the object is a list or tuple containing instances or derivatives of the specified type
+            # Check if the object is a list or tuple containing instances or
+            # derivatives of the specified type
             elif isinstance(obj, (list, tuple)):
                 for item in obj:
                     if is_instance_or_derivative(item, object_type):
                         objects.append(item)
 
     # If the path points to a file, import the module and process it directly
     if folder_path.is_file() and folder_path.suffix == ".py":
```

### Comparing `promptimize-0.1.0/promptimize/evals.py` & `promptimize-0.2.0/promptimize/evals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 Eval functions that be used/reused with Prompts
 
 All functions here are expected to:
 * receive a response string
 * [optional] receive arbitrary extra context
 * return a value from 0 to 1, 0 representing failing at the task, 1 full
-  success, and a range in-between
+success, and a range in-between
 """
 
 from typing import List
 
 
-def percentage_of_words(
-    response: str, words: List[str], case_sensitive: bool = False
-) -> float:
+def percentage_of_words(response: str, words: List[str], case_sensitive: bool = False) -> float:
     """
     Calculate the percentage of words from a list that are present in the given response.
 
     Args:
         response (str): The string to search for words.
         words (List[str]): A list of words to check for their presence in the response.
         case_sensitive (bool, optional): If True, the search will be case-sensitive;
@@ -25,17 +23,19 @@
 
     Returns:
         float: The percentage of words found in the response (0.0 to 1.0).
 
     Examples:
     >>> percentage_of_words_in_response("This is an Example string.", ["example", "test"])
     0.5
-    >>> percentage_of_words_in_response("This is an Example string.", ["Example"], case_sensitive=True)
+    >>> percentage_of_words_in_response(
+        "This is an Example string.", ["Example"], case_sensitive=True)
     1.0
-    >>> percentage_of_words_in_response("This is an Example string.", ["example"], case_sensitive=True)
+    >>> percentage_of_words_in_response(
+        "This is an Example string.", ["example"], case_sensitive=True)
     0.0
     >>> percentage_of_words_in_response("This is an Example string.", ["notfound"])
     0.0
     """
     if not case_sensitive:
         response = response.lower()
         words = [w.lower() for w in words]
```

