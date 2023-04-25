# Comparing `tmp/learnware-0.0.1.99-py3-none-any.whl.zip` & `tmp/learnware-0.1.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,29 @@
-Zip file size: 3708 bytes, number of entries: 11
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-28 14:20 learnware/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-28 14:19 learnware/dataloader/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-28 14:19 learnware/learnware/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 06:39 learnware/market/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 06:39 learnware/model/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 06:39 learnware/specification/__init__.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Mar-28 14:22 learnware-0.0.1.99.dist-info/LICENSE
--rw-r--r--  2.0 unx     1737 b- defN 23-Mar-28 14:22 learnware-0.0.1.99.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 14:22 learnware-0.0.1.99.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-28 14:22 learnware-0.0.1.99.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      910 b- defN 23-Mar-28 14:22 learnware-0.0.1.99.dist-info/RECORD
-11 files, 3836 bytes uncompressed, 2134 bytes compressed:  44.4%
+Zip file size: 36577 bytes, number of entries: 27
+-rw-r--r--  2.0 unx      854 b- defN 23-Apr-25 08:52 learnware/__init__.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Apr-25 08:52 learnware/config.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Apr-25 08:52 learnware/logger.py
+-rw-r--r--  2.0 unx     1393 b- defN 23-Apr-25 08:52 learnware/utils.py
+-rw-r--r--  2.0 unx     2860 b- defN 23-Apr-25 08:52 learnware/learnware/__init__.py
+-rw-r--r--  2.0 unx     3746 b- defN 23-Apr-25 08:52 learnware/learnware/base.py
+-rw-r--r--  2.0 unx    11996 b- defN 23-Apr-25 08:52 learnware/learnware/reuse.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Apr-25 08:52 learnware/learnware/utils.py
+-rw-r--r--  2.0 unx      270 b- defN 23-Apr-25 08:52 learnware/market/__init__.py
+-rw-r--r--  2.0 unx     4492 b- defN 23-Apr-25 08:52 learnware/market/anchor.py
+-rw-r--r--  2.0 unx     5985 b- defN 23-Apr-25 08:52 learnware/market/base.py
+-rw-r--r--  2.0 unx     2940 b- defN 23-Apr-25 08:52 learnware/market/database_ops.py
+-rw-r--r--  2.0 unx    31403 b- defN 23-Apr-25 08:52 learnware/market/easy.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Apr-25 08:52 learnware/market/evolve.py
+-rw-r--r--  2.0 unx     1175 b- defN 23-Apr-25 08:52 learnware/market/evolve_anchor.py
+-rw-r--r--  2.0 unx     2885 b- defN 23-Apr-25 08:52 learnware/market/heterogeneous_feature.py
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-25 08:52 learnware/model/__init__.py
+-rw-r--r--  2.0 unx     1661 b- defN 23-Apr-25 08:52 learnware/model/base.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Apr-25 08:52 learnware/specification/__init__.py
+-rw-r--r--  2.0 unx     2925 b- defN 23-Apr-25 08:52 learnware/specification/base.py
+-rw-r--r--  2.0 unx    15787 b- defN 23-Apr-25 08:52 learnware/specification/rkme.py
+-rw-r--r--  2.0 unx     2308 b- defN 23-Apr-25 08:52 learnware/specification/utils.py
+-rw-r--r--  2.0 unx     1062 b- defN 23-Apr-25 08:53 learnware-0.1.0.99.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13476 b- defN 23-Apr-25 08:53 learnware-0.1.0.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 08:53 learnware-0.1.0.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-25 08:53 learnware-0.1.0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2268 b- defN 23-Apr-25 08:53 learnware-0.1.0.99.dist-info/RECORD
+27 files, 117515 bytes uncompressed, 32927 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,34 +1,82 @@
 Filename: learnware/__init__.py
 Comment: 
 
