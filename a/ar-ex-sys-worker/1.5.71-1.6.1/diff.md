# Comparing `tmp/ar_ex_sys_worker-1.5.71-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15896 bytes, number of entries: 11
+Zip file size: 16092 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    26635 b- defN 23-Apr-13 06:51 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19415 b- defN 23-Apr-13 07:06 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    27080 b- defN 23-Apr-25 11:01 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19883 b- defN 23-Apr-25 07:19 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
--rw-rw-rw-  2.0 fat    10331 b- defN 23-Apr-13 07:02 ar_external_sys_worker/tests/main_test.py
+-rw-rw-rw-  2.0 fat    10365 b- defN 23-Apr-25 10:52 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1127 b- defN 22-Sep-14 11:20 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/RECORD
-11 files, 60052 bytes uncompressed, 14180 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-25 11:02 ar_ex_sys_worker-1.6.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      343 b- defN 23-Apr-25 11:02 ar_ex_sys_worker-1.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 11:02 ar_ex_sys_worker-1.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-25 11:02 ar_ex_sys_worker-1.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 23-Apr-25 11:02 ar_ex_sys_worker-1.6.1.dist-info/RECORD
+11 files, 60993 bytes uncompressed, 14386 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.71.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.71.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.71.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.71.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.71.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -118,14 +118,20 @@
                   "WHERE p.photo_type={} and rp.record_id={} LIMIT 1".format(
             photo_type,
             record_id)
         response = self.sql_shell.try_execute_get(command)
         if response:
             return response[0][0]
 
+    @wsqluse.wsqluse.getTableDictStripper
+    def get_photo_types(self, sql_shell):
+        return sql_shell.get_table_dict(
+            "SELECT id, name FROM photo_types"
+        )
+
     def get_send_data(self):
         return self.get_one_unsend_act()
 
 
 class ASUActsWorker(mixins.AsuMixin, ActsWorker,
                     mixins.SignallPhotoEncoderMixin):
     def __init__(self, sql_shell, trash_cats_list, time_start, acts_limit=3,
@@ -341,25 +347,23 @@
         self.get_carriers_po_link = self.get_full_endpoint(
             self.link_get_po_links)
         self.act_id_from_response = 'act_id'
         self.mutex = allocate_lock()
 
     def format_file_before_logging(self, data):
         data = json.loads(data)
-        data.pop('photo_in')
-        data.pop('photo_out')
+        data.pop('photos')
         return str(data).replace("'", '"')
 
     def format_alerts(self, alerts):
         if not alerts:
             return []
         res = alerts.split('&&')
         return res[:-1]
 
-
     def format_send_data_old(self, act, photo_in=None, photo_out=None):
         act.pop('polygon_id')
         act.pop('rfid')
         alerts_string = act.pop('alerts')
         # alerts = self.get_alerts(act['ex_id'])
         act['platform_type'] = act.pop('pol_object')
         act_number = act.pop('act_number')
@@ -398,42 +402,49 @@
                                  containers_plan=act['containers_plan'],
                                  containers_fact=act['containers_fact'],
                                  route_num=act["route_num"],
                                  platform_type=act["platform_type"],
                                  act_number=act_number)
         return act_json
 
+    def get_photos(self, record_id):
+        photo_types = self.get_photo_types(self.sql_shell)
+        new_dict = {}
+        for photo_type in photo_types:
+            photo_path = self.get_photo_path(record_id, photo_type["id"])
+            if photo_path:
+                photo_obj = self.get_photo_data(photo_path)
+                new_dict[photo_type['name']] = photo_obj
+        return new_dict
+
+
     def format_send_data(self, act, photo_in=None, photo_out=None):
-        photo_in = self.get_photo_path(act['ex_id'], 1)
-        photo_out = self.get_photo_path(act['ex_id'], 2)
-        if photo_in:
-            photo_in = self.get_photo_data(photo_in)
-        if photo_out:
-            photo_out = self.get_photo_data(photo_out)
         data = {
             "car_number": act['car_number'],
             "ex_id": act['ex_id'],
             "gross": act['gross'],
             "tare": act['tare'],
             "cargo": act['cargo'],
             "time_in": act['time_in'].strftime(
                                      '%Y-%m-%d %H:%M:%S'),
             "time_out": act['time_out'].strftime(
                                      '%Y-%m-%d %H:%M:%S'),
             "alerts": self.format_alerts(act['alerts']),
-            "carrier": act['carrier'],
+            "carrier": {"inn": act['carrier_inn'],
+                        "kpp": act['carrier_kpp']},
+            "client": {"inn": act['client_inn'],
+                        "kpp": act['client_kpp']},
             "trash_cat": act['trash_cat'],
             "trash_type": act['trash_type'],
             "operator_comments": {'gross_comm': act['gross_comm'],
                                     'tare_comm': act['tare_comm'],
                                     'add_comm': act['add_comm'],
                                     'changing_comm': act['changing_comm'],
                                     'closing_comm': act['closing_comm']},
-            "photo_in": photo_in,
-            'photo_out': photo_out,
+            "photos": self.get_photos(act['ex_id']),
             "containers_plan": act['containers_plan'],
             'containers_fact': act['containers_fact'],
             "route_num": act["route_num"],
             'platform_type': act['pol_object'],
             "act_number": {'number': act['act_number'],
                            'package': act['package_name']},
         }
