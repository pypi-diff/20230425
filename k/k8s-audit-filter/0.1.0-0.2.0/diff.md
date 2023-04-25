# Comparing `tmp/k8s_audit_filter-0.1.0-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 17695 bytes, number of entries: 9
+Zip file size: 19455 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
--rw-r--r--  2.0 unx     1564 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
--rw-r--r--  2.0 unx     2197 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
--rw-r--r--  2.0 unx     1356 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     4848 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/RECORD
-9 files, 46065 bytes uncompressed, 16375 bytes compressed:  64.5%
+-rw-r--r--  2.0 unx     1117 b- defN 20-Feb-02 00:00 k8s_audit_filter/abstract_classes.py
+-rw-r--r--  2.0 unx     2241 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
+-rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
+-rw-r--r--  2.0 unx     2180 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
+-rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
+?rw-r--r--  2.0 unx     5880 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/RECORD
+11 files, 51225 bytes uncompressed, 17841 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: k8s_audit_filter/__about__.py
 Comment: 
 
 Filename: k8s_audit_filter/__init__.py
 Comment: 
 
+Filename: k8s_audit_filter/abstract_classes.py
+Comment: 
+
 Filename: k8s_audit_filter/audit_filter.py
 Comment: 
 
 Filename: k8s_audit_filter/fields.py
 Comment: 
 
+Filename: k8s_audit_filter/resourses_field.py
+Comment: 
+
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.1.0.dist-info/METADATA
+Filename: k8s_audit_filter-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.1.0.dist-info/WHEEL
+Filename: k8s_audit_filter-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.1.0.dist-info/RECORD
+Filename: k8s_audit_filter-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## k8s_audit_filter/audit_filter.py

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 import yaml
 
+from .abstract_classes import Rule
 from .rules import RuleFactory
 
 
 class AuditFilterException(Exception):
     pass
 
 
@@ -17,29 +18,43 @@
             if "apiVersion" not in policy or policy["apiVersion"] != "audit.k8s.io/v1":
                 raise AuditFilterException(
                     "Invalid policy, missing version or version does not match 'audit.k8s.io/v1'"
                 )
             if "kind" not in policy or policy["kind"] != "Policy":
                 raise AuditFilterException("Invalid policy, missing kind or kind does not match 'Policy'")
             self.rules = [RuleFactory.create(rule) for rule in policy["rules"]]
+            self.config: list = policy["rules"]
         elif isinstance(config, dict):
             self.rules = [RuleFactory.create(rule) for rule in config["rules"]]
+            self.config: list = config["rules"]  # type: ignore
         elif config is None:
-            self.rules = []
+            self.rules = []  # type: ignore
+            self.config: list = []  # type: ignore
         else:
-            raise TypeError("Invalid config")
+            raise AuditFilterException("Invalid config")
 
     def filter(self, log_line: dict) -> bool:
         if not self.rules:
             return True  # no rules, no filter
         for rule in self.rules:
             if rule.check_rule(log_line):
                 return True
         return False
 
     def add_rule(self, rule: dict):
-        rule = RuleFactory.create(rule)
-        self.rules.append(rule)
+        internal_rule = RuleFactory.create(rule)
+        self.rules.append(internal_rule)
+        self.config.append(internal_rule.as_dict)  # type: ignore
+
+    def add_rules(self, rules: list):
+        for rule in rules:
+            self.add_rule(rule)
 
     def remove_rule(self, rule: dict):
-        rule = RuleFactory.create(rule)
-        self.rules.remove(rule)
+        internal_rule = RuleFactory.create(rule)
+        self.rules.remove(internal_rule)
+        self.config.remove(internal_rule.as_dict)  # type: ignore
+
+    @staticmethod
+    def filter_with_rule(log_line: dict, rule: dict) -> bool:
+        internal_rule: Rule = RuleFactory.create(rule)
+        return internal_rule.check_rule(log_line)
```

## k8s_audit_filter/fields.py

```diff
@@ -1,83 +1,85 @@
 from typing import List, Union
 
+from .abstract_classes import Factory, Field, FieldException
+from .resourses_field import ResourceField
 
-class BaseField:
-    __slots__ = ("name", "value")
 
-    def __init__(self, value: Union[str, List[str], None]):
-        self.name: Union[str, None] = None
-        self.value: Union[str, List[str], None] = value
-
-    def __eq__(self, other):
-        return self.name == other.name and self.value == other.value
-
-    def check_match(self, target: dict) -> bool:
-        if target[self.name] == self.value:
-            return True
-        return False
-
-
-class LevelField(BaseField):
+class LevelField(Field):
     def __init__(self, value: Union[str, None]):
         super().__init__(value)
         self.name: Union[str, None] = "level"
         if value is None:
             raise ValueError("Invalid value for level field")
         self.value = value
 
+    def check_match(self, target: dict) -> bool:
+        if target[self.name] == self.value:
+            return True
+        return False
+
 
