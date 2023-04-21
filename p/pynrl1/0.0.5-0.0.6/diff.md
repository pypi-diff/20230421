# Comparing `tmp/pynrl1-0.0.5.tar.gz` & `tmp/pynrl1-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrl1-0.0.5.tar", last modified: Mon Apr 17 08:59:42 2023, max compression
+gzip compressed data, was "pynrl1-0.0.6.tar", last modified: Fri Apr 21 06:23:53 2023, max compression
```

## Comparing `pynrl1-0.0.5.tar` & `pynrl1-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 08:59:27.000000 pynrl1-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 08:59:42.477290 pynrl1-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-17 08:59:27.000000 pynrl1-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.473290 pynrl1-0.0.5/pynrl1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1/downlink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pbch.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pbch_dmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_sss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/nr_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/nr_prbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 08:59:42.481290 pynrl1-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 08:59:27.000000 pynrl1-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pbch.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pbch_dmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pdschdmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pdschdmrs_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_prbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pss.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_sss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.353018 pynrl1-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 06:23:43.000000 pynrl1-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-21 06:23:53.353018 pynrl1-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-21 06:23:43.000000 pynrl1-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.349018 pynrl1-0.0.6/pynrl1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.353018 pynrl1-0.0.6/pynrl1/downlink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPBCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPBCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrPSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/downlink/nrSSSIndices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.353018 pynrl1-0.0.6/pynrl1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/nrCarrierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/nrNumerologyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/nrPDSCHConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pynrl1/util/nrSymbolModulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.353018 pynrl1-0.0.6/pynrl1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-21 06:23:53.000000 pynrl1-0.0.6/pynrl1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-21 06:23:53.000000 pynrl1-0.0.6/pynrl1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:23:53.000000 pynrl1-0.0.6/pynrl1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 06:23:53.000000 pynrl1-0.0.6/pynrl1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 06:23:53.000000 pynrl1-0.0.6/pynrl1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 06:23:43.000000 pynrl1-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 06:23:53.357018 pynrl1-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 06:23:43.000000 pynrl1-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:53.353018 pynrl1-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-21 06:23:43.000000 pynrl1-0.0.6/tests/test_nrSymbolModulate.py
```

### Comparing `pynrl1-0.0.5/LICENSE` & `pynrl1-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.5/PKG-INFO` & `pynrl1-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrl1
-Version: 0.0.5
+Version: 0.0.6
 Summary: L1 NR 3GPP Python implementation
 Home-page: https://github.com/vborchsh/pynrl1
 Download-URL: https://github.com/vborchsh/pynrl1/tarball/master
 Author: Vladislav Borshch
 Author-email: borchsh.vn@mail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/vborchsh/pynrl1/issues
```

### Comparing `pynrl1-0.0.5/README.md` & `pynrl1-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs.py` & `pynrl1-0.0.6/pynrl1/downlink/nrPDSCHDMRS.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 # 38.211
 
 import numpy as np
 
-from pynrl1.util.nr_prbs import nr_prbs
-from pynrl1.util.nr_mapper import nr_mapper
-from pynrl1.util.configurations import nrPDSCH_config
-from pynrl1.util.configurations import nrCarrier_config
+from pynrl1.util.nrPRBS import nrPRBS
+from pynrl1.util.nrSymbolModulate import nrSymbolModulate
+from pynrl1.util.nrPDSCHConfig import nrPDSCHConfig
+from pynrl1.util.nrCarrierConfig import nrCarrierConfig
 
-def nr_pdschdmrs(cfg: nrPDSCH_config, carrier: nrCarrier_config):
+def nrPDSCHDMRS(cfg: nrPDSCHConfig, carrier: nrCarrierConfig):
     if cfg.dmrs_conf_type == 1:
         n_dmrs_per_re = 6
     else:
         n_dmrs_per_re = 4
     n_dmrs_bits_re = 2*n_dmrs_per_re
 
     dmrs_begin = n_dmrs_bits_re * min(cfg.PRB_set)
@@ -23,19 +23,19 @@
 
     occupied_syms = pdschdmrs_occ_symbols(cfg.dmrs_typeA_pos, cfg.symbol_allocation[1], cfg.dmrs_additional_pos)
 
     # Start generation for every symbol
     dmrs_syms = np.array([])
     for n_symb in occupied_syms:
         cinit_dmrs = nr_pdschdmrs_cinit(carrier.symbols_per_slot, carrier.n_slot, n_symb, cfg.dmrs_NIDNSCID, n_scid)
