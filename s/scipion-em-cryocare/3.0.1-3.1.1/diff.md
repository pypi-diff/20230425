# Comparing `tmp/scipion-em-cryocare-3.0.1.tar.gz` & `tmp/scipion-em-cryocare-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryocare-3.0.1.tar", last modified: Thu Jul  1 09:34:05 2021, max compression
+gzip compressed data, was "scipion-em-cryocare-3.1.1.tar", last modified: Tue Apr 25 08:38:15 2023, max compression
```

## Comparing `scipion-em-cryocare-3.0.1.tar` & `scipion-em-cryocare-3.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:34:05.928614 scipion-em-cryocare-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-07-01 09:34:05.928614 scipion-em-cryocare-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:34:05.920613 scipion-em-cryocare-3.0.1/cryocare/
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    25792 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:34:05.924614 scipion-em-cryocare-3.0.1/cryocare/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_load_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     8283 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_prepare_training_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7855 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_training.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:34:05.924614 scipion-em-cryocare-3.0.1/cryocare/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6381 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/tests/test_cryoCARE_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/cryocare/wizards.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:34:05.928614 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      763 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 09:34:05.000000 scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-01 09:34:05.928614 scipion-em-cryocare-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-07-01 09:28:21.000000 scipion-em-cryocare-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:15.318986 scipion-em-cryocare-3.1.1/cryocare/
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/cryocare/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_prepare_training_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/cryocare/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/tests/test_cryoCARE_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/cryocare/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 08:38:15.000000 scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:38:15.322986 scipion-em-cryocare-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 08:36:25.000000 scipion-em-cryocare-3.1.1/setup.py
```

### Comparing `scipion-em-cryocare-3.0.1/LICENSE` & `scipion-em-cryocare-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-3.0.1/cryocare/__init__.py` & `scipion-em-cryocare-3.1.1/cryocare/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 import pwem
 import os
 from pyworkflow.utils import Environ
 from cryocare.constants import CRYOCARE_ENV_ACTIVATION, DEFAULT_ACTIVATION_CMD, CRYOCARE_ENV_NAME, \
     CRYOCARE_DEFAULT_VERSION, CRYOCARE_HOME, CRYOCARE_CUDA_LIB, CRYOCARE
 
 _logo = "icon.png"
-_references = ['buchholz2019cryo', 'buchholz2019content']
-__version__ = "3.0.1"
+_references = ['buchholz2019cryo']
+__version__ = "3.1.1"
 
 
 class Plugin(pwem.Plugin):
-
     _homeVar = CRYOCARE_HOME
     _url = 'https://github.com/scipion-em/scipion-em-cryocare'
 
     @classmethod
     def _defineVariables(cls):
         # cryoCARE does NOT need EmVar because it uses a conda environment.
         cls._defineVar(CRYOCARE_ENV_ACTIVATION, DEFAULT_ACTIVATION_CMD)
+        cls._defineVar(CRYOCARE_CUDA_LIB, pwem.Config.CUDA_LIB)
 
     @classmethod
     def getCryocareEnvActivation(cls):
         return cls.getVar(CRYOCARE_ENV_ACTIVATION)
 
     @classmethod
     def getEnviron(cls, gpuId='0'):
@@ -62,36 +62,31 @@
         cudaLib = environ.get(CRYOCARE_CUDA_LIB, pwem.Config.CUDA_LIB)
         environ.addLibrary(cudaLib)
         return environ
 
     @classmethod
     def defineBinaries(cls, env):
         CRYOCARE_INSTALLED = '%s_%s_installed' % (CRYOCARE, CRYOCARE_DEFAULT_VERSION)
-
-        # try to get CONDA activation command
         installationCmd = cls.getCondaActivationCmd()
-
+        # try to get CONDA activation command
         # Create the environment
-        installationCmd += 'conda create -y -n %s -c conda-forge -c anaconda python=3.8 ' \
-                           'cudnn=7.6.5=cuda10.1_0 && ' % CRYOCARE_ENV_NAME
+        installationCmd += 'conda create -y -n %s python=3.8 cudatoolkit=11.0 cudnn=8.0 -c conda-forge && ' % CRYOCARE_ENV_NAME
+        # 'keras-gpu=2.3.1 ' \
 
         # Activate new the environment
         installationCmd += 'conda activate %s && ' % CRYOCARE_ENV_NAME
 
-        # Install non-conda required packages
-        installationCmd += 'pip install tensorflow-gpu==2.3.3 && '
-        installationCmd += 'pip install mrcfile && '
-        installationCmd += 'pip install csbdeep '
-        # I had the same issue and was able to fix this by setting h5py < 3.0.0.
-        # Looks like here was a 3.0 release of h5py recently where they changed how strings are stored/read.
-        # https://github.com/keras-team/keras/issues/14265
+        # Install the rest of dependencies
 
