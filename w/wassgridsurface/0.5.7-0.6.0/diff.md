# Comparing `tmp/wassgridsurface-0.5.7.tar.gz` & `tmp/wassgridsurface-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-t66qy0lz/wassgridsurface-0.5.7.tar", last modified: Sun Mar 26 13:01:17 2023, max compression
+gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-5v42hc9l/wassgridsurface-0.6.0.tar", last modified: Fri Apr 21 17:47:16 2023, max compression
```

## Comparing `wassgridsurface-0.5.7.tar` & `wassgridsurface-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-26 13:01:17.209170 wassgridsurface-0.5.7/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.5.7/.gitignore
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-01-12 09:58:42.000000 wassgridsurface-0.5.7/BUILD.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-03-26 13:01:17.209170 wassgridsurface-0.5.7/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-01-12 09:58:42.000000 wassgridsurface-0.5.7/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.5.7/environment.yml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-01-12 09:58:42.000000 wassgridsurface-0.5.7/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-03-26 13:01:17.209170 wassgridsurface-0.5.7/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-26 13:01:17.209170 wassgridsurface-0.5.7/wassgridsurface/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4865 2023-01-12 09:58:42.000000 wassgridsurface-0.5.7/wassgridsurface/DCTInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.5.7/wassgridsurface/IDWInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.5.7/wassgridsurface/TFVariationalRefinement.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.5.7/wassgridsurface/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.5.7/wassgridsurface/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6049 2023-03-26 13:00:19.000000 wassgridsurface-0.5.7/wassgridsurface/netcdfoutput.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.5.7/wassgridsurface/wass_utils.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    24389 2023-03-26 13:00:45.000000 wassgridsurface-0.5.7/wassgridsurface/wassgridsurface.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-26 13:01:17.209170 wassgridsurface-0.5.7/wassgridsurface.egg-info/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-03-26 13:01:16.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2023-03-26 13:01:17.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-03-26 13:01:16.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2023-03-26 13:01:16.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2023-03-26 13:01:16.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2023-03-26 13:01:16.000000 wassgridsurface-0.5.7/wassgridsurface.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.6.0/.gitignore
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/BUILD.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.6.0/environment.yml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/wassgridsurface/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4947 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/DCTInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.6.0/wassgridsurface/IDWInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.6.0/wassgridsurface/TFVariationalRefinement.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.6.0/wassgridsurface/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.6.0/wassgridsurface/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6083 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/netcdfoutput.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.6.0/wassgridsurface/wass_utils.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    25343 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/wassgridsurface.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/wassgridsurface.egg-info/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2023-04-21 17:47:16.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/top_level.txt
```

### Comparing `wassgridsurface-0.5.7/PKG-INFO` & `wassgridsurface-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.5.7
+Version: 0.6.0
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
```

### Comparing `wassgridsurface-0.5.7/README.md` & `wassgridsurface-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/pyproject.toml` & `wassgridsurface-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/DCTInterpolator.py` & `wassgridsurface-0.6.0/wassgridsurface/DCTInterpolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if not options_dict is None:
             if setting_name in options_dict:
                 return options_dict[setting_name] if not (options_dict[setting_name] is None) else default_settings[setting_name]
 
         return default_settings[setting_name]
 
 
-    def __call__( self, I ):
+    def __call__( self, I, verbose=True ):
         orig_pts_mask = 1-np.isnan(I).astype(np.uint8)
         mask = orig_pts_mask.astype(np.float32)
         I[ np.isnan(I) ] = 0
         I = np.copy(I)
 
         Dc = self.Dc
         Iorig = torch.tensor(I, dtype=torch.float, device=self.device )
@@ -101,17 +101,19 @@
                 return loss
 
             optimizer.step( closure )
 
             if ii%50 == 0:
                 loss, data_loss, regularizer_loss = closure( output_all_loss_components=True )
                 fdelta = torch.max( torch.abs(x-xprev)).item()
