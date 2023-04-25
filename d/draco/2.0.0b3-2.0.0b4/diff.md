# Comparing `tmp/draco-2.0.0b3.tar.gz` & `tmp/draco-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draco-2.0.0b3.tar", max compression
+gzip compressed data, was "draco-2.0.0b4.tar", max compression
```

## Comparing `draco-2.0.0b3.tar` & `draco-2.0.0b4.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0     1083 2022-04-19 20:57:42.753033 draco-2.0.0b3/LICENSE
--rw-r--r--   0        0        0     2679 2023-01-11 19:13:55.006386 draco-2.0.0b3/README.md
--rw-r--r--   0        0        0      563 2022-10-20 16:32:52.848479 draco-2.0.0b3/draco/__init__.py
--rw-r--r--   0        0        0     1029 2023-01-17 22:29:53.428967 draco-2.0.0b3/draco/asp/constraints.lp
--rw-r--r--   0        0        0     2665 2023-01-17 22:29:53.429590 draco-2.0.0b3/draco/asp/define.lp
--rw-r--r--   0        0        0      732 2023-01-31 21:37:54.540762 draco-2.0.0b3/draco/asp/examples/binned_histogram.lp
--rw-r--r--   0        0        0      378 2023-01-31 21:37:54.540875 draco-2.0.0b3/draco/asp/examples/histogram.lp
--rw-r--r--   0        0        0      442 2023-01-31 21:37:54.540983 draco-2.0.0b3/draco/asp/examples/scatter.lp
--rw-r--r--   0        0        0     2343 2023-01-17 22:29:53.431346 draco-2.0.0b3/draco/asp/generate.lp
--rw-r--r--   0        0        0    12818 2023-01-17 22:29:53.431507 draco-2.0.0b3/draco/asp/hard.lp
--rw-r--r--   0        0        0     8080 2023-01-17 22:29:53.431678 draco-2.0.0b3/draco/asp/helpers.lp
--rw-r--r--   0        0        0       93 2022-08-01 22:17:04.349097 draco-2.0.0b3/draco/asp/optimize.lp
--rw-r--r--   0        0        0    29338 2023-01-17 22:29:53.431849 draco-2.0.0b3/draco/asp/soft.lp
--rw-r--r--   0        0        0     5131 2022-09-21 02:36:09.549479 draco-2.0.0b3/draco/asp/weights.lp
--rw-r--r--   0        0        0     2793 2022-10-20 16:32:52.848814 draco-2.0.0b3/draco/asp_utils.py
--rw-r--r--   0        0        0     4645 2022-10-20 16:32:52.848942 draco-2.0.0b3/draco/data_utils.py
--rw-r--r--   0        0        0     7333 2022-09-20 21:20:21.870111 draco-2.0.0b3/draco/debug.py
--rw-r--r--   0        0        0     6582 2022-10-20 16:53:07.528196 draco-2.0.0b3/draco/draco.py
--rw-r--r--   0        0        0     4700 2022-10-20 16:32:52.849656 draco-2.0.0b3/draco/fact_utils.py
--rw-r--r--   0        0        0     1014 2022-10-20 16:32:52.849759 draco-2.0.0b3/draco/learn.py
--rw-r--r--   0        0        0      894 2022-07-20 22:03:10.295971 draco-2.0.0b3/draco/programs.py
--rw-r--r--   0        0        0      152 2022-12-14 14:56:46.108312 draco-2.0.0b3/draco/renderer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 14:56:46.108392 draco-2.0.0b3/draco/renderer/altair/__init__.py
--rw-r--r--   0        0        0    21230 2023-01-31 21:37:54.541175 draco-2.0.0b3/draco/renderer/altair/altair_renderer.py
--rw-r--r--   0        0        0     9115 2023-01-31 21:37:54.541340 draco-2.0.0b3/draco/renderer/altair/types.py
--rw-r--r--   0        0        0      690 2022-12-14 14:56:46.108996 draco-2.0.0b3/draco/renderer/base_renderer.py
--rw-r--r--   0        0        0     4245 2022-10-20 16:32:52.850407 draco-2.0.0b3/draco/run.py
--rw-r--r--   0        0        0     3824 2022-10-20 16:32:52.850557 draco-2.0.0b3/draco/schema.py
--rw-r--r--   0        0        0      123 2022-10-20 16:53:07.528276 draco-2.0.0b3/draco/server/__init__.py
--rw-r--r--   0        0        0      581 2022-10-20 16:53:07.528361 draco-2.0.0b3/draco/server/__main__.py
--rw-r--r--   0        0        0     4021 2023-01-31 21:37:54.541484 draco-2.0.0b3/draco/server/draco_api.py
--rw-r--r--   0        0        0     1657 2022-10-20 16:53:07.528533 draco-2.0.0b3/draco/server/main.py
--rw-r--r--   0        0        0        0 2022-10-20 16:53:07.528571 draco-2.0.0b3/draco/server/models/__init__.py
--rw-r--r--   0        0        0      382 2022-10-20 16:53:07.528705 draco-2.0.0b3/draco/server/models/clingo.py
--rw-r--r--   0        0        0     1042 2022-10-20 16:53:07.528771 draco-2.0.0b3/draco/server/models/draco.py
--rw-r--r--   0        0        0      279 2022-10-20 16:53:07.528834 draco-2.0.0b3/draco/server/models/shared.py
--rw-r--r--   0        0        0      555 2022-10-20 16:53:07.528909 draco-2.0.0b3/draco/server/models/utility.py
--rw-r--r--   0        0        0      231 2022-10-20 16:53:07.528985 draco-2.0.0b3/draco/server/routers/__init__.py
--rw-r--r--   0        0        0     1503 2022-11-03 14:35:21.548943 draco-2.0.0b3/draco/server/routers/base.py
--rw-r--r--   0        0        0      945 2022-11-03 14:35:21.549065 draco-2.0.0b3/draco/server/routers/clingo.py
--rw-r--r--   0        0        0     1671 2022-11-03 14:35:21.549178 draco-2.0.0b3/draco/server/routers/draco.py
--rw-r--r--   0        0        0     1156 2022-11-03 14:35:21.549282 draco-2.0.0b3/draco/server/routers/utility.py
--rw-r--r--   0        0        0        0 2022-10-20 16:53:07.529314 draco-2.0.0b3/draco/server/services/__init__.py
--rw-r--r--   0        0        0      456 2022-10-20 16:53:07.529403 draco-2.0.0b3/draco/server/services/clingo.py
--rw-r--r--   0        0        0     1139 2022-10-20 16:53:07.529475 draco-2.0.0b3/draco/server/services/draco.py
--rw-r--r--   0        0        0     1036 2022-10-20 16:53:07.529542 draco-2.0.0b3/draco/server/services/utility.py
--rw-r--r--   0        0        0      460 2022-10-20 16:53:07.529609 draco-2.0.0b3/draco/server/utils.py
--rw-r--r--   0        0        0       87 2022-10-20 16:32:52.852528 draco-2.0.0b3/draco/types.py
--rw-r--r--   0        0        0      121 2022-07-20 22:03:10.273941 draco-2.0.0b3/draco/utils.py
--rw-r--r--   0        0        0     1344 2022-10-20 16:32:52.853238 draco-2.0.0b3/draco/weights.py
--rw-r--r--   0        0        0     1837 2023-01-31 22:51:29.044320 draco-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 draco-2.0.0b3/setup.py
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 draco-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-04-19 20:57:42.753033 draco-2.0.0b4/LICENSE
+-rw-r--r--   0        0        0     3549 2023-04-25 09:07:22.107407 draco-2.0.0b4/README.md
+-rw-r--r--   0        0        0      707 2023-04-25 09:07:22.130663 draco-2.0.0b4/draco/__init__.py
+-rw-r--r--   0        0        0      937 2023-03-14 21:04:07.214822 draco-2.0.0b4/draco/asp/constraints.lp
+-rw-r--r--   0        0        0     2665 2023-02-21 20:03:46.615187 draco-2.0.0b4/draco/asp/define.lp
+-rw-r--r--   0        0        0      732 2023-02-22 00:53:57.429000 draco-2.0.0b4/draco/asp/examples/binned_histogram.lp
+-rw-r--r--   0        0        0      378 2023-02-22 00:53:57.429114 draco-2.0.0b4/draco/asp/examples/histogram.lp
+-rw-r--r--   0        0        0      442 2023-02-22 00:53:57.429223 draco-2.0.0b4/draco/asp/examples/scatter.lp
+-rw-r--r--   0        0        0     2350 2023-03-14 21:04:07.215023 draco-2.0.0b4/draco/asp/generate.lp
+-rw-r--r--   0        0        0    13784 2023-04-25 09:07:22.130837 draco-2.0.0b4/draco/asp/hard.lp
+-rw-r--r--   0        0        0     8080 2023-02-21 20:03:46.616073 draco-2.0.0b4/draco/asp/helpers.lp
+-rw-r--r--   0        0        0       93 2022-08-01 22:17:04.349097 draco-2.0.0b4/draco/asp/optimize.lp
+-rw-r--r--   0        0        0    29338 2023-03-14 21:04:07.217532 draco-2.0.0b4/draco/asp/soft.lp
+-rw-r--r--   0        0        0     5131 2022-09-21 02:36:09.549479 draco-2.0.0b4/draco/asp/weights.lp
+-rw-r--r--   0        0        0     2793 2022-10-20 16:32:52.848814 draco-2.0.0b4/draco/asp_utils.py
+-rw-r--r--   0        0        0     4644 2023-02-22 00:53:57.429357 draco-2.0.0b4/draco/data_utils.py
+-rw-r--r--   0        0        0    11482 2023-04-25 09:07:22.132754 draco-2.0.0b4/draco/debug.py
+-rw-r--r--   0        0        0     6569 2023-03-14 21:04:07.219601 draco-2.0.0b4/draco/draco.py
+-rw-r--r--   0        0        0     4700 2022-10-20 16:32:52.849656 draco-2.0.0b4/draco/fact_utils.py
+-rw-r--r--   0        0        0     1014 2022-10-20 16:32:52.849759 draco-2.0.0b4/draco/learn.py
+-rw-r--r--   0        0        0      894 2022-07-20 22:03:10.295971 draco-2.0.0b4/draco/programs.py
+-rw-r--r--   0        0        0      152 2022-12-14 14:56:46.108312 draco-2.0.0b4/draco/renderer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-14 14:56:46.108392 draco-2.0.0b4/draco/renderer/altair/__init__.py
+-rw-r--r--   0        0        0    21230 2023-02-22 00:53:57.429553 draco-2.0.0b4/draco/renderer/altair/altair_renderer.py
+-rw-r--r--   0        0        0     9115 2023-02-22 00:53:57.429707 draco-2.0.0b4/draco/renderer/altair/types.py
+-rw-r--r--   0        0        0      690 2022-12-14 14:56:46.108996 draco-2.0.0b4/draco/renderer/base_renderer.py
+-rw-r--r--   0        0        0     4245 2022-10-20 16:32:52.850407 draco-2.0.0b4/draco/run.py
+-rw-r--r--   0        0        0     3824 2022-10-20 16:32:52.850557 draco-2.0.0b4/draco/schema.py
+-rw-r--r--   0        0        0      123 2022-10-20 16:53:07.528276 draco-2.0.0b4/draco/server/__init__.py
+-rw-r--r--   0        0        0      581 2022-10-20 16:53:07.528361 draco-2.0.0b4/draco/server/__main__.py
+-rw-r--r--   0        0        0     4245 2023-04-25 09:07:22.132928 draco-2.0.0b4/draco/server/draco_api.py
+-rw-r--r--   0        0        0     2333 2023-04-25 09:07:22.133360 draco-2.0.0b4/draco/server/main.py
+-rw-r--r--   0        0        0        0 2022-10-20 16:53:07.528571 draco-2.0.0b4/draco/server/models/__init__.py
+-rw-r--r--   0        0        0      382 2022-10-20 16:53:07.528705 draco-2.0.0b4/draco/server/models/clingo.py
+-rw-r--r--   0        0        0     1042 2022-10-20 16:53:07.528771 draco-2.0.0b4/draco/server/models/draco.py
+-rw-r--r--   0        0        0      231 2023-04-25 09:07:22.133555 draco-2.0.0b4/draco/server/models/renderer.py
+-rw-r--r--   0        0        0      279 2022-10-20 16:53:07.528834 draco-2.0.0b4/draco/server/models/shared.py
+-rw-r--r--   0        0        0      555 2022-10-20 16:53:07.528909 draco-2.0.0b4/draco/server/models/utility.py
+-rw-r--r--   0        0        0      290 2023-04-25 09:07:22.133756 draco-2.0.0b4/draco/server/routers/__init__.py
+-rw-r--r--   0        0        0     1503 2022-11-03 14:35:21.548943 draco-2.0.0b4/draco/server/routers/base.py
+-rw-r--r--   0        0        0      945 2022-11-03 14:35:21.549065 draco-2.0.0b4/draco/server/routers/clingo.py
+-rw-r--r--   0        0        0     1671 2022-11-03 14:35:21.549178 draco-2.0.0b4/draco/server/routers/draco.py
+-rw-r--r--   0        0        0     1157 2023-04-25 09:07:22.133856 draco-2.0.0b4/draco/server/routers/renderer.py
+-rw-r--r--   0        0        0     1156 2022-11-03 14:35:21.549282 draco-2.0.0b4/draco/server/routers/utility.py
+-rw-r--r--   0        0        0        0 2022-10-20 16:53:07.529314 draco-2.0.0b4/draco/server/services/__init__.py
+-rw-r--r--   0        0        0      456 2022-10-20 16:53:07.529403 draco-2.0.0b4/draco/server/services/clingo.py
+-rw-r--r--   0        0        0     1139 2022-10-20 16:53:07.529475 draco-2.0.0b4/draco/server/services/draco.py
+-rw-r--r--   0        0        0      417 2023-04-25 09:07:22.133951 draco-2.0.0b4/draco/server/services/renderer.py
+-rw-r--r--   0        0        0     1036 2022-10-20 16:53:07.529542 draco-2.0.0b4/draco/server/services/utility.py
+-rw-r--r--   0        0        0     1177 2023-04-25 09:07:22.134096 draco-2.0.0b4/draco/server/utils.py
+-rw-r--r--   0        0        0       87 2022-10-20 16:32:52.852528 draco-2.0.0b4/draco/types.py
+-rw-r--r--   0        0        0      121 2022-07-20 22:03:10.273941 draco-2.0.0b4/draco/utils.py
+-rw-r--r--   0        0        0     1344 2022-10-20 16:32:52.853238 draco-2.0.0b4/draco/weights.py
+-rw-r--r--   0        0        0     2233 2023-04-25 09:35:43.821264 draco-2.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 draco-2.0.0b4/PKG-INFO
```

### Comparing `draco-2.0.0b3/LICENSE` & `draco-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/asp/constraints.lp` & `draco-2.0.0b4/draco/asp/constraints.lp`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 % ====== Constraints ======
 
 % @definition(invalid_domain) Only valid domain values are allowed.
 violation(invalid_domain) :- attribute(P,_,V), domain(P,_), not domain(P,V).
 
 % @definition(duplicate_attribute) Do not define the same attribute twice.
-violation(duplicate_attribute) :- attribute(P,O,V1), attribute(P,O,V2), domain(P,_), V1!=V2.
+violation(duplicate_attribute) :- attribute(P,O,V1), attribute(P,O,V2), domain(P,_), V1<V2.
 
 % @definition(duplicate_field_name) Do not allow same field names.
-violation(duplicate_field_name) :- attribute((field,name),F1,N), attribute((field,name),F2,N), F1!=F2.
+violation(duplicate_field_name) :- attribute((field,name),F1,N), attribute((field,name),F2,N), F1<F2.
 
 % @definition(valid_fields) Only allow fields that have been defined.
 violation(existing_field) :- attribute(((encoding;facet),field),_,N), not attribute((field,name),_,N).
-violation(existing_field) :- helper(((encoding;facet),field),_,F), not entity(field,_,F).
 
 % @definition(attribute_entity) The type of an attribute path should link to the correct entity.
 violation(attribute_entity) :- attribute((P,_),E,_), entity(_,_,E), not entity(P,_,E).
 
 % @definition(violation) No violations allowed.
 :- violation(_).
```

