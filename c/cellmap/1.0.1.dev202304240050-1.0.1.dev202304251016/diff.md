# Comparing `tmp/cellmap-1.0.1.dev202304240050-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304251016-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390535 bytes, number of entries: 6
+Zip file size: 1391053 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    63494 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/RECORD
-6 files, 4512858 bytes uncompressed, 1389649 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    66992 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304251016.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304251016.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304251016.dist-info/RECORD
+6 files, 4516356 bytes uncompressed, 1390167 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304240050.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304251016.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304240050.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304251016.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304240050.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304251016.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -24,14 +24,40 @@
 def create_graph(
     X,
     cutedge_vol = None,
     cutedge_length = None,
     cut_std = None,
     return_type = 'edges',
 ):
+    # tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
+    # X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
+    # length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
+    # x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
+    # x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
+    # x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
+    # vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
+    # length_ = np.max([(x1-x2)**2+(y1-y2)**2,(x2-x3)**2+(y2-y3)**2,(x3-x1)**2+(y3-y1)**2],axis=0)
+    # if cut_std == None:
+    #     std_delta_ = 0.1
+    #     std_min_ = 1
+    #     cut_std = std_min_
+    #     while 1:
+    #         if len(np.unique(tri_.edges[length_edge_ < cut_std*np.std(length_edge_)].reshape(-1,1).T[0])) == X.shape[0]:
+    #             break
+    #         cut_std = cut_std + std_delta_
+    # if cutedge_vol == None:
+    #     judge_vol_tri_ = vol_ < cut_std*np.std(vol_)
+    # else:
+    #     judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
+    # if cutedge_length == None:
+    #     judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
+    #     judge_length_tri_= length_ < cut_std*np.std(length_)
+    # else:
+    #     judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
+    #     judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)#np.percentile(length_,100-cutedge_length)
     tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
     X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
     length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
     x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
     x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
     x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
     vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
@@ -49,20 +75,25 @@
     else:
         judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
     if cutedge_length == None:
         judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
         judge_length_tri_= length_ < cut_std*np.std(length_)
     else:
         judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
-        judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)#np.percentile(length_,100-cutedge_length)
-    if return_type == 'edges': return tri_.edges[judge_length_edge_].T
-    if return_type == 'triangles':
-        idx_mask_ = judge_vol_tri_ & judge_length_tri_
-        tri_.set_mask(idx_mask_==False)
-        return tri_,idx_mask_
+        judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)
+    idx_mask_ = judge_vol_tri_ & judge_length_tri_
+    tri_.set_mask(idx_mask_==False)
+    edge_tri_ = np.vstack((np.vstack((tri_.triangles[idx_mask_][:,[0,1]],tri_.triangles[idx_mask_][:,[1,2]])),tri_.triangles[idx_mask_][:,[2,0]]))
+    edge_tri_sort_ = np.array([np.sort(e) for e in edge_tri_])
+    np.sort(edge_tri_sort_,axis=0),np.unique(edge_tri_sort_,axis=0).shape
+    edges_,count_ = np.unique(edge_tri_sort_,axis=0,return_counts=True)
+    idx_bd_ = np.unique(edges_[count_==1].reshape(1,-1)[0])
+    if return_type == 'edges': return edges_.T
+    if return_type == 'edges_bd': return edges_[:,0],edges_[:,1],idx_bd_
+    if return_type == 'triangles': return tri_,idx_mask_
 
 
 
 def check_arguments(
     adata,
     verbose = True,
     **kwargs
@@ -246,14 +277,15 @@
     vkey  = 'velocity',
     exp_key = None,
     potential_key = 'potential',
     rotation_key = 'rotation',
     vorticity_key = 'vorticity',
     streamline_key = 'stream_line',
     graph_key = 'CellMap_graph',
+    edge_vel_key = 'edge_velocity',
     graph_method = 'Delauney',
     HD_rate = 0.0,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     cut_std = None,
@@ -298,16 +330,17 @@
     if logscale_vel:
         vel_HD = (adata.obs['n_counts'].values*vel_HD.T).T/np.exp(exp_HD)
     exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
     vel_LD = adata.obsm[vel_2d_key_][:,:2] if vel_2d_key_ in adata.obsm.keys() else adata.layers[vel_2d_key_][:,:2]
     
     ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
+    idx_bd_  = []
     if graph_method == 'Delauney':
-        source, target = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,cut_std=cut_std,return_type='edges')
+        source, target, idx_bd_ = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,cut_std=cut_std,return_type='edges_bd')
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(exp_HD)
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
@@ -330,68 +363,89 @@
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
     lap = -np.dot(div_mat,grad_mat)
     edge_vel = (1-HD_rate)*edge_vel_LD+HD_rate*edge_vel_HD
     source_term = np.dot(div_mat,edge_vel)
