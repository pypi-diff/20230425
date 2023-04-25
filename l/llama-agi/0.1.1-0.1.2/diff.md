# Comparing `tmp/llama_agi-0.1.1.tar.gz` & `tmp/llama_agi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_agi-0.1.1.tar", max compression
+gzip compressed data, was "llama_agi-0.1.2.tar", max compression
```

## Comparing `llama_agi-0.1.1.tar` & `llama_agi-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1093 2023-04-24 02:20:57.763744 llama_agi-0.1.1/LICENSE
--rw-r--r--   0        0        0     1865 2023-04-24 02:20:57.763744 llama_agi-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/__init__.py
--rw-r--r--   0        0        0     4588 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/default_task_prompts.py
--rw-r--r--   0        0        0     2471 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/execution_agent/SimpleExecutionAgent.py
--rw-r--r--   0        0        0     3306 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/execution_agent/ToolExecutionAgent.py
--rw-r--r--   0        0        0      177 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/execution_agent/__init__.py
--rw-r--r--   0        0        0     1991 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/execution_agent/base.py
--rw-r--r--   0        0        0     3007 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/runners/AutoAGIRunner.py
--rw-r--r--   0        0        0     5088 2023-04-24 04:16:41.753772 llama_agi-0.1.1/llama_agi/runners/AutoStreamlitAGIRunner.py
--rw-r--r--   0        0        0      166 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/runners/__init__.py
--rw-r--r--   0        0        0      692 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/runners/base.py
--rw-r--r--   0        0        0     6990 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/task_manager/LlamaTaskManager.py
--rw-r--r--   0        0        0       87 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/task_manager/__init__.py
--rw-r--r--   0        0        0     2446 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/task_manager/base.py
--rw-r--r--   0        0        0      721 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/tools/NoteTakingTools.py
--rw-r--r--   0        0        0     1188 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/tools/WebpageSearchTool.py
--rw-r--r--   0        0        0      178 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/tools/__init__.py
--rw-r--r--   0        0        0     1261 2023-04-24 02:20:57.763744 llama_agi-0.1.1/llama_agi/utils.py
--rw-r--r--   0        0        0     1050 2023-04-24 04:18:37.503772 llama_agi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 llama_agi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-24 02:20:57.763744 llama_agi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1865 2023-04-24 02:20:57.763744 llama_agi-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/__init__.py
+-rw-r--r--   0        0        0     4588 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/default_task_prompts.py
+-rw-r--r--   0        0        0     2471 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/SimpleExecutionAgent.py
+-rw-r--r--   0        0        0     3306 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/ToolExecutionAgent.py
+-rw-r--r--   0        0        0      177 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/__init__.py
+-rw-r--r--   0        0        0     1991 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/base.py
+-rw-r--r--   0        0        0     3007 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/AutoAGIRunner.py
+-rw-r--r--   0        0        0     5245 2023-04-25 01:24:45.683530 llama_agi-0.1.2/llama_agi/runners/AutoStreamlitAGIRunner.py
+-rw-r--r--   0        0        0      166 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/__init__.py
+-rw-r--r--   0        0        0      692 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/base.py
+-rw-r--r--   0        0        0     6990 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/LlamaTaskManager.py
+-rw-r--r--   0        0        0       87 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/__init__.py
+-rw-r--r--   0        0        0     2446 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/base.py
+-rw-r--r--   0        0        0      721 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/NoteTakingTools.py
+-rw-r--r--   0        0        0     1188 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/WebpageSearchTool.py
+-rw-r--r--   0        0        0      178 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/__init__.py
+-rw-r--r--   0        0        0     1261 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/utils.py
+-rw-r--r--   0        0        0     1052 2023-04-25 01:30:58.533532 llama_agi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 llama_agi-0.1.2/PKG-INFO
```

### Comparing `llama_agi-0.1.1/LICENSE` & `llama_agi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/README.md` & `llama_agi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/default_task_prompts.py` & `llama_agi-0.1.2/llama_agi/default_task_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/execution_agent/SimpleExecutionAgent.py` & `llama_agi-0.1.2/llama_agi/execution_agent/SimpleExecutionAgent.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/execution_agent/ToolExecutionAgent.py` & `llama_agi-0.1.2/llama_agi/execution_agent/ToolExecutionAgent.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/execution_agent/base.py` & `llama_agi-0.1.2/llama_agi/execution_agent/base.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/runners/AutoAGIRunner.py` & `llama_agi-0.1.2/llama_agi/runners/AutoAGIRunner.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/runners/AutoStreamlitAGIRunner.py` & `llama_agi-0.1.2/llama_agi/runners/AutoStreamlitAGIRunner.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,112 +25,111 @@
         self,
         objective: str,
         initial_task: str,
         sleep_time: int,
         initial_task_list: Optional[List[str]] = None,
         max_iterations: Optional[int] = None
     ) -> None:
