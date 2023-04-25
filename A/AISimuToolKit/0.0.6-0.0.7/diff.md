# Comparing `tmp/AISimuToolKit-0.0.6.tar.gz` & `tmp/AISimuToolKit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.0.6.tar", last modified: Sun Apr 23 13:50:25 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.0.7.tar", last modified: Tue Apr 25 13:10:41 2023, max compression
```

## Comparing `AISimuToolKit-0.0.6.tar` & `AISimuToolKit-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,27 @@
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       85 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      112 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      307 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      434 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/base_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1317 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/finetune_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1273 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/instruct_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2091 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/probe_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2410 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/reflection_action.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       83 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      610 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/agent.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2769 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/memory.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6732 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/experiment.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/model/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      237 2023-04-23 08:27:14.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9510 2023-04-23 13:44:17.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/model.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2352 2023-04-23 13:48:33.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/register.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/store/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       39 2023-04-23 08:55:06.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/store/text/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       47 2023-04-23 08:54:42.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/text/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6494 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/text/logger.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/AISimuToolKit/utils/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      559 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/utils/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1369 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/utils/utils.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      902 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       44 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/setup.cfg
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1011 2023-04-23 13:50:23.000000 AISimuToolKit-0.0.6/setup.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.035383 AISimuToolKit-0.0.7/
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 13:38:26.000000 AISimuToolKit-0.0.7/AISimuToolKit/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/exp/
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      429 2023-04-25 04:52:37.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1477 2023-04-25 04:52:37.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1282 2023-04-22 13:38:26.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1913 2023-04-25 04:52:37.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/probe_action.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)    13036 2023-04-25 12:26:38.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     8808 2023-04-25 12:26:38.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     5252 2023-04-25 12:26:38.000000 AISimuToolKit-0.0.7/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/model/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9390 2023-04-25 04:52:37.000000 AISimuToolKit-0.0.7/AISimuToolKit/model/model.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2046 2023-04-23 15:29:38.000000 AISimuToolKit-0.0.7/AISimuToolKit/model/register.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit/utils/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1493 2023-04-23 14:56:39.000000 AISimuToolKit-0.0.7/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-25 13:10:41.031383 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-25 13:10:40.000000 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      582 2023-04-25 13:10:40.000000 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-25 13:10:40.000000 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      132 2023-04-25 13:10:40.000000 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-25 13:10:40.000000 AISimuToolKit-0.0.7/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-25 13:10:41.035383 AISimuToolKit-0.0.7/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-25 13:10:41.035383 AISimuToolKit-0.0.7/setup.cfg
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1102 2023-04-25 13:10:07.000000 AISimuToolKit-0.0.7/setup.py
```

### Comparing `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/finetune_action.py` & `AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/finetune_action.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+from typing import List
+
 from AISimuToolKit.exp.actions.base_action import BaseAction
 from AISimuToolKit.exp.experiment import Experiment
-from typing import List
 
 
 class FinetuneAction(BaseAction):
     """
     让Agent在给定的语料上微调, 这里的语料是memory中的question和answer
     """
-    
+
     def __init__(self, expe: Experiment):
         super().__init__(expe)
-        
+
     def run(self, finetunes: List[dict], *args, **kwargs):
         """
         对多个agent进行微调, num表示采用的memory数量
-        :param instructions:[{"agent_id":agent_id,"num":num}]
+        :param finetunes:[{"agent_id":agent_id,"num":num}]
         """
         # 每个都进行finetune
         for item in finetunes:
             self.finetune(agent_id=item['agent_id'],
                           num=item['num'])
-            
+
     def finetune(self,
                  agent_id: int,
                  num: int):