-                tqdm.write("Iteration %05d - Loss: %6.5f =  data: %6.5f  reg: %6.5f   F max delta: %3.5f"%(ii, loss.item(), data_loss.item(), regularizer_loss.item(), fdelta ) )
+                if verbose:
+                    tqdm.write("Iteration %05d - Loss: %6.5f =  data: %6.5f  reg: %6.5f   F max delta: %3.5f"%(ii, loss.item(), data_loss.item(), regularizer_loss.item(), fdelta ) )
                 if fdelta < TOLERANCE_CHANGE:
-                    print("Reached min tolerance change, exiting")
+                    if verbose:
+                        print("Reached min tolerance change, exiting")
                     break
 
             xprev = torch.clone(x)
 
 
         full_signal = torch.nn.functional.pad( x, (0,self.height-self.Nfreqs,0,self.width-self.Nfreqs), "constant", 0 )
         Irec = Dc.T @ full_signal @ Dc
```

### Comparing `wassgridsurface-0.5.7/wassgridsurface/IDWInterpolator.py` & `wassgridsurface-0.6.0/wassgridsurface/IDWInterpolator.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/TFVariationalRefinement.py` & `wassgridsurface-0.6.0/wassgridsurface/TFVariationalRefinement.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/__init__.py` & `wassgridsurface-0.6.0/wassgridsurface/__init__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/__main__.py` & `wassgridsurface-0.6.0/wassgridsurface/__main__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/netcdfoutput.py` & `wassgridsurface-0.6.0/wassgridsurface/netcdfoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.kx.field = "Kx, scalar, series"
 
         self.ky = self.rootgrp.createVariable( "Ky", "f8", ("X","Y",) )
         self.ky.units = "wavenumbers"
         self.ky.long_name = "Vertical wavenumbers"
         self.ky.field = "Ky, scalar, series"
 
-        self.Z = self.rootgrp.createVariable( "Z", "f4", ("count", "X","Y",)) #, chunksizes=(1,M//8,N//8) )
+        self.Z = self.rootgrp.createVariable( "Z", "f4", ("count", "X","Y",), chunksizes=(8,M,N) )
         self.Z.units = "millimeter"
         self.Z.long_name = "Z data on time over the XY grid"
         self.Z.field = "Z, scalar, series"
 
         self.maskZ = self.rootgrp.createVariable( "maskZ", "f4", ("X","Y",) )
         self.maskZ.units = ""
         self.maskZ.long_name = "Z mask over the XY grid"
@@ -136,17 +136,19 @@
     #         idx = self.count.shape[0]
     #         self.Z[idx,:,:] = np.expand_dims( Zdata, axis=0 )
     #         self.count[idx] = idx
     #         self.time[idx] = time
     #         if idx%10 == 0:
     #             self.rootgrp.sync() # Flush data to disk
 
-    def push_Z( self, Zdata, time, workdir, image=None, imagemask=None ):
+    def push_Z( self, Zdata, time, workdir, image=None, imagemask=None, idx=None ):
         if self.rootgrp != None:
-            idx = self.count.shape[0]
+            if idx is None:
+                idx = self.count.shape[0]
+
             self.Z[idx,:,:] = np.expand_dims( Zdata, axis=0 )
             self.count[idx] = idx
             self.time[idx] = time
             self.workdir[idx] = workdir
 
             if not image is None:
                 self.cam0images[idx] = image
```

### Comparing `wassgridsurface-0.5.7/wassgridsurface/wass_utils.py` & `wassgridsurface-0.6.0/wassgridsurface/wass_utils.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.5.7/wassgridsurface/wassgridsurface.py` & `wassgridsurface-0.6.0/wassgridsurface/wassgridsurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,32 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
-VERSION = "0.5.7"
+VERSION = "0.6.0"
 
 
 import argparse
 import configparser
 import scipy.io as sio
 import scipy.interpolate
 import os
 import sys
 import glob