-        # Install cryoCARE
-        installationCmd += 'pip install %s==%s &&' % (CRYOCARE, CRYOCARE_DEFAULT_VERSION)
+        installationCmd += 'pip install tensorflow==2.4.0 && '
+        installationCmd += 'pip install matplotlib==3.6.3 && '
 
+        # Install cryoCARE
+        installationCmd += 'pip install %s==%s && ' % (CRYOCARE, CRYOCARE_DEFAULT_VERSION)
+        
         # Flag installation finished
         installationCmd += 'touch %s' % CRYOCARE_INSTALLED
 
         cryocare_commands = [(installationCmd, CRYOCARE_INSTALLED)]
 
         envPath = os.environ.get('PATH', "")  # keep path since conda likely in there
         installEnvVars = {'PATH': envPath} if envPath else None
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/bibtex.py` & `scipion-em-cryocare-3.1.1/cryocare/bibtex.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,20 +32,8 @@
   booktitle = "2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019)",
   pages = "502--506",
   year = "2019",
   organization = "IEEE",
   doi = "http://doi.org/10.1109/ISBI.2019.8759519",
   url = "https://ieeexplore.ieee.org/document/87595192",
 }
-
-@article{buchholz2019content,
-  title = "Content-aware image restoration for electron microscopy.",
-  author = "Buchholz, Tim-Oliver and Krull, Alexander and Shahidi, R{\'e}za and Pigino, Gaia and J{\'e}kely, G{\'a}sp{\'a}r and Jug, Florian",
-  journal = "Methods in cell biology",
-  volume = "152",
-  pages = "277--289",
-  year = "2019",
-  publisher = "Cornell University",
-  url = "http://arxiv.org/abs/1810.05420",
-  doi = "http://arxiv.org/abs/1810.05420",
-}
 """
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/constants.py` & `scipion-em-cryocare-3.1.1/cryocare/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'you@yourinstitution.email'
 # *
 # **************************************************************************
 
 CRYOCARE_HOME = 'CRYOCARE_HOME'
-V0_1_1 = '0.1.1'
-CRYOCARE_DEFAULT_VERSION = V0_1_1
+V0_2_2 = '0.2.2'
+CRYOCARE_DEFAULT_VERSION = V0_2_2
 CRYOCARE = 'cryoCARE'
 CRYOCARE_ENV_NAME = '%s-%s' % (CRYOCARE, CRYOCARE_DEFAULT_VERSION)
 CRYOCARE_ENV_ACTIVATION = 'CRYOCARE_ENV_ACTIVATION'
 DEFAULT_ACTIVATION_CMD = 'conda activate %s' % CRYOCARE_ENV_NAME
 CRYOCARE_CUDA_LIB = 'CRYOCARE_CUDA_LIB'
 
 TRAIN_DATA_DIR = 'train_data'
 TRAIN_DATA_FN = 'train_data.npz'
 VALIDATION_DATA_FN = 'val_data.npz'
 MEAN_STD_FN = 'mean_std.npz'
 TRAIN_DATA_CONFIG = 'training_data_config'
 CRYOCARE_MODEL = 'cryoCARE_model'
+CRYOCARE_MODEL_TGZ = CRYOCARE_MODEL + '.tar.gz'
 PREDICT_CONFIG = 'predict_config'
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/icon.png` & `scipion-em-cryocare-3.1.1/cryocare/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-3.0.1/cryocare/objects.py` & `scipion-em-cryocare-3.1.1/cryocare/objects.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from os.path import join
 
 import pyworkflow.object as pwobj
+from cryocare.constants import CRYOCARE_MODEL
 from pwem import EMObject
 
 
 class CryocareTrainData(EMObject):
     def __init__(self, train_data_dir=None, patch_size=None, **kwargs):
         EMObject.__init__(self, **kwargs)
         self._train_data_dir = pwobj.String(train_data_dir)
@@ -16,20 +18,20 @@
         return self._patch_size.get()
 
     def __str__(self):
         return "CryoCARE Train Data (path=%s)" % self.getTrainDataDir()
 
 
 class CryocareModel(EMObject):
-    def __init__(self, basedir=None, train_data_dir=None, **kwargs):
+    def __init__(self, model_file=None, train_data_dir=None, **kwargs):
         EMObject.__init__(self, **kwargs)
-        self._basedir = pwobj.String(basedir)
+        self._model_file = pwobj.String(model_file)
         self._train_data_dir = pwobj.String(train_data_dir)
 
     def getPath(self):
-        return self._basedir.get()
+        return self._model_file.get()
 
     def getTrainDataDir(self):
         return self._train_data_dir.get()
 
     def __str__(self):
         return "CryoCARE Model (path=%s)" % self.getPath()
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/protocols/__init__.py` & `scipion-em-cryocare-3.1.1/cryocare/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_load_model.py` & `scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_load_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-import glob
+from enum import Enum
 from os.path import exists, join
 
+from cryocare.utils import makeDatasetSymLinks, getModelName
 from pwem.protocols import EMProtocol
 from pyworkflow import BETA
 from pyworkflow.protocol import PathParam, FileParam
 from pyworkflow.utils import Message, createLink
 
-from cryocare.constants import TRAIN_DATA_FN, VALIDATION_DATA_FN, CRYOCARE_MODEL
+from cryocare.constants import TRAIN_DATA_FN, VALIDATION_DATA_FN
 from cryocare.objects import CryocareModel
-from cryocare.utils import makeDatasetSymLinks
+
+
+class outputObjects(Enum):
+    model = CryocareModel
 
 
 class ProtCryoCARELoadModel(EMProtocol):
-    """Use two data-independent reconstructed tomograms to train a 3D cryo-CARE network."""
+    """Load a previously trained model."""
 
-    _label = 'CryoCARE Load Model'
+    _label = 'CryoCARE Load Trained Model'
     _devStatus = BETA
+    _possibleOutputs = outputObjects
 
     # -------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         """ Define the input parameters that will be used.
         Params:
             form: this is the form to be populated with sections and params.
         """
         # You need a params to belong to a section:
         form.addSection(label=Message.LABEL_INPUT)
-        form.addParam('basedir', PathParam,
-                      label='Base directory of the trained cryoCARE model',
+        form.addParam('trainDataModel', PathParam,
+                      label='Pre-trained cryoCARE model (.tar.gz)',
                       important=True,
                       allowsNull=False,
-                      help='It must contain a model in .h5 format.')
+                      help='It is a .tar.gz file containing a folder that contains, in turn, the following files:\n\n'
+                           '\t- config.json\n'
+                           '\t- history.dat\n'
+                           '\t- norm.json\n'
+                           '\t- weights_best.h5\n'
+                           '\t- weights_last.h5\n')
         form.addParam('trainDataDir', FileParam,
                       label='Directory of the prepared data for training',
                       important=True,
                       allowsNull=False,
                       help='It must contain two files: train_data.npz and val_data.npz, generated when '
                            'preparing the training data.')
 
@@ -42,27 +52,25 @@
         self._insertFunctionStep(self.createOutputStep)
 
     def _initialize(self):
         # The prediction is expecting the training and validation datasets to be in the same place as the training
         # model, but they are located in the training data generation extra directory. Hence, a symbolic link will
         # be created
         makeDatasetSymLinks(self, self.trainDataDir.get())
-        createLink(join('..', self.basedir.get()), self._getExtraPath(CRYOCARE_MODEL))
+        createLink(join(self.trainDataModel.get()), getModelName(self))
 
     def createOutputStep(self):
-        model = CryocareModel(basedir=self._getExtraPath(), train_data_dir=self._getExtraPath())
-        self._defineOutputs(model=model)
+        model = CryocareModel(model_file=getModelName(self), train_data_dir=self._getExtraPath())
+        self._defineOutputs(**{outputObjects.model.name: model})
 
     # --------------------------- INFO functions -----------------------------------
     def _validate(self):
         errors = []
-        if not exists(self.basedir.get()):
-            errors.append('Training model base directory does not exists.')
-        elif not glob.glob(join(self.basedir.get(), '*.h5')):
-            errors.append('No model files were found in the introduced training model base directory.')
+        if not exists(self.trainDataModel.get()):
+            errors.append('Training model introduced does not exists.')
 
         if not exists(self.trainDataDir.get()):
             errors.append('Directory of the prepared data for training does not exists.')
         else:
             if not exists(join(self.trainDataDir.get(), TRAIN_DATA_FN)):
                 errors.append('No %s file was found in the introduced training model base directory.' 
                               % TRAIN_DATA_FN)
@@ -71,9 +79,10 @@
                               % VALIDATION_DATA_FN)
         return errors
 
     def _summary(self):
         summary = []
 
         if self.isFinished():
-            summary.append("Loaded training model_dir = *%s*" % self.basedir.get())
+            summary.append("Loaded training model_dir = *%s*" % self.trainDataModel.get())
         return summary
+
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_prepare_training_data.py` & `scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_prepare_training_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import glob
 import json
+from enum import Enum
 from os.path import join
 import numpy as np
 
+from cryocare.utils import checkInputTomoSetsSize
 from pwem.protocols import EMProtocol
 from pyworkflow import BETA
 from pyworkflow.protocol import params, IntParam, FloatParam, Positive, LT, GT, LEVEL_ADVANCED, EnumParam
 from pyworkflow.utils import Message, makePath, moveFile
 from scipion.constants import PYTHON
 
 from cryocare import Plugin
 from cryocare.constants import TRAIN_DATA_DIR, TRAIN_DATA_FN, TRAIN_DATA_CONFIG, VALIDATION_DATA_FN
 from cryocare.objects import CryocareTrainData
-from cryocare.utils import CryocareUtils as ccutils
 
 # Tilt axis values
 X_AXIS = 0
 Y_AXIS = 1
 Z_AXIS = 2
 X_AXIS_LABEL = 'X'
 Y_AXIS_LABEL = 'Y'
 Z_AXIS_LABEL = 'Z'
 
 
+class outputObjects(Enum):
+    train_data = CryocareTrainData
+
+
 class ProtCryoCAREPrepareTrainingData(EMProtocol):
     """Operate the data to make it be expressed as expected by cryoCARE net."""
 
-    _label = 'CryoCARE Training Data Extraction'
+    _label = 'CryoCARE Generate Training Data'
     _devStatus = BETA
     _configFile = None
+    _possibleOutputs = outputObjects
 
     # -------------------------- DEFINE param functions ----------------------
 
     def _defineParams(self, form):
         """ Define the input parameters that will be used.
         Params:
             form: this is the form to be populated with sections and params.