-Filename: learnware/dataloader/__init__.py
+Filename: learnware/config.py
+Comment: 
+
+Filename: learnware/logger.py
+Comment: 
+
+Filename: learnware/utils.py
 Comment: 
 
 Filename: learnware/learnware/__init__.py
 Comment: 
 
+Filename: learnware/learnware/base.py
+Comment: 
+
+Filename: learnware/learnware/reuse.py
+Comment: 
+
+Filename: learnware/learnware/utils.py
+Comment: 
+
 Filename: learnware/market/__init__.py
 Comment: 
 
+Filename: learnware/market/anchor.py
+Comment: 
+
+Filename: learnware/market/base.py
+Comment: 
+
+Filename: learnware/market/database_ops.py
+Comment: 
+
+Filename: learnware/market/easy.py
+Comment: 
+
+Filename: learnware/market/evolve.py
+Comment: 
+
+Filename: learnware/market/evolve_anchor.py
+Comment: 
+
+Filename: learnware/market/heterogeneous_feature.py
+Comment: 
+
 Filename: learnware/model/__init__.py
 Comment: 
 
+Filename: learnware/model/base.py
+Comment: 
+
 Filename: learnware/specification/__init__.py
 Comment: 
 
-Filename: learnware-0.0.1.99.dist-info/LICENSE
+Filename: learnware/specification/base.py
+Comment: 
+
+Filename: learnware/specification/rkme.py
+Comment: 
+
+Filename: learnware/specification/utils.py
+Comment: 
+
+Filename: learnware-0.1.0.99.dist-info/LICENSE
 Comment: 
 
-Filename: learnware-0.0.1.99.dist-info/METADATA
+Filename: learnware-0.1.0.99.dist-info/METADATA
 Comment: 
 
-Filename: learnware-0.0.1.99.dist-info/WHEEL
+Filename: learnware-0.1.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: learnware-0.0.1.99.dist-info/top_level.txt
+Filename: learnware-0.1.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: learnware-0.0.1.99.dist-info/RECORD
+Filename: learnware-0.1.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## learnware/__init__.py

```diff
@@ -1 +1,27 @@
-__version__ = "0.0.1.99"
+__version__ = "0.1.0.99"
+
+import os
+from .logger import get_module_logger
+
+
+def init(make_dir: bool = False, tf_loglevel: str = "2", **kwargs):
+    from .config import C
+
+    C.reset()
+    C.update(**kwargs)
+
+    logger = get_module_logger("Initialization")
+    logger.info(f"init learnware market with {kwargs}")
+
+    ## make dirs
+    if make_dir:
+        os.makedirs(C.root_path, exist_ok=True)
+        os.makedirs(C.database_path, exist_ok=True)
+        os.makedirs(C.learnware_pool_path, exist_ok=True)
+        os.makedirs(C.learnware_zip_pool_path, exist_ok=True)
+        os.makedirs(C.learnware_folder_pool_path, exist_ok=True)
+        logger.info(f"make learnware dir successfully!")
+
+    ## ignore tensorflow warning
+    # os.environ["TF_CPP_MIN_LOG_LEVEL"] = tf_loglevel
+    # logger.info(f"The tensorflow log level is setted to {tf_loglevel}")
```

## learnware/learnware/__init__.py

