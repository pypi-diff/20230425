# Comparing `tmp/pyVIA-0.1.8.tar.gz` & `tmp/pyVIA-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyVIA-0.1.8.tar", last modified: Mon Jan 18 06:24:25 2021, max compression
+gzip compressed data, was "dist/pyVIA-0.1.9.tar", last modified: Tue Jan 19 04:52:20 2021, max compression
```

## Comparing `pyVIA-0.1.8.tar` & `pyVIA-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-18 06:24:25.000000 pyVIA-0.1.8/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       38 2021-01-18 06:24:25.000000 pyVIA-0.1.8/setup.cfg
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      787 2021-01-18 06:24:02.000000 pyVIA-0.1.8/setup.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     9635 2021-01-13 00:37:15.000000 pyVIA-0.1.8/README.md
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    11082 2021-01-18 06:24:25.000000 pyVIA-0.1.8/PKG-INFO
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      103 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/requires.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        1 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/dependency_links.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        6 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/top_level.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      194 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/SOURCES.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    11082 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA.egg-info/PKG-INFO
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-18 06:24:25.000000 pyVIA-0.1.8/pyVIA/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       19 2020-09-15 07:09:22.000000 pyVIA-0.1.8/pyVIA/__init__.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)   306355 2021-01-18 06:16:23.000000 pyVIA-0.1.8/pyVIA/core.py
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)       38 2021-01-19 04:52:20.000000 pyVIA-0.1.9/setup.cfg
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      831 2021-01-19 04:50:44.000000 pyVIA-0.1.9/setup.py
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    15408 2021-01-19 04:51:47.000000 pyVIA-0.1.9/README.md
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    17255 2021-01-19 04:52:20.000000 pyVIA-0.1.9/PKG-INFO
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/pyVIA.egg-info/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      138 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/requires.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)        1 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/dependency_links.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)        6 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/top_level.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      194 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/SOURCES.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    17255 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/PKG-INFO
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/pyVIA/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)       19 2020-09-15 07:09:22.000000 pyVIA-0.1.9/pyVIA/__init__.py
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)   293535 2021-01-19 04:50:36.000000 pyVIA-0.1.9/pyVIA/core.py
```

### Comparing `pyVIA-0.1.8/setup.py` & `pyVIA-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pyVIA',
-    version='0.1.8', #18-Jan-2021
+    version='0.1.9', #18-Jan-2021
     packages=['pyVIA',],
     license='MIT',
     author_email = 'shobana.venkat88@gmail.com',
     url = 'https://github.com/ShobiStassen/VIA',
     setup_requires = ['numpy>=1.17','pybind11'],
-    install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','python-igraph','leidenalg>=0.7.0', 'sklearn', 'termcolor','pygam'],
+    install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','python-igraph','leidenalg>=0.7.0', 'sklearn', 'termcolor','pygam', 'matplotlib','scanpy','umap-learn','phate'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `pyVIA-0.1.8/README.md` & `pyVIA-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,86 @@
 # Via
 VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
 
 ## Getting Started
-### install using pip
+### install using pip takes a few minutes on a clean environment
 We recommend setting up a new conda environment
 ```
 conda create --name ViaEnv pip 
 pip install pyVIA // tested on linux
 ```
+This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
+```
+pip install pybind11
+pip install hnswlib
+pip install pyVIA
+```
 ### install by cloning repository and running setup.py (ensure dependencies are installed)
 ```
 git clone https://github.com/ShobiStassen/VIA.git 
 python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
 ```
 
 ### install dependencies separately if needed (linux)
 If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
 ```
-pip install python-igraph, leidenalg>=0.7.0, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
+pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
 pip install pyVIA
 ```
-## Examples
-### 1.a Human Embryoid Bodies (wrapper function)
-### 1.b Human Embryoid Bodies (Configuring VIA)
-### 2.a Toy Data (multifurcation)
-### 2.b Toy Data (disconnected)
+## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+### 1.a Toy Data (multifurcation)
+### 1.b Toy Data (disconnected)
+### 2.a Human Embryoid Bodies (wrapper function)
+### 2.b Human Embryoid Bodies (Configuring VIA)
 ### 3.a General input format and wrapper function
 ### 3.b General disconnected trajectories wrapper function
 ------------------------------------------------------
