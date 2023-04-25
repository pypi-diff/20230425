# Comparing `tmp/pawpaw-1.0.0a9.tar.gz` & `tmp/pawpaw-1.0.0rc1.tar.gz`

## Comparing `pawpaw-1.0.0a9.tar` & `pawpaw-1.0.0rc1.tar`

### file list

```diff
@@ -1,114 +1,117 @@
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/CONTRIBUTING.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/SECURITY.md
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tinker.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tmp.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/modules.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/pawpaw.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/vcs.xml
--rw-r--r--   0        0        0    36360 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/0. Introduction.md
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/1. Segment and Span.md
--rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/2. In Text Object.md
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/3. Visualization.md
--rw-r--r--   0        0        0    19023 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/4. Arborform.md
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/5. Traversal & Query.md
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/6. Xml.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/7. NLP.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/8. Serialization.md
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/Pawpaw Cookbook.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/Using Pawpaw with nltk.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/description.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/input.txt
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/parser_compact.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/parser_verbose.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/solution.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/gettysburg_address/gettysburg_address.txt
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.py
--rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.txt
--rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/images/pawpaw.png
--rw-r--r--   0        0        0   160416 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/images/pawpaw2.png
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_furcation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_predicated_value.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_type_magic.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_version.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/errors.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/infix.py
--rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/ito.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/span.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/util.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/__init__.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/desc.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/extract.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/filter.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/itorator.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/reflect.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/split.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/value_func.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/postorator.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/stacked_reduce.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/windowed_join.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/nlp/__init__.py
--rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/nlp/nlp.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/query/__init__.py
--rw-r--r--   0        0        0    27492 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/query/_query.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/__init__.py
--rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/ascii_box.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/highlighter.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/pepo/__init__.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/pepo/pepo.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/__init__.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/sgr.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/palettes/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/palettes/palettes.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/descriptors.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/xml_helper.py
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/xml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/__init__.py
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_child_itos.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_furcation.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_invoke_func.py
--rw-r--r--   0        0        0    19841 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito.py
--rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_ctor.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_regex_equivalence_methods.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_serialization.py
--rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_str_equivalence_methods.py
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_desc.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_extract.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_filter.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_reflect.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_split.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_value_func.py
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_nlp.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_postorator.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_postorator_windowed_join.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_predicated_value.py
--rw-r--r--   0        0        0    40963 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_query_and_traversal.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_sgr.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_span.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_type_magic.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_util.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_visualization_ascii_box.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_xml_helper.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_xml_parser.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/util.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/LICENSE
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/README.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pyproject.toml
--rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/PKG-INFO
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/SECURITY.md
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tinker.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/.gitignore
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/modules.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/pawpaw.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/vcs.xml
+-rw-r--r--   0        0        0    37396 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/0. Introduction.md
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/1. Segment and Span.md
+-rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/2. In Text Object.md
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/3. Visualization.md
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/4. Arborform.md
+-rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/5. Traversal & Query.md
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/6. Xml.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/7. NLP.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/8. Serialization.md
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/Pawpaw Cookbook.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/Using Pawpaw with nltk.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/Q&A/description.md
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/Q&A/solution.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/description.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/input.txt
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/parser_compact.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/parser_verbose.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/solution.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/gettysburg_address/gettysburg_address.txt
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/description.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.py
+-rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.txt
+-rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/images/pawpaw.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/__init__.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/_type_magic.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/_version.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/errors.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/infix.py
+-rw-r--r--   0        0        0    53884 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/ito.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/span.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/util.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/desc.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/extract.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/filter.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/itorator.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/reflect.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/split.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/value_func.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/postorator.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/stacked_reduce.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/windowed_join.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/__init__.py
+-rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/nlp.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/table.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/query/__init__.py
+-rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/query/_query.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/__init__.py
+-rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/ascii_box.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/highlighter.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/pepo/__init__.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/pepo/pepo.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/__init__.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/sgr.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/palettes/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/palettes/palettes.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/descriptors.py
+-rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/xml_helper.py
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/xml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_child_itos.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_invoke_func.py
+-rw-r--r--   0        0        0    20727 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito.py
+-rw-r--r--   0        0        0    20370 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_ctor.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_descend.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_regex_equivalence_methods.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_serialization.py
+-rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_str_equivalence_methods.py
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_nlp.py
+-rw-r--r--   0        0        0    41635 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_query_and_traversal.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_span.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_type_magic.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_util.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_version.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_xml_helper.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_xml_parser.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/util.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/__init__.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_connectors.py
+-rw-r--r--   0        0        0    14065 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_desc.py
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_extract.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_filter.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_reflect.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_split.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_value_func.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_postorator.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_postorator_windowed_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/test_sgr.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/test_visualization_ascii_box.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/PKG-INFO
```

### Comparing `pawpaw-1.0.0a9/CODE_OF_CONDUCT.md` & `pawpaw-1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/CONTRIBUTING.md` & `pawpaw-1.0.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/SECURITY.md` & `pawpaw-1.0.0rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tinker.py` & `pawpaw-1.0.0rc1/tinker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 import sys
+
 # Force Python XML parser, not faster C accelerators because we can't hook the C implementation (3.x hack)
 sys.modules['_elementtree'] = None
 import xml.etree.ElementTree as ET
 from dataclasses import dataclass, field
 import typing
 
 import regex
 import pawpaw
 from pawpaw import Ito
 from pawpaw.visualization import sgr, Highlighter, pepo
 
+from pawpaw import Ito, arborform, visualization
 
+s = 'Hello, world!'
+i = Ito(s)
+itor_reflect = arborform.Reflect()  # Reflects current ito (no transformation)
+vis_compact = visualization.pepo.Compact()
+for result in itor_reflect(i):
+    print(vis_compact.dumps(result))
+
+itor_desc = arborform.Desc(lambda ito: 'Changed')  # Changes descriptor
+con = arborform.Connectors.Delegate(itor_desc)
+itor_reflect.connections.append(con)
+for result in itor_reflect(i):
+    print(vis_compact.dumps(result))
 
-
-
+exit(0)
 
 itor_funcs: typing.List[typing.Callable[[Ito], bool]]
 
-
-
 v_compact = pepo.Compact()
 v_tree = pepo.Tree()
 v_xml = pepo.Xml()
 v_json = pepo.Json()
 
-
-
 import xml.etree.ElementTree as ET
 from pawpaw import xml
+
 text = \
-"""<?xml version="1.0"?>
-<music xmlns:mb="http://musicbrainz.org/ns/mmd-1.0#" xmlns="http://mymusic.org/xml/">
-    <?display table-view?>
-    <album genre="R&amp;B" mb:id="123-456-789-0">
-        Robson Jorge &amp; Lincoln Olivetti <!-- 1982, Vinyl -->
-    </album>
-</music>"""
+    """<?xml version="1.0"?>
+    <music xmlns:mb="http://musicbrainz.org/ns/mmd-1.0#" xmlns="http://mymusic.org/xml/">
+        <?display table-view?>
+        <album genre="R&amp;B" mb:id="123-456-789-0">
+            Robson Jorge &amp; Lincoln Olivetti <!-- 1982, Vinyl -->
+        </album>
+    </music>"""
 root = ET.fromstring(text, parser=xml.XmlParser())
 
 highlighter = Highlighter(sgr.palettes.PAWPAW)
 highlighter.print(root.ito)
 exit(0)
 
 print(pepo.Tree().dumps(root.ito))
 exit(0)
 
-
-
 import pawpaw.visualization.ascii_box as box
 
 # Box tests:
 
 c = '─'
 bdc = box.BoxDrawingChar.from_char(c)
 boxer = box.from_sides(bdc)
@@ -147,15 +155,14 @@
 
 boxer = box.from_corners(box.BoxDrawingChar.from_char('╬'), box.BoxDrawingChar.from_char('╯'))
 for line in boxer.from_srcs('Hello, world!'):
     print(line)
 
 print()
 
-
 exit(0)
 
 # Test 1 = get from_char
 c = '─'
 bdc = box.BoxDrawingChar.from_char(c)
 print(bdc)
 
@@ -243,23 +250,19 @@
 word_itor = pawpaw.arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.word_tokenize(str(ito))))
 sent_itor.itor_children = word_itor
 
 i.children.add(*(sent_itor(i)))
 print(v_tree.dumps(i))
 exit(0)
 
-
 ws_tok = nltk.tokenize.WhitespaceTokenizer()
 splitter = pawpaw.arborform.Split(regex.compile(ws_tok._pattern, ws_tok._flags))
 i = pawpaw.Ito('The quick brown fox.')
 [str(i) for i in splitter(i)]
 
-
-
-
 # # VERSION
 #
 # print(pawpaw.__version__)
 # print(pawpaw.__version__.major)
 # print(pawpaw.__version__.pre_release)
 # print(pawpaw.__version__._asdict())
 # exit(0)
@@ -290,44 +293,42 @@
 wrds_nums.itor_children = chrs_digs
 
 root.children.add(*phrases(root))
 
 print(dump.Compact().dumps(root))
 exit(0)
 
-    
-# SGR    
+# SGR
 
 for effect in sgr.Intensity, sgr.Italic, sgr.Underline, sgr.Blink, sgr.Invert, sgr.Conceal, sgr.Strike, sgr.Font, sgr.Fore, sgr.Back:
     print(f'{effect.__name__.upper()}')
-    
+
     if effect in (sgr.Fore, sgr.Back):
         attrs = {nc.name: effect(nc) for nc in sgr.Colors.Named}
     else:
         names = filter(lambda n: n.isupper() and not n.startswith('_') and not n.startswith('RESET'), dir(effect))
         attrs = {name: getattr(effect, name) for name in names}
-        
+
     for name, attr in attrs.items():
         print(f'\t{name}: Before Sgr... {attr}Sgr applied!{effect.RESET} Sgr turned off.')
-    
+
     print()
 
 from random import randint
 
 for line in range(1, 50):
     for color in sgr.Fore, sgr.Back:
         for col in range(1, 120):
             rgb = sgr.Colors.Rgb(randint(0, 255), randint(0, 255), randint(0, 255))
             print(effect(rgb), end='')
             print(chr(ord('A') + randint(0, 25)) + effect.RESET, end='')
         print()
 
 exit()
 
