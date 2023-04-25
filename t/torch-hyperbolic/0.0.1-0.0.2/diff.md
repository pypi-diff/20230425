# Comparing `tmp/torch_hyperbolic-0.0.1.tar.gz` & `tmp/torch_hyperbolic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_hyperbolic-0.0.1.tar", last modified: Mon Apr 24 12:59:42 2023, max compression
+gzip compressed data, was "torch_hyperbolic-0.0.2.tar", last modified: Tue Apr 25 10:27:19 2023, max compression
```

## Comparing `torch_hyperbolic-0.0.1.tar` & `torch_hyperbolic-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 12:59:42.478613 torch_hyperbolic-0.0.1/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1073 2023-04-24 11:21:18.000000 torch_hyperbolic-0.0.1/LICENSE.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-24 12:59:42.478224 torch_hyperbolic-0.0.1/PKG-INFO
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      286 2023-04-24 11:21:18.000000 torch_hyperbolic-0.0.1/README.md
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       38 2023-04-24 12:59:42.478685 torch_hyperbolic-0.0.1/setup.cfg
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      329 2023-04-24 12:57:55.000000 torch_hyperbolic-0.0.1/setup.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 12:59:42.468152 torch_hyperbolic-0.0.1/torch_hyperbolic/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 11:39:11.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/__init__.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594    14002 2023-04-24 12:25:29.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/manifolds.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 12:59:42.477706 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      130 2023-04-24 11:49:25.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/__init__.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      884 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hact.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      984 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hdecoder.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      915 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hencoder.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     9837 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hgat.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     4397 2023-04-24 12:49:54.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hgcn.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1774 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hlinear.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     7252 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/optim.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1542 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.1/torch_hyperbolic/utils.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 12:59:42.471778 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-24 12:59:42.000000 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/PKG-INFO
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      551 2023-04-24 12:59:42.000000 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/SOURCES.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594        1 2023-04-24 12:59:42.000000 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/dependency_links.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       31 2023-04-24 12:59:42.000000 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/requires.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       17 2023-04-24 12:59:42.000000 torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/top_level.txt
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.254868 torch_hyperbolic-0.0.2/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1073 2023-04-24 11:21:18.000000 torch_hyperbolic-0.0.2/LICENSE.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 10:27:19.253980 torch_hyperbolic-0.0.2/PKG-INFO
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     3429 2023-04-25 10:19:14.000000 torch_hyperbolic-0.0.2/README.md
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       38 2023-04-25 10:27:19.255067 torch_hyperbolic-0.0.2/setup.cfg
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      318 2023-04-25 10:26:27.000000 torch_hyperbolic-0.0.2/setup.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.232031 torch_hyperbolic-0.0.2/torch_hyperbolic/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 11:39:11.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594    14001 2023-04-25 09:46:50.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/manifolds.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.239075 torch_hyperbolic-0.0.2/torch_hyperbolic/models/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       19 2023-04-25 08:18:26.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     2560 2023-04-25 09:35:38.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/hgnn.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 16:01:54.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/hmlp.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.252761 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      130 2023-04-24 16:20:44.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      999 2023-04-25 08:25:34.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hact.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1036 2023-04-24 15:34:16.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hdecoder.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1053 2023-04-24 15:39:13.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hencoder.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     9837 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgat.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     4397 2023-04-24 12:49:54.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgcn.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1784 2023-04-25 08:26:39.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hlinear.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     7252 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/optim.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1542 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/utils.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.236581 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/PKG-INFO
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      651 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/SOURCES.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594        1 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/dependency_links.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       31 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/requires.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       17 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/top_level.txt
```

### Comparing `torch_hyperbolic-0.0.1/LICENSE.txt` & `torch_hyperbolic-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/manifolds.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/manifolds.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     def mobius_matvec(self, m, x, c):
         sqrt_c = c ** 0.5
         x_norm = x.norm(dim=-1, keepdim=True, p=2).clamp_min(self.min_norm)
         mx = x @ m.transpose(-1, -2)
         mx_norm = mx.norm(dim=-1, keepdim=True, p=2).clamp_min(self.min_norm)
         res_c = tanh(mx_norm / x_norm * artanh(sqrt_c * x_norm)) * mx / (mx_norm * sqrt_c)
