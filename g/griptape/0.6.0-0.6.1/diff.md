# Comparing `tmp/griptape-0.6.0.tar.gz` & `tmp/griptape-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.6.0.tar", max compression
+gzip compressed data, was "griptape-0.6.1.tar", max compression
```

## Comparing `griptape-0.6.0.tar` & `griptape-0.6.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.6.0/LICENSE
--rw-r--r--   0        0        0     3948 2023-04-24 16:47:45.514675 griptape-0.6.0/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.6.0/griptape/__init__.py
--rw-r--r--   0        0        0      241 2023-04-23 17:45:35.146322 griptape-0.6.0/griptape/adapters/__init__.py
--rw-r--r--   0        0        0      218 2023-04-24 18:12:25.680142 griptape-0.6.0/griptape/adapters/base_adapter.py
--rw-r--r--   0        0        0     2642 2023-04-24 19:03:51.310926 griptape-0.6.0/griptape/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1003 2023-04-24 18:12:25.650475 griptape-0.6.0/griptape/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      309 2023-04-24 18:12:25.669734 griptape-0.6.0/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0      149 2023-04-24 16:38:24.945579 griptape-0.6.0/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      458 2023-04-24 18:12:25.682521 griptape-0.6.0/griptape/artifacts/error_output.py
--rw-r--r--   0        0        0      440 2023-04-24 18:12:25.667144 griptape-0.6.0/griptape/artifacts/text_input.py
--rw-r--r--   0        0        0      487 2023-04-24 18:12:25.686120 griptape-0.6.0/griptape/artifacts/text_output.py
--rw-r--r--   0        0        0      107 2023-04-24 19:02:43.266538 griptape-0.6.0/griptape/core/__init__.py
--rw-r--r--   0        0        0     5142 2023-04-24 18:12:25.668816 griptape-0.6.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      529 2023-04-16 19:45:11.589553 griptape-0.6.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      765 2023-04-24 18:12:25.643316 griptape-0.6.0/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.6.0/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.6.0/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.6.0/griptape/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.6.0/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1186 2023-04-24 18:12:25.666029 griptape-0.6.0/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1307 2023-04-24 18:12:25.656929 griptape-0.6.0/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1950 2023-04-24 18:12:25.630445 griptape-0.6.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1727 2023-04-24 18:12:25.681575 griptape-0.6.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     3077 2023-04-24 18:12:25.677566 griptape-0.6.0/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.6.0/griptape/executors/__init__.py
--rw-r--r--   0        0        0      840 2023-04-24 19:03:51.304633 griptape-0.6.0/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3080 2023-04-24 19:03:51.306144 griptape-0.6.0/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     1905 2023-04-24 19:03:51.303111 griptape-0.6.0/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.6.0/griptape/memory/__init__.py
--rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.6.0/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.6.0/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.6.0/griptape/memory/run.py
--rw-r--r--   0        0        0     2011 2023-04-24 18:12:25.671465 griptape-0.6.0/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      156 2023-04-23 17:45:35.149028 griptape-0.6.0/griptape/middleware/__init__.py
--rw-r--r--   0        0        0      188 2023-04-21 21:53:47.740258 griptape-0.6.0/griptape/middleware/base_middleware.py
--rw-r--r--   0        0        0      160 2023-04-24 18:12:25.683755 griptape-0.6.0/griptape/middleware/storage_middleware.py
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.6.0/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.6.0/griptape/rules/__init__.py
--rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.6.0/griptape/rules/json.py
--rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.6.0/griptape/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.6.0/griptape/rules/rule.py
--rw-r--r--   0        0        0     1876 2023-04-23 23:15:24.558398 griptape-0.6.0/griptape/schemas/__init__.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.6.0/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.6.0/griptape/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.6.0/griptape/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.6.0/griptape/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.6.0/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.6.0/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.6.0/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.6.0/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.6.0/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.6.0/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.6.0/griptape/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.0/griptape/schemas/structures/__init__.py
--rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.6.0/griptape/schemas/structures/agent_schema.py
--rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.6.0/griptape/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.6.0/griptape/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.6.0/griptape/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.0/griptape/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.6.0/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.6.0/griptape/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.6.0/griptape/schemas/tasks/__init__.py
--rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.6.0/griptape/schemas/tasks/prompt_task_schema.py
--rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.6.0/griptape/schemas/tasks/task_schema.py
--rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.6.0/griptape/schemas/tasks/toolkit_task_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.0/griptape/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.6.0/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.6.0/griptape/structures/__init__.py
--rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.6.0/griptape/structures/agent.py
--rw-r--r--   0        0        0     2886 2023-04-24 18:12:25.641492 griptape-0.6.0/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     3803 2023-04-24 18:12:25.635132 griptape-0.6.0/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.6.0/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     3048 2023-04-24 18:12:25.653947 griptape-0.6.0/griptape/structures/workflow.py
--rw-r--r--   0        0        0      197 2023-04-24 18:12:25.651772 griptape-0.6.0/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      939 2023-04-24 18:12:25.674815 griptape-0.6.0/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      466 2023-04-23 22:46:42.629051 griptape-0.6.0/griptape/summarizers/summarizer.py
--rw-r--r--   0        0        0      286 2023-04-23 22:37:19.590856 griptape-0.6.0/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     3747 2023-04-24 18:12:25.663488 griptape-0.6.0/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     1678 2023-04-24 18:12:25.655397 griptape-0.6.0/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     6093 2023-04-24 19:03:51.309485 griptape-0.6.0/griptape/tasks/tool_subtask.py
--rw-r--r--   0        0        0     3041 2023-04-24 19:03:51.301381 griptape-0.6.0/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.6.0/griptape/templates/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.6.0/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0     1502 2023-04-23 22:36:52.421821 griptape-0.6.0/griptape/templates/prompts/base.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.6.0/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.6.0/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.6.0/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.6.0/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.6.0/griptape/templates/prompts/tasks/prompt.j2
--rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.6.0/griptape/templates/prompts/tasks/tool/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.6.0/griptape/templates/prompts/tasks/tool/subtasks.j2
--rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.6.0/griptape/templates/prompts/tasks/tool/tool.j2
--rw-r--r--   0        0        0      255 2023-04-18 17:19:47.832750 griptape-0.6.0/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.6.0/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.6.0/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.6.0/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.6.0/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.6.0/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.6.0/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      517 2023-04-23 21:35:35.626969 griptape-0.6.0/griptape/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape-0.6.0/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.6.0/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.6.0/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.6.0/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.6.0/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.6.0/griptape/utils/python_runner.py
--rw-r--r--   0        0        0      678 2023-04-24 19:03:51.307687 griptape-0.6.0/griptape/utils/tool_loader.py
--rw-r--r--   0        0        0      967 2023-04-24 19:20:20.920342 griptape-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 griptape-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3948 2023-04-24 16:47:45.514675 griptape-0.6.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.6.1/griptape/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-23 17:45:35.146322 griptape-0.6.1/griptape/adapters/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-24 18:12:25.680142 griptape-0.6.1/griptape/adapters/base_adapter.py
+-rw-r--r--   0        0        0     2642 2023-04-24 19:03:51.310926 griptape-0.6.1/griptape/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1003 2023-04-24 18:12:25.650475 griptape-0.6.1/griptape/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      309 2023-04-24 18:12:25.669734 griptape-0.6.1/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0      149 2023-04-24 16:38:24.945579 griptape-0.6.1/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      458 2023-04-24 18:12:25.682521 griptape-0.6.1/griptape/artifacts/error_output.py
+-rw-r--r--   0        0        0      440 2023-04-24 18:12:25.667144 griptape-0.6.1/griptape/artifacts/text_input.py
+-rw-r--r--   0        0        0      487 2023-04-24 18:12:25.686120 griptape-0.6.1/griptape/artifacts/text_output.py
+-rw-r--r--   0        0        0      107 2023-04-24 19:02:43.266538 griptape-0.6.1/griptape/core/__init__.py
+-rw-r--r--   0        0        0     5142 2023-04-24 18:12:25.668816 griptape-0.6.1/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      529 2023-04-16 19:45:11.589553 griptape-0.6.1/griptape/core/decorators.py
+-rw-r--r--   0        0        0      765 2023-04-24 18:12:25.643316 griptape-0.6.1/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.6.1/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.6.1/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.6.1/griptape/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.6.1/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1186 2023-04-24 18:12:25.666029 griptape-0.6.1/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1307 2023-04-24 18:12:25.656929 griptape-0.6.1/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1950 2023-04-24 18:12:25.630445 griptape-0.6.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1727 2023-04-24 18:12:25.681575 griptape-0.6.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     3077 2023-04-24 18:12:25.677566 griptape-0.6.1/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.6.1/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-24 21:08:44.879753 griptape-0.6.1/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3080 2023-04-24 19:03:51.306144 griptape-0.6.1/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     1905 2023-04-24 19:03:51.303111 griptape-0.6.1/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.6.1/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.6.1/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.6.1/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.6.1/griptape/memory/run.py
+-rw-r--r--   0        0        0     2011 2023-04-24 18:12:25.671465 griptape-0.6.1/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      156 2023-04-23 17:45:35.149028 griptape-0.6.1/griptape/middleware/__init__.py
+-rw-r--r--   0        0        0      188 2023-04-21 21:53:47.740258 griptape-0.6.1/griptape/middleware/base_middleware.py
+-rw-r--r--   0        0        0      210 2023-04-24 21:08:44.883031 griptape-0.6.1/griptape/middleware/storage_middleware.py
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.6.1/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.6.1/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.6.1/griptape/rules/json.py
+-rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.6.1/griptape/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.6.1/griptape/rules/rule.py
+-rw-r--r--   0        0        0     1876 2023-04-23 23:15:24.558398 griptape-0.6.1/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.6.1/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.6.1/griptape/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.6.1/griptape/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.6.1/griptape/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.6.1/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.6.1/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.6.1/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.6.1/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.6.1/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.6.1/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.6.1/griptape/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.6.1/griptape/schemas/structures/agent_schema.py
+-rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.6.1/griptape/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.6.1/griptape/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.6.1/griptape/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.6.1/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.6.1/griptape/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.6.1/griptape/schemas/tasks/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.6.1/griptape/schemas/tasks/prompt_task_schema.py
+-rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.6.1/griptape/schemas/tasks/task_schema.py
+-rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.6.1/griptape/schemas/tasks/toolkit_task_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.6.1/griptape/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.6.1/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.6.1/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.6.1/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2886 2023-04-24 18:12:25.641492 griptape-0.6.1/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     3803 2023-04-24 18:12:25.635132 griptape-0.6.1/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.6.1/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     3048 2023-04-24 18:12:25.653947 griptape-0.6.1/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      197 2023-04-24 18:12:25.651772 griptape-0.6.1/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      939 2023-04-24 18:12:25.674815 griptape-0.6.1/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      466 2023-04-23 22:46:42.629051 griptape-0.6.1/griptape/summarizers/summarizer.py
+-rw-r--r--   0        0        0      286 2023-04-23 22:37:19.590856 griptape-0.6.1/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     3747 2023-04-24 18:12:25.663488 griptape-0.6.1/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     1678 2023-04-24 18:12:25.655397 griptape-0.6.1/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     6093 2023-04-24 19:03:51.309485 griptape-0.6.1/griptape/tasks/tool_subtask.py
+-rw-r--r--   0        0        0     3041 2023-04-24 19:03:51.301381 griptape-0.6.1/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.6.1/griptape/templates/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.6.1/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0     1502 2023-04-23 22:36:52.421821 griptape-0.6.1/griptape/templates/prompts/base.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.6.1/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.6.1/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.6.1/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.6.1/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.6.1/griptape/templates/prompts/tasks/prompt.j2
+-rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.6.1/griptape/templates/prompts/tasks/tool/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.6.1/griptape/templates/prompts/tasks/tool/subtasks.j2
+-rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.6.1/griptape/templates/prompts/tasks/tool/tool.j2
+-rw-r--r--   0        0        0      255 2023-04-18 17:19:47.832750 griptape-0.6.1/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.6.1/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.6.1/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.6.1/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.6.1/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.6.1/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.6.1/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      517 2023-04-23 21:35:35.626969 griptape-0.6.1/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape-0.6.1/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.6.1/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.6.1/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.6.1/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.6.1/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.6.1/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0      678 2023-04-24 19:03:51.307687 griptape-0.6.1/griptape/utils/tool_loader.py
+-rw-r--r--   0        0        0      972 2023-04-24 23:57:13.527389 griptape-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 griptape-0.6.1/PKG-INFO
```

### Comparing `griptape-0.6.0/LICENSE` & `griptape-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/README.md` & `griptape-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/adapters/chatgpt_plugin_adapter.py` & `griptape-0.6.1/griptape/adapters/chatgpt_plugin_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/adapters/langchain_tool_adapter.py` & `griptape-0.6.1/griptape/adapters/langchain_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/core/base_tool.py` & `griptape-0.6.1/griptape/core/base_tool.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/core/decorators.py` & `griptape-0.6.1/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/__init__.py` & `griptape-0.6.1/griptape/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.6.1/griptape/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.6.1/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.6.1/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.6.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.6.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.6.1/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/executors/base_executor.py` & `griptape-0.6.1/griptape/executors/base_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
         return result
 
     def before_execute(self, tool_action: callable, value: bytes) -> bytes:
         return value
 
     def after_execute(self, tool_action: callable, result: bytes) -> bytes:
+        tool: BaseTool = tool_action.__self__
+
+        middleware = tool.middleware.get(tool_action)
+
+        if middleware:
+            result = middleware.process_output(result)
+
         return result
 
     @abstractmethod
     def try_execute(self, tool_action: callable, value: bytes) -> bytes:
         ...
 
     def tool_dir(self, tool: BaseTool):
```

### Comparing `griptape-0.6.0/griptape/executors/docker_executor.py` & `griptape-0.6.1/griptape/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/executors/local_executor.py` & `griptape-0.6.1/griptape/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/memory/buffer_memory.py` & `griptape-0.6.1/griptape/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/memory/memory.py` & `griptape-0.6.1/griptape/memory/memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/memory/summary_memory.py` & `griptape-0.6.1/griptape/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/schemas/__init__.py` & `griptape-0.6.1/griptape/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/schemas/drivers/openai_prompt_driver_schema.py` & `griptape-0.6.1/griptape/schemas/drivers/openai_prompt_driver_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/schemas/polymorphic_schema.py` & `griptape-0.6.1/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/schemas/tasks/toolkit_task_schema.py` & `griptape-0.6.1/griptape/schemas/tasks/toolkit_task_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/structures/agent.py` & `griptape-0.6.1/griptape/structures/agent.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/structures/pipeline.py` & `griptape-0.6.1/griptape/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/structures/structure.py` & `griptape-0.6.1/griptape/structures/structure.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/structures/structure_with_memory.py` & `griptape-0.6.1/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/structures/workflow.py` & `griptape-0.6.1/griptape/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/summarizers/prompt_driver_summarizer.py` & `griptape-0.6.1/griptape/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tasks/base_task.py` & `griptape-0.6.1/griptape/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tasks/prompt_task.py` & `griptape-0.6.1/griptape/tasks/prompt_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tasks/tool_subtask.py` & `griptape-0.6.1/griptape/tasks/tool_subtask.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tasks/toolkit_task.py` & `griptape-0.6.1/griptape/tasks/toolkit_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/templates/prompts/base.j2` & `griptape-0.6.1/griptape/templates/prompts/base.j2`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tokenizers/base_tokenizer.py` & `griptape-0.6.1/griptape/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.6.1/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.6.1/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.6.1/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/utils/__init__.py` & `griptape-0.6.1/griptape/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/utils/j2.py` & `griptape-0.6.1/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/utils/python_runner.py` & `griptape-0.6.1/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/griptape/utils/tool_loader.py` & `griptape-0.6.1/griptape/utils/tool_loader.py`

 * *Files identical despite different names*

### Comparing `griptape-0.6.0/pyproject.toml` & `griptape-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.6.0"
+version = "0.6.1"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
@@ -40,8 +40,8 @@
 pytest = "~=7.1"
 pytest-mock = "*"
 pytest-cover = "*"
 twine = ">=4"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `griptape-0.6.0/PKG-INFO` & `griptape-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.6.0
+Version: 0.6.1
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

