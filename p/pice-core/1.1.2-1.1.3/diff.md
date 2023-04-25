# Comparing `tmp/pice_core-1.1.2-py3-none-any.whl.zip` & `tmp/pice_core-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,51 +1,38 @@
-Zip file size: 44910 bytes, number of entries: 49
--rw-rw-rw-  2.0 fat      727 b- defN 23-Jan-06 06:48 pice_core/INSTALL.md
--rw-rw-rw-  2.0 fat     5200 b- defN 23-Mar-23 03:29 pice_core/QUICKSTART.md
--rw-rw-rw-  2.0 fat     7034 b- defN 23-Feb-13 08:55 pice_core/Readme.md
+Zip file size: 35764 bytes, number of entries: 36
 -rw-rw-rw-  2.0 fat      358 b- defN 23-Apr-07 08:07 pice_core/__init__.py
 -rw-rw-rw-  2.0 fat     1154 b- defN 23-Apr-04 06:16 pice_core/global_variables_for_test_report.py
 -rw-rw-rw-  2.0 fat     1370 b- defN 23-Mar-23 07:09 pice_core/log_handler.py
--rw-rw-rw-  2.0 fat      481 b- defN 23-Mar-31 02:06 pice_core/read_test_info.py
--rw-rw-rw-  2.0 fat      251 b- defN 23-Mar-22 05:31 pice_core/requirements.txt
--rw-rw-rw-  2.0 fat      364 b- defN 23-Apr-02 10:58 pice_core/can_related/__init__.py
--rw-rw-rw-  2.0 fat     6635 b- defN 23-Apr-04 02:18 pice_core/can_related/can_control.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Apr-24 07:23 pice_core/read_test_info.py
+-rw-rw-rw-  2.0 fat      430 b- defN 23-Apr-25 03:28 pice_core/can_related/__init__.py
+-rw-rw-rw-  2.0 fat     6602 b- defN 23-Apr-25 03:26 pice_core/can_related/can_control.py
 -rw-rw-rw-  2.0 fat     6695 b- defN 23-Mar-23 06:38 pice_core/can_related/canoe_connect.py
 -rw-rw-rw-  2.0 fat     6702 b- defN 23-Apr-04 06:16 pice_core/can_related/kvaser_connect.py
 -rw-rw-rw-  2.0 fat    12751 b- defN 23-Apr-13 03:05 pice_core/can_related/parse_canoe_tools.py
 -rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/cb_related/__init__.py
--rw-rw-rw-  2.0 fat     7517 b- defN 23-Apr-14 08:27 pice_core/cb_related/codebeamer_connect.py
+-rw-rw-rw-  2.0 fat     8600 b- defN 23-Apr-25 05:28 pice_core/cb_related/codebeamer_connect.py
 -rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/config/__init__.py
 -rw-rw-rw-  2.0 fat      957 b- defN 23-Mar-22 08:00 pice_core/config/report.css
 -rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/dataset_handler/__init__.py
 -rw-rw-rw-  2.0 fat     5922 b- defN 23-Apr-02 02:34 pice_core/dataset_handler/data_set.py
--rw-rw-rw-  2.0 fat     2555 b- defN 23-Apr-19 05:39 pice_core/instrument_control/__init__.py
+-rw-rw-rw-  2.0 fat     3345 b- defN 23-Apr-25 03:26 pice_core/instrument_control/__init__.py
 -rw-rw-rw-  2.0 fat     3654 b- defN 23-Apr-17 03:27 pice_core/instrument_control/battery_chroma_control.py
 -rw-rw-rw-  2.0 fat     2593 b- defN 23-Apr-17 03:33 pice_core/instrument_control/battery_gmc_control.py
 -rw-rw-rw-  2.0 fat     3508 b- defN 23-Apr-17 03:33 pice_core/instrument_control/battery_itech_control.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-17 03:33 pice_core/instrument_control/battery_korad_control.py
 -rw-rw-rw-  2.0 fat     2614 b- defN 23-Apr-17 03:33 pice_core/instrument_control/battery_ngi.py
 -rw-rw-rw-  2.0 fat     5166 b- defN 23-Apr-19 01:39 pice_core/instrument_control/bin_set_module_control.py
 -rw-rw-rw-  2.0 fat     2556 b- defN 23-Apr-02 02:26 pice_core/instrument_control/read_curr_vol_module_control.py
 -rw-rw-rw-  2.0 fat     2609 b- defN 23-Mar-23 06:20 pice_core/instrument_control/serial_control.py
 -rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/parse_config_file/__init__.py
 -rw-rw-rw-  2.0 fat      972 b- defN 23-Mar-23 07:24 pice_core/parse_config_file/parse_config.py
 -rw-rw-rw-  2.0 fat      860 b- defN 23-Mar-23 06:38 pice_core/parse_config_file/parse_yaml_case.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Apr-17 09:39 pice_core/utils/__init__.py
--rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/utils/code_gen/__init__.py
--rw-rw-rw-  2.0 fat      116 b- defN 22-Dec-14 10:00 pice_core/utils/code_gen/demo_msg_sig_env_def.py
--rw-rw-rw-  2.0 fat     1022 b- defN 23-Mar-23 06:24 pice_core/utils/code_gen/gen_cdd_name_def.py
--rw-rw-rw-  2.0 fat     1007 b- defN 23-Mar-23 06:24 pice_core/utils/code_gen/gen_dbc_name_def.py
--rw-rw-rw-  2.0 fat      944 b- defN 23-Mar-23 06:24 pice_core/utils/code_gen/gen_ni_map_def.py
--rw-rw-rw-  2.0 fat     1007 b- defN 23-Mar-23 06:24 pice_core/utils/code_gen/gen_pdx_name_def.py
--rw-rw-rw-  2.0 fat     1008 b- defN 23-Mar-23 06:24 pice_core/utils/code_gen/gen_sys_name_def.py
--rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/utils/testcase_gen/__init__.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Mar-23 03:29 pice_core/utils/testcase_gen/gen_testcase_from_codebeamer.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 23-Apr-25 02:16 pice_core/utils/__init__.py
 -rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-23 03:18 pice_core/veristand_related/__init__.py
 -rw-rw-rw-  2.0 fat     1939 b- defN 23-Apr-13 06:23 pice_core/veristand_related/gen_mapping.py
 -rw-rw-rw-  2.0 fat      124 b- defN 23-Feb-28 09:18 pice_core/veristand_related/ni_connect.py
--rw-rw-rw-  2.0 fat     7650 b- defN 23-Apr-19 05:43 pice_core-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:43 pice_core-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      286 b- defN 23-Apr-19 05:43 pice_core-1.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-19 05:43 pice_core-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4610 b- defN 23-Apr-19 05:43 pice_core-1.1.2.dist-info/RECORD
-49 files, 116610 bytes uncompressed, 37350 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat    11008 b- defN 23-Apr-25 06:40 pice_core-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 06:40 pice_core-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      286 b- defN 23-Apr-25 06:40 pice_core-1.1.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-25 06:40 pice_core-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3390 b- defN 23-Apr-25 06:40 pice_core-1.1.3.dist-info/RECORD
+36 files, 100910 bytes uncompressed, 30172 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -1,31 +1,19 @@
-Filename: pice_core/INSTALL.md
-Comment: 
-
-Filename: pice_core/QUICKSTART.md
-Comment: 
-
-Filename: pice_core/Readme.md
-Comment: 
-
 Filename: pice_core/__init__.py
 Comment: 
 
 Filename: pice_core/global_variables_for_test_report.py
 Comment: 
 
 Filename: pice_core/log_handler.py
 Comment: 
 
 Filename: pice_core/read_test_info.py
 Comment: 
 
-Filename: pice_core/requirements.txt
-Comment: 
-
 Filename: pice_core/can_related/__init__.py
 Comment: 
 
 Filename: pice_core/can_related/can_control.py
 Comment: 
 
 Filename: pice_core/can_related/canoe_connect.py
@@ -90,59 +78,32 @@
 
 Filename: pice_core/parse_config_file/parse_yaml_case.py
 Comment: 
 
 Filename: pice_core/utils/__init__.py
 Comment: 
 
