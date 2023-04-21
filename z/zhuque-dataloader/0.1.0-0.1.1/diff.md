# Comparing `tmp/zhuque-dataloader-0.1.0.tar.gz` & `tmp/zhuque-dataloader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.1.0.tar", last modified: Thu Apr 20 08:56:43 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.1.1.tar", last modified: Fri Apr 21 01:46:31 2023, max compression
```

## Comparing `zhuque-dataloader-0.1.0.tar` & `zhuque-dataloader-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:56:43.185425 zhuque-dataloader-0.1.0/
--rw-rw-rw-   0        0        0      192 2023-04-20 08:56:43.185425 zhuque-dataloader-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    13680 2023-04-20 08:55:22.000000 zhuque-dataloader-0.1.0/loader.py
--rw-rw-rw-   0        0        0       42 2023-04-20 08:56:43.186426 zhuque-dataloader-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-04-20 08:56:31.000000 zhuque-dataloader-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:56:43.183426 zhuque-dataloader-0.1.0/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-20 08:56:43.000000 zhuque-dataloader-0.1.0/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 08:56:43.000000 zhuque-dataloader-0.1.0/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:56:43.000000 zhuque-dataloader-0.1.0/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 08:56:43.000000 zhuque-dataloader-0.1.0/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 01:46:31.028503 zhuque-dataloader-0.1.1/
+-rw-rw-rw-   0        0        0      192 2023-04-21 01:46:31.027501 zhuque-dataloader-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13683 2023-04-21 01:45:41.000000 zhuque-dataloader-0.1.1/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:46:31.028503 zhuque-dataloader-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-21 01:46:27.000000 zhuque-dataloader-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:46:31.025502 zhuque-dataloader-0.1.1/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-21 01:46:30.000000 zhuque-dataloader-0.1.1/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-21 01:46:30.000000 zhuque-dataloader-0.1.1/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:46:30.000000 zhuque-dataloader-0.1.1/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 01:46:30.000000 zhuque-dataloader-0.1.1/zhuque_dataloader.egg-info/top_level.txt
```

### Comparing `zhuque-dataloader-0.1.0/loader.py` & `zhuque-dataloader-0.1.1/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,17 @@
             "mountPath": "/zhuque_goofys"
         }
     }
 }
 
 
 def load_graph(args):
-    data_name = args.data_name
     data_loader = args.data_loader
-    frame_type = args.frame_type
-    if not data_name or not data_loader or not frame_type:
-        raise Exception('please check dataset parameters')
+    if not data_loader:
+        raise Exception('please check dataloader parameters')
     dataloader_path = os.path.join(LOCAL_DATALOADER_PATH, data_loader + '.yml')
     try:
         dl_file = open(dataloader_path, "r", encoding="UTF-8")
         dataloader = yaml.load(dl_file, Loader=yaml.FullLoader)
     except:
         raise Exception('read dataloader file error')
 
@@ -67,40 +65,42 @@
     if storage_format in ['csv', 'ogb'] and 'platform' not in dataloader.keys():
         raise Exception('check the dataloader, platform does not exsits')
 
     # 朱雀平台格式csv数据集
     if storage_format == 'csv':
         platform = dataloader['platform']
         if platform == 'graphscope':
-            return load_graph_csv_gs(data_name, dataloader)
+            return load_graph_csv_gs(dataloader)
         elif platform == 'wholegraph':
-            return load_graph_wg(data_name)
+            return load_graph_wg(dataloader['dataset'])
     elif storage_format == 'ogb':
         platform = dataloader['platform']
         if platform == 'ogbofficial':
-            return load_graph_ogb_official(dataloader, frame_type)
+            return load_graph_ogb_official(dataloader, args.frame_type)
         elif platform == 'wholegraph':
-            return load_graph_wg(data_name)
+            return load_graph_wg(dataloader['ogbName'])
         elif platform == 'graphscope':
-            return load_graph_ogb_gs(data_name, dataloader)
+            return load_graph_ogb_gs(dataloader)
     elif storage_format in ('npy', 'npz'):
         return load_graph_numpy(dataloader)
     elif storage_format == 'other':
