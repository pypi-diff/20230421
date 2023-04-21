# Comparing `tmp/sciopy-0.6.2-py3-none-any.whl.zip` & `tmp/sciopy-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 22938 bytes, number of entries: 15
--rw-rw-r--  2.0 unx     3863 b- defN 23-Mar-17 08:24 sciopy/__init__.py
+Zip file size: 25398 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx     4427 b- defN 23-Apr-21 07:14 sciopy/__init__.py
 -rw-rw-r--  2.0 unx     2314 b- defN 23-Feb-03 15:20 sciopy/com_handling.py
--rw-rw-r--  2.0 unx    39449 b- defN 23-Mar-16 15:11 sciopy/configurations.py
+-rw-rw-r--  2.0 unx    39449 b- defN 23-Mar-24 09:14 sciopy/configurations.py
 -rw-rw-r--  2.0 unx     4417 b- defN 23-Feb-07 14:52 sciopy/doteit.py
--rw-rw-r--  2.0 unx     8849 b- defN 23-Mar-16 14:27 sciopy/npztocsv.py
--rw-rw-r--  2.0 unx     6598 b- defN 23-Mar-17 13:35 sciopy/prepare_data.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Apr-21 07:14 sciopy/meshing.py
+-rw-rw-r--  2.0 unx     8922 b- defN 23-Apr-21 07:14 sciopy/npztocsv.py
+-rw-rw-r--  2.0 unx     9375 b- defN 23-Apr-21 07:14 sciopy/prepare_data.py
 -rw-rw-r--  2.0 unx     4372 b- defN 23-Mar-16 14:59 sciopy/print_command_info.py
--rw-rw-r--  2.0 unx     3484 b- defN 23-Mar-17 07:12 sciopy/sciopy_dataclasses.py
--rw-rw-r--  2.0 unx    20412 b- defN 23-Mar-16 15:13 sciopy/setup_m.py
--rw-rw-r--  2.0 unx     7469 b- defN 23-Mar-17 13:35 sciopy/visualization.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-Mar-23 14:15 sciopy-0.6.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2625 b- defN 23-Mar-23 14:15 sciopy-0.6.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-23 14:15 sciopy-0.6.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-23 14:15 sciopy-0.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1168 b- defN 23-Mar-23 14:15 sciopy-0.6.2.dist-info/RECORD
-15 files, 106181 bytes uncompressed, 21036 bytes compressed:  80.2%
+-rw-rw-r--  2.0 unx     3484 b- defN 23-Mar-24 09:14 sciopy/sciopy_dataclasses.py
+-rw-rw-r--  2.0 unx    20412 b- defN 23-Mar-24 09:14 sciopy/setup_m.py
+-rw-rw-r--  2.0 unx     7482 b- defN 23-Apr-21 07:14 sciopy/visualization.py
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Apr-21 07:17 sciopy-0.6.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2396 b- defN 23-Apr-21 07:17 sciopy-0.6.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 07:17 sciopy-0.6.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-21 07:17 sciopy-0.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1242 b- defN 23-Apr-21 07:17 sciopy-0.6.3.dist-info/RECORD
+16 files, 114138 bytes uncompressed, 23386 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: sciopy/configurations.py
 Comment: 
 
 Filename: sciopy/doteit.py
 Comment: 
 
+Filename: sciopy/meshing.py
+Comment: 
+
 Filename: sciopy/npztocsv.py
 Comment: 
 
 Filename: sciopy/prepare_data.py
 Comment: 
 
 Filename: sciopy/print_command_info.py
@@ -24,23 +27,23 @@
 
 Filename: sciopy/setup_m.py
 Comment: 
 
 Filename: sciopy/visualization.py
 Comment: 
 
-Filename: sciopy-0.6.2.dist-info/LICENSE
+Filename: sciopy-0.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: sciopy-0.6.2.dist-info/METADATA
+Filename: sciopy-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: sciopy-0.6.2.dist-info/WHEEL
+Filename: sciopy-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: sciopy-0.6.2.dist-info/top_level.txt
+Filename: sciopy-0.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sciopy-0.6.2.dist-info/RECORD
+Filename: sciopy-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sciopy/__init__.py