```diff
@@ -0,0 +1,179 @@
+00000000: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
+00000010: 2063 6f70 790a 0a66 726f 6d20 2e62 6173   copy..from .bas
+00000020: 6520 696d 706f 7274 204c 6561 726e 7761  e import Learnwa
+00000030: 7265 2c20 4261 7365 5265 7573 6572 0a66  re, BaseReuser.f
+00000040: 726f 6d20 2e72 6575 7365 2069 6d70 6f72  rom .reuse impor
+00000050: 7420 4a6f 6253 656c 6563 746f 7252 6575  t JobSelectorReu
+00000060: 7365 722c 2041 7665 7261 6769 6e67 5265  ser, AveragingRe
+00000070: 7573 6572 0a0a 6672 6f6d 202e 7574 696c  user..from .util
+00000080: 7320 696d 706f 7274 2067 6574 5f73 7461  s import get_sta
+00000090: 745f 7370 6563 5f66 726f 6d5f 636f 6e66  t_spec_from_conf
+000000a0: 6967 2c20 6765 745f 6d6f 6465 6c5f 6672  ig, get_model_fr
+000000b0: 6f6d 5f63 6f6e 6669 670a 6672 6f6d 202e  om_config.from .
+000000c0: 2e73 7065 6369 6669 6361 7469 6f6e 2069  .specification i
+000000d0: 6d70 6f72 7420 5370 6563 6966 6963 6174  mport Specificat
+000000e0: 696f 6e0a 6672 6f6d 202e 2e75 7469 6c73  ion.from ..utils
+000000f0: 2069 6d70 6f72 7420 7265 6164 5f79 616d   import read_yam
+00000100: 6c5f 746f 5f64 6963 740a 6672 6f6d 202e  l_to_dict.from .
+00000110: 2e6c 6f67 6765 7220 696d 706f 7274 2067  .logger import g
+00000120: 6574 5f6d 6f64 756c 655f 6c6f 6767 6572  et_module_logger
+00000130: 0a66 726f 6d20 2e2e 636f 6e66 6967 2069  .from ..config i
+00000140: 6d70 6f72 7420 430a 0a6c 6f67 6765 7220  mport C..logger 
+00000150: 3d20 6765 745f 6d6f 6475 6c65 5f6c 6f67  = get_module_log
+00000160: 6765 7228 226c 6561 726e 7761 7265 2e6c  ger("learnware.l
+00000170: 6561 726e 7761 7265 2229 0a0a 0a64 6566  earnware")...def
+00000180: 2067 6574 5f6c 6561 726e 7761 7265 5f66   get_learnware_f
+00000190: 726f 6d5f 6469 7270 6174 6828 6964 3a20  rom_dirpath(id: 
+000001a0: 7374 722c 2073 656d 616e 7469 635f 7370  str, semantic_sp
+000001b0: 6563 3a20 6469 6374 2c20 6c65 6172 6e77  ec: dict, learnw
+000001c0: 6172 655f 6469 7270 6174 683a 2073 7472  are_dirpath: str
+000001d0: 203d 204e 6f6e 6529 202d 3e20 4c65 6172   = None) -> Lear
+000001e0: 6e77 6172 653a 0a20 2020 2022 2222 4765  nware:.    """Ge
+000001f0: 7420 7468 6520 6c65 6172 6e77 6172 6520  t the learnware 
+00000200: 6f62 6a65 6374 2066 726f 6d20 6469 7270  object from dirp
+00000210: 6174 682c 2061 6e64 2070 726f 7669 6465  ath, and provide
+00000220: 2074 6865 206d 616e 6167 6520 696e 7465   the manage inte
+00000230: 7266 6163 6520 746f 7220 4c65 6172 6e77  rface tor Learnw
+00000240: 6172 6520 636c 6173 730a 0a20 2020 2050  are class..    P
+00000250: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000260: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6420  --------.    id 
+00000270: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
+00000280: 6520 6c65 6172 6e77 6172 6520 6964 2074  e learnware id t
+00000290: 6861 7420 6973 2067 6976 656e 2062 7920  hat is given by 
+000002a0: 6c65 6172 6e77 6172 6520 6d61 726b 6574  learnware market
+000002b0: 0a20 2020 2073 656d 616e 7469 635f 7370  .    semantic_sp
+000002c0: 6563 203a 2064 6963 740a 2020 2020 2020  ec : dict.      
+000002d0: 2020 5468 6520 6c65 6172 6e77 6172 6520    The learnware 
+000002e0: 7365 6d61 6e74 6963 6520 7370 6563 6966  semantice specif
+000002f0: 6163 7469 6f6e 730a 2020 2020 6c65 6172  actions.    lear
+00000300: 6e77 6172 655f 6469 7270 6174 6820 3a20  nware_dirpath : 
+00000310: 7374 720a 2020 2020 2020 2020 5468 6520  str.        The 
+00000320: 6469 7270 6174 6820 6f66 206c 6561 726e  dirpath of learn
+00000330: 7761 7265 2066 6f6c 6465 720a 0a20 2020  ware folder..   
+00000340: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00000350: 2d2d 2d2d 0a20 2020 204c 6561 726e 7761  ----.    Learnwa
+00000360: 7265 0a20 2020 2020 2020 2054 6865 2063  re.        The c
+00000370: 6f6e 7472 7563 7465 6420 6c65 6172 6e77  ontructed learnw
+00000380: 6172 6520 6f62 6a65 6374 2c20 7265 7475  are object, retu
+00000390: 726e 204e 6f6e 6520 6966 2062 7569 6c64  rn None if build
+000003a0: 2066 6169 6c65 640a 2020 2020 2222 220a   failed.    """.
+000003b0: 2020 2020 6c65 6172 6e77 6172 655f 636f      learnware_co
+000003c0: 6e66 6967 203d 207b 0a20 2020 2020 2020  nfig = {.       
+000003d0: 2022 6d6f 6465 6c22 3a20 7b0a 2020 2020   "model": {.    
+000003e0: 2020 2020 2020 2020 2263 6c61 7373 5f6e          "class_n
+000003f0: 616d 6522 3a20 224d 6f64 656c 222c 0a20  ame": "Model",. 
+00000400: 2020 2020 2020 2020 2020 2022 6b77 6172             "kwar
+00000410: 6773 223a 207b 7d2c 0a20 2020 2020 2020  gs": {},.       
+00000420: 207d 2c0a 2020 2020 2020 2020 2273 7461   },.        "sta
+00000430: 745f 7370 6563 6966 6963 6174 696f 6e73  t_specifications
+00000440: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00000450: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000460: 2020 2022 6d6f 6475 6c65 5f70 6174 6822     "module_path"
+00000470: 3a20 226c 6561 726e 7761 7265 2e73 7065  : "learnware.spe
+00000480: 6369 6669 6361 7469 6f6e 222c 0a20 2020  cification",.   
+00000490: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
+000004a0: 6173 735f 6e61 6d65 223a 2022 524b 4d45  ass_name": "RKME
+000004b0: 5374 6174 5370 6563 6966 6963 6174 696f  StatSpecificatio
+000004c0: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+000004d0: 2020 2020 2266 696c 655f 6e61 6d65 223a      "file_name":
+000004e0: 2022 7374 6174 5f73 7065 632e 6a73 6f6e   "stat_spec.json
+000004f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000500: 2020 2022 6b77 6172 6773 223a 207b 7d2c     "kwargs": {},
+00000510: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000520: 2020 2020 2020 2020 5d2c 0a20 2020 207d          ],.    }
+00000530: 0a0a 2020 2020 6966 206c 6561 726e 7761  ..    if learnwa
+00000540: 7265 5f64 6972 7061 7468 2069 7320 6e6f  re_dirpath is no
+00000550: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00000560: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00000570: 2079 616d 6c5f 636f 6e66 6967 203d 2072   yaml_config = r
+00000580: 6561 645f 7961 6d6c 5f74 6f5f 6469 6374  ead_yaml_to_dict
+00000590: 286f 732e 7061 7468 2e6a 6f69 6e28 6c65  (os.path.join(le
+000005a0: 6172 6e77 6172 655f 6469 7270 6174 682c  arnware_dirpath,
+000005b0: 2043 2e6c 6561 726e 7761 7265 5f66 6f6c   C.learnware_fol
+000005c0: 6465 725f 636f 6e66 6967 5b22 7961 6d6c  der_config["yaml
+000005d0: 5f66 696c 6522 5d29 290a 2020 2020 2020  _file"])).      
+000005e0: 2020 6578 6365 7074 2046 696c 654e 6f74    except FileNot
+000005f0: 466f 756e 6445 7272 6f72 3a0a 2020 2020  FoundError:.    
+00000600: 2020 2020 2020 2020 7961 6d6c 5f63 6f6e          yaml_con
+00000610: 6669 6720 3d20 7b7d 0a0a 2020 2020 6966  fig = {}..    if
+00000620: 2022 6e61 6d65 2220 696e 2079 616d 6c5f   "name" in yaml_
+00000630: 636f 6e66 6967 3a0a 2020 2020 2020 2020  config:.        
+00000640: 6c65 6172 6e77 6172 655f 636f 6e66 6967  learnware_config
+00000650: 5b22 6e61 6d65 225d 203d 2079 616d 6c5f  ["name"] = yaml_
+00000660: 636f 6e66 6967 5b22 6e61 6d65 225d 0a20  config["name"]. 
+00000670: 2020 2069 6620 226d 6f64 656c 2220 696e     if "model" in
+00000680: 2079 616d 6c5f 636f 6e66 6967 3a0a 2020   yaml_config:.  
+00000690: 2020 2020 2020 6c65 6172 6e77 6172 655f        learnware_
+000006a0: 636f 6e66 6967 5b22 6d6f 6465 6c22 5d2e  config["model"].
+000006b0: 7570 6461 7465 2879 616d 6c5f 636f 6e66  update(yaml_conf
+000006c0: 6967 5b22 6d6f 6465 6c22 5d29 0a20 2020  ig["model"]).   
+000006d0: 2069 6620 2273 7461 745f 7370 6563 6966   if "stat_specif
+000006e0: 6963 6174 696f 6e73 2220 696e 2079 616d  ications" in yam
+000006f0: 6c5f 636f 6e66 6967 3a0a 2020 2020 2020  l_config:.      
+00000700: 2020 6c65 6172 6e77 6172 655f 636f 6e66    learnware_conf
+00000710: 6967 5b22 7374 6174 5f73 7065 6369 6669  ig["stat_specifi
+00000720: 6361 7469 6f6e 7322 5d20 3d20 7961 6d6c  cations"] = yaml
+00000730: 5f63 6f6e 6669 675b 2273 7461 745f 7370  _config["stat_sp
+00000740: 6563 6966 6963 6174 696f 6e73 225d 2e63  ecifications"].c
+00000750: 6f70 7928 290a 0a20 2020 2069 6620 226d  opy()..    if "m
+00000760: 6f64 756c 655f 7061 7468 2220 6e6f 7420  odule_path" not 
+00000770: 696e 206c 6561 726e 7761 7265 5f63 6f6e  in learnware_con
+00000780: 6669 675b 226d 6f64 656c 225d 3a0a 2020  fig["model"]:.  
+00000790: 2020 2020 2020 6c65 6172 6e77 6172 655f        learnware_
+000007a0: 636f 6e66 6967 5b22 6d6f 6465 6c22 5d5b  config["model"][
+000007b0: 226d 6f64 756c 655f 7061 7468 225d 203d  "module_path"] =
+000007c0: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
+000007d0: 2020 2020 2020 2020 2020 206c 6561 726e             learn
+000007e0: 7761 7265 5f64 6972 7061 7468 2c20 432e  ware_dirpath, C.
+000007f0: 6c65 6172 6e77 6172 655f 666f 6c64 6572  learnware_folder
+00000800: 5f63 6f6e 6669 675b 226d 6f64 756c 655f  _config["module_
+00000810: 6669 6c65 225d 0a20 2020 2020 2020 2029  file"].        )
+00000820: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
+00000830: 2020 206c 6561 726e 7761 7265 5f73 7065     learnware_spe
+00000840: 6320 3d20 5370 6563 6966 6963 6174 696f  c = Specificatio
+00000850: 6e28 290a 2020 2020 2020 2020 666f 7220  n().        for 
+00000860: 5f73 7461 745f 7370 6563 2069 6e20 6c65  _stat_spec in le
+00000870: 6172 6e77 6172 655f 636f 6e66 6967 5b22  arnware_config["
+00000880: 7374 6174 5f73 7065 6369 6669 6361 7469  stat_specificati
+00000890: 6f6e 7322 5d3a 0a20 2020 2020 2020 2020  ons"]:.         
+000008a0: 2020 2073 7461 745f 7370 6563 203d 205f     stat_spec = _
+000008b0: 7374 6174 5f73 7065 632e 636f 7079 2829  stat_spec.copy()
+000008c0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+000008d0: 745f 7370 6563 5b22 6669 6c65 5f6e 616d  t_spec["file_nam
+000008e0: 6522 5d20 3d20 6f73 2e70 6174 682e 6a6f  e"] = os.path.jo
+000008f0: 696e 286c 6561 726e 7761 7265 5f64 6972  in(learnware_dir
+00000900: 7061 7468 2c20 7374 6174 5f73 7065 635b  path, stat_spec[
+00000910: 2266 696c 655f 6e61 6d65 225d 290a 2020  "file_name"]).  
+00000920: 2020 2020 2020 2020 2020 7374 6174 5f73            stat_s
+00000930: 7061 635f 6e61 6d65 2c20 7374 6174 5f73  pac_name, stat_s
+00000940: 7065 635f 696e 7374 203d 2067 6574 5f73  pec_inst = get_s
+00000950: 7461 745f 7370 6563 5f66 726f 6d5f 636f  tat_spec_from_co
+00000960: 6e66 6967 2873 7461 745f 7370 6563 290a  nfig(stat_spec).
+00000970: 2020 2020 2020 2020 2020 2020 6c65 6172              lear
+00000980: 6e77 6172 655f 7370 6563 2e75 7064 6174  nware_spec.updat
+00000990: 655f 7374 6174 5f73 7065 6328 2a2a 7b73  e_stat_spec(**{s
+000009a0: 7461 745f 7370 6163 5f6e 616d 653a 2073  tat_spac_name: s
+000009b0: 7461 745f 7370 6563 5f69 6e73 747d 290a  tat_spec_inst}).
+000009c0: 0a20 2020 2020 2020 206c 6561 726e 7761  .        learnwa
+000009d0: 7265 5f73 7065 632e 7570 6c6f 6164 5f73  re_spec.upload_s
+000009e0: 656d 616e 7469 635f 7370 6563 2863 6f70  emantic_spec(cop
+000009f0: 792e 6465 6570 636f 7079 2873 656d 616e  y.deepcopy(seman
+00000a00: 7469 635f 7370 6563 2929 0a20 2020 2020  tic_spec)).     
+00000a10: 2020 2023 206c 6561 726e 7761 7265 5f6d     # learnware_m
+00000a20: 6f64 656c 203d 2067 6574 5f6d 6f64 656c  odel = get_model
+00000a30: 5f66 726f 6d5f 636f 6e66 6967 286c 6561  _from_config(lea
+00000a40: 726e 7761 7265 5f63 6f6e 6669 675b 226d  rnware_config["m
+00000a50: 6f64 656c 225d 290a 0a20 2020 2065 7863  odel"])..    exc
+00000a60: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00000a70: 2065 3a0a 2020 2020 2020 2020 6c6f 6767   e:.        logg
+00000a80: 6572 2e77 6172 6e69 6e67 2866 224c 6f61  er.warning(f"Loa
+00000a90: 6420 4c65 6172 6e77 6172 6520 7b69 647d  d Learnware {id}
+00000aa0: 2066 6169 6c65 6421 2044 7565 2074 6f20   failed! Due to 
+00000ab0: 7b72 6570 7228 6529 7d22 290a 2020 2020  {repr(e)}").    
+00000ac0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00000ad0: 0a20 2020 2072 6574 7572 6e20 4c65 6172  .    return Lear
+00000ae0: 6e77 6172 6528 6964 3d69 642c 206d 6f64  nware(id=id, mod
+00000af0: 656c 3d6c 6561 726e 7761 7265 5f63 6f6e  el=learnware_con
+00000b00: 6669 675b 226d 6f64 656c 225d 2c20 7370  fig["model"], sp
+00000b10: 6563 6966 6963 6174 696f 6e3d 6c65 6172  ecification=lear
+00000b20: 6e77 6172 655f 7370 6563 290a            nware_spec).
```