@@ -97,15 +103,14 @@
     def _insertAllSteps(self):
         self._initialize()
         self._insertFunctionStep(self.prepareTrainingDataStep)
         self._insertFunctionStep(self.runDataExtraction)
         self._insertFunctionStep(self.createOutputStep)
 
     def _initialize(self):
-        makePath(self._getTrainDataDir())
         makePath(self._getTrainDataConfDir())
         self._configFile = join(self._getTrainDataConfDir(), TRAIN_DATA_CONFIG)
 
     def prepareTrainingDataStep(self):
         config = {
             'even': self._getListOfTomoNames(self.evenTomos.get()),
             'odd': self._getListOfTomoNames(self.oddTomos.get()),
@@ -122,15 +127,17 @@
     def runDataExtraction(self):
         Plugin.runCryocare(self, PYTHON, '$(which cryoCARE_extract_train_data.py) --conf %s' % self._configFile)
 
     def createOutputStep(self):
         # Generate a train data object containing the resulting data
         train_data = CryocareTrainData(train_data_dir=self._getTrainDataDir(),
                                        patch_size=self.patch_shape.get())
-        self._defineOutputs(train_data=train_data)
+        self._defineOutputs(**{outputObjects.train_data.name: train_data})
+        self._defineSourceRelation(self.evenTomos.get(), train_data)
+        self._defineSourceRelation(self.oddTomos.get(), train_data)
 
     # --------------------------- INFO functions -----------------------------------
     def _summary(self):
         summary = []
 
         if self.isFinished():
             summary.append("Generated training data info:\n"
@@ -140,22 +147,33 @@
                             self._getTrainDataFile(),
                             self._getValidationDataFile(),
                             self.patch_shape.get()))
         return summary
 
     def _validate(self):
         validateMsgs = []
