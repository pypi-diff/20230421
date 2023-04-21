# Comparing `tmp/opencv_stubs-0.0.3.tar.gz` & `tmp/opencv_stubs-0.0.4.tar.gz`

## Comparing `opencv_stubs-0.0.3.tar` & `opencv_stubs-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/requirements/requirements.txt
--rw-r--r--   0        0        0    48826 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/src/cv2-stubs/__init__.pyi
--rw-r--r--   0        0        0    16615 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/src/cv2-stubs/constants.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/src/cv2-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/LICENSE
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/README.md
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 opencv_stubs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements.txt
+-rw-r--r--   0        0        0    49905 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0    18359 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/constants.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/py.typed
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/README.md
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/PKG-INFO
```

### Comparing `opencv_stubs-0.0.3/.pre-commit-config.yaml` & `opencv_stubs-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.3/requirements/requirements-build.txt` & `opencv_stubs-0.0.4/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.3/requirements/requirements-dev.txt` & `opencv_stubs-0.0.4/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.3/src/cv2-stubs/__init__.pyi` & `opencv_stubs-0.0.4/src/cv2-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 from collections.abc import Iterable, Sequence
 from typing import TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
@@ -113,14 +113,18 @@
     """rectangle(img, pt1, pt2, color[, thickness[, lineType[, shift]]]) -> img\n.   @brief Draws a simple, thick, or filled up-right rectangle.\n.   \n.   The function cv::rectangle draws a rectangle outline or a filled rectangle whose two opposite corners\n.   are pt1 and pt2.\n.   \n.   @param img Image.\n.   @param pt1 Vertex of the rectangle.\n.   @param pt2 Vertex of the rectangle opposite to pt1 .\n.   @param color Rectangle color or brightness (grayscale image).\n.   @param thickness Thickness of lines that make up the rectangle. Negative values, like #FILLED,\n.   mean that the function has to draw a filled rectangle.\n.   @param lineType Type of the line. See #LineTypes\n.   @param shift Number of fractional bits in the point coordinates.\n\n\n\nrectangle(img, rec, color[, thickness[, lineType[, shift]]]) -> img\n.   @overload\n.   \n.   use `rec` parameter as alternative specification of the drawn rectangle: `r.tl() and\n.   r.br()-Point(1,1)` are opposite corners."""
     ...
 
 def resize(src: npt.NDArray[TImg], dsize: tuple[int, int], dst: npt.NDArray[TImg] = ..., fx: int = ..., fy: int = ..., interpolation: int = ...) -> npt.NDArray[TImg]:
     "resize(src, dsize[, dst[, fx[, fy[, interpolation]]]]) -> dst\n.   @brief Resizes an image.\n.   \n.   The function resize resizes the image src down to or up to the specified size. Note that the\n.   initial dst type or size are not taken into account. Instead, the size and type are derived from\n.   the `src`,`dsize`,`fx`, and `fy`. If you want to resize src so that it fits the pre-created dst,\n.   you may call the function as follows:\n.   @code\n.       // explicitly specify dsize=dst.size(); fx and fy will be computed from that.\n.       resize(src, dst, dst.size(), 0, 0, interpolation);\n.   @endcode\n.   If you want to decimate the image by factor of 2 in each direction, you can call the function this\n.   way:\n.   @code\n.       // specify fx and fy and let the function compute the destination image size.\n.       resize(src, dst, Size(), 0.5, 0.5, interpolation);\n.   @endcode\n.   To shrink an image, it will generally look best with #INTER_AREA interpolation, whereas to\n.   enlarge an image, it will generally look best with c#INTER_CUBIC (slow) or #INTER_LINEAR\n.   (faster but still looks OK).\n.   \n.   @param src input image.\n.   @param dst output image; it has the size dsize (when it is non-zero) or the size computed from\n.   src.size(), fx, and fy; the type of dst is the same as of src.\n.   @param dsize output image size; if it equals zero, it is computed as:\n.    \\f[\\texttt{dsize = Size(round(fx*src.cols), round(fy*src.rows))}\\f]\n.    Either dsize or both fx and fy must be non-zero.\n.   @param fx scale factor along the horizontal axis; when it equals 0, it is computed as\n.   \\f[\\texttt{(double)dsize.width/src.cols}\\f]\n.   @param fy scale factor along the vertical axis; when it equals 0, it is computed as\n.   \\f[\\texttt{(double)dsize.height/src.rows}\\f]\n.   @param interpolation interpolation method, see #InterpolationFlags\n.   \n.   @sa  warpAffine, warpPerspective, remap."
     ...
 