-        dmrs_prbs = nr_prbs(cinit_dmrs, dmrs_size )
+        dmrs_prbs = nrPRBS(cinit_dmrs, dmrs_size)
 
         # Cut PRBS sequency
         dmrs_prbs = dmrs_prbs[dmrs_begin:dmrs_end]
-        dmrs_syms = np.append(dmrs_syms, nr_mapper(dmrs_prbs, "QPSK"))
+        dmrs_syms = np.append(dmrs_syms, nrSymbolModulate(dmrs_prbs, "QPSK"))
 
     return dmrs_syms
 
 # LUT for DMRS occupied symbols positions
 def pdschdmrs_occ_symbols(typeA_pos, sym_alloc, add_pos):
     l1 = 11
 
@@ -43,15 +43,15 @@
     occupied_syms = np.append(occupied_syms, typeA_pos)
 
     if sym_alloc in [8, 9]:
         occupied_syms = np.append(occupied_syms, 7)
     elif sym_alloc in [10, 11]:
         if add_pos == 1:
             occupied_syms = np.append(occupied_syms, 9)
-        if add_pos == 2 or add_pos == 3:
+        elif add_pos == 2 or add_pos == 3:
             occupied_syms = np.append(occupied_syms, [6, 9])
     elif sym_alloc == 12:
         if add_pos == 1:
             occupied_syms = np.append(occupied_syms, 11)
         elif add_pos == 2:
             occupied_syms = np.append(occupied_syms, [7, 11])
         elif add_pos == 3:
@@ -62,8 +62,8 @@
         elif add_pos == 2:
             occupied_syms = np.append(occupied_syms, [7, 11])
         elif add_pos == 3:
             occupied_syms = np.append(occupied_syms, [5, 8, 11])
     return occupied_syms
 
 def nr_pdschdmrs_cinit(sps, n_slot, n_symb, NIDSCID, n_scid):
-    return (1 << 17) * (sps * n_slot + n_symb + 1) * ((NIDSCID << 1) + 1) + ((NIDSCID << 1) + n_scid)
+    return 2**17 * (sps * n_slot + n_symb + 1) * (2*NIDSCID + 1) + 2*NIDSCID + n_scid
```

### Comparing `pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs_indices.py` & `pynrl1-0.0.6/pynrl1/downlink/nrPDSCHDMRSIndices.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 # 38.211
 
 import numpy as np
 
-from pynrl1.downlink.nr_pdschdmrs import pdschdmrs_occ_symbols
-from pynrl1.util.configurations import nrPDSCH_config
+from pynrl1.downlink.nrPDSCHDMRS import pdschdmrs_occ_symbols
+from pynrl1.util.nrPDSCHConfig import nrPDSCHConfig
 
-def nr_pdschdmrs_indices(cfg: nrPDSCH_config):
+def nrPDSCHDMRSIndices(cfg: nrPDSCHConfig):
     frame_begin = cfg.n_rb_size * min(cfg.PRB_set)
     frame_end = cfg.n_rb_size * (max(cfg.PRB_set)+1)
     frame_size = cfg.n_rb_size * cfg.n_size_bwp
 
     # Single frame DMRS positions
     dmrs_full_range = np.array(list(range(frame_begin, frame_end)))
 
@@ -20,15 +20,14 @@
         occupied_res = dmrs_full_range[::2]
     elif cfg.dmrs_conf_type == 2:
         # Takes every 4th couple of symbols
         occupied_res = dmrs_full_range.reshape(-1, 2)[::3].ravel()
 
     # Calculates occupied symbols numbers. Time positions
     occupied_syms = pdschdmrs_occ_symbols(cfg.dmrs_typeA_pos, cfg.symbol_allocation[1], cfg.dmrs_additional_pos)
-    print(occupied_syms)
 
     dmrs_indices = np.array([])
     for idx, sym in enumerate(occupied_syms):
         sym_offset = sym*frame_size
         dmrs_indices = np.append(dmrs_indices, (occupied_res + sym_offset))
 
     return dmrs_indices
```

### Comparing `pynrl1-0.0.5/pynrl1/downlink/nr_sss.py` & `pynrl1-0.0.6/pynrl1/downlink/nrSSS.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import numpy as np
 