-        recent_memory = self.expe.agents[agent_id].memory.retrive_by_recentness(num)
-        
+        recent_memory = self.expe.agents[agent_id].memory.retrieve_by_recentness(num)
+        self.logger.info(f"start finetuning agent_{agent_id} based on recent {num} memories")
         # 需要把finetune所使用的memory存储起来, 以便后续查看
         self.expe.models[agent_id].finetune(exp=self.expe.id,
                                             path=self.expe.agents[agent_id].path,
                                             agent=agent_id,
                                             config=self.expe.agents[agent_id].config, datas=recent_memory)
+        self.logger.info(f"successfully finetuned agent_{agent_id} based on recent {num} memories")
```

### Comparing `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/instruct_action.py` & `AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/instruct_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,18 @@
         为多个agent下达指令
         :param instructions:[{"agent_id":agent_id,"question":question,"answer":answer}]
         :param args:
         :param kwargs:
         :return:
         """
         for item in instructions:
-            self.instruct(agent_id=int(item["agent_id"]), 
+            self.instruct(agent_id=int(item["agent_id"]),
                           question=item["question"],
                           answer=item["answer"])
 
-    def instruct(self, 
-                 agent_id: int, 
-                 question: str, 
+    def instruct(self,
+                 agent_id: int,
+                 question: str,
                  answer: str):
-        self.logger.info("written in agent_{}'s memory : question\n {}; \nanswer\n {}".format(agent_id, question, answer))
+        self.logger.info(
+            "written in agent_{}'s memory : question\n {}; \nanswer\n {}".format(agent_id, question, answer))
         self.expe.agents[agent_id].memory.store(interactant=self.interactant, question=question, answer=answer)
```

### Comparing `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/probe_action.py` & `AISimuToolKit-0.0.7/AISimuToolKit/exp/actions/probe_action.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 from typing import List
 
 from AISimuToolKit.exp.actions.base_action import BaseAction
 
+
 # TODO 探测的prompt应该需要实现可配置
 class ProbeAction(BaseAction):
     """
     运行过程中通过对话的形式检查agent的状态，该动作不会影响agent
     """
 
     def __init__(self, expe):
         super().__init__(expe)
 
     def run(self, probes: List[dict], *args, **kwargs):
         """
         为多个agent下达指令
-        :param probes:[{"agent_id":agent_id,"input":input, "prompt": prompt}]
+        :param probes:[{"agent_id":agent_id,"message":message, "prompt": prompt}]
         :param args:
         :param kwargs:
         :return:
         """
         answers = []
         for item in probes:
             agent_id = int(item["agent_id"])
-            input = item["input"]
+            input = item["message"]
             answer = self.probe(agent_id=agent_id, input=input, prompt=item["prompt"])
             answers.append(answer)
         return answers
 
     def probe(self,
-              agent_id: str,
+              agent_id: int,
               input: str,
-              prompt: str="Your name is {}\n Your profile: {}. Now I will interview you. \n{}"):
-        """_summary_ 采访, 不会留下记忆
-
-        Args:
-            agent_id (str): _description_
-            input (str): _description_
-            prompt (_type_, optional): _description_. Defaults to "Your name is {}\n Your profile: {}. Now I will interview you. \n{}". 需要根据任务自己设计
-
-        Returns:
-            _type_: _description_ 
+              prompt: str = "Your name is {}\n Your profile_list: {}. Now I will interview you. \n{}"):
+        """
+        采访, 不会留下记忆
+        :param agent_id:
+        :param input:
+        :param prompt: 需要根据任务自己设计
+        :return:
         """
         name = self.expe.agents[agent_id].name
-        profile = ''.join(self.expe.agents[agent_id].profile)
+        profile = ''.join(self.expe.agents[agent_id].profile_list)
         whole_input = prompt.format(name, profile, input)
         answer = self.expe.models[agent_id].chat(query=whole_input,
                                                  exp=self.expe.id,
                                                  agent=agent_id,
                                                  config=self.expe.agents[agent_id].config)
         self.logger.history("user probe: {}".format(input))
-        self.logger.history("whole input:\n {}".format(whole_input))
+        self.logger.history("whole message:\n {}".format(whole_input))
         self.logger.history("agent_{}: {}".format(agent_id, answer))
         return answer
