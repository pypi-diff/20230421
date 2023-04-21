# Comparing `tmp/cellmap-1.0.1.dev202304200124-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304210546-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390356 bytes, number of entries: 6
+Zip file size: 1390469 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    63297 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304200124.dist-info/RECORD
-6 files, 4512661 bytes uncompressed, 1389470 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    63503 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210546.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210546.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304210546.dist-info/RECORD
+6 files, 4512867 bytes uncompressed, 1389583 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304200124.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304210546.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304200124.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304210546.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304200124.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304210546.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -2,15 +2,14 @@
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.cm
 import matplotlib.colors
 from matplotlib import patheffects as PathEffects
-
 import networkx as nx
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 import pandas as pd
@@ -20,38 +19,42 @@
 import scanpy
 import scvelo as scv
 
 
 
 def create_graph(
     X,
-    Y,
     cutedge_vol = None,
     cutedge_length = None,
     cut_std = 1,
-    return_mask = False
+    return_type = 'edges',
 ):
-    tri_ = matplotlib.tri.Triangulation(X,Y)
-    x1,y1 = X[tri_.triangles[:,0]],Y[tri_.triangles[:,0]]
-    x2,y2 = X[tri_.triangles[:,1]],Y[tri_.triangles[:,1]]
-    x3,y3 = X[tri_.triangles[:,2]],Y[tri_.triangles[:,2]]
-    vol = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
-    length = np.max([(x1-x2)**2+(y1-y2)**2,(x2-x3)**2+(y2-y3)**2,(x3-x1)**2+(y3-y1)**2],axis=0)
+    tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
+    X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
+    length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
+    x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
+    x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
+    x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
+    vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
+    length_ = np.max([(x1-x2)**2+(y1-y2)**2,(x2-x3)**2+(y2-y3)**2,(x3-x1)**2+(y3-y1)**2],axis=0)
     if cutedge_vol == None:
-        judge_vol = vol < cut_std*np.std(vol)
+        judge_vol_tri_ = vol_ < cut_std*np.std(vol_)
     else:
-        judge_vol = vol < np.percentile(vol,100-cutedge_vol)
+        judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
     if cutedge_length == None:
-        judge_length = length < cut_std*np.std(length)
+        judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
+        judge_length_tri_= length_ < cut_std*np.std(length_)
     else:
-        judge_length = length < np.percentile(length,100-cutedge_length)
-    tri_mask_ = judge_vol & judge_length
-    tri_.set_mask(tri_mask_==False)
-    if return_mask: return tri_,tri_mask_
-    else: return tri_
+        judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
+        judge_length_tri_ = length_ < np.percentile(length_,100-cutedge_length)
+    if return_type == 'edges': return tri_.edges[judge_length_edge_].T
+    if return_type == 'triangles':
+        idx_mask_ = judge_vol_tri_ & judge_length_tri_
+        tri_.set_mask(idx_mask_==False)
+        return tri_,idx_mask_
 
 
 
 def check_arguments(
     adata,
     verbose = True,
     **kwargs
@@ -203,18 +206,19 @@
         normalization = True,
 ):
     idx_vel = np.isnan(vel[0])==False
     X1,X2 = X[:,idx_vel][source],X[:,idx_vel][target]
     V1,V2 = vel[:,idx_vel][source],vel[:,idx_vel][target]
     Dis = np.linalg.norm(X2-X1,axis=1)
     Dis[Dis==0] = 1
