# Comparing `tmp/paitest-0.0.12-py3-none-any.whl.zip` & `tmp/paitest-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24739 bytes, number of entries: 13
+Zip file size: 24727 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       40 b- defN 80-Jan-01 00:00 paitest/__init__.py
 -rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
 -rw-r--r--  2.0 unx     2581 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
 -rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
 -rw-r--r--  2.0 unx    14188 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
 -rw-r--r--  2.0 unx     4706 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 paitest/log.py
--rw-r--r--  2.0 unx    18563 b- defN 80-Jan-01 00:00 paitest/paitest.py
+-rw-r--r--  2.0 unx    18540 b- defN 80-Jan-01 00:00 paitest/paitest.py
 -rw-r--r--  2.0 unx     1692 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/LICENSE
--rw-r--r--  2.0 unx     3451 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-0.0.12.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1005 b- defN 16-Jan-01 00:00 paitest-0.0.12.dist-info/RECORD
-13 files, 82139 bytes uncompressed, 23085 bytes compressed:  71.9%
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3437 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.0.0.dist-info/RECORD
+13 files, 82098 bytes uncompressed, 23081 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: paitest/paitest.py
 Comment: 
 
 Filename: paitest/paitest.pyi
 Comment: 
 
-Filename: paitest-0.0.12.dist-info/LICENSE
+Filename: paitest-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: paitest-0.0.12.dist-info/METADATA
+Filename: paitest-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: paitest-0.0.12.dist-info/WHEEL
+Filename: paitest-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: paitest-0.0.12.dist-info/RECORD
+Filename: paitest-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paitest/paitest.py

```diff
@@ -111,15 +111,15 @@
                         % (j + 1, testout_frame, i + 1, N)
                     )
 
             testin_frame = FrameGen.GenTest2InFrame(
                 self._fixed_chip_coord, core_coord, self._fixed_core_star_coord
             )
             ti_list.append(testin_frame)
-            
+
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
         if isinstance(work_dir, Path):
@@ -415,15 +415,15 @@
     def _GetNParams(
         self,
         N: int,
         core_coords: Union[List[Coord], Coord],
         is_legal: bool = False,
     ) -> List[Tuple[int, ...]]:
         """
-        Generate 'N' parameters reg for parameter register.
+        Generate 'N' random parameters register.
         - `is_legal`: whether to generate legal parameters for every core
         """
 
         def _ParamGenerator():
             test_chip_coord: Coord = self._direction.value + self._fixed_chip_coord
 
             while True:
```

## Comparing `paitest-0.0.12.dist-info/LICENSE` & `paitest-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paitest-0.0.12.dist-info/METADATA` & `paitest-1.0.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paitest
-Version: 0.0.12
+Version: 1.0.0
 Summary: Test module for PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAITest
 License: AGPL v3.0
 Keywords: PAICookers,PAITest,PAICORE
 Author: KafCoppelia
 Author-email: k740677208@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -24,15 +24,15 @@
 
 # PAITest
 
 </div>
 
 ## 📦 版本
 
-[v0.0.12 Prerelease](https://github.com/PAICookers/PAITest/releases/tag/v0.0.12)
+[v1.0.0](https://github.com/PAICookers/PAITest/releases/tag/v1.0.0)
 
 ## 🛠️ 使用生成
 
 配置帧及对应测试输入帧，以实现硬件通路的简单测试，后续将芯片实际测试输出帧与预期结果进行对比即可。
 
 ⚠️ 由于配置帧/测试帧I型需要配合串口配置使用，因此目前仅采用**配置/测试帧II型**方案，且 `CHIP_ADDR` 与 `CORE*_ADDR` 均固定为 `(0, 0)`。
 
@@ -83,11 +83,11 @@
    ```python
    # Save into ./test/config.bin
    PAITestManager.SaveFrames("./test/config.bin", replaced)
    ```
 
 ## 🗓️ TODO
 
-- [ ] 上板验证
+- [X] 上板验证
 - [ ] 参数检验
 - [ ] 配置/测试帧III/IV型
```

## Comparing `paitest-0.0.12.dist-info/RECORD` & `paitest-1.0.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 paitest/__init__.py,sha256=ZJN5Lf-VYbem3hDg45chGHznWqQvNQ4qYRHTIY4l_lI,40
 paitest/frames/__init__.py,sha256=xF0aeAVW27e8tCnJaxhR6MHM4qKYLZ0GSfhowLj0mUg,267
 paitest/frames/coord.py,sha256=Jg_YGEcclIFmmFtu5P1CKxaEocXPby6PXREJDI9gv8w,2581
 paitest/frames/coord.pyi,sha256=yogiWEB90vYATDc5SRPMmsVs_F0Ur4GwFM0Mx1hrEc8,805
 paitest/frames/frame.py,sha256=uwXMi2T-PXRtg-SXoY9_yt8-20Ur5Oe8qyPBLkmkOPo,14188
 paitest/frames/frame_params.py,sha256=nlK23_RL1jZ3oyuCInuFLQ40x7KkKrCIOLgnMCmvzwE,4706
 paitest/log.py,sha256=0wn34g4m7nr837MwHNNsgZiNr9me-ywlGtfV4-iOTe4,230
-paitest/paitest.py,sha256=L3H3ZXKwQA_SKriYQ5o1x8UxaBmz1vkunbnGgGtEZTU,18563
+paitest/paitest.py,sha256=16jrXE5-XX4lZOVEWqJNekLttIISlVYIpqZbRe_0lL4,18540
 paitest/paitest.pyi,sha256=ENTfqauMvGCjBU69gWo0H85oqDtUMA1JtQapwIezcoQ,1692
-paitest-0.0.12.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-paitest-0.0.12.dist-info/METADATA,sha256=gT8-iUdTWGXfWHeY3heiaLlcuCjmfqpVP646RBF7IY0,3451
-paitest-0.0.12.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-paitest-0.0.12.dist-info/RECORD,,
+paitest-1.0.0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+paitest-1.0.0.dist-info/METADATA,sha256=W0hEWOUnMmx4ATEkcoDH_6m1V8IYzNfxu2sScUv3568,3437
+paitest-1.0.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+paitest-1.0.0.dist-info/RECORD,,
```