-Filename: pice_core/utils/code_gen/__init__.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/demo_msg_sig_env_def.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/gen_cdd_name_def.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/gen_dbc_name_def.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/gen_ni_map_def.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/gen_pdx_name_def.py
-Comment: 
-
-Filename: pice_core/utils/code_gen/gen_sys_name_def.py
-Comment: 
-
-Filename: pice_core/utils/testcase_gen/__init__.py
-Comment: 
-
-Filename: pice_core/utils/testcase_gen/gen_testcase_from_codebeamer.py
-Comment: 
-
 Filename: pice_core/veristand_related/__init__.py
 Comment: 
 
 Filename: pice_core/veristand_related/gen_mapping.py
 Comment: 
 
 Filename: pice_core/veristand_related/ni_connect.py
 Comment: 
 
-Filename: pice_core-1.1.2.dist-info/METADATA
+Filename: pice_core-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pice_core-1.1.2.dist-info/WHEEL
+Filename: pice_core-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pice_core-1.1.2.dist-info/entry_points.txt
+Filename: pice_core-1.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pice_core-1.1.2.dist-info/top_level.txt
+Filename: pice_core-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pice_core-1.1.2.dist-info/RECORD
+Filename: pice_core-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pice_core/read_test_info.py

```diff
@@ -2,20 +2,20 @@
 
 path = 'test_information.txt'
 
 file = open(path, "r", encoding='utf-8')
 data = str(file.readlines())
 file.close()
 data = data.replace(r"\n", "").replace(r"]", "")
-
-
 # name = 'tester'
 
+
 def get_test_info(key: str):
     if key in data:
         tester = re.findall(r"'{} = .*".format(key), data)[0]
         d = tester.split(r",")
         d = str(d[0]).split("=")
 
         return str(d[1]).replace("'", "").replace(" ", "")
+    else:
+        raise Exception("{} is not in {}", key, data)
 
-# print(get_test_info(name))
```

## pice_core/can_related/__init__.py

```diff
@@ -1,9 +1,10 @@
 from ..parse_config_file import parse_config
 from .can_control import Msg
+from ..instrument_control import default_config
 
 
-def connect_can_control_by_vector_hardware(config: parse_config.ConfigHandler, can_fd=True):
+def connect_can_control_by_vector_hardware(config: parse_config.ConfigHandler = default_config, can_fd=True):
     serial = config.get_config_by_name('vector_hardware')['serial_number']
     channel = config.get_config_by_name('vector_hardware')['channel']
 
     return Msg(serial, channel, can_fd)
```

## pice_core/can_related/can_control.py

```diff
@@ -4,16 +4,16 @@
 @Author: Siwei.Lu
 @Date: 2022.11.26
 """
 
 import can
 import math
 import sys
+import time
 
-from ..parse_config_file import parse_config
 from .. import logger
 
 
 FC = [0x30]
 
 
 class Msg:
```

## pice_core/cb_related/codebeamer_connect.py