```diff
@@ -18,15 +18,24 @@
 from .print_command_info import (
     print_syntax,
     print_general_system_messages,
     print_acknowledge_messages,
     print_command_list,
 )
 
-from .prepare_data import create_prep_directory, prepare_all_samples_for_16_el
+from .prepare_data import (
+    create_prep_directory,
+    extract_potentials_from_sample_n_el_16,
+    comp_tank_relative_r_phi,
+    check_n_el_condition,
+    extract_electrodepotentials,
+    norm_data,
+    prepare_all_samples_for_16_el,
+    compute_v,
+)
 
 from .visualization import (
     plot_el_sign,
     plot_potential_matrix,
     plot_completeness,
     plot_temperatur_curve,
 )
@@ -79,14 +88,21 @@
 from .npztocsv import (
     clear_s_dict,
     single_measurement_to_csv_n_el_16,
     convert_measurement_directory_n_el_16,
     convert_measurement_directory_n_el_16_r_split,
 )
 
+from .meshing import (
+    create_empty_2d_mesh,
+    add_circle_anomaly,
+    plot_mesh,
+    mesh_sample,
+)
+
 # TBD from .configurations import configuration_01
 
 __all__ = [
     # .doteit
     "doteit_in_SingleEitFrame",
     "list_eit_files",
     "list_all_files",
@@ -143,19 +159,30 @@
     "configuration_02",
     "configuration_03",
     "configuration_04",
     "configuration_05",
     "configure_configuration",
     # .prepare_data
     "create_prep_directory",
+    "extract_potentials_from_sample_n_el_16",
+    "comp_tank_relative_r_phi",
+    "check_n_el_condition",
+    "extract_electrodepotentials",
+    "norm_data",
     "prepare_all_samples_for_16_el",
+    "compute_v",
     # .visualization
     "plot_potential_matrix",
     "plot_el_sign",
     "plot_completeness",
     "plot_temperatur_curve",
     # .npztocsv
     "clear_s_dict",
     "single_measurement_to_csv_n_el_16",
     "convert_measurement_directory_n_el_16",
     "convert_measurement_directory_n_el_16_r_split",
+    # .meshing
+    "create_empty_2d_mesh",
+    "add_circle_anomaly",
+    "plot_mesh",
+    "mesh_sample",
 ]
```

## sciopy/npztocsv.py

```diff
@@ -226,19 +226,20 @@
     """
 
     if len(s_dict_n_el_16["n_sample"]) != 0:
         # clear directory
         print("clearing: s_dict_n_el_16")
         s_dict_n_el_16 = clear_s_dict(s_dict_n_el_16)
 
-    for ele in tqdm(os.listdir(lpath)):
-        tmp_sample = np.load(lpath + ele, allow_pickle=True)
-        s_dict_n_el_16 = single_measurement_to_csv_n_el_16(
-            tmp_sample, s_dict_n_el_16, r_split=r_split
-        )
+    for ch_mod, ele in tqdm(enumerate(np.sort(os.listdir(lpath)))):
+        if ch_mod % 10 != 0:
+            tmp_sample = np.load(lpath + ele, allow_pickle=True)
+            s_dict_n_el_16 = single_measurement_to_csv_n_el_16(
+                tmp_sample, s_dict_n_el_16, r_split=r_split
+            )
 
     if export_csv is True:
         try:
             os.mkdir(f"{lpath[:-1]}_csv")
             print(f"Created save directory at:\n\t{lpath[:-1]}_csv/")
         except BaseException:
             pass
```

## sciopy/prepare_data.py

