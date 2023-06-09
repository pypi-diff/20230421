# Comparing `tmp/bacteria-0.0.3.tar.gz` & `tmp/bacteria-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.3.tar", last modified: Fri Apr 21 11:17:49 2023, max compression
+gzip compressed data, was "bacteria-0.0.4.tar", last modified: Fri Apr 21 11:22:19 2023, max compression
```

## Comparing `bacteria-0.0.3.tar` & `bacteria-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.940000 bacteria-0.0.3/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:17:49.870000 bacteria-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.497000 bacteria-0.0.3/bacteria/
--rw-rw-rw-   0        0        0      681 2023-04-21 11:17:27.000000 bacteria-0.0.3/bacteria/__init__.py
--rw-rw-rw-   0        0        0   163931 2023-04-21 10:50:06.000000 bacteria-0.0.3/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 11:16:40.000000 bacteria-0.0.3/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:17:49.793000 bacteria-0.0.3/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-21 11:17:49.000000 bacteria-0.0.3/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 11:17:48.000000 bacteria-0.0.3/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:17:49.908000 bacteria-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-04-21 11:17:38.000000 bacteria-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.539000 bacteria-0.0.4/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:22:19.456000 bacteria-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.179000 bacteria-0.0.4/bacteria/
+-rw-rw-rw-   0        0        0      681 2023-04-21 11:22:10.000000 bacteria-0.0.4/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   147595 2023-04-21 11:22:10.000000 bacteria-0.0.4/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 11:22:09.000000 bacteria-0.0.4/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.439000 bacteria-0.0.4/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:22:19.512000 bacteria-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 11:22:08.000000 bacteria-0.0.4/setup.py
```

### Comparing `bacteria-0.0.3/PKG-INFO` & `bacteria-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.3/bacteria/__init__.py` & `bacteria-0.0.4/bacteria/__init__.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.3/bacteria/functions.py` & `bacteria-0.0.4/bacteria/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3758,430 +3758,14 @@
 		if key == 'all':
 			out.append(ax.set_title('{} cells'.format(key.capitalize()),fontsize = 17))
 		else:
 			out.append(ax.set_title('{} {} min cells'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17))
 		out.append(ax.legend())
 		return out
 