```diff
@@ -1,20 +1,21 @@
 """
 This file is used to get information from CodeBeamer.
 
 Please make sure you have REST API access permission of the related project.
 
 @author: siwei.lu
-@date: 2023.3.2
+@date: 2023.4.24
 """
 
 import json
+import math
 import re
 import time
-import os
+
 import requests
 import yaml
 
 from multiprocessing import Process
 
 from ..parse_config_file import parse_config
 
@@ -22,34 +23,34 @@
 
 base_yaml_path = '/test_fixture/test_configuration/config.yaml'
 
 
 class CodeBeamerHandler:
     def __init__(self, project_name, user_name, user_password):
         self.__project_name = project_name
-        self.__project_config_path = "{}". format(project_name) + base_yaml_path
+        self.__project_config_path = "{}".format(project_name) + base_yaml_path
         self.__config = parse_config.ConfigHandler(self.__project_config_path)
 
         self.__project_num = self.__config.get_config_by_name('codebeamer')['project_num']
+
         self.__hostname = "172.16.200.236:8080"
         self._url_response_time = 0.5
         self.__items_url = "http://{host_name}/cb/rest/category/{project}/items".format(host_name=self.__hostname,
                                                                                         project=self.__project_num)
         self.__name = user_name
         self.__password = user_password
 
         self.__test_case_info_dict = {}
         self.__case_step_name = []
         self.__parents = []
 
-        self.__project_items = self.get_json_data_from_url(self.__items_url)  # 获取所有case items
+        self.__project_items = self.get_json_data_from_url(
+            '{url}/page/{page}'.format(url=self.__items_url, page=1))  # 获取所有case items
         self.__test_case_items = self.__project_items["items"]
-        self.__ids = [item['id'] for item in self.__test_case_items]
-
-        # print(len(self.__ids))
+        self._get_all_test_case_ids()
 
         self.json_data = []
         # self.multi_process()
         self.get_test_cases_info()
 
     def get_json_data_from_url(self, url, file_name=None):
         data = requests.get(url=url, auth=(self.__name, self.__password))
@@ -58,14 +59,27 @@
 
         if file_name:
             with open(file_name, "w", encoding='utf-8') as file:
                 json.dump(format_json_data, file, indent=4, ensure_ascii=False)
 
         return json_data
 
+    def _get_all_test_case_ids(self):
+        total_items = self.__project_items["total"]
+        page_size = self.__project_items["size"]
+        print("total_items = {}, page_size = {}".format(total_items, page_size))
+
+        for page in range(2, math.ceil(total_items / page_size) + 1):
+            project_items = self.get_json_data_from_url('{url}/page/{page}'.format(url=self.__items_url, page=page))
+            case_items = project_items["items"]
+            self.__test_case_items.extend(case_items)
+            time.sleep(self._url_response_time)
+
+        self.__ids = [item['id'] for item in self.__test_case_items]
+
     def multi_process(self):
         process = []
         for test_case_id in self.__ids:
             process.append(Process(target=self.get_test_case_according_item_id, args=(test_case_id,)))
         [p.start() for p in process]
         [p.join() for p in process]
 
@@ -153,15 +167,16 @@
         with open("tc_xxx.yaml", "w", encoding='utf-8') as file:
             yaml.dump(self.__test_case_info_dict, file, encoding='utf-8', allow_unicode=True, indent=4)
 
     def write_case_to_py(self):
         generate_path = r'{}/test_profile/test_case/'.format(self.__project_name)
 
         for key, values in self.__test_case_info_dict.items():
-            py_file_name = key.replace(" ", "_").replace("-", "_")
+            py_file_name = self._replace_abnormal_char(key)
+
             with open(generate_path + "tc_{}.py".format(py_file_name), "w", encoding='utf-8') as file_py:
                 file_py.write("# {}\n".format(key))
                 for value in values:
                     file_py.write("def test_{}():\n".format(value["case_id"]))
                     file_py.write("    print(\"{}\")\n".format(value["description"]))
                     file_py.write("    # todo:{}: {}\n".format("preAction", value["preAction"]))
 
@@ -169,13 +184,23 @@
                         file_py.write("    # todo:step_{}: {}\n".format(i + 1, value["testSteps"][i]))
 
                     for i in range(len(value["expect_result"])):
                         file_py.write("    # todo:expect_result_{}: {}\n".format(i + 1, value["expect_result"][i]))
 
                     file_py.write('    pass\r\n\n')
 
+    @staticmethod
+    def _replace_abnormal_char(input_char: str):
+        abnormal_char_list_to_null = [" "]
+        abnormal_char_list_to_dash = ["*", "-", "=", "<", ">",
+                                      "[", "]", "+", "/", "&",
+                                      "%", "(", ")", ",", ".",
+                                      ":", "。", ";", "\\", "~",
+                                      "∈"]
+
+        for character in abnormal_char_list_to_null:
+            input_char = input_char.replace(character, "")
+
+        for character in abnormal_char_list_to_dash:
+            input_char = input_char.replace(character, "_")
 
-# def read_yaml():
-#     with open("tc_xxx_1.yaml", "r", encoding='utf-8') as file:
-#         data = yaml.load(file, Loader=yaml.FullLoader)
-#         for item in data["功能优先级测试"]:
-#             print(item)
+        return input_char
```

## pice_core/instrument_control/__init__.py