### Comparing `draco-2.0.0b3/draco/asp/define.lp` & `draco-2.0.0b4/draco/asp/define.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/asp/examples/binned_histogram.lp` & `draco-2.0.0b4/draco/asp/examples/binned_histogram.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/asp/generate.lp` & `draco-2.0.0b4/draco/asp/generate.lp`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 % @generator(coordinates) Each view requires coordinates.
 required((view,coordinates)).
 
 % maximum number of additional marks for each view.
 #const max_marks = 2.
 { mark_id(V,0..max_marks-1) } :- entity(view,root,V).
 :- mark_id(V,ID), not mark_id(V,ID-1), ID > 0.
-{ entity(mark,V,(V,M)) } :- mark_id(V,M).
+{ entity(mark,V,(V,M)) } = 1 :- mark_id(V,M).
 
 % maximum number for additional encoding channels.
 #const max_encs = 4.
 { enc_id(M,0..max_encs-1) } :- entity(mark,V,M).
-:- enc_id(M,ID), not mark_id(M,ID-1), ID > 0.
-{ entity(encoding,M,(M,E)) } :- enc_id(M,E).
+:- enc_id(M,ID), not enc_id(M,ID-1), ID > 0.
+{ entity(encoding,M,(M,E)) } = 1 :- enc_id(M,E).
 
 % @generate(encoding_channel) Each encoding requires a channel.
 required((encoding,channel)).
 % @generator(mark_type) Each mark requires a type.
 required((mark,type)).
 % @generator(task) Each root requires a task.
 root_required(task).
