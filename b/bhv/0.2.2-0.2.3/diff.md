# Comparing `tmp/bhv-0.2.2.tar.gz` & `tmp/bhv-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.2.tar", last modified: Thu Apr 13 23:23:36 2023, max compression
+gzip compressed data, was "bhv-0.2.3.tar", last modified: Thu Apr 20 22:30:47 2023, max compression
```

## Comparing `bhv-0.2.2.tar` & `bhv-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-13 23:23:36.918571 bhv-0.2.2/PKG-INFO
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11347 2023-04-13 17:08:27.000000 bhv-0.2.2/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9571 2023-04-12 17:37:58.000000 bhv-0.2.2/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     7088 2023-04-12 17:37:58.000000 bhv-0.2.2/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8750 2023-04-13 22:34:48.000000 bhv-0.2.2/bhv/symbolic.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      246 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-13 23:23:36.918571 bhv-0.2.2/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-13 22:35:40.000000 bhv-0.2.2/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-20 22:30:47.164835 bhv-0.2.3/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3038 2023-04-18 21:57:32.000000 bhv-0.2.3/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.3/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12037 2023-04-18 17:15:37.000000 bhv-0.2.3/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.3/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.3/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.3/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-17 15:03:13.000000 bhv-0.2.3/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9164 2023-04-17 13:54:04.000000 bhv-0.2.3/bhv/symbolic.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      256 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-20 22:30:47.164835 bhv-0.2.3/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-20 22:29:22.000000 bhv-0.2.3/setup.py
```

### Comparing `bhv-0.2.2/PKG-INFO` & `bhv-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.2
+Version: 0.2.3
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.2/bhv/abstract.py` & `bhv-0.2.3/bhv/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,38 @@
 
     def flip_frac_off(self, flip_off_frac) -> Self:
         return self & self.flip_frac(2*flip_off_frac)
 
     def permute(self, permutation_id: int) -> Self:
         raise NotImplementedError()
 
+    def swap_halves(self) -> Self:
+        raise NotImplementedError()
+
+    def rehash(self) -> Self:
+        raise NotImplementedError()
+
+    _FEISTAL_ROUNDS = 8
+
+    @classmethod
+    def _feistal_round(cls, block: Self, round_key: Self) -> Self:
+        L = block & cls.HALF
+        R = (block ^ (L ^ round_key).rehash().swap_halves()) & ~cls.HALF
+
+        return (L | R).swap_halves()
+
+    def feistal(self, k: Self, inv=False) -> Self:
+        block = self
+        rounds = range(self._FEISTAL_ROUNDS)
+
+        for r in reversed(rounds) if inv else rounds:
+            block = self._feistal_round(block, self._FEISTAL_SUBKEYS[r] & k)
+
+        return block.swap_halves()
+
     @classmethod
     def majority3(cls, x, y, z) -> Self:
         return cls.majority([x, y, z])
 
     @classmethod
     def majority(cls, vs: list[Self]) -> Self:
         n = len(vs)
@@ -301,14 +325,15 @@
     def _majority7_via_3(cls, a: Self, b: Self, c: Self, d: Self, e: Self, f: Self, g: Self) -> Self:
         mdef = cls._majority3(d, e, f)
         mabc = cls._majority3(a, b, c)
         return cls._majority3(g, cls._majority3(c, mdef, cls._majority3(a, b, mdef)), cls._majority3(f, mabc, cls._majority3(d, e, mabc)))
 
     ZERO: Self
     ONE: Self
+    HALF: Self
 
 
 class MemoizedPermutation:
     _permutations: 'dict[int | tuple[int, ...], Self]'
 
     @classmethod
     def nrandom(cls, n) -> list[Self]:
```

### Comparing `bhv-0.2.2/bhv/embedding.py` & `bhv-0.2.3/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.2/bhv/np.py` & `bhv-0.2.3/bhv/np.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,20 @@
     @classmethod
     def random(cls, active=0.5) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.random.binomial(1, active, DIMENSION))
 
     def select(self, when1: 'NumPyBoolBHV', when0: 'NumPyBoolBHV') -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.where(self.data, when1.data, when0.data))
 