+        
+        run_initial_task = False
+        if 'logs' not in st.session_state:
+            st.session_state['logs'] = []
+            st.session_state['state_str'] = "No state yet!"
+            st.session_state['tasks_summary'] = ""
+            run_initial_task = True
+
         logs_col, state_col = st.columns(2)
 
-        logs = []
         with logs_col:
             st.subheader("Execution Log")
             st_logs = st.empty()
-        st_logs.write("No logs yet!")
+        st_logs.write(st.session_state['logs'])
         
         with state_col:
             st.subheader("AGI State")
             st_state = st.empty()
-        st_state.write("No state yet!")
+        st_state.write(st.session_state['state_str'])
 
-        # get initial list of tasks
-        if initial_task_list:
-            self.task_manager.add_new_tasks(initial_task_list)
-        else:
-            initial_completed_tasks_summary = (
-                self.task_manager.get_completed_tasks_summary()
-            )
-            initial_task_prompt = initial_task + "\nReturn the list as an array."
+        if run_initial_task:
+            # get initial list of tasks
+            if initial_task_list:
+                self.task_manager.add_new_tasks(initial_task_list)
+            else:
+                initial_completed_tasks_summary = (
+                    self.task_manager.get_completed_tasks_summary()
+                )
+                initial_task_prompt = initial_task + "\nReturn the list as an array."
 
-            # create simple execution agent using current agent
-            simple_execution_agent = SimpleExecutionAgent(
-                llm=self.execution_agent._llm,
-                max_tokens=self.execution_agent.max_tokens,
-                prompts=self.execution_agent.prompts,
-            )
-            initial_task_list_result = simple_execution_agent.execute_task(
-                objective=objective,
-                task=initial_task_prompt,
-                completed_tasks_summary=initial_completed_tasks_summary,
-            )
+                # create simple execution agent using current agent
+                simple_execution_agent = SimpleExecutionAgent(
+                    llm=self.execution_agent._llm,
+                    max_tokens=self.execution_agent.max_tokens,
+                    prompts=self.execution_agent.prompts,
+                )
+                initial_task_list_result = simple_execution_agent.execute_task(
+                    objective=objective,
+                    task=initial_task_prompt,
+                    completed_tasks_summary=initial_completed_tasks_summary,
+                )
 
-            initial_task_list = self.task_manager.parse_task_list(initial_task_list_result['output'])
+                initial_task_list = self.task_manager.parse_task_list(initial_task_list_result['output'])
 
-            # add tasks to the task manager
-            self.task_manager.add_new_tasks(initial_task_list)
+                # add tasks to the task manager
+                self.task_manager.add_new_tasks(initial_task_list)
 
-        # prioritize initial tasks
-        self.task_manager.prioritize_tasks(objective)
+            # prioritize initial tasks
+            self.task_manager.prioritize_tasks(objective)
 
-        completed_tasks_summary = initial_completed_tasks_summary
-
-        # update streamlit state
-        state_str = log_current_status(initial_task, initial_task_list_result['output'], completed_tasks_summary, self.task_manager.current_tasks, return_str=True)
-        if state_str:
-            st_state.markdown(state_str.replace("\n", "\n\n"))
-
-        iteration = 0
-        paused = False
-        while True:
-            if paused and st.button(f"Continue for {max_iterations} more steps?"):
-                paused = False
-                st.success("Continuing..")
-            else:
-                iteration += 1
+            tasks_summary = initial_completed_tasks_summary
+            st.session_state['tasks_summary'] = tasks_summary
 
-                # Get the next task
-                cur_task = self.task_manager.get_next_task()
+            # update streamlit state
+            st.session_state['state_str'] = log_current_status(initial_task, initial_task_list_result['output'], tasks_summary, self.task_manager.current_tasks, return_str=True)
+            if st.session_state['state_str']:
+                st_state.markdown(st.session_state['state_str'].replace("\n", "\n\n"))
 