```

### Comparing `draco-2.0.0b3/draco/asp/hard.lp` & `draco-2.0.0b4/draco/asp/hard.lp`

 * *Files 4% similar despite different names*

```diff
@@ -70,27 +70,23 @@
     attribute((field,min),F,MIN),
     attribute((field,max),F,MAX),
     MIN < 0,
     MAX > 0.
 
 % @hard(encoding_repeat_channel) Cannot use single channels twice for the same mark.
 violation(encoding_repeat_channel) :-
-    entity(encoding,M,E1),
-    entity(encoding,M,E2),
-    attribute((encoding,channel),E1,C),
-    attribute((encoding,channel),E2,C),
-    E1 > E2.
+    entity(mark,_,M),
+    domain(single_channel,C),
+    2 <= #count { E : entity(encoding,M,E), attribute((encoding,channel),E,C) }.
 
 % @hard(scale_repeat_channel) Cannot use single channels twice for the same view.
 violation(scale_repeat_channel) :-
-    entity(scale,V,S1),
-    entity(scale,V,S2),
-    attribute((scale,channel),S1,C),
-    attribute((scale,channel),S2,C),
-    S1 > S2.
+    entity(view,root,V),
+    domain(single_channel,C),
+    2 <= #count { S : entity(scale,V,S), attribute((scale,channel),S,C) }.
 
 % @hard(encoding_channel_without_scale) Encoding channel doesn't have a corresponding scale channel.
 violation(encoding_channel_without_scale) :-
     entity(mark,V,M),
     helper((mark,channel),M,C),
     not domain(scale_channel,V,C).
 
@@ -257,14 +253,31 @@
 % @hard(col_no_x) Don't use column without x. Just using x is simpler.
 violation(col_no_x) :-
     entity(facet,V,F),
     attribute((facet,channel),F,col),
     entity(mark,V,M),
     not helper((mark,channel),M,x).
 
+% @hard(facet_no_duplicate_field) Don't use the same field twice when faceting.
+violation(facet_no_duplicate_field) :-
+    entity(facet,V,F1),
+    entity(facet,V,F2),
+    F1 != F2,
+    attribute((facet,field),F1,F),
+    attribute((facet,field),F2,F).
+
+% @hard(facet_no_duplicate_channel_on_same_view) Don't use the same channel twice for faceting on the same view.
+violation(facet_no_duplicate_channel_on_same_view) :-
+    entity(view,root,V),
+    entity(facet,V,F1),
+    entity(facet,V,F2),
+    F1 != F2,
+    attribute((facet,channel),F1,C),
+    attribute((facet,channel),F2,C).
+
 % @hard(stack_without_bar_area) Only use stacking for bar and area.
 violation(stack_without_bar_area) :-
     helper(mark_with_stack,M),
     not attribute((mark,type),M,bar),
     not attribute((mark,type),M,area).
 
 % @hard(stack_without_summative_agg) Don't stack if aggregation is not summative (summative are count, sum, distinct, valid, missing).
@@ -343,7 +356,19 @@
     attribute((field,max),F,MAX),
     MIN > MAX.
 
 % @hard(invalid_non_string_freq) Frequency for strings only.
 violation(invalid_non_string_freq) :-
     attribute((field,freq),F,_),
     not attribute((field,type),F,string).