-
 # HIGHLIGHTER
 
 s = 'The quick brown fox'
 ito = pawpaw.Ito(s)
 ito.children.add(*ito.split(regex.compile('\s+')))
 
 highlighter = Highlighter(
```

### Comparing `pawpaw-1.0.0a9/tmp.py` & `pawpaw-1.0.0rc1/docs/demos/Q&A/solution.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import regex
-from pawpaw import Ito, arborform
+from pawpaw import Ito, arborform, visualization
 
 # INPUT
 text = """\na\n\nQ So I do first want to bring up exhibit No. 46, which is in the binder 
 in front of\nyou.\n\nAnd that is a letter [to] Alston\n& Bird...
 \n\nIs that correct?\n\nA This is correct.\n\nQ Okay."""
 
 # BUILD PARSER
 itor_split = arborform.Split(regex.compile(r'\n+(?=Q_? )', regex.DOTALL), desc='Q/A tuple')
 
 itor_filt = arborform.Filter(lambda i: i.str_startswith('Q'))  # toss "random text" stuff
-itor_split.itor_next = itor_filt
+con = arborform.Connectors.Delegate(itor_filt)
+itor_split.connections.append(con)
 
-itor_qa_split = arborform.Split(regex.compile(r'\n+(?=A_? )', regex.DOTALL))
-itor_filt.itor_children = itor_qa_split
+# Assumes only one answer per question
+itor_qa_split = arborform.Split(regex.compile(r'\n+(?=A_? )', regex.DOTALL), limit=1)
+con = arborform.Connectors.Children.Add(itor_qa_split)
+itor_filt.connections.append(con)
 
 itor_extract = arborform.Extract(
     regex.compile(r'([QA])_? (?<QorA>.+)', regex.DOTALL),
     desc_func=lambda ito, match, group: match.group(1))
-itor_qa_split.itor_next = itor_extract
+con = arborform.Connectors.Children.Add(itor_extract)
+itor_qa_split.connections.append(con)
 
-# from pawpaw import visualization
-# root = Ito(text)
-# root.children.add(*itor_split(root))
-# print(visualization.pepo.Tree().dumps(root))
-# exit(0)
+# OUTPUT TREE
+root = Ito(text)
+tree_vis = visualization.pepo.Tree()
+for i in itor_split(root):
+    print(tree_vis.dumps(i))
+print()
 
-# OUTPUT
-for i, tup in enumerate(itor_split(Ito(text))):
+# OUTPUT TUPLE
+for i, tup in enumerate(itor_split(root)):
     print(f'{tup:%desc} {i:,}:')
     for qa in tup.children:
         print(f'\t{qa:%desc% : %substr!r}')
     print()
-
-op = """
-Q/A tuple 0:
-    Q: 'So I do first want to bring up exhibit No. 46, which is in the binder \nin front of\nyou.\n\nAnd that is a letter [to] Alston\n& Bird...\n\n\nIs that correct?'
-    A: 'This is correct.'
-
-Q/A tuple 1: 
-    Q: 'Okay.'
-"""
```

### Comparing `pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md` & `pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md` & `pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/.idea/workspace.xml` & `pawpaw-1.0.0rc1/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `pawpaw-1.0.0a9/.idea/workspace.xml` & `pawpaw-1.0.0rc1/.idea/workspace.xml`

```diff
@@ -1,9 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
+  <component name="AutoImportSettings">
+    <option name="autoReloadType" value="SELECTIVE"/>
+  </component>
   <component name="ChangeListManager">
     <list default="true" id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -14,53 +17,49 @@
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
     <option name="UPDATE_TYPE" value="REBASE"/>
   </component>
-  <component name="GithubProjectSettings">
-    <option name="branchProtectionPatterns">
-      <list>
-        <option value="master"/>
-      </list>
-    </option>
-  </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2HYqL0C1amxRmfYJALzRD6Il7pD"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
     &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;ignore.virus.scanning.warn.message&quot;: &quot;true&quot;,
     &quot;last_opened_file_path&quot;: &quot;C:/Users/rlaye/Documents/PycharmProjects/pawpaw/pawpaw/arborform/itorator&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;Console&quot;
+    &quot;settings.editor.selected.configurable&quot;: &quot;project.propVCSSupport.CommitDialog&quot;
   },
   &quot;keyToStringList&quot;: {
     &quot;com.intellij.ide.scratch.ScratchImplUtil$2/New Scratch File&quot;: [
       &quot;TEXT&quot;
     ]
   }
 }</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
+      <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\arborform"/>
+      <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\visualization"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
   </component>
   <component name="RunManager" selected="Python tests. All Unittests">
-    <configuration name="solution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="solution (1)" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
@@ -73,104 +72,118 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
+    <configuration name="solution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
-      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/Q&amp;A"/>
+      <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/Q&amp;A/solution.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name=" All Unittests" type="tests" factoryName="Unittests">
+    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
       <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
-      <option name="WORKING_DIRECTORY" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="_new_pattern" value="&quot;&quot;"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_itorator_extract.TestExtract.test_desc_func" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="us_constitution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/us_constitution"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_itorator_extract.TestExtract.test_desc_func&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_itorator_extract.TestExtract.test_group_filter_default" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name=" All Unittests" type="tests" factoryName="Unittests">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
-      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
+      <option name="WORKING_DIRECTORY" value=""/>
+      <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <option name="_new_pattern" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_itorator_extract.TestExtract.test_group_filter_default&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
+      <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_itorator_filter.TestFilter.test_traverse_partial" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests in test_child_itos.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_itorator_filter.TestFilter.test_traverse_partial&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_child_itos.py&quot;"/>
+      <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_itorator_split.TestSplit.test_limit" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests in test_nlp.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_itorator_split.TestSplit.test_limit&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_nlp.py&quot;"/>
+      <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact" type="tests" factoryName="Unittests" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
@@ -183,131 +196,40 @@
       <option name="_new_target" value="&quot;test_type_magic.TestTypeMagic.test_is_callable_exact&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.tinker"/>
       <item itemvalue="Python.solution"/>
+      <item itemvalue="Python.solution (1)"/>
+      <item itemvalue="Python.us_constitution"/>
       <item itemvalue="Python tests.Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact"/>
       <item itemvalue="Python tests. All Unittests"/>
-      <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_desc_func"/>
-      <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_group_filter_default"/>
-      <item itemvalue="Python tests.Python tests for test_itorator_filter.TestFilter.test_traverse_partial"/>
-      <item itemvalue="Python tests.Python tests for test_itorator_split.TestSplit.test_limit"/>
+      <item itemvalue="Python tests.Python tests in test_nlp.py"/>
+      <item itemvalue="Python tests.Python tests in test_child_itos.py"/>
     </list>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.Python tests for test_itorator_split.TestSplit.test_limit"/>
-        <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_group_filter_default"/>
-        <item itemvalue="Python tests.Python tests for test_itorator_filter.TestFilter.test_traverse_partial"/>
-        <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_desc_func"/>
+        <item itemvalue="Python tests.Python tests in test_nlp.py"/>
+        <item itemvalue="Python.us_constitution"/>
         <item itemvalue="Python.solution"/>
+        <item itemvalue="Python.solution (1)"/>
+        <item itemvalue="Python tests.Python tests in test_child_itos.py"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
       <created>1668472305766</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1668472305766</updated>
     </task>
-    <task id="LOCAL-00020" summary="Fixes">
-      <created>1670458671852</created>
-      <option name="number" value="00020"/>
-      <option name="presentableId" value="LOCAL-00020"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670458671852</updated>
-    </task>
-    <task id="LOCAL-00021" summary="Header cleanups">
-      <created>1670459015339</created>
-      <option name="number" value="00021"/>
-      <option name="presentableId" value="LOCAL-00021"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670459015339</updated>
-    </task>
-    <task id="LOCAL-00022" summary="nlp doc trim fix">
-      <created>1670459935622</created>
-      <option name="number" value="00022"/>
-      <option name="presentableId" value="LOCAL-00022"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670459935622</updated>
-    </task>
-    <task id="LOCAL-00023" summary="nlp number fix">
-      <created>1670466456009</created>
-      <option name="number" value="00023"/>
-      <option name="presentableId" value="LOCAL-00023"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670466456009</updated>
-    </task>
-    <task id="LOCAL-00024" summary="nlp fixes">
-      <created>1670466680641</created>
-      <option name="number" value="00024"/>
-      <option name="presentableId" value="LOCAL-00024"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670466680641</updated>
-    </task>
-    <task id="LOCAL-00025" summary="xml comment handling">
-      <created>1670813446517</created>
-      <option name="number" value="00025"/>
-      <option name="presentableId" value="LOCAL-00025"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670813446517</updated>
-    </task>
-    <task id="LOCAL-00026" summary="typos">
-      <created>1670894649215</created>
-      <option name="number" value="00026"/>
-      <option name="presentableId" value="LOCAL-00026"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670894649215</updated>
-    </task>
-    <task id="LOCAL-00027" summary="Sentence improvements">
-      <created>1670978443873</created>
-      <option name="number" value="00027"/>
-      <option name="presentableId" value="LOCAL-00027"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670978443873</updated>
-    </task>
-    <task id="LOCAL-00028" summary="Whitespace PEP fixes">
-      <created>1670996921635</created>
-      <option name="number" value="00028"/>
-      <option name="presentableId" value="LOCAL-00028"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670996921635</updated>
-    </task>
-    <task id="LOCAL-00029" summary="Typos">
-      <created>1671169474955</created>
-      <option name="number" value="00029"/>
-      <option name="presentableId" value="LOCAL-00029"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671169474955</updated>
-    </task>
-    <task id="LOCAL-00030" summary="Typos and doc edits">
-      <created>1671248466018</created>
-      <option name="number" value="00030"/>
-      <option name="presentableId" value="LOCAL-00030"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671248466018</updated>
-    </task>
-    <task id="LOCAL-00031" summary="Xml Doc edits">
-      <created>1671578513768</created>
-      <option name="number" value="00031"/>
-      <option name="presentableId" value="LOCAL-00031"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671578513768</updated>
-    </task>
-    <task id="LOCAL-00032" summary="__version__ = '1.0.0.a7'">
-      <created>1671747114228</created>
-      <option name="number" value="00032"/>
-      <option name="presentableId" value="LOCAL-00032"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671747114228</updated>
-    </task>
     <task id="LOCAL-00033" summary="__version__ = '1.0.0.a7'">
       <created>1671850838352</created>
       <option name="number" value="00033"/>
       <option name="presentableId" value="LOCAL-00033"/>
       <option name="project" value="LOCAL"/>
       <updated>1671850838352</updated>
     </task>
@@ -552,66 +474,152 @@
     <task id="LOCAL-00068" summary="Typehint and PEP cleanups">
       <created>1676602967110</created>
       <option name="number" value="00068"/>
       <option name="presentableId" value="LOCAL-00068"/>
       <option name="project" value="LOCAL"/>
       <updated>1676602967110</updated>
     </task>
-    <option name="localTasksCounter" value="69"/>
+    <task id="LOCAL-00069" summary=".from_gaps ctor refactoring &amp; rewrite">
+      <created>1676934862942</created>
+      <option name="number" value="00069"/>
+      <option name="presentableId" value="LOCAL-00069"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676934862942</updated>
+    </task>
+    <task id="LOCAL-00070" summary="Tests added to expose add_hierarchical bug">
+      <created>1676945255456</created>
+      <option name="number" value="00070"/>
+      <option name="presentableId" value="LOCAL-00070"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676945255456</updated>
+    </task>
+    <task id="LOCAL-00071" summary="Arborform refactoring complete">
+      <created>1677216850640</created>
+      <option name="number" value="00071"/>
+      <option name="presentableId" value="LOCAL-00071"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1677216850640</updated>
+    </task>
+    <task id="LOCAL-00072" summary="Comment updates">
+      <created>1678422910329</created>
+      <option name="number" value="00072"/>
+      <option name="presentableId" value="LOCAL-00072"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678422910329</updated>
+    </task>
+    <task id="LOCAL-00073" summary="Comment updates">
+      <created>1678422955370</created>
+      <option name="number" value="00073"/>
+      <option name="presentableId" value="LOCAL-00073"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678422955370</updated>
+    </task>
+    <task id="LOCAL-00074" summary="Minor arborform refactoring">
+      <created>1678643018348</created>
+      <option name="number" value="00074"/>
+      <option name="presentableId" value="LOCAL-00074"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678643018348</updated>
+    </task>
+    <task id="LOCAL-00075" summary="Doc whitespace updates">
+      <created>1678671064208</created>
+      <option name="number" value="00075"/>
+      <option name="presentableId" value="LOCAL-00075"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678671064208</updated>
+    </task>
+    <task id="LOCAL-00076" summary="Doc whitespace updates">
+      <created>1678753093761</created>
+      <option name="number" value="00076"/>
+      <option name="presentableId" value="LOCAL-00076"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678753093761</updated>
+    </task>
+    <task id="LOCAL-00077" summary="Doc whitespace updates">
+      <created>1678754106682</created>
+      <option name="number" value="00077"/>
+      <option name="presentableId" value="LOCAL-00077"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678754106682</updated>
+    </task>
+    <task id="LOCAL-00078" summary="Example cleanups">
+      <created>1678839189977</created>
+      <option name="number" value="00078"/>
+      <option name="presentableId" value="LOCAL-00078"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1678839189977</updated>
+    </task>
+    <task id="LOCAL-00079" summary="Whitespace and comment spelling fixes">
+      <created>1681877711766</created>
+      <option name="number" value="00079"/>
+      <option name="presentableId" value="LOCAL-00079"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681877711766</updated>
+    </task>
+    <task id="LOCAL-00080" summary="Minor PEP cleanups">
+      <created>1681878340410</created>
+      <option name="number" value="00080"/>
+      <option name="presentableId" value="LOCAL-00080"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681878340410</updated>
+    </task>
+    <task id="LOCAL-00081" summary="Unit test count update">
+      <created>1682384148587</created>
+      <option name="number" value="00081"/>
+      <option name="presentableId" value="LOCAL-00081"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682384148587</updated>
+    </task>
+    <option name="localTasksCounter" value="82"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Documentation spelling and typo fixes"/>
-    <MESSAGE value="Ascii box from_corners redo"/>
-    <MESSAGE value="Ascii box rotation approach complete"/>
-    <MESSAGE value="Ascii box exception on un-mappable corner"/>
-    <MESSAGE value="Large refactoring to address circular TypeDef issue"/>
-    <MESSAGE value="Typehting pawpaw.Ito -&gt; Ito as appropriate; added .tag to itorator"/>
-    <MESSAGE value="Added .tag to postorator"/>
-    <MESSAGE value="type_magic cleanup &amp; tests"/>
-    <MESSAGE value="Exceeded 4k unit tests"/>
     <MESSAGE value="Whitespace"/>
     <MESSAGE value="Arborform .itor_next &amp; .itor_children now are monads (i.e., class Furcation)"/>
     <MESSAGE value="Unit test fix"/>
     <MESSAGE value="Format string typo"/>
     <MESSAGE value="Concrete Itorators all return new or clones"/>
     <MESSAGE value="Cleanup + tags"/>
     <MESSAGE value="Itorator refactor; postorator roll-back"/>
     <MESSAGE value="Itorator function decorations"/>
     <MESSAGE value="Grammer, whitespace, and table-formatting"/>
     <MESSAGE value="import directive cleanups"/>
     <MESSAGE value="typehint corrections"/>
     <MESSAGE value="import cleanups"/>
-    <MESSAGE value="Unit test count update"/>
     <MESSAGE value="Refactor typos &amp; bugfixes"/>
     <MESSAGE value="test_limit subtests expansion"/>
     <MESSAGE value="Typehint and PEP cleanups"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Typehint and PEP cleanups"/>
+    <MESSAGE value=".from_gaps ctor refactoring &amp; rewrite"/>
+    <MESSAGE value="Tests added to expose add_hierarchical bug"/>
+    <MESSAGE value="Arborform refactoring complete"/>
+    <MESSAGE value="Comment updates"/>
+    <MESSAGE value="Minor arborform refactoring"/>
+    <MESSAGE value="Doc whitespace updates"/>
+    <MESSAGE value="Example cleanups"/>
+    <MESSAGE value="Whitespace and comment spelling fixes"/>
+    <MESSAGE value="Minor PEP cleanups"/>
+    <MESSAGE value="Unit test count update"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Unit test count update"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>15</line>
           <option name="timeStamp" value="1"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tinker.py</url>
-          <line>266</line>
-          <option name="timeStamp" value="18"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_query_and_traversal.py</url>
-          <line>679</line>
+          <line>695</line>
           <option name="timeStamp" value="72"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_query_and_traversal.py</url>
-          <line>766</line>
+          <line>782</line>
           <option name="timeStamp" value="76"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>116</line>
           <option name="timeStamp" value="80"/>
         </line-breakpoint>
@@ -632,115 +640,135 @@
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito.py</url>
           <line>375</line>
           <option name="timeStamp" value="84"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tinker.py</url>
-          <line>189</line>
-          <option name="timeStamp" value="91"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/visualization/ascii_box.py</url>
           <line>1262</line>
           <option name="timeStamp" value="125"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/visualization/ascii_box.py</url>
           <line>1301</line>
           <option name="timeStamp" value="127"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
-          <line>111</line>
+          <line>109</line>
           <option name="timeStamp" value="128"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
-          <line>99</line>
+          <line>97</line>
           <option name="timeStamp" value="129"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tinker.py</url>
-          <line>34</line>
-          <option name="timeStamp" value="130"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_type_magic.py</url>
           <line>144</line>
           <option name="timeStamp" value="133"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>97</line>
           <option name="timeStamp" value="134"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
-          <line>1351</line>
+          <line>1418</line>
           <option name="timeStamp" value="137"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
-          <line>72</line>
+          <line>77</line>
           <option name="timeStamp" value="138"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
-          <line>71</line>
+          <line>76</line>
           <option name="timeStamp" value="139"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>135</line>
           <option name="timeStamp" value="144"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>217</line>
           <option name="timeStamp" value="146"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>287</line>
           <option name="timeStamp" value="147"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>294</line>
           <option name="timeStamp" value="149"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>307</line>
           <option name="timeStamp" value="150"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>305</line>
           <option name="timeStamp" value="151"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/itorator.py</url>
+          <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/itorator_old.py</url>
           <line>127</line>
           <option name="timeStamp" value="154"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator_extract.py</url>
+          <url>file://$PROJECT_DIR$/tests/arborform/test_itorator_extract.py</url>
           <line>43</line>
           <option name="timeStamp" value="155"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_itorator_extract.py</url>
+          <url>file://$PROJECT_DIR$/tests/arborform/test_itorator_extract.py</url>
           <line>42</line>
           <option name="timeStamp" value="157"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/extract.py</url>
-          <line>71</line>
+          <line>73</line>
           <option name="timeStamp" value="160"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
+          <line>181</line>
+          <option name="timeStamp" value="162"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
+          <line>196</line>
+          <option name="timeStamp" value="163"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
+          <line>177</line>
+          <option name="timeStamp" value="166"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
+          <line>696</line>
+          <option name="timeStamp" value="169"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_child_itos.py</url>
+          <line>78</line>
+          <option name="timeStamp" value="175"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/filter.py</url>
+          <line>17</line>
+          <option name="timeStamp" value="180"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
 </project>
```

### Comparing `pawpaw-1.0.0a9/docs/0. Introduction.md` & `pawpaw-1.0.0rc1/docs/0. Introduction.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/1. Segment and Span.md` & `pawpaw-1.0.0rc1/docs/1. Segment and Span.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - has immutable elements.
  
 Because they are tuples, ``Span`` objects are themselves immutable.  This ensures that immutable representation for segments within Pawpaw.
 
 Creating a ``Span`` only requires a pair of ``int`` value for ``start`` and ``stop``:
 
 ```python
+>>> from pawpaw import Span
 >>> Span(0, 3)
 Span(start=0, stop=3)
 ```
 
 As a named tuple, ``Span`` can be used as direct replacement for a tuple:
 
 ```python
```

### Comparing `pawpaw-1.0.0a9/docs/2. In Text Object.md` & `pawpaw-1.0.0rc1/docs/2. In Text Object.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/3. Visualization.md` & `pawpaw-1.0.0rc1/docs/3. Visualization.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/4. Arborform.md` & `pawpaw-1.0.0rc1/docs/4. Arborform.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,318 @@
 # Arborform
 
 ## Introduction
 
-Pawpaw supports the rapid creation of complex, pipelined text parsers via the arborform module, which consists of two class hierarchies:
+### Common Parser Development Issues
 
-* ``Itorator``[^itorator_name]: Generator-based pipelined ``Ito`` transformations 
-* ``Postorator``: Generator-based ``Ito`` sequence consolidation
+If you've previously written complex text parsers you might have noticed a pattern in how they progress.  Your initial, first-attempt parsers seem to almost write themselves.  Things are going great!  But as you continue to implement more and more rules, your code starts to become unweildy.  Small changes to one one rule result in unintended consequences elsewhere, and it becomes difficult to visualize and/or understand state at various points in the programs' flows.
 
-## Itorator
+### Pipelining
+
+Pawpaw's arborform framework makes it easier to develop large, complex parsers using a *pipeline* approach.  In a pipeline, each task is encapsulated, with results received from, and feeding into, another.  This not only simplifies task implementation, it also makes it easier to keep track of state, which helps with managing unintended side-effects.
+
+### Example
+
+For example, NLP processing typically comprises multiple smaller tasks.  A typically scneario might involve processing a segment by performing these three actions:
+
+1. Split paragraphs
+2. Split sentences
+3. Split words
+
+It might be possible to perform all of these tasks using a single regular expression.  On the other hand, NLP boundary detection tasks are non-trivial.  For reasonable precision and accuracy, a singular regular expression will quickly become too unweildy.
+
+Alternatively, each of these tasks could be performed in a pipeline:
+
+```mermaid
+flowchart LR
+  trim --> psplit["paragraph split"]
+  psplit --> wsplit["word split"]
+```
+
+Lateral...
+
+```python
+>>> from pawpaw import arborform
+>>> itor_para, itor_sent, itor_word = ...
+>>> con = aborform.Connectors.Recurse(itor_sent)
+>>> itor_para.connections.append(con))
+>>> con = aborform.Connectors.Recurse(itor_word)
+>>> itor_sent.connections.append(con))
+```
+
+Top-down... alternatively:
+
+```python
+>>> itor_para.connections.append(Connectors.Recurse(itor_sent))
+>>> itor_para.connections.append(Connectors.Recurse(itor_word))
+```
+
+### Overview
 
-The ``Itorator`` class encapsulates a single step in a parser pipeline.  Each step involves a *transformation* in which a given ``Ito`` is transformed into an ``Ito`` *sequence*.
+Pipelines are implemented in arborform using the Python generator/iterator[^python_iter_gen] idiom and achieve a reasonable mixture of performance and memory conservation.  The resulting architecture is highly flexible and scalable, and is highly flexible and scalable for your needs.  The key classes in arborform are:
 
-Note that an ``Ito`` *sequence* can have zero, one, or more itos.  Some examples of transformations you might wish to perform are:
+* ``Itorator``[^itorator_name]: Generator-based ``Ito`` transformation
+* ``Connector``: Defines connection type between itorators
+* ``Postorator``: Generator-based ``Iterable[Ito]`` consolidation
+
+## Itorator
+
+The ``Itorator`` class encapsulates a single *transformation* step in a parser pipeline, whereby a given ``Ito`` is transformed into zero, one, or more itos, represented by a ``typing.Iterable[Ito]``.  Examples of transformations you may wish to perform are:
 
 * Use ``.str_strip`` to get a shortened ito
 * Split an ito into multiple itos
 * Filter out an ito so that it doesn't show in the final output
 
-Itorators are callable objects[^callable_object], which allows you to invoke them using simple function syntax.  The return type is a generator, which you can iterate over, unpack into a container, etc.  For example:
+Itorators are callable objects[^callable_object], which allows you to invoke them using simple function syntax.  The single input parameter is an ``Ito``, and the return type is a generator, which you can iterate over, unpack into a container, etc:
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> i  # Starting ito has no .desc
 Ito('Hello, world!', 0, 13, None)
 >>> itor_desc = arborform.Desc('changed')  # Desc itorator: changes .desc property
->>> next(itor_desc(i))  # Get first item from pipeline
+>>> next(itor_desc(i))  # Invoke itorator and get first item from pipeline
 Ito('Hello, world!', 0, 13, 'changed')
 ```
-When invoked, an itorator generates a **sequence** of new itos, leaving the starting, input ito unaltered:
+
+When invoked, an itorator clones the input Ito, ensured that it is left unaltered:
 
 ```python
 >>> i  # Original remains unmodified
 Ito('Hello, world!', 0, 13, None)
 ```
 
-Transformations are performed in the ``._transform`` method, which is abstract for the base class ``Itorator``.  Several concrete itorators with implementations for ``._transform`` are available:
+Transformations are performed in the ``._transform`` method, which is abstract for the base class ``Itorator``.  The ``._transform`` method is not intended to be called directly, rather, it is available for you to override in derived classes.  Several concrete itorators with implementations for ``._transform`` are available:
 
 | Concrete Class | Description                                          |
 |:---------------|:-----------------------------------------------------|
 | ``Reflect``    | Returns an unaltered ito                             |
 | ``Filter``     | Conditionally reflects an ito                        |
 | ``Desc``       | Alters the ``.desc`` for an ito and returns it       |
 | ``ValueFunc``  | Alters the ``.value_func`` for an ito and returns it |
 | ``Split``      | Splits an ito and returns the result                 |
 | ``Extract``    | Extracts and return an ito hierarchy                 |
 
-You can implement new functionality by deriving a new class from ``Itorator`` and implementing ``._transform``.
-
-Alternatively, you can wrap arbitrary transformations using the ``Itorator.wrap`` method:
+The arborform module also supports dynamically defining ``._transform`` behavior via the ``Itorator.wrap`` method.  This method creates a *wrapped, concrete itorator* whose behavior is defined by a method parameter you pass to it: 
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> itor = arborform.Itorator.wrap(lambda ito: ito.str_split())
 >>> for r in itor(i):
 ...   print(r)
 Hello,
 world!
 ```
 
-Note that the return type for your wrapped transformation must be an ito **sequence**.  If you intend to return a single ``Ito``, be sure to wrap it in a sequence such as a ``tuple`` or ``list``.  Otherwise, because an ``Ito`` is itself a sequence of char itos, your transformation results are going to be very different than what you intended!
+Note that the return type for your wrapped transformation must be ``typing.Iterable[Ito]``.  If your intent is to return a single ``Ito``, you can:
+
+* use a single ``yield`` statement
+* return a single element long ``tuple``, ``list``, or other iterable collection 
+
+Note that if you use a ``return`` statement with a single Ito, the *ito itself* will be treated as iterable return type.  This can be useful if you need to return a series of one character long itos.
 
 ```python
->>> arborform.Itorator.wrap(lambda i: i.clone())  # warning: returns an Ito, which itself is a sequence of char itos - probably not what you intended!
->>> arborform.Itorator.wrap((lambda i: i.clone(),))  # ok: returns a tuple containing a single ito
+>>> from pawpaw import Ito
+>>> from pawpaw.arborform import Itorator
+>>> i = Itorator.wrap(lambda i: [i.clone()])  # ok: returns a list with 1 ito
+>>> [*i(Ito('abc'))]
+[Ito('abc', 0, 3, None)]
+
+>>> i = Itorator.wrap(lambda i: (i.clone(),))  # ok: returns a tuple with 1 ito
+>>> [*i(Ito('abc'))]
+[Ito('abc', 0, 3, None)]
+
+>>> i = Itorator.wrap(lambda i: i.clone())  # warning: returns an Ito...
+>>> [*i(Ito('abc'))] # ...which is also a 3-Ito sequence
+[Ito('abc', 0, 1, None), Ito('abc', 1, 2, None), Ito('abc', 2, 3, None)]
 ```
 
-Class ``Itorator`` also features a ``.tag`` property, which is a convenience field that allows you to assign arbitrary labels in order to assist in testing and development of your pipelines.
+``Itorator`` also features a ``.tag`` property, which is a convenience field that allows you to assign arbitrary labels in order to assist in the development and testing of your pipelines.
+
+Itorator chaining is implemented via the ``.connections`` property.  For more details, refer to [The Pipeline](https://github.com/rlayers/pawpaw/blob/master/docs/4.%20Arborform.md#the-pipeline) below.
 
 ### Itorator Class Diagram
 
 ```mermaid
 classDiagram
   class Itorator{
-      +itor_sub Furcation[Ito, Itorator]
-      +itor_next Furcation[Ito, Itorator]
-      +itor_children Furcation[Ito, Itorator]
+      <<Abstract>>
       +tag str | None
+      +connections list[Connector]
       +postorator Postorator | Types.F_ITOS_2_BITOS | None
-      +_transform(ito) C_IT_ITOS
+      +clone() Itorator
+      #_transform(ito)* C_IT_ITOS
       +__call__(ito) C_IT_ITOS
-      +wrap(F_ITO_2_SQ_ITOS)
+      +wrap(F_ITO_2_SQ_ITOS)$
   }
   
   Itorator <|-- Reflect
   Itorator <|-- Filter
   Itorator <|-- Desc
   Itorator <|-- ValueFunc
   Itorator <|-- Split
   Itorator <|-- Extract
 ```
 
+## Connector
+
+Data flow between Itorators is indicated through ``Connector`` objects.  
+
+A connector object consists of a single ``Itorator`` and an optional predicate[^predicate]:
+
+```mermaid
+classDiagram
+class Connector{
+  <<Abstract>>
+  +itorator Itorator
+  +predicate typing.Callable[[Ito], Bool]
+}
+```
+
+A variety of concrete connector classes are available:
+
+```mermaid
+classDiagram
+Connector <|-- Delegate
+<<Abstract>> Connector
+Connector <|-- Recurse
+Connector <|-- Subroutine
+Connector <|-- ChildrenConector
+<<Abstract>> ChildrenConector
+ChildrenConector <|-- Add
+ChildrenConector <|-- AddHierarchical
+ChildrenConector <|-- Replace
+ChildrenConector <|-- Delete
+```
+
+The behavior of each concrete type is explained in [The Pipeline](https://github.com/rlayers/pawpaw/blob/master/docs/4.%20Arborform.md#the-pipeline).
+
 ## The Pipeline
 
-``Itorator`` objects are chained together via the ``.itor_next``, ``.itor_children``, & ``.itor_sub``  properties.  For unconditional chaining, you can simply set these properties to the next itorator you wish to connect to.  More complex chaining approaches are also possible - see the [Advanced Chaining](#advanced-chaining) section below for more details.)
+To create a pipeline, wrap a target itorator in a ``Connection`` and add it to the ``.connections`` list of another:
 
-### ``itor_next``
+```python
+>>> itor_1 = arborform.Reflect()
+>>> itor_2 = arborform.Trim()
+>>> itor_1.connections.append(Connectors.Delegate(itor_2))
+```
 
-The ``.itor_next`` property is feeds an ito sequence as a *lateral* flow.  This is the most basic type of pipeline connection:
+Data will now flow unconditionally from itor_1 to ito_2:
 
 ```mermaid
 flowchart LR
-  A["A()"] -->|".iter_next"| B["B()"]
-  B -.-> C[...]
+  itor_1 --> itor_2
 ```
 
-I.e., each ``Ito`` in the sequence is passed to an ``Itorator`` which then **transforms** it via its ``._transform`` method.  For example, an ``Itorator`` that performs a word split can pass its output to another ``Itorator`` that performs a char split.  The overall output will consist of char ``Ito`` objects:
+Conditional flow can be achieving by adding a predicate to the Connector object:
+
+```python
+>>> itor_1.connections.clear()
+>>> itor_1.connections.append(Connection.Delegate(itor_2, lambda ito: len(ito) > 1)
+```
+
+Now flow moves conditionally from from itor_1 to itor_2:
+
+```mermaid
+flowchart LR
+  itor_1 --> p{"len(ito) > 1"}
+  p -->|"True"| itor_2
+  p -->|"False"| x["..."]
+```
+
+Note that a default value of a tautology[^tautology] is used if a predicate is not supplied to the connector's constructor.  In other words, ``Connector`` objects *always* have a value for their predicate.
+
+Pipelines are constructed using an itorator's ``.connections`` property, which comprises a list of ``Connector`` objects.  Each connector has an itorator, which can have its own list connectors, along with a predicate.
+
+Itorator invocation can be visualized with the following pseudo-code:
+
+```python
+clone = ito.clone()
+for cur in self._transfrom(clone):
+    for connector self.connections
+        if connection.predicate(cur):
+            <impl>
+    yield ito
+```
+
+For brevity, assume ``f = connection.itorator.__call'__``.  The behavior of <impl> is as follows:
+
+| Connector | Description | Typical Usage |
+|:---------------|:-----------------------|:-----------------------|
+| ``Connectors.Delegate`` | 1. Yields ``f(cur)``<br>2. Breaks out of inner loop | Cannonical |
+| ``Connectors.Recurse`` | 1. Invokes ``f(cur)``<br>2. for each item in cached result, yield the result of allowing it to *complete* the inner loop<br>3. Breaks out of inner loop | Connect to multiple end-points of a sub-flow |
+| ``Connectors.Subroutine`` | 1. invokes ``f(cur)``, ignoring any result<br>2. Continues inner loop with ``cur`` | perform a transformation to cur without disrupting flow |
+| ``Connectors.Children.Add`` | 1. Caches result of ``f(cur)``<br>2. Adds cached result to cur.children<br>3. Yields cached result<br>4. Breaks out of inner loop | adding children |
+| ``Connectors.Children.AddHierarchical`` |  1. Caches result of ``f(cur)``<br>2. Adds cached result hierarchically to cur.children<br>3. Yields cached result<br>4. Breaks out of inner loop | adding children  hierarchically |
+| ``Connectors.Children.Replace`` | 1. Caches result of ``f(cur)``<br>2. Clears cur.children<br>3. Adds cached result to cur.children<br>4. Yields cached result<br>5. Breaks out of inner loop | adding or replacing children |
+| ``Connectors.Children.Delete`` | 1. Caches result of ``f(cur)``<br>2. Calls ``cur.children.delete`` for each item in cached result<br>3. Yield cached result<br>4. Breaks out of inner loop | deleting children |
+
+If an itorator has a ``.postorator``, the result the entire flow is wrapped in an iterator and passed to it.
+
+### ``Connectors.Delegate``
+
+YieldBreak is the cannonical connector type in that it delegates all subsequent flow processing to another itorator and yields the results.
 
 ```python
 >>> from pawpaw import Ito, arborform, visualization
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
->>> split_reflect = arborform.Reflect()  # Reflects current ito (no transformation)
+>>> itor_reflect = arborform.Reflect()  # Reflects current ito (no transformation)
 >>> vis_compact = visualization.pepo.Compact()
->>> for result in split_words(i):
->>>   print(vis_compact.dumps(r)
-1: (0, 13) 'None' : 'Hello, world!'
->>>
+>>> for result in itor_reflect(i):
+...    print(vis_compact.dumps(result))
+1: (0, 13) None : 'Hello, world!'
+>>> 
 >>> itor_desc = arborform.Desc(lambda ito: 'Changed')  # Changes descriptor
->>> itor_reflect.itor_next = itor_desc
->>> for result in split_words(i):
->>>   print(vis_compact.dumps(r)
+>>> con = arborform.Connectors.Delegate(itor_desc)
+>>> itor_reflect.connections.append(con)
+>>> for result in itor_reflect(i):
+...    print(vis_compact.dumps(result))
 1: (0, 13) 'Changed' : 'Hello, world!'
 ```
 
-### ``itor_children``
+### ``Connectors.Recurse``
 
-The ``.itor_children`` feeds an ito sequence as a *downward flow*.  Each ``Ito`` in the sequence is passed to an ``Itorator`` whose output is then appended to the ito's children:
+The ``Recurse`` connector is useful when designing a *sub-pipeline* that has multiple end-points and whose output needs to be sent to another itorator:
 
 ```mermaid
 flowchart LR
-  A["A()"] -->|".iter_children"| B[".children.add(B())"]
-  B -.-> D[...]
+  A["A()"] -->|"Connectors.Recurse"| sub-pipeline
+  subgraph sub-pipeline
+    direction LR
+    B["B()"] --> C["C()"]
+    B --> D["D()"]
+  end
+  sub-pipeline -.-> E[...]
 ```
 
-For example, an ``Itorator`` that performs a word split can pass its output to another ``Itorator`` that performs a char split.  The overall output will consist of *trees* whose roots are words and leaves are chars:
+By using a ``Sub`` connector, the output of both C and D will be fed into the next itorator in a connections list.
+
+### ``Connectors.Subroutine``
+
+This type is also aliases as ``Sub``...
+
+TODO
+
+### ``Connectors.Children``
+
+Several connections apply results to the child of a given ito.  For example, an ``Itorator`` that performs a word split can pass its output to another ``Itorator`` that performs a char split.  The overall output will consist of *trees* whose roots are words and leaves are chars:
 
 ```python
 >>> from pawpaw import Ito, arborform, visualization
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> split_words = arborform.Itorator.wrap(lambda ito: ito.str_split())  # str split
 >>> split_chars = arborform.Itorator.wrap(lambda ito: [*ito])  # extract char itos
->>> split_words.itor_children = split_chars
->>> tree_vis = pawpaw.visualization.pepo.Tree()
+>>> con = arborform.Connectors.Children.Add(split_chars)
+>>> split_words.connections.append(con)
+>>> tree_vis = visualization.pepo.Tree()
 >>> for result in split_words(i):
 >>>   print(tree_vis.dumps(result))
 (0, 6) 'None' : 'Hello,'
 ├──(0, 1) 'None' : 'H'
 ├──(1, 2) 'None' : 'e'
 ├──(2, 3) 'None' : 'l'
 ├──(3, 4) 'None' : 'l'
@@ -162,117 +324,24 @@
 ├──(8, 9) 'None' : 'o'
 ├──(9, 10) 'None' : 'r'
 ├──(10, 11) 'None' : 'l'
 ├──(11, 12) 'None' : 'd'
 └──(12, 13) 'None' : '!'
 ```
 
-### ``itor_sub``
-
-The ``.itor_sub`` property is used to define a *sub-pipeline*.  Using sub-pipelines allows you to better encapsulate regions within a pipeline, and to provide a single connection point for subsequent processing.
-
-```mermaid
-flowchart LR
-  A["A()"] -->|".iter_sub"| sub-pipeline
-  subgraph sub-pipeline
-    direction LR
-    B["B()"] --> C["C()"]
-    B --> D["D()"]
-  end
-  sub-pipeline -.-> E[...]
-```
-
-An itorator can have values for any combination of ``.itor_sub``, ``.itor_next``, & ``.itor_children``.  If no connections are specified, then no further processing take place and the given ito sequence is yielded back to the previous pipeline segment.
-
-### Order of Evaluation
+## DOCUMENTATION BEYOND THIS POINT IS NOW DEPRECATED
 
-The order of evaluation for an ``Itorator`` is as follows:
-
-1. ``._transform`` : Ito → Sequence
-2. ``.itor_sub`` : Sequence → Sequence
-3. ``.itor_children`` : Sequence → Sequence
-4. ``.itor_next`` : Sequence → Sequence
-
-```mermaid
-stateDiagram-v2
-  direction LR
-  
-  Ito --> _transform
-  state _transform {
-    direction TB
-    [*] --> itosP
-    itosP : ito seq
-    itosP --> [*]
-  }
-  _transform --> itor_sub
-  state itor_sub {
-    direction TB
-    [*] --> itosS
-    itosS: ito seq
-    itosS --> [*]
-  }
-  itor_sub --> itor_children
-
-  state itor_children {
-    direction TB
-    [*] --> as_children
-    as_children: .children.add(ito seq)
-    as_children --> [*]
-  }
-  itor_children --> itor_next
-
-  state itor_next {
-    direction TB
-    [*] --> itosN
-    itosN: ito seq
-    itosN --> [*]
-  }
-
-  itor_next --> [*]
-```
-
-### Pipeline Branching
-
-In the examples so far, ``.itor_sub``, ``.itor_next``, & ``.itor_children`` were set to a *single* Itorator.  This results in unconditional flow to the subsequent ``Itorator``.
-
-Alternatively, you can *conditionally* flow using a predicate.  For example:
-
-```python
->>> from pawpaw import Ito, arborform
->>> s = '4 out of 5'
->>> i = Ito(s)
->>> split_lexer = arborform.Itorator.wrap(lambda ito: ito.str_split())
->>> int_value_func = arborform.ValueFunc(lambda i: int(str(i)), 'integer')
->>> non_int_val = arborform.Desc('non-int')
->>> split_lexer.itor_next = lambda ito: ito.str_isnumeric(), int_value_func  # conditional flow - if predicate():
->>> for ito in split_lexer(i):
->>>    print(f'substr: {ito:%substr!r}; .value(): {repr(ito.value())}')
-substr: '4'; .value(): 4
-substr: 'out'; .value(): 'out'
-substr: 'of'; .value(): 'of'
-substr: '5'; .value(): 5
-```
-
-The example above flows from split_lexer to int_value_func **if** a given ito is numeric:
+The ``.itor_next`` property is feeds an ito sequence as a *lateral* flow.  This is the most basic type of pipeline connection:
 
 ```mermaid
 flowchart LR
-    split_lexer --> predicate{".str_isnumeric() ?"}
-    predicate -->|True| int_value_func
-    int_value_func --> a[...]
-    predicate -->|False| b[...] 
+  A["A()"] -->|".iter_next"| B["B()"]
+  B -.-> C[...]
 ```
 
-
-## Parsing Strategy
-
-If you have written complex text parsers before, you might have noticed a pattern in these projects.  Your initial, first-attempt parsers seem to almost write themselves.  Things are going great!  But as you continue to implmeent more and more rules, your code base starts to become large and unweildy.  Small changes to one part have unintended consequences for other parts, and fixing a problem for one file often causes problems with another.
-
-A good strategy for avoiding these scenarios it to utilize a divide-and-conquer approach to your parsing approaches.  This strategy is baked into the Pawpaw architecture, whereby each pipelined ``Itorator`` encapsulates a concrete step, the status of which can be inspected and/or tested.  Successful use of this strategy means keeping your ``Itorator`` steps "small".  For example, large complex regular expressions are not only difficult to write, but equally hard to test, diagnose, and change.  Breaking apart the regular expression into more fine-grained tasks via itorator not only results in easier patterns, but also helps to de-couple the various operations in a way that reduces unintended cause and effect.
-
 ## Concrete Itorator Types
 
 ### Extract
 
 Notes:
 
 * group_filter defaults to only **named** groups, but it can be set to nothing (i.e., allow *all* groups.)  Note that if all groups are allowed, then the output will always consist of a tree whose root is the entire match (group 0), with all other sub-groups present as descendants
@@ -467,16 +536,19 @@
     +__call__(itos) C_IT_BITOS
   }
 
   Postorator <|-- stacked_reduce
   Postorator <|-- windowed_join
 ```
 
-[^itorator_name]: The name "Itorator" comes from a portmanteau of "Ito" and "Iterator"
+[^python_iter_gen]: See [generator objects](https://docs.python.org/3/c-api/gen.html) and [iterator objects](https://docs.python.org/3/c-api/iterator.html) for more information.
 
-[^callable_object]: See [object.__call__](https://docs.python.org/3/reference/datamodel.html#object.__call__) in Python docs for more detail.
+[^itorator_name]: The name "Itorator" comes from a portmanteau of "Ito" and "Iterator"
 
 [^predicate]: A function that returns a Boolean value.
 
+[^tautology]: A function that always returns True.
+
+[^callable_object]: See [object.__call__](https://docs.python.org/3/reference/datamodel.html#object.__call__) in Python docs for more detail.
+
 [^furcation_name]: A "Furcation" is the act or process of forking or branching out, e.g., bifurcation, trifurcation, etc.
 
-[^tautology]: A function that always returns True.
```

### Comparing `pawpaw-1.0.0a9/docs/5. Traversal & Query.md` & `pawpaw-1.0.0rc1/docs/5. Traversal & Query.md`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 | ``'desc'``            |            ``'d'``            | One or more ``str`` values used to match againss ``.desc`` of axis; values must be separated with commas, literal commas must be escaped | ``[d:number]``<br />``[d:word,char]`` |
 | ``'str'``          |            ``'s'``            | A ``str`` used to match against ``str()`` of axis | ``[s:foo]``<br />``[s:foo,goo]``|
 | ``'str-casefold'`` |   ``'scf'``,<br />``'lcs'``   | Checks if casefolded ``str()`` of axis matches casefolded value | ``[scf:FoO,GoO]`` |
 | ``'str-casefold-ew'`` | ``'scfew'``,<br />``'lcsew'`` | Checks if casefolded ``str()`` of axis ends with with casefolded value | ``[scfew:a,1]`` |
 | ``'str-casefold-sw'`` | ``'scfsw'``,<br />``'lcssw'`` | Checks if casefolded ``str()`` of axis starts with with casefolded value | ``[scfsw:a,1]`` |
 | ``'str-ew'`` |           ``'sew'``           | Checks if ``str()`` of axis starts with value | ``[scfew:a,1]`` |
 | ``'str-sw'`` |           ``'ssw'``           | Checks if ``str()`` of axis ends with with value | ``[scfsw:a,1]`` |
-| ``'index'`` |            ``'v'``            | One or more tuples consisting of a *start* and optional *stop* ``int`` values used to match against the enumeration index(ices) of the axis; *start* and *stop* must be separated with hyphens, tuples must be separated with commas | ``[i:1]``<br />``[i:2,3,4]``<br />``[i:2-3]``<br />``[i:2,5-7]`` |
+| ``'index'`` |            ``'v'``            | One or more ``int`` tuples consisting of a *start* and optional *stop* values; matches against the enumeration index(ices) of the axis; start and stop must be non-negative integers; start and stop behave like a *slice*, i.e., stop should be *one more than* the last desired value; tuples must be separated with commas; *start* and *stop* must be separated with hyphens; a start followed by a hypen *without* a stop will be intepreted as ≥ , e.g. ``[i:5-]`` means *index(ices) greater than or equal to 5* | ``[i:1]``<br />``[i:2,3,4]``<br />``[i:2-3]``<br />``[i:2,5-7]``<br />``[i:0,5-,3]`` |
 | ``'predicate'`` |            ``'p'``            | Key for filter function used to match against axis A ``str`` used as a key to entry in dictionary of type:     typing.Dict[str, typing.Callable[[int, Ito], bool]  The value retrieved from the ``dict`` use used as a filter against the axis | ``[p:key1]``<br />``[p:key1,key2]`` |
 | ``'value'`` |            ``'v'``            | A ``str`` used as a key to entry in dictionary of type::      typing.Dict[str, typing.Any]  The value retrieved from the ``dict`` is used to match against the ``.value()`` of the axis | ``[p:key]``<br />``[p:key1, key2]`` |
 
 Parentheses are allowed to perform logical grouping:
 
 #### Examples
```

### Comparing `pawpaw-1.0.0a9/docs/6. Xml.md` & `pawpaw-1.0.0rc1/docs/6. Xml.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/7. NLP.md` & `pawpaw-1.0.0rc1/docs/7. NLP.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/8. Serialization.md` & `pawpaw-1.0.0rc1/docs/8. Serialization.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/Pawpaw Cookbook.md` & `pawpaw-1.0.0rc1/docs/Pawpaw Cookbook.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/Using Pawpaw with nltk.md` & `pawpaw-1.0.0rc1/docs/Using Pawpaw with nltk.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/demos/class_grades/description.md` & `pawpaw-1.0.0rc1/docs/demos/class_grades/description.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## From
+
+* [stackoverflow question 47982949](https://stackoverflow.com/questions/47982949/how-to-parse-complex-text-files-using-python)
+
+* [codereview question 183668](https://codereview.stackexchange.com/questions/183668/parse-complex-text-files-using-python)
+
+## Description
+
 Given the a file containing this text:
 
 ```text
 School = Riverdale High
 Grade = 1
 Student number, Name
 0, Phoebe
@@ -63,14 +71,8 @@
                3     0                   Fred      0
                      1                 George      0
 Riverdale High 1     0                 Phoebe      3
                      1                 Rachel      7
                2     0                 Angela      6
                      1                Tristan      3
                      2                 Aurora      9
-```
-
-For more details, see:
-
-* [stackoverflow question 47982949](https://stackoverflow.com/questions/47982949/how-to-parse-complex-text-files-using-python)
-
-* [codereview question 183668](https://codereview.stackexchange.com/questions/183668/parse-complex-text-files-using-python)
+```
```

### Comparing `pawpaw-1.0.0a9/docs/demos/class_grades/input.txt` & `pawpaw-1.0.0rc1/docs/demos/class_grades/input.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/demos/class_grades/solution.py` & `pawpaw-1.0.0rc1/docs/demos/class_grades/solution.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/demos/gettysburg_address/gettysburg_address.txt` & `pawpaw-1.0.0rc1/docs/demos/gettysburg_address/gettysburg_address.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.py` & `pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 import sys
 import os.path
 
 import regex
 import pawpaw
-from pawpaw import arborform, Ito
+from pawpaw import arborform
 
 """
 DEMO: US CONSTITUTION
 
-This demo shows an exmaple of how to parse, visualize, and query the US Constitution using Pawpaw.
+This demo shows an example of how to parse, visualize, and query the US Constitution using Pawpaw.
 
 Note: The text for the constitution was taken from https://www.archives.gov/founding-docs/constitution-transcript
 """
 
 def get_parser() -> arborform.Itorator:
     # Article: could be preamble
     a_splitter = arborform.Split(
         regex.compile(r'(?<=\n+)(?=Article\.)', regex.DOTALL),
         boundary_retention=arborform.Split.BoundaryRetention.NONE,
         tag='article splitter')
 
     a_desc = arborform.Desc(
         desc=lambda ito: 'article' if ito.str_startswith('Article.') else 'preamble',
         tag='article desc')
-    a_splitter.itor_next = a_desc
+    con = arborform.Connectors.Delegate(a_desc)
+    a_splitter.connections.append(con)
+
+    con = arborform.Connectors.Children.Add(pawpaw.nlp.SimpleNlp().itor, lambda ito: ito.desc == 'preamble')
+    a_desc.connections.append(con)
 
     a_extractor = arborform.Extract(
         regex.compile(r'Article\. (?<key>[A-Z]+)\.\n(?<value>.+)', regex.DOTALL),
         tag='article extractor')
-    a_desc.itor_children = lambda ito: ito.desc == 'article', a_extractor
-    nlp = pawpaw.nlp.SimpleNlp().itor
-    a_desc.itor_children.append(nlp)
+    con = arborform.Connectors.Children.Add(a_extractor, lambda ito: ito.desc == 'article')
+    a_desc.connections.append(con)
 
     # Section: only some articles have sections
     s_splitter = arborform.Split(
         regex.compile(r'(?<=\n+)(?=Section\.)', regex.DOTALL),
         boundary_retention=arborform.Split.BoundaryRetention.LEADING,
         desc='section',
         tag='section splitter')
-    nlp.tag = 'nlp'
-    a_extractor.itor_children = lambda ito: ito.desc == 'value' and ito.str_startswith('Section.'), s_splitter
-    a_extractor.itor_children.append((lambda ito: ito.desc == 'value', nlp))
+    con = arborform.Connectors.Children.Add(s_splitter, lambda ito: ito.desc == 'value' and ito.str_startswith('Section.'))
+    a_extractor.connections.append(con)
+    con = arborform.Connectors.Children.Add(pawpaw.nlp.SimpleNlp().itor, lambda ito: ito.desc == 'value' and not ito.str_startswith('Section.'))
+    a_extractor.connections.append(con)
 
     s_extractor = arborform.Extract(regex.compile(r'Section\. (?<key>\d+)\.\n(?<value>.+)', regex.DOTALL))
-    s_splitter.itor_children = s_extractor
-
-    s_extractor.itor_children = lambda ito: ito.desc == 'value', nlp
+    con = arborform.Connectors.Children.Add(s_extractor)
+    s_splitter.connections.append(con)
+    con = arborform.Connectors.Children.Add(pawpaw.nlp.SimpleNlp().itor, lambda ito: ito.desc == 'value')
+    s_extractor.connections.append(con)
 
     return a_splitter
 
 
-# Segment
 def get_text() -> pawpaw.Ito:
     with open(os.path.join(sys.path[0], 'us_constitution.txt')) as f:
         return pawpaw.Ito(f.read(), desc='constitution')
 
+
 # Visualize
 print(f'\nVISUALIZE:\n')
 i = get_text()
 tree_vis = pawpaw.visualization.pepo.Tree()
 parser = get_parser()
 i.children.add(*parser(i))
 print(tree_vis.dumps(i))
```

### Comparing `pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.txt` & `pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/images/pawpaw.png` & `pawpaw-1.0.0rc1/images/pawpaw.png`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/_type_magic.py` & `pawpaw-1.0.0rc1/pawpaw/_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/errors.py` & `pawpaw-1.0.0rc1/pawpaw/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,12 @@
     def _build_types_str(cls, *allowed: typing.Type) -> str:
         return ' or '.join(cls._get_type_strs(*allowed))
 
     @classmethod
     def parameter_invalid_type(cls, name: str, value: typing.Any, *allowed: typing.Type) -> TypeError:
         actual = str(inspect.signature(value)) if callable(value) else repr(value)
         return TypeError(f'parameter \'{name}\' must be type {cls._build_types_str(*allowed)}, not {actual}')
+
+    @classmethod
+    def parameter_iterable_contains_invalid_type(cls, name: str, value: typing.Any, *allowed: typing.Type) -> TypeError:
+        actual = str(inspect.signature(value)) if callable(value) else repr(value)
+        return TypeError(f'parameter \'{name}\' must contain elements of type {cls._build_types_str(*allowed)}, however, it contains an element of type {actual}: {value}')
```

### Comparing `pawpaw-1.0.0a9/pawpaw/infix.py` & `pawpaw-1.0.0rc1/pawpaw/infix.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/ito.py` & `pawpaw-1.0.0rc1/pawpaw/ito.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 import bisect
 import collections.abc
 import json
 import types
 import typing
+if typing.TYPE_CHECKING:
+    from _typeshed import SupportsRichComparison
 
 import regex
 
 import pawpaw.query
 from pawpaw import Infix, Span, Errors, type_magic
 from .util import find_escapes
 
@@ -148,46 +150,101 @@
 
         for count, m in enumerate(re.finditer(s, *span), 1):
             yield cls.from_match(m, *exclude_keys, desc=desc)
             if limit is not None and count >= limit:
                 break
 
     @classmethod
-    def from_spans(cls, src: str | pawpaw.Ito, *spans: Span, desc: str | None = None) -> typing.Iterable[pawpaw.Ito]:
+    def from_spans(cls, src: str | pawpaw.Ito, spans: typing.Iterable[Span], desc: str | None = None) -> typing.Iterable[pawpaw.Ito]:
         """Generate Itos from spans
         
         Args:
             src: a str or Ito to use as the basis
-            spans: one or more spans within the basis
+            spans: one or more spans within the basis; can be unordred & overlapping
             desc: a descriptor for the generated Itos
             
         Yields:
-            Itos; stream ordering will match that of spans; if spans overlap, so will the resulting Itos
+            Itos that match spans
         """
         yield from (cls(src, *s, desc=desc) for s in spans)
-        
+
     @classmethod
-    def from_gaps(cls, src: str | pawpaw.Ito, *gaps: Span, desc: str | None = None) -> typing.Iterable[pawpaw.Ito]:
-        """Generate Itos from gaps (negative space)
-        
+    def from_gaps(
+            cls,
+            src: str | pawpaw.Ito,
+            non_gaps: typing.Iterable[Span | pawpaw.Ito],
+            return_zero_widths: bool = False,
+            desc: str | None = None
+    ) -> typing.Iterable[pawpaw.Ito]:
+        """Generate Itos based on negative space (gaps)
+
         Args:
             src: a str or Ito to use as the basis
-            gaps: one or more Spans that resulting Itos will exclude
+            non_gaps: one or more Spans (relative to src) or Itos (whose .string matches basis) to be excluded from the result; must be ordered; overlaps are fine spans within the basis; can be unordered; overlaps are fine; zero-widths are fine
+            return_zero_widths: If true, zero-width Itos will be returned for non-overlapping, adjacent non-gaps
             desc: a descriptor for the generated Itos
-            
+
         Yields:
-            Itos; stream ordering will be left to right; overlapping spans are allowed
+            Itos whose spans occupy the space between the non-gaps
         """
-        stop = 0
-        for gap in sorted(gaps):
-            if gap.start > stop:
-                yield cls(src, stop, gap.start, desc=desc)
-            stop = gap.stop
-        if stop < len(src):
-            yield cls(src, stop, desc=desc)
+        if isinstance(src, str):
+            basis = src
+            start = 0
+            end = len(src)
+            offset = 0
+        elif isinstance(src, Ito):
+            basis = src.string
+            start, end = src.span
+            offset = start
+        else:
+            raise Errors.parameter_invalid_type('src', src, str, Ito)
+
+        it_ng = iter(non_gaps)
+
+        def next_ng_span() -> Span | None:
+            try:
+                ng = next(it_ng)
+            except StopIteration:
+                return None
+
+            if isinstance(ng, Span):
+                return ng.offset(offset)
+            elif isinstance(ng, Ito):
+                if ng.string != basis:
+                    raise ValueError('parameter \'non_gaps\' contains Itos whose .string does not match src')
+                return ng.span
+            else:
+                raise Errors.parameter_iterable_contains_invalid_type('non_gaps', ng, Span, Ito)
+
+        if (last := next_ng_span()) is None:
+            if start < end:
+                yield cls(basis, start, end, desc=desc)
+            return
+
+        if start < last.start:
+            yield cls(basis, start, min(last.start, end), desc=desc)
+
+        while last.stop < end:
+            if (cur := next_ng_span()) is None:
+                break
+            elif cur.start < last.start:  # unordered
+                raise ValueError('parameter \'non_gaps\' is unordered')
+            elif cur.start < last.stop:  # overlapping
+                pass
+            elif cur.start == last.stop:  # adjacent
+                if return_zero_widths:
+                    yield cls(basis, last.stop, cur.start, desc=desc)
+            elif cur.start >= end:
+                break
+            else:  # non-adjacent
+                yield cls(basis, last.stop, cur.start, desc=desc)
+            last = cur
+
+        if last.stop < end:
+            yield cls(basis, last.stop, end, desc=desc)
 
     @classmethod
     def from_substrings(
             cls,
             src: str | Ito,
             *substrings: str,
             desc: str | None = None
@@ -599,44 +656,44 @@
             *itos: an arbitrarily ordered sequence of itos that have
                 a) identical values for .string
                 b) non-overlapping edges
             desc: a descriptor for the parent ito
 
         Returns:
             An Ito whose .span matches the min .start and max .stop of the
-            input sequence, and to whose .children clones of the input sequence
-            have been hierarchically added
+            input sequence, and whose .children consist of clones
+             of the input sequence, hierarchically added
         """
         _iter = iter(itos)
         try:
             ito = next(_iter)
         except StopIteration:
             raise ValueError(f'parameter \'{itos}\' is empty')
             
         string = ito._string
         start = ito.start
         stop = ito.stop
-        children_lists: typing.List[ChildItos] = [ito.children]
+        cached = set[Ito]([ito])
 
         while True:
             try:
                 ito = next(_iter)
             except StopIteration:
                 break
                 
             if string != ito.string:
                 raise ValueError(f'parameter \'{itos}\' have differing values for .string')
             start = min(start, ito.start)
             stop = max(stop, ito.stop)
-            children_lists.append(ito.children)
+            cached.add(ito)
             
         rv = cls(string, start, stop, desc)
         
-        for children in children_lists:
-            rv.children.add_hierarchical(*(c.clone() for c in children))
+        for ito in cached:
+            rv.children.add_hierarchical(ito.clone())
 
         return rv
 
     @classmethod
     def join(cls, *itos: pawpaw.Ito, desc: str | None = None) -> pawpaw.Ito:
         """Synthesizes a new Ito whose .span contains the supplied objects
 
@@ -683,50 +740,40 @@
             start = self.children[0].start
             stop = self.children[-1].stop
             if (start > self.start) or (stop < self.stop):
                 return self.clone(start, stop)
         
         return self
 
-    def invert_children(self) -> pawpaw.Ito:
-        """Creates a clone of the self having children in the gaps
+    def invert_children(self, desc: str | None = None) -> pawpaw.Ito:
+        """Creates a clone with children occupying the negative space of self's children
+
+        Args:
+            desc: a descriptor used for any created children
         
+        Args:
+            desc: a descriptor used for any created children
+
         Returns:
-            A clone whose children occupy the gaps of self.
+            - If .len(self) is zero: returns clone having no children.
             
-            - If len(self) is zero: the returned clone will have no no children.
+            - Else if self has no children, returns clone with a single, contiguous child
             
-            - If self has no gaps: returned clone will have no children.
+            - Else if self has contiguous children, returns childless clone.
 
-            - If self is empty: returned clone will have a single, contiguous child.
-        """            
+            - Else returns a clone with children corresponding to the non-overlapping, non-contiguous gpas in self's children.
+        """
         rv = self.clone(clone_children=False)
         
         if len(self) == 0:
             return rv
-            
-        if len(self.children) == 0:
-            rv.children.add(rv.clone())
-            return rv
-        
-        left = self.children[0]
-        if left.start > self.start:
-            rv.children.add(rv.clone(stop=left.start, clone_children=False))
-            
-        for right in self.children[1:]:
-            if left.stop < right.start:
-                rv.children.add(rv.clone(left.stop, right.start, clone_children=False))
-                
-            left = right
-            
-        if left.stop < self.stop:
-            rv.children.add(rv.clone(left.stop, self.stop, clone_children=False))
-            
+
+        rv.children.add(*self.from_gaps(rv, self.children, False, desc))
         return rv
-    
+
     def split_iter(
             self,
             re: regex.Pattern,
             max_split: int = 0,
             keep_seps: bool = False,
             desc: str | typing.Callable | None = None
     ) -> typing.Iterable[pawpaw.Ito]:
@@ -886,21 +933,27 @@
         return self._string.startswith(prefix, *norms)
 
     # endregion
 
     # region find, index, rfind, rindex
    
     def str_find(self, sub: str, start: int | None = None, end: int | None = None) -> int:
-        return self._string.find(sub, *Span.from_indices(self, start, end).offset(self.start)) - self.start
+        rv = self._string.find(sub, *Span.from_indices(self, start, end).offset(self.start))
+        if rv != -1:
+            rv -= self.start
+        return rv
 
     def str_index(self, sub: str, start: int | None = None, end: int | None = None) -> int:
         return self._string.index(sub, *Span.from_indices(self, start, end).offset(self.start)) - self.start
     
     def str_rfind(self, sub: str, start: int | None = None, end: int | None = None) -> int:
-        return self._string.rfind(sub, *Span.from_indices(self, start, end).offset(self.start)) - self.start
+        rv = self._string.rfind(sub, *Span.from_indices(self, start, end).offset(self.start))
+        if rv != -1:
+            rv -= self.start
+        return rv
 
     def str_rindex(self, sub: str, start: int | None = None, end: int | None = None) -> int:
         return self._string.rindex(sub, *Span.from_indices(self, start, end).offset(self.start)) - self.start
 
     # endregion
 
     # region 'is' predicates
@@ -1197,14 +1250,28 @@
                 yield Types.C_EITO(start, child)
 
     def walk_descendants(self, reverse: bool = False) -> Types.C_IT_EITOS:
         yield from (ito for lvl, ito in self.walk_descendants_levels(reverse=reverse))
 
     # endregion
 
+    # region descends_from & has_descendant
+
+    def descends_from(self, ancestor: Ito) -> bool:
+        cur = self
+        while cur is not None:
+            if (cur := cur._parent) is ancestor:
+                return True
+        return False
+
+    def has_descendant(self, descendant: Ito) -> bool:
+        return descendant.descends_from(self)
+
+    # endregion
+
     # region query
 
     def find_all(
             self,
             path: pawpaw.Types.C_QPATH,
             values: typing.Dict[str, typing.Any] | None = None,
             predicates: typing.Dict[str, typing.Callable[[int, pawpaw.Ito], bool]] | None = None
@@ -1356,38 +1423,47 @@
                 raise ValueError('parameter \'itos\' has overlapping element')
 
             i = ~i
             self.__ensure_between(ito, i, i)
             ito._set_parent(self.__parent)
             self.__store.insert(i, ito)
 
-    def add_hierarchical(self, *itos: pawpaw.Ito):
+    def add_hierarchical(self, *itos: pawpaw.Ito, key: typing.Callable[[Ito], SupportsRichComparison] = None):
+        '''
+            key is None: itos with duplicate spans are added sequentially as children to one another
+            key is not None: itos with duplicate spans are ordered in geneology by key
+        '''
         for ito in itos:
+            if not isinstance(ito, pawpaw.Ito):
+                raise Errors.parameter_iterable_contains_invalid_type('itos', ito, pawpaw.Ito)
+
             if ito._parent is not None:
                 raise ValueError('contained elsewhere...')
 
             if len(self.__store) == 0:
                 ito._set_parent(self.__parent)
                 self.__store.append(ito)
                 continue
 
-            # do empty span insertions here
+            while (len(ito.children) > 0):
+                child = ito.children.pop(-1)
+                self.add_hierarchical(child, key=key)
 
             i = self.__bfind_start(ito)
             if i >= 0:
                 tmp = self.__store[i]
-                if ito.stop <= tmp.stop:
-                    tmp.children.add_hierarchical(ito)
+                if ito.stop < tmp.stop:
+                    tmp.children.add_hierarchical(ito, key=key)
                     continue
             else:
                 i = ~i
                 if i > 0:
                     tmp = self.__store[i-1]
                     if ito.stop <= tmp.stop:
-                        tmp.children.add_hierarchical(ito)
+                        tmp.children.add_hierarchical(ito, key=key)
                         continue
 
                     if ito.start < tmp.stop:
                         raise ValueError('Overlaps Case A')
 
             j = self.__bfind_stop(ito)
             if j >= 0:
@@ -1402,20 +1478,36 @@
                 if j < len(self.__store):
                     tmp = self.__store[j]
                     if ito.start < tmp.start < ito.stop:
                         raise ValueError('Overlaps Case C')
 
             if i == j:
                 self.__store.insert(i, ito)
-            else:
-                tmp = self[i:j]
-                del self[i:j]
-                ito.children.add(*tmp)
-                self.__store.insert(i, ito)
                 ito._set_parent(self.__parent)
+                continue
+
+            if j - i == 1:
+                tmp = self.__store[i]
+                if ito.span == tmp.span:
+                    if key is None or key(ito) >= key(tmp):
+                        tmp.children.add_hierarchical(ito, key=key)
+                        continue
+
+            tmp = self[i:j]
+            del self[i:j]
+            ito.children.add(*tmp)
+            self.__store.insert(i, ito)
+            ito._set_parent(self.__parent)
+
+    # endregion
+
+    # region __repr__
+
+    def __repr__(self) -> str:
+        return f'{type(self).__name__}(parent={self.__parent.__repr__()}, *{self.__store.__repr__()}'    
 
     # endregion
 
 
 class Types:
     # Ito
     C_SQ_ITOS = typing.Sequence[Ito]
```

### Comparing `pawpaw-1.0.0a9/pawpaw/span.py` & `pawpaw-1.0.0rc1/pawpaw/span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/util.py` & `pawpaw-1.0.0rc1/pawpaw/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/itorator/desc.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/desc.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,10 +10,13 @@
         if isinstance(desc, str):
             self._desc_func = lambda ito: desc
         elif type_magic.functoid_isinstance(desc, Types.F_ITO_2_DESC):
             self._desc_func = desc
         else:
             raise Errors.parameter_invalid_type('desc', desc, str | Types.F_ITO_2_DESC)
 
-    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def clone(self, tag: str | None = None) -> Desc:
+        return type(self())(self._desc_func, self.tag if tag is None else tag)
+
+    def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
         ito.desc = self._desc_func(ito)
-        return ito,
+        yield ito
```

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/itorator/extract.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import typing
 import types
 
 import regex
 from pawpaw import Ito, Types, Errors, type_magic
 from pawpaw.arborform.itorator import Itorator
 
-
 class Extract(Itorator):
     def __init__(self,
                  re: regex.Pattern,
                  limit: int | None = None,
                  desc_func: Types.F_ITO_M_GK_2_DESC = lambda ito, match, group_key: str(group_key),
                  group_filter: collections.abc.Container[str] | Types.P_ITO_M_GK | None = lambda ito, m, gk: isinstance(gk, str),
                  tag: str | None = None):
@@ -23,14 +22,17 @@
         if limit is not None and not isinstance(limit, int):
             raise Errors.parameter_invalid_type('limit', limit, int)
         self.limit = limit
 
         self.desc_func = desc_func
         self.group_filter = group_filter  
 
+    def clone(self, tag: str | None = None) -> Extract:
+        return type(self())(self._re, self.limit, self.desc_func, self._group_filter, self.tag if tag is None else tag)
+
     @classmethod
     def _get_group_keys(cls, re: regex.Pattern) -> list[Types.C_GK]:
         rv = [i for i in range(0, re.groups + 1)]
         for n, i in re.groupindex.items():
             rv[i] = n
         return rv
 
@@ -64,15 +66,15 @@
             raise Errors.parameter_invalid_type(
                 'group_filter',
                 group_filter,
                 typing.Container[Types.C_GK],
                 Types.P_ITO_M_GK,
                 types.NoneType)
 
-    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
         rv: typing.List[Ito] = []
         for count, m in enumerate(ito.regex_finditer(self._re), 1):
             path_stack: typing.List[Ito] = []
             match_itos: typing.List[Ito] = []
             filtered_gks = (gk for i, gk in enumerate(self._group_keys) if self.group_filter(ito, m, i) or self.group_filter(ito, m, gk))
             span_gks = ((span, gk) for gk in filtered_gks for span in m.spans(gk))
             for span, gk in sorted(span_gks, key=lambda val: (val[0][0], -val[0][1])):
```

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/itorator/filter.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 class Filter(Itorator):
     def __init__(self, filter_: Types.P_ITO, tag: str | None = None):
         super().__init__(tag)
         if not (filter_ is None or type_magic.functoid_isinstance(filter_, Types.P_ITO)):
             raise Errors.parameter_invalid_type('filter', filter_, Types.P_ITO)
         self._filter = filter_
 
-    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def clone(self, tag: str | None = None) -> Filter:
+        return type(self())(self._filter, self.tag if tag is None else tag)
+
+    def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
         if self._filter(ito):
-            return ito,
-        else:
-            return ()
+            yield ito
```

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/itorator/split.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/split.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,15 +51,25 @@
         self.re = re
         self.limit = limit
         self.group = group
         self.boundary_retention = boundary_retention
         self.return_zero_split = return_zero_split
         self.desc = desc
 
-    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def clone(self, tag: str | None = None) -> Split:
+        return type(self())(
+            self._re,
+            self.limit,
+            self.group,
+            self.boundary_retention,
+            self.return_zero_split,
+            self.desc,
+            self.tag if tag is None else tag)
+
+    def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
         if self.limit == 0:
             return ito,
 
         rv: typing.List[Ito] = []
         
         count = 0
         prior: Span | None = None
@@ -84,24 +94,24 @@
                 else:  # TRAILING
                     start = prior.stop
                     stop = cur.stop
 
             count += 1
 
             if start != stop:
-                rv.append(ito.clone(start, stop, self.desc))
+                rv.append(ito.clone(start, stop, self.desc, False))
 
             prior = cur
 
         if prior is not None and self.boundary_retention != self.BoundaryRetention.TRAILING:
             if self.boundary_retention == self.BoundaryRetention.NONE:
                 start = prior.stop
             else:  # LEADING
                 start = prior.start
             stop = ito.stop
             if start != stop:
-                rv.append(ito.clone(start, stop, self.desc))
+                rv.append(ito.clone(start, stop, self.desc, False))
 
         if len(rv) == 0 and self.return_zero_split:
-            rv.append(ito.clone(desc=self.desc))  # TODO : Don't clone this!
+            rv.append(ito.clone(desc=self.desc, clone_children=False))
 
         return rv
```

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/postorator/postorator.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/postorator/stacked_reduce.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/stacked_reduce.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 class StackedReduce(Postorator):
     F_SQ_ITOS_2_ITO = typing.Callable[[Types.C_SQ_ITOS], Ito]
     P_SQ_ITOS_ITO = typing.Callable[[Types.C_SQ_ITOS, Ito], bool]
     
     def __init__(
             self,
             reduce_func: F_SQ_ITOS_2_ITO,
-            push_predicate: Types.P_ITO,
+            push_predicate: P_SQ_ITOS_ITO,
             pop_predicate: P_SQ_ITOS_ITO | None = None,
             tag: str | None = None
     ):
         super().__init__(tag)
         if not type_magic.functoid_isinstance(reduce_func, self.F_SQ_ITOS_2_ITO):
             raise Errors.parameter_invalid_type('reduce_func', reduce_func, self.F_SQ_ITOS_2_ITO)
         self.reduce_func = reduce_func
 
-        if not type_magic.functoid_isinstance(push_predicate, Types.P_ITO):
-            raise Errors.parameter_invalid_type('push_predicate', push_predicate, Types.P_ITO)
+        if not type_magic.functoid_isinstance(push_predicate, self.P_SQ_ITOS_ITO):
+            raise Errors.parameter_invalid_type('push_predicate', push_predicate, self.P_SQ_ITOS_ITO)
         self.push_predicate = push_predicate
 
         if pop_predicate is None or type_magic.functoid_isinstance(pop_predicate, self.P_SQ_ITOS_ITO):
             self.pop_predicate = pop_predicate
         else:
             raise Errors.parameter_invalid_type('pop_predicate', pop_predicate, self.P_SQ_ITOS_ITO, None)
 
     def _transform(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
         stack: typing.List[Ito] = []
         for ito in itos:
-            if stack:
+            if len(stack) > 0:
                 if self.pop_predicate is not None and self.pop_predicate(stack, ito):
                     yield self.reduce_func(stack)
                     stack.clear()
                 else:
                     stack.append(ito)
 
-            if not stack:
-                if self.push_predicate(ito):
+            if len(stack) == 0:
+                if self.push_predicate(stack, ito):
                     stack.append(ito)
                 else:
                     yield ito
 
-        if stack:
+        if len(stack) > 0:
             yield self.reduce_func(stack)
```

### Comparing `pawpaw-1.0.0a9/pawpaw/arborform/postorator/windowed_join.py` & `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/nlp/nlp.py` & `pawpaw-1.0.0rc1/pawpaw/nlp/nlp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import ABC, abstractmethod, abstractproperty
 import locale
 
 import regex
 import pawpaw
 from pawpaw import nuco
 
 # See https://www.unicode.org/Public/UNIDATA/NamesList.txt
@@ -73,58 +74,85 @@
 
     'HEAVY DOUBLE TURNED COMMA QUOTATION MARK ORNAMENT':    '\u275D',
     'HEAVY DOUBLE COMMA QUOTATION MARK ORNAMENT':           '\u275E',
 
     'HEAVY LOW DOUBLE COMMA QUOTATION MARK ORNAMENT':       '\u2760',
 }
 
+unicode_bullets = {
+    'BULLET':                                               '\u2022',  # •
+    'TRIANGULAR BULLET':                                    '\u2023',  # ‣
+    'HYPHEN BULLET':                                        '\u2043',  # ⁃
+    'BLACK LEFTWARDS BULLET':                               '\u204C',  # ⁌
+    'BLACK RIGHTWARDS BULLET':                              '\u204D',  # ⁍
+    'BULLET OPERATOR':                                      '\u2219',  # ∙
+    'BLACK VERY SMALL SQUARE':                              '\u2B1D',  # ⬝
+    'BLACK SMALL SQUARE aka SQUARE BULLET':                 '\u25AA',  # ▪
+    'FISHEYE aka tainome':                                  '\u25C9',  # ◉
+    'INVERSE BULLET':                                       '\u25D8',  # ◘
+    'WHITE BULLET':                                         '\u25E6',  # ◦
+    'REVERSED ROTATED FLORAL HEART BULLET':                 '\u2619',  # ☙
+}
+
+trimmable_ws = list(byte_order_controls.values())
+trimmable_ws.extend(unicode_white_space_LF_FF.values())
+trimmable_ws.extend(unicode_white_space_other.values())
+
+class NlpComponent(ABC):
+    @abstractproperty
+    @property
+    def re(self) -> regex.Pattern:
+        ...
+
+    @abstractmethod
+    def get_itor(self) -> pawpaw.arborform.Itorator:
+        ...
+
 
 class Number:
     _sign_pat = r'(?P<sign>[-+])'
     _sci_exp_e_notation_pat = r'[Ee]' + _sign_pat + r'?\d+'
     _sci_exp_x10_notation_pat = r' ?[Xx\u2715] ?10\^ ?' + _sign_pat + r'?\d+'
     _sci_exp_pat = r'(?P<exponent>' + '|'.join([_sci_exp_e_notation_pat, _sci_exp_x10_notation_pat]) + r')'
 
-    def build_integer_pat(self) -> None:
-        self._int_pat = r'(?P<integer>\d{1,3}(?:' + regex.escape(self.thousands_sep) + r'\d{3})*'
+    def build_integer_pat(self) -> str:
+        rv = r'(?P<integer>\d{1,3}(?:' + regex.escape(self.thousands_sep) + r'\d{3})*'
         if self.thousands_sep_optional:
-            self._int_pat += r'|\d+'
-        self._int_pat += r')'
+            rv += r'|\d+'
+        rv += r')'
+        return rv
 
-    def build_decimal_pat(self) -> None:
-        self._decimal_pat = r'(?P<decimal>' + regex.escape(self.decimal_point) + r'\d+)'
+    def build_decimal_pat(self) -> str:
+        return r'(?P<decimal>' + regex.escape(self.decimal_point) + r'\d+)'
 
-    def build_num_pat_re(self) -> None:
-        self.build_integer_pat()
-        self.build_decimal_pat()
-        self._num_pat = f'(?P<number>{self._sign_pat}?' \
+    def build_num_pat_re(self) -> tuple[str, regex]:
+        num_pat = f'(?P<number>{self._sign_pat}?' \
             f'(?:{self._int_pat}{self._decimal_pat}?' \
             f'|{self._decimal_pat})' \
             f'{self._sci_exp_pat}?)'
-
-        self._re = regex.compile(self._num_pat, regex.DOTALL)
+        re = regex.compile(num_pat, regex.DOTALL)
+        return num_pat, re
 
     def __init__(self, **kwargs):
         # defaults
         loc = locale.localeconv()
         self._decimal_point = loc['decimal_point']
         self._thousands_sep = loc['thousands_sep'] if loc['thousands_sep'] != '' else ','
         self._thousands_sep_optional = True
 
         # kwargs
         for k, v in kwargs.items():
             setattr(self, k, v)
 
         # build patterns & re
-        self._int_pat: str
-        self._decimal_pat: str
+        self._int_pat: str = self.build_integer_pat()
+        self._decimal_pat: str = self.build_decimal_pat()
         self._num_pat: str
         self._re: regex.Pattern
-
-        self.build_num_pat_re()
+        self._num_pat, self._re = self.build_num_pat_re()
 
     # region properties
 
     @property
     def decimal_point(self) -> str:
         return self._decimal_point
 
@@ -171,129 +199,77 @@
     def num_pat(self) -> str:
         return self._num_pat
 
     @property
     def re(self) -> regex.Pattern:
         return self._re
 
+    # endregion
+
 
-class Table:
+class KeyedPrefix:
     """
-    Style 1: md style
+    Lists, legal documents, etc.
 
-    | A | B | C |
-    |---|:-:|--:|
-    | a | b | c |
-    | d | e | f |
-
-    Style 2: Misc ASCII
-
-    +───+───+───+
-    | A | B | C |
-    +───+───+───+
-    | a | b | c |
-    | d | e | f |
-    +───+───+───+
-
-    +---+---+---+
-    | A | B | C |
-    +---+---+---+
-    | a | b | c |
-    +---+---+---+
-    | d | e | f |
-    +---+---+---+
-
-    ╔═══╦═══╦═══╗
-    ║ A ║ B ║ C ║
-    ╠═══╬═══╬═══╣
-    ║ a ║ b ║ c ║
-    ╠═══╬═══╬═══╣
-    ║ d ║ e ║ f ║
-    ╚═══╩═══╩═══╝    
-
-    Style 3a: rst  Simple
-
-    =====  =====  ======
-       Inputs     Output
-    ------------  ------
-    A      B    A or B
-    =====  =====  ======
-    False  False  False
-    True   False  True
-    False  True   True
-    True   True   True
-    =====  =====  ======
-
-    Style 3b: rst Grid
-
-    +------------+------------+-----------+
-    | Header 1   | Header 2   | Header 3  |
-    +============+============+===========+
-    | body row 1 | column 2   | column 3  |
-    +------------+------------+-----------+
-    | body row 2 | Cells may span columns.|
-    +------------+------------+-----------+
-    | body row 3 | Cells may  | - Cells   |
-    +------------+ span rows. | - contain |
-    | body row 4 |            | - blocks. |
-    +------------+------------+-----------+
-
-    Style 4: Ascii doc
-
-    [cols="e,m,^,>s",width="25%"]
-    |============================
-    |1 >s|2 |3 |4
-    ^|5 2.2+^.^|6 .3+<.>m|7
-    ^|8
-    |9 2+>|10
-    |============================
-
-    Style 5: [Unamed]
-
-    -----+-----+-----
-      A  |  B  |  C
-    -----+-----+-----      
-     aaa | bbb | ccc
-    -----+-----+-----      
+    Some ideas:
 
-    Style 6: Tabbed
+        \d.\d...\d.?    :
+        \d-\d-...\d     :
+        §{1,2}          :  Section (Silcrow) : "16 U.S.C. § 580(p)",  "§§ 13–21"
+        [A-Z]{1,2}      :
+        [MDCLXVI]+      : Latin numerals (could be case insensitive - but should all be same case)
+       
+    """
 
-    A\tB\tC
-    a\tb\tc
+    # \d+[sepchar]    : 1) 2. 3] 4:
+    __int_pat = r'(?<key>\d+)[\)\]\.\-:]'
 
+    # \d.\d...\d.?
+    # \d-\d-...\d
+    __compound_int_pat = r'(?<key>\d+(?:[\.\-]\d+)+)\.?'
 
+    _key_prefix_pat = r'(?:' + '|'.join((__compound_int_pat, __int_pat)) + r')[ \t]+'
 
 
-    """
+class Paragraph(NlpComponent):
+    _paragraph_pat = r'(?:\r?\n\L<other_ws>*){2,}'
+    _paragraph_re = regex.compile(_paragraph_pat, regex.DOTALL, other_ws=unicode_white_space_other.values())
+
+    def __init__(self, min_newlines: int = 2):
+        self._re: regex.Pattern
+        self.min_newlines = min_newlines
 
-    pass
+    @property
+    def min_newlines(self) -> int:
+        return self._min_newlines 
 
+    @min_newlines.setter
+    def min_newlines(self, val: int):
+        if isinstance(val, int):
+            self._min_newlines = val
+            pat = r'(?:\r?\n\L<other_ws>*){' + str(self._min_newlines) + ',}'
+            self._re = regex.compile(pat, regex.DOTALL, other_ws=unicode_white_space_other.values())
+        else:
+            raise pawpaw.Errors.parameter_invalid_type('val', val, int)
 
-class List:
-    """
-    quantifier patterns
-        \d+  :
-        §{1,2}  :  Section (Silcrow) : "16 U.S.C. § 580(p)",  "§§ 13–21"
-        [A-Z]{1,2}  :
-        [MDCLXVI]+  : Latin numerals (could be case insensitive - but should all be same case)
-
-    prefix patterns:
-        •  : Before quantifier
-
-    suffix patterns
-        -
-        .
-        :
-        .)
-       
-    """
+    @property
+    def re(self) -> regex.Pattern:
+        return self._re
+
+    def get_itor(self) -> pawpaw.arborform.Itorator:
+        rv = pawpaw.arborform.Split(self._re, desc='paragraph', tag='para splitter')
 
-    pass
+        ws_trimmer = pawpaw.arborform.Itorator.wrap(lambda ito: [ito.str_strip(''.join(trimmable_ws))], tag='para trimmer')
+        con = pawpaw.arborform.Connectors.Recurse(ws_trimmer)
+        rv.connections.append(con)
+
+        return rv
 
-class Sentence:
+
+class Sentence(NlpComponent):
     _prefix_chars = list(unicode_single_quote_marks.values())
     _prefix_chars.extend(unicode_double_quote_marks.values())
     _prefix_chars.extend(c for c in '([{')
 
     _terminators = [
         r'\.',      # Full stop
         r'\.{3,}',  # Ellipses; three periods
@@ -439,53 +415,45 @@
         ignores=_ignores,
     )
 
     @property
     def re(self) -> regex.Pattern:
         return self._re
 
+    def get_itor(self) -> pawpaw.arborform.Itorator:
+        return pawpaw.arborform.Split(Sentence().re, desc='sentence', tag='sentence')       
 
-class SimpleNlp:
-    _paragraph_pat = r'(?:\r?\n\L<other_ws>*){2,}'
-    _paragraph_re = regex.compile(_paragraph_pat, regex.DOTALL, other_ws=unicode_white_space_other)
-
-    _trimmable_ws = list(byte_order_controls.values())
-    _trimmable_ws.extend(unicode_white_space_LF_FF.values())
-    _trimmable_ws.extend(unicode_white_space_other.values())
 
+class SimpleNlp:
     _word_pat = r'\w(?:(?:\L<sqs>|-\s*)?\w)*'
 
-    def get_paragraph(self) -> pawpaw.arborform.Itorator:
-        rv = pawpaw.arborform.Split(self._paragraph_re, desc='paragraph', tag='para splitter')
-
-        trimmer = pawpaw.arborform.Itorator.wrap(lambda ito: [ito.str_strip(''.join(self._trimmable_ws))], tag='para trimmer')
-        rv.itor_sub.append(trimmer)
-
-        return rv
-
-    def get_sentence(self) -> pawpaw.arborform.Itorator:
+    @classmethod
+    def get_sentence(cls) -> pawpaw.arborform.Itorator:
         return pawpaw.arborform.Split(Sentence().re, desc='sentence', tag='sentence')
 
     def __init__(self, number: Number | None = None, chars: bool = False):
         super().__init__()
 
-        paragraph = self.get_paragraph()
+        paragraph = Paragraph().get_itor()
 
-        sentence = self.get_sentence()
-        paragraph.itor_children = sentence
+        sentence = Sentence().get_itor()
+        con = pawpaw.arborform.Connectors.Children.Add(sentence)
+        paragraph.connections.append(con)
 
         self._number = number |nuco| Number()
         word_num_re = regex.compile(self._number.num_pat + r'|(?P<word>' + self._word_pat + r')', regex.DOTALL, sqs=list(unicode_single_quote_marks.values()))
 
         word_number = pawpaw.arborform.Extract(word_num_re)
-        sentence.itor_children = word_number
+        con = pawpaw.arborform.Connectors.Children.Add(word_number)
+        sentence.connections.append(con)
 
         if chars:
             char = pawpaw.arborform.Extract(regex.compile(r'(?P<char>\w)', regex.DOTALL))
-            word_number.itor_children = lambda ito: char if ito.desc == 'word' else None
+            con = pawpaw.arborform.Connectors.Children.Add(char, lambda ito: ito.desc == 'word')
+            word_number.connections.append(con)
 
         self.itor = paragraph
 
     @property
     def number(self) -> Number:
         return self._number
```

### Comparing `pawpaw-1.0.0a9/pawpaw/query/_query.py` & `pawpaw-1.0.0rc1/pawpaw/query/_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -431,34 +431,47 @@
         if key in FILTER_KEYS['str-sw']:
             if not_ == '~':
                 return lambda ec, values, predicates: all(not ec.ito.str_startswith(descape(s)) for s in pawpaw.split_unescaped(value, ','))
             else:
                 return lambda ec, values, predicates: any(ec.ito.str_startswith(descape(s)) for s in pawpaw.split_unescaped(value, ','))
 
         if key in FILTER_KEYS['index']:
-            ints: typing.Set[int] = set()
+            ranges = list[tuple[int]]()
+
             for i_chunk in value.split(','):
                 try:
-                    _is = [int(i.strip()) for i in i_chunk.split('-')]
+                    vals = i_chunk.split('-')
+                    if len(vals) > 2:
+                        raise ValueError()
+
+                    vals[0] = int(vals[0])
+                    
+                    if len(vals) == 2:
+                        val2 = vals[1]
+                        if val2.isdigit():
+                            val2 = int(val2)
+                        elif val2 == '' or val2.isspace():
+                            val2 = float('inf')
+                        else:
+                            raise ValueError()
+                        vals[1] = val2
+                        vals = tuple(vals)
+
+                    else:  # len == 1
+                        vals = (vals[0], vals[0] + 1)
+
                 except ValueError:
-                    raise ValueError(f'invalid integer in \'value\'')
+                    raise ValueError(f'invalid filter index value \'{i_chunk}\'')
 
-                len_is = len(_is)
-                if len_is == 1:
-                    ints.add(_is[0])
-                elif len_is == 2:
-                    for i in range(*_is):
-                        ints.add(i)
-                else:
-                    raise ValueError('invalid index item \'value\'')
+                ranges.append(vals)
 
             if not_ == '~':
-                return lambda ec, values, predicates: ec.index not in ints
+                return lambda ec, values, predicates: not any(r[0] <= ec.index < r[1] for r in ranges)
             else:
-                return lambda ec, values, predicates: ec.index in ints
+                return lambda ec, values, predicates: any(r[0] <= ec.index < r[1] for r in ranges)
 
         if key in FILTER_KEYS['predicate']:
             keys = [descape(s) for s in pawpaw.split_unescaped(value, ',')]
             if not_ == '~':
                 return lambda ec, values, predicates: all(not p(ec) for p in [v for k, v in cls.validate_predicates(predicates).items() if k in keys])
             else:
                 return lambda ec, values, predicates: all(p(ec) for p in [v for k, v in cls.validate_predicates(predicates).items() if k in keys])
```

### Comparing `pawpaw-1.0.0a9/pawpaw/visualization/ascii_box.py` & `pawpaw-1.0.0rc1/pawpaw/visualization/ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/pawpaw/visualization/pepo/pepo.py` & `pawpaw-1.0.0rc1/pawpaw/visualization/pepo/pepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             level += 1
             for eic in (pawpaw.Types.C_EITO(i, ito) for i, ito in enumerate(ei.ito.children, start=1)):
                 self._dump(fs, eic, level)
 
     def dump(self, fs: typing.IO, *itos: pawpaw.Ito) -> None:
         for ei in (pawpaw.Types.C_EITO(i, ito) for i, ito in enumerate(itos, start=1)):
             if not isinstance(ei.ito, pawpaw.Ito):
-                raise pawpaw.Errors.parameter_invalid_type('*itos', ei.ito, pawpaw.Ito)
+                raise pawpaw.Errors.parameter_iterable_contains_invalid_type('itos', ei.ito, pawpaw.Ito)
             self._dump(fs, ei)
 
 
 class Tree(_PepoFstr):
     HORZ = ascii_box.BoxDrawingChar.from_char('─')
     VERT = ascii_box.BoxDrawingChar.from_char('│')
     TEE = ascii_box.BoxDrawingChar.from_char('├')
@@ -121,15 +121,15 @@
         fs.write(f'{level * self.indent}</ito>{self.linesep}')
 
     def dump(self, fs: typing.IO, *itos: pawpaw.Ito) -> None:
         fs.write(f'<?xml version="1.0" encoding="UTF-8" ?>{self.linesep}')
         fs.write(f'<itos>{self.linesep}')
         for ito in itos:
             if not isinstance(ito, pawpaw.Ito):
-                raise pawpaw.Errors.parameter_invalid_type('*itos', ito, pawpaw.Ito)
+                raise pawpaw.Errors.parameter_iterable_contains_invalid_type('itos', ito, pawpaw.Ito)
             self._dump(fs, pawpaw.Types.C_EITO(0, ito), 1)
         fs.write(f'<itos>{self.linesep}')
 
 
 class Json(Pepo):
     def __init__(self, indent: str = '    ', children: bool = True):
         super().__init__(indent, children)
```

### Comparing `pawpaw-1.0.0a9/pawpaw/visualization/sgr/sgr.py` & `pawpaw-1.0.0rc1/pawpaw/visualization/sgr/sgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
             232-255:  grayscale from dark to light in 24 steps
         """
         pass
 
 
 Colors = _Colors()
 
-
 C_COLOR = Colors.Named | Colors.Rgb | Colors.EightBit
 C_PALETTE = typing.Sequence[C_COLOR]
 
 
 @dataclass(frozen=True)
 class Fore(_Sgr):
     _NAMED_OFFSET: int = 30
```

### Comparing `pawpaw-1.0.0a9/pawpaw/xml/xml_helper.py` & `pawpaw-1.0.0rc1/pawpaw/xml/xml_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 
 
 class XmlErrors:
     @classmethod
     def element_lacks_ito_attr(cls, name: str, value: typing.Any) -> ValueError:
         return ValueError(f'parameter \'{name}\' missing attr \'.ito\' - did you forget to use pawpaw.xml.XmlParser?')
 
+    @classmethod
+    def ito_value_not_element(cls, name: str, value: typing.Any) -> ValueError:
+        return ValueError(f'parameter \'{name}\' has a .value() that is not instance of xml.etree.ElementTree.Element - did you forget to use pawpaw.xml.XmlParser?')
+
 
 class XmlHelper:
     @classmethod
     def get_qualified_name(cls, ito: Ito) -> QualifiedName:
         if not isinstance(ito, Ito):
             raise Errors.parameter_invalid_type('ito', ito, Ito)
         elif ito.desc not in (xml.descriptors.START_TAG, xml.descriptors.ATTRIBUTE):
@@ -128,16 +132,22 @@
         Raises:
             Errors.parameter_invalid_type
             ValueError
         """
         return {str(qn.local_part): str(val) for qn, val in cls.get_xmlns(element).items() if qn.prefix is not None}
 
     @classmethod
-    def get_default_namespace(cls, element: ET.ElementTree) -> Ito | None:
-        return next((val for qn, val in cls.get_xmlns(element).items() if qn.prefix is None), None)
+    def get_default_namespace(cls, element: ET.ElementTree) -> str | None:
+        while element is not None:
+            rv = next((val for qn, val in cls.get_xmlns(element).items() if qn.prefix is None), None)
+            if rv is not None:
+                return f'{{{rv}}}'
+            element = cls.get_parent_element(element)
+
+        return None
 
     @classmethod
     def get_element_text_if_found(cls, element: ET.Element, path: str) -> str | None:
         if not isinstance(element, ET.Element):
             raise Errors.parameter_invalid_type('element', element, ET.Element)
 
         if not isinstance(path, str):
@@ -183,20 +193,36 @@
                 yield e
 
     @classmethod
     def find_descendant_by_local_name(cls, element: ET.Element, local_name: str) -> ET.Element | None:
         return next(cls.find_all_descendants_by_local_name(element, local_name), None)
 
     @classmethod
+    def get_text_itos(cls, element: ET.ElementTree) -> typing.Iterable[Ito]:
+        yield from element.ito.find_all(f'*[d:{xml.descriptors.TEXT}]')
+
+    @classmethod
+    def get_parent_element(cls, element: ET.Element) -> ET.Element | None:
+        if not isinstance(element, ET.Element):
+            raise Errors.parameter_invalid_type('element', element, ET.Element)
+        elif not hasattr(element, 'ito'):
+            raise XmlErrors.element_lacks_ito_attr('element', element)
+
+        if (ito := element.ito.find(f'...[d:{xml.descriptors.ELEMENT}]')) is not None:
+            return ito.value()
+
+        return None
+
+    @classmethod
     def reverse_find(cls, element: ET.Element, predicate: str) -> ET.Element | None:
         """ElementTree support for XPATH is limited, and the '..' operator will
         not traverse upwards beyond the node you issued a .find or .find_all with.
         This method applies an XPATH predicate to the current node, and returns if
         it passes.  If it fails, it uses the .ito to traverse UP to the parent,
-        and repeates the process.
+        and repeats the process.
 
         Args:
             element: _description_
             predicate: _description_
 
         Raises:
             Errors.parameter_invalid_type: _description_
@@ -215,13 +241,10 @@
         if not isinstance(predicate, str):
             raise Errors.parameter_invalid_type('predicate', predicate, str)
 
         while element is not None:
             if element.find(f'.[{predicate}]') is not None:
                 return element
 
-            if (parent := element.ito.find(f'...[d:{xml.descriptors.ELEMENT}]')) is None:
-                return None
-            
-            element = parent.value()
+            element = cls.get_parent_element(element)
 
         return element
```

### Comparing `pawpaw-1.0.0a9/pawpaw/xml/xml_parser.py` & `pawpaw-1.0.0rc1/pawpaw/xml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_invoke_func.py` & `pawpaw-1.0.0rc1/tests/test_invoke_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_ito.py` & `pawpaw-1.0.0rc1/tests/test_ito.py`

 * *Files 7% similar despite different names*

```diff
@@ -413,18 +413,20 @@
 
         children = [*Ito.from_substrings(s, *s.split(), desc='children')]
         for child in children:
             child.children.add(*Ito.from_substrings(s, *str(child), desc='grandchild'))
         grandchildren = [*itertools.chain.from_iterable(ito.children for ito in children)]
 
         adopted = Ito.adopt(children, desc=adopted_desc)
-        self.assertTrue(all(adopted is not child for child in children))
+        self.assertListEqual(children, [*adopted.children])
+        adopted_ids = [id(c) for c in adopted.children]
+        self.assertTrue(all(id(child) not in adopted_ids for child in children))
         self.assertEqual(s, str(adopted))
         self.assertEqual(adopted_desc, adopted.desc)
-        self.assertListEqual(grandchildren, [*adopted.children])
+        self.assertListEqual(grandchildren, [*itertools.chain.from_iterable(ito.children for ito in adopted.children)])
         
     def test_join(self):
         s = 'the quick brown fox'
         joined_desc = 'joined'
         children = [*Ito.from_substrings(s, *s.split(), desc='children')]
 
         joined = Ito.join(*children, desc=joined_desc)
@@ -457,38 +459,55 @@
                 ito.children.clear()
 
     def test_invert_children(self):
         for s in '', 'AB', ' AB', 'A B', 'AB ', ' A B', 'A B ', ' A B ':
             parent = Ito(s)
             with self.subTest(string=s, children_added=False):
                 inverted = parent.invert_children()
-                expected = ''.join(str(c) for c in inverted.children)
-                self.assertEqual(s, expected)
+                self.assertEqual(parent, inverted)
+
+                if len(s) == 0:
+                    self.assertEqual(0, len(inverted.children))
+                else:
+                    self.assertEqual(1, len(inverted.children))
+                    self.assertEqual(inverted, inverted.children[0])
 
             parent.children.add(*parent.str_split())
             with self.subTest(string=s, children_added=True):
                 inverted = parent.invert_children()
-                clone = parent.clone(clone_children=False)
-                clone.children.add(*(c.clone() for c in parent.children))
-                clone.children.add(*(c.clone() for c in inverted.children))
-                expected = ''.join(str(c) for c in clone.children)
-                self.assertEqual(s, expected)
+                self.assertEqual(parent, inverted)
+
+                if len(s) == 0:
+                    self.assertEqual(0, len(inverted.children))
+                elif len(parent.children) == 0:
+                    self.assertEqual(1, len(inverted.children))
+                    self.assertEqual(inverted, inverted.children[0])
+                else:
+                    count_spaces = sum(1 for i in s if i == ' ')
+                    self.assertEqual(count_spaces, len(inverted.children))
+
+                    if (count_spaces) > 0:
+                        parent_child_chars = [*itertools.chain(*parent.children)]
+                        inverted_chars = [*inverted]
+                        all_chars = parent_child_chars + inverted_chars
+                        all_chars.sort(key=lambda i: i.start)
+                        self.assertEqual(s, str(Ito.join(*all_chars)))
         
     def test_split_iter_simple(self):
         basis = 'A B C D E'
         for sep in ' ', '-':
             s = sep.join(basis.split())
             for padding in '', '=':
                 s = f'{padding}{s}{padding}'
                 ito = Ito(s, len(padding), len(s) - len(padding))
                 for pattern in f'(?<={regex.escape(sep)})', regex.escape(sep), f'(?={regex.escape(sep)})':
                     re = regex.compile(pattern)
                     with self.subTest(string=s, separator=sep, pattern=pattern):
-                        gaps = [Span(*m.span(0)).offset(-ito.start) for m in re.finditer(s, ito.start, ito.stop)]
-                        expected = [*Ito.from_gaps(ito, *gaps)]
+                        non_gaps = [*ito.from_re(re, ito)]
+                        expected = [*Ito.from_gaps(ito, non_gaps)]
                         actual = [*ito.split_iter(re)]
                         self.assertListEqual(expected, actual)
                                 
     def test_split_iter_sep_not_present(self):
         basis = 'A B C D E'
         for sep in ' ', '-':
             s = sep.join(basis.split())
```

### Comparing `pawpaw-1.0.0a9/tests/test_ito_ctor.py` & `pawpaw-1.0.0rc1/tests/test_ito_ctor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import itertools
-
 import regex
 from pawpaw import Ito, Span
 from tests.util import _TestIto, IntIto, RandSpans, RandSubstrings
 
 
 class TestItoCtor(_TestIto):
     def test_ctor_invalid_src(self):
@@ -91,15 +89,15 @@
 
     def test_from_re(self):
         s = 'the quick brown fox'
 
         re = 'abc'
         with self.subTest(re='abc'):
             with self.assertRaises(TypeError):
-                actual = [*Ito.from_re(re, s)]
+                [*Ito.from_re(re, s)]
 
         re = regex.compile(r'(?<word>\w+)')
         with self.subTest(re=re, limit=None):
             expected = [*Ito.from_substrings(s, *s.split(), desc='0')]
             for e in expected:
                 e.children.add(e.clone(desc='word'))
             actual = [*Ito.from_re(re, s)]
@@ -146,77 +144,219 @@
 
     def test_from_spans_simple(self):
         s = 'abcd' * 100
         spans = [*RandSpans(Span(1, 10), Span(0, 3)).generate(s)]
         desc = 'x'
         for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
             with self.subTest(_class=cls_name):
-                for i in _class.from_spans(s, *spans, desc=desc):
+                for i in _class.from_spans(s, spans, desc=desc):
                     self.assertIsInstance(i, _class)
                     self.assertIs(s, i.string)
                     self.assertIn(i.span, spans)
                     self.assertEqual(desc, i.desc)
                     
     def test_from_spans_complex(self):
         s = 'abcd' * 100
         spans = [Span(20, 50), Span(0, 25), Span(50, 75)]  # Overlapping and unordered
         desc = 'x'
         for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
             with self.subTest(_class=cls_name):
                 expected = [_class(s, *span, desc) for span in spans]
-                actual = [*_class.from_spans(s, *spans, desc=desc)]
+                actual = [*_class.from_spans(s, spans, desc=desc)]
                 self.assertListEqual(expected, actual)
                     
     def test_from_spans_ito(self):
         s = ' abc '
         src = Ito(s, 1, -1)
         spans = [Span(1, 3), Span(0, 2)]  # Overlapping and unordered
         desc = 'x'
         for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
             with self.subTest(_class=cls_name):
                 expected = [_class(src, *span, desc) for span in spans]
-                actual = [*_class.from_spans(src, *spans, desc=desc)]
+                actual = [*_class.from_spans(src, spans, desc=desc)]
                 self.assertListEqual(expected, actual)
 
+    def test_from_gaps_src_str_1(self):
+        desc = 'non gap'
+        for s in '', 'a', ' ', 'ab', ' ab', 'a b', 'ab ', ' a b ':
+            non_gaps = list[Ito]()
+            expected = list[Ito]()
+            for i in Ito(s):
+                if i.str_isspace():
+                    expected.append(i.clone(desc=desc))
+                else:
+                    non_gaps.append(i)
+
+            for ngs in non_gaps, [ng.span for ng in non_gaps]:
+                with self.subTest(src=s, non_gaps=ngs):
+                    actual = [*Ito.from_gaps(s, ngs, desc=desc)]
+                    self.assertSequenceEqual(expected, actual)
+
+    def test_from_gaps_src_ito_1(self):
+        desc = 'non gap'
+        for s in '', 'a', ' ', 'ab', ' ab', 'a b', 'ab ', ' a b ':
+            s = f' {s} '
+            src = Ito(s, 1, -1)
+            non_gaps = list[Ito]()
+            expected = list[Ito]()
+            for i in src:
+                if i.str_isspace():
+                    expected.append(i.clone(desc=desc))
+                else:
+                    non_gaps.append(i)
+
+            for ngs in non_gaps, [ng.span.offset(-1) for ng in non_gaps]:
+                with self.subTest(src=src, non_gaps=ngs):
+                    actual = [*Ito.from_gaps(src, ngs, desc=desc)]
+                    self.assertSequenceEqual(expected, actual)
+
+    def test_from_gaps_src_str_2(self):
+        src = ' abc '
+        non_gap_starts = src.find('a'), src.find('c')
+
+        for width in 0, 1:
+            for ngt in 'Span', 'Ito':
+                if ngt == 'Span':
+                    non_gaps = [Span(s, s + width) for s in non_gap_starts]
+                elif ngt == 'Ito':
+                    non_gaps = [Ito(src, s, s + width) for s in non_gap_starts]
+                for return_zero_widths in True, False:
+                    with self.subTest(src=src, non_gap_width=width, non_gap_type=ngt, return_zero_widths=return_zero_widths):
+                        expected = list[Ito]()
+                        expected.append(Ito(src, stop=non_gaps[0].start))
+                        expected.append(Ito(src, non_gaps[0].stop, non_gaps[-1].start))
+                        expected.append(Ito(src, non_gaps[-1].stop))
+                        if not return_zero_widths:
+                            expected = [e for e in expected if len(e) > 0]
+                        actual = [*Ito.from_gaps(src, non_gaps)]
+                        self.assertListEqual(expected, actual)
+
+    def test_from_gaps_src_ito_2(self):
+        string = ' abc '
+        src = Ito(string, 1, -1)
+        non_gap_starts = src.str_find('a'), src.str_find('c')  # relative to src, not string
+
+        for width in 0, 1:
+            for ngt in 'Span', 'Ito':
+                if ngt == 'Span':
+                    non_gaps = [Span(s, s + width) for s in non_gap_starts]
+                    offset = 0
+                elif ngt == 'Ito':
+                    non_gaps = [Ito(src, s, s + width) for s in non_gap_starts]
+                    offset = -src.start
+                for return_zero_widths in True, False:
+                    with self.subTest(src=src, non_gap_width=width, non_gap_type=ngt, return_zero_widths=return_zero_widths):
+                        expected = list[Ito]()
+                        expected.append(Ito(src, non_gaps[0].stop + offset, non_gaps[-1].start + offset))
+                        expected.append(Ito(src, non_gaps[-1].stop + offset, src.stop + offset))
+                        if len(expected[-1]) == 0:
+                            expected.pop(-1)
+                        if not return_zero_widths:
+                            expected = [e for e in expected if len(e) > 0]
+                        actual = [*Ito.from_gaps(src, non_gaps)]
+                        self.assertListEqual(expected, actual)
+
+    def test_from_gaps_none(self):
+        src = 'abc'
+        desc = 'X'
+        expected = Ito(src, desc=desc)
+        actual = next(Ito.from_gaps(src, [], desc=desc), None)
+        self.assertIsNotNone(actual)
+        self.assertEqual(expected, actual)
+
+    def test_from_gaps_identity(self):
+        src = 'abc'
+        desc = 'X'
+        actual = next(Ito.from_gaps(src, [Ito(src)], desc=desc), None)
+        self.assertIsNone(actual)
+
+    def test_from_gaps_contiguous_non_gaps(self):
+        src = 'abc'
+        desc = 'X'
+        actual = next(Ito.from_gaps(src, Ito(src), desc=desc), None)
+        self.assertIsNone(actual)            
+
+    def test_from_gaps_with_zero_widths(self):
+        desc = 'non gap'
+
+        with self.subTest(non_gap_count=2, non_gap_proximity='adjacent', non_gap_extent='contained'):
+            s = ' abc '
+            root = Ito(s, 1, -1)
+            root.children.add(*root)
+            expected = [Ito(root, i, i, desc) for i in range(1, len(root))]
+            rv = [*root.from_gaps(root, root.children, return_zero_widths=True, desc=desc)]
+            self.assertEqual(len(expected), len(rv))
+            self.assertSequenceEqual(expected, rv)
+
+        with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='contained'):
+            overlapping_non_gaps = [Ito(s, *root.span), Ito(s, root.start + 1, root.stop)]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            self.assertEqual(0, len(rv))
+
+        with self.subTest(non_gap_count=3, non_gap_proximity='overlapping', non_gap_extent='contained'):
+            overlapping_non_gaps = [Ito(s, root.start + i, root.stop) for i in range(0, len(root))]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            self.assertEqual(0, len(rv))
+
+        with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='non-contained'):
+            overlapping_non_gaps = [Ito(s, 0, len(s) - 1), Ito(s, 1, len(s) + 2)]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            self.assertEqual(0, len(rv))
+
+        with self.subTest(non_gap_count=1, non_gap_proximity='N/A', non_gap_extent='non-contained', location='prior'):
+            ng_prior = [Ito(s, 0, 1)]
+            rv = [*root.from_gaps(root, ng_prior, return_zero_widths=True, desc=desc)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(root.clone(desc=desc), rv[0])
+
+        with self.subTest(non_gap_count=1, non_gap_proximity='N/A', non_gap_extent='non-contained', location='after'):
+            ng_after = [Ito(s, -1)]
+            rv = [*root.from_gaps(root, ng_after, return_zero_widths=True, desc=desc)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(root.clone(desc=desc), rv[0])
+
+        with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='non-contained'):
+            ng = ng_prior + ng_after
+            rv = [*root.from_gaps(root, ng, return_zero_widths=True, desc=desc)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(root.clone(desc=desc), rv[0])
+
     def test_from_gaps_simple(self):
         s = 'abcd' * 10
-        gaps = [*RandSpans(Span(1, 8), Span(0, 3)).generate(s)]
+        non_gaps = [*RandSpans(Span(1, 8), Span(0, 3)).generate(s)]
         desc = 'x'
         for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
             with self.subTest(_class=cls_name):
-                for i in _class.from_gaps(s, *gaps, desc=desc):
+                for i in _class.from_gaps(s, non_gaps, desc=desc):
                     self.assertIsInstance(i, _class)
                     self.assertIs(s, i.string)
-                    self.assertFalse(any(gap.start <= i.start <= i.stop <= gap.stop for gap in gaps))
+                    self.assertFalse(any(gap.start <= i.start <= i.stop <= gap.stop for gap in non_gaps))
                     self.assertEqual(desc, i.desc)
-                    
+
     def test_from_gaps_complex(self):
         s = 'abcd' * 10
-        gaps = [Span(10, 20), Span(5, 10), Span(20, 25)]  # Overlapping and unordered
+        non_gaps = [Span(10, 20), Span(5, 10), Span(20, 25)]  # Overlapping and unordered
         desc = 'x'
-        for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
-            with self.subTest(_class=cls_name):
-                expected = [
-                    _class(s, 0, min(gap.start for gap in gaps), desc),
-                    _class(s, max(gap.stop for gap in gaps), desc=desc)
-                ]
-                actual = [*_class.from_gaps(s, *gaps, desc=desc)]
-                self.assertListEqual(expected, actual)
-                    
-    def test_from_gaps_ito(self):
-        s = ' abc '
-        src = Ito(s, 1, -1)
-        gaps = [Span(1, 2), Span(0, 1)]  # Overlapping and unordered
-        desc = 'x'
-        for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
-            with self.subTest(_class=cls_name):
-                expected = [_class(src, 2, desc=desc)]
-                actual = [*_class.from_gaps(src, *gaps, desc=desc)]
-                self.assertListEqual(expected, actual)
-                    
+        for ordered in True, False:
+            for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
+                with self.subTest(_class=cls_name, ordered=ordered):
+                    if ordered:
+                        ngs = non_gaps.copy()
+                        ngs.sort(key=lambda i: i.start)
+                        expected = [
+                            _class(s, 0, min(gap.start for gap in non_gaps), desc),
+                            _class(s, max(gap.stop for gap in non_gaps), desc=desc)
+                        ]
+                        actual = [*_class.from_gaps(s, ngs, desc=desc)]
+                        self.assertListEqual(expected, actual)
+                    else:
+                        ngs = non_gaps.copy()
+                        with self.assertRaises(ValueError):
+                            [*_class.from_gaps(s, ngs, desc=desc)]
+
     def test_from_substrings(self):
         string = 'abcd' * 10
         string = f' {string} '
 
         with self.subTest(spacing='Consecutive'):
             for size in ((1, 1), (2, 2), (1, 3), (2, 3)):
                 with self.subTest(size_range=size):
@@ -235,15 +375,15 @@
 
         with self.subTest(spacing='Overlaps'):
             for size in ((3, 3),):
                 with self.subTest(size_range=size):
                     rs = RandSubstrings(size, Span(-1, -1))
                     subs = [*rs.generate(string, 1, -1)]
                     with self.assertRaises(Exception):
-                        itos = [*Ito.from_substrings(string, *subs)]
+                        [*Ito.from_substrings(string, *subs)]
 
     def test_clone_basic(self):
         string = 'abc'
         d = 'x'
         ito = Ito(string, 1, 2, desc=d)
 
         params = [
@@ -287,25 +427,28 @@
         clone = parent.clone()
         self.assertEqual(len(parent.children), len(clone.children))
         for c, cc in zip(parent.children, clone.children):
             self.assertIsNot(c, cc)
             self.assertEqual(c, cc)
 
     def test_clone_children(self):
-        s = 'abc'
-        parent = Ito(s, desc='parent')
-        self.add_chars_as_children(parent, 'child')
-
-        for cc in (True, False):
-            with self.subTest(clone_children=cc):
-                clone = parent.clone(clone_children=cc)
-                if cc:
-                    self.assertSequenceEqual([*parent.children], [*clone.children])
-                else:
-                    self.assertEqual(0, len(clone.children))
+        s = ' one two three '
+        root = Ito(s, 1, -1, 'root')
+        root.children.add(*root.str_split())
+        for c in root.children:
+            c.children.add(*c)
+
+        self.assertEqual(len(s.split()), len(root.children))
+        for c in root.children:
+            self.assertEqual(len(c), len(c.children))
+
+        clone = root.clone()
+        self.assertSequenceEqual([*root.children], [*clone.children])
+        for rc, cc in zip(root.children, clone.children):
+            self.assertSequenceEqual([*rc.children], [*cc.children])
 
     def test_clone_with_value_func(self):
         string = ' abcdef '
         f1 = lambda ito: str(ito).strip()
         f2 = lambda ito: str(ito).upper()
 
         root = Ito(string)
```

### Comparing `pawpaw-1.0.0a9/tests/test_ito_regex_equivalence_methods.py` & `pawpaw-1.0.0rc1/tests/test_ito_regex_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_ito_serialization.py` & `pawpaw-1.0.0rc1/tests/test_ito_serialization.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_ito_str_equivalence_methods.py` & `pawpaw-1.0.0rc1/tests/test_ito_str_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_itorator.py` & `pawpaw-1.0.0rc1/tests/arborform/test_itorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,401 +1,386 @@
+import itertools
 import typing
 
 import regex
-from pawpaw import Ito, Types, PredicatedValue
-from pawpaw.arborform import Itorator, Postorator, Reflect, Desc
+from pawpaw import Ito, Types
+from pawpaw.arborform import Itorator, Connectors, Postorator
 from tests.util import _TestIto
 
 
 class TestItorator(_TestIto):
-    """Uses Reflect and Wrap classes, which have trivial implementation, to test base class functionality"""
-
-    def test_add_self_itor_sub(self):
-        i1 = Reflect()
-
-        for itor in i1, Reflect():
-            with self.subTest(itor_is_self=itor is i1):
-                i1.itor_sub = itor
-                self.assertEqual(1, len(i1.itor_sub))
-                self.assertEqual(itor, i1.itor_sub[0].value)
-                
-                i1.itor_sub = None
-                self.assertEqual(0, len(i1.itor_sub))
-
-    def test_add_self_itor_children(self):
-        i1 = Reflect()
-
-        for itor in i1, Reflect():
-            with self.subTest(itor_is_self=itor is i1):
-                i1.itor_children = itor
-                self.assertEqual(1, len(i1.itor_children))
-                self.assertEqual(itor, i1.itor_children[0].value)
-                
-                i1.itor_children = None
-                self.assertEqual(0, len(i1.itor_children))
-
-    def test_add_self_itor_next(self):
-        i1 = Reflect()
-
-        for itor in i1, Reflect():
-            with self.subTest(itor_is_self=itor is i1):
-                i1.itor_next = itor
-                self.assertEqual(1, len(i1.itor_next))
-                self.assertEqual(itor, i1.itor_next[0].value)
-                
-                i1.itor_next = None
-                self.assertEqual(0, len(i1.itor_next))                
-
-    def test_update_itor_children_mode_valid(self):
-        itor = Reflect()
-
-        # Loop twice in case the initial set is the default value
-        for i in range(2):
-            for icm in Itorator.ItorChildrenMode:
-                itor.itor_children_mode = icm
-                self.assertEqual(icm, itor.itor_children_mode)
-
-    def test_update_itor_children_mode_ivalid(self):
-        itor = Reflect()
-
+    @classmethod
+    def get_reflect(cls) -> Itorator:
+        return Itorator.wrap(lambda ito: (ito,))
+
+    @classmethod
+    def change_desc(cls, ito: Ito, desc: str | None) -> Types.C_IT_ITOS:
+        ito.desc = desc
+        return ito,
+
+    @classmethod
+    def get_desc(cls, desc: str | None) -> Itorator:
+        return Itorator.wrap(lambda ito: cls.change_desc(ito, desc))
+
+    def test_call_fails_on_non_ito(self):
+        s = ' abc '
+        itor = self.get_reflect()
         with self.assertRaises(TypeError):
-            itor.itor_children_mode = 'a'
+            next(itor(s))
 
-        with self.assertRaises(TypeError):
-            itor.itor_children_mode = None
+    def test_call_clones_ito(self):
+        s = ' abc '
+        root = Ito(s, 1, -1)
+        itor = self.get_reflect()
+        rv = next(itor(root))
+        self.assertEqual(root, rv)
+        self.assertIsNot(root, rv)
 
-    def test_wrap_lambda(self):
-        s = 'abc'
-        root = Ito(s)
-        itor = Itorator.wrap(lambda ito: [ito[:1]])
-        self.assertSequenceEqual(root[:1], [*itor(root)])
+    def test_traverse_does_not_clone(self):
+        s = ' abc '
+        root = Ito(s, 1, -1)
+        itor = self.get_reflect()
+        rv = next(itor._traverse(root))
+        self.assertIs(root, rv)
 
-    def test_wrap_method(self):
-        def my_split(ito: Ito) -> Types.C_SQ_ITOS:
-            yield from ito.str_split()
+    def test_wrap(self):
+        s = ' abc '
+        root = Ito(s, 1, -1)
+        desc = 'x'
+        itor = self.get_desc(desc)
+        rv = next(itor(root))
+        self.assertNotEqual(desc, root.desc)
+        self.assertEqual(desc, rv.desc)
 
-        s = 'one two three'
-        root = Ito(s)
-        itor = Itorator.wrap(my_split)
-        self.assertSequenceEqual([*Ito.from_substrings(s, *s.split())], [*itor(root)])
+    def test_clone(self):
+        s = ' abc '
+        root = Ito(s, 1, -1)
+        tag = 'x'
+        itor_r = self.get_reflect()
+        itor_r.tag = tag
 
-    def test_traverse_clones(self):
-        s = 'abc'
-        root = Ito(s)
-        reflect = Reflect()
-        rv = [*reflect(root)]
-        self.assertEqual(1, len(rv))
-        self.assertEqual(root, rv[0])
-        self.assertIsNot(root, rv[0])
+        itor_d = self.get_desc('foo')
+        con = Connectors.Delegate(itor_d)
+        itor_r.connections.append(con)
 
-    def test_traverse_does_clone(self):
-        s = 'abc'
-        root = Ito(s)
-        root.children.add(*root)
+        self.assertEqual(tag, itor_r.tag)
+        self.assertEqual(1, len(itor_r.connections))
 
-        reflect = Reflect()
-        rv = [*reflect(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(root, rv[0])
-        self.assertIsNot(root, rv[0])
+        itor_c = itor_r.clone()
+        self.assertIsNot(itor_r, itor_c)
+        self.assertEqual(tag, itor_c.tag)
+        self.assertEqual(0, len(itor_c.connections))
 
-        self.assertSequenceEqual([*root.children], [*rv[0].children])
-        self.assertTrue(root_c is not rv_c for root_c, rv_c in zip(root.children, rv[0].children))
+    #region Connectors
 
-    def test_traverse_with_itor_sub(self):
-        s = 'abc'
+    def test_yield_break_1(self):
+        s = '123a321'
         root = Ito(s)
 
-        itor_root = Reflect()
-        itor_root.itor_sub = Itorator.wrap(lambda ito: (Ito(ito, 1, -1),))
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertNotEqual(root, rv[0])
-        self.assertSequenceEqual([*root.children], [*rv[0].children])
+        itor_1 = Itorator.wrap(lambda ito: [ito.str_strip('1')])
+        itor_2 = Itorator.wrap(lambda ito: [ito.str_strip('2')])
+        itor_3 = Itorator.wrap(lambda ito: [ito.str_strip('3')])
 
-    def test_traverse_with_itor_sub_bifurcation(self):
-        s = 'abcde'
-        root = Ito(s)
-        vowels = 'aeiou'
+        itor_1.connections.append(Connectors.Delegate(itor_2))
+        itor_1.connections.append(Connectors.Delegate(itor_3))
+        rv = [*itor_1(root)]
 
-        chars = Itorator.wrap(lambda ito: [*ito])
-        chars.itor_sub = lambda ito: str(ito) in vowels, Desc('vowel')
-        chars.itor_sub.append(Desc('consonant'))
-
-        results = [*chars(root)]
-        self.assertEqual(len(s), len(results))
-        self.assertListEqual([i for i in s if i in vowels], [str(i) for i in results if i.desc == 'vowel'])
-        self.assertListEqual([i for i in s if i not in vowels], [str(i) for i in results if i.desc == 'consonant'])
-
-        chars.itor_next = Desc('changed')
-        results = [*chars(root)]
-        self.assertEqual(len(s), len(results))
-        self.assertTrue(all(i.desc == 'changed' for i in results))        
+        self.assertSequenceEqual([Ito(root, 2, -2)], rv)
 
-    def test_traverse_with_itor_children_mode_add(self):
-        s = 'abc'
-        root = Ito(s)
+        itor_1.connections.clear()
+        itor_1.connections.append(Connectors.Delegate(itor_2))
+        itor_2.connections.append(Connectors.Delegate(itor_3))
+        rv = [*itor_1(root)]
 
-        itor_root = Reflect()
-        itor_root.itor_children = Itorator.wrap(lambda ito: ito)
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(str(root), str(rv[0]))
+        self.assertSequenceEqual([Ito(root, 3, -3)], rv)
 
-        self.assertEqual(0, len(root.children))  # Ensure input ito.children unaffected
-        self.assertSequenceEqual(root, rv[0].children)
+    def test_yield_break_2(self):
+        s = ' abc '
+        root = Ito(s, 1, -1)
+        desc = 'x'
+        itor_r = self.get_reflect()
+        itor_d = self.get_desc(desc)
+
+        lambdas = {
+            '[default]': None,
+            'Always True': lambda ito: True,
+            'Always False': lambda ito: False,
+        }
+
+        for lam_desc, lam_f in lambdas.items():
+            with self.subTest(lambda_=lam_desc):
+                if lam_f is None:
+                    itor_r.connections.append(Connectors.Delegate(itor_d))
+                else:
+                    itor_r.connections.append(Connectors.Delegate(itor_d, lam_f))
+
+                if lam_f is None or lam_f(root):
+                    expected = self.change_desc(root, desc)[0]
+                else:
+                    expected = root
+
+                rv = next(itor_r(root))
+                self.assertEqual(expected, rv)
+
+    def test_assign(self):
+        s = '123a321'
+        root = Ito(s)
+
+        itor_1 = Itorator.wrap(lambda ito: [ito.str_strip('1')])
+        itor_2 = Itorator.wrap(lambda ito: [ito.str_strip('2')])
+        itor_3 = Itorator.wrap(lambda ito: [ito.str_strip('3')])
+
+        itor_1.connections.append(Connectors.Recurse(itor_2))
+        itor_1.connections.append(Connectors.Recurse(itor_3))
+        rv = [*itor_1(root)]
+
+        self.assertSequenceEqual([Ito(root, 3, -3)], rv)
+
+        itor_1.connections.clear()
+        itor_1.connections.append(Connectors.Recurse(itor_2))
+        itor_2.connections.append(Connectors.Recurse(itor_3))
+        rv = [*itor_1(root)]
 
-    def test_traverse_with_itor_children_mode_replace_with_self(self):
-        s = 'a b c'
-        root = Ito(s)
-        root.children.add(*root)
+        self.assertSequenceEqual([Ito(root, 3, -3)], rv)
 
-        itor_root = Reflect()
+    def test_assign_with_pipeline(self):
+        s = ' one 123 two 456 '
+        root = Ito(s, 1, -1)
 
-        itor_children = lambda ito: ito.children
-        itor_root.itor_children = itor_children
-        itor_root.itor_children_mode = Itorator.ItorChildrenMode.REPLACE
+        itor_r = self.get_reflect()
 
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(str(root), str(rv[0]))
+        # create sub-pipeline with two endpoints
+        itor_tok_split = Itorator.wrap(lambda ito: ito.str_split())
+        con = Connectors.Recurse(itor_tok_split)
+        itor_r.connections.append(con)
 
-        self.assertSequenceEqual([*root.children], [*rv[0].children])
+        itor_desc_word = self.get_desc('word')
+        con = Connectors.Delegate(itor_desc_word, lambda ito: not ito.str_isnumeric())
+        itor_tok_split.connections.append(con)
 
-    def test_traverse_with_itor_children_mode_replace_with_clones(self):
-        s = 'a b c'
-        root = Ito(s)
-        root.children.add(*root)
+        itor_desc_num = self.get_desc('number')
+        con = Connectors.Delegate(itor_desc_num)
+        itor_tok_split.connections.append(con)
 
-        itor_root = Reflect()
+        # ensure this works as expected
+        rv = [*itor_r(root)]
+        self.assertEqual(len(root.str_split()), len(rv))
+        self.assertTrue(all(i.desc in ['word', 'number'] for i in rv))
 
-        itor_children = lambda ito: [c.clone() for c in ito.children]
-        itor_root.itor_children = itor_children
-        itor_root.itor_children_mode = Itorator.ItorChildrenMode.REPLACE
+        # now add a Next connection AFTER the sub-pipeline
+        def prepend_x(ito) -> Types.C_IT_ITOS:
+            ito.desc = 'x' + ito.desc
+            return ito,
 
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(str(root), str(rv[0]))
+        itor_desc_pre_x = Itorator.wrap(prepend_x)
+        con = Connectors.Delegate(itor_desc_pre_x)
+        itor_r.connections.append(con)
 
-        self.assertSequenceEqual([*root.children], [*rv[0].children])        
+        # ensure next connects to all the sub-pipeline's endpoints
+        rv = [*itor_r(root)]
+        self.assertEqual(len(root.str_split()), len(rv))
+        self.assertTrue(all(i.desc.startswith('x') for i in rv))
 
-    def test_traverse_with_itor_children_mode_replace_with_different(self):
-        s = 'a b c'
+    def test_sub(self):
+        s = '123a321'
         root = Ito(s)
-        root.children.add(*root)
-
-        f = lambda ito: (Ito(ito, 1, -1),)
 
-        itor_root = Reflect()
-        itor_root.itor_children = Itorator.wrap(f)
-        itor_root.itor_children_mode = Itorator.ItorChildrenMode.REPLACE
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(str(root), str(rv[0]))
-
-        self.assertNotEqual(len(root.children), len(rv[0].children))
-        self.assertEqual(1, len(rv[0].children))
-        
-        self.assertSequenceEqual([*f(root)], [*rv[0].children])        
-
-    def test_traverse_with_itor_children_mode_delete(self):
-        s = 'a b c'
-        root = Ito(s)
-        root.children.add(*root)
+        itor_1 = Itorator.wrap(lambda ito: [ito.str_strip('1')])
+        itor_2 = Itorator.wrap(lambda ito: [ito.str_strip('2')])
 
-        f = lambda ito: ito.children[1:-1]
+        itor_1.connections.append(Connectors.Subroutine(itor_2))
+        rv = [*itor_1(root)]
 
-        itor_root = Reflect()
-        itor_root.itor_children = Itorator.wrap(f)
-        itor_root.itor_children_mode = Itorator.ItorChildrenMode.DEL
-        rv = [*itor_root(root)]
-            
-        self.assertEqual(1, len(rv))
-        self.assertEqual(str(root), str(rv[0]))
+        self.assertSequenceEqual([Ito(root, 1, -1)], rv)
 
-        self.assertNotEqual(len(root.children), len(rv[0].children))
-        self.assertEqual(2, len(rv[0].children))
-        
-        expected = [c for c in root.children if c not in f(root)]
-        self.assertSequenceEqual(expected, [*rv[0].children])
-        
-    def test_traverse_with_plumule_on_added_children(self):
-        s = ' one two three '
-        root = Ito(s, 1, -1)
+        def sec_desc_x(ito) -> typing.Iterable[Ito]:
+            ito.desc = 'x'
+            return  # don't yield anything
+            yield  # this forces interpretation as a generator method
 
-        expected = root.clone()
-        expected.children.add(*expected.str_split())
-        for c in expected.children:
-            c.children.add(*c)
+        itor_2 = Itorator.wrap(sec_desc_x)
 
-        itor_split_wrds = Itorator.wrap(lambda ito: ito.str_split())
+        itor_1.connections.clear()
+        itor_1.connections.append(Connectors.Subroutine(itor_2))
+        rv = [*itor_1(root)]
 
-        itor_split_chrs = Itorator.wrap(lambda ito: ito)
-        itor_split_wrds.itor_children = itor_split_chrs
+        self.assertSequenceEqual([Ito(root, 1, -1, 'x')], rv)
 
-        itor_word_desc = Desc('word')
-        itor_split_wrds.itor_next = lambda ito: ito.find('*') is not None, itor_word_desc  # plumule child search
+    def test_children(self):
+        s = ' one 123 two 456 '
+        root = Ito(s, 1, -1)
+        
+        itor_r = self.get_reflect()
 
-        itor_children = Itorator.wrap(lambda ito: ito.children)
-        itor_word_desc.itor_children_mode = Itorator.ItorChildrenMode.REPLACE
-        itor_word_desc.itor_children = itor_children
+        # Add
+        itor_tok_split = Itorator.wrap(lambda ito: ito.str_split())
+        con = Connectors.Children.Add(itor_tok_split)
+        itor_r.connections.append(con)
 
-        itor_chr_desc = Desc('char')
-        itor_children.itor_next = lambda ito: ito.find('..') is not None, itor_chr_desc  # plumule parent search
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(len(root.str_split()), len(rv[0].children))
 
-        rv = root.clone()
-        rv.children.add(*itor_split_wrds(root))
+        all_tokens_root = rv[0]
 
-        self.assertSequenceEqual(
-            [str(i) for i in expected.find_all('**')],
-            [str(i) for i in rv.find_all('**')]
-        )
+        # AddHierarchical
+        itor_char_split = Itorator.wrap(lambda ito: itertools.chain.from_iterable(ito.children))
+        con = Connectors.Children.AddHierarchical(itor_char_split)
+        itor_r.connections.clear()
+        itor_r.connections.append(con)
 
-        for child in rv.children:
-            self.assertEqual('word', child.desc)
-            for gc in child.children:
-                self.assertEqual('char', gc.desc)
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(all_tokens_root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(len(root.str_split()), len(rv[0].children))
+            for t in rv[0].children:
+                self.assertEqual(len(t), len(t.children))
+
+        # Delete
+        def numerics(ito) -> Types.C_IT_ITOS:
+            for c in ito.children:
+                if c.str_isnumeric():
+                    yield c
+        itor_numerics = Itorator.wrap(numerics)
+        con = Connectors.Children.Delete(itor_numerics)
+        itor_r.connections.clear()
+        itor_r.connections.append(con)
+        
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(all_tokens_root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(sum(1 for i in all_tokens_root.children if i.str_isnumeric()), len(rv[0].children))
 
-    def test_traverse_with_itor_next(self):
-        s = 'abc'
-        root = Ito(s)
+        # Replace
+        def alphas(ito) -> Types.C_IT_ITOS:
+            for c in ito.children:
+                if not c.str_isnumeric():
+                    c.desc = 'alpha'
+                    yield c
+        itor_alphas = Itorator.wrap(alphas)
+        con = Connectors.Children.Replace(itor_alphas)
+        itor_r.connections.clear()
+        itor_r.connections.append(con)
 
-        itor_root = Reflect()
-        itor_root.itor_next = Itorator.wrap(lambda ito: (Ito(ito, 1, -1),))
-        rv = [*itor_root(root)]
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(all_tokens_root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(sum(1 for i in all_tokens_root.children if not i.str_isnumeric()), len(rv[0].children))
+            self.assertTrue(all(i.desc == 'alpha' for i in rv[0].children))
             
-        self.assertEqual(1, len(rv))
-        self.assertNotEqual(root, rv[0])
-        self.assertSequenceEqual([*root.children], [*rv[0].children])
-        
-    def test_traverse_with_carry_through(self):
-        s = 'abc'
-        root = Ito(s)
-        d_changed = 'changed'
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(all_tokens_root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(sum(1 for i in all_tokens_root.children if i.str_isnumeric()), len(rv[0].children))
 
-        reflect = Reflect()
-        make_chars = Itorator.wrap(lambda ito: tuple(ito.clone(i, i+1, 'char') for i in range(*ito.span)))
-        reflect.itor_children = make_chars
-        rename = Itorator.wrap(lambda ito: (ito.clone(desc=d_changed),))
-        make_chars.itor_next = rename
-        rv = [*reflect(root)]
-            
-        self.assertEqual(1, len(rv))
-        ito = rv[0]
-        self.assertIsNot(root, ito)
-        self.assertSequenceEqual(s, [str(i) for i in ito.children])
-        self.assertTrue(all(c.desc == d_changed for c in ito.children))
+        def alphas(ito) -> Types.C_IT_ITOS:
+            for c in ito.children:
+                if not c.str_isnumeric():
+                    c.desc = 'alpha'
+                    yield c
+        itor_alphas = Itorator.wrap(alphas)
+        con = Connectors.Children.Replace(itor_alphas)
+        itor_r.connections.clear()
+        itor_r.connections.append(con)
 
-    def test_traverse_with_postorator(self):
+        with self.subTest(children_type=type(con).__name__):
+            rv = [*itor_r(all_tokens_root)]
+            self.assertEqual(1, len(rv))
+            self.assertEqual(sum(1 for i in all_tokens_root.children if not i.str_isnumeric()), len(rv[0].children))
+            self.assertTrue(all(i.desc == 'alpha' for i in rv[0].children))
+
+    def test_postorator(self):
         s = 'abc def ghi'
         root = Ito(s)
 
-        reflect = Reflect()
-
-        word_splitter = Itorator.wrap(lambda ito: ito.str_split())
-        reflect.itor_next = word_splitter
-
-        char_splitter = Itorator.wrap(lambda ito: [*ito])
-
         def simple_join(itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
             yield Ito.join(*itos)
 
-        with self.subTest(chain_length=1, scenario='itor_next'):
-            rv = [*reflect(root)]
-            self.assertEqual(3, len(rv))
+        word_splitter = Itorator.wrap(lambda ito: ito.str_split())
+
+        with self.subTest(chain_length=1, chain_depth=0):
+            rv = [*word_splitter(root)]
+            self.assertSequenceEqual(root.str_split(), rv)
 
             word_splitter.postorator = Postorator.wrap(simple_join)
-            rv = [*reflect(root)]
+            rv = [*word_splitter(root)]
             self.assertEqual(1, len(rv))
+            self.assertEqual(root, rv[0])
 
-        with self.subTest(chain_length=2, scenario='itor_next'):
-            word_splitter.postorator = None
-            word_splitter.itor_next = char_splitter
-            rv = [*reflect(root)]
-            self.assertEqual(9, len(rv))
+        with self.subTest(chain_length=2, chain_depth=0):
+            word_splitter = word_splitter.clone()
 
-            char_splitter.postorator = Postorator.wrap(simple_join)
-            rv = [*reflect(root)]
-            self.assertEqual(3, len(rv))
+            char_splitter = Itorator.wrap(lambda ito: ito)
+            con = Connectors.Delegate(char_splitter)
+            word_splitter.connections.append(con)
+            expected = [j for i in word_splitter(root) for j in i]
+            rv = [*word_splitter(root)]
+            self.assertSequenceEqual(expected, rv)
 
             word_splitter.postorator = Postorator.wrap(simple_join)
-            rv = [*reflect(root)]
+            rv = [*word_splitter(root)]
             self.assertEqual(1, len(rv))
+            self.assertEqual(root, rv[0])
 
-            char_splitter.postorator = None
-            rv = [*reflect(root)]
-            self.assertEqual(1, len(rv))
-
-        with self.subTest(chain_length=2, scenario='itor_child'):
             word_splitter.postorator = None
-            word_splitter.itor_next = None
-            word_splitter.itor_children = char_splitter
-            rv = [*reflect(root)]
-            self.assertEqual(3, len(rv))
-            self.assertEqual(9, sum(len(i.children) for i in rv))            
-
             char_splitter.postorator = Postorator.wrap(simple_join)
-            rv = [*reflect(root)]
-            self.assertEqual(3, len(rv))
-            self.assertEqual(3, sum(len(i.children) for i in rv))            
+            rv = [*word_splitter(root)]
+            self.assertSequenceEqual(root.str_split(), rv)
+
+        with self.subTest(chain_length=1, chain_depth=1):
+            word_splitter = word_splitter.clone()
+            char_splitter = char_splitter.clone()
+
+            con = Connectors.Children.Add(char_splitter)
+            word_splitter.connections.append(con)
+            rv = [*word_splitter(root)]
+            self.assertSequenceEqual(root.str_split(), rv)
+            for w in rv:
+                self.assertSequenceEqual([*w], [*w.children])
 
             word_splitter.postorator = Postorator.wrap(simple_join)
-            rv = [*reflect(root)]
+            rv = [*word_splitter(root)]
             self.assertEqual(1, len(rv))
-            self.assertEqual(0, len(rv[0].children))  # Ito.join doesn't include children
+            self.assertEqual(root, rv[0])
+
+            word_splitter.postorator = None
+            char_splitter.postorator = Postorator.wrap(simple_join)
+            rv = [*word_splitter(root)]
+            self.assertSequenceEqual(root.str_split(), rv)
+            for w in rv:
+                self.assertSequenceEqual([w,], [*w.children])
 
     def test_traverse_complex(self):
-        basis = 'ABcd123'
-        s = f' {basis} - {basis} '
-        root = Ito(s, desc='root')
-        
-        func = lambda ito: [*ito.split(regex.compile(r'\-'), desc='phrase')]
-        splt_space = Itorator.wrap(func)
-        
-        func = lambda ito: [ito.str_strip()]
-        stripper = Itorator.wrap(func)
-        splt_space.itor_children = stripper
-        
-        func = lambda ito: [*ito.split(regex.compile(r'(?<=[A-Za-z])(?=\d)'))]
-        splt_alpha_num = Itorator.wrap(func)
-        stripper.itor_children = splt_alpha_num
-        
-        func = lambda ito: [ito.clone(desc='numeric' if str(ito).isnumeric() else 'alpha')]
-        namer = Itorator.wrap(func)
-        splt_alpha_num.itor_next = namer
-        
-        func = lambda ito: [*ito.split(regex.compile(r'(?<=\d)(?=\d)'), desc='digit')]
-        splt_digits = Itorator.wrap(func)
-        
-        func = lambda ito: [*ito.split(regex.compile(r'(?<=[A-Z])(?=[a-z])'), desc='upper or lower')]
-        splt_case = Itorator.wrap(func)
-        
-        namer.itor_children = (lambda ito: ito.desc == 'numeric', splt_digits)
-        namer.itor_children.append(splt_case)
-        
-        func = lambda ito: [ito.clone(i, i + 1, desc='char') for i in range(ito.start, ito.stop)]
-        splt_chars = Itorator.wrap(func)
-        splt_case.itor_children = splt_chars
-        
-        root.children.add(*splt_space(root))
-        
-        expected_child_count = s.count('-') + 1
-        self.assertEqual(expected_child_count, len(root.children))
-        
-        expected_alpha_count = expected_child_count
-        self.assertEqual(expected_alpha_count, sum(1 for i in root.find_all('**[d:alpha]')))
+        s = ' one two three '
+        root = Ito(s, 1, -1)
         
-        expected_leaves_count = len(basis) * 2
-        self.assertEqual(expected_leaves_count, sum(1 for i in root.find_all('***')))
-            
-        depth = 1
-        cur = root
-        while len(cur.children) > 0:
-            cur = cur.children[0]
-            depth += 1
-        self.assertEqual(6, depth)
+        itor_wrd_split = Itorator.wrap(lambda ito: ito.str_split())
+
+        itor_wrd_desc = Itorator.wrap(lambda ito: [ito.clone(desc='word'), ])
+        con = Connectors.Recurse(itor_wrd_desc)
+        itor_wrd_split.connections.append(con)
+
+        itor_char_split = Itorator.wrap(lambda ito: ito)
+        con = Connectors.Children.Add(itor_char_split)
+        itor_wrd_split.connections.append(con)
+
+        itor_char_desc = Itorator.wrap(lambda ito: [ito.clone(desc='char'), ])
+        con = Connectors.Recurse(itor_char_desc)
+        itor_char_split.connections.append(con)
+
+        itor_char_desc_vowel = Itorator.wrap(lambda ito: [ito.clone(desc='char-vowel'), ])
+        con = Connectors.Recurse(itor_char_desc_vowel, lambda ito: str(ito) in 'aeiou')
+        itor_char_desc.connections.append(con)
+
+        rv = [*itor_wrd_split(root)]
+
+        self.assertSequenceEqual(root.split(regex.compile(r'\s+'), desc='word'), rv)
+        for word in rv:
+            self.assertEqual(len(word), len(word.children))
+            for c in word.children:
+                if str(c) in 'aeiou':
+                    self.assertEqual('char-vowel', c.desc)
+                else:
+                    self.assertEqual('char', c.desc)
+
+    #endregion
```

### Comparing `pawpaw-1.0.0a9/tests/test_itorator_extract.py` & `pawpaw-1.0.0rc1/tests/arborform/test_itorator_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import regex
 from pawpaw import Ito
 from pawpaw.arborform import Extract
 from tests.util import _TestIto
 
 
 class TestExtract(_TestIto):
-    def test_iter(self):
+    def test_transform(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )+')
         itor = Extract(re)
-        rv = itor._transform(root)
+        rv = [*itor._transform(root)]
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(3, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
             self.assertEqual(2, len(phrase.children))
```

### Comparing `pawpaw-1.0.0a9/tests/test_itorator_split.py` & `pawpaw-1.0.0rc1/tests/arborform/test_itorator_split.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_nlp.py` & `pawpaw-1.0.0rc1/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_postorator.py` & `pawpaw-1.0.0rc1/tests/arborform/test_postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_postorator_windowed_join.py` & `pawpaw-1.0.0rc1/tests/arborform/test_postorator_windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_query_and_traversal.py` & `pawpaw-1.0.0rc1/tests/test_query_and_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,36 +36,35 @@
 
         self.leaves = [d for d in self.root.walk_descendants() if len(d.children) == 0]
 
         self.leaf = next(i for i in self.leaves if str(i.parent) == 'eleven' and str(i) == 'v')
 
         self.descs = ['root', 'phrase', 'word', 'char']
 
-
     def test_walk_descendants(self):
-
-        for node_type, node in {'root': self.root, 'leaf': self.leaf}.items():
-            for start in 0, 5:
-                with self.subTest(node=node_type, start=start):
-                    forward = [*node.walk_descendants_levels(start)]
-                    _reversed = [*node.walk_descendants_levels(start, True)]
-
-                    if node is self.root:
-                        self.assertEqual(self.descendants_count, len(forward))
-                        self.assertEqual(self.descendants_count, len(_reversed))
-                    elif node is self.leaf:
-                        self.assertEqual(0, len(forward))
-                        self.assertEqual(0, len(_reversed))
-                    if 0 < len(forward) == len(_reversed):
-                        self.assertEqual(start, forward[0].index)
-                        max_level = max(ei.index for ei in forward)
-                        self.assertEqual(max_level, _reversed[0].index)
-
-                    _reversed.reverse()
-                    self.assertListEqual(forward, _reversed)
+        s = " one two three "
+        counter = 0
+        root = Ito(s, 1, -2, str(counter))
+
+        for word in root.str_split():
+            word.desc = str(counter := counter + 1)
+            root.children.add(word)
+            for c in word:
+                c.desc = str(counter := counter + 1)
+                word.children.add(c)
+
+        with self.subTest(reverse=False):
+            expected = [str(i) for i in range(1, counter + 1)]
+            actual = [i.desc for i in root.walk_descendants()]
+            self.assertListEqual(expected, actual)
+
+        with self.subTest(reverse=True):
+            expected = [str(i) for i in range(counter, 0, -1)]
+            actual = [i.desc for i in root.walk_descendants(reverse=True)]
+            self.assertListEqual(expected, actual)
 
 
 class TestItoQuery(TestItoTraversal):
     #region declarations
 
     def test_filter_keys_unique(self):
         fks = [*itertools.chain(*pawpaw.query.FILTER_KEYS.values())]
@@ -608,14 +607,31 @@
                     with self.subTest(node=node_type, order=order, index=istr, path=path):
                         expected = [c for c in node.children]
                         if order == '-':
                             expected.reverse()
                         expected = expected[slice(*index)]
                         actual = [*node.find_all(path)]
                         self.assertSequenceEqual(expected, actual)
+                
+    def test_filter_index_range_unbounded(self):
+        for node_type, node in {'root': self.root}.items():
+            for order in '', '+', '-':
+                for index in 0, 1, 2:
+                    for negation in True, False:
+                        path = f'{order}*[{"~" if negation else ""}i:{index}-]'
+                        with self.subTest(node=node_type, order=order, index=f'{index}-', path=path):
+                            expected = [c for c in node.children]
+                            if order == '-':
+                                expected.reverse()
+                            if negation:
+                                expected = expected[:index]
+                            else:
+                                expected = expected[index:]
+                            actual = [*node.find_all(path)]
+                            self.assertSequenceEqual(expected, actual)
 
     def test_filter_index_mix(self):
         for node_type, node in {'root': self.root}.items():
             for order in '', '+', '-':
                 for istr, _slices in (('0,2-4,6', (slice(0, 1), slice(2, 4), slice(6, 7))), ):
                     path = f'{order}**[i:{istr}]'
                     with self.subTest(node=node_type, order=order, index=istr, path=path):
```

### Comparing `pawpaw-1.0.0a9/tests/test_sgr.py` & `pawpaw-1.0.0rc1/tests/visualization/test_sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_span.py` & `pawpaw-1.0.0rc1/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_type_magic.py` & `pawpaw-1.0.0rc1/tests/test_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_util.py` & `pawpaw-1.0.0rc1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_visualization_ascii_box.py` & `pawpaw-1.0.0rc1/tests/visualization/test_visualization_ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/test_xml_helper.py` & `pawpaw-1.0.0rc1/tests/test_xml_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             with self.subTest(xml_sample_index=sample_index):
                 root = ET.fromstring(sample.xml, xml.XmlParser())
                 xmlns = xml.XmlHelper.get_xmlns(root)
                 xmlns = {str(k.local_part): str(v) for k, v in xmlns.items()}
                 if sample.default_namespace is None:
                     self.assertIsNone(xmlns.get('xmlns'))
                 else:
-                    self.assertLessEqual({'xmlns': sample.default_namespace}.items(), xmlns.items())
+                    self.assertLessEqual({'xmlns': sample.default_namespace[1:-1]}.items(), xmlns.items())
                 self.assertLessEqual(sample.root_prefix_map.items(), xmlns.items())
 
     def test_get_prefix_map_root(self):
         for sample_index, sample in enumerate(XML_TEST_SAMPLES):
             with self.subTest(xml_sample_index=sample_index):
                 root = ET.fromstring(sample.xml, xml.XmlParser())
                 self.assertDictEqual(sample.root_prefix_map, xml.XmlHelper.get_prefix_map(root))
@@ -58,20 +58,24 @@
                 actual = {}
                 for e in root.findall('.//'):
                     actual |= xml.XmlHelper.get_prefix_map(e)
                 self.assertDictEqual(sample.descendants_composite_prefix_map, actual)
 
     def test_get_default_namespace(self):
         for sample_index, sample in enumerate(XML_TEST_SAMPLES):
-            with self.subTest(xml_sample_index=sample_index):
-                root = ET.fromstring(sample.xml, xml.XmlParser())
-                if sample.default_namespace is None:
-                    self.assertIsNone(xml.XmlHelper.get_default_namespace(root))
-                else:
-                    self.assertEqual(sample.default_namespace, str(xml.XmlHelper.get_default_namespace(root)))
+            depth = 0
+            element = ET.fromstring(sample.xml, xml.XmlParser())
+            while element is not None:
+                with self.subTest(xml_sample_index=sample_index, depth=depth):
+                    if sample.default_namespace is None:
+                        self.assertIsNone(xml.XmlHelper.get_default_namespace(element))
+                    else:
+                        self.assertEqual(sample.default_namespace, str(xml.XmlHelper.get_default_namespace(element)))
+                depth += 1
+                element = element.find('*')
 
     def test_get_element_text_if_found(self):
         for sample_index, sample in enumerate(XML_TEST_SAMPLES):
             path = sample.text_containing_descendant_path
             with self.subTest(xml_sample_index=sample_index, path=path):
                 root = ET.fromstring(sample.xml, xml.XmlParser())
                 expected = root.find(path).text
@@ -79,14 +83,30 @@
                 self.assertEqual(expected, actual)
 
             invalid_path = path + '/.[tag=""]'  # ensures path returns nothing
             with self.subTest(xml_sample_index=sample_index, path=invalid_path):
                 actual = xml.XmlHelper.get_element_text_if_found(root, invalid_path)
                 self.assertIsNone(actual)
 
+    def test_get_parent_element(self):
+        for sample_index, sample in enumerate(XML_TEST_SAMPLES):
+            root = ET.fromstring(sample.xml, xml.XmlParser())
+            
+            depth = 0
+            with self.subTest(xml_sample_index=sample_index, depth=depth):
+                self.assertIsNone(xml.XmlHelper.get_parent_element(root))
+
+            parent = root
+            while (child := parent.find('*')) is not None:
+                depth += 1
+                with self.subTest(xml_sample_index=sample_index, depth=depth):
+                    actual = xml.XmlHelper.get_parent_element(child)
+                    self.assertIs(parent, actual)
+                parent = child
+
     def test_reverse_find(self):
         for sample_index, sample in enumerate(XML_TEST_SAMPLES):
             desC_QPATH, anc_pred = sample.descendant_path_with_ancestor_predicate
             with self.subTest(xml_sample_index=sample_index, descendant_path=desC_QPATH, ancestor_predicate=anc_pred):
                 root = ET.fromstring(sample.xml, xml.XmlParser())
 
                 desc = root.find(desC_QPATH)
```

### Comparing `pawpaw-1.0.0a9/tests/test_xml_parser.py` & `pawpaw-1.0.0rc1/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/tests/util.py` & `pawpaw-1.0.0rc1/tests/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         <neighbor name="Colombia" direction="E"/>
     </country>
 </data>"""        
     ),
 
     XmlTestSample(
         source='https://docs.python.org/3/library/xml.etree.elementtree.html',
-        default_namespace='http://people.example.com',
+        default_namespace='{http://people.example.com}',
         root_prefix_map={'fictional': 'http://characters.example.com'},
         descendants_composite_prefix_map={},
         text_containing_descendant_path='.//{http://people.example.com}name',
         descendant_path_with_ancestor_predicate=('.//{http://characters.example.com}character', '{http://people.example.com}actor'),
         xml=
 """<?xml version="1.0"?>
 <actors xmlns:fictional="http://characters.example.com"
```

### Comparing `pawpaw-1.0.0a9/LICENSE` & `pawpaw-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/README.md` & `pawpaw-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 <!-- ![Pawpaw](svg/title.svg) -->
 
 # Pawpaw  [![High Performance Text Segmentation, Parsing, & Query][byline-img]][repo]
 
 Pawpaw is a high performance parsing & text segmentation framework that allows you to quickly and easily build complex, pipelined parsers.  Segments are automatically organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language called *plumule*.
 
-<img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png"> 
+<img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png" /> 
 
 - Indexed string and substring representation
   - Efficient memory utilization
   - Fast processing
   - Pythonic relative indexing and slicing
   - Runtime & polymorphic value extraction
   - Tree graphs for all indexed text
@@ -39,15 +39,15 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,100 unit tests and counting!
+  - Over 4,300 unit tests and counting!
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -273,45 +273,43 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- HISTORY & ROADMAP -->
 ## History & Roadmap
 
-Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in alpha, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
+Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in release-candidate status, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
 
 - [x] arborform
   - [x] itorator
     - [x] Desc
     - [x] Extract
     - [x] Reflect
     - [x] Split
     - [x] ValueFunc
   - [x] postorator
-    - [ ] StackedReduce
+    - [x] StackedReduce
     - [x] WindowedJoin
 - [x] core
   - [x] Errors
-  - [x] Furcation
   - [x] Infix
   - [x] Ito
   - [x] ItoChildren
   - [x] nuco
-  - [x] PredicatedValue
   - [x] Span
   - [x] Types
 - [ ] documentation & examples
 - [x] query
   - [x] radicle query engine
   - [x] plumule
 - [ ] nlp
-- [ ] visualization
+- [x] visualization
   - [x] ascibox
   - [x] highlighter
-  - [ ] pepo
+  - [x] pepo
   - [x] sgr
 - [x] xml
   - [x] XmlHelper
   - [x] XmlParser
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -22,15 +22,15 @@
 resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
 and Pawpaw datastructures in one go; with cross-linked nodes between trees -
 NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
 for downstream NLP consumption and b) *storing and searching* NLP generated
 content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
 Efficient pickling and JSON persistence - Security option enables persistence
 of index-only data, with reference strings re-injected during de-serialization
-- Stable & Defect Free - Over 4,100 unit tests and counting!
+- Stable & Defect Free - Over 4,300 unit tests and counting!
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -138,24 +138,24 @@
 Pawpaw, you can easily verify that it is installed correctly. Just open Python
 prompt and type: ```python >>> from pawpaw import Ito >>> Ito('Hello, World!')
 Ito('Hello, World!', 0, 13, None) ``` If your last line looks like this, you
 are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
-called *Ito*. Currently in alpha, many components and features are production
-ready. However, documentation is still being written and some newer features
-are still undergoing work. A rough outline of which components are finalized is
-as follows: - [x] arborform - [x] itorator - [x] Desc - [x] Extract - [x]
-Reflect - [x] Split - [x] ValueFunc - [x] postorator - [ ] StackedReduce - [x]
-WindowedJoin - [x] core - [x] Errors - [x] Furcation - [x] Infix - [x] Ito -
-[x] ItoChildren - [x] nuco - [x] PredicatedValue - [x] Span - [x] Types - [ ]
-documentation & examples - [x] query - [x] radicle query engine - [x] plumule -
-[ ] nlp - [ ] visualization - [x] ascibox - [x] highlighter - [ ] pepo - [x]
-sgr - [x] xml - [x] XmlHelper - [x] XmlParser
+called *Ito*. Currently in release-candidate status, many components and
+features are production ready. However, documentation is still being written
+and some newer features are still undergoing work. A rough outline of which
+components are finalized is as follows: - [x] arborform - [x] itorator - [x]
+Desc - [x] Extract - [x] Reflect - [x] Split - [x] ValueFunc - [x] postorator -
+[x] StackedReduce - [x] WindowedJoin - [x] core - [x] Errors - [x] Infix - [x]
+Ito - [x] ItoChildren - [x] nuco - [x] Span - [x] Types - [ ] documentation &
+examples - [x] query - [x] radicle query engine - [x] plumule - [ ] nlp - [x]
+visualization - [x] ascibox - [x] highlighter - [x] pepo - [x] sgr - [x] xml -
+[x] XmlHelper - [x] XmlParser
                                                                   (back_to_top)
  ## Contributing Contributions to Pawpaw are **greatly appreciated** - please
 refer to the [contributing guildelines](/contributing.md) for details.
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE](LICENSE) for more
 information.
                                                                   (back_to_top)
```

### Comparing `pawpaw-1.0.0a9/pyproject.toml` & `pawpaw-1.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a9/PKG-INFO` & `pawpaw-1.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawpaw
-Version: 1.0.0a9
+Version: 1.0.0rc1
 Summary: High Performance Text Processing & Segmentation Framework
 Project-URL: Homepage, https://github.com/rlayers/pawpaw
 Project-URL: Bug Tracker, https://github.com/rlayers/pawpaw/issues
 Author-email: "Robert L. Ayers" <rlayers@yahoo.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: extract-text,hierarchical-text-segmentation,information-extraction,knowledge-graph,nlp,python,text-processing,text-segmentation,xml-parser
@@ -34,15 +34,15 @@
 
 <!-- ![Pawpaw](svg/title.svg) -->
 
 # Pawpaw  [![High Performance Text Segmentation, Parsing, & Query][byline-img]][repo]
 
 Pawpaw is a high performance parsing & text segmentation framework that allows you to quickly and easily build complex, pipelined parsers.  Segments are automatically organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language called *plumule*.
 
-<img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png"> 
+<img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png" /> 
 
 - Indexed string and substring representation
   - Efficient memory utilization
   - Fast processing
   - Pythonic relative indexing and slicing
   - Runtime & polymorphic value extraction
   - Tree graphs for all indexed text
@@ -61,15 +61,15 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,100 unit tests and counting!
+  - Over 4,300 unit tests and counting!
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -295,45 +295,43 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- HISTORY & ROADMAP -->
 ## History & Roadmap
 
-Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in alpha, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
+Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in release-candidate status, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
 
 - [x] arborform
   - [x] itorator
     - [x] Desc
     - [x] Extract
     - [x] Reflect
     - [x] Split
     - [x] ValueFunc
   - [x] postorator
-    - [ ] StackedReduce
+    - [x] StackedReduce
     - [x] WindowedJoin
 - [x] core
   - [x] Errors
-  - [x] Furcation
   - [x] Infix
   - [x] Ito
   - [x] ItoChildren
   - [x] nuco
-  - [x] PredicatedValue
   - [x] Span
   - [x] Types
 - [ ] documentation & examples
 - [x] query
   - [x] radicle query engine
   - [x] plumule
 - [ ] nlp
-- [ ] visualization
+- [x] visualization
   - [x] ascibox
   - [x] highlighter
-  - [ ] pepo
+  - [x] pepo
   - [x] sgr
 - [x] xml
   - [x] XmlHelper
   - [x] XmlParser
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0a9 Summary: High Performance
+Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0rc1 Summary: High Performance
 Text Processing & Segmentation Framework Project-URL: Homepage, https://
 github.com/rlayers/pawpaw Project-URL: Bug Tracker, https://github.com/rlayers/
 pawpaw/issues Author-email: "Robert L. Ayers"
 yahoo.com> License-Expression: MIT License-File: LICENSE Keywords: extract-
 text,hierarchical-text-segmentation,information-extraction,knowledge-
 graph,nlp,python,text-processing,text-segmentation,xml-parser Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
@@ -35,15 +35,15 @@
 resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
 and Pawpaw datastructures in one go; with cross-linked nodes between trees -
 NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
 for downstream NLP consumption and b) *storing and searching* NLP generated
 content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
 Efficient pickling and JSON persistence - Security option enables persistence
 of index-only data, with reference strings re-injected during de-serialization
-- Stable & Defect Free - Over 4,100 unit tests and counting!
+- Stable & Defect Free - Over 4,300 unit tests and counting!
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -151,24 +151,24 @@
 Pawpaw, you can easily verify that it is installed correctly. Just open Python
 prompt and type: ```python >>> from pawpaw import Ito >>> Ito('Hello, World!')
 Ito('Hello, World!', 0, 13, None) ``` If your last line looks like this, you
 are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
-called *Ito*. Currently in alpha, many components and features are production
-ready. However, documentation is still being written and some newer features
-are still undergoing work. A rough outline of which components are finalized is
-as follows: - [x] arborform - [x] itorator - [x] Desc - [x] Extract - [x]
-Reflect - [x] Split - [x] ValueFunc - [x] postorator - [ ] StackedReduce - [x]
-WindowedJoin - [x] core - [x] Errors - [x] Furcation - [x] Infix - [x] Ito -
-[x] ItoChildren - [x] nuco - [x] PredicatedValue - [x] Span - [x] Types - [ ]
-documentation & examples - [x] query - [x] radicle query engine - [x] plumule -
-[ ] nlp - [ ] visualization - [x] ascibox - [x] highlighter - [ ] pepo - [x]
-sgr - [x] xml - [x] XmlHelper - [x] XmlParser
+called *Ito*. Currently in release-candidate status, many components and
+features are production ready. However, documentation is still being written
+and some newer features are still undergoing work. A rough outline of which
+components are finalized is as follows: - [x] arborform - [x] itorator - [x]
+Desc - [x] Extract - [x] Reflect - [x] Split - [x] ValueFunc - [x] postorator -
+[x] StackedReduce - [x] WindowedJoin - [x] core - [x] Errors - [x] Infix - [x]
+Ito - [x] ItoChildren - [x] nuco - [x] Span - [x] Types - [ ] documentation &
+examples - [x] query - [x] radicle query engine - [x] plumule - [ ] nlp - [x]
+visualization - [x] ascibox - [x] highlighter - [x] pepo - [x] sgr - [x] xml -
+[x] XmlHelper - [x] XmlParser
                                                                   (back_to_top)
  ## Contributing Contributions to Pawpaw are **greatly appreciated** - please
 refer to the [contributing guildelines](/contributing.md) for details.
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE](LICENSE) for more
 information.
                                                                   (back_to_top)
```