## learnware/market/__init__.py

```diff
@@ -0,0 +1,17 @@
+00000000: 6672 6f6d 202e 616e 6368 6f72 2069 6d70  from .anchor imp
+00000010: 6f72 7420 416e 6368 6f72 6564 5573 6572  ort AnchoredUser
+00000020: 496e 666f 2c20 416e 6368 6f72 6564 4d61  Info, AnchoredMa
+00000030: 726b 6574 0a66 726f 6d20 2e62 6173 6520  rket.from .base 
+00000040: 696d 706f 7274 2042 6173 6555 7365 7249  import BaseUserI
+00000050: 6e66 6f2c 2042 6173 654d 6172 6b65 740a  nfo, BaseMarket.
+00000060: 6672 6f6d 202e 6576 6f6c 7665 5f61 6e63  from .evolve_anc
+00000070: 686f 7220 696d 706f 7274 2045 766f 6c76  hor import Evolv
+00000080: 6564 416e 6368 6f72 6564 4d61 726b 6574  edAnchoredMarket
+00000090: 0a66 726f 6d20 2e65 766f 6c76 6520 696d  .from .evolve im
+000000a0: 706f 7274 2045 766f 6c76 6564 4d61 726b  port EvolvedMark
+000000b0: 6574 0a66 726f 6d20 2e65 6173 7920 696d  et.from .easy im
+000000c0: 706f 7274 2045 6173 794d 6172 6b65 740a  port EasyMarket.
+000000d0: 6672 6f6d 202e 6865 7465 726f 6765 6e65  from .heterogene
+000000e0: 6f75 735f 6665 6174 7572 6520 696d 706f  ous_feature impo
+000000f0: 7274 2048 6574 6572 6f67 656e 656f 7573  rt Heterogeneous
+00000100: 4665 6174 7572 654d 6172 6b65 740a       FeatureMarket.
```