+import time
 import numpy as np
 import matplotlib.pyplot as plt
 import cv2 as cv
 from os import path
 from tqdm import tqdm
+from tqdm.contrib.concurrent import thread_map
+
 
 import colorama
 colorama.init()
 from colorama import Fore, Back, Style
 
 from wassgridsurface.netcdfoutput import NetCDFOutput
 from wassgridsurface.wass_utils import load_camera_mesh, align_on_sea_plane, align_on_sea_plane_RT, compute_sea_plane_RT, filter_mesh_outliers
@@ -162,15 +165,15 @@
         "y_spacing":y_spacing,
         "fps":fps,
         "timestring":timestring
     } )
 
 
 
-def grid( wass_frames, matfile, outdir, subsample_percent=100, mf=0, algorithm="DCT", user_mask_filename=None, alg_options=None ):
+def grid( wass_frames, matfile, outdir, subsample_percent=100, mf=0, algorithm="DCT", user_mask_filename=None, alg_options=None, NUM_PARALLEL_PROCESSES=1 ):
     step=150
     gridsetup = sio.loadmat( matfile )
     XX = gridsetup["XX"]
     YY = gridsetup["YY"]
 
     Rpl = gridsetup["Rpl"]
     Tpl = gridsetup["Tpl"]
@@ -196,35 +199,50 @@
 
     outdata.set_instrinsics( np.zeros( (3,3), dtype=np.float32),
                              np.zeros( (3,3), dtype=np.float32),
                              np.zeros( (5,1), dtype=np.float32),
                              np.zeros( (5,1), dtype=np.float32),
                              gridsetup["P0plane"])
 
-    Zmean = 0.0
-    Zmin = np.Inf
-    Zmax = -np.Inf
-    N_frames = 1
+
+    wass_frames_with_indices = [ x for x in enumerate(wass_frames) ]
+    N_frames = len( wass_frames_with_indices )
+
 
     user_mask = np.ones( XX.shape, dtype=np.float32 )
 
     if not user_mask_filename is None:
         print("Loading %s"%user_mask_filename )
         user_mask = cv.imread( user_mask_filename, cv.IMREAD_GRAYSCALE )
         user_mask = (user_mask>0).astype(np.float32)
 
 
     print("Interpolation algorithm: "+Fore.RED+algorithm+Fore.RESET )
-    interpolator = IDWInterpolator( KSIZE=5, reps=1 ) if algorithm=="IDW" else DCTInterpolator( img_width=XX.shape[1], img_height=XX.shape[0], alg_options=alg_options )
+    print("Using %d thread(s) for reconstruction..."%NUM_PARALLEL_PROCESSES )
+
+
+    # Create a dedicated interpolator for each parallel process
+    interpolators = [ IDWInterpolator( KSIZE=5, reps=1 ) if algorithm=="IDW" else DCTInterpolator( img_width=XX.shape[1], img_height=XX.shape[0], alg_options=alg_options ) for x in range(NUM_PARALLEL_PROCESSES) ]
+
+    Zmeans = []
+    Zmins = []
+    Zmaxs = []
+
+    def _grid_task( iteration_element ):
+
+        idx, wdir = iteration_element
+        interpolator = interpolators[ idx % NUM_PARALLEL_PROCESSES ]
 
-    for wdir in tqdm(wass_frames):
         tqdm.write(wdir)
         dirname = path.split( wdir )[-1]
         FRAME_IDX = int(dirname[:-3])
 
+        if idx<=NUM_PARALLEL_PROCESSES:
+            time.sleep( idx ) # wait to optimize disk access
+
         meshname = path.join( wdir, "mesh_cam.xyzC")
         mesh = load_camera_mesh(meshname)
         mesh_aligned = align_on_sea_plane_RT( mesh, gridsetup["Rpl"], gridsetup["Tpl"]) * gridsetup["CAM_BASELINE"]
         mesh_aligned = mesh_aligned[:, np.random.permutation(mesh_aligned.shape[1]) ]
 
         # 3D point grid quantization
         scalefacx = (gridsetup["xmax"]-gridsetup["xmin"])