+
+% @hard(enforce_order) property should follow natural order for generated entities.
+violation(enforce_order):-
+    entity(view,root,V), M1 < M2,
+    attribute((mark,type),(V,M1),T1),
+    attribute((mark,type),(V,M2),T2),
+    not T1 < T2.
+violation(enforce_order):-
+    entity(mark,_,M), E1 < E2,
+    attribute((encoding,channel),(M,E1),C1),
+    attribute((encoding,channel),(M,E2),C2),
+    not C1 < C2.
```

### Comparing `draco-2.0.0b3/draco/asp/helpers.lp` & `draco-2.0.0b4/draco/asp/helpers.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/asp/soft.lp` & `draco-2.0.0b4/draco/asp/soft.lp`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     not helper((mark,channel),M,x).
 
 % @soft(binned_orientation_not_x) Prefer binned quantative on x axis.
 preference(binned_orientation_not_x,E) :-
     attribute((field,type),F,(number;datetime)),
     helper((encoding,field),E,F),
     attribute((encoding,binning),E,_),
-    not attribute((encoding,channel),E,x).
+    not attribute((encoding,channel),_,x).
 
 % @soft(high_cardinality_ordinal) Prefer not to use ordinal for fields with high cardinality.
 preference(high_cardinality_ordinal,E) :-
     helper(encoding_cardinality,E,N),
     helper((encoding,scale_type),E,ordinal),
     N > 30.
```

### Comparing `draco-2.0.0b3/draco/asp/weights.lp` & `draco-2.0.0b4/draco/asp/weights.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/asp_utils.py` & `draco-2.0.0b4/draco/asp_utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/data_utils.py` & `draco-2.0.0b4/draco/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     """given a specs partition, convert them into feature vectors."""
     processed_specs, fields, partition_data = input_data
 
     columns = get_nested_index()
     dfs = []
 
     for example in partition_data:
-
         neg_feature_vec = count_preferences_memoized(
             processed_specs, f"{example['pair_id']}_{fields[0]}", example[fields[0]]
         )
 
         pos_feature_vec = count_preferences_memoized(
             processed_specs, f"{example['pair_id']}_{fields[1]}", example[fields[1]]
         )
```

### Comparing `draco-2.0.0b3/draco/draco.py` & `draco-2.0.0b4/draco/draco.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,37 +94,38 @@
         and hard constraints.
 
         :param spec: The specification to check
         """
         if not isinstance(spec, str):
             spec = "\n".join(spec)
 
-        program = self.define + self.constraints + self.helpers + self.hard + spec
+        program = [self.define, self.constraints, self.helpers, self.hard, spec]
+
         return is_satisfiable(program)
 
     def complete_spec(self, spec: Specification, models=1):
         """Get optimal completions for the partial input specification.
 
         :param spec: The partial specification to complete.
         :param models: The number of completions to return, defaults to 1
         """
         if not isinstance(spec, str):
             spec = "\n".join(spec)
 
-        program = (
-            self.define
-            + self.generate
-            + self.constraints
-            + self.helpers
-            + self.hard
-            + self.soft
-            + self.assign_weights
-            + self.optimize
-            + spec
-        )
+        program = [
+            self.define,
+            self.generate,
+            self.constraints,
+            self.helpers,
+            self.hard,
+            self.soft,
+            self.assign_weights,
+            self.optimize,
+            spec,
+        ]
 
         # pass the weights as constraint to Clingo
         args = [f"-c {w}={v}" for w, v in self.weights.items()]
 
         return run_clingo(program, models, True, args)
 
     def count_preferences(self, spec: Specification):
@@ -135,15 +136,15 @@
         and soft constraints.
 
         :param spec: The specification to check
         """
         if not isinstance(spec, str):
             spec = "\n".join(spec)
 
-        program = self.define + self.constraints + self.helpers + self.soft + spec
+        program = [self.define, self.constraints, self.helpers, self.soft, spec]
 
         try:
             result: DefaultDict[str, int] = defaultdict(int)
 
             model = next(run_clingo(program, 1))
 
             for symbol in model.answer_set:
@@ -162,21 +163,21 @@
         constraint that disallows violations), helpers, and hard constraints.
 
         :param spec: The specification to check
         """
         if not isinstance(spec, str):
             spec = "\n".join(spec)
 
-        program = (
-            self.define
-            + self._constraints_no_violation
-            + self.helpers
-            + self.hard
-            + spec
-        )
+        program = [
+            self.define,
+            self._constraints_no_violation,
+            self.helpers,
+            self.hard,
+            spec,
+        ]
 
         try:
             model = next(run_clingo(program, 1))
 
             return [
                 symbol.arguments[0].name
                 for symbol in model.answer_set
```

### Comparing `draco-2.0.0b3/draco/fact_utils.py` & `draco-2.0.0b4/draco/fact_utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/learn.py` & `draco-2.0.0b4/draco/learn.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/programs.py` & `draco-2.0.0b4/draco/programs.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/renderer/altair/altair_renderer.py` & `draco-2.0.0b4/draco/renderer/altair/altair_renderer.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/renderer/altair/types.py` & `draco-2.0.0b4/draco/renderer/altair/types.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/renderer/base_renderer.py` & `draco-2.0.0b4/draco/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/run.py` & `draco-2.0.0b4/draco/run.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/schema.py` & `draco-2.0.0b4/draco/schema.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/__main__.py` & `draco-2.0.0b4/draco/server/__main__.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/draco_api.py` & `draco-2.0.0b4/draco/server/draco_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,19 @@
     ):
         """
         Creates a new :code:`DracoAPI` instance. If no parameters are passed in,
         the default configuration of :code:`Draco` and :code:`FastAPI` is used.
 
         The :code:`base_routers` parameter governs the routers which get registered
         to the :code:`FastAPI` instance, that is, they define the actual endpoints
-        which will be available. Three routers get registered automatically:
+        which will be available. Default routers get registered automatically:
 
         - :code:`DracoRouter` - exposes the core functionality of :code:`Draco`
         - :code:`ClingoRouter` - exposes the functionality of the Clingo solver
+        - :code:`RendererRouter` - exposes renderer functionality
         - :code:`UtilityRouter` - exposes various utility endpoints
 
         If you wish to enable only a subset of these endpoints,
         you can pass in a list of routers to the :code:`base_routers` parameter.
         The routers will be registered in the order they appear in the list.
         Note that to avoid inconsistencies between the :code:`Draco` instance
         and the routers, you should declare a :code:`Draco` instance first,
@@ -70,16 +71,22 @@
         self.draco = draco
         self.app = app
 
         # Creating the base routers if none were passed in
         if base_routers is None:
             draco_router = routers.DracoRouter(draco)
             clingo_router = routers.ClingoRouter(draco)
+            renderer_router = routers.RendererRouter(draco)
             utility_router = routers.UtilityRouter(draco)