-def format_images(src_folder, double = True):
-    """
-    Copy files from a folder using SuperSegger format. 
-    
-    Parameters
-    --------------
-    src_folder: str
-        raw images path (in .tif)
-    double : bool (optional, default True)
-        create a fake channel in the data (BF and GFP)
-        
-    Returns
-    --------------
-    None
-    """
-    raw_folder = src_folder + os.sep + 'orig_images' + os.sep if src_folder[-1] != os.sep else src_folder + 'orig_images' + os.sep
-    ref_xy  = 'xy' 
-    ref_bf  = 'c1.tif' 
-    ref_gfp = 'c2.tif' 
-    sub_folders = [folder.path for folder in os.scandir(src_folder) if folder.is_dir()]
-
-    # # fetch all files in all sub-folders
-    if len(sub_folders):
-        for idx_f,folder in enumerate(sub_folders):
-            ref_idx = sub_folders[idx_f].split(os.sep)[-1]
-            for idx,file_name in enumerate(natsorted(os.listdir(folder))):
-                # construct full file path
-                source = folder + os.sep + file_name if folder[-1] != os.sep else folder + file_name
-                # copy only tif images
-                if source[-4:] == '.tif':
-                    shutil.copy(source, src_folder + os.sep + 't%05d' % (idx+1) + ref_xy + '%03d' % int(ref_idx) + ref_bf)
-                    # duplicate images in two channels (BF and GFP)
-                    if double:
-                        shutil.copy(source, src_folder + os.sep + 't%05d' % (idx+1) + ref_xy + '%03d' % int(ref_idx) + ref_gfp)
-    else:
-        try:
-            os.makedirs(raw_folder)
-        except FileExistsError:
-            pass
-
-        for idx,file_name in enumerate(natsorted(os.listdir(src_folder))):
-            # construct full file path
-            source = src_folder + os.sep + file_name if src_folder[-1] != os.sep else src_folder + file_name
-            if source[-4:] == '.tif':
-                shutil.move(source, raw_folder)
-
-        for idx,file_name in enumerate(natsorted(os.listdir(raw_folder))):
-            # construct full file path
-            source = raw_folder + os.sep + file_name if raw_folder[-1] != os.sep else raw_folder + file_name
-            
-            # copy only tif images
-            if source[-4:] == '.tif':
-                shutil.copy(source, src_folder + os.sep + 't%05d' % (idx+1) + 'xy001c1.tif')
-                # duplicate images in two channels (BF and GFP)
-                if double:
-                    shutil.copy(source, src_folder + os.sep + 't%05d' % (idx+1) + 'xy001c2.tif')
-                    
-def sub_folders_path(src_folder):
-    """
-    Create the path for omnipose. 
-    
-    Parameters
-    --------------
-    src_folder : str
-        folders or raw images(in .tif) path 
-        
-    Returns
-    --------------
-    folder_omni : list
-        phase paths for each data in the source folder
-    folder_mask : list
-        mask path for each data in the source folder
-    clist_list : list
-        clist path for each output from supersegger
-    """
-    sub_folder = [folder.path for folder in os.scandir(src_folder) if folder.is_dir()]
-    folder_omni = []
-    folder_mask = []
-    clist_list = []
-    s = os.sep
-
-    for idx,_ in enumerate(sub_folder):
-        ref_idx = sub_folder[idx].split(os.sep)[-1]
-        folder_omni.append(src_folder + s + 'xy' + str(ref_idx) + s +'phase'+ s if src_folder[-1] != s else src_folder + 'xy' + str(ref_idx) + s +'phase' + s)
-        folder_mask.append(src_folder + s + 'xy' + str(ref_idx) + s +'masks'+ s if src_folder[-1] != s else src_folder + 'xy' + str(ref_idx) + s +'masks' + s)
-        clist_list.append(src_folder + s + 'xy' + str(ref_idx) + s +'clist.mat' if src_folder[-1] != s else src_folder + 'xy' + str(ref_idx) + s +'clist.mat')
-    return natsorted(folder_omni),natsorted(folder_mask),natsorted(clist_list)
-
-def multiple_experiments(data_path,format_image, align):
-    """
-    Run the Pipeline* for multiple experiments. 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - Data Folder ('data_path' with all experiments):
-        - Experiment 1
-        - Experiment 2
-        - Experiment 3
-            - 01 (FOV 1 - must have 0 first to run in order)
-            - 02 (FOV 2)
-            - 03 (FOV 3)
-            ...
-            - 30 (FOV 30)
-
-    * SuperSegger -> Omnipose -> SuperSegger 
-    
-    Parameters
-    --------------
-    data_path : str
-        folder path with all experiments inside
-    format_image : bool
-        format image to be used by SuperSegger
-    align : bool
-        Use the SuperSegger algorithm to align 
-        all the images with the first one 
-        
-    Returns
-    --------------
-    None
-    """
-
-    print('Running - Multiple Experiments Analysis')
-
-    experiments = natsorted([fd.path for fd in os.scandir(data_path) if fd.is_dir()])
-
-    if align == True:
-        align_var = 1
-    else:
-        align_var = 0
-
-    for _,experiment in enumerate(experiments):
-        print('Experiment: ' + experiment)
-        if format_image: format_images(experiment)
-
-        sub_folders = natsorted([fd.path for fd in os.scandir(experiment) if fd.is_dir()])
-        folder_omni,folder_mask,clist_list = sub_folders_path(experiment)
-
-        st = time.time()
-
-        print('Loading matlab')
-        eng = matlab.engine.start_matlab()
-        print('Starting the segmentation')
-        eng.pipeline(experiment,align_var,nargout=0)
-
-        time_idx = {}
-
-        for xy,_ in enumerate(sub_folders):
-            st_idx = time.time()
-            ref_log = sub_folders[xy].split(os.sep)[-1]
-            print('Checking masks for xy'+str(ref_log)+'...') if 'xy' not in ref_log else print('Checking masks for '+str(ref_log)+'...')
-
-            if os.path.exists(folder_mask[xy]) == False and 'xy' not in ref_log and 'raw' not in ref_log:
-                print('Masks not generated for xy'+str(ref_log)) if 'xy' not in ref_log else print('Masks not generated for '+str(ref_log))
-                print('Starting Omnipose!')
-                if os.path.exists(folder_omni[xy]) == False:
-                    temp = experiment + os.sep + 'xy' + str(ref_log[-1]) + os.sep +'phase'+ os.sep if experiment[-1] != os.sep else experiment + 'xy' + str(ref_log[-1]) + os.sep +'phase' + os.sep
-                    os.system('python -m omnipose --dir %s --save_png --dir_above --no_npy --in_folders  --omni --pretrained_model bact_fluor_omni --cluster --mask_threshold 1 --flow_threshold 0 --diameter 30'%(temp))
-                else:
-                    os.system('python -m omnipose --dir %s --save_png --dir_above --no_npy --in_folders  --omni --pretrained_model bact_fluor_omni --cluster --mask_threshold 1 --flow_threshold 0 --diameter 30'%(folder_omni[xy]))       
-            else:
-                print('Masks already generated for xy'+str(ref_log)) if 'xy' not in ref_log else print('Masks already generated for '+str(ref_log)),print('Skipping this step')
-
-            print('Finishing the segmentation for xy'+str(ref_log)) if 'xy' not in ref_log else print('Finishing the segmentation for '+str(ref_log))
-            et_idx = time.time()
-            elapsed_time_idx = et_idx - st_idx
-            time_idx[ref_log] = str(timedelta(seconds = elapsed_time_idx))[:7]
-            
-        eng.pipeline2(experiment,align_var,nargout=0)
-        
-        et = time.time()
-        elapsed_time = str(timedelta(seconds = (et - st)))
-
-        print('Execution time : ', elapsed_time, ' seconds')
-
-        log_path = experiment + os.sep + 'log-'+str(date.today())+'.txt' if experiment[-1] != os.sep else experiment + 'log-'+str(date.today())+'.txt'   
-        title_log = 'Log Pipeline ' + str(date.today())
-        total_time = 'Experiment: ' +  experiment.split(os.sep)[-1] + ', Execution time: ' + str(elapsed_time) + ' (h/m/s)'
-
-        with open(log_path, "w") as f:
-            f.write(str(title_log))
-            for idx, data in time_idx.items():
-                f.write('\n'+'Experiment '+ experiment.split(os.sep)[-1] + ', Field of view '+str(idx) + ': '+ str(data) + ' (h/m/s)')
-            f.write('\n')
-            f.write(str(total_time))
-
-def multiple_fovs(data_path, format_image, align):
-    """
-    Run the Pipeline* for multiple Field of Views (FOV's). 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - Experiment folder ('data_path' with all FOV's):
-        - 01 (FOV 1 - must have 0 first to run in order)
-        - 02 (FOV 2)
-        - 03 (FOV 3)
-        ...
-        - 30 (FOV 30)
-
-    * SuperSegger -> Omnipose -> SuperSegger 
-    
-    Parameters
-    --------------
-    data_path : str
-        folder path with all experiments inside
-    format_image : bool
-        format image to be used by SuperSegger 
-    align : bool
-        Use the SuperSegger algorithm to align 
-        all the images with the first one 
-        
-    Returns
-    --------------
-    None
-    """
-
-    print("Running - Multiple FOV's Analysis")
-
-    folder = data_path
-
-    if align == True:
-        align_var = 1
-    else:
-        align_var = 0
-
-    if format_image: format_images(folder)
-
-    sub_folders = natsorted([fd.path for fd in os.scandir(folder) if fd.is_dir()])
-    folder_omni,folder_mask,_ = sub_folders_path(folder)
-
-    st = time.time()
-
-    print('Loading matlab')
-    eng = matlab.engine.start_matlab()
-    print('Starting the segmentation')
-    eng.pipeline(folder,align_var,nargout=0)
-
-    time_idx = {}
-
-    for xy,_ in enumerate(sub_folders):
-        st_idx = time.time()
-        ref_log = sub_folders[xy].split(os.sep)[-1]
-        print('Checking masks for xy'+str(ref_log)+'...') if 'xy' not in ref_log else print('Checking masks for '+str(ref_log)+'...')
-        if os.path.exists(folder_mask[xy]) == False and 'xy' not in ref_log and 'raw' not in ref_log:
-            print('Masks not generated for xy'+str(ref_log)) if 'xy' not in ref_log else print('Masks not generated for '+str(ref_log))
-            print('Starting Omnipose!')
-            os.system('python -m omnipose --dir %s --save_png --dir_above --no_npy --in_folders  --omni --pretrained_model bact_fluor_omni --cluster --mask_threshold 1 --flow_threshold 0 --diameter 30'%(folder_omni[xy]))
-            print(folder_omni[xy]),print(folder_mask[xy]),print('Omnipose finished')
-        else:
-            print('Masks already generated for xy'+str(ref_log)) if 'xy' not in ref_log else print('Masks already generated for '+str(ref_log)),print('Skipping this step')
-
-        print('Finishing the segmentation for xy'+str(ref_log)) if 'xy' not in ref_log else print('Finishing the segmentation for '+str(ref_log))
-        et_idx = time.time()
-        elapsed_time_idx = et_idx - st_idx
-        time_idx[ref_log] = str(timedelta(seconds = elapsed_time_idx))[:7]
-        
-    eng.pipeline2(folder,align_var,nargout=0)
-
-    et = time.time()
-    elapsed_time = str(timedelta(seconds = (et - st)))
-
-    print('Execution time : ', elapsed_time, ' seconds')
-
-    log_path = folder + os.sep + 'log-'+str(date.today())+'.txt' if folder[-1] != os.sep else folder + 'log-'+str(date.today())+'.txt'
-    title_log = 'Log Pipeline ' + str(date.today())
-    total_time = 'Execution time: ' + str(elapsed_time) + ' (h/m/s)'
-
-    with open(log_path, "w") as f:
-        f.write(str(title_log))
-        for idx, data in time_idx.items():
-            f.write('\n'+'Field of view '+str(idx) + ': '+ str(data) + ' (h/m/s)')
-        f.write('\n')
-        f.write(str(total_time))
-
-def one_fov(data_path,format_image, align):   
-    """
-    Run the Pipeline* for one Field of View (FOV). 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - FOV folder ('data_path' with the images)
-
-    * SuperSegger -> Omnipose -> SuperSegger 
-    
-    Parameters
-    --------------
-    data_path : str
-        folder path with all experiments inside
-    format_image : bool
-        format image to be used by SuperSegger 
-    align : bool
-        Use the SuperSegger algorithm to align 
-        all the images with the first one 
-        
-    Returns
-    --------------
-    None
-    """
-    print('Running - One FOV Analysis')
-
-    folder = data_path
-
-    if align == True:
-        align_var = 1
-    else:
-        align_var = 0
-
-    folder_omni = folder + os.sep + 'xy1/phase/' if folder[-1] != os.sep else folder + 'xy1/phase/'
-    folder_mask = folder + os.sep + 'xy1/masks/' if folder[-1] != os.sep else folder + 'xy1/masks/'
-
-    st = time.time()
-
-    if format_image: format_images(folder)
-
-    print('Loading matlab')
-    eng = matlab.engine.start_matlab()
-    print('Starting the segmentation')
-    eng.pipeline(folder,align_var,nargout=0)
-
-    print('Checking masks...')
-
-    if os.path.exists(folder_mask) == False and 'xy':
-        print('Masks not generated')
-        print('Starting Omnipose!')
-        os.system('python -m omnipose --dir %s --save_png --dir_above --no_npy --in_folders  --omni --pretrained_model bact_fluor_omni --cluster --mask_threshold 1 --flow_threshold 0 --diameter 30'%(folder_omni))
-        print(folder_omni)
-        print(folder_mask)
-    else:
-        print('Masks already generated, skipping this step')
-
-    print('Omnipose finished')
-
-    et = time.time()
-    elapsed_time = str(timedelta(seconds = (et - st)))
-
-    log_path = folder + os.sep + 'log-'+str(date.today())+'.txt' if folder[-1] != os.sep else folder + 'log-'+str(date.today())+'.txt'   
-    title_log = 'Log Pipeline ' + str(date.today())
-    total_time = 'Execution time: ' + str(elapsed_time) + ' (h/m/s)'
-
-    with open(log_path, "w") as f:
-        f.write(str(title_log))
-        f.write('\n')
-        f.write(str(total_time))  
-    
-    print('Finishing the segmentation')
-    eng.pipeline2(folder,align_var,nargout=0)
-
-def help_pipeline():
-    """
-    One FOV
-    --------------
-    Run the Pipeline* for one Field of View (FOV). 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - FOV folder ('data_path' with the images)
-
-    Multiple FOV's
-    --------------
-    Run the Pipeline* for multiple Field of Views (FOV's). 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - Experiment folder ('data_path' with all FOV's):
-        - 01 (FOV 1 - must have 0 first to run in order)
-        - 02 (FOV 2)
-        - 03 (FOV 3)
-        ...
-        - 30 (FOV 30)
-
-    Multiple Experiments
-    --------------
-    Run the Pipeline* for multiple experiments. 
-    To use 'format_image': bool variable, 0 the data must
-    be already in the SuperSegger format, if 1 the data must
-    be in sequence in .tiff files. This code will duplicate
-    the files and format the name properly (ch1 and ch2).
-    
-    To run this code the data must be organized as:
-    - Data Folder ('data_path' with all experiments):
-        - Experiment 1
-        - Experiment 2
-        - Experiment 3
-            - 01 (FOV 1 - must have 0 first to run in order)
-            - 02 (FOV 2)
-            - 03 (FOV 3)
-            ...
-            - 30 (FOV 30)
-
-    * SuperSegger -> Omnipose -> SuperSegger 
-    
-    Parameters
-    --------------
-    data_path : str
-        folder path with all experiments inside
-    format_image : bool
-        format image to be used by SuperSegger
-    align : bool
-        Use the SuperSegger algorithm to align 
-        all the images with the first one  
-    """
-
 # !pip install session-info
 # !pip install pipreqs
 # !pip install nbconvert
 # %cd code
 # !jupyter nbconvert --output-dir="./reqs" --to script 200707.ipynb
 # %cd reqs
 # !pipreqs
```

### Comparing `bacteria-0.0.3/bacteria/pipeline.py` & `bacteria-0.0.4/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.3/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.4/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.3/setup.py` & `bacteria-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.3',      
+    version = '0.0.4',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

