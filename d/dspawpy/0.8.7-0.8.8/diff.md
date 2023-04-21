# Comparing `tmp/dspawpy-0.8.7-py3-none-any.whl.zip` & `tmp/dspawpy-0.8.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 67612 bytes, number of entries: 20
+Zip file size: 69387 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/__init__.py
--rw-rw-rw-  2.0 fat    27378 b- defN 23-Apr-06 03:08 dspawpy/plot.py
+-rw-rw-rw-  2.0 fat    29176 b- defN 23-Apr-20 08:41 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    47545 b- defN 23-Apr-13 03:15 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    47547 b- defN 23-Apr-13 06:12 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
 -rw-rw-rw-  2.0 fat     9607 b- defN 23-Apr-13 05:59 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    48170 b- defN 23-Apr-11 08:22 dspawpy/diffusion/nebtools.py
+-rw-rw-rw-  2.0 fat    52973 b- defN 23-Apr-21 04:37 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-13 05:52 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    21646 b- defN 23-Apr-04 06:32 dspawpy/io/read.py
+-rw-rw-rw-  2.0 fat    21646 b- defN 23-Apr-19 06:23 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7910 b- defN 23-Apr-04 06:32 dspawpy/io/read_json.py
 -rw-rw-rw-  2.0 fat    10331 b- defN 23-Apr-04 06:32 dspawpy/io/structure.py
 -rw-rw-rw-  2.0 fat    29355 b- defN 23-Apr-13 03:18 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    11049 b- defN 23-Apr-04 09:19 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat    11045 b- defN 23-Apr-17 08:05 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1794 b- defN 23-Apr-04 06:32 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat      754 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1581 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/RECORD
-20 files, 248365 bytes uncompressed, 65062 bytes compressed:  73.8%
+-rw-rw-rw-  2.0 fat     1462 b- defN 23-Apr-21 06:37 dspawpy-0.8.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 06:37 dspawpy-0.8.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-21 06:37 dspawpy-0.8.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1582 b- defN 23-Apr-21 06:37 dspawpy-0.8.8.dist-info/RECORD
+20 files, 255673 bytes uncompressed, 66837 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.8.7.dist-info/METADATA
+Filename: dspawpy-0.8.8.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.8.7.dist-info/WHEEL
+Filename: dspawpy-0.8.8.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.8.7.dist-info/top_level.txt
+Filename: dspawpy-0.8.8.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.8.7.dist-info/RECORD
+Filename: dspawpy-0.8.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/plot.py