```diff
@@ -1,63 +1,76 @@
 from ..parse_config_file import parse_config
+from ..global_variables_for_test_report import g_project
 from . import battery_ngi, battery_itech_control, battery_gmc_control, battery_korad_control, battery_chroma_control, \
     read_curr_vol_module_control, bin_set_module_control
+import os
 
+yaml_path_use_run = os.path.abspath('.') + r"/Project/{}/test_fixture/test_configuration/config.yaml".format(g_project)
+yaml_path_use_pre = os.path.dirname(os.path.dirname(os.path.abspath('.'))) + r"/test_fixture/test_configuration" \
+                                                                             r"/config.yaml"
 
-def set_battery_ngi_by_serial(config: parse_config.ConfigHandler):
+if os.path.exists(yaml_path_use_run):
+    default_config = parse_config.ConfigHandler(yaml_path_use_run)
+elif os.path.exists(yaml_path_use_pre):
+    default_config = parse_config.ConfigHandler(yaml_path_use_pre)
+else:
+    default_config = None
+
+
+def set_battery_ngi_by_serial(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_NGI')
     baud = config.get_baud_rate('power_supply_NGI')
     com = config.get_com('power_supply_NGI')
 
     return battery_ngi.BatControlNGIBySerial(baud, com, vbat_config)
 
 
-def set_battery_itech_by_visa(config: parse_config.ConfigHandler):
+def set_battery_itech_by_visa(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_IT6512')
     resource = vbat_config['visa_resource']
 
     return battery_itech_control.BatIT6512ControlByVisa(resource, vbat_config)
 
 
-def set_battery_gmc_by_serial(config: parse_config.ConfigHandler):
+def set_battery_gmc_by_serial(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_gmc')
     baud = config.get_baud_rate('power_supply_gmc')
     com = config.get_com('power_supply_gmc')
 
     return battery_gmc_control.BatGMCControlBySerial(baud, com, vbat_config)
 
 
-def set_battery_korad_by_serial(config: parse_config.ConfigHandler):
+def set_battery_korad_by_serial(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_korad')
     baud = config.get_baud_rate('power_supply_korad')
     com = config.get_com('power_supply_korad')
 
     return battery_korad_control.BatKoradControlBySerial(baud, com, vbat_config)
 
 
-def set_battery_chroma_by_visa(config: parse_config.ConfigHandler):
+def set_battery_chroma_by_visa(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_chroma')
     resource = vbat_config['visa_resource']
 
     return battery_chroma_control.BatChromaControlByVisa(resource, vbat_config)
 
 
-def set_battery_chroma_by_serial(config: parse_config.ConfigHandler):
+def set_battery_chroma_by_serial(config: parse_config.ConfigHandler = default_config):
     vbat_config = config.get_config_by_inst('power_supply_chroma')
     baud = config.get_baud_rate('power_supply_chroma')
     com = config.get_com('power_supply_chroma')
 
     return battery_chroma_control.BatChromaControlBySerial(baud, com, vbat_config)
 
 
-def set_curr_vol_module(config: parse_config.ConfigHandler):
+def set_curr_vol_module(config: parse_config.ConfigHandler = default_config):
     baud = config.get_baud_rate('read_current_voltage_module')
     com = config.get_com('read_current_voltage_module')
 
     return read_curr_vol_module_control.ReadCurrVolModuleControl(baud=baud, com=com)
 
 
-def set_bin_module(config: parse_config.ConfigHandler):
+def set_bin_module(config: parse_config.ConfigHandler = default_config):
     baud = config.get_baud_rate('bin_set_module')
     com = config.get_com('bin_set_module')
 
     return bin_set_module_control.BinSetModuleControl(baud=baud, com=com)
```

## pice_core/utils/__init__.py

```diff
@@ -1,11 +1,9 @@
 import os
 
-# os.path.abspath('.')
-
 from ..can_related import parse_canoe_tools
 from ..veristand_related import gen_mapping
 from ..cb_related.codebeamer_connect import CodeBeamerHandler
 
 work_path = os.path.abspath('.')
 
 
@@ -57,15 +55,15 @@
     try:
         print("work_path = ", work_path)
         print("Enter codebeamer Account name:")
         name = input()
         print("Enter codebeamer Password:")
         password = input()
 
-        print("Start create test case file...")
+        print("\nStart create test case file...")
 
         cb = CodeBeamerHandler(work_path, name, password)
         cb.write_case_to_py()
 
         print("\ntest case write successfully! \n")
 
     except BaseException as err:
```