```

### Comparing `AISimuToolKit-0.0.6/AISimuToolKit/model/model.py` & `AISimuToolKit-0.0.7/AISimuToolKit/model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import openai
-import requests
-from typing import List
-from AISimuToolKit.store.text.logger import Logger
-from AISimuToolKit.utils.utils import get_file_stream
 import json
 import os
+from typing import List
+
+import openai
+import requests
+
+from AISimuToolKit.store.logger import Logger
+
 
 # TODO 调整为model和toolkit继承不同的基类，但都继承自ApiBase
 class ApiBase:
     _instance = None  # 类变量用于存储单例实例
-    
+
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         if not hasattr(cls, 'logger'):
             cls.logger = Logger()
         return cls._instance
 
@@ -23,39 +25,38 @@
     def finetune(self, *args, **kwargs):
         """_summary_ 对某个实验下某个agent使用某个文件finetune
         
         Raises:
             NotImplementedError: _description_
         """
         raise NotImplementedError
-    
+
     @classmethod
     def get_backend(cls):
         raise NotImplementedError
 
 
 class PublicApiBase(ApiBase):
     """公开的, 只能chat"""
-    
+
     def finetune(self, *args, **kwargs):
         self.logger.warning("{} does not support finetune".format(self.get_backend()))
-    
+        raise NotImplementedError
 
 
 # @ModelApiRegister.register("chatgpt")
 class GPT_35_API(PublicApiBase):