-                # Execute current task
-                result_dict = self.execution_agent.execute_task(
-                    objective=objective,
-                    cur_task=cur_task,
-                    completed_tasks_summary=completed_tasks_summary,
-                )
-                result = result_dict['output']
-                
-                # update logs 
-                log = make_intermediate_steps_pretty(json.dumps(result_dict['intermediate_steps'])) + [result]
-                logs.append(log)
-                st_logs.write(log)
-
-                # store the task and result as completed
-                self.task_manager.add_completed_task(cur_task, result)
-
-                # generate new task(s), if needed
-                self.task_manager.generate_new_tasks(objective, cur_task, result)
-
-                # Summarize completed tasks
-                completed_tasks_summary = self.task_manager.get_completed_tasks_summary()
-
-                # log state of AGI to streamlit
-                state_str = log_current_status(
-                    cur_task,
-                    result,
-                    completed_tasks_summary,
-                    self.task_manager.current_tasks,
-                    return_str=True
-                )
-                if state_str is not None:
-                    st_state.markdown(state_str.replace("\n", "\n\n"))
+        for _ in range(0, max_iterations):
+            # Get the next task
+            cur_task = self.task_manager.get_next_task()
 
-                # Quit the loop?
-                if len(self.task_manager.current_tasks) == 0:
-                    st.success("Out of tasks! Objective Accomplished?")
-                    break
-
-                if max_iterations is not None and iteration % max_iterations == 0:
-                    st.warning("Reached max iterations, pausing!")
-                    paused = True
+            # Execute current task
+            result_dict = self.execution_agent.execute_task(
+                objective=objective,
+                cur_task=cur_task,
+                completed_tasks_summary=st.session_state['tasks_summary'],
+            )
+            result = result_dict['output']
+            
+            # update logs 
+            log = make_intermediate_steps_pretty(json.dumps(result_dict['intermediate_steps'])) + [result]
+            st.session_state['logs'].append(log)
+            st_logs.write(st.session_state['logs'])
+
+            # store the task and result as completed
+            self.task_manager.add_completed_task(cur_task, result)
+
+            # generate new task(s), if needed
+            self.task_manager.generate_new_tasks(objective, cur_task, result)
+
+            # Summarize completed tasks
+            completed_tasks_summary = self.task_manager.get_completed_tasks_summary()
+            st.session_state['tasks_summary'] = completed_tasks_summary
+
+            # log state of AGI to streamlit
+            st.session_state['state_str'] = log_current_status(
+                cur_task,
+                result,
+                completed_tasks_summary,
+                self.task_manager.current_tasks,
+                return_str=True
+            )
+            if st.session_state['state_str'] is not None:
+                st_state.markdown(st.session_state['state_str'].replace("\n", "\n\n"))
 
-                # wait a bit to let you read what's happening
-                time.sleep(sleep_time)
+            # Quit the loop?
+            if len(self.task_manager.current_tasks) == 0:
+                st.success("Out of tasks! Objective Accomplished?")
+                break
+
+            # wait a bit to let you read what's happening
+            time.sleep(sleep_time)
+
```

### Comparing `llama_agi-0.1.1/llama_agi/runners/base.py` & `llama_agi-0.1.2/llama_agi/runners/base.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/task_manager/LlamaTaskManager.py` & `llama_agi-0.1.2/llama_agi/task_manager/LlamaTaskManager.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/task_manager/base.py` & `llama_agi-0.1.2/llama_agi/task_manager/base.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/tools/NoteTakingTools.py` & `llama_agi-0.1.2/llama_agi/tools/NoteTakingTools.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/tools/WebpageSearchTool.py` & `llama_agi-0.1.2/llama_agi/tools/WebpageSearchTool.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/llama_agi/utils.py` & `llama_agi-0.1.2/llama_agi/utils.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.1/pyproject.toml` & `llama_agi-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llama_agi"
-version = "0.1.1"
+version = "0.1.2"
 description = "Building AGI loops using LlamaIndex and Langchain"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/run-llama/llama-lab/tree/main/llama_agi"
 include = [
     "LICENSE",
@@ -42,8 +42,8 @@
     ".ruff_cache",
     "examples",
     "notebooks",
 ]
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `llama_agi-0.1.1/PKG-INFO` & `llama_agi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-agi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Building AGI loops using LlamaIndex and Langchain
 Home-page: https://github.com/run-llama/llama-lab/tree/main/llama_agi
 License: MIT
 Keywords: LLM,LlamaIndex,Langchain,AGI
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