-
-        msg = ccutils.checkInputTomoSetsSize(self.evenTomos.get(), self.oddTomos.get())
+        sideLength = self.patch_shape.get()
+        evenTomos = self.evenTomos.get()
+        oddTomos = self.oddTomos.get()
+        xe, ye, ze = evenTomos.getDimensions()
+        xo, yo, zo = oddTomos.getDimensions()
+        # Check the length and the dimensions of the sets introduced
+        msg = checkInputTomoSetsSize(evenTomos, oddTomos)
         if msg:
-            validateMsgs.append()
-
-        if self.patch_shape.get() % 2 != 0:
+            validateMsgs.append(msg)
+        # Check the patch conditions
+        if sideLength % 2 != 0:
             validateMsgs.append('Patch shape has to be an even number.')
-
+        for idim in [xe, ye, ze, xo, yo, zo]:
+            if idim <= 2 * sideLength:
+                validateMsgs.append('X, Y and Z dimensions of the tomograms introduced must satisfy the '
+                                    'condition\n\n*dimension > 2 x SideLength*\n\n'
+                                    '(X, Y, Z) = (%i, %i, %i)\n'
+                                    'SideLength = %i\n\n' % (xe, ye, ze, sideLength))
+                break
         return validateMsgs
 
     # --------------------------- UTIL functions -----------------------------------
     @staticmethod
     def _combineTrainDataFiles(pattern, outputFile):
         files = glob.glob(pattern)
         if len(files) == 1:
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/protocols/protocol_training.py` & `scipion-em-cryocare-3.1.1/cryocare/protocols/protocol_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import json
 import operator
+from enum import Enum
 
+from cryocare.utils import makeDatasetSymLinks, getModelName
 from pwem.protocols import EMProtocol
 from pyworkflow import BETA
 from pyworkflow.protocol import IntParam, PointerParam, FloatParam, params, GT, LEVEL_ADVANCED, GE, Positive
 from pyworkflow.utils import Message
 from scipion.constants import PYTHON
