# Comparing `tmp/pyllms-0.1.9.tar.gz` & `tmp/pyllms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.9.tar", last modified: Sun Apr 23 03:41:14 2023, max compression
+gzip compressed data, was "pyllms-0.2.0.tar", last modified: Tue Apr 25 01:27:17 2023, max compression
```

## Comparing `pyllms-0.1.9.tar` & `pyllms-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.560379 pyllms-0.1.9/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.9/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    16914 2023-04-23 03:41:14.560065 pyllms-0.1.9/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    15601 2023-04-23 03:36:41.000000 pyllms-0.1.9/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.554361 pyllms-0.1.9/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.9/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    19018 2023-04-23 03:31:42.000000 pyllms-0.1.9/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.558381 pyllms-0.1.9/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.1.9/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2449 2023-04-23 01:59:45.000000 pyllms-0.1.9/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2696 2023-04-23 02:28:11.000000 pyllms-0.1.9/llms/providers/aleph.py
--rw-r--r--   0 prelovac   (502) staff       (20)     6612 2023-04-23 03:05:56.000000 pyllms-0.1.9/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3641 2023-04-23 02:28:09.000000 pyllms-0.1.9/llms/providers/cohere.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2551 2023-04-23 03:25:52.000000 pyllms-0.1.9/llms/providers/huggingface.py
--rw-r--r--   0 prelovac   (502) staff       (20)     5558 2023-04-23 01:59:45.000000 pyllms-0.1.9/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-23 03:41:14.559726 pyllms-0.1.9/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    16914 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      387 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       85 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-23 03:41:14.000000 pyllms-0.1.9/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-23 03:41:14.560469 pyllms-0.1.9/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1882 2023-04-23 03:37:05.000000 pyllms-0.1.9/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.287240 pyllms-0.2.0/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.0/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    16542 2023-04-25 01:27:17.286931 pyllms-0.2.0/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    15229 2023-04-25 00:51:55.000000 pyllms-0.2.0/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.283096 pyllms-0.2.0/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.0/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    18832 2023-04-25 01:23:34.000000 pyllms-0.2.0/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.285346 pyllms-0.2.0/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.2.0/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2336 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2672 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     8069 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)      950 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/base_provider.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3664 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2514 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     5692 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.286612 pyllms-0.2.0/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    16542 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      419 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       85 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 01:27:17.287307 pyllms-0.2.0/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1882 2023-04-25 01:24:12.000000 pyllms-0.2.0/setup.py
```

### Comparing `pyllms-0.1.9/LICENSE` & `pyllms-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.9/PKG-INFO` & `pyllms-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.9
+Version: 0.2.0
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
@@ -28,15 +28,15 @@
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
 PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
 It is ideal for fast prototyping and evaluating different models thanks to:
-- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
+- Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
@@ -57,20 +57,23 @@
 model = llms.init()
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
-Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+export COHERE_API_KEY="your_api_key_here"
+export ALEPHALPHA_API_KEY="your_api_key_here"
+export HUGGINFACEHUB_API_KEY="your_api_key_here"
 
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
@@ -92,49 +95,61 @@
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
 The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