## learnware/model/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 6261 7365 2069 6d70 6f72  from .base impor
+00000010: 7420 4261 7365 4d6f 6465 6c0a            t BaseModel.
```

## learnware/specification/__init__.py

```diff
@@ -0,0 +1,9 @@
+00000000: 6672 6f6d 202e 7574 696c 7320 696d 706f  from .utils impo
+00000010: 7274 2067 656e 6572 6174 655f 7374 6174  rt generate_stat
+00000020: 5f73 7065 630a 6672 6f6d 202e 6261 7365  _spec.from .base
+00000030: 2069 6d70 6f72 7420 5370 6563 6966 6963   import Specific
+00000040: 6174 696f 6e2c 2042 6173 6553 7461 7453  ation, BaseStatS
+00000050: 7065 6369 6669 6361 7469 6f6e 0a66 726f  pecification.fro
+00000060: 6d20 2e72 6b6d 6520 696d 706f 7274 2052  m .rkme import R
+00000070: 4b4d 4553 7461 7453 7065 6369 6669 6361  KMEStatSpecifica
+00000080: 7469 6f6e 0a                             tion.
```

## Comparing `learnware-0.0.1.99.dist-info/LICENSE` & `learnware-0.1.0.99.dist-info/LICENSE`

 * *Files identical despite different names*

