# Comparing `tmp/pii_codex-0.4.3.tar.gz` & `tmp/pii_codex-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii_codex-0.4.3.tar", max compression
+gzip compressed data, was "pii_codex-0.4.4.tar", max compression
```

## Comparing `pii_codex-0.4.3.tar` & `pii_codex-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0     1522 2022-12-28 19:36:37.734170 pii_codex-0.4.3/LICENSE
--rw-r--r--   0        0        0    21913 2022-12-28 19:36:37.734170 pii_codex-0.4.3/LICENSE-ETHICS
--rw-r--r--   0        0        0     7333 2022-12-28 19:36:37.734170 pii_codex-0.4.3/README.md
--rw-r--r--   0        0        0       22 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/__init__.py
--rw-r--r--   0        0        0      185 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/config.py
--rw-r--r--   0        0        0     6019 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/data/v1/pii_type_mappings.csv
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/__init__.py
--rw-r--r--   0        0        0     4413 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/analysis.py
--rw-r--r--   0        0        0     2035 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/aws_pii.py
--rw-r--r--   0        0        0    21249 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/azure_pii.py
--rw-r--r--   0        0        0     3961 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/common.py
--rw-r--r--   0        0        0     1289 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/models/microsoft_presidio_pii.py
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/__init__.py
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/__init__.py
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/__init__.py
--rw-r--r--   0        0        0     3853 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
--rw-r--r--   0        0        0     1788 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
--rw-r--r--   0        0        0      766 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
--rw-r--r--   0        0        0     2011 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
--rw-r--r--   0        0        0    14870 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/analysis_service.py
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/analyzers/__init__.py
--rw-r--r--   0        0        0     8658 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/analyzers/presidio_analysis.py
--rw-r--r--   0        0        0     2744 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/services/assessment_service.py
--rw-r--r--   0        0        0        0 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/__init__.py
--rw-r--r--   0        0        0     4099 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/file_util.py
--rw-r--r--   0        0        0      460 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/logging.py
--rw-r--r--   0        0        0      157 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/package_installer_util.py
--rw-r--r--   0        0        0     6230 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/pii_mapping_util.py
--rw-r--r--   0        0        0     1248 2022-12-28 19:36:37.734170 pii_codex-0.4.3/pii_codex/utils/statistics_util.py
--rw-r--r--   0        0        0     2514 2022-12-28 19:36:37.738170 pii_codex-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8592 1970-01-01 00:00:00.000000 pii_codex-0.4.3/setup.py
--rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 pii_codex-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-04-25 01:18:04.404435 pii_codex-0.4.4/LICENSE
+-rw-r--r--   0        0        0     8623 2023-04-25 01:18:04.404435 pii_codex-0.4.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/config.py
+-rw-r--r--   0        0        0     6019 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/data/v1/pii_type_mappings.csv
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/__init__.py
+-rw-r--r--   0        0        0     4413 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/analysis.py
+-rw-r--r--   0        0        0     2035 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/aws_pii.py
+-rw-r--r--   0        0        0    21249 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/azure_pii.py
+-rw-r--r--   0        0        0     4031 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/common.py
+-rw-r--r--   0        0        0     1289 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/models/microsoft_presidio_pii.py
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/__init__.py
+-rw-r--r--   0        0        0     3853 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py
+-rw-r--r--   0        0        0     1702 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py
+-rw-r--r--   0        0        0      766 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py
+-rw-r--r--   0        0        0     2011 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py
+-rw-r--r--   0        0        0    14870 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analysis_service.py
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analyzers/__init__.py
+-rw-r--r--   0        0        0     8658 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/analyzers/presidio_analysis.py
+-rw-r--r--   0        0        0     2744 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/services/assessment_service.py
+-rw-r--r--   0        0        0        0 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/file_util.py
+-rw-r--r--   0        0        0      460 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/logging.py
+-rw-r--r--   0        0        0      157 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/package_installer_util.py
+-rw-r--r--   0        0        0     6300 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/pii_mapping_util.py
+-rw-r--r--   0        0        0     1248 2023-04-25 01:18:04.408435 pii_codex-0.4.4/pii_codex/utils/statistics_util.py
+-rw-r--r--   0        0        0     2486 2023-04-25 01:18:04.412435 pii_codex-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 pii_codex-0.4.4/PKG-INFO
```

### Comparing `pii_codex-0.4.3/LICENSE` & `pii_codex-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/README.md` & `pii_codex-0.4.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,48 +5,69 @@
 PII Detection, Categorization, and Severity Assessment
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/EdyVision/pii-codex/graphs/commit-activity)
 [![codecov](https://codecov.io/gh/EdyVision/pii-codex/branch/main/graph/badge.svg?token=QO7DNMP87X)](https://codecov.io/gh/EdyVision/pii-codex)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![License: Hippocratic 3.0](https://img.shields.io/badge/License-Hippocratic_3.0-green.svg)](https://firstdonoharm.dev)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![DOI](https://zenodo.org/badge/533554671.svg)](https://zenodo.org/badge/latestdoi/533554671)
 
 </div>
 
 ---
-The <em>PII Codex</em> project was built as a core part of an ongoing research effort in Personal Identifiable Information (PII) detection and risk assessment. There was a need to not only detect PII in text, but also identify its severity, associated categorizations in cybersecurity research and policy documentation, and provide a way for others in similar research efforts to reproduce or extend the research. PII Codex is a combination of systematic research, conceptual frameworks, third-party open source software, and cloud service provider integrations. The categorizations are directly influenced by the research of Milne et al. (2016) while the ranking is a result of category severities on the scale provided by Schwartz and Solove (2012) from Non-Identifiable, Semi-Identifiable, and Identifiable.
+The <em>PII Codex</em> project was built as a core part of an ongoing research effort in Personal Identifiable Information (PII) detection and risk assessment (to be publicly released later in 2023). There was a need to not only detect PII in text, but also identify its severity, associated categorizations in cybersecurity research and policy documentation, and provide a way for others in similar research efforts to reproduce or extend the research. PII Codex is a combination of systematic research, conceptual frameworks, third-party open source software, and cloud service provider integrations. The categorizations are directly influenced by the research of Milne et al. (2016) while the ranking is a result of category severities on the scale provided by Schwartz and Solove (2012) from Non-Identifiable, Semi-Identifiable, and Identifiable.
 
 The outputs of the primary PII Codex analysis and adapter functions are AnalysisResult or AnalysisResultSet objects that will provide a listing of detections, severities, mean risk scores for each string processed, and summary statistics on the analysis made. The final outputs do not contain the original texts but instead will provide where to find the detections should the end-user care for this information in their analysis.
 
+## Statement of Need
+
+The general knowledge base of identifiable data, the usage restrictions of this data, and the associated policies surrounding it have shifted drastically over the years. The tech industry has had to adjust to many policy changes regarding the tracking of individuals, the usage of data from online profiles and platforms, and the right to be forgotten entirely from a service or platform (GDPR). While the shift has provided data protections around the globe, the majority of technology users continue to have little to no control over their personal information with third-party data consumers (Trepte, 2020). 
+
+Understanding if identifiable data types exist in a data set can prevent accidental sharing of such data by allowing its detection in the first place and, in the case of this software package, present sanitized strings, the reasons to why the token was considered to be PII, and permit for the results to be publishable.
+
+## Potential Usages
+Potential usages include sanitizing of dataset strings (e.g. a collection of social media posts), presenting results to users for software examining their interactions (e.g. UX research on user-awareness in cybersecurity applications), etc.
+
 <hr/>
 
+## Running Locally
+This project uses Poetry. To run this project, install `poetry` and proceed to follow the instructions under `/docs/LOCAL_SETUP.md`.
+
+`Note: This project has only been tested with Ubuntu and MacOS.`
+
 ## Importing
+Before adding `pii-codex` on your project, download the spaCy `en_core_web_lg` model:
+
+```bash
+python3 -m spacy download en_core_web_lg
+```
+
+
 The repository releases are hosted on PyPi.
 
-Using pip:
+Using pip (must have latest pip version and running Python 3.9 or 3.10):
 
 ```bash
-pip3 install -i pii-codex
+pip install --upgrade pip
+pip install pii-codex
+pip install pii-codex[detections]
 ```
 
 Using Poetry:
 
 ```bash
+poetry update
 poetry add pii-codex
+poetry install pii-codex --extras="detections"
 ```
 
-If you are in need of the integrated Microsoft Presidio Analyzer, you'll also need to install the `en_core_web_lg` and the PII-Codex extras:
+For those using Google Collab, check out the example notebook:
 
-```bash
-poetry install pii-codex --extras="detections"
-python3 -m spacy download en_core_web_lg
-```
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/EdyVision/802ce21aab21eb5d9afa9e43d301eef7/pii-codex-sample-notebook.ipynb)
 
 ## Usage
 
 ### Sample Input / Output
 The built-in analyzer uses Microsoft Presidio. Feed in a collection of strings with analyze_collection() or just a single string with analyze_item(). Those analyzing a collection of strings will also be provided with statistics calculated on the risk scores for detected items.
 ```python
 from pii_codex.services.analysis_service import PIIAnalysisService
@@ -120,16 +141,9 @@
 | PII Type Mappings           | [PII Mappings](docs/MAPPING.md)                              | Overview of how to perform mappings between PII types and how to review store PII types. |
 | PII Detections and Analysis | [PII Detection and Analysis](docs/DETECTION_AND_ANALYSIS.md) | Overview of how to detect and analyze strings                                            |
 | Local Repo Setup            | [Local Repo Setup](docs/LOCAL_SETUP.md)                      | Instructions for local repository setup                                                  |
 | Example Analysis            | [Example Analysis Notebook](notebooks/pii-analysis-ms-presidio.ipynb)  | Notebook with example analysis using MSFT Presidio                             |
 
 <hr/>
 
-## Community Guidelines
-### Contributions
-In general, you can contribute to this project by creating issues. You are also welcome to contribute to the source code directly by forking the project, modifying the code, and creating pull requests. Please use clear and organized descriptions when creating issues and pull requests and leverage the templates when possible.
-
-### Bug Report and Support Requests
-You can use issues to report bugs and seek support. Before creating any new issues, please check for similar ones in the issue list first.
-
 ## Attributions
-This project benefited greatly from a number of PII research works like that from Milne et al (2016), Schwartz and Solove (2012), and the documentation by NIST, DHS, and HIPAA. A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy, Jupyter, and several others.
+This project benefited greatly from a number of PII research works like that from Milne et al (2016) with the definition of the types and categories, Schwartz and Solove (2012) with the severity levels of Non-Identifiable, Semi-Identifiable, and Identifiable, and the documentation by NIST, DHS (2012), and HIPAA. A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy (2017), Jupyter, and several others.
```

### Comparing `pii_codex-0.4.3/pii_codex/data/v1/pii_type_mappings.csv` & `pii_codex-0.4.4/pii_codex/data/v1/pii_type_mappings.csv`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/models/analysis.py` & `pii_codex-0.4.4/pii_codex/models/analysis.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/models/aws_pii.py` & `pii_codex-0.4.4/pii_codex/models/aws_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/models/azure_pii.py` & `pii_codex-0.4.4/pii_codex/models/azure_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/models/common.py` & `pii_codex-0.4.4/pii_codex/models/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class RiskLevel(Enum):
     LEVEL_ONE: int = 1  # Not-Identifiable
     LEVEL_TWO: int = 2  # Semi-Identifiable
     LEVEL_THREE: int = 3  # Identifiable
 
 
 class RiskLevelDefinition(Enum):
+    # Levels on the continuum presented by Schwartz and Solove (2011)
     LEVEL_ONE: str = "Non-Identifiable"  # Default if no entities were detected, risk level is set to this
     LEVEL_TWO: str = "Semi-Identifiable"
     LEVEL_THREE: str = "Identifiable"  # Level associated with Directly PII, PHI, and Standalone PII info types
 
 
 class MetadataType(Enum):
     SCREEN_NAME: str = "screen_name"
```

### Comparing `pii_codex-0.4.3/pii_codex/models/microsoft_presidio_pii.py` & `pii_codex-0.4.4/pii_codex/models/microsoft_presidio_pii.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py` & `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/aws_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py` & `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/azure_detection_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from typing import List
 
 from pii_codex.config import PII_MAPPER
 from pii_codex.models.analysis import DetectionResultItem, DetectionResult
 from pii_codex.services.adapters.detection_adapters.detection_adapter_base import (
     BasePIIDetectionAdapter,
 )
-from pii_codex.utils.pii_mapping_util import PIIMapper
 
 
 class AzurePIIDetectionAdapter(BasePIIDetectionAdapter):
-
-    pii_mapper = PIIMapper()
-
     def convert_analyzed_item(self, pii_detection: dict):
         """
         Converts a detection result into a collection of DetectionResultItem
 
         @param pii_detection: dict
         @return: List[DetectionResultItem]
         """
```

### Comparing `pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py` & `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/detection_adapter_base.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py` & `pii_codex-0.4.4/pii_codex/services/adapters/detection_adapters/presidio_detection_adapter.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/analysis_service.py` & `pii_codex-0.4.4/pii_codex/services/analysis_service.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/analyzers/presidio_analysis.py` & `pii_codex-0.4.4/pii_codex/services/analyzers/presidio_analysis.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/services/assessment_service.py` & `pii_codex-0.4.4/pii_codex/services/assessment_service.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/utils/file_util.py` & `pii_codex-0.4.4/pii_codex/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pii_codex/utils/pii_mapping_util.py` & `pii_codex-0.4.4/pii_codex/utils/pii_mapping_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class PIIMapper:
     def __init__(self):
         self._pii_mapping_data_frame = open_pii_type_mapping_csv("v1")
 
     def map_pii_type(self, pii_type: str) -> RiskAssessment:
         """
         Maps the PII Type to a full RiskAssessment including categories it belongs to, risk level, and
-        its location in the text.
+        its location in the text. This cross-references some of the types listed by Milne et al. (2016)
 
         @param pii_type:
         @return:
         """
 
         information_detail_lookup = self._pii_mapping_data_frame[
             self._pii_mapping_data_frame.PII_Type == pii_type
```

### Comparing `pii_codex-0.4.3/pii_codex/utils/statistics_util.py` & `pii_codex-0.4.4/pii_codex/utils/statistics_util.py`

 * *Files identical despite different names*

### Comparing `pii_codex-0.4.3/pyproject.toml` & `pii_codex-0.4.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "pii-codex"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Eidan J. Rosado"]
 license = "BSD 3-Clause"
 readme = "README.md"
 homepage = "https://github.com/EdyVision/pii-codex"
 repository = "https://github.com/EdyVision/pii-codex"
 keywords = ["PII", "PII topology", "risk categories", "personal identifiable information", "risk assessment"]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3", ]
-include = ["LICENSE", "LICENSE-ETHICS"]
+include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 dataclasses-json = "^0.5.7"
 pydantic = {extras = ["dotenv"], version = "^1.10.2"}
 pandas = "^1.4.4"
 pillow = "^9.3.0"  # security dependency
 
 # Optional items for analyses - users have the option to use the integrated Presidio analyzer or
 # avoid installing the following and bring their own detector, using the adapters
-spacy = { version = "^3.4.1", optional = true }
-presidio-analyzer = { version = "^2.2.31", optional = true }
-presidio-anonymizer = { version ="^2.2.31", optional = true }
+spacy = { version = "^3.5.2", optional = true }
+presidio-analyzer = { version = "^2.2.32", optional = true }
+presidio-anonymizer = { version ="^2.2.32", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 black = "22.12.0"
 pylint = "^2.15.4"
 mypy = "^0.982"
 coverage = "^6.4.4"
@@ -39,15 +39,15 @@
 matplotlib = "^3.6.1"
 ipykernel = "^6.16.0"
 jupyter = "^1.0.0"
 jupyter_core = "^4.11.2"
 importlib-resources = "^5.9.0"
 seaborn = "^0.12.0"
 pre-commit = "^2.20.0"
-en_core_web_lg = {url="https://github.com/explosion/spacy-models/releases/download/en_core_web_lg-3.4.0/en_core_web_lg-3.4.0.tar.gz#egg=en_core_web_lg"}
+en_core_web_lg = {url="https://github.com/explosion/spacy-models/releases/download/en_core_web_lg-3.5.0/en_core_web_lg-3.5.0.tar.gz#egg=en_core_web_lg"}
 
 [tool.poetry.extras]
 detections = [
     "spacy",
     "presidio-analyzer",
     "presidio-anonymizer"
 ]
@@ -79,9 +79,9 @@
 
 log_file = "pytest.log"
 log_file_level = "DEBUG"
 log_file_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_file_date_format = "%Y-%m-%d %H:%M:%S"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry>=1.0.0"]
+build-backend = "poetry.masonry.api"
```

### Comparing `pii_codex-0.4.3/setup.py` & `pii_codex-0.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,178 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['pii_codex',
- 'pii_codex.models',
- 'pii_codex.services',
- 'pii_codex.services.adapters',
- 'pii_codex.services.adapters.detection_adapters',
- 'pii_codex.services.analyzers',
- 'pii_codex.utils']
-
-package_data = \
-{'': ['*'], 'pii_codex': ['data/v1/*']}
-
-install_requires = \
-['dataclasses-json>=0.5.7,<0.6.0',
- 'pandas>=1.4.4,<2.0.0',
- 'pillow>=9.3.0,<10.0.0',
- 'pydantic[dotenv]>=1.10.2,<2.0.0']
-
-extras_require = \
-{'detections': ['spacy>=3.4.1,<4.0.0',
-                'presidio-analyzer>=2.2.31,<3.0.0',
-                'presidio-anonymizer>=2.2.31,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'pii-codex',
-    'version': '0.4.3',
-    'description': '',
-    'long_description': '<div align="center">\n\n![alt text](https://github.com/EdyVision/pii-codex/blob/main/docs/PII_Codex_Logo.svg?raw=true)\n\nPII Detection, Categorization, and Severity Assessment\n\n[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)\n![](https://img.shields.io/badge/code%20style-black-000000.svg)\n[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/EdyVision/pii-codex/graphs/commit-activity)\n[![codecov](https://codecov.io/gh/EdyVision/pii-codex/branch/main/graph/badge.svg?token=QO7DNMP87X)](https://codecov.io/gh/EdyVision/pii-codex)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n[![License: Hippocratic 3.0](https://img.shields.io/badge/License-Hippocratic_3.0-green.svg)](https://firstdonoharm.dev)\n[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)\n[![DOI](https://zenodo.org/badge/533554671.svg)](https://zenodo.org/badge/latestdoi/533554671)\n\n</div>\n\n---\nThe <em>PII Codex</em> project was built as a core part of an ongoing research effort in Personal Identifiable Information (PII) detection and risk assessment. There was a need to not only detect PII in text, but also identify its severity, associated categorizations in cybersecurity research and policy documentation, and provide a way for others in similar research efforts to reproduce or extend the research. PII Codex is a combination of systematic research, conceptual frameworks, third-party open source software, and cloud service provider integrations. The categorizations are directly influenced by the research of Milne et al. (2016) while the ranking is a result of category severities on the scale provided by Schwartz and Solove (2012) from Non-Identifiable, Semi-Identifiable, and Identifiable.\n\nThe outputs of the primary PII Codex analysis and adapter functions are AnalysisResult or AnalysisResultSet objects that will provide a listing of detections, severities, mean risk scores for each string processed, and summary statistics on the analysis made. The final outputs do not contain the original texts but instead will provide where to find the detections should the end-user care for this information in their analysis.\n\n<hr/>\n\n## Importing\nThe repository releases are hosted on PyPi.\n\nUsing pip:\n\n```bash\npip3 install -i pii-codex\n```\n\nUsing Poetry:\n\n```bash\npoetry add pii-codex\n```\n\nIf you are in need of the integrated Microsoft Presidio Analyzer, you\'ll also need to install the `en_core_web_lg` and the PII-Codex extras:\n\n```bash\npoetry install pii-codex --extras="detections"\npython3 -m spacy download en_core_web_lg\n```\n\n## Usage\n\n### Sample Input / Output\nThe built-in analyzer uses Microsoft Presidio. Feed in a collection of strings with analyze_collection() or just a single string with analyze_item(). Those analyzing a collection of strings will also be provided with statistics calculated on the risk scores for detected items.\n```python\nfrom pii_codex.services.analysis_service import PIIAnalysisService\nPIIAnalysisService().analyze_collection(\n    texts=["your collection of strings"],\n    language_code="en",\n    collection_name="Data Set Label", # Optional Labeling\n    collection_type="SAMPLE" # Defaults to POPULATION, used stats calculations\n)\n```\n\nYou can also pass in a `data` param (dataframe) instead of simple text array with a text column and a metadata column to be analyzed for those analyzing social media posts. Current metadata supported are `URL`, `LOCATION`, and `SCREEN_NAME`.\n\nSample output (results object converted to `dict` from notebook):\n```\n{\n    "collection_name": "PII Collection 1",\n    "collection_type": "POPULATION",\n    "analyses": [\n        {\n            "analysis": [\n                {\n                    "pii_type_detected": "PERSON",\n                    "risk_level": 3,\n                    "risk_level_definition": "Identifiable",\n                    "cluster_membership_type": "Financial Information",\n                    "hipaa_category": "Protected Health Information",\n                    "dhs_category": "Linkable",\n                    "nist_category": "Directly PII",\n                    "entity_type": "PERSON",\n                    "score": 0.85,\n                    "start": 21,\n                    "end": 24,\n                }\n            ],\n            "index": 0,\n            "risk_score_mean": 3,\n            "sanitized_text: "Hi! My name is <REDACTED>",\n        },\n        ...\n    ],\n    "detection_count": 5,\n    "risk_scores": [3, 2.6666666666666665, 1, 2, 1],\n    "risk_score_mean": 1.9333333333333333,\n    "risk_score_mode": 1,\n    "risk_score_median": 2,\n    "risk_score_standard_deviation": 0.8273115763993905,\n    "risk_score_variance": 0.6844444444444444,\n    "detected_pii_types": {\n        "LOCATION",\n        "EMAIL_ADDRESS",\n        "URL",\n        "PHONE_NUMBER",\n        "PERSON",\n    },\n    "detected_pii_type_frequencies": {\n        "PERSON": 1,\n        "EMAIL_ADDRESS": 1,\n        "PHONE_NUMBER": 1,\n        "URL": 1,\n        "LOCATION": 1,\n    },\n}\n```\n\n### Docs\nFor more information on usage, check out the respective documentation for guidance on using PII-Codex.\n\n| Topic                       | Document                                                     | Description                                                                              |\n|-----------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------|\n| PII Type Mappings           | [PII Mappings](docs/MAPPING.md)                              | Overview of how to perform mappings between PII types and how to review store PII types. |\n| PII Detections and Analysis | [PII Detection and Analysis](docs/DETECTION_AND_ANALYSIS.md) | Overview of how to detect and analyze strings                                            |\n| Local Repo Setup            | [Local Repo Setup](docs/LOCAL_SETUP.md)                      | Instructions for local repository setup                                                  |\n| Example Analysis            | [Example Analysis Notebook](notebooks/pii-analysis-ms-presidio.ipynb)  | Notebook with example analysis using MSFT Presidio                             |\n\n<hr/>\n\n## Community Guidelines\n### Contributions\nIn general, you can contribute to this project by creating issues. You are also welcome to contribute to the source code directly by forking the project, modifying the code, and creating pull requests. Please use clear and organized descriptions when creating issues and pull requests and leverage the templates when possible.\n\n### Bug Report and Support Requests\nYou can use issues to report bugs and seek support. Before creating any new issues, please check for similar ones in the issue list first.\n\n## Attributions\nThis project benefited greatly from a number of PII research works like that from Milne et al (2016), Schwartz and Solove (2012), and the documentation by NIST, DHS, and HIPAA. A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy, Jupyter, and several others.\n',
-    'author': 'Eidan J. Rosado',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/EdyVision/pii-codex',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<3.11',
+Metadata-Version: 2.1
+Name: pii-codex
+Version: 0.4.4
+Summary: 
+Home-page: https://github.com/EdyVision/pii-codex
+License: BSD 3-Clause
+Keywords: PII,PII topology,risk categories,personal identifiable information,risk assessment
+Author: Eidan J. Rosado
+Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: detections
+Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
+Requires-Dist: pandas (>=1.4.4,<2.0.0)
+Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: presidio-analyzer (>=2.2.32,<3.0.0) ; extra == "detections"
+Requires-Dist: presidio-anonymizer (>=2.2.32,<3.0.0) ; extra == "detections"
+Requires-Dist: pydantic[dotenv] (>=1.10.2,<2.0.0)
+Requires-Dist: spacy (>=3.5.2,<4.0.0) ; extra == "detections"
+Project-URL: Repository, https://github.com/EdyVision/pii-codex
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+![alt text](https://github.com/EdyVision/pii-codex/blob/main/docs/PII_Codex_Logo.svg?raw=true)
+
+PII Detection, Categorization, and Severity Assessment
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+![](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/EdyVision/pii-codex/graphs/commit-activity)
+[![codecov](https://codecov.io/gh/EdyVision/pii-codex/branch/main/graph/badge.svg?token=QO7DNMP87X)](https://codecov.io/gh/EdyVision/pii-codex)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![DOI](https://zenodo.org/badge/533554671.svg)](https://zenodo.org/badge/latestdoi/533554671)
+
+</div>
+
+---
+The <em>PII Codex</em> project was built as a core part of an ongoing research effort in Personal Identifiable Information (PII) detection and risk assessment (to be publicly released later in 2023). There was a need to not only detect PII in text, but also identify its severity, associated categorizations in cybersecurity research and policy documentation, and provide a way for others in similar research efforts to reproduce or extend the research. PII Codex is a combination of systematic research, conceptual frameworks, third-party open source software, and cloud service provider integrations. The categorizations are directly influenced by the research of Milne et al. (2016) while the ranking is a result of category severities on the scale provided by Schwartz and Solove (2012) from Non-Identifiable, Semi-Identifiable, and Identifiable.
+
+The outputs of the primary PII Codex analysis and adapter functions are AnalysisResult or AnalysisResultSet objects that will provide a listing of detections, severities, mean risk scores for each string processed, and summary statistics on the analysis made. The final outputs do not contain the original texts but instead will provide where to find the detections should the end-user care for this information in their analysis.
+
+## Statement of Need
+
+The general knowledge base of identifiable data, the usage restrictions of this data, and the associated policies surrounding it have shifted drastically over the years. The tech industry has had to adjust to many policy changes regarding the tracking of individuals, the usage of data from online profiles and platforms, and the right to be forgotten entirely from a service or platform (GDPR). While the shift has provided data protections around the globe, the majority of technology users continue to have little to no control over their personal information with third-party data consumers (Trepte, 2020). 
+
+Understanding if identifiable data types exist in a data set can prevent accidental sharing of such data by allowing its detection in the first place and, in the case of this software package, present sanitized strings, the reasons to why the token was considered to be PII, and permit for the results to be publishable.
+
+## Potential Usages
+Potential usages include sanitizing of dataset strings (e.g. a collection of social media posts), presenting results to users for software examining their interactions (e.g. UX research on user-awareness in cybersecurity applications), etc.
+
+<hr/>
+
+## Running Locally
+This project uses Poetry. To run this project, install `poetry` and proceed to follow the instructions under `/docs/LOCAL_SETUP.md`.
+
+`Note: This project has only been tested with Ubuntu and MacOS.`
+
+## Importing
+Before adding `pii-codex` on your project, download the spaCy `en_core_web_lg` model:
+
+```bash
+python3 -m spacy download en_core_web_lg
+```
+
+
+The repository releases are hosted on PyPi.
+
+Using pip (must have latest pip version and running Python 3.9 or 3.10):
+
+```bash
+pip install --upgrade pip
+pip install pii-codex
+pip install pii-codex[detections]
+```
+
+Using Poetry:
+
+```bash
+poetry update
+poetry add pii-codex
+poetry install pii-codex --extras="detections"
+```
+
+For those using Google Collab, check out the example notebook:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/EdyVision/802ce21aab21eb5d9afa9e43d301eef7/pii-codex-sample-notebook.ipynb)
+
+## Usage
+
+### Sample Input / Output
+The built-in analyzer uses Microsoft Presidio. Feed in a collection of strings with analyze_collection() or just a single string with analyze_item(). Those analyzing a collection of strings will also be provided with statistics calculated on the risk scores for detected items.
+```python
+from pii_codex.services.analysis_service import PIIAnalysisService
+PIIAnalysisService().analyze_collection(
+    texts=["your collection of strings"],
+    language_code="en",
+    collection_name="Data Set Label", # Optional Labeling
+    collection_type="SAMPLE" # Defaults to POPULATION, used stats calculations
+)
+```
+
+You can also pass in a `data` param (dataframe) instead of simple text array with a text column and a metadata column to be analyzed for those analyzing social media posts. Current metadata supported are `URL`, `LOCATION`, and `SCREEN_NAME`.
+
+Sample output (results object converted to `dict` from notebook):
+```
+{
+    "collection_name": "PII Collection 1",
+    "collection_type": "POPULATION",
+    "analyses": [
+        {
+            "analysis": [
+                {
+                    "pii_type_detected": "PERSON",
+                    "risk_level": 3,
+                    "risk_level_definition": "Identifiable",
+                    "cluster_membership_type": "Financial Information",
+                    "hipaa_category": "Protected Health Information",
+                    "dhs_category": "Linkable",
+                    "nist_category": "Directly PII",
+                    "entity_type": "PERSON",
+                    "score": 0.85,
+                    "start": 21,
+                    "end": 24,
+                }
+            ],
+            "index": 0,
+            "risk_score_mean": 3,
+            "sanitized_text: "Hi! My name is <REDACTED>",
+        },
+        ...
+    ],
+    "detection_count": 5,
+    "risk_scores": [3, 2.6666666666666665, 1, 2, 1],
+    "risk_score_mean": 1.9333333333333333,
+    "risk_score_mode": 1,
+    "risk_score_median": 2,
+    "risk_score_standard_deviation": 0.8273115763993905,
+    "risk_score_variance": 0.6844444444444444,
+    "detected_pii_types": {
+        "LOCATION",
+        "EMAIL_ADDRESS",
+        "URL",
+        "PHONE_NUMBER",
+        "PERSON",
+    },
+    "detected_pii_type_frequencies": {
+        "PERSON": 1,
+        "EMAIL_ADDRESS": 1,
+        "PHONE_NUMBER": 1,
+        "URL": 1,
+        "LOCATION": 1,
+    },
 }
+```
+
+### Docs
+For more information on usage, check out the respective documentation for guidance on using PII-Codex.
+
+| Topic                       | Document                                                     | Description                                                                              |
+|-----------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------|
+| PII Type Mappings           | [PII Mappings](docs/MAPPING.md)                              | Overview of how to perform mappings between PII types and how to review store PII types. |
+| PII Detections and Analysis | [PII Detection and Analysis](docs/DETECTION_AND_ANALYSIS.md) | Overview of how to detect and analyze strings                                            |
+| Local Repo Setup            | [Local Repo Setup](docs/LOCAL_SETUP.md)                      | Instructions for local repository setup                                                  |
+| Example Analysis            | [Example Analysis Notebook](notebooks/pii-analysis-ms-presidio.ipynb)  | Notebook with example analysis using MSFT Presidio                             |
+
+<hr/>
 
+## Attributions
+This project benefited greatly from a number of PII research works like that from Milne et al (2016) with the definition of the types and categories, Schwartz and Solove (2012) with the severity levels of Non-Identifiable, Semi-Identifiable, and Identifiable, and the documentation by NIST, DHS (2012), and HIPAA. A special thanks to all the open source projects, and frameworks that made the setup and structuring of this project much easier like Poetry, Microsoft Presidio, spaCy (2017), Jupyter, and several others.
 
-setup(**setup_kwargs)
```