-{'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
+{
+  'model': 'gpt-3.5-turbo', 
+  'tokens': 34, 
+  'tokens_prompt': 20, 
+  'tokens_completion': 14, 
+  'cost': '0.00007', 
+  'latency': 1.4
+}
 ```
 
 
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
-['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
+[
+ 'The capital of the country where Mozart was born is Vienna, Austria.', 
+ 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.'
+]
 
 >>> print(result.meta)
-[{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
+[
+ {'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, 
+ {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}
+]
+```
+
+## Async support
+Async completion is supported for compatible models. It is not supported in multi-models mode yet.
+```
+result = await model.acomplete("what is the capital of country where mozzart was born")
 ```
 
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
->>> model= llms.init('claude-v1')
->>> result = model.complete_stream("write an essay on civil war")
->>> for chunk in result:
-...        if chunk is not None:
-...          print(chunk, end='')   
-... 
-
-Here is a paragraph about civil rights:
-
-
-Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
-
+model= llms.init('claude-v1')
+result = model.complete_stream("write an essay on civil war")
+for chunk in result:
+   if chunk is not None:
+      print(chunk, end='')   
 ```
 
 Current limitations:
 - When streaming, 'meta' is not available
 - Multi-models are not supported for streaming
 
 
@@ -160,16 +175,18 @@
 2) Speed
 3) Cost
 
 PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'command-xlarge-nightly'])
+
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
+
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 |             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
@@ -236,36 +253,41 @@
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+```
+
+Here is a pretty table of supported models (in alphabetical order).
+```
 
 | Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
 |---------------------|------------------------|-------------|-----------------|-------------|
 | AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
 | AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
 | AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
 | AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
 | AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
 | AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
 | AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
 | AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
-| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
-| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-beta    |        25.0 |            25.0 |        8192 |
+| CohereProvider      | command-xlarge-nightly |        25.0 |            25.0 |        8192 |
+| HuggingfaceHub      | hf_pythia              |         0.0 |             0.0 |        2048 |
 | OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
 | OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
 
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
-[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)\
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)\
 [Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.9/README.md` & `pyllms-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
 PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
 It is ideal for fast prototyping and evaluating different models thanks to:
-- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
+- Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
@@ -31,20 +31,23 @@
 model = llms.init()
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
-Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+export COHERE_API_KEY="your_api_key_here"
+export ALEPHALPHA_API_KEY="your_api_key_here"
+export HUGGINFACEHUB_API_KEY="your_api_key_here"
 
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
@@ -66,49 +69,61 @@
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
 The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
-{'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
+{
+  'model': 'gpt-3.5-turbo', 
+  'tokens': 34, 
+  'tokens_prompt': 20, 
+  'tokens_completion': 14, 
+  'cost': '0.00007', 
+  'latency': 1.4
+}
 ```
 
 
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
-['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
+[
+ 'The capital of the country where Mozart was born is Vienna, Austria.', 
+ 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.'
+]
 
 >>> print(result.meta)
-[{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
+[
+ {'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, 
+ {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}
+]
+```
+
+## Async support
+Async completion is supported for compatible models. It is not supported in multi-models mode yet.
+```
+result = await model.acomplete("what is the capital of country where mozzart was born")
 ```
 
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
->>> model= llms.init('claude-v1')
->>> result = model.complete_stream("write an essay on civil war")
->>> for chunk in result:
-...        if chunk is not None:
-...          print(chunk, end='')   
-... 
-
-Here is a paragraph about civil rights:
-
-
-Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
-
+model= llms.init('claude-v1')
+result = model.complete_stream("write an essay on civil war")
+for chunk in result:
+   if chunk is not None:
+      print(chunk, end='')   
 ```
 
 Current limitations:
 - When streaming, 'meta' is not available
 - Multi-models are not supported for streaming
 
 
@@ -134,16 +149,18 @@
 2) Speed
 3) Cost
 
 PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'command-xlarge-nightly'])
+
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
+
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 |             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
@@ -210,36 +227,41 @@
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+```
+
+Here is a pretty table of supported models (in alphabetical order).
+```
 
 | Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
 |---------------------|------------------------|-------------|-----------------|-------------|
 | AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
 | AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
 | AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
 | AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
 | AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
 | AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
 | AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
 | AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
-| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
-| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-beta    |        25.0 |            25.0 |        8192 |
+| CohereProvider      | command-xlarge-nightly |        25.0 |            25.0 |        8192 |
+| HuggingfaceHub      | hf_pythia              |         0.0 |             0.0 |        2048 |
 | OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
 | OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
 
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
-[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)\
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)\
 [Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.9/llms/llms.py` & `pyllms-0.2.0/llms/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self,
         model=None,
         openai_api_key=None,
         anthropic_api_key=None,
         ai21_api_key=None,
         cohere_api_key=None,
         alephalpha_api_key=None,
-        huggingfacehub_api_key=None
+        huggingfacehub_api_key=None,
     ):
         if openai_api_key is None:
             openai_api_key = os.getenv("OPENAI_API_KEY")
 
         if anthropic_api_key is None:
             anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 
@@ -52,15 +52,15 @@
         if cohere_api_key is None:
             cohere_api_key = os.getenv("COHERE_API_KEY")
 
         if alephalpha_api_key is None:
             alephalpha_api_key = os.getenv("ALEPHALPHA_API_KEY")
 
         if huggingfacehub_api_key is None:
-            huggingfacehub_api_key = os.getenv("HUGGINFACEHUB_API_KEY")    
+            huggingfacehub_api_key = os.getenv("HUGGINFACEHUB_API_KEY")
 
         if model is None:
             model = os.getenv("LLMS_DEFAULT_MODEL")
             if model is None:
                 model = ["gpt-3.5-turbo"]
             else:
                 model = [model]
@@ -98,29 +98,34 @@
                     AlephAlphaProvider(api_key=alephalpha_api_key, model=single_model)
                 )
             elif (
                 huggingfacehub_api_key is not None
                 and single_model in HuggingfaceHubProvider.MODEL_INFO
             ):
                 self._providers.append(
-                    HuggingfaceHubProvider(api_key=huggingfacehub_api_key, model=single_model)
-                )    
+                    HuggingfaceHubProvider(
+                        api_key=huggingfacehub_api_key, model=single_model
+                    )
+                )
             else:
                 raise ValueError("Invalid API key and model combination", single_model)
 
+    def __repr__(self) -> str:
+        return f"LLMS({self.model})"
+
     def list(self, query=None):
         model_info_list = []
 
         all_providers = [
             OpenAIProvider,
             AI21Provider,
             AnthropicProvider,
             CohereProvider,
             AlephAlphaProvider,
-            HuggingfaceHubProvider
+            HuggingfaceHubProvider,
         ]
 
         for provider in all_providers:
             for model, cost in provider.MODEL_INFO.items():
                 if query and (
                     (query.lower() not in model.lower())
                     and (query.lower() not in provider.__name__.lower())
@@ -173,15 +178,14 @@
                 results.append(future.result())
 
         return Result(results)
 
     async def acomplete(
         self,
         prompt: str,
-        history: Optional[List[tuple]] = None,
         **kwargs,
     ):
         if len(self._providers) > 1:
             raise NotImplementedError("acomplete not supported for multi-models yet.")
         provider = self._providers[0]
         response = await provider.acomplete(prompt, **kwargs)
 
@@ -200,16 +204,14 @@
                 }
             ]
         )
 
     def complete_stream(self, prompt, **kwargs):
         if len(self._providers) > 1:
             raise ValueError("Streaming is possible only with a single model")
