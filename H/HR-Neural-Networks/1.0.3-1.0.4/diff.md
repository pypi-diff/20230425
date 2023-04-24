# Comparing `tmp/HR_Neural_Networks-1.0.3.tar.gz` & `tmp/HR_Neural_Networks-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HR_Neural_Networks-1.0.3.tar", last modified: Fri Mar  3 18:06:00 2023, max compression
+gzip compressed data, was "HR_Neural_Networks-1.0.4.tar", last modified: Mon Apr 24 21:56:55 2023, max compression
```

## Comparing `HR_Neural_Networks-1.0.3.tar` & `HR_Neural_Networks-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,60 @@
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-03-03 18:06:00.246638 HR_Neural_Networks-1.0.3/
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-03-03 18:06:00.235961 HR_Neural_Networks-1.0.3/HR_Neural_Networks/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    11518 2023-03-03 17:57:46.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks/HR.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-03-03 18:06:00.246291 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-03-03 18:05:59.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/PKG-INFO
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      274 2023-03-03 18:06:00.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)        1 2023-03-03 18:05:59.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       37 2023-03-03 18:05:59.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/requires.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       19 2023-03-03 18:05:59.000000 HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/top_level.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1094 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.3/LICENSE.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-03-03 18:06:00.246813 HR_Neural_Networks-1.0.3/PKG-INFO
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6863 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.3/README.md
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       79 2023-03-03 18:06:00.249084 HR_Neural_Networks-1.0.3/setup.cfg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1983 2023-03-03 18:04:31.000000 HR_Neural_Networks-1.0.3/setup.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.170526 HR_Neural_Networks-1.0.4/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     8196 2023-04-24 21:54:05.000000 HR_Neural_Networks-1.0.4/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.018607 HR_Neural_Networks-1.0.4/HR_Neural_Networks/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-04-24 21:53:26.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12307 2023-04-24 21:50:52.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/HR.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.042270 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.055294 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.1/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.1/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      343 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.1/CIFAR_10_note.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12540 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.1/mnist_single_param.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.074709 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.086949 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21968 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/Rice_HR.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.108556 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21736 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/Rice_TRADES.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6099 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/trades.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.120752 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4597 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/preactresnet.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     5537 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4208 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/preactresnet.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4043 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.2/utils.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.128160 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.3/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    17499 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.3/CIFAR_10_all_error_sources.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4538 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/Section_6.3/resnet.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.134338 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1739 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/__pycache__/helper_functions.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1928 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks/Paper_experiments/helper_functions.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.029447 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-24 21:56:54.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1787 2023-04-24 21:56:54.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)        1 2023-04-24 21:56:54.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       37 2023-04-24 21:56:54.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/requires.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       19 2023-04-24 21:56:54.000000 HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/top_level.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1094 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/LICENSE.txt
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.166759 HR_Neural_Networks-1.0.4/Misc/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/Misc/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    27583 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/Misc/Classifiers.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)   307785 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/DRO_gif.gif
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    56951 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/HD.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    22190 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/HR.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1017 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/Misc/Julia.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)  1056373 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/Misc/SVP-gif.gif
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     2369 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/colab.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      987 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/mosek.lic
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1213 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/pt_badge.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4781 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/python.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     3601 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.4/Misc/tf.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-24 21:56:55.170984 HR_Neural_Networks-1.0.4/PKG-INFO
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     7303 2023-04-24 21:53:35.000000 HR_Neural_Networks-1.0.4/README.md
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       54 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.4/__init__.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.168010 HR_Neural_Networks-1.0.4/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      206 2023-04-16 13:18:40.000000 HR_Neural_Networks-1.0.4/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-24 21:56:55.169565 HR_Neural_Networks-1.0.4/dist/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 18:07:47.000000 HR_Neural_Networks-1.0.4/dist/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       79 2023-04-24 21:56:55.172991 HR_Neural_Networks-1.0.4/setup.cfg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1983 2023-04-24 21:55:08.000000 HR_Neural_Networks-1.0.4/setup.py
```

### Comparing `HR_Neural_Networks-1.0.3/HR_Neural_Networks/HR.py` & `HR_Neural_Networks-1.0.4/HR_Neural_Networks/HR.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import numpy as np
 from torch.autograd import Variable
 import torchattacks
 import warnings
 import mosek
 import os
 import torch.nn as nn
+import time
+import warnings
 warnings.filterwarnings("ignore")
 os.environ['MOSEKLM_LICENSE_FILE'] = "mosek.lic"
 
 class HR_Neural_Networks:
 
     def __init__(self, NN_model,
                  train_batch_size,
@@ -20,26 +22,28 @@
                  α_choice,
                  r_choice,
                  ϵ_choice,
                  learning_approach = "HD",
                  adversarial_steps=10,
                  adversarial_step_size=0.2,
                  noise_set = "l-2",
+                 defense_method = "PGD",
                  output_return = "pytorch_loss_function"
                  ):
 
         # End model
         self.NN_model = NN_model
         self.train_batch_size = train_batch_size
         self.adversarial_steps = adversarial_steps
         self.adversarial_step_size = adversarial_step_size
         self.numerical_eps = 0.000001
         self.noise_set = noise_set
         self.learning_approach = learning_approach
         self.output_return = output_return