@@ -249,32 +267,32 @@
             for ii in range(NREPS):
                 np.random.shuffle( indices )
                 curr_indices = np.copy( indices[:n_pts] )
                 ZZ[ pts_y[indices[curr_indices]], pts_x[indices[curr_indices]], ii ] = pts_z[indices[curr_indices]]
 
             ZZ = np.nanmedian( ZZ, axis=-1 )
 
-            if N_frames == 1:
+            if idx == 0:
                 fig = plt.figure( figsize=(20,20))
                 plt.imshow( ZZ, vmin=gridsetup["zmin"], vmax=gridsetup["zmax"] )
                 figfile = path.join(outdir,"points.png" )
                 fig.savefig(figfile,bbox_inches='tight')
                 plt.close()
 
-            Zi, mask = interpolator(ZZ)
+            Zi, mask = interpolator(ZZ, verbose=(NUM_PARALLEL_PROCESSES==1) )
             mask *= user_mask
             Zi[ mask==0 ] = np.nan
 
             if mf>0:
                 Zi = Zi.astype(np.float32)
                 Zi[ mask==0 ] = 0
                 Zi = cv.medianBlur(Zi, ksize=mf)
                 Zi[ mask==0 ] = np.nan
 
-            if N_frames == 1:
+            if idx == 0:
                 fig = plt.figure( figsize=(20,20))
                 plt.imshow( Zi, vmin=gridsetup["zmin"], vmax=gridsetup["zmax"] )
                 figfile = path.join(outdir,"gridded.png" )
                 fig.savefig(figfile,bbox_inches='tight')
                 plt.close()
 
                 zmin, zmax = np.nanmin(Zi), np.nanmax(Zi)
@@ -389,55 +407,61 @@
             Zi = np.reshape( Zi, XX.shape )
             tqdm.write("done")
         else:
             print("Invalid interpolation algorithm, aborting")
             return
 
 
-        # Zi here contains the interpolated surface
-        Zmean = Zmean + (np.nanmean(Zi)-Zmean)/N_frames
-        Zmin = min( Zmin, np.nanmin(Zi) )
-        Zmax = max( Zmax, np.nanmax(Zi) )
+        # Zi now contains the interpolated surface
+
+        Zmeans.append( np.nanmean(Zi) )
+        Zmins.append( np.nanmin(Zi) )
+        Zmaxs.append( np.nanmax(Zi) )
 
 
         I0 = cv.imread( path.join(wdir,"00000000_s.png"))
         outdata.add_meta_attribute("image_width", I0.shape[1] )
         outdata.add_meta_attribute("image_height", I0.shape[0] )
         ret, imgjpeg = cv.imencode(".jpg", I0 )
 
         mask_filename = path.join( wdir, "undistorted", "mask0.png" ) 
         imagemask = None
         if path.exists( mask_filename ): 
             with open( mask_filename, "rb" ) as f:
                 imagemask = np.fromfile(f, np.uint8 );
 
-        outdata.push_Z( Zi*1000, float(N_frames-1)/float(fps) if fps>0 else 0.0, FRAME_IDX, imgjpeg, imagemask )
+        outdata.push_Z( Zi*1000, float(idx)/float(fps) if fps>0 else 0.0, FRAME_IDX, imgjpeg, imagemask, idx=idx )
 
 
         #aux = ((Zi-gridsetup["zmin"])/(gridsetup["zmax"]-gridsetup["zmin"])*255).astype(np.uint8)
         #cv.imwrite( path.join(outdir,"area_interp.png"), cv.resize(aux,(800,800), interpolation=cv.INTER_NEAREST ) )
 
         # fig = plt.figure( figsize=(20,20))
         # plt.imshow(Zi, vmin=gridsetup["zmin"], vmax=gridsetup["zmax"] )
         # figfile = path.join(outdir,"area_interp_%08d.png"%FRAME_IDX)
         # fig.savefig(figfile,bbox_inches='tight')
         # plt.close()
 