-    lap_inv = np.linalg.pinv(lap)
-    potential = np.dot(lap_inv,source_term)
+    # for i in idx_bd_:
+    #     lap[i,:] = 0
+    #     lap[i,i] = 1
+    #     source_term[i] = 0
+    lap_inv_ = np.linalg.pinv(lap)
+    potential = np.dot(lap_inv_,source_term)
     pot_flow_ = -np.dot(grad_mat,potential)
     rot_flow_ = edge_vel - pot_flow_
     adata.obs[potential_key] = potential - np.min(potential)
 
 
     # Compute potential & rotational flow
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
     vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
+    src_trg_ = np.hstack((source,target))
+    trg_src_ = np.hstack((target,source))
+    pot_flow_2_ = np.hstack((pot_flow_,-pot_flow_))
+    rot_flow_2_ = np.hstack((rot_flow_,-rot_flow_))
+    edge_vel_norm = np.linalg.norm(edge_velocity(exp_LD,vel_LD,source,target,normalization=False))
     if graph_method == 'Delauney':
-        edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
         for i in range(adata.shape[0]):
-            idx_s = source == i
-            idx_t = target == i
-            if sum(idx_s) > 0:
-                ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
-                vel_potential[i] += 2*np.linalg.norm(edge_vel)*np.sum(pot_flow_[idx_s]*ex_s.T,axis=1)
-                vel_rotation[i]  += 2*np.linalg.norm(edge_vel)*np.sum(rot_flow_[idx_s]*ex_s.T,axis=1)
-            if sum(idx_t) > 0:
-                ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
-                edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
-                vel_potential[i] += -2*np.linalg.norm(edge_vel)*np.sum(pot_flow_[idx_t]*ex_t.T,axis=1)
-                vel_rotation[i]  += -2*np.linalg.norm(edge_vel)*np.sum(rot_flow_[idx_t]*ex_t.T,axis=1)
+            idx_ = src_trg_ == i
+            ex_s = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]])/np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],ord=2)
+            vel_potential[i] = edge_vel_norm*edge_vel_norm*np.sum(pot_flow_2_[idx_]*ex_s.T,axis=1)
+            vel_rotation[i]  = edge_vel_norm*edge_vel_norm*np.sum(rot_flow_2_[idx_]*ex_s.T,axis=1)
+            # idx_s = source == i
+            # idx_t = target == i
+            # if sum(idx_s) > 0:
+            #     ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
+            #     vel_potential[i] += 2*edge_vel_norm*np.sum(pot_flow_[idx_s]*ex_s.T,axis=1)
+            #     vel_rotation[i]  += 2*edge_vel_norm*np.sum(rot_flow_[idx_s]*ex_s.T,axis=1)
+            # if sum(idx_t) > 0:
+            #     ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
+            #     vel_potential[i] += -2*edge_vel_norm*np.sum(pot_flow_[idx_t]*ex_t.T,axis=1)
+            #     vel_rotation[i]  += -2*edge_vel_norm*np.sum(rot_flow_[idx_t]*ex_t.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
         # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
         adata.obsm[rot_vkey_] = vel_rotation
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
-            vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
+            vel_potential[i] = -edge_vel_norm*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
         # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
         adata.obsm[rot_vkey_] = vel_rotation
     
+    # for i in idx_bd_:
+    #     lap[i,:] = 0
+    #     lap[i,i] = 1
+    # lap_inv_ = np.linalg.pinv(lap)
     ## Solve vorticity & stream line
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target))
-    stream_line_ = -np.dot(lap_inv,vorticity_)
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
+    source_term_ = vorticity_
+    # source_term_[idx_bd_] = 100
+    stream_line_ = -np.dot(lap_inv_,source_term_)
     # vorticity_ = -np.dot(lap,stream_line_)
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = stream_line_-np.min(stream_line_)
 
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target))
-    stream_line_ = -np.dot(lap_inv,vorticity_)
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
+    source_term_ = vorticity_
+    # source_term_[idx_bd_] = 100
+    stream_line_ = -np.dot(lap_inv_,source_term_)
     # vorticity_ = -np.dot(lap,stream_line_)
     adata.obs[pot_vor_key_] = vorticity_
     adata.obs[pot_sl_key_] = stream_line_-np.min(stream_line_)
 
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target))
-    stream_line_ = -np.dot(lap_inv,vorticity_)
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
+    source_term_ = vorticity_
+    # source_term_[idx_bd_] = 100
+    stream_line_ = -np.dot(lap_inv_,source_term_)
     # vorticity_ = -np.dot(lap,stream_line_)
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = stream_line_-np.min(stream_line_)
 
     adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
