# Comparing `tmp/mcc_api-1.0.3.tar.gz` & `tmp/mcc_api-1.0.4.tar.gz`

## Comparing `mcc_api-1.0.3.tar` & `mcc_api-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.3/docs/conf.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.3/docs/index.rst
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/exceptions.py
--rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/responses.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/run_tests.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_event.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_halloffame.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_participants.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_rundown.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_halloffame_game.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_participants_team.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.3/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.3/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.4/docs/conf.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.4/docs/index.rst
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/exceptions.py
+-rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.4/mcc_api/responses.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/run_tests.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_event.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_halloffame.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_participants.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_halloffame_game.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_participants_team.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/400_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.4/tests/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.4/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.4/PKG-INFO
```

### Comparing `mcc_api-1.0.3/.github/workflows/docs.yml` & `mcc_api-1.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/.github/workflows/pypi_publish.yml` & `mcc_api-1.0.4/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/.github/workflows/tests.yml` & `mcc_api-1.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/docs/index.rst` & `mcc_api-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/mcc_api/__init__.py` & `mcc_api-1.0.4/mcc_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "get_rundown",
     "get_participants",
 
     "enums",
     "exceptions",
     "responses"
 ]
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 __base_url: t.Final[str] = "https://api.mcchampionship.com/v1"
 __user_agent: t.Final[str] = f"python_mcc_api/{__version__} (https://github.com/JamesMCo/python_mcc_api)"
 
 
 @ratelimit.sleep_and_retry
 @ratelimit.limits(calls=40, period=60)
@@ -72,15 +72,15 @@
 
     .. warning::
        The /halloffame endpoint is deprecated and will be removed in a future release of the API.
        See https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.0
     """
     warnings.warn("The /halloffame endpoint is deprecated and will be removed in a future release of the API. "
                   "See https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.0",
-                  DeprecationWarning)
+                  DeprecationWarning, stacklevel=2)
     if game:
         return HallOfFameGameResponse(__request(f"halloffame/{game}"))
     else:
         return HallOfFameResponse(__request("halloffame"))
 
 
 def get_rundown(event: t.Optional[str] = None) -> RundownResponse:
```

### Comparing `mcc_api-1.0.3/mcc_api/enums.py` & `mcc_api-1.0.4/mcc_api/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/mcc_api/exceptions.py` & `mcc_api-1.0.4/mcc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/mcc_api/responses.py` & `mcc_api-1.0.4/mcc_api/responses.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/run_tests.py` & `mcc_api-1.0.4/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/test_event.py` & `mcc_api-1.0.4/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/test_halloffame.py` & `mcc_api-1.0.4/tests/test_halloffame.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/test_participants.py` & `mcc_api-1.0.4/tests/test_participants.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/test_rundown.py` & `mcc_api-1.0.4/tests/test_rundown.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/mock_data/200_halloffame.json` & `mcc_api-1.0.4/tests/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/mock_data/200_participants.json` & `mcc_api-1.0.4/tests/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/mock_data/200_participants_team.json` & `mcc_api-1.0.4/tests/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/tests/mock_data/200_rundown.json` & `mcc_api-1.0.4/tests/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/.gitignore` & `mcc_api-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/LICENSE` & `mcc_api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/README.md` & `mcc_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/pyproject.toml` & `mcc_api-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.3/PKG-INFO` & `mcc_api-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcc-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