```

## ar_external_sys_worker/mixins.py

```diff
@@ -31,23 +31,26 @@
 
 class SignallMixin:
     link_host = "https://signall.qodex.tech"
     #link_host = "https://signalltestdev.qodex.tech"
     link_auth = '/v1/user/login'
     link_get_po_links = "/v1/gravity/get_po_clients"
     port = None
-    link_create_act = '/v1/acts/create_act'
+    link_create_act = '/v1/acts/create_act_with_inn_and_kpp'
     ex_sys_id = 1
     auth_key_in_headers = 'Authorization'
     response_token_key = 'token'
     login_key_to_ex_sys = 'email'
     pass_key_to_ex_sys = 'password'
     login_column_name = 'signall_login'
     pass_column_name = 'signall_pass'
 
+    def set_signall_test(self):
+        self.link_host = "https://signalltestdev.qodex.tech"
+
 
 class TokenAuth():
     link_get_token = '/v1/gravity/get_gravity_token'
     gravity_ip = None
     gravity_port = None
     inn = None
     kpp = None
@@ -381,29 +384,33 @@
 
     def set_limit(self, limit: int):
         self.limit = limit
 
     def get_acts_all_command(self):
         command = "SELECT distinct on (r.id) r.id as ex_id, a.car_number, r.brutto as gross, " \
                   "r.tara as tare, r.cargo, r.time_in, r.time_out, " \
-                  "cji.inn as carrier, tc.name as trash_cat, " \
+                  "carrier_cji.inn as carrier_inn, carrier_cji.kpp as carrier_kpp," \
+                  "client_cji.inn as client_inn, client_cji.kpp as client_kpp," \
+                  "tc.name as trash_cat, " \
                   "tt.name as trash_type, oc.gross as gross_comm," \
                   "oc.tare as tare_comm, oc.additional as add_comm, " \
                   "oc.changing as changing_comm, oc.closing as closing_comm," \
                   "dro.owner as polygon_id, ai.number as rfid, rri.route_num," \
                   "rri.containers_plan, rri.containers_fact, ra.alerts," \
                   "pol_objects.name as pol_object," \
                   "aprm.number as act_number, acts_packages.name as package_name " \
                   "FROM records r " \
-                  "INNER JOIN clients ON (r.carrier=clients.id) " \
+                  "INNER JOIN clients carriers ON (r.carrier=carriers.id) " \
+                  "INNER JOIN clients ON (r.client_id=clients.id) " \
                   "INNER JOIN trash_cats tc ON (r.trash_cat=tc.id) " \
                   "INNER JOIN trash_types tt ON (r.trash_type=tt.id) " \
                   "LEFT JOIN operator_comments oc ON (r.id=oc.record_id) " \
                   "LEFT JOIN auto a ON (a.id=r.auto) " \
-                  "LEFT JOIN clients_juridical_info cji ON (cji.client_id=clients.id) " \
+                  "LEFT JOIN clients_juridical_info carrier_cji ON (carrier_cji.client_id=carriers.id) " \
+                  "LEFT JOIN clients_juridical_info client_cji ON (carrier_cji.client_id=clients.id) " \
                   "LEFT JOIN ex_sys_data_send_reports esdsr ON (esdsr.local_id = r.id)" \
                   "LEFT JOIN duo_records_owning dro on r.id = dro.record " \
                   "LEFT JOIN auto_idents ai ON ai.id=a.identifier " \
                   "LEFT JOIN records_routes_info rri ON r.id=rri.record_id " \
                   "LEFT JOIN records_alerts ra ON ra.record_id=r.id " \
                   "LEFT JOIN records_pol_objects_mapping rpom ON rpom.record_id=r.id " \
                   "LEFT JOIN pol_objects ON rpom.object_id=pol_objects.id " \
```

## ar_external_sys_worker/tests/main_test.py

```diff
@@ -216,20 +216,21 @@
     def test_signall_worker_token(self):
         inst = main.SignAllActsWorkerToken(self.sql_shell,
                                            ['ТКО', 'Прочее', 'ПО', 'Хвосты'],
                                            '2021.05.05',
                                            1,
                                            gravity_ip='172.16.9.20',
                                            test=True)
+        inst.set_signall_test()
         #inst.link_host = 'https://signalltestdev.qodex.tech'
         inst.auth()
+        inst.send_unsend_acts()
        # print(inst.link_host)
-        #inst.send_unsend_acts()
-        res = inst.get_carriers_po().json()
-        print(f"PO_CARRIERS: {res}\nLen: {len(res['transporters'])}")
+        #res = inst.get_carriers_po().json()
+        #print(f"PO_CARRIERS: {res}\nLen: {len(res['transporters'])}")
 
     @unittest.SkipTest
     def test_send_acts(self):
         self.inst.send_unsend_acts()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `ar_ex_sys_worker-1.5.71.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