-        return load_graph_other(dataloader, args.data_path)
+        return load_graph_other(dataloader)
 
     raise Exception('load data fail')
 
 
 
 # 加载ogb格式数据集 官方方式
 def load_graph_ogb_official(dataloader, frame_type):
     from ogb.graphproppred import PygGraphPropPredDataset, DglGraphPropPredDataset, GraphPropPredDataset
     from ogb.linkproppred import PygLinkPropPredDataset, DglLinkPropPredDataset, LinkPropPredDataset
     from ogb.nodeproppred import PygNodePropPredDataset, DglNodePropPredDataset, NodePropPredDataset
 
+    if not frame_type:
+        raise Exception('please check frame info')
     ogb_name = dataloader['ogbName']
     ogb_root = dataloader['ogbRoot']
     task = get_ogb_task(ogb_name)
     params = []
     normal_ogb_name = ogb_name.replace("_", "-")
     params.append('name=\'' + normal_ogb_name + '\'')
     params.append('root=\'' + ogb_root + '\'')
@@ -141,15 +141,15 @@
         raise Exception('task not supported')
 
     train_data, valid_data, test_data = load_pickle_data(ogb_root, normal_graph_name, True)
     return train_data, valid_data, test_data
 
 
 # 加载ogb格式数据集 在graphscope框架
-def load_graph_ogb_gs(data_name, dataloader):
+def load_graph_ogb_gs(dataloader):
     import graphscope as gs
     from graphscope.dataset.ogbl_collab import load_ogbl_collab
     from graphscope.dataset.ogbl_ddi import load_ogbl_ddi
     from graphscope.dataset.ogbn_arxiv import load_ogbn_arxiv
     from graphscope.dataset.ogbn_mag import load_ogbn_mag
     from graphscope.dataset.ogbn_proteins import load_ogbn_proteins
 
@@ -184,27 +184,28 @@
     params = dataloader['params']
     obj_str = 'np.load' + construct_param(params)
     print(obj_str)
     return eval(obj_str)
 
 
 # 加载other格式数据集
-def load_graph_other(dataloader, data_path):
+def load_graph_other(dataloader):
     code = dataloader['code']
     print(code)
     exec_data = {}
     exec(code, globals(), exec_data)
     return exec_data["data"]
 
 
 # 加载csv格式数据集在graphscope框架
-def load_graph_csv_gs(data_name, dataloader):
+def load_graph_csv_gs(dataloader):
     import graphscope
     # from graphscope.dataset import *
 
+    data_name = dataloader['dataset']
     data_path = os.path.join(LOCAL_DATASET_PATH, data_name)
     sess = graphscope.session(mount_dataset="/dataset", k8s_volumes=k8s_volumes, k8s_coordinator_cpu=4,
                               k8s_coordinator_mem="8Gi")
     if dataloader["oidType"] == 'string':
         graph = sess.g(oid_type=dataloader["oidType"])
     else:
         graph = sess.g()
@@ -218,24 +219,25 @@
         pro = []
         for feature in value['features']:
             pro.append((feature['name'], feature['type']))
         graph = graph.add_edges(os.path.join(data_path, value['path']), label=key, src_label=value['srcLabel'],
                                 dst_label=value['dstLabel'], src_field=0, dst_field=1, properties=pro)
     return graph
 
-def load_graph_csv_wg_old(data_name, dataloader):
+def load_graph_csv_wg_old(dataloader):
     from wg_torch.graph_ops import (
         graph_name_normalize, load_pickle_data
     )
     from zhuque_graph.dataloader.wholegraph.homograph_data_convert_node_classification import \
         homograph_data_convert_node_classification
     from zhuque_graph.dataloader.wholegraph.homograph_data_convert_link_prediction import \
         homograph_data_convert_link_prediction
 
     task = dataloader['task']
+    data_name = dataloader['dataset']
     data_path = os.path.join(LOCAL_DATASET_PATH, data_name)
     if not task or not data_name:
         raise Exception('please check task or dataset name')
     node_name = ''
     node_file = ''
     edge_name = ''
     edge_file = ''
```

### Comparing `zhuque-dataloader-0.1.0/setup.py` & `zhuque-dataloader-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhuque-dataloader',
-    version='0.1.0',
+    version='0.1.1',
     description='zhuque graph platform dataloader component',
     author='yanrisheng',
     author_email='yanrs@zhejianglab.com',
     packages=find_packages(),
     py_modules=['loader'],
     requires=[],  # 定义依赖
     license='GPL 3.0'
```