+        self.defense_method = defense_method
  
         if loss_fn == None:
             print("Loss is defaulted to cross entropy loss. Consider changing if not doing classification.")
             self.loss_fn = nn.CrossEntropyLoss(reduction="none")
 
         else:
             self.loss_fn = loss_fn
@@ -48,15 +52,15 @@
         if α_choice == 0:
             self.α_choice = self.numerical_eps
         else:
             self.α_choice = α_choice
         
         # Handling choice of r
         if r_choice == 0 and α_choice != 0:
-            self.r_choice = 0.001 # For numerical stability. 0 or very small values of r cause problems.
+            self.r_choice = 0.001 # For numerical stability. 0 or very small values of r cause algorithm to be slow.
         else:
             self.r_choice = r_choice
             
         # Handling choice of epsilon. We wont set equal to numerical eps, since running PGD is very slow
         self.ϵ_choice = ϵ_choice
         
         # Initialising either HR or HD to be used in DPP. DPP is an approach where the decision variables,
@@ -185,29 +189,44 @@
         self.model = cp.Problem(
             objective=objective,
             constraints=complete_constraints)
 
     def _initialise_adversarial_setup(self):
         
         if self.noise_set == "l-2":
+            
+            if self.defense_method == "PGD":
 
-            self.adversarial_attack_train = torchattacks.PGDL2(self.NN_model,
-                                                               eps=self.ϵ_choice,
-                                                               alpha=self.adversarial_step_size,
-                                                               steps=self.adversarial_steps,
-                                                               random_start=True,
-                                                               eps_for_division=1e-10)
+                self.adversarial_attack_train = torchattacks.PGDL2(self.NN_model,
+                                                                   eps=self.ϵ_choice,
+                                                                   alpha=self.adversarial_step_size,
+                                                                   steps=self.adversarial_steps,
+                                                                   random_start=True,
+                                                                   eps_for_division=1e-10)
+                
+            elif self.defense_method == "FFGSM":
+                
+                raise Exception("FGSM for l-2 defense not currently supported")
+                
             
         elif self.noise_set == "l-inf":
             
-            self.adversarial_attack_train = torchattacks.attacks.pgd.PGD(self.NN_model,
-                                             eps=self.ϵ_choice,
-                                             alpha=self.adversarial_step_size,
-                                             steps=self.adversarial_steps,
-                                             random_start=True)
+            if self.defense_method == "PGD":
+
+                self.adversarial_attack_train = torchattacks.attacks.pgd.PGD(self.NN_model,
+                                                 eps=self.ϵ_choice,
+                                                 alpha=self.adversarial_step_size,
+                                                 steps=self.adversarial_steps,
+                                                 random_start=True)
+            
+            elif self.defense_method == "FFGSM":
+
+                self.adversarial_attack_train = torchattacks.FFGSM(self.NN_model, 
+                                                                   eps=self.ϵ_choice, 
+                                                                   alpha=self.adversarial_step_size)
 
 
     def HR_criterion(self, inputs = None, 
                            targets = None, 
                            inf_loss = None, 
                            device='cuda'):
```

### Comparing `HR_Neural_Networks-1.0.3/HR_Neural_Networks.egg-info/PKG-INFO` & `HR_Neural_Networks-1.0.4/HR_Neural_Networks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HR-Neural-Networks
-Version: 1.0.3
+Version: 1.0.4
 Summary: Holistic Robust Neural Networks
 Home-page: https://github.com/RyanLucas3/HR_Neural_Networks
-Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.3.tar.gz
+Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.4.tar.gz
 Author: Amine Bennouna, Bart Van Parys, Ryan Lucas
 Author-email: ryanlu@mit.edu
 License: MIT
 Keywords: Neural Networks,Robustness,Machine Learning,Data Science,Adversarial Attacks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HR_Neural_Networks-1.0.3/LICENSE.txt` & `HR_Neural_Networks-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.3/PKG-INFO` & `HR_Neural_Networks-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HR_Neural_Networks
-Version: 1.0.3
+Version: 1.0.4
 Summary: Holistic Robust Neural Networks
 Home-page: https://github.com/RyanLucas3/HR_Neural_Networks
-Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.3.tar.gz
+Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.4.tar.gz
 Author: Amine Bennouna, Bart Van Parys, Ryan Lucas
 Author-email: ryanlu@mit.edu
 License: MIT
 Keywords: Neural Networks,Robustness,Machine Learning,Data Science,Adversarial Attacks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HR_Neural_Networks-1.0.3/README.md` & `HR_Neural_Networks-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Holistic Robust Neural Networks (HR)