-        cond = (mx == 0).prod(-1, keepdim=True, dtype=torch.uint8)
+        cond = (mx == 0).prod(-1, keepdim=True, dtype=torch.bool)
         res_0 = torch.zeros(1, dtype=res_c.dtype, device=res_c.device)
         res = torch.where(cond, res_0, res_c)
         return res
 
     def init_weights(self, w, c, irange=1e-5):
         w.data.uniform_(-irange, irange)
         return w
@@ -323,24 +323,24 @@
         # clamp distance to avoid nans in Fermi-Dirac decoder
         return torch.clamp(sqdist, max=50.0)
 
     def proj(self, x, c):
         K = 1. / c
         d = x.size(-1) - 1
         y = x.narrow(-1, 1, d)
-        y_sqnorm = torch.norm(y, p=2, dim=1, keepdim=True) ** 2 
+        y_sqnorm = torch.norm(y, p=2, dim=1, keepdim=True) ** 2
         mask = torch.ones_like(x)
         mask[:, 0] = 0
         vals = torch.zeros_like(x)
         vals[:, 0:1] = torch.sqrt(torch.clamp(K + y_sqnorm, min=self.eps[x.dtype]))
         return vals + mask * x
 
     def proj_tan(self, u, x, c):
         K = 1. / c
-        d = x.size(1) - 1
+        d = x.size(-1) - 1
         ux = torch.sum(x.narrow(-1, 1, d) * u.narrow(-1, 1, d), dim=1, keepdim=True)
         mask = torch.ones_like(u)
         mask[:, 0] = 0
         vals = torch.zeros_like(u)
         vals[:, 0:1] = ux / torch.clamp(x[:, 0:1], min=self.eps[x.dtype])
         return vals + mask * u
```

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hact.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hdecoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-"""Hyperbolic layers."""
 import torch.nn as nn
+import torch
 from torch.nn.modules.module import Module
-import torch_hyperbolic.manifolds as manifolds
+from torch_hyperbolic import manifolds
 
-class HypAct(Module):
-    """
-    Hyperbolic activation layer.
-    """
 
-    def __init__(self, act, c_in=None, c_out=None, manifold="PoincareBall"):
-        super(HypAct, self).__init__()
+class HyperbolicDecoder(Module):
+    def __init__(self, manifold: str = "PoincareBall", curvature=None):
+        """ The decode() method of the LinearDecoder from https://github.com/HazyResearch/hgcn/edit/master/models/decoders.py as an explicit class
+            This implementation does NOT include an additional Linear layer, so it is intended to be used before the final Linear layer """
+        super(HyperbolicDecoder, self).__init__()
+        self.curvature = nn.Parameter(torch.Tensor([1.])) if curvature is None else curvature
         self.manifold = getattr(manifolds, manifold)()
-        self.act = act
-        self.c_in = c_in
-        self.c_out = c_out
 
     def forward(self, x):
-        x = self.act(self.manifold.logmap0(x, c=self.c_in))
-        x = self.manifold.proj_tan0(x, c=self.c_out)
-        return self.manifold.proj(self.manifold.expmap0(x, c=self.c_out), c=self.c_out)
+        """ Projects x from hyperbolic back into euclidean space """
+        x = self.manifold.logmap0(x, c=self.curvature)
+        if isinstance(self.manifold, manifolds.Hyperboloid):
+            x = x[:, 1:]
+        return x
 
     def extra_repr(self):
-        return 'c_in={}, c_out={}'.format(
-            self.c_in, self.c_out
-        )
-
-    def __call__(self, *args, **kwargs):
-        return self.forward(*args, **kwargs)
+        return 'c={}'.format(self.curvature)
```

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hdecoder.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hencoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import torch.nn as nn
 import torch
 from torch.nn.modules.module import Module