-
 from cryocare import Plugin
 from cryocare.constants import CRYOCARE_MODEL
 from cryocare.objects import CryocareModel
-from cryocare.utils import makeDatasetSymLinks
+
+
+class outputObjects(Enum):
+    model = CryocareModel
 
 
 class ProtCryoCARETraining(EMProtocol):
-    """Use two data-independent reconstructed tomograms to train a 3D cryo-CARE network."""
+    """Use two data-independent reconstructed tomograms to train a 3D cryoCARE network."""
 
     _label = 'CryoCARE Training'
     _devStatus = BETA
+    _possibleOutputs = outputObjects
     _configPath = None
 
     # -------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         """ Define the input parameters that will be used.
         Params:
             form: this is the form to be populated with sections and params.
@@ -124,17 +129,18 @@
             json.dump(config, f, indent=2)
 
     def trainingStep(self):
         Plugin.runCryocare(self, PYTHON, '$(which cryoCARE_train.py) --conf {}'.format(self._configPath),
                            gpuId=getattr(self, params.GPU_LIST).get())
 
     def createOutputStep(self):
-        model = CryocareModel(basedir=self._getExtraPath(),
+        model = CryocareModel(model_file=getModelName(self),
                               train_data_dir=self._getPreparedTrainingDataDir())
-        self._defineOutputs(model=model)
+        self._defineOutputs(**{outputObjects.model.name: model})
+        self._defineSourceRelation(self.train_data.get(), model)
 
     # --------------------------- INFO functions -----------------------------------
     def _summary(self):
         summary = []
 
         if self.isFinished():
             summary.append("Generated training model in location: *%s*" % self._getExtraPath(CRYOCARE_MODEL))
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/protocols.conf` & `scipion-em-cryocare-3.1.1/cryocare/protocols.conf`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [PROTOCOLS]
 Tomography = [
-    {"tag": "section", "text": "Imports", "children": [
-        {"tag": "protocol", "value": "ProtCryoCARELoadModel", "text": "cryocare - import training model"}
-    ]},
-	{"tag": "section", "text": "Postprocessing", "children": [
-        {"tag": "protocol_group", "text": "Denoise", "openItem": "False", "children": [
-            {"tag": "protocol", "value": "ProtCryoCAREPrepareTrainingData", "text": "cryocare - prepare training data"},
-            {"tag": "protocol", "value": "ProtCryoCARETraining", "text": "cryocare - training"},
-            {"tag": "protocol", "value": "ProtCryoCAREPrediction", "text": "cryocare - predict"}
+	{"tag": "section", "text": "Imports", "children": [
+            {"tag": "protocol", "value": "ProtCryoCARELoadModel", "text": "cryocare - import training model"}
+        ]},
+	{"tag": "section", "text": "Tomograms", "children": [
+            {"tag": "protocol_group", "text": "Denoise", "openItem": "False", "children": [
+                {"tag": "protocol", "value": "ProtCryoCAREPrepareTrainingData", "text": "cryocare - prepare training data"},
+                {"tag": "protocol", "value": "ProtCryoCARETraining", "text": "cryocare - training"},
+                {"tag": "protocol", "value": "ProtCryoCAREPrediction", "text": "cryocare - predict"}
+            ]}
         ]}
-	]}
- ]
+ ]
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/tests/test_cryoCARE_workflow.py` & `scipion-em-cryocare-3.1.1/cryocare/tests/test_cryoCARE_workflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,119 @@
+# **************************************************************************
+# *
+# * Authors:     Scipion Team
+# *
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# *
+# * This program is free software; you can redistribute it and/or modify
+# * it under the terms of the GNU General Public License as published by
+# * the Free Software Foundation; either version 2 of the License, or
+# * (at your option) any later version.
+# *
+# * This program is distributed in the hope that it will be useful,
+# * but WITHOUT ANY WARRANTY; without even the implied warranty of
+# * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# * GNU General Public License for more details.
+# *
+# * You should have received a copy of the GNU General Public License
+# * along with this program; if not, write to the Free Software
+# * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
+# * 02111-1307  USA
+# *
+# *  All comments concerning this program package may be sent to the
+# *  e-mail address 'scipion@cnb.csic.es'
+# *
+# **************************************************************************
+
 from os.path import exists
-from pyworkflow.tests import BaseTest, setupTestProject
-import tomo.protocols
+from cryocare.tests import CRYOCARE, DataSetCryoCARE
+from pyworkflow.tests import BaseTest, setupTestProject, DataSet
 from pyworkflow.utils import magentaStr
-
-from . import DataSet
-from ..constants import TRAIN_DATA_FN, TRAIN_DATA_CONFIG, TRAIN_DATA_DIR, VALIDATION_DATA_FN, CRYOCARE_MODEL
-from ..objects import CryocareTrainData, CryocareModel
-from ..protocols import ProtCryoCAREPrediction, ProtCryoCAREPrepareTrainingData, ProtCryoCARELoadModel, \
-    ProtCryoCARETraining
+from tomo.protocols import ProtImportTomograms
+from cryocare.protocols.protocol_prepare_training_data import outputObjects as prepTrainDataOutputs, \
+    ProtCryoCAREPrepareTrainingData
+from cryocare.protocols.protocol_load_model import outputObjects as loadTrainingModelOutputs, ProtCryoCARELoadModel
+from cryocare.protocols.protocol_training import outputObjects as trainOutputs, ProtCryoCARETraining
+from cryocare.protocols.protocol_predict import outputObjects as predictOutputs, ProtCryoCAREPrediction
+from cryocare.constants import TRAIN_DATA_FN, TRAIN_DATA_CONFIG, TRAIN_DATA_DIR, VALIDATION_DATA_FN, CRYOCARE_MODEL_TGZ
+from cryocare.objects import CryocareTrainData, CryocareModel
 
 
 class TestCryoCARE(BaseTest):
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet('cryocare')
-        cls.sRate = 2.355
+        cls.dataset = DataSet.getDataSet(CRYOCARE)
+        cls.sRate = 4.71
 
     def _runImportTomograms(self, tomoFile, mode):
         print(magentaStr("\n==> Importing the %s tomograms:" % mode))
-        protImport = self.newProtocol(
-            tomo.protocols.ProtImportTomograms,
-            filesPath=self.dataset.getFile(tomoFile),
-            samplingRate=self.sRate)
+        protImport = self.newProtocol(ProtImportTomograms,
+                                      filesPath=self.dataset.getFile(tomoFile),
+                                      samplingRate=self.sRate)
+        protImport.setObjLabel('Import %s tomograms' % mode)
         self.launchProtocol(protImport)
-        output = getattr(protImport, 'outputTomograms', None)
+        output = getattr(protImport, 'Tomograms', None)
         self.assertSetSize(output, size=1)
         return protImport
 
     def _runPrepareTrainingData(self, protImportEven, protImportOdd):
         print(magentaStr("\n==> Preparing the training data:"))
+        patchSize = 40
         protPrepTrainingData = self.newProtocol(ProtCryoCAREPrepareTrainingData,
-                                                evenTomos=protImportEven.outputTomograms,
-                                                oddTomos=protImportOdd.outputTomograms)
+                                                evenTomos=protImportEven.Tomograms,
+                                                oddTomos=protImportOdd.Tomograms,
+                                                patch_shape=patchSize,
+                                                num_slices=400,
+                                                n_normalization_samples=60)
         self.launchProtocol(protPrepTrainingData)
-        cryoCareTrainData = getattr(protPrepTrainingData, 'train_data', None)
+        cryoCareTrainData = getattr(protPrepTrainingData, prepTrainDataOutputs.train_data.name, None)
 
         # Check generated object
         self.assertEqual(type(cryoCareTrainData), CryocareTrainData)
         self.assertEqual(cryoCareTrainData.getTrainDataDir(), protPrepTrainingData._getExtraPath(TRAIN_DATA_DIR))
-        self.assertEqual(cryoCareTrainData.getPatchSize(), 72)
+        self.assertEqual(cryoCareTrainData.getPatchSize(), patchSize)
         # Check files generated
         self.assertTrue(exists(protPrepTrainingData._getExtraPath(TRAIN_DATA_DIR, TRAIN_DATA_FN)))
         self.assertTrue(exists(protPrepTrainingData._getExtraPath(TRAIN_DATA_DIR, VALIDATION_DATA_FN)))
         self.assertTrue(exists(protPrepTrainingData._getExtraPath(TRAIN_DATA_CONFIG, TRAIN_DATA_CONFIG)))
 
         return protPrepTrainingData
 
     def _runTrainingData(self, protPrepTrainingData):
-        # # Skipped because of it long execution time. Generated model was stored as part of the test
-        # # dataset and imported in the prediction test
-        # print(magentaStr("\n==> Skipping training due to its long execution time"))
-        # return []
         print(magentaStr("\n==> Training"))
         protTraining = self.newProtocol(ProtCryoCARETraining,
                                         train_data=getattr(protPrepTrainingData, 'train_data', None),
-                                        batch_size=8)
+                                        epochs=2,
+                                        steps_per_epoch=10)
 
         self.launchProtocol(protTraining)
-        cryoCareModel = getattr(protTraining, 'model', None)
+        cryoCareModel = getattr(protTraining, trainOutputs.model.name, None)
         # Check generated model
         self.assertEqual(type(cryoCareModel), CryocareModel)
-        self.assertEqual(cryoCareModel.getPath(), protTraining._getExtraPath())
+        self.assertEqual(cryoCareModel.getPath(), protTraining._getExtraPath(CRYOCARE_MODEL_TGZ))
         self.assertEqual(cryoCareModel.getTrainDataDir(), protPrepTrainingData._getExtraPath(TRAIN_DATA_DIR))
         # Check files and links generated
         self.assertTrue(exists(protTraining._getExtraPath('train_config.json')))
         self.assertTrue(exists(protTraining._getExtraPath(TRAIN_DATA_FN)))
         self.assertTrue(exists(protTraining._getExtraPath(VALIDATION_DATA_FN)))
-        self.assertTrue(exists(protTraining._getExtraPath(CRYOCARE_MODEL, 'config.json')))
-        self.assertTrue(exists(protTraining._getExtraPath(CRYOCARE_MODEL, 'weights_best.h5')))
-        self.assertTrue(exists(protTraining._getExtraPath(CRYOCARE_MODEL, 'weights_last.h5')))
+        self.assertTrue(exists(protTraining._getExtraPath(CRYOCARE_MODEL_TGZ)))
         return protTraining
 
     def _runLoadTrainingModel(self):
         print(magentaStr("\n==> Loading a pre-trained model:"))
         protImportTM = self.newProtocol(
             ProtCryoCARELoadModel,
-            basedir=self.dataset.getFile('model_dir'),
-            trainDataDir=self.dataset.getFile('training_data_dir'))
+            trainDataModel=self.dataset.getFile(DataSetCryoCARE.training_data_model.name),
+            trainDataDir=self.dataset.getFile(DataSetCryoCARE.training_data_dir.name))
         protImportTM = self.launchProtocol(protImportTM)
-        cryoCareModel = getattr(protImportTM, 'model', None)
+        cryoCareModel = getattr(protImportTM, loadTrainingModelOutputs.model.name, None)
         self.assertEqual(type(cryoCareModel), CryocareModel)
-        self.assertEqual(cryoCareModel.getPath(), protImportTM._getExtraPath())
+        self.assertEqual(cryoCareModel.getPath(), protImportTM._getExtraPath(CRYOCARE_MODEL_TGZ))
         self.assertEqual(cryoCareModel.getTrainDataDir(), protImportTM._getExtraPath())
         return protImportTM
 
     def _runPredict(self, protImportEven, protImportOdd, **kwargs):
         protLoadPreTrainedModel = kwargs.get("protLoadPreTrainedModel", None)
         protTraining = kwargs.get("protTraining", None)
         if protLoadPreTrainedModel:
@@ -94,28 +121,28 @@
             trainedModelProt = protLoadPreTrainedModel
         else:
             print(magentaStr("\n==> Predicting:"))
             trainedModelProt = protTraining
 
         # Predict
         protPredict = self.newProtocol(ProtCryoCAREPrediction,
-                                       even=protImportEven.outputTomograms,
-                                       odd=protImportOdd.outputTomograms,
-                                       model=getattr(trainedModelProt, 'model', None))
+                                       even=protImportEven.Tomograms,
+                                       odd=protImportOdd.Tomograms,
+                                       model=getattr(trainedModelProt, trainOutputs.model.name, None))
 
         self.launchProtocol(protPredict)
-        output = getattr(protPredict, 'outputTomograms', None)
-        self.assertEqual(output.getDim(), (1236, 1279, 209))
+        output = getattr(protPredict, predictOutputs.tomograms.name, None)
+        self.assertEqual(output.getDim(), (618, 639, 104))
         self.assertEqual(output.getSize(), 1)
         self.assertEqual(output.getSamplingRate(), self.sRate)
-        self.assertTrue(exists(protPredict._getExtraPath('Tomo110_bin6_denoised.mrc')))
+        self.assertTrue(exists(protPredict._getExtraPath('Tomo110__bin6_denoised', 'Tomo110__bin6.mrc')))
 
     def testWorkflow(self):
-        importTomoProtEven = self._runImportTomograms('tomo_even', 'even')
-        importTomoProtOdd = self._runImportTomograms('tomo_odd', 'odd')
+        importTomoProtEven = self._runImportTomograms(DataSetCryoCARE.tomo_even.name, 'even')
+        importTomoProtOdd = self._runImportTomograms(DataSetCryoCARE.tomo_odd.name, 'odd')
         prepTrainingDataProt = self._runPrepareTrainingData(importTomoProtEven, importTomoProtOdd)
-        # protTraining = self._runTrainingData(prepTrainingDataProt)
+        protTraining = self._runTrainingData(prepTrainingDataProt)
         # Prediction from training
-        # self._runPredict(importTomoProtEven, importTomoProtOdd, protTraining=protTraining)
+        self._runPredict(importTomoProtEven, importTomoProtOdd, protTraining=protTraining)
         # Load a pre-trained model and predict
         protLoadPreTrainedModel = self._runLoadTrainingModel()
         self._runPredict(importTomoProtEven, importTomoProtOdd, protTraining=protLoadPreTrainedModel)
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/utils.py` & `scipion-em-cryocare-3.1.1/cryocare/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **************************************************************************
 # *
-# * Authors:     you (you@yourinstitution.email)
+# * Authors:     Scipion Team
 # *
-# * your institution
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -19,40 +19,43 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from os.path import join, exists
-
+from os.path import join
 from pyworkflow.utils import createLink
+from cryocare.constants import TRAIN_DATA_FN, VALIDATION_DATA_FN, CRYOCARE_MODEL_TGZ
+
 
-from cryocare.constants import TRAIN_DATA_FN, VALIDATION_DATA_FN
+def checkInputTomoSetsSize(evenTomoSet, oddTomoSet):
+    message = ''
+    xe, ye, ze = evenTomoSet.getDimensions()
+    xo, yo, zo = oddTomoSet.getDimensions()
+    ne = evenTomoSet.getSize()
+    no = oddTomoSet.getSize()
+    if (xe, ye, ze, ne) != (xo, yo, zo, no):
+        message = ('Size of even and odd set of tomograms must be the same:\n'
+                   'Even --> (x, y, z, n) = ({xe}, {ye}, {ze}, {ne})\n'
+                   'Odd  --> (x, y, z, n) = ({xo}, {yo}, {zo}, {no})'.format(
+                    xe=xe, ye=ye, ze=ze, ne=ne, xo=xo, yo=yo, zo=zo, no=no))
+
+    return message
 
 
 def makeDatasetSymLinks(prot, trainDataDir):
     # The prediction is expecting the training and validation datasets to be in the same place as the training
     # model, but they are located in the training data generation extra directory. Hence, a symbolic link will
     # be created for each one
     linkedTrainingDataFile = prot._getExtraPath(TRAIN_DATA_FN)
     linkedValidationDataFile = prot._getExtraPath(VALIDATION_DATA_FN)
-    if not exists(linkedTrainingDataFile):
-        createLink(join(trainDataDir, TRAIN_DATA_FN), linkedTrainingDataFile)
-    if not exists(linkedValidationDataFile):
-        createLink(join(trainDataDir, VALIDATION_DATA_FN), linkedValidationDataFile)
-
-class CryocareUtils:
-    @staticmethod
-    def checkInputTomoSetsSize(evenTomoSet, oddTomoSet):
-        message = ''
-        xe, ye, ze = evenTomoSet.getDimensions()
-        xo, yo, zo = oddTomoSet.getDimensions()
-        ne = evenTomoSet.getSize()
-        no = oddTomoSet.getSize()
-        if (xe, ye, ze, ne) != (xo, yo, zo, no):
-            message = ('Size of even and odd set of tomograms must be the same:\n'
-                       'Even --> (x, y, z, n) = ({xe}, {ye}, {ze}, {ne})\n'
-                       'Odd  --> (x, y, z, n) = ({xo}, {yo}, {zo}, {no})'.format(
-                        xe=xe, ye=ye, ze=ze, ne=ne, xo=xo, yo=yo, zo=zo, no=no))
+    createLink(join(trainDataDir, TRAIN_DATA_FN), linkedTrainingDataFile)
+    createLink(join(trainDataDir, VALIDATION_DATA_FN), linkedValidationDataFile)
+
+
+def getModelName(prot):
+    return prot._getExtraPath(CRYOCARE_MODEL_TGZ)
+
+
+
 
-        return message
```

### Comparing `scipion-em-cryocare-3.0.1/cryocare/wizards.py` & `scipion-em-cryocare-3.1.1/cryocare/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-3.0.1/scipion_em_cryocare.egg-info/SOURCES.txt` & `scipion-em-cryocare-3.1.1/scipion_em_cryocare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-3.0.1/setup.py` & `scipion-em-cryocare-3.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,17 +26,34 @@
 
 setup(
     name='scipion-em-cryocare',  # Required
     version=__version__,  # Required
     description='Plugin to use cryoCARE inside scipion.',  # Required
     long_description=long_description,  # Optional
     url='https://github.com/scipion-em/scipion-em-cryocare',  # Optional
-    author='you',  # Optional
-    author_email='you@yourinstitution.email',  # Optional
+    author='Tim-Oliver Buchholz, Scipion Team',  # Optional
+    author_email='scipion@cnb.csic.es',  # Optional
     keywords='scipion cryoem imageprocessing scipion-3.0 tomagraphy',  # Optional
     packages=find_packages(),
     install_requires=[requirements],
     entry_points={'pyworkflow.plugin': 'cryocare = cryocare'},
     package_data={  # Optional
        'cryocare': ['icon.png', 'protocols.conf'],
-    }
+    },
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 4 - Beta',
+
+        # Indicate who your project is intended for
+        #   'Intended Audience :: Users',
+
+        # Pick your license as you wish
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3'
+    ],
 )
```