-class VerbsField(BaseField):
+class VerbsField(Field):
     def __init__(self, value: List[str]):
         self.name = "verb"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
         if target[self.name] in self.value:
             return True
         return False
 
 
-class UsersField(BaseField):
+class UsersField(Field):
     def __init__(self, value: List[str]):
         self.name = "user"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
         if target[self.name]["username"] in self.value:
             return True
         return False
 
 
-class UserGroupsField(BaseField):
+class UserGroupsField(Field):
     def __init__(self, value: List[str]):
-        self.name = "user"
+        self.name = "userGroups"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
-        for group in target[self.name]["groups"]:
+        for group in target["user"]["groups"]:
             if group in self.value:
                 return True
         return False
 
 
-class FieldException(Exception):
-    pass
+class NamespacesField(Field):
+    def __init__(self, value: List[str]):
+        self.name = "namespace"
+        self.value: List[str] = value
+
+    def check_match(self, target: dict) -> bool:
+        for space in self.value:
+            if target.get("objectRef") and target["objectRef"].get("namespace") == space:
+                return True
+        return False
 
 
-class FieldFactory:
-    field_mapping = {
+class FieldFactory(Factory):
+    mapping = {
         "level": LevelField,
         "verbs": VerbsField,
         "users": UsersField,
         "userGroups": UserGroupsField,
+        "namespaces": NamespacesField,
+        "resources": ResourceField,
     }
 
     @classmethod
-    def create(cls, fields: dict):
+    def create(cls, entities: dict):
         result = []
-        for key, vale in fields.items():
-            if key in cls.field_mapping:
-                result.append(cls.field_mapping[key](vale))
+        for key, vale in entities.items():
+            if key in cls.mapping:
+                result.append(cls.mapping[key](vale))
                 continue
             raise FieldException(f"Invalid field {key} for Rule")
         return result
```

## k8s_audit_filter/rules.py

```diff
@@ -1,55 +1,41 @@
-from abc import ABC
-
+from .abstract_classes import Factory, Rule, RuleException
 from .fields import FieldFactory
 
 
-class Rule(ABC):
+class RuleInitMixin:
     def __init__(self, fields: dict):
         self.as_dict = fields
         self.fields = FieldFactory.create(fields)
 
-    def __str__(self):
-        return f"{self.__class__.__qualname__}: {self.as_dict}"
-
-    def __eq__(self, other):
-        return self.fields == other.fields
 
-    def check_rule(self, instance: dict) -> bool:
-        raise NotImplementedError
-
-
-class IncludeRule(Rule):
+class IncludeRule(Rule, RuleInitMixin):
     def check_rule(self, instance: dict) -> bool:
         for field in self.fields:
             if not field.check_match(instance):
                 return False
         return True
 
 
-class ExcludeRule(Rule):
+class ExcludeRule(Rule, RuleInitMixin):
     def check_rule(self, instance: dict) -> bool:
         for field in self.fields:
             if field.check_match(instance):
                 return False
         return True
 
 
-class RuleException(Exception):
-    pass
-
-
-class RuleFactory:
-    rule_mapping = {
+class RuleFactory(Factory):
+    mapping = {
         "include": IncludeRule,
         "exclude": ExcludeRule,
     }
 
     @classmethod
-    def create(cls, rule: dict):
+    def create(cls, entity: dict) -> Rule:
         # check if rule has level field
-        if "level" not in rule:
+        if "level" not in entity:
             raise RuleException("Invalid rule, missing level")
-        if rule["level"] is None:
-            del rule["level"]
-            return cls.rule_mapping["exclude"](rule)
-        return cls.rule_mapping["include"](rule)
+        if entity["level"] is None:
+            del entity["level"]
+            return cls.mapping["exclude"](entity)
+        return cls.mapping["include"](entity)
```

## Comparing `k8s_audit_filter-0.1.0.dist-info/METADATA` & `k8s_audit_filter-0.2.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -15,15 +15,16 @@
 Description-Content-Type: text/markdown
 
 # Filter K8s Audit Logs
 
 ## Abstract
 
 This library provides a simple way to filter Kubernetes audit logs, if you, whit some reason, are not able to apply
-audit policy directly at your cloud (e. g. in yandex cloud).
+audit policy directly at your cloud (e. g. in yandex cloud) and have to filter it with python script. 
+Also you can use this library to analyze audit logs.
 The library does not provide any service, it just give you easy way to filter audit logs in your python script
 with ```AuditFilter``` class interfaces.
 
 ## Instalation
 
 ```bash
 pip install k8s-audit-filter
@@ -99,30 +100,60 @@
 
 See example of audit policy:
 
 ```yaml
 apiVersion: audit.k8s.io/v1 # This is required.
 
 kind: Policy
-# Don't generate audit events for all requests in RequestReceived stage.
-
-omitStages:
-  - "RequestReceived"
 
 rules:
   # Include line in the audit log which contains verb "get" and have level "Metadata"
   - level: Metadata
     verbs:
       - "get"
 
   # Exclude line in the audit log which contains verb "create"
   - level: None
     verbs:
       - "create"
 
+  - level: Request
+    users:
+      - "admin"
+
+  - level: Request
+    userGroups:
+      - "system:admins"
+
+```
+
+## Describing Audit Policy in Python
+
+If you want to describe audit policy in python, you can describe it in the same way as in yaml file with dict:
+
+```python
+from k8s_audit_filter import AuditFilter
+
+audit_filter = AuditFilter()
+
+rules = [
+    {'level': 'Metadata', 'verbs': ['get']},
+    {'level': 'None', 'verbs': ['create']},
+    {'level': 'Request', 'users': ['admin']},
+    {'level': 'Request', 'userGroups': ['system:admins']},
+    {'level': 'Request', 'namespaces': ['kube-system']},
+    {'level': 'RequestResponse',
+     'resources': [
+             {'group': '', 'resources': ['deployments'], 'resourceNames': ['pods']},
+             {'group': 'apps', 'resources': ['leases'], 'resourceNames': ['test']}
+         ]
+     }
+]
+audit_filter.add_rules(rules)
+
 ```
 
 ## Supported Rules
 
 Please note, that ```level``` is required field for every rule, and should have of one of next values:
 
 - ```None``` - do not log events that match this rule (this is ExcludeRule)
@@ -132,18 +163,18 @@
 
 The library supports the following rules k8s audit PolicyRules:
 
 - ```level```
 - ```verbs```
 - ```users```
 - ```userGroups```
+- ```namespaces```
+- ```resources``` - Partly supported. Please read about limitations below
 
 ## Limitations
 
-Currently, the library does not support following rules:
+The library does not support following k8s Audit rules:
 
-- ```nonResourceURLs``` - will be supported in the future
-- ```resources``` - will be supported in the future
-- ```namespaces``` - will be supported in the future
-- ```omitStages``` - now it does not distinguish any stages, and filter any string provided
-  to ```AuditFilter.filter()```
-- ```omitManagedFields```
+- ```resources``` - please note, that unlike original k8s audit policy, empty string "" in "group" field will not return "core" group, but will return all groups
+- ```nonResourceURLs``` - notResourceURLs are not declared explicitly in audit logs
+- ```omitStages``` - now it does not discern any stages
+- ```omitManagedFields``` - omitManagedFields is not declared explicitly in audit logs
```

## Comparing `k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `k8s_audit_filter-0.1.0.dist-info/RECORD` & `k8s_audit_filter-0.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-k8s_audit_filter/__about__.py,sha256=kUR5RAFc7HCeiqdlX36dZOHkUI5wI6V_43RpEcD8b-0,22
+k8s_audit_filter/__about__.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
 k8s_audit_filter/__init__.py,sha256=Ygyj50ubIBSq7rPmZA5toFWotAC4D3Mc6DzCq_07s2k,81
-k8s_audit_filter/audit_filter.py,sha256=Fmq9JLln-LpQ-deHajwYSKB-v0RCOuPgKIBiwEX1scM,1564
-k8s_audit_filter/fields.py,sha256=aZVkr1Xj2S3v90T6AlPImk3MUDaLKIRvqIS8ZMMCZXA,2197
-k8s_audit_filter/rules.py,sha256=RpURuZqj0rdEkBj70eNjAKoQxrXeqMHv4IfvlpxyI1s,1356
-k8s_audit_filter-0.1.0.dist-info/METADATA,sha256=Rcpu1bsnupznJX51Wxp9HVW5imMZJXQ7bUfyQ3R-p6o,4848
-k8s_audit_filter-0.1.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-k8s_audit_filter-0.1.0.dist-info/RECORD,,
+k8s_audit_filter/abstract_classes.py,sha256=-sZIS-NuNElW5IGcMpCeh0nUDm5KxhTdYIr1GYktewE,1117
+k8s_audit_filter/audit_filter.py,sha256=OS88j6Vqv0rHVp1FiAmlnBCdadRMI6Mj0hbNFjH1pP4,2241
+k8s_audit_filter/fields.py,sha256=9ZK-wXtuOeT3qs-a74x562YT5WbIkGMEdkX6DzRizYg,2369
+k8s_audit_filter/resourses_field.py,sha256=3zuS8sLf5X84TvJad2zWaenyNj9Va8J8xudhLmZTWUE,2180
+k8s_audit_filter/rules.py,sha256=vuXE1etcQpnkhHUwcAIEw0Xf4GnSHecZWaZ8QPB-prY,1153
+k8s_audit_filter-0.2.0.dist-info/METADATA,sha256=NrBlTpT0dkCYCLcGfP0HDQcf6QohYgxh6L_dAqcF8aQ,5880
+k8s_audit_filter-0.2.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+k8s_audit_filter-0.2.0.dist-info/RECORD,,
```

