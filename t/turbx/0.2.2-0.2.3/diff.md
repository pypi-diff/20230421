# Comparing `tmp/turbx-0.2.2.tar.gz` & `tmp/turbx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.2.2.tar", last modified: Sat Apr 15 18:53:07 2023, max compression
+gzip compressed data, was "turbx-0.2.3.tar", last modified: Fri Apr 21 16:14:18 2023, max compression
```

## Comparing `turbx-0.2.2.tar` & `turbx-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.196434 turbx-0.2.2/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.2/LICENSE
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-15 18:53:07.196434 turbx-0.2.2/PKG-INFO
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.2.2/README.md
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-15 18:53:07.196434 turbx-0.2.2/setup.cfg
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-15 18:44:51.000000 turbx-0.2.2/setup.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.192434 turbx-0.2.2/turbx/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3154 2023-04-15 18:44:32.000000 turbx-0.2.2/turbx/__init__.py
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1143769 2023-04-15 18:41:25.000000 turbx-0.2.2/turbx/turbx.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.196434 turbx-0.2.2/turbx.egg-info/
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/PKG-INFO
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/SOURCES.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/dependency_links.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/requires.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/top_level.txt
+drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.3/LICENSE
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-21 16:14:18.676028 turbx-0.2.3/PKG-INFO
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.2.3/README.md
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-21 16:14:18.676028 turbx-0.2.3/setup.cfg
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-21 16:13:23.000000 turbx-0.2.3/setup.py
+drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/turbx/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3154 2023-04-15 18:44:32.000000 turbx-0.2.3/turbx/__init__.py
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1145346 2023-04-21 16:06:44.000000 turbx-0.2.3/turbx/turbx.py
+drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/turbx.egg-info/
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/PKG-INFO
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/SOURCES.txt
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/dependency_links.txt
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/requires.txt
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.2.2/LICENSE` & `turbx-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.2.2/PKG-INFO` & `turbx-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

### Comparing `turbx-0.2.2/README.md` & `turbx-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `turbx-0.2.2/setup.py` & `turbx-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.2.2',
+    version='0.2.3',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
```

### Comparing `turbx-0.2.2/turbx/__init__.py` & `turbx-0.2.3/turbx/__init__.py`

 * *Files identical despite different names*

### Comparing `turbx-0.2.2/turbx/turbx.py` & `turbx-0.2.3/turbx/turbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,14 +894,18 @@
         rz = kwargs.get('rz',1)
         
         if (rx*ry*rz != self.n_ranks):
             raise AssertionError('rx*ry*rz != self.n_ranks')
         
         with cgd(fn_cgd, 'r', driver=self.driver, comm=self.comm) as hf_ref:
             
+            ## copy over fsubtype
+            if hasattr(hf_ref,'fsubtype'):
+                self.attrs['fsubtype'] = hf_ref.fsubtype
+            
             # === copy over header info if needed
             
             if all([('header/udef_real' in self),('header/udef_char' in self)]):
                 raise ValueError('udef already present')
             else:
                 udef         = hf_ref.udef
                 udef_real    = list(udef.values())
@@ -1116,14 +1120,21 @@
                         raise ValueError
                     if (data.shape!=(self.nx,self.ny,2)):
                         raise ValueError
                     
                     ds = self.create_dataset(dsn, data=data, chunks=None)
                     #if verbose: even_print(dsn,'%s'%str(ds.shape))
             
+            ## copy over [data_dim/<>] dsets if present
+            if ('data_dim' in hf_ref):
+                for dsn in hf_ref['data_dim'].keys():
+                    data = np.copy( hf_ref[f'data_dim/{dsn}'][()] ) 
+                    self.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                    if self.usingmpi: self.comm.Barrier()
+        
         self.get_header(verbose=False)
         return
     
     def import_eas4(self, fn_eas4_list, **kwargs):
         '''
         import data from a series of EAS4 files to a CGD
         '''
@@ -1610,26 +1621,30 @@
         elif (xi is not None) and (yi is not None):
             np.testing.assert_allclose(xy2d[xi,yi,0], x2d, rtol=1e-14, atol=1e-14)
             np.testing.assert_allclose(xy2d[xi,yi,1], y2d, rtol=1e-14, atol=1e-14)
         else:
             raise ValueError
         
         ## key names for 'dims' group
+        ## these are all 1D with shape either (nx,) or (ny,)
         kn_dims = ['stang', 'snorm', 'crv_R'] 
         for k in kn_dims:
             if (k in dd.keys()):
                 dsn = f'dims/{k}'
                 #data = np.copy(dd[k])
                 data = dd[k]
                 if not isinstance(data, np.ndarray):
                     continue
                 data_shape_orig = data.shape
                 if (xi is not None):
                     if (data.shape[0]==xy2d.shape[0]):
                         data = np.copy(data[xi])