```diff
@@ -1,13 +1,14 @@
 import os
 import math
 from tqdm import tqdm
 import numpy as np
 
 from .sciopy_dataclasses import PreperationConfig
+from .meshing import create_empty_2d_mesh, add_circle_anomaly
 
 
 def create_prep_directory(prep_cnf: PreperationConfig) -> str:
     """
     Creates the directory to prepare the environment for data preperation.
 
     Parameters
@@ -119,15 +120,15 @@
     if set_ch_group == ch_group_to_check and set_n_el == n_el_to_check:
         return True
     else:
         print("\tError: Data has not the right number of channels and/or electrodes!")
         return False
 
 
-def extract_electrode_signal_without_excitation_stgs(
+def extract_electrodepotentials(
     potential_matrix: np.ndarray,
     sample: np.lib.npyio.NpzFile,
     del_ex_stgs: bool = True,
 ) -> np.array:
     """
     Extracts the electrode signal without the corresponding excitation stages.
 
@@ -182,42 +183,114 @@
     diff_arr = max(data) - min(data)
     for i in data:
         temp = (((i - min(data)) * diff) / diff_arr) + low_bound
         norm_data.append(temp)
     return np.array(norm_data)
 
 
-def prepare_all_samples_for_16_el(prep_cnf: PreperationConfig) -> None:
+def prepare_all_samples_for_16_el(
+    prep_cnf: PreperationConfig,
+    gen_mesh: bool = True,
+    h0: float = 0.05,
+    obj_perm: float = 10.0,
+    x_y_offset: float = 180,
+    tank_r_inner: float = 97.0,
+) -> None:
     """
     Converts all samples inside one directory that were recorded in 16
     electrode mode and save the potential and positional data to a target directory.
+    Furthermore a mesh is generated.
 
     Parameters
     ----------
     prep_cnf : PreperationConfig
-        _description_
+        configuration dataclass
+    gen_mesh : bool, optional
+        generate a mesh, by default True
+    obj_perm : float, optional
+        permittivity of the circle object, by default 10.0
+    x_y_offset : float, optional
+        Ender 5 x,y-axis offset, by default 180
+    tank_r_inner : float, optional
+        inner tank radius, by default 97.0
     """
 
     check_result = check_n_el_condition(
         prep_cnf, ch_group_to_check=[1], n_el_to_check=16
     )
 
+    if gen_mesh:
+        mesh_empty = create_empty_2d_mesh(h0=h0)
+    sf_numbering = 0
     if check_result:
-        for sample_path in tqdm(np.sort(os.listdir(prep_cnf.lpath))):
-            tmp_sample = np.load(prep_cnf.lpath + sample_path, allow_pickle=True)
-            tmp_p_mat = extract_potentials_from_sample_n_el_16(tmp_sample)
-            v_without_ext = extract_electrode_signal_without_excitation_stgs(
-                tmp_p_mat, tmp_sample, True
-            )
-            np.savez(
-                prep_cnf.spath + sample_path,
-                potential_matrix=tmp_p_mat,
-                v_with_ext=extract_electrode_signal_without_excitation_stgs(
-                    tmp_p_mat, tmp_sample, False
-                ),
-                v_without_ext=v_without_ext,
-                abs_v_norm_without_ext=norm_data(v_without_ext),
-                r_phi=comp_tank_relative_r_phi(tmp_sample),
-                config=tmp_sample["config"].tolist().__dict__,
-            )
+        for ch_mod, sample_path in tqdm(enumerate(np.sort(os.listdir(prep_cnf.lpath)))):
+            if ch_mod % 10 != 0:
+                tmp_sample = np.load(prep_cnf.lpath + sample_path, allow_pickle=True)
+
+                ender_stat = tmp_sample["enderstat"].tolist()
+                cnfg = tmp_sample["config"].tolist()
+                abs_x_pos = (ender_stat["abs_x_pos"] - x_y_offset) / tank_r_inner
+                abs_y_pos = (ender_stat["abs_y_pos"] - x_y_offset) / tank_r_inner
+
+                tmp_p_mat = extract_potentials_from_sample_n_el_16(tmp_sample)
+                p_without_ext = extract_electrodepotentials(tmp_p_mat, tmp_sample, True)
+                p_with_ext = extract_electrodepotentials(tmp_p_mat, tmp_sample, False)
+
+                if gen_mesh:
+                    mesh_obj = add_circle_anomaly(
+                        mesh_empty, abs_x_pos, abs_y_pos, cnfg.size, obj_perm
+                    )
+                    np.savez(
+                        prep_cnf.spath + f"sample_{sf_numbering:06}.npz",
+                        mesh=mesh_obj,
+                        potential_matrix=tmp_p_mat,
+                        p_with_ext=p_with_ext,
+                        p_without_ext=p_without_ext,
+                        abs_p_norm_without_ext=np.abs(norm_data(p_without_ext)),
+                        v_with_ext=compute_v(p_with_ext),
+                        v_without_ext=compute_v(p_without_ext),
+                        abs_v_norm_without_ext=norm_data(compute_v(p_without_ext)),
+                        r_phi=comp_tank_relative_r_phi(tmp_sample),
+                        config=tmp_sample["config"].tolist().__dict__,
+                    )
+                else:
+                    np.savez(
+                        prep_cnf.spath + f"sample_{sf_numbering:06}.npz",
+                        potential_matrix=tmp_p_mat,
+                        p_with_ext=p_with_ext,
+                        p_without_ext=p_without_ext,
+                        abs_p_norm_without_ext=np.abs(norm_data(p_without_ext)),
+                        v_with_ext=compute_v(p_with_ext),
+                        v_without_ext=compute_v(p_without_ext),
+                        abs_v_norm_without_ext=norm_data(compute_v(p_without_ext)),
+                        r_phi=comp_tank_relative_r_phi(tmp_sample),
+                        config=tmp_sample["config"].tolist().__dict__,
+                    )
+                sf_numbering += 1
+            else:
+                pass
+                # Due to errors inside the ScioSpec software taking only burst_count-1 samples
     else:
         print("Could not start converting.")
+
+
+def compute_v(p: np.ndarray) -> np.ndarray:
+    """
+    Computes the voltage out of the potential.
+    Therefore p[0,1,...,16] - p[1,2,...,0] is computed.
+
+    Parameters
+    ----------
+    p : np.ndarray
+        measured potentials
+
+    Returns
+    -------
+    np.ndarray
+        voltage vector
+    """
+    v = []
+    for i in range(len(p) - 1):
+        v.append(p[i] - p[i + 1])
+    v.append(p[len(p) - 1] - p[0])
+
+    return np.array(v)
```