+# Holistic Robust (HR) Neural Networks
 
 <p align="left">
   <img width="150" height="40" src="Misc/python.svg">
    <img width="180" height="40" src="Misc/tf.svg">
     <img width="150" height="40" src="Misc/pt_badge.svg">
 </p>
 
 ```python
 pip install HR_Neural_Networks
 ```
 
-### This code base is an open-source implementation of "Certified Robust Neural Networks: Generalization and Corruption Resistance".
+### This code base is an open-source implementation of the paper ["Certified Robust Neural Networks: Generalization and Corruption Resistance"](https://arxiv.org/pdf/2303.02251.pdf).
 
 Holistic Robust Learning (HR) is a learning approach which provides _certified_ protection against data poisoning and evasion attacks, while enjoying _guaranteed_ generalization. HR minimizes a loss function that is guaranteed to be an upper bound on the out-of-sample performance of the trained networks with high probability. Hence, when training with HR, the out-of-sample performance is at least as good as the observed in-sample performance. This is both guaranteed theoretically and verified empirically.
 Robustness is controlled by three parameters: 
 * $\alpha$: controls protection against generic data poisoning at training time. This encompasses any kind of corruption in the training data; for instance training examples that have been obscured or which are wholly misspecified. For a given chosen $\alpha$, HR is certified when up to a fraction $\alpha$ of data points are corrupted.
 * $\epsilon$: controls protection against small perturbations to the testing or training examples, such as noise or evasive attacks. HR is certified to any adversarial attacks limited to the norm ball { $\delta: ||\delta|| \leq \epsilon$ }. The current implementation supports $\ell_2$ and $\ell_\infty$ balls.
 * $r$: controls protection against overfitting to the training instances. The parameter sets the desired strength of generalization and the conservativeness of training. It also reduces variance to randomness of the training data. HR in-sample loss is guaranteed to be an upper bound on the out-of-sample loss with probability $1-e^{-nr +O(1)}$ where $n$ is the data size.
 
@@ -59,15 +59,15 @@
 
 ```python
 
 criterion = F.cross_entropy(reduction = 'none') # note the change from mean -> none
 
 ########### HR Model Instantiation ###############
 
-from HR import * 
+from HR_Neural_Networks.HR import * 
 
 α_choice = 0.05 
 r_choice = 0.1
 ϵ_choice = 0.5
        
 HR = HR_Neural_Networks(NN_model = model,
                         train_batch_size = 128,
@@ -108,8 +108,19 @@
 
 The HR objective function is an upper bound on the test performance with probability $1-e^{-rn+O(1)}$ when less then a fraction $\alpha$ of all $n$ samples are tampered by poisoning, and the evasion corruption is bounded within the set $\mathcal{N}$.
 The parameters $\mathcal{N}, r$ and $\alpha$ hence are important design choices and directly reflect the desired robustness. In this implementation, we chose $\mathcal{N} =$ { $\delta: ||\delta|| \leq \epsilon $}.
 
 The HR loss is also proven to be a ``tight'' upper bound. That is, corruption and generalization are efficiently captured and the provided robustness is not overly conservative. In particular, HR captures efficiently the interaction between generalization and corruption. 
 For example, when used in conjunction $\mathcal{N}$ and $r$ can provide protection to the well-known phenomenon of  [robust overfitting](https://arxiv.org/abs/2002.11569), where adversarial training exhibit severe overfitting.
 
+## Reference
+```
+@article{bennouna2023certified,
+  title={Certified Robust Neural Networks: Generalization and Corruption Resistance},
+  author={Bennouna, Amine and Lucas, Ryan and Van Parys, Bart},
+  journal={arXiv preprint arXiv:2303.02251},
+  year={2023}
+}
+```
+
+Please contact amineben@mit.edu and ryanlu@mit.edu if you have any question about the paper or the codes.
```

### Comparing `HR_Neural_Networks-1.0.3/setup.py` & `HR_Neural_Networks-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'HR_Neural_Networks',         # How you named your package folder (MyLib)
   packages = ['HR_Neural_Networks'],   # Chose the same as "name"
-  version = '1.0.3',      # Start with a small number and increase it with every change you make
+  version = '1.0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Holistic Robust Neural Networks',   # Give a short description about your library
   author = 'Amine Bennouna, Bart Van Parys, Ryan Lucas',                   # Type in your name
   author_email = 'ryanlu@mit.edu',      # Type in your E-Mail
   url = 'https://github.com/RyanLucas3/HR_Neural_Networks',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.3.tar.gz',
+  download_url = 'https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.4.tar.gz',
   keywords = ['Neural Networks', 'Robustness', 'Machine Learning', "Data Science", "Adversarial Attacks"],   # Keywords that define your package best
   install_requires=[ # I get to this in a second
           'mosek',
           'torchattacks',
           'numpy',
           'cvxpy',
           'torch'
```