## Comparing `pice_core-1.1.2.dist-info/RECORD` & `pice_core-1.1.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,36 @@
-pice_core/INSTALL.md,sha256=sTB0uNwEjTKNmh0HVdVB0ufXJjc5ZdTehczONiy0ScI,727
-pice_core/QUICKSTART.md,sha256=Zt6ZbgxwGC-m_S1w7HhK64dZMaGJLpvSmpl384nXA9A,5200
-pice_core/Readme.md,sha256=93bC75_YsbpecdRR7cQhPtqwXBE9Hhq1aUtOxJdXsQM,7034
 pice_core/__init__.py,sha256=5Yp2pNTiYFbzkgehFkkxtJR978XYB0Wt6U-LrhIWB4s,358
 pice_core/global_variables_for_test_report.py,sha256=1ZGHly3pFJdr2UPe92ImAv1XZTZaD9mpN0CwnFLUpaM,1154
 pice_core/log_handler.py,sha256=ao5ECD9aWmsqTezhfXqYcCwOSqva9jWPu-hg2_tAGU8,1370
-pice_core/read_test_info.py,sha256=kI3SCWxH8rz74OU0HGamTPaFjfD9ND8iZWvlWlaZeIM,481
-pice_core/requirements.txt,sha256=QQ7lMmW_Eh2cDoQOxa11kdxGS9FH74yxwNvbpFJJgMM,251
-pice_core/can_related/__init__.py,sha256=GQuEIexSoTCE8mMRF3cII1SIZ4jDo0SLZoiG_EMRdb8,364
-pice_core/can_related/can_control.py,sha256=oFNMOhzeM6tBoArsYQCuVr9yQrctIkldCvqcVK5aEw4,6635
+pice_core/read_test_info.py,sha256=119_tcT0LXjFusxQj6GGcpsK4IGjsoljV5Ik855hNEs,515
+pice_core/can_related/__init__.py,sha256=e5uD541-jtww1XBGtFOosP509PM1nMAlQNU29cOYGNA,430
+pice_core/can_related/can_control.py,sha256=BHEcel6bklxB0i_sH6-3qjKrQyYkaHtAEsbXjO0pZt4,6602
 pice_core/can_related/canoe_connect.py,sha256=FGhHGLZwSHdYJGjuegvcw0xQgstiqU9LMb_bjZQ4GmI,6695
 pice_core/can_related/kvaser_connect.py,sha256=IWMKeYLUdrF5tXIwS4T566ZOohwoXKpULU9SpKpQQBU,6702
 pice_core/can_related/parse_canoe_tools.py,sha256=x8kFbhYb6hP6KPdtHVhRTZylvZCIoR3tkeGc6_bAeFg,12751
 pice_core/cb_related/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
-pice_core/cb_related/codebeamer_connect.py,sha256=0BJxoCqDs-dOoaBKDqIfyeOnZVTKNGNcHL9auyB1fKk,7517
+pice_core/cb_related/codebeamer_connect.py,sha256=4CygRoziVoAQSOZbqoGglx7ioz-EgT0xpo5js_n56Ug,8600
 pice_core/config/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
 pice_core/config/report.css,sha256=8SjYzqzixA4wWzO-fEshVxwRn-KsPgLOWA5etDC0Dj4,957
 pice_core/dataset_handler/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
 pice_core/dataset_handler/data_set.py,sha256=DcBVGSa4qtZ1JPTDZNRldj89nj9ZHZDspVvrqW3pmOE,5922
-pice_core/instrument_control/__init__.py,sha256=fgknDPM8mfnDQOPwdO1OQX5waog7y7KgsntiKTrXM_g,2555
+pice_core/instrument_control/__init__.py,sha256=-N4EuZq47RLWhiTfwoZiquTC0l4e_rlc0U31myYLru8,3345
 pice_core/instrument_control/battery_chroma_control.py,sha256=6nn1jJyI-X6D-su-UOrk3mCQN-u39xAu-g2M2UoRxaE,3654
 pice_core/instrument_control/battery_gmc_control.py,sha256=CeHGsc5_FvH9XkOYGczP7QJtZby6ME3-28WgRGvs9SA,2593
 pice_core/instrument_control/battery_itech_control.py,sha256=MwPJg8daQ7W6zyMCsvkT64U6hs2k9h6egRlpwbaJ3y0,3508
 pice_core/instrument_control/battery_korad_control.py,sha256=nPO0Hu4IVEVN8jxtgQqFsDiuVcmEMSB5r8J2mZYcMys,2231
 pice_core/instrument_control/battery_ngi.py,sha256=Nt41T5-SwgNCph_c4WnRa8yPOaGRxKEWNC9Fnnjjrm8,2614
 pice_core/instrument_control/bin_set_module_control.py,sha256=B_td3l9lwokqef70Yvi8gi4ZcA1K1kkOYsBS73QtQTs,5166
 pice_core/instrument_control/read_curr_vol_module_control.py,sha256=gkhxo5Hf4DD4ukrDIJvm9Z0w3l5YUhlqFEobUq-j3H4,2556
 pice_core/instrument_control/serial_control.py,sha256=3IeYJI3xZaBtLf3NAoijaLs_Rrzi-0RuCiO3IO6S7WA,2609
 pice_core/parse_config_file/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
 pice_core/parse_config_file/parse_config.py,sha256=rjxjeSLazvrYp66AYGjpN8WhfqvzGExPz1QPlN2Eofw,972
 pice_core/parse_config_file/parse_yaml_case.py,sha256=PA0mmjGCvMQWOB505l-AC7bHivk9gRkTHlMwPQNzDyM,860