## sciopy/visualization.py

```diff
@@ -13,19 +13,19 @@
 
     Parameters
     ----------
     sample : np.lib.npyio.NpzFile
         prepared sample
     """
     fig, (ax1, ax2, ax3) = plt.subplots(1, 3, figsize=(12, 4))
-    ax1.set_title("$\Re\{P_m\}$")
+    ax1.set_title(r"$\Re\{P_m\}$")
     ax1.imshow(np.real(sample["potential_matrix"]))
-    ax2.set_title("$\Im\{P_m\}$")
+    ax2.set_title(r"$\Im\{P_m\}$")
     ax2.imshow(np.imag(sample["potential_matrix"]))
-    ax3.set_title("$Abs\{P_m\}$")
+    ax3.set_title(r"$|P_m|$")
     ax3.imshow(np.abs(sample["potential_matrix"]))
     fig.tight_layout()
     plt.show()
 
 
 def plot_el_sign(sample: np.lib.npyio.NpzFile, norm: bool = False) -> None:
     """
@@ -39,20 +39,20 @@
         normalization between 0 and 1, by default False
     """
 
     n_el = sample["config"].tolist()["n_el"]
     steps = len(sample["v_without_ext"]) / n_el
 
     fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=(9, 9))
-    ax1.set_title("Real signal part without excitation electrodes")
-    ax1.set_ylabel("$\Re\{\phi\}$")
-    ax2.set_title("Imaginary signal part without excitation electrodes")
-    ax2.set_ylabel("$\Im\{\phi\}$")
-    ax3.set_title("Absolute signal without excitation electrodes")
-    ax3.set_ylabel("$|\phi|$")
+    ax1.set_title(r"Real signal part without excitation electrodes")
+    ax1.set_ylabel(r"$\Re\{\phi\}$")
+    ax2.set_title(r"Imaginary signal part without excitation electrodes")
+    ax2.set_ylabel(r"$\Im\{\phi\}$")
+    ax3.set_title(r"Absolute signal without excitation electrodes")
+    ax3.set_ylabel(r"$|\phi|$")
     if norm is False:
         real = np.real(sample["v_without_ext"])
         imag = np.imag(sample["v_without_ext"])
         absol = np.abs(sample["v_without_ext"])
         ax1.stem(real)
         ax2.stem(imag)
         ax3.stem(absol)
@@ -220,15 +220,16 @@
     plt.figure(figsize=(8, 4))
     # enable with new data
     plt.title(f"{lpath.split('/')[-2:-1][0]}, {dt_string[2:-2]}")
     plt.grid()
     plt.plot(temperature)
     plt.ylabel("temperature °C")
     plt.xticks(
-        ticks=np.arange(len(time))[:: len(time) // 8], labels=time[:: len(time) // 8]
+        ticks=np.arange(len(time))[:: len(time) // 8],
+        labels=time[:: len(time) // 8],
     )
     plt.xlabel("time HH:MM")
     plt.show()
 
     print(f"mean temperature:\t {mean_t}")
     print(f"standart deviation:\t {std_dev}")
     print(f"max(t)-min(t):\t {max_min_diff}")
```

## Comparing `sciopy-0.6.2.dist-info/LICENSE` & `sciopy-0.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sciopy-0.6.2.dist-info/METADATA` & `sciopy-0.6.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciopy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python based interface module for serial communication with the ScioSpec Electrical Impedance Tomography (EIT) device.
 Home-page: https://github.com/spatialaudio/sciopy.git
 Author: Jacob Peter Thönes
 Author-email: jacob.thoenes@uni-rostock.de
 License: UNKNOWN
 Keywords: ScioSpec,EIT
 Platform: any