-### 1.a Human Embryoid Bodies (wrapper function)
+### 1.a/b Toy data (Multifurcation and Disconnected)
+Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
+```
+import pyVIA.core as via
+#multifurcation
+#the root is automatically set to  root_user = 'M1'
+via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
+#disconnected trajectory
+#the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
+via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
+```
+## Output of Multifurcating toy dataset
+![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
+## Output of disconnected toy dataset
+![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
+
+### 2.a Human Embryoid Bodies (wrapper function)
 save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
 
 The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
 ```
-import pyVia.core as via
+import pyVIA.core as via
 via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
 ```
-### 1.b Human Embryoid Bodies (Configuring VIA)
+### 2.b Human Embryoid Bodies (Configuring VIA)
 If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+Expected runtime will be around 2 minutes
 ```
-import pyVia.core as via
+import pyVIA.core as via
 #pre-process the data as needed and provide to via as a numpy array
 #root_user is the index of the cell corresponding to a suitable start/root cell
 
-v0 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
-             too_big_factor=v0_too_big, root_user=1, dataset='EB', random_seed=v0_random_seed,
+v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+             too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
              do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
 v0.run_VIA()
 
 
 tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
 
-v1 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+v1 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
              too_big_factor=v1_too_big, super_cluster_labels=v0.labels, super_node_degree_list=v0.node_degree_list,
-             super_terminal_cells=tsi_list, root_user=1, is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
+             super_terminal_cells=tsi_list, root_user=[1], is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
              full_distance_array=v0.full_distance_array, ig_full_graph=v0.ig_full_graph,
              csr_array_locally_pruned=v0.csr_array_locally_pruned,
              x_lazy=0.95, alpha_teleport=0.99, preserve_disconnected=True, dataset='EB',
              super_terminal_clusters=v0.terminal_clusters, random_seed=21)
 v1.run_VIA()
 
 #Plot the true and inferred times and pseudotimes
@@ -68,45 +91,27 @@
 ax1.set_title('Embyroid Data: Days')
 ax2.set_title('Embyroid Data: VIA')
 plt.show()
 
 #obtain the single-cell locations of the terminal clusters to be used for visualization of trajectories/lineages 
 super_clus_ds_PCA_loc = via.sc_loc_ofsuperCluster_PCAspace(v0, v1, np.arange(0, len(v1.labels)))
 #draw the overall lineage paths on the embedding
-draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
+via.draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
                          v1.x_lazy, v1.alpha_teleport, v1.single_cell_pt_markov, time_labels, knn=v0.knn,
                          final_super_terminal=v1.revised_super_terminal_clusters,
                          sub_terminal_clusters=v1.terminal_clusters,
                          title_str='Pseudotime and path', ncomp=ncomps)
 
 2D_knn_hnsw = via.make_knn_embeddedspace(Y_phate) #used to visualize the path obtained in the high-dimensional KNN
 #draw the individual lineage paths and cell-fate probabilities at single-cell level 
 via.draw_sc_evolution_trajectory_dijkstra(v1, Y_phate, 2D_knn_hnsw, v0.full_graph_shortpath,
                                       idx=np.arange(0, input_data.shape[0]))
 plt.show()
 ```
 ![Output of VIA on Human Embryoid](https://github.com/ShobiStassen/VIA/blob/master/Figures/EB_fig1.png?raw=true)
-
-
-### 2.a/b Toy data (Multifurcation and Disconnected)
-Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
-```
-import pyVia.core as via
-#multifurcation
-#the root is automatically set to  root_user = 'M1'
-via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
-#disconnected trajectory
-#the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
-via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
-```
-## Output of Multifurcating toy dataset
-![Output of VIA multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
-## Output of disconnected toy dataset
-![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
-
 ### 3.a General input format and wrapper function (uses example of pre-B cell differentiation) 
 Datasets and labels used in this example are provided in [Datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets).
 
 ```
 # Read the two files:
 # 1) the first file contains 200PCs of the Bcell filtered and normalized data for the first 5000 HVG.
 # 2)The second file contains raw count data for marker genes
@@ -126,27 +131,71 @@
 marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
 # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
 via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
             random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
 ```
 ### 3.b VIA wrapper for generic disconnected trajectory
 ```
+import scanpy as sc
+import pandas as pd
+
 #foldername corresponds to the location where you have saved the Toy Disconnected data (shown in example 2)
 #Read in the data and labels
 df_counts = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000.csv", 'rt', delimiter=",")
 df_ids = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000_ids.csv", 'rt', delimiter=",")
 
 # Make AnnData object for wrapper function to read-in data and do PCA
 df_ids['cell_id_num'] = [int(s[1::]) for s in df_ids['cell_id']]
 df_counts = df_counts.drop('Unnamed: 0', 1)
 df_ids = df_ids.sort_values(by=['cell_id_num'])
 df_ids = df_ids.reset_index(drop=True)
 true_label = df_ids['group_id']
 adata_counts = sc.AnnData(df_counts, obs=df_ids)
-sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=ncomps)
+sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=10)
 
 #Since there are 2 disconnected trajectories, we provide 2 arbitrary roots (start cells).If there are more disconnected paths, then VIA arbitrarily selects roots. #The root can also just be arbitrarily set as [1] and VIA can detect how many additional roots it must add
-via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+via.via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
 
 #in the case of connected data (i.e. only 1 graph component. e.g. Toy Data Multifurcating) then the wrapper function from example 3.a can be used:
-#via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
-```
+via.via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+```
+## Parameters and Attributes
+
+### Parameters
+
+| Input Parameter for class VIA | Description |
+| ---------- |----------|
+| `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
+| `true_label` | (list) 'ground truth' annotations or placeholder|
+| `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
+|`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+| `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
+| `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
+| `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
+|`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
+|`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
+| `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
+| `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
+| `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
+| `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
+| `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
+|`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
+|`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
+
+As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
+
+| Input Parameter | Description |
+| ---------- |----------|
+| `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
+|`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
+|`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
+|`full_neighbor_array`|full_neighbor_array=v0.full_neighbor_array. KNN graph from first pass of via - neighbor array|
+|`full_distance_array`|full_distance_array=v0.full_distance_array. KNN graph from first pass of via - edge weights|
+|`ig_full_graph`|ig_full_graph=v0.ig_full_graph igraph of the KNN graph from first pass of via|
+|`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
+
+| Attributes | Description |
+| ---------- |----------|
+| `labels` | (list) length n_samples of corresponding cluster labels |
+| `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
+| `single_cell_pt_markov` | (list) computed pseudotime|
+| `terminal clusters` | (list) terminal clusters found by VIA|
```

### Comparing `pyVIA-0.1.8/PKG-INFO` & `pyVIA-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,93 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Description: # Via
         VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
         
         ## Getting Started
-        ### install using pip
+        ### install using pip takes a few minutes on a clean environment
         We recommend setting up a new conda environment
         ```
         conda create --name ViaEnv pip 
         pip install pyVIA // tested on linux
         ```
+        This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
+        ```
+        pip install pybind11
+        pip install hnswlib
+        pip install pyVIA
+        ```
         ### install by cloning repository and running setup.py (ensure dependencies are installed)
         ```
         git clone https://github.com/ShobiStassen/VIA.git 
         python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
         ```
         
         ### install dependencies separately if needed (linux)
         If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
         ```
-        pip install python-igraph, leidenalg>=0.7.0, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
+        pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
         pip install pyVIA
         ```
-        ## Examples
-        ### 1.a Human Embryoid Bodies (wrapper function)
-        ### 1.b Human Embryoid Bodies (Configuring VIA)
-        ### 2.a Toy Data (multifurcation)
-        ### 2.b Toy Data (disconnected)
+        ## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+        ### 1.a Toy Data (multifurcation)
+        ### 1.b Toy Data (disconnected)
+        ### 2.a Human Embryoid Bodies (wrapper function)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
         ### 3.a General input format and wrapper function
         ### 3.b General disconnected trajectories wrapper function
         ------------------------------------------------------
-        ### 1.a Human Embryoid Bodies (wrapper function)
+        ### 1.a/b Toy data (Multifurcation and Disconnected)
+        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
+        ```
+        import pyVIA.core as via
+        #multifurcation
+        #the root is automatically set to  root_user = 'M1'
+        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
+        #disconnected trajectory
+        #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
+        via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
+        ```
+        ## Output of Multifurcating toy dataset
+        ![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
+        ## Output of disconnected toy dataset
+        ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
+        
+        ### 2.a Human Embryoid Bodies (wrapper function)
         save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
         
         The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
         ```
-        import pyVia.core as via
+        import pyVIA.core as via
         via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
         ```
-        ### 1.b Human Embryoid Bodies (Configuring VIA)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
         If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+        Expected runtime will be around 2 minutes
         ```
-        import pyVia.core as via
+        import pyVIA.core as via
         #pre-process the data as needed and provide to via as a numpy array
         #root_user is the index of the cell corresponding to a suitable start/root cell
         
-        v0 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
-                     too_big_factor=v0_too_big, root_user=1, dataset='EB', random_seed=v0_random_seed,
+        v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+                     too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
                      do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
         v0.run_VIA()
         
         
         tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
         
-        v1 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+        v1 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
                      too_big_factor=v1_too_big, super_cluster_labels=v0.labels, super_node_degree_list=v0.node_degree_list,
-                     super_terminal_cells=tsi_list, root_user=1, is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
+                     super_terminal_cells=tsi_list, root_user=[1], is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
                      full_distance_array=v0.full_distance_array, ig_full_graph=v0.ig_full_graph,
                      csr_array_locally_pruned=v0.csr_array_locally_pruned,
                      x_lazy=0.95, alpha_teleport=0.99, preserve_disconnected=True, dataset='EB',
                      super_terminal_clusters=v0.terminal_clusters, random_seed=21)
         v1.run_VIA()
         
         #Plot the true and inferred times and pseudotimes
@@ -75,45 +98,27 @@
         ax1.set_title('Embyroid Data: Days')
         ax2.set_title('Embyroid Data: VIA')
         plt.show()
         
         #obtain the single-cell locations of the terminal clusters to be used for visualization of trajectories/lineages 
         super_clus_ds_PCA_loc = via.sc_loc_ofsuperCluster_PCAspace(v0, v1, np.arange(0, len(v1.labels)))
         #draw the overall lineage paths on the embedding
-        draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
+        via.draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
                                  v1.x_lazy, v1.alpha_teleport, v1.single_cell_pt_markov, time_labels, knn=v0.knn,
                                  final_super_terminal=v1.revised_super_terminal_clusters,
                                  sub_terminal_clusters=v1.terminal_clusters,
                                  title_str='Pseudotime and path', ncomp=ncomps)
         
         2D_knn_hnsw = via.make_knn_embeddedspace(Y_phate) #used to visualize the path obtained in the high-dimensional KNN
         #draw the individual lineage paths and cell-fate probabilities at single-cell level 
         via.draw_sc_evolution_trajectory_dijkstra(v1, Y_phate, 2D_knn_hnsw, v0.full_graph_shortpath,
                                               idx=np.arange(0, input_data.shape[0]))
         plt.show()
         ```
         ![Output of VIA on Human Embryoid](https://github.com/ShobiStassen/VIA/blob/master/Figures/EB_fig1.png?raw=true)
-        
-        
-        ### 2.a/b Toy data (Multifurcation and Disconnected)
-        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
-        ```
-        import pyVia.core as via
-        #multifurcation
-        #the root is automatically set to  root_user = 'M1'
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
-        #disconnected trajectory
-        #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
-        ```
-        ## Output of Multifurcating toy dataset
-        ![Output of VIA multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
-        ## Output of disconnected toy dataset
-        ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
-        
         ### 3.a General input format and wrapper function (uses example of pre-B cell differentiation) 
         Datasets and labels used in this example are provided in [Datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets).
         
         ```
         # Read the two files:
         # 1) the first file contains 200PCs of the Bcell filtered and normalized data for the first 5000 HVG.
         # 2)The second file contains raw count data for marker genes
@@ -133,29 +138,74 @@
         marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
         # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
         via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
                     random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
         ```
         ### 3.b VIA wrapper for generic disconnected trajectory
         ```
+        import scanpy as sc
+        import pandas as pd
+        
         #foldername corresponds to the location where you have saved the Toy Disconnected data (shown in example 2)
         #Read in the data and labels
         df_counts = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000.csv", 'rt', delimiter=",")
         df_ids = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000_ids.csv", 'rt', delimiter=",")
         
         # Make AnnData object for wrapper function to read-in data and do PCA
         df_ids['cell_id_num'] = [int(s[1::]) for s in df_ids['cell_id']]
         df_counts = df_counts.drop('Unnamed: 0', 1)
         df_ids = df_ids.sort_values(by=['cell_id_num'])
         df_ids = df_ids.reset_index(drop=True)
         true_label = df_ids['group_id']
         adata_counts = sc.AnnData(df_counts, obs=df_ids)
-        sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=ncomps)
+        sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=10)
         
         #Since there are 2 disconnected trajectories, we provide 2 arbitrary roots (start cells).If there are more disconnected paths, then VIA arbitrarily selects roots. #The root can also just be arbitrarily set as [1] and VIA can detect how many additional roots it must add
-        via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+        via.via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
         
         #in the case of connected data (i.e. only 1 graph component. e.g. Toy Data Multifurcating) then the wrapper function from example 3.a can be used:
-        #via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+        via.via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
         ```
+        ## Parameters and Attributes
+        
+        ### Parameters
+        
+        | Input Parameter for class VIA | Description |
+        | ---------- |----------|
+        | `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
+        | `true_label` | (list) 'ground truth' annotations or placeholder|
+        | `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
+        |`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+        | `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
+        | `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
+        | `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
+        |`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
+        |`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
+        | `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
+        | `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
+        | `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
+        | `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
+        | `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
+        |`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
+        |`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
+        
+        As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
+        
+        | Input Parameter | Description |
+        | ---------- |----------|
+        | `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
+        |`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
+        |`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
+        |`full_neighbor_array`|full_neighbor_array=v0.full_neighbor_array. KNN graph from first pass of via - neighbor array|
+        |`full_distance_array`|full_distance_array=v0.full_distance_array. KNN graph from first pass of via - edge weights|
+        |`ig_full_graph`|ig_full_graph=v0.ig_full_graph igraph of the KNN graph from first pass of via|
+        |`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
+        
+        | Attributes | Description |
+        | ---------- |----------|
+        | `labels` | (list) length n_samples of corresponding cluster labels |
+        | `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
+        | `single_cell_pt_markov` | (list) computed pseudotime|
+        | `terminal clusters` | (list) terminal clusters found by VIA|
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyVIA-0.1.8/pyVIA.egg-info/PKG-INFO` & `pyVIA-0.1.9/pyVIA.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,93 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Description: # Via
         VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
         
         ## Getting Started
-        ### install using pip
+        ### install using pip takes a few minutes on a clean environment
         We recommend setting up a new conda environment
         ```
         conda create --name ViaEnv pip 
         pip install pyVIA // tested on linux
         ```
+        This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
+        ```
+        pip install pybind11
+        pip install hnswlib
+        pip install pyVIA
+        ```
         ### install by cloning repository and running setup.py (ensure dependencies are installed)
         ```
         git clone https://github.com/ShobiStassen/VIA.git 
         python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
         ```
         
         ### install dependencies separately if needed (linux)
         If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
         ```
-        pip install python-igraph, leidenalg>=0.7.0, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
+        pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
         pip install pyVIA
         ```
-        ## Examples
-        ### 1.a Human Embryoid Bodies (wrapper function)
-        ### 1.b Human Embryoid Bodies (Configuring VIA)
-        ### 2.a Toy Data (multifurcation)
-        ### 2.b Toy Data (disconnected)
+        ## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+        ### 1.a Toy Data (multifurcation)
+        ### 1.b Toy Data (disconnected)
+        ### 2.a Human Embryoid Bodies (wrapper function)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
         ### 3.a General input format and wrapper function
         ### 3.b General disconnected trajectories wrapper function
         ------------------------------------------------------
-        ### 1.a Human Embryoid Bodies (wrapper function)
+        ### 1.a/b Toy data (Multifurcation and Disconnected)
+        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
+        ```
+        import pyVIA.core as via
+        #multifurcation
+        #the root is automatically set to  root_user = 'M1'
+        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
+        #disconnected trajectory
+        #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
+        via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
+        ```
+        ## Output of Multifurcating toy dataset
+        ![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
+        ## Output of disconnected toy dataset
+        ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
+        
+        ### 2.a Human Embryoid Bodies (wrapper function)
         save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
         
         The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
         ```
-        import pyVia.core as via
+        import pyVIA.core as via
         via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
         ```
-        ### 1.b Human Embryoid Bodies (Configuring VIA)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
         If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+        Expected runtime will be around 2 minutes
         ```
-        import pyVia.core as via
+        import pyVIA.core as via
         #pre-process the data as needed and provide to via as a numpy array
         #root_user is the index of the cell corresponding to a suitable start/root cell
         
-        v0 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
-                     too_big_factor=v0_too_big, root_user=1, dataset='EB', random_seed=v0_random_seed,
+        v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+                     too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
                      do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
         v0.run_VIA()
         
         
         tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
         
-        v1 = VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
+        v1 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
                      too_big_factor=v1_too_big, super_cluster_labels=v0.labels, super_node_degree_list=v0.node_degree_list,
-                     super_terminal_cells=tsi_list, root_user=1, is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
+                     super_terminal_cells=tsi_list, root_user=[1], is_coarse=False, full_neighbor_array=v0.full_neighbor_array,
                      full_distance_array=v0.full_distance_array, ig_full_graph=v0.ig_full_graph,
                      csr_array_locally_pruned=v0.csr_array_locally_pruned,
                      x_lazy=0.95, alpha_teleport=0.99, preserve_disconnected=True, dataset='EB',
                      super_terminal_clusters=v0.terminal_clusters, random_seed=21)
         v1.run_VIA()
         
         #Plot the true and inferred times and pseudotimes
@@ -75,45 +98,27 @@
         ax1.set_title('Embyroid Data: Days')
         ax2.set_title('Embyroid Data: VIA')
         plt.show()
         
         #obtain the single-cell locations of the terminal clusters to be used for visualization of trajectories/lineages 
         super_clus_ds_PCA_loc = via.sc_loc_ofsuperCluster_PCAspace(v0, v1, np.arange(0, len(v1.labels)))
         #draw the overall lineage paths on the embedding
-        draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
+        via.draw_trajectory_gams(Y_phate, super_clus_ds_PCA_loc, v1.labels, v0.labels, v0.edgelist_maxout,
                                  v1.x_lazy, v1.alpha_teleport, v1.single_cell_pt_markov, time_labels, knn=v0.knn,
                                  final_super_terminal=v1.revised_super_terminal_clusters,
                                  sub_terminal_clusters=v1.terminal_clusters,
                                  title_str='Pseudotime and path', ncomp=ncomps)
         
         2D_knn_hnsw = via.make_knn_embeddedspace(Y_phate) #used to visualize the path obtained in the high-dimensional KNN
         #draw the individual lineage paths and cell-fate probabilities at single-cell level 
         via.draw_sc_evolution_trajectory_dijkstra(v1, Y_phate, 2D_knn_hnsw, v0.full_graph_shortpath,
                                               idx=np.arange(0, input_data.shape[0]))
         plt.show()
         ```
         ![Output of VIA on Human Embryoid](https://github.com/ShobiStassen/VIA/blob/master/Figures/EB_fig1.png?raw=true)
-        
-        
-        ### 2.a/b Toy data (Multifurcation and Disconnected)
-        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
-        ```
-        import pyVia.core as via
-        #multifurcation
-        #the root is automatically set to  root_user = 'M1'
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
-        #disconnected trajectory
-        #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
-        ```
-        ## Output of Multifurcating toy dataset
-        ![Output of VIA multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
-        ## Output of disconnected toy dataset
-        ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
-        
         ### 3.a General input format and wrapper function (uses example of pre-B cell differentiation) 
         Datasets and labels used in this example are provided in [Datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets).
         
         ```
         # Read the two files:
         # 1) the first file contains 200PCs of the Bcell filtered and normalized data for the first 5000 HVG.
         # 2)The second file contains raw count data for marker genes
@@ -133,29 +138,74 @@
         marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
         # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
         via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
                     random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
         ```
         ### 3.b VIA wrapper for generic disconnected trajectory
         ```
+        import scanpy as sc
+        import pandas as pd
+        
         #foldername corresponds to the location where you have saved the Toy Disconnected data (shown in example 2)
         #Read in the data and labels
         df_counts = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000.csv", 'rt', delimiter=",")
         df_ids = pd.read_csv(foldername + "toy_disconnected_M9_n1000d1000_ids.csv", 'rt', delimiter=",")
         
         # Make AnnData object for wrapper function to read-in data and do PCA
         df_ids['cell_id_num'] = [int(s[1::]) for s in df_ids['cell_id']]
         df_counts = df_counts.drop('Unnamed: 0', 1)
         df_ids = df_ids.sort_values(by=['cell_id_num'])
         df_ids = df_ids.reset_index(drop=True)
         true_label = df_ids['group_id']
         adata_counts = sc.AnnData(df_counts, obs=df_ids)
-        sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=ncomps)
+        sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=10)
         
         #Since there are 2 disconnected trajectories, we provide 2 arbitrary roots (start cells).If there are more disconnected paths, then VIA arbitrarily selects roots. #The root can also just be arbitrarily set as [1] and VIA can detect how many additional roots it must add
-        via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+        via.via_wrapper_disconnected(adata_counts, true_label, embedding=adata_counts.obsm['X_pca'][:, 0:2], root=[1,1], preserve_disconnected=True, knn=30, ncomps=10,cluster_graph_pruning_std = 1)
         
         #in the case of connected data (i.e. only 1 graph component. e.g. Toy Data Multifurcating) then the wrapper function from example 3.a can be used:
-        #via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
+        via.via_wrapper(adata_counts, true_label, embedding=  adata_counts.obsm['X_pca'][:,0:2], root=[1], knn=30, ncomps=10,cluster_graph_pruning_std = 1)
         ```
+        ## Parameters and Attributes
+        
+        ### Parameters
+        
+        | Input Parameter for class VIA | Description |
+        | ---------- |----------|
+        | `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
+        | `true_label` | (list) 'ground truth' annotations or placeholder|
+        | `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
+        |`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+        | `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
+        | `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
+        | `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
+        |`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
+        |`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
+        | `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
+        | `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
+        | `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
+        | `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
+        | `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
+        |`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
+        |`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
+        
+        As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
+        
+        | Input Parameter | Description |
+        | ---------- |----------|
+        | `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
+        |`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
+        |`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
+        |`full_neighbor_array`|full_neighbor_array=v0.full_neighbor_array. KNN graph from first pass of via - neighbor array|
+        |`full_distance_array`|full_distance_array=v0.full_distance_array. KNN graph from first pass of via - edge weights|
+        |`ig_full_graph`|ig_full_graph=v0.ig_full_graph igraph of the KNN graph from first pass of via|
+        |`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
+        
+        | Attributes | Description |
+        | ---------- |----------|
+        | `labels` | (list) length n_samples of corresponding cluster labels |
+        | `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
+        | `single_cell_pt_markov` | (list) computed pseudotime|
+        | `terminal clusters` | (list) terminal clusters found by VIA|
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyVIA-0.1.8/pyVIA/core.py` & `pyVIA-0.1.9/pyVIA/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import umap
 import phate
 import scanpy as sc
 from scipy.sparse.csgraph import connected_components
 import pygam as pg
 import matplotlib.colors as colors
 import matplotlib.cm as cm
-import palantir
 from termcolor import colored
 import seaborn as sns
 from matplotlib.path import get_path_collection_extents
 
 def getbb(sc, ax):
     """
     Function to return a list of bounding boxes in data coordinates for a scatter plot.
@@ -2159,15 +2158,15 @@
                 loc_i_sc = np.where(np.asarray(sc_pt) <= max_val_pt)[0]
 
                 loc_ = np.intersect1d(loc_i_bp, loc_i_sc)
 
                 gam_in = np.asarray(sc_pt)[loc_]
                 x = gam_in.reshape(-1, 1)
                 y = np.asarray(gene_exp)[loc_].reshape(-1, 1)
-                
+
 
                 weights = np.asarray(sc_bp[:, i])[loc_].reshape(-1, 1)
 
                 if len(loc_) > 1:
                     geneGAM = pg.LinearGAM(n_splines=10, spline_order=4, lam=10).fit(x, y, weights=weights)
                     nx_spacing = 100
                     xval = np.linspace(min(sc_pt), max_val_pt, nx_spacing * 2)
@@ -2220,15 +2219,15 @@
                     geneGAM = pg.LinearGAM(n_splines=10, spline_order=4, lam=10).fit(x, y, weights=weights)
                     nx_spacing = 100
                     xval = np.linspace(min(sc_pt), max_val_pt, nx_spacing * 2)
                     yg = geneGAM.predict(X=xval)
                 else:
                     print('loc_ has length zero')
                 # cmap_[i]
-                ax.plot(xval, yg, color='navy', linewidth=2, zorder=3,
+                ax.plot(xval, yg, color='navy', linewidth=3.5, zorder=3,
                        label='TS:' + str(self.terminal_clusters[i]))
             plt.legend()
             ax.set_title(title_gene)
         return
 
     def do_magic(self, df_gene, magic_steps=3, gene_list=[]):
         # ad_gene is an ann data object from scanpy
@@ -3395,49 +3394,14 @@
             self.f1_accumulated = f1_accumulated
             self.f1_mean = f1_mean
             self.stats_df = df_accuracy
             self.majority_truth_labels = majority_truth_labels
         return
 
 
-def run_palantir_func_human34(ad, ncomps, knn, tsne, revised_clus, start_cell='c4823'):
-    norm_df_pal = pd.DataFrame(ad.X)
-    # print('norm df', norm_df_pal)
-    new = ['c' + str(i) for i in norm_df_pal.index]
-    norm_df_pal.index = new
-    norm_df_pal.columns = [i for i in ad.var_names]
-    pca_projections, _ = palantir.utils.run_pca(norm_df_pal, n_components=ncomps)
-
-    sc.tl.pca(ad, svd_solver='arpack')
-    dm_res = palantir.utils.run_diffusion_maps(pca_projections, n_components=ncomps, knn=knn)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-    print('ms data', ms_data.shape)
-    # tsne =  pd.DataFrame(tsnem)#palantir.utils.run_tsne(ms_data)
-    tsne.index = new
-    # print(type(tsne))
-    str_true_label = pd.Series(revised_clus, index=norm_df_pal.index)
-
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # start_cell = 'c4823'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-
-    pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=1200, knn=knn)
-    palantir.plot.plot_palantir_results(pr_res, tsne, knn, ncomps)
-    # plt.show()
-    imp_df = palantir.utils.run_magic_imputation(norm_df_pal, dm_res)
-    # imp_df.to_csv('/home/shobi/Trajectory/Datasets/HumanCD34/MAGIC_palantir_knn30ncomp100.csv')
-
-    genes = ['GATA1', 'GATA2', 'ITGA2B']  # , 'SPI1']#['CD34','GATA1', 'IRF8','ITGA2B']
-    gene_trends = palantir.presults.compute_gene_trends(pr_res, imp_df.loc[:, genes])
-    palantir.plot.plot_gene_trends(gene_trends)
-    genes = ['MPO', 'ITGAX', 'IRF8', 'CSF1R', 'IL3RA']  # 'CD34','MPO', 'CD79B'
-    gene_trends = palantir.presults.compute_gene_trends(pr_res, imp_df.loc[:, genes])
-    palantir.plot.plot_gene_trends(gene_trends)
-    plt.show()
 
 
 def cellrank_Human(ncomps=80, knn=30, v0_random_seed=7):
     import scvelo as scv
     dict_abb = {'Basophils': 'BASO1', 'CD4+ Effector Memory': 'TCEL7', 'Colony Forming Unit-Granulocytes': 'GRAN1',
                 'Colony Forming Unit-Megakaryocytic': 'MEGA1', 'Colony Forming Unit-Monocytes': 'MONO1',
                 'Common myeloid progenitors': "CMP", 'Early B cells': "PRE_B2", 'Eosinophils': "EOS2",
@@ -3555,16 +3519,14 @@
     df_selected_genes = pd.DataFrame(adata_counts.X, columns=[cc for cc in adata_counts.var_names])
     df_selected_genes = df_selected_genes[genes_save]
     # df_selected_genes.to_csv("/home/shobi/Trajectory/Datasets/HumanCD34/selected_genes.csv")
 
     sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=ncomps)
     marker = ['x', '+', (5, 0), '>', 'o', (5, 2)]
     import colorcet as cc
-    if run_palantir_func == True:
-        run_palantir_func_human34(ad, ncomps, knn, tsne, revised_clus, start_cell='c4823')
 
     # tsnem = TSNE().fit_transform(adata_counts.obsm['X_pca'])
     '''
     f, (ax1, ax2, ax3) = plt.subplots(1, 3, sharey=True)
 
     line = np.linspace(0, 1, len(set(revised_clus)))
 
@@ -3832,56 +3794,32 @@
     sc.tl.paga(adata_counts, groups='leiden')
     # sc.pl.paga(adata_counts, color=['louvain','group_id'])
 
     sc.tl.dpt(adata_counts, n_dcs=ncomps)
     # sc.pl.paga(adata_counts, color=['leiden', 'group_id', 'dpt_pseudotime'],             title=['leiden (knn:' + str(knn) + ' ncomps:' + str(ncomps) + ')',                   'group_id (ncomps:' + str(ncomps) + ')', 'pseudotime (ncomps:' + str(ncomps) + ')'])
     # X = df_counts.values
 
-    print(palantir.__file__)  # location of palantir source code
-    counts = palantir.io.from_csv("/home/shobi/Trajectory/Datasets/Toy4/toy_disconnected_M9_n1000d1000.csv")
-    # counts = palantir.io.from_csv("/home/shobi/Trajectory/Datasets/Toy3/toy_multifurcating_M8_n1000d1000.csv")
-    # counts = palantir.io.from_csv("/home/shobi/Trajectory/Datasets/ToyCyclic/ToyCyclic_M4_n1000d1000.csv")
-    print('counts', counts)
+
     str_true_label = true_label.tolist()
     str_true_label = [(i[1:]) for i in str_true_label]
 
-    str_true_label = pd.Series(str_true_label, index=counts.index)
-    norm_df = counts  # palantir.preprocess.normalize_counts(counts)
-    # palantir
-    '''
-    pca_projections, _ = palantir.utils.run_pca(norm_df, n_components=ncomps)
-    dm_res = palantir.utils.run_diffusion_maps(pca_projections, n_components=ncomps, knn=knn)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-
-    tsne = palantir.utils.run_tsne(ms_data)
-
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-
-    pr_res = palantir.core.run_palantir(ms_data, start_cell, num_waypoints=500, knn=knn)
-    palantir.plot.plot_palantir_results(pr_res, tsne, n_knn=knn, n_comps=ncomps)
-    plt.show()
-    '''
     # clusters = palantir.utils.determine_cell_clusters(pca_projections)
 
     from sklearn.decomposition import PCA
     pca = PCA(n_components=ncomps)
     pc = pca.fit_transform(df_counts)
 
     v0 = VIA(adata_counts.obsm['X_pca'][:, 0:ncomps], true_label, jac_std_global=0.15, dist_std_local=1, knn=knn,
              too_big_factor=0.3, root_user=root_user, preserve_disconnected=True, dataset='toy',
              random_seed=random_seed, is_coarse=True)  # *.4 root=2,
     v0.run_VIA()
     super_labels = v0.labels
 
     super_edges = v0.edgelist
-    super_pt = v0.scaled_hitting_times  # pseudotime pt
-    # 0.05 for p1 toobig
+
 
     p = hnswlib.Index(space='l2', dim=adata_counts.obsm['X_pca'][:, 0:ncomps].shape[1])
     p.init_index(max_elements=adata_counts.obsm['X_pca'][:, 0:ncomps].shape[0], ef_construction=200, M=16)
     p.add_items(adata_counts.obsm['X_pca'][:, 0:ncomps])
     p.set_ef(50)
     tsi_list = []  # find the single-cell which is nearest to the average-location of a terminal cluster in PCA space (
     for tsi in v0.terminal_clusters:
@@ -4157,47 +4095,14 @@
                           'group_id (ncomps:' + str(ncomps) + ')', 'pseudotime (ncomps:' + str(ncomps) + ')'])
         sc.pl.draw_graph(adata_counts, color='dpt_pseudotime', legend_loc='on data')
         print('dpt format', adata_counts.obs['dpt_pseudotime'])
         plt.scatter(embedding[:, 0], embedding[:, 1], c=adata_counts.obs['dpt_pseudotime'].values, cmap='viridis')
         plt.title('PAGA DPT')
         plt.show()
 
-    def run_palantir_func_Bcell(ad1, ncomps, knn, tsne_X, true_label):
-        ad = ad1.copy()
-        tsne = pd.DataFrame(tsne_X, index=ad.obs_names, columns=['x', 'y'])
-        norm_df_pal = pd.DataFrame(ad.X)
-        new = ['c' + str(i) for i in norm_df_pal.index]
-        norm_df_pal.columns = [i for i in ad.var_names]
-        # print('norm df', norm_df_pal)
-
-        norm_df_pal.index = new
-        pca_projections, _ = palantir.utils.run_pca(norm_df_pal, n_components=ncomps)
-
-        sc.tl.pca(ad, svd_solver='arpack')
-        dm_res = palantir.utils.run_diffusion_maps(pca_projections, n_components=ncomps, knn=knn)
-
-        ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-        print('ms data shape: determined using eigengap', ms_data.shape)
-        # tsne =  pd.DataFrame(tsnem)#palantir.utils.run_tsne(ms_data)
-        tsne.index = new
-        # print(type(tsne))
-        str_true_label = pd.Series(true_label, index=norm_df_pal.index)
-
-        palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-        start_cell = 'c42'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-
-        pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=1200, knn=knn)
-        palantir.plot.plot_palantir_results(pr_res, tsne, n_knn=knn, n_comps=ncomps)
-        imp_df = palantir.utils.run_magic_imputation(norm_df_pal, dm_res)
-        Bcell_marker_gene_list = ['Igll1', 'Myc', 'Ldha', 'Foxo1', 'Lig4']  # , 'Slc7a5']#,'Slc7a5']#,'Sp7','Zfp629']
-        gene_trends = palantir.presults.compute_gene_trends(pr_res, imp_df.loc[:, Bcell_marker_gene_list])
-        palantir.plot.plot_gene_trends(gene_trends)
-        plt.show()
-
     def find_time_Bcell(s):
         start = s.find("Ik") + len("Ik")
         end = s.find("h")
         return int(s[start:end])
 
     def find_cellID_Bcell(s):
         start = s.find("h") + len("h")
@@ -5152,58 +5057,14 @@
                          final_super_terminal=v1.revised_super_terminal_clusters,
                          sub_terminal_clusters=v1.terminal_clusters,
                          title_str='Markov Hitting Times (Gams)', ncomp=28)
     # draw_sc_evolution_trajectory_dijkstra(v1, U, knn_hnsw, v0.full_graph_shortpath, np.arange(0, n_umap))
     plt.show()
 
 
-def run_palantir_mESC(ad, knn, tsne, str_true_label, start_cell='c4823'):
-    t0 = time.time()
-    norm_df_pal = pd.DataFrame(ad.X)
-    # print('norm df', norm_df_pal)
-    new = ['c' + str(i) for i in norm_df_pal.index]
-    ncomps = ad.X.shape[1]
-    loc_start = np.where(np.asarray(str_true_label) == '0.0')[0][0]
-    start_cell = 'c' + str(loc_start)
-    print('start cell', start_cell)
-    norm_df_pal.index = new
-    norm_df_pal.columns = [i for i in ad.var_names]
-    # pca_projections, _ = palantir.utils.run_pca(norm_df_pal, n_components=ncomps)
-    # print(type(pca_projections)) Dataframe
-    pca_projections = norm_df_pal
-    # sc.tl.pca(ad, svd_solver='arpack')
-    dm_res = palantir.utils.run_diffusion_maps(pca_projections, knn=knn, n_components=ncomps)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-    print('ms data', ms_data.shape)
-    tsne = pd.DataFrame(tsne, columns=['x', 'y'])  # palantir.utils.run_tsne(ms_data)
-    tsne.index = new
-    # print(type(tsne))
-
-    str_true_label = pd.Series(str_true_label, index=norm_df_pal.index)
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # start_cell = 'c4823'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-    num_waypoints = 1200  # 5000 takes 20 mins and not good. 1200 is default and similar accuracy to 5000wp
-    pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=num_waypoints, knn=knn)
-    print('time end palantir', round(time.time() - t0))
-    palantir.plot.plot_palantir_results(pr_res, tsne, knn, ncomps)
-    # plt.show()
-    imp_df = palantir.utils.run_magic_imputation(norm_df_pal, dm_res)
-    # imp_df.to_csv('/home/shobi/Trajectory/Datasets/HumanCD34/MAGIC_palantir_knn30ncomp100.csv')
-
-    # genes = ['GATA1', 'GATA2', 'ITGA2B']#, 'SPI1']#['CD34','GATA1', 'IRF8','ITGA2B']
-    # gene_trends = palantir.presults.compute_gene_trends( pr_res, imp_df.loc[:, genes])
-    # palantir.plot.plot_gene_trends(gene_trends)
-    # genes = ['MPO','ITGAX','IRF8','CSF1R','IL3RA']#'CD34','MPO', 'CD79B'
-    # gene_trends = palantir.presults.compute_gene_trends(pr_res, imp_df.loc[:, genes])
-    # palantir.plot.plot_gene_trends(gene_trends)
-    plt.show()
-
-
 def paga_faced(ad, knn, embedding, true_label):
     adata_counts = ad.copy()
     adata_counts.obs['group_id'] = true_label
     ncomps = adata_counts.X.shape[1]
     # sc.tl.pca(adata_counts, svd_solver='arpack', n_comps=ncomps)
     adata_counts.uns['iroot'] = 2628  # np.where(np.asarray(adata_counts.obs['group_id']) == '0')[0][0]
 
@@ -5229,121 +5090,14 @@
     # sc.pl.draw_graph(adata_counts, color='dpt_pseudotime', legend_loc='on data')
     # print('dpt format', adata_counts.obs['dpt_pseudotime'])
     plt.scatter(embedding[:, 0], embedding[:, 1], c=adata_counts.obs['dpt_pseudotime'].values, cmap='viridis')
     plt.title('PAGA DPT')
     plt.show()
 
 
-def run_palantir_faced(ad, knn, tsne, str_true_label):
-    t0 = time.time()
-    norm_df_pal = pd.DataFrame(ad.X)
-    # print('norm df', norm_df_pal)
-    new = ['c' + str(i) for i in norm_df_pal.index]
-
-    loc_start = np.where(np.asarray(str_true_label) == 'T1_M1')[0][0]
-    start_cell = 'c' + str(loc_start)
-    print('start cell', start_cell)
-    norm_df_pal.index = new
-    norm_df_pal.columns = [i for i in ad.var_names]
-    ncomps = norm_df_pal.values.shape[1]
-    print('palantir ncomps', ncomps)
-    dm_res = palantir.utils.run_diffusion_maps(norm_df_pal, knn=knn, n_components=ncomps)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-    print('ms data', ms_data.shape)
-    tsne = pd.DataFrame(tsne, columns=['x', 'y'])  # palantir.utils.run_tsne(ms_data)
-    tsne.index = new
-    # print(type(tsne))
-    tsne = palantir.utils.run_tsne(ms_data)
-    str_true_label = pd.Series(str_true_label, index=norm_df_pal.index)
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # start_cell = 'c4823'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-    num_waypoints = 1200  # 1200 default
-    pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=num_waypoints, knn=knn)
-    print('time end palantir', round(time.time() - t0))
-    palantir.plot.plot_palantir_results(pr_res, tsne, knn, ncomps)
-
-
-def run_palantir_EB(ad, ncomps, knn, tsne, str_true_label):
-    t0 = time.time()
-    norm_df_pal = pd.DataFrame(ad.X)
-    # print('norm df', norm_df_pal)
-    new = ['c' + str(i) for i in norm_df_pal.index]
-
-    loc_start = np.where(np.asarray(str_true_label) == '1')[0][0]
-    start_cell = 'c' + str(loc_start)
-    print('start cell', start_cell)
-    norm_df_pal.index = new
-    norm_df_pal.columns = [i for i in ad.var_names]
-    pca_projections, _ = palantir.utils.run_pca(norm_df_pal, n_components=ncomps)
-
-    # sc.tl.pca(ad, svd_solver='arpack')
-    dm_res = palantir.utils.run_diffusion_maps(pca_projections, knn=knn, n_components=ncomps)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap
-    print('ms data', ms_data.shape)
-    tsne = pd.DataFrame(tsne, columns=['x', 'y'])  # palantir.utils.run_tsne(ms_data)
-    tsne.index = new
-    # print(type(tsne))
-
-    str_true_label = pd.Series(str_true_label, index=norm_df_pal.index)
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # start_cell = 'c4823'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-    num_waypoints = 1200  # 1200 default
-    pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=num_waypoints, knn=knn)
-    print('time end palantir', round(time.time() - t0))
-    palantir.plot.plot_palantir_results(pr_res, tsne, knn, ncomps)
-    # plt.show()
-    # imp_df = palantir.utils.run_magic_imputation(norm_df_pal, dm_res)
-    # imp_df.to_csv('/home/shobi/Trajectory/Datasets/HumanCD34/MAGIC_palantir_knn30ncomp100.csv')
-
-    # genes = ['GATA1', 'GATA2', 'ITGA2B']#, 'SPI1']#['CD34','GATA1', 'IRF8','ITGA2B']
-    # gene_trends = palantir.presults.compute_gene_trends( pr_res, imp_df.loc[:, genes])
-    # palantir.plot.plot_gene_trends(gene_trends)
-    # genes = ['MPO','ITGAX','IRF8','CSF1R','IL3RA']#'CD34','MPO', 'CD79B'
-    # gene_trends = palantir.presults.compute_gene_trends(pr_res, imp_df.loc[:, genes])
-    # palantir.plot.plot_gene_trends(gene_trends)
-    plt.show()
-
-
-def palantir_scATAC_Hemato(pc_array, knn, tsne, str_true_label):
-    t0 = time.time()
-    norm_df_pal = pd.DataFrame(pc_array)
-    # print('norm df', norm_df_pal)
-
-    new = ['c' + str(i) for i in norm_df_pal.index]
-
-    # loc_start = np.where(np.asarray(str_true_label) == 'T1_M1')[0][0]
-    start_cell = 'c1200'
-    print('start cell', start_cell)
-    norm_df_pal.index = new
-
-    ncomps = norm_df_pal.values.shape[1]
-    print('palantir ncomps', ncomps)
-    dm_res = palantir.utils.run_diffusion_maps(norm_df_pal, knn=knn, n_components=ncomps)
-
-    ms_data = palantir.utils.determine_multiscale_space(dm_res)  # n_eigs is determined using eigengap.
-    ## In this case n_eigs becomes 1. to increase sensitivity then increase n_eigs in this dataset
-    print('ms data', ms_data.shape)
-    tsne = pd.DataFrame(tsne, columns=['x', 'y'])  # palantir.utils.run_tsne(ms_data)
-    tsne.index = new
-
-    str_true_label = pd.Series(str_true_label, index=norm_df_pal.index)
-    print('c1200 in str true label', str_true_label['c1200'])
-    palantir.plot.plot_cell_clusters(tsne, str_true_label)
-
-    # start_cell = 'c4823'  # '#C108 for M12 connected' #M8n1000d1000 start - c107 #c1001 for bifurc n2000d1000 #disconnected n1000 c108, "C1 for M10 connected" # c10 for bifurcating_m4_n2000d1000
-    num_waypoints = 1200  # 1200  # 1200 default
-    pr_res = palantir.core.run_palantir(ms_data, early_cell=start_cell, num_waypoints=num_waypoints, knn=knn)
-    print('time end palantir', round(time.time() - t0))
-    palantir.plot.plot_palantir_results(pr_res, tsne, knn, ncomps)
-
-
 def main_scATAC_zscores(knn=20, ncomps=30):
     # datasets can be downloaded from the link below
     # https://nbviewer.jupyter.org/github/pinellolab/STREAM/blob/master/tutorial/archives/v0.4.1_and_earlier_versions/4.STREAM_scATAC-seq_k-mers.ipynb?flush_cache=true
 
     # these are the kmers based feature matrix
     # https://www.dropbox.com/sh/zv6z7f3kzrafwmq/AACAlU8akbO_a-JOeJkiWT1za?dl=0
     # https://github.com/pinellolab/STREAM_atac
@@ -5971,14 +5725,15 @@
                 'Phase Fiber Centroid Displacement', 'Phase Fiber Pixel >Upper Percentile', 'Phase Fiber Pixel >Median',
                 'Mean Phase Arrangement', 'Phase Arrangement Var', 'Phase Arrangement Skewness',
                 'Phase Orientation Var', 'Phase Orientation Kurtosis']
     plot_n = 7
     fig, axs = plt.subplots(2, plot_n)  # (2,10)
     for enum_i, pheno_i in enumerate(all_cols[0:14]):  # [0:14]
         subset_ = df[pheno_i].values
+        #subset_ = (subset_ - subset_.mean()) / subset_.std()
         print('subset shape', subset_.shape)
         if enum_i >= plot_n:
             row = 1
             col = enum_i - plot_n
         else:
             row = 0
             col = enum_i
@@ -6023,15 +5778,15 @@
                          final_super_terminal=v1.revised_super_terminal_clusters,
                          sub_terminal_clusters=v1.terminal_clusters,
                          title_str='Hitting times: Markov Simulation on biased edges', ncomp=ncomps)
     plt.show()
 
 
 def main():
-    dataset = 'Toy'  #
+    dataset = 'faced'  #
     # dataset = 'mESC'  # 'EB'#'mESC'#'Human'#,'Toy'#,'Bcell'  # 'Toy'
     if dataset == 'Human':
         main_Human(ncomps=80, knn=30, v0_random_seed=3,
                    run_palantir_func=False)  # 100 comps, knn30, seed=4 is great// pc=100, knn20 rs=1
         # cellrank_Human(ncomps = 20, knn=30)
     elif dataset == 'Bcell':
         main_Bcell(ncomps=20, knn=20, random_seed=1)  # 0 is good
```