-import torch_hyperbolic.manifolds as manifolds
+from torch_hyperbolic import manifolds
 
 
-class HyperbolicDecoder(Module):
-    def __init__(self, manifold: str, curvature=None):
-        """ The decode() method of the LinearDecoder from https://github.com/HazyResearch/hgcn/edit/master/models/decoders.py as an explicit class
-            This implementation does NOT include an additional Linear layer, so it is intended to be used before the final Linear layer """
-        super(HyperbolicDecoder, self).__init__()
+class HyperbolicEncoder(Module):
+    def __init__(self, manifold: str = "PoincareBall", curvature=None):
+        """ The encode() method of the HGCN and HNN from https://github.com/HazyResearch/hgcn/edit/master/models/encoders.py as an explicit class """
+        super(HyperbolicEncoder, self).__init__()
         self.curvature = nn.Parameter(torch.Tensor([1.])) if curvature is None else curvature
         self.manifold = getattr(manifolds, manifold)()
 
     def forward(self, x):
-        """ Projects x from hyperbolic back into euclidean space """
-        h = self.manifold.proj_tan0(self.manifold.logmap0(x, c=self.curvature), c=self.curvature)
-        return h
+        """ Projects x into hyperbolic space """
+        if isinstance(self.manifold, manifolds.Hyperboloid):
+            x = torch.cat((torch.zeros_like(x)[:, 0:1], x), dim=-1)
+        x_tan = self.manifold.proj_tan0(x, self.curvature)
+        x_hyp = self.manifold.expmap0(x_tan, c=self.curvature)
+        x_hyp = self.manifold.proj(x_hyp, c=self.curvature)
+        return x_hyp
 
     def extra_repr(self):
         return 'c={}'.format(self.curvature)
```

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hgat.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgat.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hgcn.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgcn.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/nn/hlinear.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hlinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         super(HypLinear, self).__init__()
         self.manifold = getattr(manifolds, manifold)()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.c = c
         self.dropout = dropout
         self.use_bias = use_bias
-        self.bias = nn.Parameter(torch.Tensor(out_channels))
-        self.weight = nn.Parameter(torch.Tensor(out_channels, in_channels))
+        self.bias = nn.Parameter(torch.Tensor(self.out_channels))
+        self.weight = nn.Parameter(torch.Tensor(self.out_channels, in_channels))
         self.reset_parameters()
 
     def reset_parameters(self):
         init.xavier_uniform_(self.weight, gain=math.sqrt(2))
         init.constant_(self.bias, 0)
 
     def forward(self, x):
```

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/optim.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/optim.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic/utils.py` & `torch_hyperbolic-0.0.2/torch_hyperbolic/utils.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.1/torch_hyperbolic.egg-info/SOURCES.txt` & `torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 torch_hyperbolic/optim.py
 torch_hyperbolic/utils.py
 torch_hyperbolic.egg-info/PKG-INFO
 torch_hyperbolic.egg-info/SOURCES.txt
 torch_hyperbolic.egg-info/dependency_links.txt
 torch_hyperbolic.egg-info/requires.txt
 torch_hyperbolic.egg-info/top_level.txt
+torch_hyperbolic/models/__init__.py
+torch_hyperbolic/models/hgnn.py
+torch_hyperbolic/models/hmlp.py
 torch_hyperbolic/nn/__init__.py
 torch_hyperbolic/nn/hact.py
 torch_hyperbolic/nn/hdecoder.py
 torch_hyperbolic/nn/hencoder.py
 torch_hyperbolic/nn/hgat.py
 torch_hyperbolic/nn/hgcn.py
 torch_hyperbolic/nn/hlinear.py
```