-def nr_sss(ncellid):
+def nrSSS(ncellid):
 
     assert ncellid <= 1007 and ncellid >= 0
 
     sss_precomp0 = np.array([
         0, 1, 1, 1, 1, 1, 1, 0, 1, 1, 0, 1, 1, 0, 0, 1, 0,
         1, 1, 0, 0, 0, 0, 1, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0,
         0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 0, 0, 1, 1, 1, 0,
@@ -46,15 +46,15 @@
     shift0 = nr_sss_m0(ncellid)
     shift1 = nr_sss_m1(ncellid)
 
     seq0 = sss_precomp0[shift0:(shift0+127)]
     seq1 = sss_precomp1[shift1:(shift1+127)]
 
     # XNOR
-    return [480+np.array(range(56, 183)), np.invert(np.logical_xor(seq0, seq1))*1]
+    return np.invert(np.logical_xor(seq0, seq1))*1
 
 
 def nr_sss_m0(ncellid):
     n1 = ncellid // 3
     n2 = ncellid % 3
     return 15*(n1 // 112) + 5*n2
```

### Comparing `pynrl1-0.0.5/pynrl1/util/nr_mapper.py` & `pynrl1-0.0.6/pynrl1/util/nrSymbolModulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # 38.211 5.1 Modulation mapper
 
 import numpy as np
 
-def nr_mapper(databits, modtype):
-    int_modtype = modtype.lower()
+def nrSymbolModulate(databits, modulation):
+    int_modtype = modulation.lower()
 
     assert int_modtype in ['bpsk_pi2', 'bpsk', 'qpsk', 'qam16', 'qam64', 'qam256'], "modulation type is incorrect"
     assert len(databits) > 0, "length of databits must be greater 0"
     assert max(databits) < 2 and min(databits) >= 0, "databits must be list of 0s and 1s"
 
     if int_modtype == 'bpsk':
         res_arr = np.zeros(len(databits), dtype=(complex))
```

### Comparing `pynrl1-0.0.5/pynrl1/util/nr_prbs.py` & `pynrl1-0.0.6/pynrl1/util/nrPRBS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # 38.211 5.2.1 Pseudo-random sequence generation
 
 import numpy as np
 
-def nr_prbs(cinit, n):
+def nrPRBS(cinit, n):
 
     assert n > 0
 
     # 9 = [1 0 0 1], 15 = [1 1 1 1] (both arranged msb->lsb)
     poly = [9, 15]
 
     # Register initialization
```

### Comparing `pynrl1-0.0.5/pynrl1.egg-info/PKG-INFO` & `pynrl1-0.0.6/pynrl1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrl1
-Version: 0.0.5
+Version: 0.0.6
 Summary: L1 NR 3GPP Python implementation
 Home-page: https://github.com/vborchsh/pynrl1
 Download-URL: https://github.com/vborchsh/pynrl1/tarball/master
 Author: Vladislav Borshch
 Author-email: borchsh.vn@mail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/vborchsh/pynrl1/issues
```

### Comparing `pynrl1-0.0.5/setup.cfg` & `pynrl1-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.5/tests/test_nr_mapper.py` & `pynrl1-0.0.6/tests/test_nrSymbolModulate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import matlab.engine
 import numpy as np
 import pytest
 import itertools
 
-from pynrl1.util.nr_mapper import nr_mapper
+from pynrl1.util.nrSymbolModulate import nrSymbolModulate
 
 def get_bin_symbols(bps, symbols):
     databits = np.array(list(range(symbols)))
     databits = np.array([(x & (2**np.arange(bps)) != 0).astype(int) for x in databits])
     return np.concatenate(databits, axis=0)
 
 def run_nr_mapper(eng, modtype):
     if modtype == 'bpsk':
         databits = get_bin_symbols(1, 2)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "BPSK")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     elif modtype == 'bpsk_pi2':
         databits = get_bin_symbols(1, 2)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "pi/2-BPSK")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     elif modtype == 'qpsk':
         databits = get_bin_symbols(2, 4)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "QPSK")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     elif modtype == 'qam16':
         databits = get_bin_symbols(4, 16)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "16QAM")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     elif modtype == 'qam64':
         databits = get_bin_symbols(6, 64)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "64QAM")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     elif modtype == 'qam256':
         databits = get_bin_symbols(8, 256)
         ref_data = eng.nrSymbolModulate(eng.transpose(eng.logical(databits)), "256QAM")
-        data = nr_mapper(databits, modtype)
+        data = nrSymbolModulate(databits, modtype)
 
     ref_data = np.around(np.array(list(itertools.chain(*ref_data))), 4)
     data = np.around(data, 4)
 
     assert (ref_data == data).all()
 
 @pytest.mark.parametrize("modtype", ['bpsk', 'bpsk_pi2', 'qpsk', 'qam16', 'qam64', 'qam256'])