-pice_core/utils/__init__.py,sha256=erNz4A0WgkfYZ10Bb_Nx8jLFw2x8LKYPFnNoeCzcR2g,1901
-pice_core/utils/code_gen/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
-pice_core/utils/code_gen/demo_msg_sig_env_def.py,sha256=XajfY1vG1UQxJ6EWq9KI9IWxw-Y4kPU2tGQjBJcj6_4,116
-pice_core/utils/code_gen/gen_cdd_name_def.py,sha256=VHHTrGGg7tueyCl_3LEq8hUGEgeA0QN9Znzr52czQZo,1022
-pice_core/utils/code_gen/gen_dbc_name_def.py,sha256=H94Gt9ldYZFpd_pqqbnSqzjq81avf_NBSAVADoxb5rM,1007
-pice_core/utils/code_gen/gen_ni_map_def.py,sha256=ib9snFroUWujnz0bw9KJYJgpCTXxDcKrndzsjOsrKmo,944
-pice_core/utils/code_gen/gen_pdx_name_def.py,sha256=O2uMJa_zOpYklUU0a6sM_bfPCuSyrQqtYPI114ScJnY,1007
-pice_core/utils/code_gen/gen_sys_name_def.py,sha256=zREuadpJ7QEd-j6x0jx8zqOnUQwpx4Xpr49M4v6sZWs,1008
-pice_core/utils/testcase_gen/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
-pice_core/utils/testcase_gen/gen_testcase_from_codebeamer.py,sha256=GS_htVg2Lxz38JYofdkku09EkooFfgj9yZnvWUtCBek,1430
+pice_core/utils/__init__.py,sha256=TvwQgWKGUEgKhMUWmh5IsuCp3CkWtQ7AXeiZfMN_c4c,1877
 pice_core/veristand_related/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
 pice_core/veristand_related/gen_mapping.py,sha256=G0PkvobiQ_7f_97l-hy2G01q2pZl2VIncMC3JFKegkU,1939
 pice_core/veristand_related/ni_connect.py,sha256=M2e-BltXBNXWkp1jY3dLzR6e58bI7REwm02QPtLc4J8,124
-pice_core-1.1.2.dist-info/METADATA,sha256=OZzHq9v5Dy5iIUtm3Xhbhr4_UxqEKYAYZDumSEkj8vM,7650
-pice_core-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pice_core-1.1.2.dist-info/entry_points.txt,sha256=4XxfvRyfgHxp7gyz2JZKsrn2ZYGYdXWzRFhi9TGMyBU,286
-pice_core-1.1.2.dist-info/top_level.txt,sha256=n-PbqsIksMjUV2lQKdkUNtq2HXYkHeLAIkoezbPPTzg,10
-pice_core-1.1.2.dist-info/RECORD,,
+pice_core-1.1.3.dist-info/METADATA,sha256=XIRQlo6ZvoOmcA3FJEbnaa3A-EbI4VUWiZi-vGLGC3Y,11008
+pice_core-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pice_core-1.1.3.dist-info/entry_points.txt,sha256=4XxfvRyfgHxp7gyz2JZKsrn2ZYGYdXWzRFhi9TGMyBU,286
+pice_core-1.1.3.dist-info/top_level.txt,sha256=n-PbqsIksMjUV2lQKdkUNtq2HXYkHeLAIkoezbPPTzg,10
+pice_core-1.1.3.dist-info/RECORD,,
```