-    
-    def __new__(cls, 
-                urls: List[str], 
-                conf: dict,
+
+    def __new__(cls,
+                config: dict,
                 *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            openai.api_base = urls[0]
-            openai.api_key = conf['key'][0]
+            openai.api_base = config['url'][0]
+            openai.api_key = config['key'][0]
         return cls._instance
 
     # TODO 加入多轮对话
     # TODO 设置system
     # TODO 测试长对话，目前没有找到返回为length的例子
     def chat(self, query: str, config: dict, *args, **kwargs):
         """
@@ -126,31 +127,31 @@
     @classmethod
     def get_backend(cls):
         return "GPT-3.5-turbo"
 
 
 class PrivateApiBase(ApiBase):
     """自己部署的, 可以finetune"""
-    
-    def __new__(cls, urls: List[str], *args, **kwargs):
+
+    def __new__(cls, config: dict, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls.urls = {url: None for url in urls}
+            cls.urls = {url: None for url in config['url']}
         return cls._instance
-        
+
     # TODO 维护一个字典, 采用某种策略选择url去chat或finetune以使最少load, 高效运行
-    def get_url(self, exp: str, agent: str=None):
+    def get_url(self, exp: str, agent: str = None):
         """
         从urls中选择一个代价最小的
         TODO agent=None表示这个实验还没创建...是否需要负载均衡地将每个实验放到不同的url上, 还是在每个url上复制一份
         """
         return list(self.urls.keys())[0]
 
     @classmethod
-    def memory2finetunedata(cls, datas, *args, **kwargs):
+    def memory2finetunedata(cls, datas: List[dict], *args, **kwargs):
         raise NotImplementedError
 
 
 # TODO 实现ChatGlmAPI
 class ChatGLMAPI(PrivateApiBase):
 
     def chat(self, *args, **kwargs):
@@ -161,113 +162,108 @@
 
     @classmethod
     def get_backend(cls):
         return "ChatGLM"
 
 
 class LLaMAAPI(PrivateApiBase):
-    
-    def __new__(cls, exp: str, agents: List[str], urls: List[str], *args, **kwargs):
+
+    def __new__(cls, exp: str, agents: List[str], config: dict, *args, **kwargs):
         """_summary_  
 
         Args:
             exp (str): _description_ 实验ID
             agents (List[str]): _description_ agents的IDs
 
         Returns:
             _type_: _description_
         """
         if cls._instance is None:
-            cls._instance = super().__new__(cls, urls=urls)
+            cls._instance = super().__new__(cls, config=config)
         cls._instance.new_exp(exp=exp, agents=agents)
         return cls._instance
-    
-    
-    def new_exp(self, exp: str, agents: List[str])-> bool:
+
+    def new_exp(self, exp: str, agents: List[str]) -> bool:
         """_summary_ 对接部署服务, 存储文件
 
         Args:
             exp (str): _description_
             agents (List): _description_
         """
         url = self.get_url(exp=exp)
         params = {"id": exp, "override": True}
-        response = requests.post(url=f'{url}/exp/new', params=params, 
+        response = requests.post(url=f'{url}/exp/new', params=params,
                                  json=[str(agent) for agent in agents])
-        if json.loads(response.text)['code']=='success':
+        if json.loads(response.text)['code'] == 'success':
             self.logger.info(f"{self.get_backend()} created exp_{exp} in {url} server !")
             return True
         else:
             raise Exception(f'{self.get_backend()} failed to create exp_{exp} in {url} server !')
-            return False
-        
 
-    def finetune(self, exp: str, agent: str, config: dict, 
+    def finetune(self, exp: str, agent: str, config: dict,
                  path: str, datas: List[dict]) -> bool:
         """
         LLaMA的数据格式是
         [{ "instruction": "Give three tips for staying healthy.",
-        "input": "", "output": "1. Eat a balanced }]
-        :param url:
+        "message": "", "output": "1. Eat a balanced "}]
+        :param config:
         :param agent:
         :param exp:
-        :param path 为agent的路径
-        :param datas 为记忆
+        :param path: 为agent的路径
+        :param datas: 为记忆
         """
         file_path = self.memory2finetunedata(datas=datas, path=path)
-        
+
         url = self.get_url(exp=exp, agent=agent)
         files = {'file': open(file_path, 'rb')}
         params = {"exp": exp, "agent": agent}
         for key in config:
             params[key] = config[key]
         response = requests.post(f'{url}/finetune', params=params, files=files)
         # TODO 测试一下返回值
-        if json.loads(response.text)['code']=='success':
+        if json.loads(response.text)['code'] == 'success':
             return True
         else:
             raise Exception(f'{self.get_backend()} failed to finetune exp_{exp} agent_{agent} in {url} server !')
-            return False
 
-    def chat(self, 
-             exp: str, agent: str, 
-             query: str, instruction: str=None, 
-             history: list=[],
+    def chat(self,
+             exp: str, agent: str,
+             query: str, instruction: str = None,
+             history: list = [],
              *args, **kwargs):
         # 在LLaMA中, instruction+query实际上对应其他模型的query
         # TODO 暂不支持history 还没使用
         url = self.get_url(exp=exp, agent=agent)
         params = {
-            "exp": exp, "agent": str(agent), 
+            "exp": exp, "agent": str(agent),
             "query": '', "instruction": query
         }
         response = requests.post(f'{url}/chat', params=params, json=history)
         # TODO 测试一下返回值
         return json.loads(response.text)['response']
 
-
     @classmethod
     def get_backend(cls):
         return "LLaMA"
 
     @classmethod
-    def memory2finetunedata(cls, datas: List[dict], path: str, *args, **kwargs)->str:
+    def memory2finetunedata(cls, datas: List[dict], path: str, *args, **kwargs) -> str:
         """_summary_ 将memory格式的数据转成模型特定的处理
 
         Args:
             datas (_type_): _description_
         """
         results = []
         for data in datas:
             results.append({
                 "instruction": data['question'],
-                "input": "",
+                "message": "",
                 "output": data['answer']
             })
         path = f'{path}/finetune'
         if not os.path.exists(path):
             os.makedirs(path)
         num = len(os.listdir(path))
-        file_path=f'{path}/{num}.jsonl'
+        file_path = f'{path}/{num}.jsonl'
         with open(file=file_path, mode='w', encoding="utf-8") as f:
             f.write(json.dumps(results, ensure_ascii=False))
         return file_path
```

### Comparing `AISimuToolKit-0.0.6/AISimuToolKit/utils/utils.py` & `AISimuToolKit-0.0.7/AISimuToolKit/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 @author: Guo Shiguang
 @software: PyCharm
 @file: utils.py
 @time: 2023/4/17 0:06
 """
 from datetime import datetime
+import json
 import yaml
 
 
 def generate_experiment_id():
     now = datetime.now()
     return "{}-{}-{}-{}-{}-{}".format(now.year, now.month, now.day, now.hour, now.minute, now.second)
 
@@ -28,32 +29,38 @@
 def get_fromat_len(num: int):
     """
     :param num 表示agent的个数 
     对agent ID(文件夹)的命名规范=>使用相同长度的进行编码
     避免出现 agent_1、agent_2、agent_11
     而统一编码为 agent_01、agent_02、agent_11
     """
-    return max(2, num//10+1)
+    return max(2, num // 10 + 1)
 
 
 def get_file_stream(file: str):
     """_summary_ 得到文件流, 用于传输给finetune
 
     Args:
         file (str): _description_
     """
     with open(file, 'rb') as f:
         return f
 
 
-def parse_yaml_config(path: str)->dict:
+def parse_yaml_config(path: str) -> dict:
     """_summary_ 
 
     Args:
         path (str): _description_ 文件位置
 
     Returns:
         dict: _description_
     """
-    with open(file=path, mode="r",encoding="utf-8") as f:
+    with open(file=path, mode="r", encoding="utf-8") as f:
         conf = yaml.load(f.read(), Loader=yaml.FullLoader)
     return conf
+
+
+
+def save_config(config: dict, path: str):
+    with open(path, "w") as f:
+        json.dump(config, f)
```

### Comparing `AISimuToolKit-0.0.6/setup.py` & `AISimuToolKit-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
-#-*- coding:utf-8 -*-
+# -*- coding:utf-8 -*-
 
-from setuptools import setup, find_packages            #这个包没有的可以pip一下
+from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
-    name = "AISimuToolKit",      #这里是pip项目发布的名称
-    version = "0.0.6",  #版本号，数值大的会优先被pip
-    keywords = ["pip", "AISimuToolKit"],			# 关键字
-    description = "ICIP's private utils.",	# 描述
-    long_description = "ICIP's private utils. The development version will be released when it is sufficiently refined",
-    license = "MIT Licence",		# 许可证
-    url = "http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",     #项目相关文件地址，一般是github项目地址即可
-    author = "Ren & Guo",			# 作者
-    author_email = "renmengjie22@mails.ucas.ac.cn",
-    packages = find_packages(),
-    include_package_data = True,
-    platforms = "any",
+    name="AISimuToolKit",  # 这里是pip项目发布的名称
+    version="0.0.7",  # 版本号，数值大的会优先被pip
+    keywords=["pip", "AISimuToolKit"],  # 关键字
+    description="ICIP's private utils.",  # 描述
+    long_description="ICIP's private utils. The development version will be released when it is sufficiently refined",
+    license="MIT Licence",  # 许可证
+    url="http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",  # 项目相关文件地址，一般是github项目地址即可
+    author="Ren & Guo",  # 作者
+    author_email="renmengjie22@mails.ucas.ac.cn",
+    packages=find_packages(),
+    include_package_data=True,
+    platforms="any",
     python_requires='>=3.10',
-    install_requires = ["openai==0.27.4", "Requests==2.28.2", "pyyaml==6.0"]   #这个项目依赖的第三方库
+    install_requires=["openai==0.27.4", "pandas==1.5.3", "PyYAML==6.0", "Requests==2.28.2", "scikit_learn==1.2.2",
+                      "setuptools==65.6.3", "torch==1.13.1", "transformers==4.24.0", ]
+    # 这个项目依赖的第三方库
 )
```