@@ -400,15 +454,16 @@
     norm_grad = np.linalg.norm(pot_flow_)
     norm_curl = np.linalg.norm(rot_flow_)
     log_["Contribution_ratio"]['Potential'] = '{:.2%}'.format(norm_grad/(norm_grad+norm_curl))
     log_["Contribution_ratio"]['Rotation']  = '{:.2%}'.format(norm_curl/(norm_grad+norm_curl))
     adata.uns['CellMap_log'] = log_
     if verbose: print(adata.uns['CellMap_log'])
 
-    if graph_key not in adata.uns.keys(): adata.uns[graph_key] = np.vstack((source,target))
+    adata.uns[graph_key] = {'source':source,'target':target}
+    adata.uns[edge_vel_key] = {edge_vel_key:edge_vel,edge_vel_key+'_pot':pot_flow_,edge_vel_key+'_rot':rot_flow_}
 
 def Hodge_decomposition_genes(
     adata,
     genes,
     basis = 'umap',
     vkey  = 'velocity',
     exp_key = None,
@@ -1272,15 +1327,15 @@
 
 
 def view_trajectory(
     adata,
     source_cluster,
     target_clusters,
     n_cells = 50,
-    register = 10,
+    register = 100,
     basis = 'umap',
     potential_key = 'potential',
     cluster_key = 'clusters',
     graph_method = 'Delauney',
     path_key = 'path',
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
@@ -1310,19 +1365,27 @@
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(data_pos.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
+    
+    G = nx.Graph()
+    for i in range(len(source)):
+        G.add_edge(source[i],target[i],w=np.linalg.norm(data_pos[source[i]]-data_pos[target[i]]))
+    degree_centrality = nx.degree_centrality(G)
 
     G = nx.DiGraph()
+    dis_mean = np.mean(np.linalg.norm(data_pos[source]-data_pos[target],axis=1))
 
     def cost(data_pos,s,t,g,reg):
-        return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])
+        # return np.exp(-g*reg*(degree_centrality[s]+degree_centrality[t]))*np.linalg.norm(data_pos[s]-data_pos[t])
+        return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])*np.exp(np.linalg.norm(data_pos[s]-data_pos[t])/dis_mean)
+    
     grad_ = adata.obs[potential_key][source].values - adata.obs[potential_key][target].values
     G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
     G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
     G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
     G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
     
     cmap_ = plt.get_cmap("tab10")
@@ -1409,16 +1472,17 @@
                     x_data = np.append(x_data,np.linspace(0,1,len(pi)))
                     y_data = np.append(y_data,data_exp[:,adata.var.index==gene][pi])
                 X = x_data[:, np.newaxis]
                 poly = PolynomialFeatures(degree=10)
                 X_poly = poly.fit_transform(X)
                 model = LinearRegression()
                 model.fit(X_poly, y_data)
-                plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05)
+                plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05,zorder=0)
                 plot_x = np.linspace(0,1,100)
-                plt.plot(plot_x, model.predict(poly.fit_transform(plot_x[:, np.newaxis])),color=cmap_(i),lw=5,label=target_clusters[i])
+                plt.plot(plot_x, model.predict(poly.fit_transform(plot_x[:, np.newaxis])),color='w',lw=8,zorder=1)
+                plt.plot(plot_x, model.predict(poly.fit_transform(plot_x[:, np.newaxis])),color=cmap_(i),lw=5,label=target_clusters[i],zorder=2)
             plt.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0,title='Target', fontsize=fontsize_legend, title_fontsize=fontsize_legend)
             plt.xticks([0,1],['Source\n(%s)' % source_cluster,'Target'],fontsize=fontsize_label)
             plt.title(gene,fontsize=fontsize_title)
             plt.show()
         else:
             print('Gene \"%s\" was not found' % gene)
```

## Comparing `cellmap-1.0.1.dev202304240050.dist-info/METADATA` & `cellmap-1.0.1.dev202304251016.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304240050
+Version: 1.0.1.dev202304251016
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