```diff
@@ -147,16 +147,16 @@
 ):
     """AIMD任务完成后，绘制关键物理量的收敛过程图
 
     aimd.h5 -> aimd.png
 
     Parameters
     ----------
-    datafile : str
-        h5文件位置. 默认 'aimd.h5'
+    datafile : str or list
+        h5文件位置. 例如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
     show : bool
         是否展示交互界面. 默认 False
     figName : str
         保存的图片路径. 默认 'aimd.h5'
     flags_str : str
         子图编号.
         1. 动能
@@ -637,15 +637,23 @@
            [-2.86362371e-05, -1.72479598e+01, -3.61790588e-05],
            [-5.52844691e-05, -6.03482453e+00, -2.71118952e-05],
            [-3.63338519e-05, -1.92737729e+01, -6.94462350e-06],
            [ 9.30116520e-06, -5.74668477e+00,  2.91334059e-05],
            [-4.53814037e-05,  8.71545041e+00,  1.18885825e-06]])
     """
 
-    subfolders = next(os.walk(directory))[1]
+    raw_subfolders = next(os.walk(directory))[1]
+    subfolders = []
+    for subfolder in raw_subfolders:
+        try:
+            assert 0 <= int(subfolder) < 100
+            subfolders.append(subfolder)
+        except:
+            pass
+    subfolders.sort()  # 从小到大排序
     if os.path.exists(f"{subfolders[0]}/polarization.json"):
         # quantum number if constant across the whole calculation,
         # so, read only once
         with open(f"{subfolders[0]}/polarization.json", "r") as f:
             quantum = json.load(f)["PolarizationInfo"]["Quantum"]
         # the Total number is not constant
         totals = np.empty(shape=(len(subfolders), 3))
@@ -714,47 +722,76 @@
 
 
 def _read_aimd_converge_data(datafile: str, index: str = None):
     """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
 
     Parameters
     ----------
-    datafile : str
-        hdf5文件路径
+    datafile : str or list
+        hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
     index : str
         编号, 默认 None
 
     Returns
     -------
     xs : np.ndarray
         x轴数据
     ys : np.ndarray
         y轴数据
     """
-    hf = h5py.File(datafile)  # 加载h5文件
-    Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
-    ys = np.empty(Nstep)  # 准备一个空数组
-
-    # 开始读取
-    if index == "5":
-        for i in range(1, Nstep + 1):
-            ys[i - 1] = np.linalg.det(hf.get("/Structures/Step-%d/Lattice" % i))
-    else:
-        map = {
-            "1": "IonsKineticEnergy",
-            "2": "TotalEnergy0",
-            "3": "PressureKinetic",
-            "4": "Temperature",
-        }
-        for i in range(1, Nstep + 1):
-            # 如果计算中断，则没有PressureKinetic这个键
-            try:
-                ys[i - 1] = np.array(hf.get("/AimdInfo/Step-%d/%s" % (i, map[index])))
-            except:
-                ys[i - 1] = 0
-                ys = np.delete(ys, -1)
-                print(f"-> 计算中断于第{Nstep}步，未读取到该步的压力数据！")
+    if isinstance(datafile, list):
+        xs = []
+        ys = []
+        for i, df in enumerate(datafile):
+            # concentrate returned np.ndarray
+            x, y = _read_aimd_converge_data(df, index)
+            xs.extend(x)
+            ys.extend(y)
+        xs = np.linspace(1, len(xs), len(xs))
+        return xs, ys
+        
+    # search datafile in the given directory
+    elif isinstance(datafile, str):
+        if os.path.isdir(datafile): # 如果是文件夹
+            directory = datafile  # specified datafile is actually a directory
+            print(f"您指定了一个文件夹，正在{directory}中自动查找aimd.h5...")
+            if os.path.exists(os.path.join(directory, "aimd.h5")):
+                datafile = os.path.join(directory, "aimd.h5")
+                print("Reading aimd.h5...")
+            else:
+                raise FileNotFoundError("未找到aimd.h5文件！")
+            
+        elif datafile.endswith(".h5"): # 如果是h5文件
+            hf = h5py.File(datafile)  # 加载h5文件
+            print(f' reading {os.path.abspath(datafile)}...')
+            Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
+            ys = np.empty(Nstep)  # 准备一个空数组
+            # 开始读取
+            if index == "5":
+                for i in range(1, Nstep + 1):
+                    ys[i - 1] = np.linalg.det(hf.get("/Structures/Step-%d/Lattice" % i))
+            else:
+                map = {
+                    "1": "IonsKineticEnergy",
+                    "2": "TotalEnergy0",
+                    "3": "PressureKinetic",
+                    "4": "Temperature",
+                }
+                for i in range(1, Nstep + 1):
+                    # 如果计算中断，则没有PressureKinetic这个键
+                    try:
+                        ys[i - 1] = np.array(hf.get("/AimdInfo/Step-%d/%s" % (i, map[index])))
+                    except:
+                        ys[i - 1] = 0
+                        ys = np.delete(ys, -1)
+                        print(f"-> 计算中断于第 {Nstep} 步，未读取到第 {i} 步的 {map[index]} 数据！")
+                        break
+
+            Nstep = len(ys)  # 步数更新为实际完成的步数
 
-    Nstep = len(ys)  # 步数更新为实际完成的步数
+            # 返回xs，ys两个数组
+            return np.linspace(1, Nstep, Nstep), np.array(ys)
 
-    # 返回xs，ys两个数组
-    return np.linspace(1, Nstep, Nstep), np.array(ys)
+        else:
+            raise TypeError("仅支持读取h5文件！")
+    else:
+        raise TypeError("datafile必须是字符串或列表！")
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -1024,15 +1024,15 @@
         元素，例如 'C'，'H'，'O'，'N'
     index : int
         优化过程中的第几步
 
     Returns
     -------
     dumpfile: str
-        写入xyz格式的轨迹文件，默认为aimdTraj.xyz
+        写入dump格式的轨迹文件，默认为aimdTraj.dump
 
     Example
     -------
     >>> from dspawpy.analysis.aimdtools import write_dump_traj
     >>> write_dump_traj(datafile='aimd.h5', ai=[1,2,3], index=1, dumpfile='aimdTraj.dump')
     """
     if isinstance(datafile, list):
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -1,15 +1,15 @@
 import os
 import h5py
 import json
 import pandas as pd
 import numpy as np
 
 np.set_printoptions(suppress=True)  # 不使用科学计数法
-from dspawpy.io.utils import get_pos_ele_lat, get_ele_from_h5
+from dspawpy.io.utils import get_pos_ele_lat, get_ele_from_h5, get_spo_ele_lat
 import matplotlib.pyplot as plt
 
 
 def get_distance(
     spo1: np.ndarray, spo2: np.ndarray, lat1: np.ndarray, lat2: np.ndarray
 ):
     """根据两个结构的分数坐标和晶胞计算距离
@@ -238,15 +238,14 @@
     if raw:
         pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv", index=False)
         pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
             "raw_interpolated_xy.csv", index=False
         )
         
     # plot
-    plt.clf()
     if kwargs:
         plt.plot(xnew, ynew, label=method + str(kwargs))
     else:
         plt.plot(xnew, ynew, label=method)
     plt.scatter(rcs, dEs, c="r")
     plt.xlabel("Reaction Coordinate (Å)")
     plt.ylabel("Energy (eV)")
@@ -390,15 +389,15 @@
     """
     subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
     # printout summary
     print("构型\t受力(eV/Å)\t反应坐标(Å)\t此构型的能量(eV)\t与初始构型的能量差(eV)")
     for i in range(len(subfolders)):  # 注意格式化输出，对齐
         print(
             "%s\t%8.4f\t%8.4f\t%12.4f\t%20.4f"
-            % (subfolders[i], resort_mfs[i], rcs[i], ens[i][0], dEs[i])
+            % (subfolders[i], resort_mfs[i], rcs[i], ens[i], dEs[i])
         )
 
 
 def restart(directory: str, inputin: str, output: str):
     """将旧NEB任务归档压缩，并在原路径下准备续算
 
     Parameters
@@ -543,14 +542,15 @@
     """
     # 1. 绘制能垒图
     print("--> 1. 打印NEB计算时各构型的能量和受力...")
     printef(directory)
 
     # 2. 打印各构型受力、反应坐标、能量、与初始构型的能量差
     print("\n--> 2. 绘制能垒图...")
+    plt.clf() # 清空画布再画图
     plot_barrier(directory=directory, raw=raw, **kwargs)
 
     # 3. 绘制并保存结构优化过程的能量和受力收敛过程图到各构型文件夹中
     print("\n--> 3. 绘制收敛过程图到各构型文件夹中...")
     subfolders = get_neb_subfolders(directory)
     for subfolder in subfolders[1 : len(subfolders) - 1]:
         print(f"----> {subfolder}/converge.png...")
@@ -571,15 +571,17 @@
     Parameters
     ----------
     preview : bool
         是否预览模式，默认否
     directory : str
         计算结果所在目录. 默认当前路径
     step: int
-        离子步编号. 默认-1，读取整个NEB计算过程信息
+        离子步编号. 默认-1，读取整个NEB计算过程信息。
+        0表示初插结构（未完成离子步）；
+        1表示第一个离子步，以此类推。
 
     Returns
     ----------
     neb_movie*.json文件
 
     Examples
     ----------
@@ -596,36 +598,141 @@
 
     if preview:  # preview mode, write neb_movie_init.json from structure.as
         print("正在根据初插结构保存neb_movie_init.json...")
         try:
             raw = _from_structures(directory)
         except FileNotFoundError:
             print("未找到初始插值结构！")
-        except:
-            print("初始插值结构读取失败！请检查structure*.as文件内容！")
+        except Exception as e:
+            print("初始插值结构读取失败！", e)
     else:
         if step == 0:  # try preview mode to save time
             try:
                 raw = _from_structures(directory)
-            except:
+            except FileNotFoundError:
                 print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
+            except Exception as e:
+                print("初始插值结构读取失败！", e)
         else:
             try:  # read from h5 file
                 raw = _from_h5(directory, step)
             except FileNotFoundError:
                 try:  # read from json file
                     raw = _from_json(directory, step)
-                except FileNotFoundError:
-                    print("h5和json文件都不存在！")
                 except json.decoder.JSONDecodeError:
                     print("json文件格式错误！")
-            except:
-                print("h5文件内容读取失败！")
+                except Exception as e:
+                    print(e)
+            except Exception as e:
+                print("h5文件内容读取失败！", e)
     _dump_neb_movie_json(raw)
 
+def write_xyz(preview:bool=False, directory:str='.', step:int=-1):
+    """
+    将NEB结构链条写成xyz轨迹文件用于可视化
+
+    Parameters
+    ----------
+    preview : bool
+        是否预览模式，默认否
+    directory : str
+        计算结果所在目录. 默认当前路径
+    step: int
+        离子步编号. 默认-1，读取整个NEB计算过程信息。
+        0表示初插结构（未完成离子步）；
+        1表示第一个离子步，以此类推。
+
+    Returns
+    ----------
+    neb_movie.xyz文件
+
+    Examples
+    ----------
+    """
+
+    if preview:  # preview mode, write neb_movie_init.xyz from structure.as
+        print("正在根据初插结构保存neb_movie_init.xyz...")
+        try:
+            raw = _from_structures(directory)
+        except FileNotFoundError:
+            print("未找到初始插值结构！")
+        except Exception as e:
+            print("初始插值结构读取失败！", e)
+    else:
+        if step == 0:  # try preview mode to save time
+            try:
+                raw = _from_structures(directory)
+            except FileNotFoundError:
+                print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
+            except Exception as e:
+                print("初始插值结构读取失败！", e)
+        else:
+            try:  # read from h5 file
+                raw = _from_h5(directory, step)
+            except FileNotFoundError:
+                try:  # read from json file
+                    raw = _from_json(directory, step)
+                except json.decoder.JSONDecodeError:
+                    print("json文件格式错误！")
+                except Exception as e:
+                    print(e)
+            except Exception as e:
+                print("h5文件内容读取失败！", e)
+    _dump_neb_xyz(raw)
+
+def _dump_neb_xyz(raw):
+    """根据之前收集到的各数据列表，dump json文件到output"""
+    (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,
+        Poses, # Nimage x Natom x 3 , read
+        Latvs, # Nimage x 9
+        Elems, # Nimage x Natom
+        Fixs, # Natom x 3
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects
+    ) = raw
+
+    # 写入文件
+    xyzfile = output[:-5] + '.xyz'
+    Nstep = len(subfolders) # 选定离子步，展示构型链
+    with open(xyzfile, "w") as f:
+        # Nstep
+        for n in range(Nstep):
+            eles = Elems[n] # 针对每个构型
+            # 原子数不会变，就是不合并的元素总数
+            f.write("%d\n" % len(eles))
+            # lattice
+            f.write(
+                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
+                % (
+                    Latvs[n, 0],
+                    Latvs[n, 1],
+                    Latvs[n, 2],
+                    Latvs[n, 3],
+                    Latvs[n, 4],
+                    Latvs[n, 5],
+                    Latvs[n, 6],
+                    Latvs[n, 7],
+                    Latvs[n, 8],
+                )
+            )
+            # position and element
+            for i in range(len(eles)):
+                f.write(
+                    "%s %f %f %f\n"
+                    % (eles[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
+                )
+    print(f"--> {os.path.abspath(xyzfile)} 写入成功！\n")
 
 def _from_structures(directory: str):
     """从structure00.as，structure01.as，...，中读取结构信息，
     写入neb_movie_init，以便用DeviceStudio打开观察
 
     Parameters
     ----------
@@ -696,133 +803,147 @@
         tangents,
         iDirects
     )
 
 
 def _from_h5(directory: str, step: int):
     """从NEB路径下的h5文件读取指定step数的结构和能量信息，
-    写入json文件，以便用DeviceStudio打开观察
+    写入json文件，以便用DeviceStudio打开观察。
+
+    支持热读取结构信息（其他信息忽略）
 
     Parameters
     ----------
     directory : str
         NEB路径，默认当前路径
     step : int
         step数，默认-1，读取最后一个构型
 
     Returns
     -------
     用于json文件的各个数组
     """
     # ^ 前期设置
-    neb_h5 = os.path.join(directory, "01/neb01.h5")
+    neb_h5 = os.path.join(directory, '01', 'neb01.h5')
+    ele = get_ele_from_h5(hpath=neb_h5)
+    Natom = len(ele)
     data = h5py.File(neb_h5)
-    total_steps = np.array(data.get("/NebSize"))[0]
+    try:
+        total_steps = np.array(data.get("/NebSize"))[0]
+    except:
+        print("NEB计算未正常结束，正在尝试实时读取结构信息...")
+        try:
+            total_steps = np.array(data.get("/Structures/FinalStep"))[0]
+        except:
+            raise ValueError("尚未完成第一个离子步，请检查计算是否出错，否则请耐心等待离子步完成至少一个后再尝试读取！")
 
     if step == -1:
         output = "neb_movie_last.json"
-        step = total_steps - 1
-        print("正在根据最后一个离子步信息生成neb_movie_last.json...")
-    elif step > total_steps - 1:
+        step = total_steps
+        print("正在读取最后一个离子步信息...")
+    elif step > total_steps:
         output = "neb_movie_last.json"
-        step = total_steps - 1
-        print(f"您指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
-        print("正在根据最后一个离子步信息生成neb_movie_last.json...")
+        step = total_steps
+        print(f"指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
+        print("正在读取最后一个离子步信息...")
     else:
         output = "neb_movie_{}.json".format(step)
-        print(f"正在根据第{step}个离子步信息生成{output}...")
+        print(f"正在读取第{step}个离子步信息...")
 
     # ^ 读取前，准备好json文件所需数组框架
     subfolders = get_neb_subfolders(directory)
     nimage = len(subfolders)
     reactionCoordinates = np.zeros(shape=nimage)  # optional
     totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
     maxForces = np.zeros(shape=nimage - 2)  # optional
     tangents = np.zeros(shape=nimage - 2)  # optional
-    MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
-    TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional，中间构型每个离子步能量
-    Sposes = []  # nimage x Natom x 3 , read
+    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
+    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
+    # Sposes = []  # nimage x Natom x 3 , read
+    Sposes = np.empty(shape=(nimage, Natom, 3))  # nimage x Natom x 3 , read
     Elems = []  # nimage x Natom, read
     Latvs = []  # nimage x 9, read
     Fixs = []  # Natom x 3, set
 
     for folder in subfolders:
         """如果是首尾两个构型，最多只有scf.h5文件，没有neb.h5文件
         用户如果算NEB的时候，不计算首尾构型的自洽，
          或者在别处算完了但是没有复制到首尾文件夹中并命名为scf.h5，
           便不能使用第一个功能
         """
         if folder == subfolders[0] or folder == subfolders[-1]:
             h5_path = os.path.join(directory, folder, "scf.h5")
+            spath = os.path.join(directory, folder, f'structure{folder}.as')
+            assert os.path.exists(h5_path) or os.path.exists(spath), f"请确认{h5_path}或{spath}至少存在一个！"
         else:
             h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
-        assert os.path.exists(h5_path), f"请确认{h5_path}是否存在！"
+            assert os.path.exists(h5_path), f"请确认{h5_path}是否存在！"
 
     # ^ 开始分功能读取数据
     for i, folder in enumerate(subfolders):
         if folder == subfolders[0] or folder == subfolders[-1]:
             h5_path = os.path.join(directory, folder, "scf.h5")
-            data = h5py.File(h5_path)
-            # 不影响可视化，直接定为0
-            if folder == subfolders[0]:
-                reactionCoordinates[i] = 0
-            pos = np.array(data.get("/Structures/Step-1/Position"))  # scaled
-            lat = np.array(data.get("/Structures/Step-1/Lattice"))
-
+            if os.path.exists(h5_path):
+                data = h5py.File(h5_path)
+                # 不影响可视化，直接定为0
+                if folder == subfolders[0]:
+                    reactionCoordinates[i] = 0
+                pos = np.array(data.get("/Structures/Step-1/Position")).reshape(-1,3)  # scaled
+                lat = np.array(data.get("/Structures/Step-1/Lattice"))
+                ele = get_ele_from_h5(hpath=h5_path)
+                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
+            else:
+                pos, ele, lat = get_spo_ele_lat(spath)
         else:
             h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
             data = h5py.File(h5_path)
             # reading...
-            reactionCoordinates[i - 1] = np.array(data.get("/Distance/Previous"))[-1]
-            maxForces[i - 1] = np.array(data.get("/MaxForce"))[-1]
-            tangents[i - 1] = np.array(data.get("/Tangent"))[-1]
-            if folder == subfolders[-2]:
-                reactionCoordinates[i + 1] = np.array(data.get("/Distance/Next"))[-1]
-            # read MaxForces and TotalEnergies
-            nionStep = np.array(data.get("/MaxForce")).shape[0]
-            assert step <= nionStep, f"总共只完成了{nionStep}个离子步!"
-            for j in range(step + 1):
-                MaxForces[i - 1, j] = np.array(data.get("/MaxForce"))[j]
-                TotalEnergies[i - 1, j] = np.array(data.get("/TotalEnergy"))[j]
-
+            try:
+                reactionCoordinates[i - 1] = np.array(data.get("/Distance/Previous"))[-1]
+                maxForces[i - 1] = np.array(data.get("/MaxForce"))[-1]
+                tangents[i - 1] = np.array(data.get("/Tangent"))[-1]
+                if folder == subfolders[-2]:
+                    reactionCoordinates[i + 1] = np.array(data.get("/Distance/Next"))[-1]
+                # read MaxForces and TotalEnergies
+                nionStep = np.array(data.get("/MaxForce")).shape[0]
+                assert step <= nionStep, f"总共只完成了{nionStep}个离子步!"
+                for j in range(step):
+                    MaxForces[i - 1, j] = np.array(data.get("/MaxForce"))[j]
+                    TotalEnergies[i - 1, j] = np.array(data.get("/TotalEnergy"))[j]
+                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
+            except:
+                pass # 还没完成NEB计算，不影响读取结构信息用于可视化
             # read the latest structure for visualization
-            pos = np.array(data.get(f"/Structures/Step-{step+1}/Position"))  # scaled
-            lat = np.array(data.get(f"/Structures/Step-{step+1}/Lattice"))
-
-        totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
-
-        elems = get_ele_from_h5(hpath=h5_path)
-        Elems.append(elems)
+            pos = np.array(data.get(f"/Structures/Step-{step}/Position")).reshape(Natom,3)  # scaled
+            lat = np.array(data.get(f"/Structures/Step-{step}/Lattice"))
+            ele = get_ele_from_h5(hpath=h5_path)
 
-        Sposes.append(pos)
+        Elems.append(ele)
+        Sposes[i,:,:] = pos
         Latvs.append(lat)
 
-    Natom = len(Elems[0])
-    tdata = h5py.File(os.path.join(directory, "neb.h5"))
-    # atom fix, not lattice
-    # ignore this trivial message because it is not necessary for the visualization
-    if "/UnrelaxStructure/Image00/Fix" in tdata:
-        fix_array = np.array(tdata.get("/UnrelaxStructure/Image00/Fix"))
-        for fix in fix_array:
-            if fix == 0.0:
-                F = False
-            elif fix == 1.0:
-                F = True
-            else:
-                raise ValueError("Fix值只能为0或1")
-            Fixs.append(F)
+    if os.path.exists(os.path.join(directory, "neb.h5")):
+        tdata = h5py.File(os.path.join(directory, "neb.h5"))
+        # atom fix, not lattice
+        # ignore this trivial message because it is not necessary for the visualization
+        if "/UnrelaxStructure/Image00/Fix" in tdata:
+            fix_array = np.array(tdata.get("/UnrelaxStructure/Image00/Fix"))
+            for fix in fix_array:
+                if fix == 0.0:
+                    F = False
+                elif fix == 1.0:
+                    F = True
+                else:
+                    raise ValueError("Fix值只能为0或1")
+                Fixs.append(F)
+        else:
+            Fixs = np.full(shape=(Natom, 3), fill_value=False)
     else:
         Fixs = np.full(shape=(Natom, 3), fill_value=False)
 
-    # 累加reactionCoordinates中的元素
-    for i in range(1, len(reactionCoordinates)):
-        reactionCoordinates[i] += reactionCoordinates[i - 1]
-
-    # reshape data
-    Sposes = np.array(Sposes).reshape((nimage, Natom, 3))
     Elems = np.array(Elems).reshape((nimage, Natom))
     Latvs = np.array(Latvs).reshape((nimage, 9))
     Fixs = np.array(Fixs).reshape((Natom, 3))
     iDirects = [True for i in range(Natom)] # only output direct coordinates
 
     return (
         output,
@@ -862,34 +983,34 @@
     neb_js = os.path.join(directory, "01/neb01.json")
     with open(neb_js, "r") as f:
         data = json.load(f)
     total_steps = len(data)
 
     if step == -1:
         output = "neb_movie_last.json"
-        step = total_steps - 1
-        print("正在根据最后一个离子步信息生成neb_movie_last.json（h5文件不存在，尝试从json文件读取数据）")
-    elif step > total_steps - 1:
+        step = total_steps
+        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
+    elif step > total_steps:
         output = "neb_movie_last.json"
-        step = total_steps - 1
+        step = total_steps
         print(f"您指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
-        print("正在根据最后一个离子步信息生成neb_movie_last.json（h5文件不存在，尝试从json文件读取数据）")
+        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
     else:
         output = f"neb_movie_{step}.json"
-        print(f"正在根据第{step}个离子步信息生成{output}...")
+        print(f"正在读取第{step}个离子步信息...")
 
     # ^ 读取前，准备好json文件所需数组框架
     subfolders = get_neb_subfolders(directory)
     nimage = len(subfolders)
     reactionCoordinates = np.zeros(shape=nimage)  # optional
     totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
     maxForces = np.zeros(shape=nimage - 2)  # optional
     tangents = np.zeros(shape=nimage - 2)  # optional
-    MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
-    TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional，中间构型每个离子步能量
+    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
+    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
     Sposes = []  # nimage x Natom x 3 , read
     Elems = []  # nimage x Natom, read
     Latvs = []  # nimage x 9, read
     Fixs = []  # Natom x 3, set
 
     for folder in subfolders:
         """如果是首尾两个构型，最多只有system.json文件，没有neb*.json文件
@@ -1071,15 +1192,15 @@
 
     IterDict = {}
     for s, sf in enumerate(subfolders):
         if sf == subfolders[0] or sf == subfolders[-1]:
             continue
         else:
             Eflist = []
-            for l in range(step + 1):
+            for l in range(step):
                 ef = {
                     "MaxForce": MaxForces[s - 1, l],
                     "TotalEnergy": TotalEnergies[s - 1, l],
                 }
                 Eflist.append(ef)
                 iterDict = {sf: Eflist}  # construct sub-dict
                 IterDict.update(iterDict)  # append sub-dict
```

## dspawpy/io/write.py

```diff
@@ -119,15 +119,15 @@
         with open(AB, "r") as f1:
             dataAB = json.load(f1)
             rhoAB = np.array(dataAB["Rho"]["TotalCharge"])
             nGrids = dataAB["AtomInfo"]["Grid"]
         for i in range(len(dataAB["AtomInfo"]["Atoms"])):
             atom_symbol.append(dataAB["AtomInfo"]["Atoms"][i]["Element"])
             atom_pos.append(dataAB["AtomInfo"]["Atoms"][i]["Position"])
-            atom_pos = np.array(atom_pos)
+        atom_pos = np.array(atom_pos)
 
         latticeConstantMatrix = dataAB["AtomInfo"]["Lattice"]
     else:
         raise ValueError(f"file format must be either h5 or json: {AB}")
 
     print(f'读取{A}...')
     if A.endswith(".h5"):
```