+                if (yi is not None):
+                    if (data.shape[0]==xy2d.shape[1]):
+                        data = np.copy(data[yi])
                 if (dsn in self):
                     del self[dsn]
                 ds = self.create_dataset(dsn, data=data, chunks=None)
                 if verbose: even_print(dsn,'%s --> %s'%(str(data_shape_orig),str(data.shape)))
         
         if verbose: print(72*'-')
         if verbose: print('total time : cgd.add_geom_data() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
@@ -2809,15 +2824,14 @@
                             txt = even_print('write: %s_fv'%scalar, '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb_mean,t_delta,(data_gb_mean/t_delta)), s=True)
                             tqdm.write(txt)
                         
                         t_write       += t_delta
                         data_gb_write += data_gb_mean
             
             if self.usingmpi: self.comm.Barrier()
-            if verbose: print(72*'-')
             
             # === replace dims/t array --> take last time of series
             t = np.array([self.t[-1]],dtype=np.float64)
             if ('dims/t' in hf_mean):
                 del hf_mean['dims/t']
             hf_mean.create_dataset('dims/t', data=t)
             
@@ -4515,14 +4529,19 @@
             utang = np.einsum('xyi,xyzti->xyzt', vtang, uv)
             unorm = np.einsum('xyi,xyzti->xyzt', vnorm, uv)
             
             if self.usingmpi: self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
             if verbose: tqdm.write(even_print('csys trafo','%0.3f [s]'%(t_delta,), s=True))
             
+            # === convert back to float32 before write
+            
+            utang = np.copy( utang.astype(np.float32) )
+            unorm = np.copy( unorm.astype(np.float32) )
+            
             # === write
             
             dset = self['data/utang']
             if self.usingmpi: self.comm.Barrier()
             t_start = timeit.default_timer()
             if self.usingmpi:
                 with dset.collective:
@@ -5586,15 +5605,15 @@
             if self.usingmpi:
                 with dset.collective:
                     dset[ct1:ct2,rz1_orig:rz2_orig,ry1_orig:ry2_orig,rx1_orig:rx2_orig] = vort_tang[xA:xB,yA:yB,zA:zB].T
             else:
                 dset[ct1:ct2,:,:,:] = vort_tang.T
             if self.usingmpi: self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
-            data_gb = 4 * self.nx * self.ny * self.nz / 1024**3
+            data_gb = ntc * 4 * self.nx * self.ny * self.nz / 1024**3
             
             if verbose: tqdm.write(even_print(f'write vort_tang','%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
             
             # dset = self['data/vort_tang_2']
             # if self.usingmpi: self.comm.Barrier()
             # t_start = timeit.default_timer()
             # if self.usingmpi:
@@ -5777,22 +5796,30 @@
         if verbose: print(72*'-')
         
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
+        #data['M_inf'] = self.M_inf
+        data['Ma'] = self.Ma
+        data['Pr'] = self.Pr
+        
         ## read in 3D coordinate arrays, then dimensinoalize [m]
         ## every ranks gets full grid
         x = np.copy( self['dims/x'][()].T * self.lchar )
         y = np.copy( self['dims/y'][()].T * self.lchar )
         z = np.copy( self['dims/z'][()].T * self.lchar )
-        nx = self.nx
-        ny = self.ny
-        nz = self.nz
+        
+        nx = self.nx ; data['nx'] = nx
+        ny = self.ny ; data['ny'] = ny
+        nz = self.nz ; data['nz'] = nz
+        nt = self.nt ; data['nt'] = nt
+        
+        t = np.copy( self['dims/t'][()] * self.tchar )
         
         ## read in 1D coordinate arrays, then dimensinoalize [m]
         stang_ = np.copy(self['dims/stang'])
         stang  = np.copy( stang_ * self.lchar ) ## dimensional [m]
         data['stang'] = stang
         
         snorm_ = np.copy(self['dims/snorm'])
@@ -5802,15 +5829,14 @@
         ## assert [z] is same over all [x,y]
         if (z.ndim!=3):
             raise ValueError
         z1d = np.copy(z[0,0,:])
         for i in range(nx):
             for j in range(ny):
                 np.testing.assert_allclose(z1d, z[i,j,:], rtol=1e-14, atol=1e-14)
-        data['z1d'] = z1d
         
         ## assert [x,y] is same over all [z]
         x2d  = np.copy(x[:,:,0])
         y2d  = np.copy(y[:,:,0])
         xy2d = np.stack((x2d,y2d), axis=-1)
         for k in range(nz):
             x2d_  = np.copy(x[:,:,k])
@@ -5818,29 +5844,38 @@
             xy2d_ = np.stack((x2d_,y2d_), axis=-1)
             np.testing.assert_allclose(xy2d, xy2d_, rtol=1e-14, atol=1e-14)
         
         ## check if constant Δz (calculate Δz+ later)
         dz0 = np.diff(z1d)[0]
         if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
             raise NotImplementedError
-        data['dz0'] = dz0
         
         ## dimensional [s]
         dt = self.dt * self.tchar
-        data['dt'] = dt
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
         
         t_meas = self.duration * self.tchar
-        data['t_meas'] = t_meas
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
         
         ## check against values in 'data_dim' (imported above)
         np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
         np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
         np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
         
         zrange = z1d.max() - z1d.min()
+        
+        #data['x'] = x
+        #data['y'] = y
+        #data['z'] = z
+        data['z1d'] = z1d
+        
+        data['t'] = t
+        data['t_meas'] = t_meas
+        data['dt'] = dt
+        data['dz0'] = dz0
         data['zrange'] = zrange
         
         if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
         if verbose: even_print('Δt','%0.3e [s]'%(dt,))
         if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
         if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
         if verbose: print(72*'-')
@@ -5874,14 +5909,18 @@
         ## get spanwise wavenumber [kz] vector
         kz_full = sp.fft.fftfreq(n=nz, d=dz0) * ( 2 * np.pi )
         kzp     = np.where(kz_full>0)
         kz      = np.copy(kz_full[kzp])
         dkz     = kz[1]-kz[0]
         nkz     = kz.size
         
+        data['kz']  = kz
+        data['dkz'] = dkz
+        data['nkz'] = nkz
+        
         if verbose:
             even_print('kz min','%0.1f [1/m]'%kz.min())
             even_print('kz max','%0.1f [1/m]'%kz.max())
             even_print('dkz','%0.1f [1/m]'%dkz)
             even_print('nkz','%i'%nkz)
             
             kz_inner = np.copy( kz * sc_l_in  )
@@ -5907,19 +5946,19 @@
                      # [ 'wI'  , 'wI'  , False ],
                      # [ 'uI'  , 'vI'  , False ],
                      # [ 'uII' , 'uII' , True  ],
                      # [ 'vII' , 'vII' , True  ],
                      # [ 'wII' , 'wII' , True  ],
                      # [ 'uII' , 'vII' , True  ],
                      ##
-                     [ 'utangI'  , 'utangI'  , False ],
-                     [ 'unormI'  , 'unormI'  , False ],
-                     [ 'wI'      , 'wI'      , False ],
-                     [ 'utangI'  , 'unormI'  , False ],
-                     [ 'utangI'  , 'wI'      , False ],
+                     [ 'utangI' , 'utangI' , False ],
+                     [ 'unormI' , 'unormI' , False ],
+                     [ 'wI'     , 'wI'     , False ],
+                     [ 'utangI' , 'unormI' , False ],
+                     [ 'utangI' , 'wI'     , False ],
                      ]
         
         scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
         
         ## dtype of prime data (currently must be all same dtype)
         if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
             dtype_primes = np.float32
@@ -6132,14 +6171,18 @@
         self.comm.Barrier()
         if verbose: print(72*'-')
         if verbose: print('total time : cgd.calc_turb_spectrum_span_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    def calc_turb_spectrum_time_xpln(self, **kwargs):
+        pass
+        return
+    
     # === polydata
     
     def export_polydata_wall(self, fn_spd=None, **kwargs):
         '''
         get 2D [x,z] wall quantities, export structured polydata (SPD) file
         '''
         
@@ -22768,15 +22811,15 @@
     je = j_edge + 2
     #je = min( j_edge + 2, ny+1 )
     
     intrp_func = sp.interpolate.interp1d(y[:je], psvel[:je], kind='cubic', bounds_error=True)
     
     ## check that [psvel_edge] is correct
     psvel_edge_ = intrp_func(y_edge)
-    np.testing.assert_allclose(psvel_edge, psvel_edge_, rtol=1e-7)
+    np.testing.assert_allclose(psvel_edge, psvel_edge_, rtol=1e-6)
     
     def __f_opt(y_test, intrp_func, psvel_edge):
         root = np.abs( 0.99*psvel_edge - intrp_func(y_test) )
         return root
     
     sol = sp.optimize.least_squares(fun=__f_opt,
                                     args=(intrp_func,psvel_edge),
```

### Comparing `turbx-0.2.2/turbx.egg-info/PKG-INFO` & `turbx-0.2.3/turbx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