```

### Comparing `pynrl1-0.0.5/tests/test_nr_pbch.py` & `pynrl1-0.0.6/tests/test_nrPSS.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import matlab.engine
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.downlink.nr_pbch import nr_pbch
-
-def run_nr_pbch(ncellid, databits, v, eng):
-    ref_data = eng.nrPBCH(databits, matlab.double(ncellid), matlab.double(v), nargout=1)
-    ref_indices = eng.nrPBCHIndices(ncellid);
+from pynrl1.downlink.nrPSS import nrPSS
+from pynrl1.downlink.nrPSSIndices import nrPSSIndices
 
+def run_nr_pss(ncellid, eng):
+    ref_data = eng.nrPSS(matlab.double(ncellid))
     ref_data = np.array(list(itertools.chain(*ref_data)))
 
-    ref_indices = np.array(list(itertools.chain(*ref_indices)))
-    ref_indices = [x-1 for x in ref_indices]
+    ref_ind = eng.nrPSSIndices()
+    ref_ind = np.array(list(itertools.chain(*ref_ind)))
+    ref_ind = np.array(ref_ind - 1)
 
-    indices, data = nr_pbch( ncellid, v, np.array(list(itertools.chain(*databits)), dtype=(int)) )
+    data = nrPSS(ncellid)
+    data = [(x*2)-1 for x in data]
 
-    ref_data = np.around(ref_data, 4)
-    data = np.around(data, 4)
+    indices = nrPSSIndices()
 
-    assert (ref_data == data).all()
-    assert (ref_indices == indices).all()
+    assert np.all(ref_data == data)
+    assert np.all(indices == ref_ind)
 
 @pytest.mark.parametrize("ncellid", [0, 500, 1007])
-@pytest.mark.parametrize("v", list(range(8)))
-def test_nr_pbch(ncellid, v):
+def test_nr_pss(ncellid):
     eng = matlab.engine.connect_matlab()
 
     try:
-        run_nr_pbch(ncellid, eng.randi(matlab.double([0, 1]),864,1), v, eng)
+        run_nr_pss(ncellid, eng)
     finally:
-        eng.quit()
+        eng.quit()
```

### Comparing `pynrl1-0.0.5/tests/test_nr_pbch_dmrs.py` & `pynrl1-0.0.6/tests/test_nrPBCH.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import matlab.engine
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.downlink.nr_pbch_dmrs import nr_pbch_dmrs
+from pynrl1.downlink.nrPBCH import nrPBCH
+from pynrl1.downlink.nrPBCHIndices import nrPBCHIndices
+
+def run_nr_pbch(ncellid, databits, v, eng):
+    ref_data = eng.nrPBCH(databits, matlab.double(ncellid), matlab.double(v), nargout=1)
+    ref_indices = eng.nrPBCHIndices(ncellid);
 
-def run_nr_pbch_dmrs(ncellid, issb, eng):
-    ref_data = eng.nrPBCHDMRS(matlab.double(ncellid), matlab.double(issb))
     ref_data = np.array(list(itertools.chain(*ref_data)))
 
-    ref_ind = eng.nrPBCHDMRSIndices(matlab.double(ncellid))
-    ref_ind = np.array(list(itertools.chain(*ref_ind)))
-    ref_ind = np.array(ref_ind - 1)
+    ref_indices = np.array(list(itertools.chain(*ref_indices)))
+    ref_indices = [x-1 for x in ref_indices]
 
-    [indices, data] = nr_pbch_dmrs(ncellid, issb)
+    indices = nrPBCHIndices(ncellid)
+    data = nrPBCH( ncellid, v, np.array(list(itertools.chain(*databits)), dtype=(int)) )
 
     ref_data = np.around(ref_data, 4)
     data = np.around(data, 4)
 
     assert (ref_data == data).all()
-    assert (ref_ind == indices).all()
+    assert (ref_indices == indices).all()
 
 @pytest.mark.parametrize("ncellid", [0, 500, 1007])
-@pytest.mark.parametrize("issb", list(range(8)))
-def test_nr_pbch_dmrs(ncellid, issb):
+@pytest.mark.parametrize("v", list(range(8)))
+def test_nr_pbch(ncellid, v):
     eng = matlab.engine.connect_matlab()
 
     try:
-        run_nr_pbch_dmrs(ncellid, issb, eng)
+        run_nr_pbch(ncellid, eng.randi(matlab.double([0, 1]),864,1), v, eng)
     finally:
         eng.quit()