-        N_frames += 1
+    #------
+    r = thread_map(_grid_task, wass_frames_with_indices, max_workers=NUM_PARALLEL_PROCESSES )
+
 
 
+    Zmin = np.amin( np.array(Zmins)) 
+    Zmax = np.amax( np.array(Zmaxs)) 
+    Zmean = np.mean( np.array(Zmeans)) 
     outdata.add_meta_attribute("zmin", Zmin )
     outdata.add_meta_attribute("zmax", Zmax )
     outdata.add_meta_attribute("zmean", Zmean )
 
     print("Reconstructed sequence stats: ")
     print("    Zmin: ",Zmin)
     print("    Zmax: ",Zmax)
     print("   Zmean: ",Zmean)
-    print("# frames: ",N_frames-1)
+    print("# frames: ",N_frames)
 
     outdata.close()
 
 
 
 def wassgridsurface_main():
     print(" WASS surface gridder v.", VERSION )
@@ -477,14 +501,15 @@
     parser.add_argument("-f", "--fps", default=0, type=float, help="Sequence frames per second" )
     parser.add_argument("-t", "--timestring", default="", type=str, help="Sequence datetime string (ie. the RAW filename)" )
     parser.add_argument("-Iw", "--image_width", type=float, help="Camera frame width" )
     parser.add_argument("-Ih", "--image_height", type=float, help="Camera frame height" )
     parser.add_argument("--ss", "--subsample_percent", type=float, default=100, help="Point subsampling 0..100%%" )
     parser.add_argument("--mf", "--medianfilter", type=int, default=0, help="Median filter window size (0,3,5,7)" )
     parser.add_argument("-n", "--num_frames", type=int, default=-1, help="Number of frames to process. -1 to process all frames." )
+    parser.add_argument("-p", "--parallel", type=int, default=1, help="Number of parallel tasks to execute" )
     parser.add_argument("--ia", "--interpolation_algorithm", type=str, default="DCT", help='Interpolation algorithm to use. Alternatives are: "DCT", "IDW", "LinearND" ' )
     parser.add_argument("--mask", type=str, default=None, help='User supplied grid mask filename. Must be a grayscale (bw) image with the same size of the grid' )
     parser.add_argument("--dct_nfreqs", type=int, default=None, help="DCT interpolator number of frequencies" )
     parser.add_argument("--dct_regalpha", type=float, default=None, help="DCT interpolator regularizer alpha" )
     parser.add_argument("--dct_maxtol", type=float, default=None, help="DCT interpolator max function tolerance change" )
     parser.add_argument("--dct_lr", type=float, default=None, help="DCT interpolator learning rate" )
     parser.add_argument("--dct_maxiters", type=int, default=None, help="DCT interpolator max number of iterations" )
@@ -589,15 +614,16 @@
               user_mask_filename=args.mask,
               alg_options = {
                   "Nfreqs": args.dct_nfreqs,
                   "REGULARIZER_ALPHA": args.dct_regalpha,
                   "MAX_ITERS": args.dct_maxiters,
                   "TOLERANCE_CHANGE": args.dct_maxtol,
                   "LEARNING_RATE": args.dct_lr,
-                  })
+                  },
+              NUM_PARALLEL_PROCESSES=args.parallel )
 
         print("Gridding completed.")
 
     else:
         print("Invalid actions specified.")
         sys.exit(-2)
```

### Comparing `wassgridsurface-0.5.7/wassgridsurface.egg-info/PKG-INFO` & `wassgridsurface-0.6.0/wassgridsurface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.5.7
+Version: 0.6.0
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
```

### Comparing `wassgridsurface-0.5.7/wassgridsurface.egg-info/SOURCES.txt` & `wassgridsurface-0.6.0/wassgridsurface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

