# Comparing `tmp/jurebes-0.1.1a2-py3-none-any.whl.zip` & `tmp/jurebes-0.1.1a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5059 bytes, number of entries: 7
--rw-r--r--  2.0 unx    14926 b- defN 23-Apr-24 21:08 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 21:08 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 21:08 jurebes-0.1.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 21:08 jurebes-0.1.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 21:08 jurebes-0.1.1a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 21:08 jurebes-0.1.1a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 21:08 jurebes-0.1.1a2.dist-info/RECORD
-7 files, 16500 bytes uncompressed, 4091 bytes compressed:  75.2%
+Zip file size: 5339 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    15743 b- defN 23-Apr-24 21:37 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 21:37 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 21:37 jurebes-0.1.1a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 21:37 jurebes-0.1.1a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 21:37 jurebes-0.1.1a3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 21:37 jurebes-0.1.1a3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 21:37 jurebes-0.1.1a3.dist-info/RECORD
+7 files, 17317 bytes uncompressed, 4371 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.1a2.dist-info/METADATA
+Filename: jurebes-0.1.1a3.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.1a2.dist-info/WHEEL
+Filename: jurebes-0.1.1a3.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.1a2.dist-info/top_level.txt
+Filename: jurebes-0.1.1a3.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.1a2.dist-info/zip-safe
+Filename: jurebes-0.1.1a3.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.1a2.dist-info/RECORD
+Filename: jurebes-0.1.1a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -184,14 +184,17 @@
 
         exact_intents = {}
 
         for exact_intent in self.padacioso.calc_intents(query):
             if exact_intent["name"]:
                 if exact_intent["name"] in excluded_intents:
                     continue
+                # inject regex extracted entities
+                if self.padacioso.fuzz or exact_intent["conf"] >= 0.8:
+                    ents.update(exact_intent["entities"])
                 exact_intents[exact_intent["name"]] = IntentMatch(confidence=exact_intent["conf"],
                                                                   intent_name=exact_intent["name"],
                                                                   entities=exact_intent["entities"])
 
         probs = self.classifier.clf.predict_proba([query])[0]
         classes = self.classifier.clf.classes_
         ents = {k: v for k, v in ents.items() if k not in self.detached_entities}
@@ -200,17 +203,33 @@
             if intent in excluded_intents:
                 continue
             if intent in self.available_contexts:
                 for context, val in self.available_contexts[intent].items():
                     if val is not None:
                         ents[context] = val
 
-            if intent in exact_intents and self.padacioso.fuzz:
-                ents.update(exact_intents[intent].entities)
-                ents = {k: v for k, v in ents.items() if k not in self.detached_entities}
+            if intent in exact_intents:
+                # padacioso has a fake score, not a probability
+                # usually returns 1.0 for exact matches
+                # there is some variance between 0.75 and 0.95 with non-exact matches
+                conf2 = exact_intents[intent].confidence
+                ents2 = exact_intents[intent].entities
+
+                # let's increase the base prediction probability
+                # since we got 2 matches for same intent with different engines
+                if conf2 == 1.0:
+                    # sample likely in training set
+                    bonus = 1.0
+                    # regex capture group match!
+                    if ents2:
+                        bonus = prob * 0.7
+                else:
+                    bonus = conf2 * 0.5
+
+                prob = min(1.0, prob + bonus)
 
             exact_intents = {n: i for n, i in exact_intents.items()
                              if i.intent_name != intent}
 
             yield IntentMatch(confidence=prob,
                               intent_name=intent,
                               entities=ents)
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 1
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.1a2.dist-info/METADATA` & `jurebes-0.1.1a3.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