-        if isinstance(self._providers[0], AI21Provider) or isinstance(self._providers[0], AlephAlphaProvider) or isinstance(self._providers[0], HuggingfaceHubProvider):
-            raise ValueError("Streaming is not yet supported with this model")
 
         yield from self._providers[0].complete_stream(prompt, **kwargs)
 
     def benchmark(self, prompts=None, evaluator=None, show_outputs=False, html=False):
         if not prompts:
             prompts = [
                 "What is the capital of the country where Christopher Columbus was born?",
```

### Comparing `pyllms-0.1.9/llms/providers/ai21.py` & `pyllms-0.2.0/llms/providers/ai21.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # llms/providers/anthropic.py
 
 import ai21
 import time
 import itertools
 from typing import List, Optional
 
+from .base_provider import BaseProvider
 
-class AI21Provider:
+
+class AI21Provider(BaseProvider):
     # per million tokens
     MODEL_INFO = {
         "j2-grande-instruct": {"prompt": 10.0, "completion": 10.0, "token_limit": 8192},
         "j2-jumbo-instruct": {"prompt": 15.0, "completion": 15.0, "token_limit": 8192},
     }
 
     def __init__(self, api_key, model=None):
         ai21.api_key = api_key
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
-
-    def count_tokens(self, content: str):
-        return anthropic.count_tokens(content)
-
     def complete(
         self,
         prompt: str,
         history: Optional[List[tuple]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
```

### Comparing `pyllms-0.1.9/llms/providers/aleph.py` & `pyllms-0.2.0/llms/providers/aleph.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import itertools
 import os
 from aleph_alpha_client import Client, CompletionRequest, Prompt
 import time
 
 from typing import List, Optional
+from .base_provider import BaseProvider
 
 
-class AlephAlphaProvider:
+class AlephAlphaProvider(BaseProvider):
     MODEL_INFO = {
         "luminous-base": {"prompt": 6.6, "completion": 7.6, "token_limit": 2048},
         "luminous-extended": {"prompt": 9.9, "completion": 10.9, "token_limit": 2048},
         "luminous-supreme": {"prompt": 38.5, "completion": 42.5, "token_limit": 2048},
         "luminous-supreme-control": {
             "prompt": 48.5,
             "completion": 53.6,
@@ -22,20 +23,17 @@
 
     def __init__(self, api_key=None, model=None):
         if api_key is None:
             api_key = os.getenv("ALEPHALPHA_API_KEY")
         self.client = Client(api_key)
 
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
-
     def complete(
         self,
         prompt: str,
         history: Optional[List[tuple]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
```

### Comparing `pyllms-0.1.9/llms/providers/anthropic.py` & `pyllms-0.2.0/llms/providers/anthropic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,76 @@
 # llms/providers/anthropic.py
 
 import itertools
+import json
 import os
-import anthropic
 import time
+import aiohttp
+import anthropic
+
+from typing import Dict, List, Optional, Tuple, Union
+from anthropic.api import _process_request_error
+from .base_provider import BaseProvider
+
 
-from typing import List, Optional
+class AnthropicClient(anthropic.Client):
+    """Extend Anthropic Client class to accept aiosession"""
+
+    async def _arequest_as_json(
+        self,
+        method: str,
+        path: str,
+        params: dict,
+        headers: Optional[Dict[str, str]] = None,
+        request_timeout: Optional[Union[float, Tuple[float, float]]] = None,
+        aiosession: Optional[aiohttp.ClientSession] = None,
+    ) -> dict:
+        if aiosession is None:
+            super()._arequest_as_json(
+                method=method,
+                path=path,
+                params=params,
+                headers=headers,
+                request_timeout=request_timeout,
+            )
+        else:
+            request = self._request_params(
+                headers, method, params, path, request_timeout
+            )
+            async with aiosession.request(
+                request.method,
+                request.url,
+                headers=request.headers,
+                data=request.data,
+                timeout=request.timeout,
+            ) as result:
+                content = await result.text()
+                if result.status != 200:
+                    _process_request_error(method, content, result.status)
+                json_body = json.loads(content)
+                return json_body
 
 
-class AnthropicProvider:
+class AnthropicProvider(BaseProvider):
     MODEL_INFO = {
         "claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
         "claude-v1": {"prompt": 11.02, "completion": 32.68, "token_limit": 9000},
     }
 
     def __init__(self, api_key=None, model=None):
-        
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
         if api_key is None:
             api_key = os.getenv("ANTHROPIC_API_KEY")
-        self.client = anthropic.Client(api_key)
-
-
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
+        self.client = AnthropicClient(api_key)
 
     def count_tokens(self, content: str):
-        raise ValueError("Count tokens is currently not supported with AI21")
+        return anthropic.count_tokens(content)
 
     def complete(
         self,
         prompt: str,
         history: Optional[List[tuple]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
@@ -157,14 +194,15 @@
 
     def complete_stream(
         self,
         prompt: str,
         history: Optional[List[tuple]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
+        stop_sequences: Optional[List[str]] = None,
         **kwargs,
     ):
         formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
             history_prompt = "".join(
@@ -176,17 +214,20 @@
             kwargs[
                 "max_tokens_to_sample"
             ] = max_tokens  # Add maxTokens to kwargs if not present
 
         if "stream" not in kwargs:
             kwargs["stream"] = True  # Add stream param if not present
 
+        if stop_sequences is None:
+            stop_sequences = [anthropic.HUMAN_PROMPT]
+
         response = self.client.completion_stream(
             prompt=formatted_prompt,
-            stop_sequences=[anthropic.HUMAN_PROMPT],
+            stop_sequences=stop_sequences,
             temperature=temperature,
             model=self.model,
             **kwargs,
         )
 
         last_completion = ""
         for data in response:
```

### Comparing `pyllms-0.1.9/llms/providers/cohere.py` & `pyllms-0.2.0/llms/providers/cohere.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 
 import itertools
 import os
 import cohere
 import time
 
 from typing import List, Optional
+from .base_provider import BaseProvider
 
 
-class CohereProvider:
+class CohereProvider(BaseProvider):
     MODEL_INFO = {
-        "command-xlarge-beta": {"prompt": 25.0, "completion": 25, "token_limit": 8192},
-        "command-xlarge-nightly": {"prompt": 25.0, "completion": 25, "token_limit": 8192},
+        "command-xlarge-beta": {"prompt": 25.0, "completion": 25, "token_limit": 2048},
+        "command-xlarge-nightly": {
+            "prompt": 25.0,
+            "completion": 25,
+            "token_limit": 4096,
+        },
     }
 
     def __init__(self, api_key=None, model=None):
         if api_key is None:
             api_key = os.getenv("COHERE_API_KEY")
         self.client = cohere.Client(api_key)
 
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
-
     def count_tokens(self, content: str):
         tokens = self.client.tokenize(content)
         return len(tokens)
 
     def complete(
         self,
         prompt: str,
```

### Comparing `pyllms-0.1.9/llms/providers/huggingface.py` & `pyllms-0.2.0/llms/providers/huggingface.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import itertools
 import os
 from huggingface_hub.inference_api import InferenceApi
 import time
 
 from typing import List, Optional
+from .base_provider import BaseProvider
 
 
 class HuggingfaceHubProvider:
     MODEL_INFO = {
         "hf_pythia": {
             "full": "OpenAssistant/oasst-sft-4-pythia-12b-epoch-3.5",
             "prompt": 0,
@@ -22,56 +23,52 @@
             "completion": 0,
             "token_limit": -1,
         },
     }
 
     def __init__(self, api_key=None, model=None):
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
 
         self.model = model
 
         if api_key is None:
             api_key = os.getenv("HUGGINFACEHUB_API_KEY")
 
         self.client = InferenceApi(
             repo_id=self.MODEL_INFO[model]["full"], token=api_key
         )
 
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
-
     def complete(
         self,
         prompt: str,
         temperature: float = 0.01,
         max_tokens: int = 300,
         **kwargs,
     ):
         if self.model == "hf_pythia":
             prompt = "<|prompter|" + prompt + "<|endoftext|><|assistant|>"
 
-        if temperature <=0:
+        if temperature <= 0:
             temperature = 0.01
 
         if "temperature" not in kwargs:
             kwargs["temperature"] = temperature
 
         if "max_new_tokens" not in kwargs:
             kwargs["max_new_tokens"] = max_tokens
 
         start_time = time.time()
         response = self.client(inputs=prompt, params={**kwargs})
         latency = time.time() - start_time
-        #print(response)
-        if 'error' in response:
-            print("Error: ", response['error'])
+        # print(response)
+        if "error" in response:
+            print("Error: ", response["error"])
             return {}
 
-
         completion = response[0]["generated_text"][len(prompt) :]
 
         # Calculate tokens and cost
         prompt_tokens = -1
         completion_tokens = -1
 
         total_tokens = prompt_tokens + completion_tokens
```

### Comparing `pyllms-0.1.9/llms/providers/openai.py` & `pyllms-0.2.0/llms/providers/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+import aiohttp
 import itertools
 import openai
 import tiktoken
 import time
 from typing import List, Optional
 
+from .base_provider import BaseProvider
 
-class OpenAIProvider:
+
+class OpenAIProvider(BaseProvider):
     # cost is per million tokens
     MODEL_INFO = {
         "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 4000},
         "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8000},
     }
 
     def __init__(self, api_key, model=None):
         openai.api_key = api_key
         if model is None:
-            model = list(MODEL_INFO.keys())[0]
+            model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
-    def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
-
     def count_tokens(self, content: str):
         enc = tiktoken.encoding_for_model(self.model)
         return len(enc.encode(content))
 
     def complete(
         self,
         prompt: str,
@@ -81,16 +81,20 @@
 
     async def acomplete(
         self,
         prompt: str,
         history: Optional[List[tuple]] = None,
         system_message: str = None,
         temperature: float = 0,
+        aiosession: Optional[aiohttp.ClientSession] = None,
         **kwargs,
     ):
+        if aiosession is not None:
+            openai.aiosession.set(aiosession)
+
         start_time = time.time()
 
         messages = [{"role": "user", "content": prompt}]
 
         if history:
             role_cycle = itertools.cycle(("user", "assistant"))
             history_messages = itertools.chain.from_iterable(history)
```

### Comparing `pyllms-0.1.9/pyllms.egg-info/PKG-INFO` & `pyllms-0.2.0/pyllms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.9
+Version: 0.2.0
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
@@ -28,15 +28,15 @@
 # PyLLMs
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
 PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph Alpha, HuggingfaceHub) with a built-in model performance benchmark. 
 
 It is ideal for fast prototyping and evaluating different models thanks to:
-- Connect to top LLMs in s few lines of code (currently OpenAI, Anthropic and AI21 are supported)
+- Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
@@ -57,20 +57,23 @@
 model = llms.init()
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
-Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+export COHERE_API_KEY="your_api_key_here"
+export ALEPHALPHA_API_KEY="your_api_key_here"
+export HUGGINFACEHUB_API_KEY="your_api_key_here"
 
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
@@ -92,49 +95,61 @@
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
 The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
-{'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
+{
+  'model': 'gpt-3.5-turbo', 
+  'tokens': 34, 
+  'tokens_prompt': 20, 
+  'tokens_completion': 14, 
+  'cost': '0.00007', 
+  'latency': 1.4
+}
 ```
 
 
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
-['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
+[
+ 'The capital of the country where Mozart was born is Vienna, Austria.', 
+ 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.'
+]
 
 >>> print(result.meta)
-[{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
+[
+ {'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, 
+ {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}
+]
+```
+
+## Async support
+Async completion is supported for compatible models. It is not supported in multi-models mode yet.
+```
+result = await model.acomplete("what is the capital of country where mozzart was born")
 ```
 
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
->>> model= llms.init('claude-v1')
->>> result = model.complete_stream("write an essay on civil war")
->>> for chunk in result:
-...        if chunk is not None:
-...          print(chunk, end='')   
-... 
-
-Here is a paragraph about civil rights:
-
-
-Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
-
+model= llms.init('claude-v1')
+result = model.complete_stream("write an essay on civil war")
+for chunk in result:
+   if chunk is not None:
+      print(chunk, end='')   
 ```
 
 Current limitations:
 - When streaming, 'meta' is not available
 - Multi-models are not supported for streaming
 
 
@@ -160,16 +175,18 @@
 2) Speed
 3) Cost
 
 PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'command-xlarge-nightly'])
+
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
+
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
 |             Model              |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)   |    Evaluation   |
 +--------------------------------+--------------------+---------------------+----------------------+-------------------------+-----------------+
@@ -236,36 +253,41 @@
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
 
 >>> model.list("gpt') # lists only models with 'gpt' in name/provider name
+```
+
+Here is a pretty table of supported models (in alphabetical order).
+```
 
 | Provider            | Name                   | Prompt Cost | Completion Cost | Token Limit |
 |---------------------|------------------------|-------------|-----------------|-------------|
 | AI21Provider        | j2-grande-instruct     |        10.0 |            10.0 |        8192 |
 | AI21Provider        | j2-jumbo-instruct      |        15.0 |            15.0 |        8192 |
 | AlephAlphaProvider  | luminous-base          |         6.6 |             7.6 |        2048 |
 | AlephAlphaProvider  | luminous-extended      |         9.9 |            10.9 |        2048 |
 | AlephAlphaProvider  | luminous-supreme       |        38.5 |            42.5 |        2048 |
 | AlephAlphaProvider  | luminous-supreme-control |      48.5 |            53.6 |        2048 |
 | AnthropicProvider   | claude-instant-v1      |        1.63 |            5.51 |        9000 |
 | AnthropicProvider   | claude-v1              |       11.02 |           32.68 |        9000 |
-| CohereProvider      | command-xlarge-beta    |          25 |              25 |        8192 |
-| CohereProvider      | command-xlarge-nightly |          25 |              25 |        8192 |
+| CohereProvider      | command-xlarge-beta    |        25.0 |            25.0 |        8192 |
+| CohereProvider      | command-xlarge-nightly |        25.0 |            25.0 |        8192 |
+| HuggingfaceHub      | hf_pythia              |         0.0 |             0.0 |        2048 |
 | OpenAIProvider      | gpt-3.5-turbo          |         2.0 |             2.0 |        4000 |
 | OpenAIProvider      | gpt-4                  |        30.0 |            60.0 |        8000 |
 
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
-[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
-[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)
+[AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)\
+[Cohere documentation](https://cohere-sdk.readthedocs.io/en/latest/cohere.html#api)\
 [Aleph Alpha documentation](https://aleph-alpha-client.readthedocs.io/en/latest/aleph_alpha_client.html#aleph_alpha_client.CompletionRequest)
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.1.9/setup.py` & `pyllms-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.9",
+    version="0.2.0",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