+def seamlessClone(src: npt.NDArray[np.uint8], dst: npt.NDArray[np.uint8], mask: npt.NDArray[np.uint8], p: TPoint, flags: int, blend: npt.NDArray[np.uint8] = ...) -> npt.NDArray[np.uint8]:
+    "seamlessClone(src, dst, mask, p, flags[, blend]) -> blend\n.   @brief Image editing tasks concern either global changes (color/intensity corrections, filters,\n.   deformations) or local changes concerned to a selection. Here we are interested in achieving local\n.   changes, ones that are restricted to a region manually selected (ROI), in a seamless and effortless\n.   manner. The extent of the changes ranges from slight distortions to complete replacement by novel\n.   content @cite PM03 .\n.   \n.   @param src Input 8-bit 3-channel image.\n.   @param dst Input 8-bit 3-channel image.\n.   @param mask Input 8-bit 1 or 3-channel image.\n.   @param p Point in dst image where object is placed.\n.   @param blend Output image with the same size and type as dst.\n.   @param flags Cloning method that could be cv::NORMAL_CLONE, cv::MIXED_CLONE or cv::MONOCHROME_TRANSFER"
+    ...
+
 def setWindowProperty(winname: str, prop_id:int , prop_value: int) -> None:
     "setWindowProperty(winname, prop_id, prop_value) -> None\n.   @brief Changes parameters of a window dynamically.\n.   \n.   The function setWindowProperty enables changing properties of a window.\n.   \n.   @param winname Name of the window.\n.   @param prop_id Window property to edit. The supported operation flags are: (cv::WindowPropertyFlags)\n.   @param prop_value New value of the window property. The supported flags are: (cv::WindowFlags)."
     ...
 
 def threshold(src: npt.NDArray[TImg], thresh: float, maxval: float, type: int, dst: npt.NDArray[TImg] = ...) -> tuple[int, npt.NDArray[TImg]]:
     "threshold(src, thresh, maxval, type[, dst]) -> retval, dst\n.   @brief Applies a fixed-level threshold to each array element.\n.   \n.   The function applies fixed-level thresholding to a multiple-channel array. The function is typically\n.   used to get a bi-level (binary) image out of a grayscale image ( #compare could be also used for\n.   this purpose) or for removing a noise, that is, filtering out pixels with too small or too large\n.   values. There are several types of thresholding supported by the function. They are determined by\n.   type parameter.\n.   \n.   Also, the special values #THRESH_OTSU or #THRESH_TRIANGLE may be combined with one of the\n.   above values. In these cases, the function determines the optimal threshold value using the Otsu's\n.   or Triangle algorithm and uses it instead of the specified thresh.\n.   \n.   @note Currently, the Otsu's and Triangle methods are implemented only for 8-bit single-channel images.\n.   \n.   @param src input array (multiple-channel, 8-bit or 32-bit floating point).\n.   @param dst output array of the same size  and type and the same number of channels as src.\n.   @param thresh threshold value.\n.   @param maxval maximum value to use with the #THRESH_BINARY and #THRESH_BINARY_INV thresholding\n.   types.\n.   @param type thresholding type (see #ThresholdTypes).\n.   @return the computed threshold value if Otsu's or Triangle methods used.\n.   \n.   @sa  adaptiveThreshold, findContours, compare, min, max."
     ...