```

### Comparing `pynrl1-0.0.5/tests/test_nr_pdschdmrs.py` & `pynrl1-0.0.6/tests/test_nrPDSCHDMRS.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 import matlab.engine
+import os
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.downlink.nr_pdschdmrs import nr_pdschdmrs
-from pynrl1.util.configurations import nrPDSCH_config
-from pynrl1.util.configurations import nrCarrier_config
+from pynrl1.downlink.nrPDSCHDMRS import nrPDSCHDMRS
+from pynrl1.downlink.nrPDSCHDMRSIndices import nrPDSCHDMRSIndices
+from pynrl1.util.nrPDSCHConfig import nrPDSCHConfig
+from pynrl1.util.nrCarrierConfig import nrCarrierConfig
 
 def run_nr_pdschdmrs(cfg, eng):
-    carrier = nrCarrier_config();
+    carrier = nrCarrierConfig();
     carrier.subcarrier_spacing = 120;
     carrier.cyclic_prefix = 'normal';
     carrier.n_size_grid = 132;
     carrier.n_start_grid = 0;
 
-    pdsch_cfg = nrPDSCH_config();
+    pdsch_cfg = nrPDSCHConfig();
     pdsch_cfg.n_size_bwp = cfg['n_size_bwp']
     pdsch_cfg.n_start_bwp = cfg['n_start_bwp']
     pdsch_cfg.mapping_type = cfg['MappingType']
     pdsch_cfg.dmrs_typeA_pos = cfg['DMRSTypeAPosition']
     pdsch_cfg.dmrs_len = cfg['DMRSLength']
     pdsch_cfg.dmrs_additional_pos = cfg['DMRSAdditionalPosition']
     pdsch_cfg.dmrs_conf_type = cfg['DMRSConfigurationType']
     pdsch_cfg.dmrs_NIDNSCID = cfg['NIDNSCID']
     pdsch_cfg.dmrs_NSCID = cfg['NSCID']
     pdsch_cfg.PRB_set = cfg['PRBSet']
     pdsch_cfg.symbol_allocation = cfg['SymbolAllocation']
 
-    pdschdmrs_syms = nr_pdschdmrs(pdsch_cfg, carrier)
+    pdschdmrs_syms = nrPDSCHDMRS(pdsch_cfg, carrier)
+    pdschdmrs_indices = nrPDSCHDMRSIndices(pdsch_cfg)
 
     [pdschdmrs_syms_ref, pdschdmrs_indices_ref] = eng.gen_pdschdmrs(cfg, nargout=2)
     pdschdmrs_syms_ref = np.array(list(itertools.chain(*pdschdmrs_syms_ref)))
 
+    pdschdmrs_indices_ref = np.array(list(itertools.chain(*pdschdmrs_indices_ref)))
+    pdschdmrs_indices_ref = pdschdmrs_indices_ref - 1
+
     pdschdmrs_syms = np.around(pdschdmrs_syms, 4)
     pdschdmrs_syms_ref = np.around(pdschdmrs_syms_ref, 4)
 
     assert np.array_equal(pdschdmrs_syms, pdschdmrs_syms_ref)
+    assert np.array_equal(pdschdmrs_indices, pdschdmrs_indices_ref)
 
 
 @pytest.mark.parametrize('typeA_pos', [2, 3])
 @pytest.mark.parametrize('symb_alloc', [[2, 12]])
 @pytest.mark.parametrize('dmrs_add_pos', [0, 1, 2, 3])
 @pytest.mark.parametrize('PRBSet', [list(range(0, 132)), list(range(60, 132)), list(range(30, 60))])
 @pytest.mark.parametrize('dmrs_cfg_type', [1, 2])
 def test_nr_pdschdmrs(symb_alloc, dmrs_add_pos, typeA_pos, PRBSet, dmrs_cfg_type):
     eng = matlab.engine.connect_matlab()
+    eng.cd(os.path.dirname(__file__))
 
     cfg = {}
     cfg['n_size_bwp'] = 132
     cfg['n_start_bwp'] = 0
     cfg['MappingType'] = "A"
     cfg['DMRSTypeAPosition'] = typeA_pos
     cfg['DMRSLength'] = 1
