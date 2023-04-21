# Comparing `tmp/pcg_skel-0.3.1.tar.gz` & `tmp/pcg_skel-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcg_skel-0.3.1.tar", last modified: Wed Jan 18 21:58:37 2023, max compression
+gzip compressed data, was "pcg_skel-0.3.3.tar", last modified: Fri Apr 21 20:17:47 2023, max compression
```

## Comparing `pcg_skel-0.3.1.tar` & `pcg_skel-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-01-18 21:58:37.819034 pcg_skel-0.3.1/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)    12288 2023-01-18 21:58:37.818815 pcg_skel-0.3.1/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)    11994 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-01-18 21:58:37.817539 pcg_skel-0.3.1/pcg_skel/
--rw-r--r--   0 caseysm    (501) staff       (20)      117 2023-01-18 21:57:53.000000 pcg_skel-0.3.1/pcg_skel/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1926 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/chunk_cache.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13567 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/chunk_tools.py
--rw-r--r--   0 caseysm    (501) staff       (20)     7074 2023-01-18 21:46:20.000000 pcg_skel-0.3.1/pcg_skel/features.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5931 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/pcg_anno.py
--rw-r--r--   0 caseysm    (501) staff       (20)    31511 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/pcg_skel.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3216 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/skel_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2867 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/pcg_skel/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-01-18 21:58:37.818609 pcg_skel-0.3.1/pcg_skel.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)    12288 2023-01-18 21:58:37.000000 pcg_skel-0.3.1/pcg_skel.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      391 2023-01-18 21:58:37.000000 pcg_skel-0.3.1/pcg_skel.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-01-18 21:58:37.000000 pcg_skel-0.3.1/pcg_skel.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2023-01-18 21:58:37.000000 pcg_skel-0.3.1/pcg_skel.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        9 2023-01-18 21:58:37.000000 pcg_skel-0.3.1/pcg_skel.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-01-18 21:58:37.819078 pcg_skel-0.3.1/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1467 2022-11-15 01:01:33.000000 pcg_skel-0.3.1/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.782776 pcg_skel-0.3.3/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-21 20:17:47.782168 pcg_skel-0.3.3/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     9871 2023-03-08 00:43:18.000000 pcg_skel-0.3.3/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.781076 pcg_skel-0.3.3/pcg_skel/
+-rw-r--r--   0 caseysm    (501) staff       (20)      117 2023-04-21 20:17:35.000000 pcg_skel-0.3.3/pcg_skel/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1926 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/pcg_skel/chunk_cache.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15449 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/chunk_tools.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11760 2023-04-21 18:23:20.000000 pcg_skel-0.3.3/pcg_skel/features.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    25012 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/nocache.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6211 2023-04-21 18:54:26.000000 pcg_skel-0.3.3/pcg_skel/pcg_anno.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    36782 2023-04-21 20:14:20.000000 pcg_skel-0.3.3/pcg_skel/pcg_skel.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3216 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/pcg_skel/skel_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2866 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.781924 pcg_skel-0.3.3/pcg_skel.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      411 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      112 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        9 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      112 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-21 20:17:47.782872 pcg_skel-0.3.3/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1467 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/setup.py
```

### Comparing `pcg_skel-0.3.1/LICENSE.txt` & `pcg_skel-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.1/PKG-INFO` & `pcg_skel-0.3.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,271 +1,157 @@
-Metadata-Version: 2.1
-Name: pcg_skel
-Version: 0.3.1
-Summary: Skeletonization using the pychunkedgraph
-Home-page: https://github.com/AllenInstitute/pcg_skel
-Author: Casey Schneider-mizell
-Author-email: caseys@alleninstitute.org
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7703278.svg)](https://doi.org/10.5281/zenodo.7703278)
 
 # pcg_skel
 
-Save time by generating robust neuronal skeletons directly from a ChunkedGraph dynamic segmentations!
+Generate robust neuronal topology directly from PyChunkedGraph dynamic segmentations.
 
-## What you need
-
-For skeletons you just need a dynamic segmentation running on a [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) server.
-
-To also use annotations, you also need a database backend running the [MaterializationEngine](https://github.com/seung-lab/MaterializationEngine).
-
-## Key terms
-
-Ids in the PCG combine information about chunk level, spatial location, and unique object id.
-This package uses the highest-resolution chunking, level 2, to derive neuronal topology and approximate spatial extent.
-For clarity, I'll define a few terms:
-
-* *L2 object*: Collection of attributes (supervoxels, mesh, etc) associated with a level 2 id.
+Skeletonization is an essential part of measuring neuronal anatomy, but in 3d segmented data it is not always trivial to produce a skeleton.
+Segmentations and meshes are often prohibitively large to download *en mass* and can artifacts that generate ambiguities or make attaching annotations like synapses to specific locations unclear.
 
-* *L2 mesh*: The fragment of mesh associated with a level 2 id.
+PCG-skel uses the same chunking that allows the [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) (PCG) to quickly make edits to large, complex neuronal segmentations and, combined with a dynamic caching system that updates after every edit, can generate complete representations of the topology of objects in just a few seconds and minimal data downloads.
+Becuase the data is always matched to the underlying representation of the segmentation, there are no ambiguities in what parts are connected to what other or in which vertex a synapse or other annotation is associated with.
+This light data needs and rapid skeletonization make it useful in environments where analysis is being re-run on frequently changing cells.
 
-* *Chunk index/chunk index space*: The integer 3-d index of a chunk in the the grid that covers the volume, i.e. the chunk index space.
+However, there is a trade-off in terms of resolution.
+The dependency on chunk size means that vertices are roughly a chunk width apart, which in current datasets amounts to about 2 microns.
+Thus for understanding the overall structure of a cell or looking at long distance relationships between points along an arbor, these skeletons are quite good, but for detailed analysis at short length scales (0-10 microns or so) where being plus or minus a micron would hurt analysis, I recommend looking at other approaches like kimimaro, meshteasar, or CGAL skeletonization.
 
-* *Euclidean position/Euclidean space*: A position in nanometers / biological space.
 
-* *Chunk position*: The center of a specific chunk index in Euclidean space
-
-* *Refinement*: Mapping the position of an L2 object from its chunk position to a more representitive point on the mesh.
-
-## How to use
+## Example of usage
 
-There are a few potentially useful functions with progressively more features:
+It is highly recommended to run PCGSkel with a [CAVE client](https://caveclient.readthedocs.io/).
 
-### chunk_index_skeleton
-
-This function returns a meshparty skeleton with vertices given in chunk index space.
+The most basic way to get a skeleton requires only a root id and CAVEclient.
 
 ```python
-def chunk_index_skeleton(root_id,
-                         client=None,
-                         datastack_name=None,
-                         cv=None,
-                         root_point=None,
-                         invalidation_d=3,
-                         return_mesh=False,
-                         return_l2dict=False,
-                         return_mesh_l2dict=False,
-                         root_point_resolution=[4, 4, 40],
-                         root_point_search_radius=300,
-                         n_parallel=1):
-```
-
-#### Notes
-
-* A `CAVEclient` or `datastack_name` must be provided, and a cloudvolume object is suggested for performance reasons, especially if running in bulk.
-
-* If `root_point` is set, the function looks within `root_point_search_radius` for the closest point in the root_id segmentation and sets the associated level 2 ID as the root vertex. `root_point_search_radius` is in nanometers. `root_point` is in units of `root_point_resolution`, such that root_point * root_point_resolution should be correct in Euclidean space.
-
-* `return_mesh` will also return the full graph of level 2 objects as a `meshparty.Mesh` that has no faces and uses only link edges. Vertices are in chunk index space.
-
-* `return_l2dict` will also return a tuple of two dictionaries. The first, `l2dict`, is a dict mapping level 2 id to skeleton vertex index. This is one to many, since it includes passing through multiple level 2 ids that belong to the mesh and are collapsed into a common skeleton vertex. The second, `l2dict_reversed`, is a dict mapping skeleton vertex to level 2 id. This is one to one.
-
-* `return_mesh_l2dict` will return an additional tuple of two dictionaries. The first maps level 2 ids to mesh vertices, the second mesh vertex index to level 2 id.
-
-* `n_parallel` is passed directly to cloudvolume and can speed up mesh fragment downloading.
-
----
-
-### refine_chunk_index_skeleton
-
-Map a skeleton in chunk index space into Euclidean space.
+from caveclient import CAVEclient
+import pcg_skel
 
-```python
-def refine_chunk_index_skeleton(
-    sk_ch,
-    l2dict_reversed,
-    cv,
-    refine_inds='all',
-    scale_chunk_index=True,
-    root_location=None,
-    nan_rounds=20,
-    return_missing_ids=False,
-):
+client = CAVEclient('minnie65_phase3_v1')
+root_id = 864691135867734294
+sk = pcg_skel.coord_space_skeleton(root_id, client)
 ```
 
-#### Notes
+This generates a skeleton, in this case for a pyramidal cell in the MICrONs65 volume, in just a few seconds — less time than is needed to download the mesh itself. The skeleton is shown in black, and the mesh in red.
 
-* `sk_ch` is assumed to have positions in chunk index space.
+![pyramidal cell](example_skeleton.png)
 
-* `l2dict_reversed` is the second dict that comes back in the tuple you get by setting `return_l2dict` to `True` in `chunk_index_skeleton`.
+## What you need
 
-* `refine_inds` can be either `"all"` or a specific array of vertex indices. This parameter sets which vertices to refine. A handful of vertices can be processed very quickly, while a more accurate skeleton is generated by refining all vertices.
+PCG-skel requires an active [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) server.
 
-* `scale_chunk_index`, if True, will still map unrefined vertex indices from their chunk index into the chunk position in eucliden space.
+For best performance, your dataset should have an L2 Cache, a service that caches representive points and features for every chunk.
+Using the CAVEclient, you can test for this by running `client.l2cache.attributes`.
+If you get a list of attribute names back, you're good!
+If you don't have an L2 cache and still want to use PCG Skel, see the section below `How to use without an L2 Cache`.
 
-* `nan_rounds` gives how many times to try to smoothly interpolate any vertices that did not get a position due to a missing L2 mesh fragment.
+To also use annotations, you also need a database backend running the [MaterializationEngine](https://github.com/seung-lab/MaterializationEngine).
 
-* `return_missing_ids` will also return a list of the ids of any missing L2 mesh fragment, for example if you want to re-run meshing on them.
+## Key terms
 
----
+Ids in the PCG combine information about chunk level, spatial location, and unique object id.
+This package uses the highest-resolution chunking, level 2, to derive neuronal topology and approximate spatial extent.
+For clarity, I'll define a few terms:
 
-### pcg_skeleton
+* *Level 2 chunk*: A box defining a unit of data storage and representation. The entire dataset is tiled by nonoverlapping chunks. Each chunk has properties like a detailed graph of which supervoxels touch what other supervoxels, meshes associated with each segmented object inside the chunk, etc. By chunking the data and agglomerating larger objects out of these chunks, edits only have to touch those few chunks that actually change during proofreading, reducing the amount of memory and effort needed to process them.
 
-Directly build a skeleton in Euclidean space, plus optionally handle soma points.
+Chunks can exist at many scales, but "level 2" refers to the lowest level of chunking (level 1 refers to the supervoxels themselves).
 
-```python
-def pcg_skeleton(root_id,
-                 client=None,
-                 datastack_name=None,
-                 cv=None,
-                 refine='all',
-                 root_point=None,
-                 root_point_resolution=[4, 4, 40],
-                 root_point_search_radius=300,
-                 collapse_soma=False,
-                 collapse_radius=10_000.0,
-                 invalidation_d=3,
-                 return_mesh=False,
-                 return_l2dict=False,
-                 return_l2dict_mesh=False,
-                 return_missing_ids=False,
-                 nan_rounds=20,
-                 n_parallel=1):
-```
+* *Level 2 id (L2 id)*: A segmentation id that describes the state of the segmentation inside a given L2 chunk.
+Note that if two distinct parts of the same neuron enter the same chunk, each has its own level 2 id.
 
-#### Notes
+* *Level 2 graph*: Each level 2 id can be thought of as connected to level 2 ids in other chunks when an object's supervoxels run across chunk boundaries or where edges have introduced by merges during proofreading. The graph of which level 2 ids are connected to which others is called the "level 2 graph." Keeping track of the level 2 graph is one of the jobs of the PCG.
 
-* `refine` can take five values to determine which vertices to refine.
-    1. `"all"`: Refine all vertices
-    2. `"ep"`: Refine only end points.
-    3. `"bp"`: Refine only branch points.
-    4. `"bpep"` or `"epbp"`: Refine both branch and end points.
-    5. `None`: Don't refine any vertex, but still map chunk positions coarsely.
+* *Level 2 skeleton*: A reduced version of the level 2 graph that is tree-like.
 
-    Options which download few mesh fragments are much faster than `"all"`.
+* *Representitative point*: For each level 2 id, the L2 Cache determines a representative point that is guaranteed to be within the segmentation and is located at a "most central" point in the segmentation of the L2 id.
 
-* `collapse_soma`, if set to True, collapses all mesh vertices within `collapse_radius` into the root point.
-Note that the root point is not a new point, but rather the closest level 2 object to the root point location.
+## How to use
 
----
+There are three main functions to generate a neuronal representation from the pychunkedgraph and L2 Cache that build on one another. One gets the L2 graph, one processes it into an L2 skeleton, and a third collects the graph and skeleton together into a "Meshwork" object that can also handle annotations.
 
-### pcg_meshwork
+### Skeletons
 
-Build a meshwork file with skeleton out from the level 2 graph.
-Optionally, attach pre- and/or post-synaptic synapses.
+This function will return a meshparty Skeleton class. Skeleton features can be found in the [Meshparty documentation](https://meshparty.readthedocs.io/en/latest/).
 
 ```python
-def pcg_meshwork(root_id,
-                 datastack_name=None,
-                 client=None,
-                 cv=None,
-                 refine='all',
-                 root_point=None,
-                 root_point_resolution=[4, 4, 40],
-                 root_point_search_radius=300,
-                 collapse_soma=False,
-                 collapse_radius=DEFAULT_COLLAPSE_RADIUS,
-                 synapses=None,
-                 synapse_table=None,
-                 remove_self_synapse=True,
-                 invalidation_d=3,
-                 n_parallel=4,
-                 ):
+def coord_space_skeleton(
+    root_id,
+    client,
+    cv=None,
+    invalidation_d=10_000,
+    return_mesh=False,
+    return_l2dict=False,
+    return_l2dict_mesh=False,
+    root_point=None,
+    root_point_resolution=None,
+    collapse_soma=False,
+    collapse_radius=7500,
+):
 ```
 
-#### Notes
+The basic use requires only a root id and a caveclient, but there are a number of important options.
 
-* The resulting meshwork file comes back with a "mesh" made out of the level 2 graph with vertices mapped to their chunk positions, a skeleton with `refine` and `collapse_soma` options as above, and one or more annotations.
+* *cv*: Passing an initialized cloudvolume object (`cv=`) can save a second or two per skeleton. This isn't a big deal for a couple of skeletons, but may save some real time if you are creating a large number of skeletons.
 
-* All resulting meshworks have the annotation `lvl2_ids`, which is based on a dataframe with column `lvl2_id` that has level 2 ids and `mesh_ind` that has the associated mesh index.
-One can use the MeshIndex/SkeletonIndex properties like `nrn.anno.mesh_index.to_skel_index` to see the associated skeleton indices.
+* *invalidation_d*: The invalidation distance for skeletonization, in nanometers. This parameter sets the distance at which vertices of the graph are collapsed into a branch. Too big and branches might be missed, but too small and false branches might be added to thick processes. This is an important parameter to customize for your data, since different morphologies will be best represented by different values. The default value works well for cortical neurons, for example, but is probably too coarse for fly neurons.
 
-* If the `synapses` property is set to `"pre"`, `"post"`, or `"all"`, there is also an attempt to look up the root id's presynaptic synapses, postsynaptic synapses, or both (respectively).
-Presynaptic synapses are in an annotation `"pre_syn"` and postsynaptic synapses are in an annotation called `"post_syn"`.
+* *return_mesh*, *return_l2dict*, *return_l2dict_mesh*: These three values are all set to False by default, which is fine if you just want a skeleton. However, if you want to map vertices to level 2 ids or skeleton vertices back to the mesh graph, these options can give you the mesh and dictionaries mapping vertices to the l2 ids for the skeletons and the mesh graph.
 
-* If returning synapses, you must set the synapse table.
-By default, synapses whose pre- and post-synaptic ids are both the same root id are excluded, but this can be turned off by setting `remove_self_synapse` to `False`.
+* *root_point*, *root_point_resolution*: Setting a root point defines the root of the skeleton, which establishes an orientation for the skeleton. Root point is an x,y,z position, and the resolution is the value in nm of the resolution of coordinates (also in x,y,z, resolution). If the point is from neuroglancer or an annotation table, take careful note of the resolution. 
 
-## Example
+* *collapse_soma*, *collapse_radius*: These two options let you collapse vertices around a soma into the root point. Setting collapse_soma to True will collapse all vertices within the collapse radius (in nanometers) into the root point. Additionally, the root point is added as a new skeleton vertex. Again, the default value works for most cortical neurons, but cells with larger or smaller cell bodies might need different values.
 
-A minimal example to get the skeleton of an arbitrary neuron with root id `864691135761488438` and soma at the voxel-space location `253870, 236989, 20517` in the Minnie dataset:
 
-```python
-from caveclient import CAVEclient
-import pcg_skel
-
-client = CAVEclient('minnie65_phase3_v1')
-
-oid = 864691135761488438 # Root id
-root_point = [253870, 236989, 20517] # root point in vertex coordinates
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              client=client,
-                              refine='all',
-                              root_point=root_point,
-                              root_point_resolution=[4,4,40],
-                              collapse_soma=True,
-                              n_parallel=8)
-```
+### Mesh graph
 
-To generate a skeleton with 1310 vertices took about 80 seconds on a 2019 MacBook Pro, all refined through the mesh fragments.
-Most of the time is spent in refinement.
-If you just select the `refine="epbp"` argument, it only refines the 79 branch and end points and accordingly takes a mere 12.5 seconds.
-It is worth exploring sparse refinement options and interpolation if processing time is extremely important.
-
-## Caching
-
-A common use case is to have a set of neurons that you are analyzing while proofreading is still ongoing.
-However, because proofreading events leave most of the neuron unchanged we shouldn't need to do more than update new locations.
-Conveniently, the level 2 ids let us follow this intuition.
-While a neuron's root id changes for each proofreading event, the level 2 id only changes if an edit occurs exactly within that region.
-Therefore, once we've looked up a level 2 id once, we can cache it and save time for future iterations on the same neuron.
-
-The current implementation of caching uses [SQLiteDict](https://github.com/piskvorky/sqlitedict), a simple means of using a sqlite file as a persistent key-value store.
-The cache is used with the functions `refine_vertices`, `pcg_skeleton`, and `pcg_meshwork` if you specify the filename of the sqlite database.
-For example,
+This function will return a meshparty Mesh object, with a vertex at the representative point for every l2 id and edges where they connect to one another.
+Such a mesh is what the skeleton returned above is generated from.
 
 ```python
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              ...,
-                              cache='l2_cache.sqlite',
-                              save_to_cache=False,
-                              )
+def coord_space_mesh(
+    root_id,
+    client,
+    cv=None,
+    return_l2dict=False,
+):
 ```
 
-Note that if the database is not yet present, it will be created automatically.
-
-In order to avoid unintentional changes, new locations are not saved to the database by default.
-If you want to save new ids to the database as you are skeletonizing files, set the additional parameter `save_to_cache=True`.
-For adding data to the database post-hoc, please use the function `chunk_cache.save_ids_to_cache()`.
-
-## Segmentation-based localization
+There are fewer options, since the mesh graph is a more direct representation of the data.
 
-Localizing level 2 ids with mesh fragments is much faster than downloading the segmentation for a whole chunk just to get a few supervoxels, but sometimes mesh fragments don't exist.
-This can occur for both good reasons (the L2 object is too small to get a mesh) and due to bugs in the meshing backend.
-However, if you really want to get such locations correct, falling back to the segmentation is available.
+### Meshwork file
 
-You can use this by setting the `segmentation_fallback` option on any of the functions that localize vertices.
-For example,
+Meshwork files combine the mesh graph, the skeleton, and annotations linked together. They are more complex objects, but can be useful for a number of tasks and analyses.
 
 ```python
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              ...,
-                              segmentation_fallback=True,
-                              fallback_mip=2,
-                              )
+def coord_space_meshwork(
+    root_id,
+    datastack_name=None,
+    client=None,
+    cv=None,
+    root_point=None,
+    root_point_resolution=None,
+    collapse_soma=False,
+    collapse_radius=7500,
+    synapses=None,
+    synapse_table=None,
+    remove_self_synapse=True,
+    live_query=False,
+    timestamp=None,
+    invalidation_d=7500,
+):
 ```
 
-Setting `segmentation_fallback=True` activates the capability, and setting `fallback_mip` will choose the MIP-level to use (2 by default).
-If the chosen MIP does not have voxels for the L2 id in it, it will try 0 next.
-Segmentation-based points will be cached if both features are used.
+Many of the parameters are the same as in skeletonization. In addition, there are parameters controlling the addition of synapses.
+
+* *synapses*, *synapse_table*: If set to `"pre"`, `"post"`, or `"both"`, the after skeletonization the system will add pre, post, or both pre and postsynaptic annotations using the specified synapse table to the meshwork under `nrn.anno.pre_syn` and `nrn.anno.post_syn` respectively. Note that by default, `remove_self_synapse` will omit all synapses whose pre and post ids are the same neuron. This is a common form of errors, particularly around the nucleus, although it can also remove biologically real autapses.
+
+* *live_query*, *timestamp*: If live_query is True, sets the timestamp at which annotations are from. If not set, uses the most materialization defined in the caveclient.
 
-Note that this approach is much slower and more memory intensive than using the mesh fragments.
-I have found it to take 4-8 seconds per vertex with the current implementation, although parallelation helps.
 
-## To-dos
+## How to use without an L2 Cache
 
-* Improve/document/test tooling for additional annotations.
-* Alternative key-value stores for caching
+See the `nocache.md` file for instructions on how to use without a L2 cache for the chunkedgraph.
 
 ## Credit
 
 This work is by Casey Schneider-Mizell (caseys@alleninstitute.org) with suggestions from Sven Dorkenwald and Forrest Collman.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pcg_skel-0.3.1/README.md` & `pcg_skel-0.3.3/pcg_skel.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,261 +1,167 @@
-# pcg_skel
-
-Save time by generating robust neuronal skeletons directly from a ChunkedGraph dynamic segmentations!
-
-## What you need
-
-For skeletons you just need a dynamic segmentation running on a [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) server.
-
-To also use annotations, you also need a database backend running the [MaterializationEngine](https://github.com/seung-lab/MaterializationEngine).
+Metadata-Version: 2.1
+Name: pcg-skel
+Version: 0.3.3
+Summary: Skeletonization using the pychunkedgraph
+Home-page: https://github.com/AllenInstitute/pcg_skel
+Author: Casey Schneider-mizell
+Author-email: caseys@alleninstitute.org
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-## Key terms
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7703278.svg)](https://doi.org/10.5281/zenodo.7703278)
 
-Ids in the PCG combine information about chunk level, spatial location, and unique object id.
-This package uses the highest-resolution chunking, level 2, to derive neuronal topology and approximate spatial extent.
-For clarity, I'll define a few terms:
-
-* *L2 object*: Collection of attributes (supervoxels, mesh, etc) associated with a level 2 id.
+# pcg_skel
 
-* *L2 mesh*: The fragment of mesh associated with a level 2 id.
+Generate robust neuronal topology directly from PyChunkedGraph dynamic segmentations.
 
-* *Chunk index/chunk index space*: The integer 3-d index of a chunk in the the grid that covers the volume, i.e. the chunk index space.
+Skeletonization is an essential part of measuring neuronal anatomy, but in 3d segmented data it is not always trivial to produce a skeleton.
+Segmentations and meshes are often prohibitively large to download *en mass* and can artifacts that generate ambiguities or make attaching annotations like synapses to specific locations unclear.
 
-* *Euclidean position/Euclidean space*: A position in nanometers / biological space.
+PCG-skel uses the same chunking that allows the [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) (PCG) to quickly make edits to large, complex neuronal segmentations and, combined with a dynamic caching system that updates after every edit, can generate complete representations of the topology of objects in just a few seconds and minimal data downloads.
+Becuase the data is always matched to the underlying representation of the segmentation, there are no ambiguities in what parts are connected to what other or in which vertex a synapse or other annotation is associated with.
+This light data needs and rapid skeletonization make it useful in environments where analysis is being re-run on frequently changing cells.
 
-* *Chunk position*: The center of a specific chunk index in Euclidean space
+However, there is a trade-off in terms of resolution.
+The dependency on chunk size means that vertices are roughly a chunk width apart, which in current datasets amounts to about 2 microns.
+Thus for understanding the overall structure of a cell or looking at long distance relationships between points along an arbor, these skeletons are quite good, but for detailed analysis at short length scales (0-10 microns or so) where being plus or minus a micron would hurt analysis, I recommend looking at other approaches like kimimaro, meshteasar, or CGAL skeletonization.
 
-* *Refinement*: Mapping the position of an L2 object from its chunk position to a more representitive point on the mesh.
 
-## How to use
+## Example of usage
 
-There are a few potentially useful functions with progressively more features:
+It is highly recommended to run PCGSkel with a [CAVE client](https://caveclient.readthedocs.io/).
 
-### chunk_index_skeleton
-
-This function returns a meshparty skeleton with vertices given in chunk index space.
+The most basic way to get a skeleton requires only a root id and CAVEclient.
 
 ```python
-def chunk_index_skeleton(root_id,
-                         client=None,
-                         datastack_name=None,
-                         cv=None,
-                         root_point=None,
-                         invalidation_d=3,
-                         return_mesh=False,
-                         return_l2dict=False,
-                         return_mesh_l2dict=False,
-                         root_point_resolution=[4, 4, 40],
-                         root_point_search_radius=300,
-                         n_parallel=1):
-```
-
-#### Notes
-
-* A `CAVEclient` or `datastack_name` must be provided, and a cloudvolume object is suggested for performance reasons, especially if running in bulk.
-
-* If `root_point` is set, the function looks within `root_point_search_radius` for the closest point in the root_id segmentation and sets the associated level 2 ID as the root vertex. `root_point_search_radius` is in nanometers. `root_point` is in units of `root_point_resolution`, such that root_point * root_point_resolution should be correct in Euclidean space.
-
-* `return_mesh` will also return the full graph of level 2 objects as a `meshparty.Mesh` that has no faces and uses only link edges. Vertices are in chunk index space.
-
-* `return_l2dict` will also return a tuple of two dictionaries. The first, `l2dict`, is a dict mapping level 2 id to skeleton vertex index. This is one to many, since it includes passing through multiple level 2 ids that belong to the mesh and are collapsed into a common skeleton vertex. The second, `l2dict_reversed`, is a dict mapping skeleton vertex to level 2 id. This is one to one.
-
-* `return_mesh_l2dict` will return an additional tuple of two dictionaries. The first maps level 2 ids to mesh vertices, the second mesh vertex index to level 2 id.
-
-* `n_parallel` is passed directly to cloudvolume and can speed up mesh fragment downloading.
-
----
-
-### refine_chunk_index_skeleton
-
-Map a skeleton in chunk index space into Euclidean space.
+from caveclient import CAVEclient
+import pcg_skel
 
-```python
-def refine_chunk_index_skeleton(
-    sk_ch,
-    l2dict_reversed,
-    cv,
-    refine_inds='all',
-    scale_chunk_index=True,
-    root_location=None,
-    nan_rounds=20,
-    return_missing_ids=False,
-):
+client = CAVEclient('minnie65_phase3_v1')
+root_id = 864691135867734294
+sk = pcg_skel.coord_space_skeleton(root_id, client)
 ```
 
-#### Notes
+This generates a skeleton, in this case for a pyramidal cell in the MICrONs65 volume, in just a few seconds — less time than is needed to download the mesh itself. The skeleton is shown in black, and the mesh in red.
 
-* `sk_ch` is assumed to have positions in chunk index space.
+![pyramidal cell](example_skeleton.png)
 
-* `l2dict_reversed` is the second dict that comes back in the tuple you get by setting `return_l2dict` to `True` in `chunk_index_skeleton`.
+## What you need
 
-* `refine_inds` can be either `"all"` or a specific array of vertex indices. This parameter sets which vertices to refine. A handful of vertices can be processed very quickly, while a more accurate skeleton is generated by refining all vertices.
+PCG-skel requires an active [PyChunkedGraph](https://github.com/seung-lab/PyChunkedGraph) server.
 
-* `scale_chunk_index`, if True, will still map unrefined vertex indices from their chunk index into the chunk position in eucliden space.
+For best performance, your dataset should have an L2 Cache, a service that caches representive points and features for every chunk.
+Using the CAVEclient, you can test for this by running `client.l2cache.attributes`.
+If you get a list of attribute names back, you're good!
+If you don't have an L2 cache and still want to use PCG Skel, see the section below `How to use without an L2 Cache`.
 
-* `nan_rounds` gives how many times to try to smoothly interpolate any vertices that did not get a position due to a missing L2 mesh fragment.
+To also use annotations, you also need a database backend running the [MaterializationEngine](https://github.com/seung-lab/MaterializationEngine).
 
-* `return_missing_ids` will also return a list of the ids of any missing L2 mesh fragment, for example if you want to re-run meshing on them.
+## Key terms
 
----
+Ids in the PCG combine information about chunk level, spatial location, and unique object id.
+This package uses the highest-resolution chunking, level 2, to derive neuronal topology and approximate spatial extent.
+For clarity, I'll define a few terms:
 
-### pcg_skeleton
+* *Level 2 chunk*: A box defining a unit of data storage and representation. The entire dataset is tiled by nonoverlapping chunks. Each chunk has properties like a detailed graph of which supervoxels touch what other supervoxels, meshes associated with each segmented object inside the chunk, etc. By chunking the data and agglomerating larger objects out of these chunks, edits only have to touch those few chunks that actually change during proofreading, reducing the amount of memory and effort needed to process them.
 
-Directly build a skeleton in Euclidean space, plus optionally handle soma points.
+Chunks can exist at many scales, but "level 2" refers to the lowest level of chunking (level 1 refers to the supervoxels themselves).
 
-```python
-def pcg_skeleton(root_id,
-                 client=None,
-                 datastack_name=None,
-                 cv=None,
-                 refine='all',
-                 root_point=None,
-                 root_point_resolution=[4, 4, 40],
-                 root_point_search_radius=300,
-                 collapse_soma=False,
-                 collapse_radius=10_000.0,
-                 invalidation_d=3,
-                 return_mesh=False,
-                 return_l2dict=False,
-                 return_l2dict_mesh=False,
-                 return_missing_ids=False,
-                 nan_rounds=20,
-                 n_parallel=1):
-```
+* *Level 2 id (L2 id)*: A segmentation id that describes the state of the segmentation inside a given L2 chunk.
+Note that if two distinct parts of the same neuron enter the same chunk, each has its own level 2 id.
 
-#### Notes
+* *Level 2 graph*: Each level 2 id can be thought of as connected to level 2 ids in other chunks when an object's supervoxels run across chunk boundaries or where edges have introduced by merges during proofreading. The graph of which level 2 ids are connected to which others is called the "level 2 graph." Keeping track of the level 2 graph is one of the jobs of the PCG.
 
-* `refine` can take five values to determine which vertices to refine.
-    1. `"all"`: Refine all vertices
-    2. `"ep"`: Refine only end points.
-    3. `"bp"`: Refine only branch points.
-    4. `"bpep"` or `"epbp"`: Refine both branch and end points.
-    5. `None`: Don't refine any vertex, but still map chunk positions coarsely.
+* *Level 2 skeleton*: A reduced version of the level 2 graph that is tree-like.
 
-    Options which download few mesh fragments are much faster than `"all"`.
+* *Representitative point*: For each level 2 id, the L2 Cache determines a representative point that is guaranteed to be within the segmentation and is located at a "most central" point in the segmentation of the L2 id.
 
-* `collapse_soma`, if set to True, collapses all mesh vertices within `collapse_radius` into the root point.
-Note that the root point is not a new point, but rather the closest level 2 object to the root point location.
+## How to use
 
----
+There are three main functions to generate a neuronal representation from the pychunkedgraph and L2 Cache that build on one another. One gets the L2 graph, one processes it into an L2 skeleton, and a third collects the graph and skeleton together into a "Meshwork" object that can also handle annotations.
 
-### pcg_meshwork
+### Skeletons
 
-Build a meshwork file with skeleton out from the level 2 graph.
-Optionally, attach pre- and/or post-synaptic synapses.
+This function will return a meshparty Skeleton class. Skeleton features can be found in the [Meshparty documentation](https://meshparty.readthedocs.io/en/latest/).
 
 ```python
-def pcg_meshwork(root_id,
-                 datastack_name=None,
-                 client=None,
-                 cv=None,
-                 refine='all',
-                 root_point=None,
-                 root_point_resolution=[4, 4, 40],
-                 root_point_search_radius=300,
-                 collapse_soma=False,
-                 collapse_radius=DEFAULT_COLLAPSE_RADIUS,
-                 synapses=None,
-                 synapse_table=None,
-                 remove_self_synapse=True,
-                 invalidation_d=3,
-                 n_parallel=4,
-                 ):
+def coord_space_skeleton(
+    root_id,
+    client,
+    cv=None,
+    invalidation_d=10_000,
+    return_mesh=False,
+    return_l2dict=False,
+    return_l2dict_mesh=False,
+    root_point=None,
+    root_point_resolution=None,
+    collapse_soma=False,
+    collapse_radius=7500,
+):
 ```
 
-#### Notes
+The basic use requires only a root id and a caveclient, but there are a number of important options.
 
-* The resulting meshwork file comes back with a "mesh" made out of the level 2 graph with vertices mapped to their chunk positions, a skeleton with `refine` and `collapse_soma` options as above, and one or more annotations.
+* *cv*: Passing an initialized cloudvolume object (`cv=`) can save a second or two per skeleton. This isn't a big deal for a couple of skeletons, but may save some real time if you are creating a large number of skeletons.
 
-* All resulting meshworks have the annotation `lvl2_ids`, which is based on a dataframe with column `lvl2_id` that has level 2 ids and `mesh_ind` that has the associated mesh index.
-One can use the MeshIndex/SkeletonIndex properties like `nrn.anno.mesh_index.to_skel_index` to see the associated skeleton indices.
+* *invalidation_d*: The invalidation distance for skeletonization, in nanometers. This parameter sets the distance at which vertices of the graph are collapsed into a branch. Too big and branches might be missed, but too small and false branches might be added to thick processes. This is an important parameter to customize for your data, since different morphologies will be best represented by different values. The default value works well for cortical neurons, for example, but is probably too coarse for fly neurons.
 
-* If the `synapses` property is set to `"pre"`, `"post"`, or `"all"`, there is also an attempt to look up the root id's presynaptic synapses, postsynaptic synapses, or both (respectively).
-Presynaptic synapses are in an annotation `"pre_syn"` and postsynaptic synapses are in an annotation called `"post_syn"`.
+* *return_mesh*, *return_l2dict*, *return_l2dict_mesh*: These three values are all set to False by default, which is fine if you just want a skeleton. However, if you want to map vertices to level 2 ids or skeleton vertices back to the mesh graph, these options can give you the mesh and dictionaries mapping vertices to the l2 ids for the skeletons and the mesh graph.
 
-* If returning synapses, you must set the synapse table.
-By default, synapses whose pre- and post-synaptic ids are both the same root id are excluded, but this can be turned off by setting `remove_self_synapse` to `False`.
+* *root_point*, *root_point_resolution*: Setting a root point defines the root of the skeleton, which establishes an orientation for the skeleton. Root point is an x,y,z position, and the resolution is the value in nm of the resolution of coordinates (also in x,y,z, resolution). If the point is from neuroglancer or an annotation table, take careful note of the resolution. 
 
-## Example
+* *collapse_soma*, *collapse_radius*: These two options let you collapse vertices around a soma into the root point. Setting collapse_soma to True will collapse all vertices within the collapse radius (in nanometers) into the root point. Additionally, the root point is added as a new skeleton vertex. Again, the default value works for most cortical neurons, but cells with larger or smaller cell bodies might need different values.
 
-A minimal example to get the skeleton of an arbitrary neuron with root id `864691135761488438` and soma at the voxel-space location `253870, 236989, 20517` in the Minnie dataset:
 
-```python
-from caveclient import CAVEclient
-import pcg_skel
-
-client = CAVEclient('minnie65_phase3_v1')
-
-oid = 864691135761488438 # Root id
-root_point = [253870, 236989, 20517] # root point in vertex coordinates
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              client=client,
-                              refine='all',
-                              root_point=root_point,
-                              root_point_resolution=[4,4,40],
-                              collapse_soma=True,
-                              n_parallel=8)
-```
+### Mesh graph
 
-To generate a skeleton with 1310 vertices took about 80 seconds on a 2019 MacBook Pro, all refined through the mesh fragments.
-Most of the time is spent in refinement.
-If you just select the `refine="epbp"` argument, it only refines the 79 branch and end points and accordingly takes a mere 12.5 seconds.
-It is worth exploring sparse refinement options and interpolation if processing time is extremely important.
-
-## Caching
-
-A common use case is to have a set of neurons that you are analyzing while proofreading is still ongoing.
-However, because proofreading events leave most of the neuron unchanged we shouldn't need to do more than update new locations.
-Conveniently, the level 2 ids let us follow this intuition.
-While a neuron's root id changes for each proofreading event, the level 2 id only changes if an edit occurs exactly within that region.
-Therefore, once we've looked up a level 2 id once, we can cache it and save time for future iterations on the same neuron.
-
-The current implementation of caching uses [SQLiteDict](https://github.com/piskvorky/sqlitedict), a simple means of using a sqlite file as a persistent key-value store.
-The cache is used with the functions `refine_vertices`, `pcg_skeleton`, and `pcg_meshwork` if you specify the filename of the sqlite database.
-For example,
+This function will return a meshparty Mesh object, with a vertex at the representative point for every l2 id and edges where they connect to one another.
+Such a mesh is what the skeleton returned above is generated from.
 
 ```python
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              ...,
-                              cache='l2_cache.sqlite',
-                              save_to_cache=False,
-                              )
+def coord_space_mesh(
+    root_id,
+    client,
+    cv=None,
+    return_l2dict=False,
+):
 ```
 
-Note that if the database is not yet present, it will be created automatically.
-
-In order to avoid unintentional changes, new locations are not saved to the database by default.
-If you want to save new ids to the database as you are skeletonizing files, set the additional parameter `save_to_cache=True`.
-For adding data to the database post-hoc, please use the function `chunk_cache.save_ids_to_cache()`.
-
-## Segmentation-based localization
+There are fewer options, since the mesh graph is a more direct representation of the data.
 
-Localizing level 2 ids with mesh fragments is much faster than downloading the segmentation for a whole chunk just to get a few supervoxels, but sometimes mesh fragments don't exist.
-This can occur for both good reasons (the L2 object is too small to get a mesh) and due to bugs in the meshing backend.
-However, if you really want to get such locations correct, falling back to the segmentation is available.
+### Meshwork file
 
-You can use this by setting the `segmentation_fallback` option on any of the functions that localize vertices.
-For example,
+Meshwork files combine the mesh graph, the skeleton, and annotations linked together. They are more complex objects, but can be useful for a number of tasks and analyses.
 
 ```python
-sk_l2 = pcg_skel.pcg_skeleton(oid,
-                              ...,
-                              segmentation_fallback=True,
-                              fallback_mip=2,
-                              )
+def coord_space_meshwork(
+    root_id,
+    datastack_name=None,
+    client=None,
+    cv=None,
+    root_point=None,
+    root_point_resolution=None,
+    collapse_soma=False,
+    collapse_radius=7500,
+    synapses=None,
+    synapse_table=None,
+    remove_self_synapse=True,
+    live_query=False,
+    timestamp=None,
+    invalidation_d=7500,
+):
 ```
 
-Setting `segmentation_fallback=True` activates the capability, and setting `fallback_mip` will choose the MIP-level to use (2 by default).
-If the chosen MIP does not have voxels for the L2 id in it, it will try 0 next.
-Segmentation-based points will be cached if both features are used.
+Many of the parameters are the same as in skeletonization. In addition, there are parameters controlling the addition of synapses.
+
+* *synapses*, *synapse_table*: If set to `"pre"`, `"post"`, or `"both"`, the after skeletonization the system will add pre, post, or both pre and postsynaptic annotations using the specified synapse table to the meshwork under `nrn.anno.pre_syn` and `nrn.anno.post_syn` respectively. Note that by default, `remove_self_synapse` will omit all synapses whose pre and post ids are the same neuron. This is a common form of errors, particularly around the nucleus, although it can also remove biologically real autapses.
+
+* *live_query*, *timestamp*: If live_query is True, sets the timestamp at which annotations are from. If not set, uses the most materialization defined in the caveclient.
 
-Note that this approach is much slower and more memory intensive than using the mesh fragments.
-I have found it to take 4-8 seconds per vertex with the current implementation, although parallelation helps.
 
-## To-dos
+## How to use without an L2 Cache
 
-* Improve/document/test tooling for additional annotations.
-* Alternative key-value stores for caching
+See the `nocache.md` file for instructions on how to use without a L2 cache for the chunkedgraph.
 
 ## Credit
 
 This work is by Casey Schneider-Mizell (caseys@alleninstitute.org) with suggestions from Sven Dorkenwald and Forrest Collman.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pcg_skel-0.3.1/pcg_skel/chunk_cache.py` & `pcg_skel-0.3.3/pcg_skel/chunk_cache.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.1/pcg_skel/chunk_tools.py` & `pcg_skel-0.3.3/pcg_skel/chunk_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,76 @@
 import numpy as np
 from scipy import spatial
 import cloudvolume
 from . import utils, chunk_cache, skel_utils
 import multiwrapper.multiprocessing_utils as mu
+import fastremap
 
 UnshardedMeshSource = (
     cloudvolume.datasource.graphene.mesh.unsharded.GrapheneUnshardedMeshSource
 )
 ShardedMeshSource = (
     cloudvolume.datasource.graphene.mesh.sharded.GrapheneShardedMeshSource
 )
 
 L2_SERVICE_NAME = "service"
 
 
 class CompleteDataException(Exception):
     pass
 
+def build_graph_topology(lvl2_edge_graph):
+    """Extract the graph from the result of the lvl2_graph endpoint"""
+    lvl2_edge_graph = np.unique(np.sort(lvl2_edge_graph, axis=1), axis=0)
+    lvl2_ids = np.unique(lvl2_edge_graph)
+    l2dict = {l2id: ii for ii, l2id in enumerate(lvl2_ids)}
+    eg_arr_rm = fastremap.remap(lvl2_edge_graph, l2dict)
+    l2dict_reversed = {ii: l2id for l2id, ii in l2dict.items()}
+    return eg_arr_rm, l2dict, l2dict_reversed, lvl2_ids
+
+
+def build_spatial_graph(
+    lvl2_edge_graph, cv, client=None, method="chunk", require_complete=False
+):
+    """Extract spatial graph and level 2 id lookups from chunkedgraph "lvl2_graph" endpoint.
+
+    Parameters
+    ----------
+    lvl2_edge_graph : array
+        Nx2 edge list of level 2 ids
+    cv : cloudvolume.CloudVolume
+        Associated cloudvolume object
+
+    Returns
+    -------
+    eg_arr_rm : np.array
+        Nx2 edge list of indices remapped to integers starting at 0 through M, the number of unique level 2 ids.
+    l2dict : dict
+        Dict with level 2 ids as keys and vertex index as values
+    l2dict_reversed : dict
+        Dict with vertex index as keys and level 2 id as values
+    x_ch : np.array
+        Mx3 array of vertex locations in chunk index space.
+    """
+    eg_arr_rm, l2dict, l2dict_reversed, lvl2_ids = build_graph_topology(lvl2_edge_graph)
+    if method == "chunk":
+        x_ch = [np.array(cv.mesh.meta.meta.decode_chunk_position(l)) for l in lvl2_ids]
+    elif method == "service":
+        x_ch = dense_spatial_lookup(
+            lvl2_ids,
+            eg_arr_rm,
+            client,
+            require_complete=require_complete,
+        )
+    return eg_arr_rm, l2dict, l2dict_reversed, x_ch
+
+def adjust_meshwork(nrn, cv):
+    """Transform vertices in chunk index space to euclidean"""
+    nrn._mesh.vertices = utils.chunk_to_nm(nrn._mesh.vertices, cv)
+
 
 def dense_spatial_lookup(l2ids, eg, client, require_complete=False):
     l2means = np.full((len(l2ids), 3), np.nan)
     locs, inds_found = chunk_cache.get_locs_remote(l2ids, client)
     if require_complete:
         if not np.all(inds_found):
             raise CompleteDataException("Some chunk indices are not yet computed")
```

### Comparing `pcg_skel-0.3.1/pcg_skel/pcg_anno.py` & `pcg_skel-0.3.3/pcg_skel/pcg_anno.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,26 +130,32 @@
     client,
     l2dict,
     side,
     synapse_table,
     remove_self,
     live_query,
     timestamp,
+    metadata,
+    remove_crud=True,
 ):
     if live_query:
         syn_df = client.materialize.live_query(
             synapse_table,
             filter_equal_dict={f"{side}_pt_root_id": root_id},
             timestamp=timestamp,
+            metadata=metadata
         )
     else:
         syn_df = client.materialize.query_table(
             synapse_table,
             filter_equal_dict={f"{side}_pt_root_id": root_id},
+            metadata=metadata,
         )
+    if remove_crud:
+        syn_df.drop(columns=['created', 'superceded_id', 'valid'], inplace=True)
 
     if remove_self:
         syn_df = syn_df.query("pre_pt_root_id != post_pt_root_id").reset_index(
             drop=True
         )
     syn_df = annotation_to_level2_id(
         syn_df,
@@ -174,14 +180,15 @@
     client,
     synapse_table,
     remove_self=True,
     pre=True,
     post=True,
     live_query=False,
     timestamp=None,
+    metadata=False,
 ):
     live_query = timestamp is not None
 
     if timestamp is None:
         timestamp = datetime.datetime.utcnow()
     if pre is True:
         pre_syn_df = _mapped_synapses(
@@ -189,26 +196,28 @@
             client,
             l2dict,
             "pre",
             synapse_table,
             remove_self=remove_self,
             live_query=live_query,
             timestamp=timestamp,
+            metadata=metadata,
         )
     else:
         pre_syn_df = None
 
     if post is True:
         post_syn_df = _mapped_synapses(
             root_id,
             client,
             l2dict,
             "post",
             synapse_table,
             remove_self=remove_self,
             live_query=live_query,
             timestamp=timestamp,
+            metadata=metadata,
         )
     else:
         post_syn_df = None
 
     return pre_syn_df, post_syn_df
```

### Comparing `pcg_skel-0.3.1/pcg_skel/pcg_skel.py` & `pcg_skel-0.3.3/pcg_skel/pcg_skel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,85 +1,61 @@
-import fastremap
 import numpy as np
-import pandas as pd
 from caveclient import CAVEclient
-
 from meshparty import skeleton, skeletonize, trimesh_io, meshwork
 
 from . import chunk_tools, features
 from . import skel_utils as sk_utils
 from . import utils
-from . import pcg_anno
 
 DEFAULT_VOXEL_RESOLUTION = [4, 4, 40]
 DEFAULT_COLLAPSE_RADIUS = 7500.0
 DEFAULT_INVALIDATION_D = 7500
 
 skeleton_type = "pcg_skel"
 
-
-def build_graph_topology(lvl2_edge_graph):
-    """Extract the graph from the result of the lvl2_graph endpoint"""
-    lvl2_edge_graph = np.unique(np.sort(lvl2_edge_graph, axis=1), axis=0)
-    lvl2_ids = np.unique(lvl2_edge_graph)
-    l2dict = {l2id: ii for ii, l2id in enumerate(lvl2_ids)}
-    eg_arr_rm = fastremap.remap(lvl2_edge_graph, l2dict)
-    l2dict_reversed = {ii: l2id for l2id, ii in l2dict.items()}
-    return eg_arr_rm, l2dict, l2dict_reversed, lvl2_ids
-
-
-def build_spatial_graph(
-    lvl2_edge_graph, cv, client=None, method="chunk", require_complete=False
-):
-    """Extract spatial graph and level 2 id lookups from chunkedgraph "lvl2_graph" endpoint.
-
-    Parameters
-    ----------
-    lvl2_edge_graph : array
-        Nx2 edge list of level 2 ids
-    cv : cloudvolume.CloudVolume
-        Associated cloudvolume object
-
-    Returns
-    -------
-    eg_arr_rm : np.array
-        Nx2 edge list of indices remapped to integers starting at 0 through M, the number of unique level 2 ids.
-    l2dict : dict
-        Dict with level 2 ids as keys and vertex index as values
-    l2dict_reversed : dict
-        Dict with vertex index as keys and level 2 id as values
-    x_ch : np.array
-        Mx3 array of vertex locations in chunk index space.
-    """
-    eg_arr_rm, l2dict, l2dict_reversed, lvl2_ids = build_graph_topology(lvl2_edge_graph)
-    if method == "chunk":
-        x_ch = [np.array(cv.mesh.meta.meta.decode_chunk_position(l)) for l in lvl2_ids]
-    elif method == "service":
-        x_ch = chunk_tools.dense_spatial_lookup(
-            lvl2_ids,
-            eg_arr_rm,
-            client,
-            require_complete=require_complete,
-        )
-    return eg_arr_rm, l2dict, l2dict_reversed, x_ch
-
-
 def coord_space_mesh(
     root_id,
     client,
     cv=None,
     return_l2dict=False,
     nan_rounds=10,
     require_complete=False,
 ):
+    """Compute the level 2 spatial graph (or mesh) of a given root id using the l2cache.
+
+    Parameters
+    ----------
+    root_id : int
+        Root id of a segment
+    client : CAVEclient.caveclient
+        Initialized CAVEclient for the dataset.
+    cv : cloudvolume.CloudVolume, optional
+        Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
+        a pre-initizialized cloudvolume can save some time during batch processing. By default None. 
+    return_l2dict : bool, optional
+        If True, returns the mappings between l2 ids and vertices, by default False
+    nan_rounds : int, optional
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
+
+    Returns
+    -------
+    mesh : meshparty.trimesh_io.Mesh
+        Object with a vertex for every level 2 id and edges between all connected level 2 chunks.
+    l2dict : dict (optional)
+        Dictionary with keys as level 2 ids and values as mesh vertex index. Optional, only returned if `return_l2dict` is True.
+    l2dict_reverse : dict (optional)
+        Dictionary with keys as mesh vertex indices and values as level 2 id. Optional, only returned if `return_l2dict` is True.
+    """
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=False)
 
     lvl2_eg = client.chunkedgraph.level2_chunk_graph(root_id)
-    eg, l2dict_mesh, l2dict_r_mesh, x_ch = build_spatial_graph(
+    eg, l2dict_mesh, l2dict_r_mesh, x_ch = chunk_tools.build_spatial_graph(
         lvl2_eg,
         cv,
         client=client,
         method="service",
         require_complete=require_complete,
     )
     mesh_loc = trimesh_io.Mesh(
@@ -108,14 +84,59 @@
     root_point=None,
     root_point_resolution=None,
     collapse_soma=False,
     collapse_radius=7500,
     nan_rounds=10,
     require_complete=False,
 ):
+    """Produce a skeleton from the level 2 graph.
+    Parameters
+    ----------
+    root_id : int
+        Root id of a segment
+    client : CAVEclient.caveclient
+        Initialized CAVEclient for the dataset.
+    datastack_name : string, optional
+        If client is None, initializes a CAVEclient at this datastack, by default None.
+    cv : cloudvolume.CloudVolume, optional
+        Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
+        a pre-initizialized cloudvolume can save some time during batch processing. By default None. 
+    invalidation_d : int, optional
+        Distance (in nanometers) for TEASAR skeleton invalidation, by default 10_000.
+    return_mesh : bool, optional
+        If True, returns the mesh graph as well as the skeleton, by default False
+    return_l2dict : bool, optional
+        If True, returns the mappings between l2 ids and skeleton vertices, by default False
+    return_l2dict_mesh : bool, optional
+        If True, returns mappings between l2 ids and mesh graph vertices, by default False
+    root_point : list-like, optional
+        3-element list or array with the x,y,z location of the root point. Optional, by default None.
+        If None, the most distant tip is set to root.
+    root_point_resolution : list-like, optional
+        3-element list or array with the x,y,z resolution of the root point, in nanometers per voxel dimension, by default None.
+    collapse_soma : bool, optional
+        If True, collapse nearby vertices into the root point, by default False.
+    collapse_radius : int, optional
+        Distance (in nanometers) for soma collapse, by default 7500.
+    nan_rounds : int, optional
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
+
+    Returns
+    -------
+    sk : meshparty.skeleton.Skeleton
+        Skeleton for the root id
+    mesh : meshparty.trimesh_io.Mesh (optional)
+        Mesh graph that the skeleton is based on, only returned if return_mesh is True.
+    (l2dict_skel, l2dict_reverse): tuple of dicts (optional)
+        Dictionaries mapping l2 ids to skeleton vertices and skeleton vertices to l2 ids, respectively. Only returned if return_l2dict is True.
+    (l2dict_mesh, l2dict_mesh): tuple of dicts (optional)
+        Dictionaries mapping l2 ids to mesh graph vertices and mesh_graph vertices to l2 ids, respectively. Only returned if return_l2dict is True.
+    """
     if client is None:
         client = CAVEclient(datastack_name)
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=False)
 
     if root_point_resolution is None:
         root_point_resolution = cv.mip_resolution(0)
@@ -158,14 +179,130 @@
         out_list.append((l2dict_mesh, l2dict_r_mesh))
     if len(out_list) == 1:
         return out_list[0]
     else:
         return tuple(out_list)
 
 
+def coord_space_meshwork(
+    root_id,
+    datastack_name=None,
+    client=None,
+    cv=None,
+    root_point=None,
+    root_point_resolution=None,
+    collapse_soma=False,
+    collapse_radius=DEFAULT_COLLAPSE_RADIUS,
+    synapses=None,
+    synapse_table=None,
+    remove_self_synapse=True,
+    live_query=False,
+    timestamp=None,
+    invalidation_d=DEFAULT_INVALIDATION_D,
+    require_complete=False,
+    metadata=False,
+):
+    """Generate a meshwork file based on the level 2 graph.
+
+    Parameters
+    ----------
+    root_id : int
+        Root id of an object in the pychunkedgraph.
+    datastack_name : str or None, optional
+        Datastack name to use to initialize a client, if none is provided. By default None.
+    client : caveclient.CAVEclientFull or None, optional
+        Initialized CAVE client. If None is given, will use the datastack_name to create one. By default None
+    cv : cloudvolume.CloudVolume or None, optional
+        Initialized cloudvolume. If none is given, the client info will be used to create one. By default None
+    root_point : array-like or None, optional
+        3 element xyz location for the location to set the root in units set by root_point_resolution,
+        by default None. If None, a distal tip is selected.
+    root_point_resolution : array-like, optional
+        Resolution in euclidean space of the root_point, by default [4, 4, 40]
+    collapse_soma : bool, optional,
+        If True, collapses vertices within a given radius of the root point into the root vertex, typically to better
+        represent primary neurite branches. Requires a specified root_point. Default if False.
+    collapse_radius : float, optional
+        Max distance in euclidean space for soma collapse. Default is 10,000 nm (10 microns).
+    synapses : 'pre', 'post', 'all', or None, optional
+        If not None, queries the synapse_table for presynaptic synapses (if 'pre'),  postsynaptic sites (if 'post'), or both (if 'all'). By default None
+    synapse_table : str, optional
+        Name of the synapse table to query if synapses are requested, by default None
+    remove_self_synapse : bool, optional
+        If True, filters out synapses whose pre- and postsynaptic root ids are the same neuron, by default True
+    live_query : bool, optional
+        If True, expect a timestamp for querying at a give point in time. Otherwise, use the materializatio set by the client. Optional, by default False.
+    timestamp = datetime.datetime, optional
+        If set, acts as the time at which all root ids and annotations are found at. 
+    invalidation_d : int, optional
+        Invalidation radius in hops for the mesh skeletonization along the chunk adjacency graph, by default 3
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
+
+    Returns
+    -------
+    meshparty.meshwork.Meshwork
+        Meshwork object with skeleton based on the level 2 graph. See documentation for details.
+    """
+    if client is None:
+        client = CAVEclient(datastack_name)
+    if cv is None:
+        cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
+    if root_point_resolution is None:
+        root_point_resolution = cv.mip_resolution(0)
+
+    sk, mesh, (l2dict_mesh, l2dict_mesh_r) = coord_space_skeleton(
+        root_id,
+        client=client,
+        cv=cv,
+        root_point=root_point,
+        root_point_resolution=root_point_resolution,
+        collapse_soma=collapse_soma,
+        collapse_radius=collapse_radius,
+        invalidation_d=invalidation_d,
+        return_mesh=True,
+        return_l2dict_mesh=True,
+        require_complete=require_complete,
+    )
+
+    nrn = meshwork.Meshwork(mesh, seg_id=root_id, skeleton=sk)
+
+    pre, post = False, False
+    if synapses is not None and synapse_table is not None:
+        if synapses == "pre":
+            pre, post = True, False
+        elif synapses == "post":
+            pre, post = False, True
+        elif synapses == "all":
+            pre, post = True, True
+        else:
+            raise ValueError('Synapses must be one of "pre", "post", or "all".')
+
+        if not timestamp:
+            timestamp = client.materialize.get_timestamp()
+
+        features.add_synapses(
+            nrn,
+            synapse_table,
+            l2dict_mesh,
+            client,
+            root_id=root_id,
+            pre=pre,
+            post=post,
+            remove_self_synapse=remove_self_synapse,
+            timestamp=timestamp,
+            live_query=live_query,
+            metadata=metadata,
+        )
+
+    features.add_lvl2_ids(nrn, l2dict_mesh)
+    return nrn
+
+
+
 def chunk_index_mesh(
     root_id,
     client=None,
     datastack_name=None,
     cv=None,
     return_l2dict=False,
 ):
@@ -189,21 +326,23 @@
     mesh : trimesh_io.Mesh
         Chunk graph represented as a mesh, with vertices at chunk index locations and edges in the link_edges attribute.
     l2dict_mesh : dict
         l2 id to mesh vertex index dictionary. Only returned if return_l2dict is True.
     l2dict_r_mesh : dict
         Mesh vertex index to l2 id dictionary. Only returned if return_l2dict is True.
     """
+    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
+
     if client is None:
         client = CAVEclient(datastack_name)
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=False)
 
     lvl2_eg = client.chunkedgraph.level2_chunk_graph(root_id)
-    eg, l2dict_mesh, l2dict_r_mesh, x_ch = build_spatial_graph(lvl2_eg, cv)
+    eg, l2dict_mesh, l2dict_r_mesh, x_ch = chunk_tools.build_spatial_graph(lvl2_eg, cv)
     mesh_chunk = trimesh_io.Mesh(
         vertices=x_ch,
         faces=[[0, 0, 0]],  # Some functions fail if no faces are set.
         link_edges=eg,
     )
     if return_l2dict:
         return mesh_chunk, l2dict_mesh, l2dict_r_mesh
@@ -253,14 +392,16 @@
     sk : meshparty.skeleton.Skeleton
         Skeleton object
     mesh : meshparty.trimesh_io.Mesh
         Mesh object, only if return_mesh is True
     level2_dict : dict
         Level 2 id to vertex map, only if return_l2dict is True.
     """
+    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
+
     if client is None:
         client = CAVEclient(datastack_name)
     if n_parallel is None:
         n_parallel = 1
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
 
@@ -364,14 +505,15 @@
         If set to 'service', uses the l2cache service if available available. Otherwise, a filename for a sqlite database storing locations associated with level 2 ids. Default is None.
     save_to_cache : bool, optional
         If using a sqlite database, setting this to True will add values to the cache as downloads occur.
     client : CAVEclient, optional
         If using the l2cache service, provides a client that can access it.
     l2cache : bool, optional,
         Set to True if using a l2cache to localize vertices. Same as setting cache to 'service'. Default is False.
+
     Returns
     -------
     meshparty.skeleton.Skeleton
         Skeleton with remapped vertex locations
     """
     if nan_rounds is None:
         convert_missing = True
@@ -521,14 +663,16 @@
     (l2dict, l2dict_r) : (dict, dict), optional
         Mappings between level 2 ids and skeleton indices. Only if return_l2dict is True.
     (l2dict_mesh, l2dict_mesh_r) : (dict, dict), optional
         Mappings between level 2 ids and mesh indices. Only if return_l2dict_mesh is True.
     missing_ids : np.array, optional
         List of level 2 ids with missing mesh fragments. Only if return_missing_ids is True.
     """
+    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
+
     if client is None:
         client = CAVEclient(datastack_name)
     if n_parallel is None:
         n_parallel = 1
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
 
@@ -634,83 +778,14 @@
         output.append(missing_ids)
     if len(output) == 1:
         return output[0]
     else:
         return tuple(output)
 
 
-def coord_space_meshwork(
-    root_id,
-    datastack_name=None,
-    client=None,
-    cv=None,
-    root_point=None,
-    root_point_resolution=None,
-    collapse_soma=False,
-    collapse_radius=DEFAULT_COLLAPSE_RADIUS,
-    synapses=None,
-    synapse_table=None,
-    remove_self_synapse=True,
-    live_query=False,
-    timestamp=None,
-    invalidation_d=DEFAULT_INVALIDATION_D,
-    require_complete=False,
-):
-    if client is None:
-        client = CAVEclient(datastack_name)
-    if cv is None:
-        cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
-    if root_point_resolution is None:
-        root_point_resolution = cv.mip_resolution(0)
-
-    sk, mesh, (l2dict_mesh, l2dict_mesh_r) = coord_space_skeleton(
-        root_id,
-        client=client,
-        cv=cv,
-        root_point=root_point,
-        root_point_resolution=root_point_resolution,
-        collapse_soma=collapse_soma,
-        collapse_radius=collapse_radius,
-        invalidation_d=invalidation_d,
-        return_mesh=True,
-        return_l2dict_mesh=True,
-        require_complete=require_complete,
-    )
-
-    nrn = meshwork.Meshwork(mesh, seg_id=root_id, skeleton=sk)
-
-    pre, post = False, False
-    if synapses is not None and synapse_table is not None:
-        if synapses == "pre":
-            pre, post = True, False
-        elif synapses == "post":
-            pre, post = False, True
-        elif synapses == "all":
-            pre, post = True, True
-        else:
-            raise ValueError('Synapses must be one of "pre", "post", or "all".')
-
-        if not timestamp:
-            timestamp = client.materialize.get_timestamp()
-
-        features.add_synapses(
-            nrn,
-            synapse_table,
-            l2dict_mesh,
-            client,
-            root_id=root_id,
-            pre=pre,
-            post=post,
-            remove_self_synapse=remove_self_synapse,
-            timestamp=timestamp,
-            live_query=live_query,
-        )
-
-    features.add_lvl2_ids(nrn, l2dict_mesh)
-    return nrn
 
 
 def pcg_meshwork(
     root_id,
     datastack_name=None,
     client=None,
     cv=None,
@@ -782,14 +857,15 @@
         Set to True to use the l2cache. Equivalent to cache='service'.
 
     Returns
     -------
     meshparty.meshwork.Meshwork
         Meshwork object with skeleton based on the level 2 graph. See documentation for details.
     """
+    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
 
     if client is None:
         client = CAVEclient(datastack_name)
     if n_parallel is None:
         n_parallel = 1
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
@@ -844,22 +920,19 @@
             timestamp=timestamp,
             live_query=live_query,
         )
 
     features.add_lvl2_ids(nrn, l2dict_mesh)
 
     if refine != "chunk":
-        _adjust_meshwork(nrn, cv)
+        chunk_tools.adjust_meshwork(nrn, cv)
 
     return nrn
 
 
-def _adjust_meshwork(nrn, cv):
-    """Transform vertices in chunk index space to euclidean"""
-    nrn._mesh.vertices = utils.chunk_to_nm(nrn._mesh.vertices, cv)
 
 
 def collapse_pcg_skeleton(soma_pt, sk, soma_r):
     """Use soma point vertex and collapse soma as sphere
     Parameters
     ----------
     soma_pt : array
```

### Comparing `pcg_skel-0.3.1/pcg_skel/skel_utils.py` & `pcg_skel-0.3.3/pcg_skel/skel_utils.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.1/pcg_skel/utils.py` & `pcg_skel-0.3.3/pcg_skel/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from trimesh import creation
 from functools import reduce
 
-
 def chunk_dims(cv):
     """Gets the size of a chunk in euclidean space
 
     Parameters
     ----------
     cv : cloudvolume.CloudVolume
         Chunkedgraph-targeted cloudvolume object
```

### Comparing `pcg_skel-0.3.1/setup.py` & `pcg_skel-0.3.3/setup.py`

 * *Files identical despite different names*