```

### Comparing `opencv_stubs-0.0.3/src/cv2-stubs/constants.pyi` & `opencv_stubs-0.0.4/src/cv2-stubs/constants.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -255,14 +255,22 @@
 COLOR_BayerGBRG2RGBA: int
 COLOR_BayerBG2RGBA: int  # Equivalent to RGGB Bayer pattern
 COLOR_BayerGB2RGBA: int  # Equivalent to GRBG Bayer pattern
 COLOR_BayerRG2RGBA: int  # Equivalent to BGGR Bayer pattern
 COLOR_BayerGR2RGBA: int  # Equivalent to GBRG Bayer pattern
 COLOR_COLORCVT_MAX: int
 
+# ConnectedComponentsTypes
+# https://docs.opencv.org/3.4/d3/dc0/group__imgproc__shape.html#gac7099124c0390051c6970a987e7dc5c5
+CC_STAT_LEFT: int  # The leftmost (x) coordinate which is the inclusive start of the bounding box in the horizontal direction.
+CC_STAT_TOP: int  # The topmost (y) coordinate which is the inclusive start of the bounding box in the vertical direction.
+CC_STAT_WIDTH: int  # The horizontal size of the bounding box.
+CC_STAT_HEIGHT: int  # The vertical size of the bounding box.
+CC_STAT_AREA: int  # The total area (in pixels) of the connected component.
+
 # Fonts
 FONT_HERSHEY_COMPLEX: int
 FONT_HERSHEY_COMPLEX_SMALL: int
 FONT_HERSHEY_DUPLEX: int
 FONT_HERSHEY_PLAIN: int
 FONT_HERSHEY_SCRIPT_COMPLEX: int
 FONT_HERSHEY_SCRIPT_SIMPLEX: int
@@ -283,14 +291,51 @@
 MORPH_OPEN: int
 MORPH_CLOSE: int
 MORPH_GRADIENT: int
 MORPH_TOPHAT: int
 MORPH_BLACKHAT: int
 MORPH_HITMISS: int
 
+# Number Types
+CV_16S: int
+CV_16SC1: int
+CV_16SC2: int
+CV_16SC3: int
+CV_16SC4: int
+CV_16U: int
+CV_16UC1: int
+CV_16UC2: int
+CV_16UC3: int
+CV_16UC4: int
+CV_32F: int
+CV_32FC1: int
+CV_32FC2: int
+CV_32FC3: int
+CV_32FC4: int
+CV_32S: int
+CV_32SC1: int
+CV_32SC2: int
+CV_32SC3: int
+CV_32SC4: int
+CV_64F: int
+CV_64FC1: int
+CV_64FC2: int
+CV_64FC3: int
+CV_64FC4: int
+CV_8S: int
+CV_8SC1: int
+CV_8SC2: int
+CV_8SC3: int
+CV_8SC4: int
+CV_8U: int
+CV_8UC1: int
+CV_8UC2: int
+CV_8UC3: int
+CV_8UC4: int
+
 # ImreadModes
 IMREAD_UNCHANGED: int  # If set, return the loaded image as is (with alpha channel, otherwise it gets cropped). Ignore EXIF orientation.
 IMREAD_GRAYSCALE: int  # If set, always convert image to the single channel grayscale image (codec internal conversion).
 IMREAD_COLOR: int  # If set, always convert image to the 3 channel BGR color image.
 IMREAD_ANYDEPTH: int  # If set, return 16-bit/32-bit image when the input has the corresponding depth, otherwise convert it to 8-bit.
 IMREAD_ANYCOLOR: int  # If set, the image is read in any possible color format.
 IMREAD_LOAD_GDAL: int  # If set, use the gdal driver for loading the image.
@@ -353,14 +398,20 @@
 # https://docs.opencv.org/3.4/d3/dc0/group__imgproc__shape.html#ga819779b9857cc2f8601e6526a3a5bc71
 RETR_EXTERNAL: int
 RETR_LIST: int
 RETR_CCOMP: int
 RETR_TREE: int
 RETR_FLOODFILL: int
 