-    V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
-    V1_p[V1_p<0] = 0
-    V2_p[V2_p<0] = 0
-    edge_vel = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/np.sum(idx_vel)
+    # V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
+    # V1_p[V1_p<0] = 0
+    # V2_p[V2_p<0] = 0
+    # edge_vel = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/np.sum(idx_vel)
+    edge_vel = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel)
     if normalization:
         edge_vel_norm = np.linalg.norm(edge_vel)
         if edge_vel_norm > 0: edge_vel= edge_vel/edge_vel_norm
     return edge_vel
 
 def solve_vorticity_streamline(
     div_mat,
@@ -286,16 +290,15 @@
         vel_HD = (adata.obs['n_counts'].values*vel_HD.T).T/np.exp(exp_HD)
     exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
     vel_LD = adata.obsm[vel_2d_key_][:,:2] if vel_2d_key_ in adata.obsm.keys() else adata.layers[vel_2d_key_][:,:2]
     
     ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
-        tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
-        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+        source, target = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(exp_HD)
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
@@ -320,44 +323,50 @@
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
     lap = -np.dot(div_mat,grad_mat)
     edge_vel = (1-HD_rate)*edge_vel_LD+HD_rate*edge_vel_HD
     source_term = np.dot(div_mat,edge_vel)
     lap_inv = np.linalg.pinv(lap)
     potential = np.dot(lap_inv,source_term)
-    pot_flow = -np.dot(grad_mat,potential)
+    pot_flow_ = -np.dot(grad_mat,potential)
+    rot_flow_ = edge_vel - pot_flow_
     adata.obs[potential_key] = potential - np.min(potential)
 
 
-    ## Compute potential & rotational flow
+    # Compute potential & rotational flow
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
-    # vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
+    vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
     if graph_method == 'Delauney':
-        tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
-        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+        edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
         for i in range(adata.shape[0]):
             idx_s = source == i
             idx_t = target == i
-            ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
-            ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
-            edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
-            vel_potential[i] = 2*np.linalg.norm(edge_vel)*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
-                                np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
+            if sum(idx_s) > 0:
+                ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
+                vel_potential[i] += 2*np.linalg.norm(edge_vel)*np.sum(pot_flow_[idx_s]*ex_s.T,axis=1)
+                vel_rotation[i]  += 2*np.linalg.norm(edge_vel)*np.sum(rot_flow_[idx_s]*ex_s.T,axis=1)
+            if sum(idx_t) > 0:
+                ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
+                edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
+                vel_potential[i] += -2*np.linalg.norm(edge_vel)*np.sum(pot_flow_[idx_t]*ex_t.T,axis=1)
+                vel_rotation[i]  += -2*np.linalg.norm(edge_vel)*np.sum(rot_flow_[idx_t]*ex_t.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
+        # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
+        adata.obsm[rot_vkey_] = vel_rotation
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
             vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
+        # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
+        adata.obsm[rot_vkey_] = vel_rotation
     
     ## Solve vorticity & stream line
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target))
     stream_line_ = -np.dot(lap_inv,vorticity_)
     # vorticity_ = -np.dot(lap_inv,stream_line_)
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = stream_line_-np.min(stream_line_)
@@ -370,22 +379,21 @@
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target))
     stream_line_ = -np.dot(lap_inv,vorticity_)
     # vorticity_ = -np.dot(lap_inv,stream_line_)
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = stream_line_-np.min(stream_line_)
 
-    rot_flow = edge_vel - pot_flow
-    adata.obs[rotation_key] = np.array([np.mean(np.vstack((rot_flow[source==i],-rot_flow[target==i]))) for i in range(adata.shape[0])])
+    adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
     log_ = {}
     log_["Contribution_ratio"] = {}
-    norm_grad = np.linalg.norm(pot_flow)
-    norm_curl = np.linalg.norm(rot_flow)
+    norm_grad = np.linalg.norm(pot_flow_)
+    norm_curl = np.linalg.norm(rot_flow_)
     log_["Contribution_ratio"]['Potential'] = '{:.2%}'.format(norm_grad/(norm_grad+norm_curl))
     log_["Contribution_ratio"]['Rotation']  = '{:.2%}'.format(norm_curl/(norm_grad+norm_curl))
     adata.uns['CellMap_log'] = log_
     if verbose: print(adata.uns['CellMap_log'])
 
     if graph_key not in adata.uns.keys(): adata.uns[graph_key] = np.vstack((source,target))
 
@@ -438,16 +446,16 @@
     vel_HD = adata.obsm[vkey] if vkey in adata.obsm.keys() else adata.layers[vkey]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
     exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
     
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
-        tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
-        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+        source, target = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
+        # source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(exp_HD)
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate])
         knn = NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
@@ -503,15 +511,15 @@
         figsize = (10,6) if cbar else (8,6)
         
 
     data_pos = adata.obsm[basis_key]
     fig,ax = plt.subplots(figsize=figsize)
     sc = ax.scatter(data_pos[:,0],data_pos[:,1],c=adata.obs[color_key],zorder=10,**kwargs)
     if show_graph:
-        tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+        tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
         ax.tripcolor(tri_,adata.obs[color_key],lw=0.5,zorder=0,alpha=0.3,cmap=kwargs['cmap'])
     if cluster_key != None:
         if cluster_key in adata.obs.keys():
             cluster = adata.obs[cluster_key]
             for c in np.unique(cluster):
                 txt = plt.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=fontsize_text,ha='center', va='center',fontweight='bold',zorder=20)
                 txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
@@ -542,15 +550,15 @@
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
     data_pos = adata.obsm[basis_key]
     fig,ax = plt.subplots(figsize=(8,6))
-    tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+    tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     sc = ax.tricontourf(tri_,adata.obs[potential_key],zorder=0,alpha=0.9,cmap=kwargs['cmap'],levels=100)
     if cluster_key in adata.obs.keys():
         cluster = adata.obs[cluster_key]
         idx_random = np.zeros(cluster.shape,dtype=bool)
         np.random.seed(seed)
         idx_random[np.random.choice(len(idx_random),min(n_points,len(idx_random)),replace=False)] = True
         cluster_set = np.unique(cluster)
@@ -586,15 +594,15 @@
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
 
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[color_key])
     
     data_pos = adata.obsm[basis_key]
-    tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+    tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     fig,ax = plt.subplots(figsize=(8,6))
     cntr = ax.tricontourf(tri_,adata.obs[color_key],cmap=kwargs['cmap'],levels=100,zorder=2)
     fig.colorbar(cntr, shrink=0.75, orientation='vertical').set_label(color_key,fontsize=20)
     if show_graph: ax.triplot(tri_,color='w',lw=0.5,zorder=10,alpha=1)
     ax.set_xlim(np.min(data_pos[:,0])-0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])),np.max(data_pos[:,0])+0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])))
     ax.set_ylim(np.min(data_pos[:,1])-0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])),np.max(data_pos[:,1])+0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])))
     ax.tick_params(labelbottom=False,labelleft=False,labelright=False,labeltop=False,bottom=False,left=False,right=False,top=False)
@@ -676,15 +684,15 @@
     
     key_ = '%s_%s' % (contour_key,basis)
     pot_key_ = '%s_%s_%s' % (potential_key,contour_key,basis)
     rot_key_ = '%s_%s_%s' % (rotation_key,contour_key,basis)
     
     
     data_pos = adata.obsm[basis_key]
-    tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+    tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     
     contour_keys = [key_, pot_key_, rot_key_]
     camps = [cmap_earth(adata.obs[key_]),'rainbow','coolwarm']
     titles = ['RNA velocity orbit','Development orbit','Periodic orbit']
     
     fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
     for i in range(3):
@@ -790,15 +798,15 @@
     vel_HD = adata.obsm[vkey] if vkey in adata.obsm.keys() else adata.layers[vkey]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
     
     data_pos = adata.obsm[basis_key]
-    tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+    tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     
     for gene in genes:
         fig,ax = plt.subplots(1,3,figsize=(45,10))
         cntr = ax[0].tricontourf(tri_,np.squeeze(exp_HD[:,adata.var.index==gene]),cmap=kwargs['cmap'],levels=100,zorder=2)
         fig.colorbar(cntr, shrink=0.75, orientation='vertical',ax=ax[0]).set_label('gene expression',fontsize=20)
         ax[0].set_title('%s_expression' % gene,fontsize=18)
         cntr = ax[1].tricontourf(tri_,np.squeeze(vel_HD[:,adata.var.index==gene]),cmap=kwargs['cmap'],levels=100,zorder=2)
@@ -852,15 +860,15 @@
 
     x,y,z = adata.obsm[basis_key][:,0], adata.obsm[basis_key][:,1],adata.obs[potential_key]
     
     c_list  = ['#0938BF','#50D9FB','#B7E5FA','#98D685','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09']
     c_level = [0,5,20,40,60,75,80,85,90,95,99,100]
     custom_cmap = [[0.01*c_level[i],c_list[i]] for i in range(len(c_list))]
 
-    tri_,idx_tri = create_graph(x,y,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+    tri_,idx_tri = create_graph(adata.obsm[basis_key],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type = 'triangles')
     triangles = tri_.triangles[idx_tri]
 
     camera = dict(eye=dict(x=1.8, y=-1.0, z=1.8))
     idx = np.zeros(adata.shape[0],dtype=bool)
     np.random.seed(seed)
     idx[np.random.choice(adata.shape[0],min(n_points,adata.shape[0]),replace=False)] = True
     shift = 0.01*(max(z)-min(z))
@@ -1007,15 +1015,15 @@
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
     data_pos = adata.obsm[basis_key]
-    tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+    tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     fig = plt.figure(figsize=(15,15))
     ax = fig.add_subplot(111, projection='3d')
     cntr = ax.plot_trisurf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],zorder=2)
     ax.set_box_aspect(aspect = (1,1,0.8))
     fig.colorbar(cntr, shrink=0.5, orientation='vertical').set_label(potential_key,fontsize=20)
     ax.set_title(title,fontsize=18)
     if cluster_key != None:
@@ -1051,15 +1059,15 @@
                                  potential_key = potential_key,
                                  graph_key = graph_key,
                                 )
         basis = kwargs_arg['basis']
         basis_key = 'X_%s' % basis
 
         data_pos = adata.obsm[basis_key]
-        tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
+        tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
         if 'cmap' not in kwargs:
             kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
         fig = plt.figure(figsize=(15,15))
         ax = fig.add_subplot(111, projection='3d')
         cntr = ax.plot_trisurf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],zorder=2,alpha=0.9)#,cmap=cmap_CellMap,levels=100)
         ax.set_box_aspect(aspect = (1,1,0.8))
         ax.set_title(title,fontsize=18)
@@ -1196,16 +1204,15 @@
                              basis = basis,
                              map_key = map_key
                             )
     basis,map_key = kwargs_arg['basis'],kwargs_arg['map_key']
     basis_key = 'X_%s' % basis
     
     data_pos = adata.obsm[basis_key]
-    triangles = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length).triangles
-    tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+    tri_,idx_tri = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
     triangles = tri_.triangles[idx_tri]
     n_node_ = data_pos.shape[0]
     graph_ = scipy.sparse.lil_matrix(np.zeros([n_node_,n_node_]))
     idx_set = [[0,1],[1,2],[2,0]]
     # idx = np.isnan(data_vel[0])==False
     for id_x,id_y in idx_set:
         weight = adata.obs[potential_key][triangles[:,id_y]].values - adata.obs[potential_key][triangles[:,id_x]].values
@@ -1238,16 +1245,15 @@
                              map_key = map_key
                             )
     basis,vkey,map_key = kwargs_arg['basis'],kwargs_arg['vkey'],kwargs_arg['map_key']
     basis_key = 'X_%s' % basis
     
     data_pos = adata.obsm[basis_key]
     data_vel = adata.obsm['%s_%s' % (vkey,basis)]
-    triangles = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length).triangles
-    tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+    tri_,idx_tri = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
     triangles = tri_.triangles[idx_tri]
     n_node_ = data_pos.shape[0]
     graph_ = scipy.sparse.lil_matrix(np.zeros([n_node_,n_node_]))
     idx_set = [[0,1],[1,2],[2,0]]
     idx = np.isnan(data_vel[0])==False
     for id_x,id_y in idx_set:
         X1 = data_pos[:,idx][triangles[:,id_x]]
@@ -1289,16 +1295,16 @@
             raise KeyError('Cluster %s was not found' % trg_)
 
     basis_key = 'X_%s' % basis
     data_pos = adata.obsm[basis_key]
 
     ## Compute graph and edge velocities
     if graph_method == 'Delauney':
-        tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
-        source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
+        tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
+        source, target = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(data_pos)
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
@@ -1363,23 +1369,23 @@
     adata.uns[path_key] = path_all
 
 def path_gene_profile(
     adata,
     source_cluster,
     target_clusters,
     genes,
+    cluster_key = 'clusters',
     path_key = 'path',
     exp_key = None,
     fontsize_title = 16,
     fontsize_label = 14,
     fontsize_legend = 12,
 ):
     
-    kwargs_arg = check_arguments(adata, verbose = True, basis=basis)
-    basis = kwargs_arg['basis']
+    kwargs_arg = check_arguments(adata, verbose = True)
 
     if sum(adata.obs[cluster_key].values == source_cluster) == 0:
         raise KeyError('Cluster %s was not found' % source_cluster)
     for trg_ in target_clusters:
         if sum(adata.obs[cluster_key].values == source_cluster) == 0:
             raise KeyError('Cluster %s was not found' % trg_)
```

## Comparing `cellmap-1.0.1.dev202304200124.dist-info/METADATA` & `cellmap-1.0.1.dev202304210546.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304200124
+Version: 1.0.1.dev202304210546
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