+    def swap_halves(self) -> 'NumPyBoolBHV':
+        return self.roll_bits(DIMENSION//2)
+
+    def rehash(self) -> 'NumPyBoolBHV':
+        return self.pack8().rehash().unpack()
+
     def roll_bits(self, n: int) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.roll(self.data, n))
 
     def permute_bits(self, permutation: 'NumPyBoolPermutation') -> 'NumPyBoolBHV':
         return NumPyBoolBHV(self.data[permutation.data])
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> 'NumPyBoolBHV':
@@ -83,22 +89,25 @@
         return NumPyPacked8BHV(np.packbits(self.data))
 
     def pack64(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.packbits(self.data).view(dtype=np.uint64))
 
 NumPyBoolBHV.ZERO = NumPyBoolBHV(np.zeros(DIMENSION, dtype=np.bool_))
 NumPyBoolBHV.ONE = NumPyBoolBHV(np.ones(DIMENSION, dtype=np.bool_))
+NumPyBoolBHV._FEISTAL_SUBKEYS = NumPyBoolBHV.nrand2(NumPyBoolBHV._FEISTAL_ROUNDS, 4)
+_halfb = np.zeros(DIMENSION, dtype=np.bool_)
+_halfb[:DIMENSION//2] = np.bool_(True)
+NumPyBoolBHV.HALF = NumPyBoolBHV(_halfb)
 
 
 class NumPyBytePermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
     rng = np.random.default_rng()
 
     def __init__(self, array: np.ndarray):
-        print("array size", array.size)
         self.data: np.ndarray = array
 
     @classmethod
     def random(cls) -> 'NumPyBytePermutation':
         return NumPyBytePermutation(cls.rng.permutation(DIMENSION//8))
 
     def __mul__(self, other: 'NumPyBytePermutation') -> 'NumPyBytePermutation':
@@ -125,20 +134,29 @@
     def random(cls, active=0.5) -> 'NumPyPacked8BHV':
         return NumPyBoolBHV.random(active).pack8()
 
     def roll_bytes(self, n: int) -> 'NumPyPacked8BHV':
         assert abs(n) < DIMENSION//8, "only supports DIMENSION/8 rolls"
         return NumPyPacked8BHV(np.roll(self.data, n))
 
+    def swap_halves(self) -> 'NumPyPacked8BHV':
+        return self.roll_bytes(DIMENSION//16)
+
     def permute_bytes(self, permutation: 'NumPyBytePermutation') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(self.data[permutation.data])
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> 'NumPyPacked8BHV':
         return self.permute_bytes(NumPyBytePermutation.get(permutation_id))
 
+    def rehash(self) -> 'NumPyPacked8BHV':
+        byte_data = self.data.tobytes()
+        rehashed_byte_data = hashlib.shake_256(byte_data).digest(DIMENSION//8)
+        rehashed_data = np.frombuffer(rehashed_byte_data, dtype=np.uint8)
+        return NumPyPacked8BHV(rehashed_data)
+
     def __eq__(self, other: 'NumPyPacked8BHV') -> bool:
         return np.array_equal(self.data, other.data)
 
     def __xor__(self, other: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_xor(self.data, other.data))
 
     def __and__(self, other: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
@@ -152,16 +170,23 @@
 
     def active(self) -> int:
         return sum(x.bit_count() for x in self.data)
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data))
 
+    def repack64(self) -> 'NumPyPacked64BHV':
+        return NumPyPacked64BHV(self.data.view(dtype=np.uint64))
+
 NumPyPacked8BHV.ZERO = NumPyPacked8BHV(np.zeros(DIMENSION//8, dtype=np.uint8))
 NumPyPacked8BHV.ONE = NumPyPacked8BHV(np.full(DIMENSION//8, fill_value=255, dtype=np.uint8))
+NumPyPacked8BHV._FEISTAL_SUBKEYS = NumPyPacked8BHV.nrand2(NumPyPacked8BHV._FEISTAL_ROUNDS, 4)
+_half8 = np.zeros(DIMENSION//8, dtype=np.uint8)
+_half8[:DIMENSION//16] = np.uint8(255)
+NumPyPacked8BHV.HALF = NumPyPacked8BHV(_half8)
 
 
 class NumPyWordPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
     rng = np.random.default_rng()
 
     def __init__(self, array: np.ndarray):
@@ -197,14 +222,20 @@
     def random(cls, active=0.5) -> 'NumPyPacked64BHV':
         return NumPyBoolBHV.random(active).pack64()
 
     @classmethod
     def _majority_via_unpacked(cls, vs: list['NumPyPacked64BHV']) -> 'NumPyPacked64BHV':
         return NumPyBoolBHV.majority([v.unpack() for v in vs]).pack64()
 
+    def swap_halves(self) -> 'NumPyPacked64BHV':
+        return self.roll_words(DIMENSION//128)
+
+    def rehash(self) -> 'NumPyPacked64BHV':
+        return self.repack8().rehash().repack64()
+
     def roll_words(self, n: int) -> 'NumPyPacked64BHV':
         assert abs(n) < DIMENSION//64, "only supports DIMENSION/64 rolls"
         return NumPyPacked64BHV(np.roll(self.data, n))
 
     def roll_word_bits(self, n: int) -> 'NumPyPacked64BHV':
         assert abs(permutation_id) < 64, "only supports 64 rolls"
         if n == 0:
@@ -242,9 +273,16 @@
 
     def active(self) -> int:
         return sum(x.bit_count() for x in self.data)
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data.view(np.uint8)))
 
+    def repack8(self) -> 'NumPyPacked8BHV':
+        return NumPyPacked8BHV(self.data.view(dtype=np.uint8))
+
 NumPyPacked64BHV.ZERO = NumPyPacked64BHV(np.zeros(DIMENSION//64, dtype=np.uint64))
 NumPyPacked64BHV.ONE = NumPyPacked64BHV(np.full(DIMENSION//64, fill_value=-1, dtype=np.uint64))
+NumPyPacked64BHV._FEISTAL_SUBKEYS = NumPyPacked64BHV.nrand2(NumPyPacked64BHV._FEISTAL_ROUNDS, 4)
+_half64 = np.zeros(DIMENSION//64, dtype=np.uint64)
+_half64[:DIMENSION//128] = np.uint64(-1)
+NumPyPacked64BHV.HALF = NumPyPacked64BHV(_half64)
```

### Comparing `bhv-0.2.2/bhv/pytorch.py` & `bhv-0.2.3/bhv/pytorch.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,25 @@
 
     def permute_bits(self, permutation: TorchBoolPermutation) -> 'TorchBoolBHV':
         return TorchBoolBHV(self.data[permutation.data])
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> 'TorchBoolBHV':
         return self.permute_bits(TorchBoolPermutation.get(permutation_id))
 
+    def swap_halves(self) -> 'TorchBoolBHV':
+        return self.roll_bits(DIMENSION//2)
+
+    def rehash(self) -> 'TorchBoolBHV':
+        # torch to bytes is broken hence custom function https://github.com/pytorch/pytorch/issues/33041
+        offsets = [(H & self).active() for H in self._HS]
+        res = self._HASH
+        for o in offsets:
+            res = res ^ self.roll_bits(o)
+        return res
+
     def __eq__(self, other: 'TorchBoolBHV') -> bool:
         return torch.equal(self.data, other.data)
 
     def __xor__(self, other: 'TorchBoolBHV') -> 'TorchBoolBHV':
         return TorchBoolBHV(torch.bitwise_xor(self.data, other.data))
 
     def __and__(self, other: 'TorchBoolBHV') -> 'TorchBoolBHV':
@@ -105,14 +116,20 @@
         return torch.sum(self.data).item()
 
     def pack(self) -> 'TorchPackedBHV':
         return TorchPackedBHV(pack_bool_to_long(self.data))
 
 TorchBoolBHV.ZERO = TorchBoolBHV(torch.zeros(DIMENSION, dtype=torch.bool))
 TorchBoolBHV.ONE = TorchBoolBHV(torch.ones(DIMENSION, dtype=torch.bool))
+TorchBoolBHV._HASH = TorchBoolBHV.rand()
+TorchBoolBHV._HS = TorchBoolBHV.nrand2(5, power=2)
+TorchBoolBHV._FEISTAL_SUBKEYS = TorchBoolBHV.nrand2(TorchBoolBHV._FEISTAL_ROUNDS, 4)
+_halfb = torch.zeros(DIMENSION, dtype=torch.bool)
+_halfb[:DIMENSION//2] = 1
+TorchBoolBHV.HALF = TorchBoolBHV(_halfb)
 
 
 class TorchWordPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
 
     def __init__(self, tensor: torch.IntTensor):
         self.data: torch.BoolTensor = tensor
@@ -151,14 +168,20 @@
 
     def permute_words(self, permutation: TorchWordPermutation) -> 'TorchPackedBHV':
         return TorchPackedBHV(self.data[permutation.data])
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> 'TorchPackedBHV':
         return self.permute_words(TorchWordPermutation.get(permutation_id))
 
+    def swap_halves(self) -> 'TorchPackedBHV':
+        return self.roll_words(DIMENSION//128)
+
+    def rehash(self) -> 'TorchPackedBHV':
+        return self.unpack().rehash().pack()
+
     def __eq__(self, other: 'TorchBoolBHV') -> bool:
         return torch.equal(self.data, other.data)
 
     def __xor__(self, other: 'TorchPackedBHV') -> 'TorchPackedBHV':
         return TorchPackedBHV(torch.bitwise_xor(self.data, other.data))
 
     def __and__(self, other: 'TorchPackedBHV') -> 'TorchPackedBHV':
@@ -180,7 +203,11 @@
         return torch.sum(x).item()
 
     def unpack(self) -> 'TorchBoolBHV':
         return TorchBoolBHV(unpack_long_to_bool(self.data))
 
 TorchPackedBHV.ZERO = TorchPackedBHV(torch.zeros(DIMENSION//64, dtype=torch.long))
 TorchPackedBHV.ONE = TorchPackedBHV(torch.full((DIMENSION//64,), fill_value=-1, dtype=torch.long))  # -1 is all ones in torch's encoding
+TorchPackedBHV._FEISTAL_SUBKEYS = TorchPackedBHV.nrand2(TorchPackedBHV._FEISTAL_ROUNDS, 4)
+_half64 = torch.zeros(DIMENSION//64, dtype=torch.long)
+_half64[:DIMENSION//128] = -1
+TorchPackedBHV.HALF = TorchPackedBHV(_half64)
```

### Comparing `bhv-0.2.2/bhv/shared.py` & `bhv-0.2.3/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.2/bhv/symbolic.py` & `bhv-0.2.3/bhv/symbolic.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,20 @@
     @classmethod
     def majority(cls, vs: list[Self]) -> Self:
         return Majority(vs)
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> Self:
         return Permute(permutation_id, self)
 
+    def swap_halves(self) -> Self:
+        return SwapHalves(self)
+
+    def rehash(self) -> Self:
+        return ReHash(self)
+
     def __eq__(self, other: Self) -> bool:
         return Eq(self, other)
 
     def __xor__(self, other: Self) -> Self:
         return Xor(self, other)
 
     def __and__(self, other: Self) -> Self:
@@ -227,14 +233,26 @@
 class Permute(SymbolicBHV):
     id: 'int | tuple[int, ...]'
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.permute({self.id})"
 @dataclass
+class SwapHalves(SymbolicBHV):
+    v: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.v.show(**kwargs)}.swap_halves()"
+@dataclass
+class ReHash(SymbolicBHV):
+    v: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.v.show(**kwargs)}.rehash()"
+@dataclass
 class Eq:
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} == {self.r.show(**kwargs)})"
 @dataclass
```

### Comparing `bhv-0.2.2/bhv.egg-info/PKG-INFO` & `bhv-0.2.3/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.2
+Version: 0.2.3
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.2/setup.py` & `bhv-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