+# seamlessClone algorithm flags
+# https://docs.opencv.org/3.4/df/da0/group__photo__clone.html#ga19386064a1bd4e1153262844e6875bcc
+NORMAL_CLONE: int  # The power of the method is fully expressed when inserting objects with complex outlines into a new background
+MIXED_CLONE:int   # The classic method, color-based selection and alpha masking might be time consuming and often leaves an undesirable halo. Seamless cloning, even averaged with the original image, is not effective. Mixed seamless cloning based on a loose selection proves effective.
+MONOCHROME_TRANSFER: int  # Monochrome transfer allows the user to easily replace certain features of one object by alternative features.
+
 # ThresholdTypes
 THRESH_BINARY: int
 THRESH_BINARY_INV: int
 THRESH_TRUNC: int
 THRESH_TOZERO: int
 THRESH_TOZERO_INV: int
 THRESH_MASK: int
```

### Comparing `opencv_stubs-0.0.3/LICENSE` & `opencv_stubs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.3/README.md` & `opencv_stubs-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,14 @@
 The stubs include the docstrings as they are otherwise not available in the IDE (as far as I know).
 
 These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590#issuecomment-1493255962)).
 
 
 ## Installation
 
+The package is available on pypi [here](https://pypi.org/project/opencv-stubs/), you can install it with:
+
 ```
 pip install opencv-stubs
 ```
+
+The dependency on opencv is optional, and be accessed with `pip install opencv-stubs[opencv]` or `pip install opencv-stubs[opencv-headless]`.
```

### Comparing `opencv_stubs-0.0.3/pyproject.toml` & `opencv_stubs-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,30 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
 license = {text = "MIT"}
 dynamic = ["version"]
-dependencies = ["numpy>=1.21", "opencv-python>=4.7.0.0"]
+dependencies = ["numpy>=1.21"]
 requires-python = ">=3.8"
 packages = [
     { "include" = "cv2-stubs"}
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hoel-bagard/opencv-stubs"
 "Bug Tracker" = "https://github.com/hoel-bagard/opencv-stubs/issues"
 
 [project.optional-dependencies]
 dev = ["pre-commit", "pip-tools", "ruff", "pyright"]
 build = ["hatch"]
+# I couldn't figure out how to have "opencv or opencv-headless" as dependency, so they are both optional.
+opencv = ["opencv-python>=4.7.0"]
+opencv-headless = ["opencv-python-headless>=4.7.0"]
 
 [tool.hatch.version]
 path = "src/cv2-stubs/__init__.pyi"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `opencv_stubs-0.0.3/PKG-INFO` & `opencv_stubs-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-stubs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial stubs for the opencv-python package.
 Project-URL: Homepage, https://github.com/hoel-bagard/opencv-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/opencv-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: OpenCV,stubs
@@ -15,22 +15,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.21
-Requires-Dist: opencv-python>=4.7.0.0
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: opencv
+Requires-Dist: opencv-python>=4.7.0; extra == 'opencv'
+Provides-Extra: opencv-headless
+Requires-Dist: opencv-python-headless>=4.7.0; extra == 'opencv-headless'
 Description-Content-Type: text/markdown
 
 # OpenCV stubs
 
 [![PyPI](https://img.shields.io/pypi/v/opencv-stubs?color=green&style=flat)](https://pypi.org/project/opencv-stubs)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/opencv-stubs?style=flat)](https://pypi.org/project/opencv-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/opencv-stubs?style=flat)](https://pypi.org/project/opencv-stubs)
@@ -47,10 +50,14 @@
 The stubs include the docstrings as they are otherwise not available in the IDE (as far as I know).
 
 These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590#issuecomment-1493255962)).
 
 
 ## Installation
 
+The package is available on pypi [here](https://pypi.org/project/opencv-stubs/), you can install it with:
+
 ```
 pip install opencv-stubs
 ```
+
+The dependency on opencv is optional, and be accessed with `pip install opencv-stubs[opencv]` or `pip install opencv-stubs[opencv-headless]`.
```