-            self.base_routers = [clingo_router, draco_router, utility_router]
+            self.base_routers = [
+                clingo_router,
+                draco_router,
+                renderer_router,
+                utility_router,
+            ]
         else:
             self.base_routers = base_routers
 
         # Make sure we have at least one router
         if len(self.base_routers) == 0:
             raise ValueError(
                 "At least one `BaseDracoRouter` must be provided. "
```

### Comparing `draco-2.0.0b3/draco/server/main.py` & `draco-2.0.0b4/draco/server/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,90 @@
 import argparse
 
 import uvicorn
 
+from . import utils
 from .draco_api import DracoAPI
 
 
 class DracoServerArgs(argparse.Namespace):
     """Namespace for the CLI arguments expected from the user."""
 
     host: str
     port: int
     reload: bool
+    show_routes: bool
 
 
-__DEFAULT_ARGS__ = DracoServerArgs(host="127.0.0.1", port=8000, reload=False)
+__DEFAULT_ARGS__ = DracoServerArgs(
+    host="127.0.0.1", port=8000, reload=False, show_routes=False
+)
 
 
 def argument_parser() -> argparse.ArgumentParser:
     """
     Create an argument parser for the Draco server CLI.
 
     :return: the argument parser used to collect arguments from the user.
     """
     parser = argparse.ArgumentParser(
         description="FastAPI Server exposing the capabilities of Draco",
         usage="python -m draco.server [options]",
     )
-    parser.add_argument(
+
+    # Options related to running the server
+    run_group = parser.add_argument_group(
+        "Run Options", "Options related to running the server"
+    )
+    run_group.add_argument(
         "--host",
         type=str,
         default=__DEFAULT_ARGS__.host,
         help=f"Host to run server on. Defaults to {__DEFAULT_ARGS__.host}",
     )
-    parser.add_argument(
+    run_group.add_argument(
         "--port",
         type=int,
         default=__DEFAULT_ARGS__.port,
         help=f"Port to run server on. Defaults to {__DEFAULT_ARGS__.port}",
     )
-    parser.add_argument(
+    run_group.add_argument(
         "--reload",
         action="store_true",
         default=__DEFAULT_ARGS__.reload,
         help="Enable auto-reloading of the server on code changes.",
     )
+
+    # Options related to the server utilities
+    utility_group = parser.add_mutually_exclusive_group()
+    utility_group.add_argument(
+        "--show-routes",
+        action="store_true",
+        default=__DEFAULT_ARGS__.show_routes,
+        help="Show the routes registered by the server and exit",
+    )
+
     return parser
 
 
 def main(
     draco_api: DracoAPI | None = None,
     args: DracoServerArgs = __DEFAULT_ARGS__,
 ):
     """
     Run the Draco server.
 
     :param draco_api: the DracoAPI object to use for the server.
     :param args: the arguments to use in the :code:`uvicorn.run` call.
     """
+    used_draco_api = draco_api or DracoAPI()
+
+    if args.show_routes:
+        print(utils.tabulate_routes(used_draco_api.app))
+        return
+
     uvicorn.run(
-        (draco_api or DracoAPI()).app,
+        used_draco_api.app,
         host=args.host,
         port=args.port,
         reload=args.reload,
     )
```

### Comparing `draco-2.0.0b3/draco/server/models/draco.py` & `draco-2.0.0b4/draco/server/models/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/models/utility.py` & `draco-2.0.0b4/draco/server/models/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/routers/base.py` & `draco-2.0.0b4/draco/server/routers/base.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/routers/clingo.py` & `draco-2.0.0b4/draco/server/routers/clingo.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/routers/draco.py` & `draco-2.0.0b4/draco/server/routers/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/routers/utility.py` & `draco-2.0.0b4/draco/server/routers/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/services/draco.py` & `draco-2.0.0b4/draco/server/services/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/server/services/utility.py` & `draco-2.0.0b4/draco/server/services/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/draco/weights.py` & `draco-2.0.0b4/draco/weights.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b3/pyproject.toml` & `draco-2.0.0b4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "draco"
-version = "2.0.0b3"
+version = "2.0.0b4"
 description = "Visualization recommendation using constraints"
 authors = [
     "Dominik Moritz <domoritz@cmu.edu>",
     "Chenglong Wang <clwang@cs.washington.edu>",
     "JunranY <junran@cs.washington.edu>",
     "Zehua Zeng <zhzeng@umd.edu>",
     "Péter Ferenc Gyarmati <peter.ferenc.gyarmati@univie.ac.at>"
@@ -24,47 +24,68 @@
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
+altair = "^4.2.2"
 clingo = "^5.5.2"
-matplotlib = "^3.6.0"
-pandas = "^1.4.2"
+fastapi = ">=0.85,<0.96"
+pandas = ">=1.4.2,<3.0.0"
+pydantic = "^1.10.5"
 python = ">=3.10.0,<3.11"
-scikit-learn = "^1.1.1"
-fastapi = ">=0.85,<0.90"
-uvicorn = ">=0.18.3,<0.21.0"
+scikit-learn = "^1.2.1"
+uvicorn = ">=0.18.3,<0.22.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
-altair = "^4.2.0"
-black = {extras = ["jupyter"], version = "^22.12.0"}
-deepdiff = "^6.2.1"
-flake8 = "^5.0.4"
-flake8-black = "^0.3.3"
-ipywidgets = "^7.7.2"
-isort = "^5.10.1"
-jupyter-book = "^0.13.1"
+black = { extras = ["jupyter"], version = "^23.1.0" }
+mypy = ">=0.990,<1.3"
+pandas-stubs = ">=1.5.1,<3.0.0"
+pre-commit = ">=2.20,<4.0"
+pytype = ">=2022.11.10,<2024.0.0"
+ruff = ">=0.0.253,<0.0.263"
+types-tabulate = "^0.9.0.2"
+
+[tool.poetry.group.docs.dependencies]
+ipywidgets = ">=7.7.2,<9.0.0"
+jupyter-book = ">=0.13.1,<0.16.0"
 jupyterlab = "^3.3.0"
-mypy = "^0.990"
-pandas-stubs = "^1.5.1"
-pre-commit = "^2.20.0"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pytype = "^2022.11.10"
+matplotlib = "^3.6.0"
 sphinx-autodoc-typehints = "^1.19.1"
 toml = "^0.10.2"
 types-pkg-resources = "^0.1.2"
 vega-datasets = "^0.9.0"
-wheel = "^0.38.4"
-httpx = "^0.23.0"
+wheel = ">=0.38.4,<0.41.0"
+
+[tool.poetry.group.test.dependencies]
+deepdiff = "^6.2.1"
+httpx = ">=0.23,<0.25"
+pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
+
+[tool.poetry.group.web]
+optional = true
+
+[tool.poetry.group.web.dependencies]
+jupyterlite = "^0.1.0"
+libarchive-c = "^4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["draco"]
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+line-length = 88
+select = [
+    "E",
+    "F",
+    "W",
+    # isort
+    "I001"
+]
+src = ["draco"]
+fix = true
```

### Comparing `draco-2.0.0b3/setup.py` & `draco-2.0.0b4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: draco
+Version: 2.0.0b4
+Summary: Visualization recommendation using constraints
+Home-page: https://github.com/cmudig/draco2
+License: MIT
+Keywords: constraints,visualization,design,charts
+Author: Dominik Moritz
+Author-email: domoritz@cmu.edu
+Requires-Python: >=3.10.0,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: altair (>=4.2.2,<5.0.0)
+Requires-Dist: clingo (>=5.5.2,<6.0.0)
+Requires-Dist: fastapi (>=0.85,<0.96)
+Requires-Dist: pandas (>=1.4.2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: uvicorn (>=0.18.3,<0.22.0)
+Project-URL: Documentation, https://dig.cmu.edu/draco2/
+Project-URL: Repository, https://github.com/cmudig/draco2
+Description-Content-Type: text/markdown
+
+<p align="center">
+   <a href="https://github.com/cmudig/draco2">
+      <picture>
+         <source media="(prefers-color-scheme: dark)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png">
+         <source media="(prefers-color-scheme: light)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-dark.png">
+         <img alt="The Draco logo. A set of circles connected by lines depicting the draco star constellation." src="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png" width=260>
+      </picture>
+   </a>
+</p>
+
+# Draco v2
+
+[![Open in GitHub Codespaces](https://img.shields.io/badge/launch-Codespaces-blue)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=313704611&machine=standardLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+[![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/draco/)
+[![npm](https://img.shields.io/npm/v/draco-pyodide)](https://www.npmjs.com/package/draco-pyodide)
+[![Test](https://github.com/cmudig/draco2/actions/workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/actions/workflows/test.yml)
+[![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![codecov](https://codecov.io/gh/cmudig/draco2/branch/main/graph/badge.svg)](https://codecov.io/gh/cmudig/draco2)
+[![Jupyter Book Badge](https://raw.githubusercontent.com/executablebooks/jupyter-book/master/docs/images/badge.svg)](https://dig.cmu.edu/draco2)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cmudig/draco2/HEAD)
+[![Lite](https://gist.githubusercontent.com/willeppy/35cdc20a3fc26e393ce76f1df35bcdfc/raw/a7fca1d0a2d62c2b49f60c0217dffbd0fe404471/lite-badge-launch-small.svg)](https://dig.cmu.edu/draco2/jupyterlite)
+[![Pyodide Console](https://img.shields.io/badge/🐍%20launch-Pyodide%20Console-yellowgreen)](https://dig.cmu.edu/draco2/jupyterlite/static/pyodide/console.html)
+
+**Work in Progress**
+
+Draco is a formal framework for representing design knowledge about effective visualization design as a collection of
+constraints. You can use Draco to find effective visualization designs or validate existing ones. Draco's constraints
+are based on Answer Set Programming (ASP) and solved with the [Clingo](https://github.com/potassco/clingo) constraint
+solver. We also implemented a way to learn weights for the recommendation system directly from the results of graphical
+perception experiment. Draco v2 is a much improved version of the first iteration of
+[Draco](https://github.com/uwdata/draco).
+
+## Documentation
+
+Read about Draco in the online book at [https://dig.cmu.edu/draco2/](https://dig.cmu.edu/draco2/) or launch it in
+interactive mode using [Binder](https://mybinder.org/v2/gh/cmudig/draco2/HEAD). In the documentation, we just refer to
+_Draco_ without a version.
+
+## What's different from [Draco v1](https://github.com/uwdata/draco)?
+
+- Draco v2 is completely written in Python. No more need to run both Python and Node. We still use ASP for the knowledge
+  base.
+- Generalized and extended chart specification format. The new format is more extensible with custom properties.
+- Support for multiple views and view composition.
+- High test-coverage, documentation, and updated development tooling.
 
-packages = \
-['draco',
- 'draco.renderer',
- 'draco.renderer.altair',
- 'draco.server',
- 'draco.server.models',
- 'draco.server.routers',
- 'draco.server.services']
-
-package_data = \
-{'': ['*'], 'draco': ['asp/*', 'asp/examples/*']}
-
-install_requires = \
-['clingo>=5.5.2,<6.0.0',
- 'fastapi>=0.85,<0.90',
- 'matplotlib>=3.6.0,<4.0.0',
- 'pandas>=1.4.2,<2.0.0',
- 'scikit-learn>=1.1.1,<2.0.0',
- 'uvicorn>=0.18.3,<0.21.0']
-
-setup_kwargs = {
-    'name': 'draco',
-    'version': '2.0.0b3',
-    'description': 'Visualization recommendation using constraints',
-    'long_description': '<p align="center">\n   <a href="https://github.com/cmudig/draco2">\n      <picture>\n         <source media="(prefers-color-scheme: dark)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png">\n         <source media="(prefers-color-scheme: light)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-dark.png">\n         <img alt="The Draco logo. A set of circles connected by lines depicting the draco star constellation." src="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png" width=260>\n      </picture>\n   </a>\n</p>\n\n# Draco v2\n\n[![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/draco/)\n[![Test](https://github.com/cmudig/draco2/actions/workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/actions/workflows/test.yml)\n[![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![codecov](https://codecov.io/gh/cmudig/draco2/branch/main/graph/badge.svg)](https://codecov.io/gh/cmudig/draco2)\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cmudig/draco2/HEAD)\n\n**Work in Progress**\n\nDraco is a formal framework for representing design knowledge about effective visualization design as a collection of\nconstraints. You can use Draco to find effective visualization designs or validate existing ones. Draco\'s constraints\nare based on Answer Set Programming (ASP) and solved with the [Clingo](https://github.com/potassco/clingo) constraint\nsolver. We also implemented a way to learn weights for the recommendation system directly from the results of graphical\nperception experiment. Draco v2 is a much improved version of the first iteration of\n[Draco](https://github.com/uwdata/draco).\n\n## Documentation\n\nRead about Draco in the online book at [https://dig.cmu.edu/draco2/](https://dig.cmu.edu/draco2/) or launch it in\ninteractive mode using [Binder](https://mybinder.org/v2/gh/cmudig/draco2/HEAD). In the documentation, we just refer to\n_Draco_ without a version.\n\n## What\'s different from [Draco v1](https://github.com/uwdata/draco)?\n\n- Draco v2 is completely written in Python. No more need to run both Python and Node. We still use ASP for the knowledge\n  base.\n- Generalized and extended chart specification format. The new format is more extensible with custom properties.\n- Support for multiple views and view composition.\n- High test-coverage, documentation, and updated development tooling.\n\n## Contributing\n\nWe welcome any input, feedback, bug reports, and contributions. You can learn about setting up your development\nenvironment in [CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/CONTRIBUTING.md).\n',
-    'author': 'Dominik Moritz',
-    'author_email': 'domoritz@cmu.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cmudig/draco2',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10.0,<3.11',
-}
+## Contributing
 
+We welcome any input, feedback, bug reports, and contributions. You can learn about setting up your development
+environment in [CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/CONTRIBUTING.md).
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,45 +1,58 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['draco',
-'draco.renderer', 'draco.renderer.altair', 'draco.server',
-'draco.server.models', 'draco.server.routers', 'draco.server.services']
-package_data = \ {'': ['*'], 'draco': ['asp/*', 'asp/examples/*']}
-install_requires = \ ['clingo>=5.5.2,<6.0.0', 'fastapi>=0.85,<0.90',
-'matplotlib>=3.6.0,<4.0.0', 'pandas>=1.4.2,<2.0.0', 'scikit-
-learn>=1.1.1,<2.0.0', 'uvicorn>=0.18.3,<0.21.0'] setup_kwargs = { 'name':
-'draco', 'version': '2.0.0b3', 'description': 'Visualization recommendation
-using constraints', 'long_description': '
- \n \n_\n_\n_\n_[The_Draco_logo._A_set_of_circles_connected_by_lines_depicting
-                     the_draco_star_constellation.]\n_\n\n
-\n\n# Draco v2\n\n[![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://
-pypi.org/project/draco/)\n[![Test](https://github.com/cmudig/draco2/actions/
-workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/actions/
-workflows/test.yml)\n[![code style black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black)\n[![codecov]
+Metadata-Version: 2.1 Name: draco Version: 2.0.0b4 Summary: Visualization
+recommendation using constraints Home-page: https://github.com/cmudig/draco2
+License: MIT Keywords: constraints,visualization,design,charts Author: Dominik
+Moritz Author-email: domoritz@cmu.edu Requires-Python: >=3.10.0,<3.11
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
+Classifier: Environment :: MacOS X Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+MacOS :: MacOS X Classifier: Operating System :: POSIX :: Linux Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
+altair (>=4.2.2,<5.0.0) Requires-Dist: clingo (>=5.5.2,<6.0.0) Requires-Dist:
+fastapi (>=0.85,<0.96) Requires-Dist: pandas (>=1.4.2,<3.0.0) Requires-Dist:
+pydantic (>=1.10.5,<2.0.0) Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: uvicorn
+(>=0.18.3,<0.22.0) Project-URL: Documentation, https://dig.cmu.edu/draco2/
+Project-URL: Repository, https://github.com/cmudig/draco2 Description-Content-
+Type: text/markdown
+  ___[The_Draco_logo._A_set_of_circles_connected_by_lines_depicting_the_draco
+                             star_constellation.]_
+# Draco v2 [![Open in GitHub Codespaces](https://img.shields.io/badge/launch-
+Codespaces-blue)](https://github.com/codespaces/
+new?hide_repo_select=true&ref=main&repo=313704611&machine=standardLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+[![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/
+draco/) [![npm](https://img.shields.io/npm/v/draco-pyodide)](https://
+www.npmjs.com/package/draco-pyodide) [![Test](https://github.com/cmudig/draco2/
+actions/workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/
+actions/workflows/test.yml) [![code style black](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
 (https://codecov.io/gh/cmudig/draco2/branch/main/graph/badge.svg)](https://
-codecov.io/gh/cmudig/draco2)\n[![Binder](https://mybinder.org/badge_logo.svg)]
-(https://mybinder.org/v2/gh/cmudig/draco2/HEAD)\n\n**Work in
-Progress**\n\nDraco is a formal framework for representing design knowledge
-about effective visualization design as a collection of\nconstraints. You can
-use Draco to find effective visualization designs or validate existing ones.
-Draco\'s constraints\nare based on Answer Set Programming (ASP) and solved with
-the [Clingo](https://github.com/potassco/clingo) constraint\nsolver. We also
-implemented a way to learn weights for the recommendation system directly from
-the results of graphical\nperception experiment. Draco v2 is a much improved
-version of the first iteration of\n[Draco](https://github.com/uwdata/
-draco).\n\n## Documentation\n\nRead about Draco in the online book at [https://
-dig.cmu.edu/draco2/](https://dig.cmu.edu/draco2/) or launch it in\ninteractive
-mode using [Binder](https://mybinder.org/v2/gh/cmudig/draco2/HEAD). In the
-documentation, we just refer to\n_Draco_ without a version.\n\n## What\'s
-different from [Draco v1](https://github.com/uwdata/draco)?\n\n- Draco v2 is
-completely written in Python. No more need to run both Python and Node. We
-still use ASP for the knowledge\n base.\n- Generalized and extended chart
-specification format. The new format is more extensible with custom
-properties.\n- Support for multiple views and view composition.\n- High test-
-coverage, documentation, and updated development tooling.\n\n##
-Contributing\n\nWe welcome any input, feedback, bug reports, and contributions.
-You can learn about setting up your development\nenvironment in
-[CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/
-CONTRIBUTING.md).\n', 'author': 'Dominik Moritz', 'author_email':
-'domoritz@cmu.edu', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/cmudig/draco2', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.10.0,<3.11', } setup(**setup_kwargs)
+codecov.io/gh/cmudig/draco2) [![Jupyter Book Badge](https://
+raw.githubusercontent.com/executablebooks/jupyter-book/master/docs/images/
+badge.svg)](https://dig.cmu.edu/draco2) [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/cmudig/draco2/HEAD) [![Lite](https:
+//gist.githubusercontent.com/willeppy/35cdc20a3fc26e393ce76f1df35bcdfc/raw/
+a7fca1d0a2d62c2b49f60c0217dffbd0fe404471/lite-badge-launch-small.svg)](https://
+dig.cmu.edu/draco2/jupyterlite) [![Pyodide Console](https://img.shields.io/
+badge/ð%20launch-Pyodide%20Console-yellowgreen)](https://dig.cmu.edu/draco2/
+jupyterlite/static/pyodide/console.html) **Work in Progress** Draco is a formal
+framework for representing design knowledge about effective visualization
+design as a collection of constraints. You can use Draco to find effective
+visualization designs or validate existing ones. Draco's constraints are based
+on Answer Set Programming (ASP) and solved with the [Clingo](https://
+github.com/potassco/clingo) constraint solver. We also implemented a way to
+learn weights for the recommendation system directly from the results of
+graphical perception experiment. Draco v2 is a much improved version of the
+first iteration of [Draco](https://github.com/uwdata/draco). ## Documentation
+Read about Draco in the online book at [https://dig.cmu.edu/draco2/](https://
+dig.cmu.edu/draco2/) or launch it in interactive mode using [Binder](https://
+mybinder.org/v2/gh/cmudig/draco2/HEAD). In the documentation, we just refer to
+_Draco_ without a version. ## What's different from [Draco v1](https://
+github.com/uwdata/draco)? - Draco v2 is completely written in Python. No more
+need to run both Python and Node. We still use ASP for the knowledge base. -
+Generalized and extended chart specification format. The new format is more
+extensible with custom properties. - Support for multiple views and view
+composition. - High test-coverage, documentation, and updated development
+tooling. ## Contributing We welcome any input, feedback, bug reports, and
+contributions. You can learn about setting up your development environment in
+[CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/CONTRIBUTING.md).
```

### Comparing `draco-2.0.0b3/PKG-INFO` & `draco-2.0.0b4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,29 @@
-Metadata-Version: 2.1
-Name: draco
-Version: 2.0.0b3
-Summary: Visualization recommendation using constraints
-Home-page: https://github.com/cmudig/draco2
-License: MIT
-Keywords: constraints,visualization,design,charts
-Author: Dominik Moritz
-Author-email: domoritz@cmu.edu
-Requires-Python: >=3.10.0,<3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: clingo (>=5.5.2,<6.0.0)
-Requires-Dist: fastapi (>=0.85,<0.90)
-Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: uvicorn (>=0.18.3,<0.21.0)
-Project-URL: Documentation, https://dig.cmu.edu/draco2/
-Project-URL: Repository, https://github.com/cmudig/draco2
-Description-Content-Type: text/markdown
-
 <p align="center">
    <a href="https://github.com/cmudig/draco2">
       <picture>
          <source media="(prefers-color-scheme: dark)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png">
          <source media="(prefers-color-scheme: light)" srcset="https://github.com/cmudig/draco2/raw/main/docs/logo-dark.png">
          <img alt="The Draco logo. A set of circles connected by lines depicting the draco star constellation." src="https://github.com/cmudig/draco2/raw/main/docs/logo-light.png" width=260>
       </picture>
    </a>
 </p>
 
 # Draco v2
 
+[![Open in GitHub Codespaces](https://img.shields.io/badge/launch-Codespaces-blue)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=313704611&machine=standardLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
 [![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/draco/)
+[![npm](https://img.shields.io/npm/v/draco-pyodide)](https://www.npmjs.com/package/draco-pyodide)
 [![Test](https://github.com/cmudig/draco2/actions/workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/actions/workflows/test.yml)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/cmudig/draco2/branch/main/graph/badge.svg)](https://codecov.io/gh/cmudig/draco2)
+[![Jupyter Book Badge](https://raw.githubusercontent.com/executablebooks/jupyter-book/master/docs/images/badge.svg)](https://dig.cmu.edu/draco2)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cmudig/draco2/HEAD)
+[![Lite](https://gist.githubusercontent.com/willeppy/35cdc20a3fc26e393ce76f1df35bcdfc/raw/a7fca1d0a2d62c2b49f60c0217dffbd0fe404471/lite-badge-launch-small.svg)](https://dig.cmu.edu/draco2/jupyterlite)
+[![Pyodide Console](https://img.shields.io/badge/🐍%20launch-Pyodide%20Console-yellowgreen)](https://dig.cmu.edu/draco2/jupyterlite/static/pyodide/console.html)
 
 **Work in Progress**
 
 Draco is a formal framework for representing design knowledge about effective visualization design as a collection of
 constraints. You can use Draco to find effective visualization designs or validate existing ones. Draco's constraints
 are based on Answer Set Programming (ASP) and solved with the [Clingo](https://github.com/potassco/clingo) constraint
 solver. We also implemented a way to learn weights for the recommendation system directly from the results of graphical
@@ -69,8 +44,7 @@
 - Support for multiple views and view composition.
 - High test-coverage, documentation, and updated development tooling.
 
 ## Contributing
 
 We welcome any input, feedback, bug reports, and contributions. You can learn about setting up your development
 environment in [CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/CONTRIBUTING.md).
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,46 +1,41 @@
-Metadata-Version: 2.1 Name: draco Version: 2.0.0b3 Summary: Visualization
-recommendation using constraints Home-page: https://github.com/cmudig/draco2
-License: MIT Keywords: constraints,visualization,design,charts Author: Dominik
-Moritz Author-email: domoritz@cmu.edu Requires-Python: >=3.10.0,<3.11
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: Environment :: MacOS X Classifier: License :: OSI Approved :: MIT
-License Classifier: Natural Language :: English Classifier: Operating System ::
-MacOS :: MacOS X Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
-clingo (>=5.5.2,<6.0.0) Requires-Dist: fastapi (>=0.85,<0.90) Requires-Dist:
-matplotlib (>=3.6.0,<4.0.0) Requires-Dist: pandas (>=1.4.2,<2.0.0) Requires-
-Dist: scikit-learn (>=1.1.1,<2.0.0) Requires-Dist: uvicorn (>=0.18.3,<0.21.0)
-Project-URL: Documentation, https://dig.cmu.edu/draco2/ Project-URL:
-Repository, https://github.com/cmudig/draco2 Description-Content-Type: text/
-markdown
   ___[The_Draco_logo._A_set_of_circles_connected_by_lines_depicting_the_draco
                              star_constellation.]_
-# Draco v2 [![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/
-project/draco/) [![Test](https://github.com/cmudig/draco2/actions/workflows/
-test.yml/badge.svg)](https://github.com/cmudig/draco2/actions/workflows/
-test.yml) [![code style black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) [![codecov](https://codecov.io/gh/
-cmudig/draco2/branch/main/graph/badge.svg)](https://codecov.io/gh/cmudig/
-draco2) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/
-v2/gh/cmudig/draco2/HEAD) **Work in Progress** Draco is a formal framework for
-representing design knowledge about effective visualization design as a
-collection of constraints. You can use Draco to find effective visualization
-designs or validate existing ones. Draco's constraints are based on Answer Set
-Programming (ASP) and solved with the [Clingo](https://github.com/potassco/
-clingo) constraint solver. We also implemented a way to learn weights for the
-recommendation system directly from the results of graphical perception
-experiment. Draco v2 is a much improved version of the first iteration of
-[Draco](https://github.com/uwdata/draco). ## Documentation Read about Draco in
-the online book at [https://dig.cmu.edu/draco2/](https://dig.cmu.edu/draco2/
-) or launch it in interactive mode using [Binder](https://mybinder.org/v2/gh/
-cmudig/draco2/HEAD). In the documentation, we just refer to _Draco_ without a
-version. ## What's different from [Draco v1](https://github.com/uwdata/draco)?
-- Draco v2 is completely written in Python. No more need to run both Python and
-Node. We still use ASP for the knowledge base. - Generalized and extended chart
-specification format. The new format is more extensible with custom properties.
-- Support for multiple views and view composition. - High test-coverage,
-documentation, and updated development tooling. ## Contributing We welcome any
-input, feedback, bug reports, and contributions. You can learn about setting up
-your development environment in [CONTRIBUTING.md](https://github.com/cmudig/
-draco2/blob/main/CONTRIBUTING.md).
+# Draco v2 [![Open in GitHub Codespaces](https://img.shields.io/badge/launch-
+Codespaces-blue)](https://github.com/codespaces/
+new?hide_repo_select=true&ref=main&repo=313704611&machine=standardLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
+[![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/
+draco/) [![npm](https://img.shields.io/npm/v/draco-pyodide)](https://
+www.npmjs.com/package/draco-pyodide) [![Test](https://github.com/cmudig/draco2/
+actions/workflows/test.yml/badge.svg)](https://github.com/cmudig/draco2/
+actions/workflows/test.yml) [![code style black](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
+(https://codecov.io/gh/cmudig/draco2/branch/main/graph/badge.svg)](https://
+codecov.io/gh/cmudig/draco2) [![Jupyter Book Badge](https://
+raw.githubusercontent.com/executablebooks/jupyter-book/master/docs/images/
+badge.svg)](https://dig.cmu.edu/draco2) [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/cmudig/draco2/HEAD) [![Lite](https:
+//gist.githubusercontent.com/willeppy/35cdc20a3fc26e393ce76f1df35bcdfc/raw/
+a7fca1d0a2d62c2b49f60c0217dffbd0fe404471/lite-badge-launch-small.svg)](https://
+dig.cmu.edu/draco2/jupyterlite) [![Pyodide Console](https://img.shields.io/
+badge/ð%20launch-Pyodide%20Console-yellowgreen)](https://dig.cmu.edu/draco2/
+jupyterlite/static/pyodide/console.html) **Work in Progress** Draco is a formal
+framework for representing design knowledge about effective visualization
+design as a collection of constraints. You can use Draco to find effective
+visualization designs or validate existing ones. Draco's constraints are based
+on Answer Set Programming (ASP) and solved with the [Clingo](https://
+github.com/potassco/clingo) constraint solver. We also implemented a way to
+learn weights for the recommendation system directly from the results of
+graphical perception experiment. Draco v2 is a much improved version of the
+first iteration of [Draco](https://github.com/uwdata/draco). ## Documentation
+Read about Draco in the online book at [https://dig.cmu.edu/draco2/](https://
+dig.cmu.edu/draco2/) or launch it in interactive mode using [Binder](https://
+mybinder.org/v2/gh/cmudig/draco2/HEAD). In the documentation, we just refer to
+_Draco_ without a version. ## What's different from [Draco v1](https://
+github.com/uwdata/draco)? - Draco v2 is completely written in Python. No more
+need to run both Python and Node. We still use ASP for the knowledge base. -
+Generalized and extended chart specification format. The new format is more
+extensible with custom properties. - Support for multiple views and view
+composition. - High test-coverage, documentation, and updated development
+tooling. ## Contributing We welcome any input, feedback, bug reports, and
+contributions. You can learn about setting up your development environment in
+[CONTRIBUTING.md](https://github.com/cmudig/draco2/blob/main/CONTRIBUTING.md).
```