@@ -44,16 +44,8 @@
 - Parsing measurements of 32 electrodes.
 - Adjacent and opposite drive patterns for 32 electrodes.
 
 ## Contact
 
 Email: jacob.thoenes@uni-rostock.de
 
-```bibtex
-@Unpublished{Thoenes2023,
-  author = {Jacob Peter Thönes},
-  title  = {Python based interface module for serial communication with the ScioSpec Electrical Impedance Tomography (EIT) device.},
-  year   = {2023},
-}
-```
-
```

## Comparing `sciopy-0.6.2.dist-info/RECORD` & `sciopy-0.6.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-sciopy/__init__.py,sha256=35c05EPvsXyDS-1ZvqQdHcf-V119Ohm5k8ypz7i3NJA,3863
+sciopy/__init__.py,sha256=s5LWVeFDad4ulmdkvvWmH5sgZ0HOHTdTrOW6ghK09-g,4427
 sciopy/com_handling.py,sha256=U1ZMOKKRw65eWq1Jvrl6EnH7ogiurPkCJ4p1q96-8q4,2314
 sciopy/configurations.py,sha256=4_h6rS0_oQaCD-IMpWl-ngHwLMkvJCHLRNKzjmwg_eo,39449
 sciopy/doteit.py,sha256=WJjIWgYG_3abW848ccHxru3sHiBu9iRf98zWe2bSSxA,4417
-sciopy/npztocsv.py,sha256=FLzEcUe77qtLivO3-S5oOt11O62ZCqGvW7a0lQIeA3o,8849
-sciopy/prepare_data.py,sha256=wwD606Z_52jf9bhxam7H4mlkvzVM_mQINqgnngKim30,6598
+sciopy/meshing.py,sha256=jgBi9JUcOjTBn4gWgSpLsiPX3KiNqA0G4ZmJ6w1qGGs,4685
+sciopy/npztocsv.py,sha256=GcI-uffphOWBBOyhhAXrPClEATlTqt2R2TDujnCVSKU,8922
+sciopy/prepare_data.py,sha256=LL-3W2kM2ud6C_tZunZ1GtFxQZvhRCzHPrZYeehDO20,9375
 sciopy/print_command_info.py,sha256=rBnZJ1Tl_-QRCQnfqfet-znl8XnN7wvXTV4Z4krbFGQ,4372
 sciopy/sciopy_dataclasses.py,sha256=Hi2X8q2RXyAiuTatI4z_2BHyKnIKYlR8trnjyo9FrGI,3484
 sciopy/setup_m.py,sha256=t6EG_JEgMdwU5KFZdz9-gbJ4qRyYBevnloRiHV5y1_E,20412
-sciopy/visualization.py,sha256=hpfPyE_EVuApq8tY2GiftHI40GIedAOugFtp3t7_pNA,7469
-sciopy-0.6.2.dist-info/LICENSE,sha256=mvuu3JpofjFcd8rEvSAGR4EedNMH979iMwXp9BGi38Y,1062
-sciopy-0.6.2.dist-info/METADATA,sha256=hnicib-QCNWs_gMJyPh_NzsZ9e1NaFCkCp9Vjrwz6vc,2625
-sciopy-0.6.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sciopy-0.6.2.dist-info/top_level.txt,sha256=Yfokv5CD23A5gda5ZEjDy0YfFwrFeo_EOXJLRv-QoEU,7
-sciopy-0.6.2.dist-info/RECORD,,
+sciopy/visualization.py,sha256=AW_cYLVrPvwArKLDeoxEDnTveZhF6HSBMdU9pqtGa2g,7482
+sciopy-0.6.3.dist-info/LICENSE,sha256=mvuu3JpofjFcd8rEvSAGR4EedNMH979iMwXp9BGi38Y,1062
+sciopy-0.6.3.dist-info/METADATA,sha256=WV9UNu9csuNMSv3GqOrX_WAtkMwnu9vADZxlaoJ8QOk,2396
+sciopy-0.6.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sciopy-0.6.3.dist-info/top_level.txt,sha256=Yfokv5CD23A5gda5ZEjDy0YfFwrFeo_EOXJLRv-QoEU,7
+sciopy-0.6.3.dist-info/RECORD,,
```