```

### Comparing `pynrl1-0.0.5/tests/test_nr_prbs.py` & `pynrl1-0.0.6/tests/test_nrPRBS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import matlab.engine
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.util.nr_prbs import nr_prbs
+from pynrl1.util.nrPRBS import nrPRBS
 
 def run_nr_prbs(cinit, size, eng):
     ref_data = eng.nrPRBS(matlab.double(cinit), matlab.double(size))
     ref_data = list(itertools.chain(*ref_data))
     ref_data = np.array([x*1 for x in ref_data])
 
-    data = nr_prbs(cinit, size)
+    data = nrPRBS(cinit, size)
 
     assert (ref_data == data).all()
 
 @pytest.mark.parametrize("cinit", [0, 100, 1245345, 534667868])
 @pytest.mark.parametrize("size", [1024, 8192])
 def test_nr_prbs(cinit, size):
     eng = matlab.engine.connect_matlab()
```

### Comparing `pynrl1-0.0.5/tests/test_nr_pss.py` & `pynrl1-0.0.6/tests/test_nrSSS.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import matlab.engine
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.downlink.nr_pss import nr_pss
+from pynrl1.downlink.nrSSS import nrSSS
+from pynrl1.downlink.nrSSSIndices import nrSSSIndices
 
-def run_nr_pss(ncellid, eng):
-    ref_data = eng.nrPSS(matlab.double(ncellid))
+def run_nr_sss(ncellid, eng):
+    ref_data = eng.nrSSS(matlab.double(ncellid))
     ref_data = np.array(list(itertools.chain(*ref_data)))
 
-    ref_ind = eng.nrPSSIndices()
+    ref_ind = eng.nrSSSIndices()
     ref_ind = np.array(list(itertools.chain(*ref_ind)))
     ref_ind = np.array(ref_ind - 1)
 
-    [indices, data] = nr_pss(ncellid)
+    data = nrSSS(ncellid)
+    indices = nrSSSIndices()
     data = [(x*2)-1 for x in data]
 
     assert (ref_data == data).all()
     assert (indices == ref_ind).all()
 
-@pytest.mark.parametrize("ncellid", [0, 500, 1007])
-def test_nr_pss(ncellid):
+@pytest.mark.parametrize("ncellid", [0, 600, 1007])
+def test_nr_sss(ncellid):
     eng = matlab.engine.connect_matlab()
 
     try:
-        run_nr_pss(ncellid, eng)
+        run_nr_sss(ncellid, eng)
     finally:
-        eng.quit()
+        eng.quit()
+
```

### Comparing `pynrl1-0.0.5/tests/test_nr_sss.py` & `pynrl1-0.0.6/tests/test_nrPBCHDMRS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import matlab.engine
 import itertools
 import numpy as np
 import pytest
 
-from pynrl1.downlink.nr_sss import nr_sss
+from pynrl1.downlink.nrPBCHDMRS import nrPBCHDMRS
+from pynrl1.downlink.nrPBCHDMRSIndices import nrPBCHDMRSIndices
 
-def run_nr_sss(ncellid, eng):
-    ref_data = eng.nrSSS(matlab.double(ncellid))
+def run_nr_pbch_dmrs(ncellid, issb, eng):
+    ref_data = eng.nrPBCHDMRS(matlab.double(ncellid), matlab.double(issb))
     ref_data = np.array(list(itertools.chain(*ref_data)))
 
-    ref_ind = eng.nrSSSIndices()
+    ref_ind = eng.nrPBCHDMRSIndices(matlab.double(ncellid))
     ref_ind = np.array(list(itertools.chain(*ref_ind)))
     ref_ind = np.array(ref_ind - 1)
 
-    [indices, data] = nr_sss(ncellid)
-    data = [(x*2)-1 for x in data]
+    data = nrPBCHDMRS(ncellid, issb)
+    indices = nrPBCHDMRSIndices(ncellid)
 
-    assert (ref_data == data).all()
-    assert (indices == ref_ind).all()
+    ref_data = np.around(ref_data, 4)
+    data = np.around(data, 4)
 
-@pytest.mark.parametrize("ncellid", [0, 600, 1007])
-def test_nr_sss(ncellid):
+    assert np.all(ref_data == data)
+    assert np.all(ref_ind == indices)
+
+@pytest.mark.parametrize("ncellid", [0, 500, 1007])
+@pytest.mark.parametrize("issb", list(range(8)))
+def test_nr_pbch_dmrs(ncellid, issb):
     eng = matlab.engine.connect_matlab()
 
     try:
-        run_nr_sss(ncellid, eng)
+        run_nr_pbch_dmrs(ncellid, issb, eng)
     finally:
         eng.quit()
-
```

