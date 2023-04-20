# Comparing `tmp/sparclclient-1.2.0b3.dev8-py3-none-any.whl.zip` & `tmp/sparclclient-1.2.0b3.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 28607 bytes, number of entries: 17
--rw-rw-r--  2.0 unx     8000 b- defN 23-Apr-19 01:23 sparcl/Results.py
--rw-rw-r--  2.0 unx     1018 b- defN 23-Apr-19 21:21 sparcl/__init__.py
--rw-rw-r--  2.0 unx    29299 b- defN 23-Apr-19 21:11 sparcl/client.py
--rw-rw-r--  2.0 unx      953 b- defN 22-Aug-23 21:07 sparcl/conf.py
--rw-rw-r--  2.0 unx     3813 b- defN 23-Apr-19 01:21 sparcl/exceptions.py
--rw-rw-r--  2.0 unx     4949 b- defN 23-Feb-07 18:10 sparcl/fields.py
--rw-rw-r--  2.0 unx     6781 b- defN 23-Feb-08 21:54 sparcl/gather_2d.py
--rw-rw-r--  2.0 unx    13112 b- defN 22-Sep-14 20:31 sparcl/type_conversion.py
--rw-rw-r--  2.0 unx     1867 b- defN 23-Feb-08 21:54 sparcl/unsupported.py
--rw-rw-r--  2.0 unx     3965 b- defN 22-Aug-23 21:07 sparcl/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Aug-23 21:07 sparcl/benchmarks/__init__.py
--rw-rw-r--  2.0 unx     9667 b- defN 22-Nov-02 21:04 sparcl/benchmarks/benchmarks.py
--rw-r--r--  2.0 unx     1576 b- defN 23-Apr-19 21:23 sparclclient-1.2.0b3.dev8.dist-info/LICENSE
--rw-rw-r--  2.0 unx      872 b- defN 23-Apr-19 21:23 sparclclient-1.2.0b3.dev8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 21:23 sparclclient-1.2.0b3.dev8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 21:23 sparclclient-1.2.0b3.dev8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1367 b- defN 23-Apr-19 21:23 sparclclient-1.2.0b3.dev8.dist-info/RECORD
-17 files, 87338 bytes uncompressed, 26373 bytes compressed:  69.8%
+Zip file size: 30950 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx     8000 b- defN 23-Apr-20 21:46 sparcl/Results.py
+-rw-rw-r--  2.0 unx     1035 b- defN 23-Apr-20 22:56 sparcl/__init__.py
+-rw-rw-r--  2.0 unx      798 b- defN 23-Mar-15 14:12 sparcl/big_retrieve.py
+-rw-rw-r--  2.0 unx    29684 b- defN 23-Apr-20 21:46 sparcl/client.py
+-rw-rw-r--  2.0 unx      953 b- defN 23-Feb-08 18:38 sparcl/conf.py
+-rw-rw-r--  2.0 unx      887 b- defN 23-Mar-15 15:44 sparcl/dls_376.py
+-rw-rw-r--  2.0 unx     3813 b- defN 23-Apr-20 21:46 sparcl/exceptions.py
+-rw-rw-r--  2.0 unx     5002 b- defN 23-Mar-26 21:24 sparcl/fields.py
+-rw-rw-r--  2.0 unx     9799 b- defN 23-Apr-20 22:52 sparcl/gather_2d.py
+-rw-rw-r--  2.0 unx    13112 b- defN 23-Feb-08 18:38 sparcl/type_conversion.py
+-rw-rw-r--  2.0 unx     1867 b- defN 23-Feb-28 20:09 sparcl/unsupported.py
+-rw-rw-r--  2.0 unx     4682 b- defN 23-Mar-26 21:03 sparcl/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Feb-08 18:38 sparcl/benchmarks/__init__.py
+-rw-rw-r--  2.0 unx     9667 b- defN 23-Feb-08 18:38 sparcl/benchmarks/benchmarks.py
+-rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      872 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1518 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/RECORD
+19 files, 93364 bytes uncompressed, 28486 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: sparcl/Results.py
 Comment: 
 
 Filename: sparcl/__init__.py
 Comment: 
 
+Filename: sparcl/big_retrieve.py
+Comment: 
+
 Filename: sparcl/client.py
 Comment: 
 
 Filename: sparcl/conf.py
 Comment: 
 
+Filename: sparcl/dls_376.py
+Comment: 
+
 Filename: sparcl/exceptions.py
 Comment: 
 
 Filename: sparcl/fields.py
 Comment: 
 
 Filename: sparcl/gather_2d.py
@@ -30,23 +36,23 @@
 
 Filename: sparcl/benchmarks/__init__.py
 Comment: 
 
 Filename: sparcl/benchmarks/benchmarks.py
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev8.dist-info/LICENSE
+Filename: sparclclient-1.2.0b3.dev9.dist-info/LICENSE
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev8.dist-info/METADATA
+Filename: sparclclient-1.2.0b3.dev9.dist-info/METADATA
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev8.dist-info/WHEEL
+Filename: sparclclient-1.2.0b3.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev8.dist-info/top_level.txt
+Filename: sparclclient-1.2.0b3.dev9.dist-info/top_level.txt
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev8.dist-info/RECORD
+Filename: sparclclient-1.2.0b3.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparcl/__init__.py

```diff
@@ -1,9 +1,9 @@
 # List of packages to import when "from sparcl import *" is used
-__all__ = ["client"]
+__all__ = ["client", "align_records"]
 
 
 # See semantic versioning
 
 # BUT PyPi requires honoring versions like this:
 # https://packaging.python.org/specifications/core-metadata/
 # https://www.python.org/dev/peps/pep-0440/
@@ -27,8 +27,8 @@
 #__version__ = '1.0.0b1.dev7'
 #__version__ = '1.0.0b1.dev8'
 #__version__ = '1.0.0b1.dev9'
 #__version__ = '1.0.1b2.dev1'
 #__version__ = '1.1rc1'
 #__version__ = '1.1rc2'
 #__version__ = '1.1'
-__version__ = '1.2.0b3.dev8'
+__version__ = '1.2.0b3.dev9'
```

## sparcl/client.py

```diff
@@ -2,15 +2,14 @@
 This module interfaces to the SPARC-Server to get spectra data.
 """
 # python -m unittest tests.tests_api
 #
 # Doctest example:
 #   cd ~/sandbox/sparclclient
 #   activate
-#   pip install -e .
 #   python sparcl/client.py
 #   ## Returns NOTHING if everything works, else lists errors.
 
 ############################################
 # Python Standard Library
 from urllib.parse import urlencode, urlparse
 from warnings import warn
@@ -334,15 +333,16 @@
             self.apiversion = float(response.content)
         return self.apiversion
 
     def find(self, outfields=None, *,
              constraints={},  # dict(fname) = [op, param, ...]
              #dataset_list=None,
              limit=500,
-             sort=None):
+             sort=None,
+             verbose=None):
         """Find records in the SPARC database.
 
         Args:
             outfields (:obj:`list`, optional): List of fields to return.
                 Only CORE fields may be passed to this parameter.
                 Defaults to None, which will return only the sparcl_id
                 and _dr fields.
@@ -357,14 +357,17 @@
 
             limit (:obj:`int`, optional): Maximum number of records to
                 return. Defaults to 500.
 
             sort (:obj:`list`, optional): Comma separated list of fields
                 to sort by. Defaults to None. (no sorting)
 
+            verbose (:obj:`bool`, optional): Set to True for in-depth return
+                statement. Defaults to False.
+
         Returns:
             :class:`~sparcl.Results.Found`: Contains header and records.
 
         Example:
             >>> client = SparclClient()
             >>> outs = ['id', 'ra', 'dec']
             >>> cons = {'spectype': ['GALAXY'], 'redshift': [0.5, 0.9]}
@@ -373,49 +376,57 @@
             ['_dr', 'dec', 'id', 'ra']
         """
         # dataset_list (:obj:`list`, optional): List of data sets from
         #     which to find records. Defaults to None, which
         #     will find records in all data sets hosted on the SPARC
         #     database.
 
+        verbose = self.verbose if verbose is None else verbose
+
         # Let "outfields" default to ['id']; but fld may have been renamed
         if outfields is None:
             dslist = list(self.fields.all_datasets)
             idfld = self.fields._science_name('id', dslist[0])
             if idfld not in self.fields.common():
                 msg = (f'The "id" field ("{idfld}" is not common to all '
                        f'current Data Sets ({(", ").join(dslist)}) '
                        f'so we cannot use the default outfields="{idfld}".'
                        )
                 raise ex.NoCommonIdField(msg)
             outfields = [idfld]
         dataset_list = self.fields.all_drs
-        self._validate_science_fields(outfields, dataset_list=dataset_list)
+        #! self._validate_science_fields(outfields, dataset_list=dataset_list) # DLS-401
         dr = list(dataset_list)[0]
         if len(constraints) > 0:
             self._validate_science_fields(constraints.keys(),
                                           dataset_list=dataset_list)
             constraints = {self.fields._internal_name(k, dr): v
                            for k, v in constraints.items()}
         uparams = dict(limit=limit,)
         if sort is not None:
             uparams['sort'] = sort
         qstr = urlencode(uparams)
         url = f'{self.apiurl}/find/?{qstr}'
+
         outfields = [self.fields._internal_name(s, dr) for s in outfields]
         search = [[k] + v for k, v in constraints.items()]
         sspec = dict(outfields=outfields, search=search)
+        if verbose:
+            print(f'url={url} sspec={sspec}')
         res = requests.post(url, json=sspec, timeout=self.timeout)
 
         if res.status_code != 200:
-            if self.verbose and ('traceback' in res.json()):
+            if verbose and ('traceback' in res.json()):
                 print(f'DBG: Server traceback=\n{res.json()["traceback"]}')
             raise ex.genSparclException(res, verbose=self.verbose)
 
-        return Found(res.json(), client=self)
+        found = Found(res.json(), client=self)
+        if verbose:
+            print(f'Record key counts: {ut.count_values(found.records)}')
+        return found
 
     def missing(self, uuid_list, *, dataset_list=None,
                 countOnly=False, verbose=False):
         """Return the subset of sparcl_ids in the given uuid_list that are
         NOT stored in the SPARC database.
 
         Args:
```

## sparcl/fields.py

```diff
@@ -82,15 +82,16 @@
     def all_datasets(self):
         return self.all_drs
 
     def _science_name(self, internal_name, dataset):
         return self.o2n[dataset].get(internal_name)
 
     def _internal_name(self, science_name, dataset):
-        return self.n2o[dataset][science_name]
+        #!return self.n2o[dataset][science_name]
+        return self.n2o[dataset].get(science_name)
 
     def filter_fields(self, attr, dataset_list):
         fields = set()
         for dr in dataset_list:
             for k, v in self.attrs[dr].items():
                 if v.get(attr):
                     fields.add(k)
```

## sparcl/gather_2d.py

```diff
@@ -1,7 +1,10 @@
+"""Align or resample spectra related fields across multiple records."""
+# See client.py for Doctest example
+#
 # See:
 #   https://spectres.readthedocs.io/en/latest/
 # For info about problems with floating point,
 #   See:  https://docs.python.org/3/tutorial/floatingpoint.html
 #   Also: https://docs.python.org/3/library/decimal.html#floating-point-notes
 #
 import math
@@ -12,15 +15,15 @@
 #
 import sparcl.client
 
 
 # Per paper, should be able to pass all flux in one call to spectres
 # https://arxiv.org/pdf/1705.05165.pdf
 # Perhaps users would rather the bins uniform (1,5,20 Angstroms?)
-def resample_flux(records, wavstep=1):
+def _resample_flux(records, wavstep=1):
     smallest = math.floor(min([min(r.wavelength) for r in records]))
     largest = math.ceil(max([max(r.wavelength) for r in records]))
 
     #!wrange = largest - smallest
     #new_wavs = np.fromfunction(lambda i: i + smallest, (wrange,), dtype=int)
     #flux_2d = np.ones([len(records), wrange])
 
@@ -31,20 +34,20 @@
         flux_2d[idx] = spectres.spectres(new_wavs,
                                          rec.wavelength,
                                          rec.flux,
                                          verbose=False)
     return flux_2d, new_wavs
 
 
-def tt0(numrecs=20):
+def _tt0(numrecs=20):
     client = sparcl.client.SparclClient()
     found = client.find(constraints=dict(data_release=['BOSS-DR16']),
                         limit=numrecs)
     got = client.retrieve(found.ids)
-    flux_2d, new_wavs = resample_flux(got.records)
+    flux_2d, new_wavs = _resample_flux(got.records)
     return flux_2d, new_wavs
 
 
 # Map every wavelength of every record to index (ri,wi)
 # where
 #   ri: Record Index
 #   wi: Window Index (offset of wavelength in WINDOW)
@@ -58,25 +61,25 @@
 #!                 wi = window.index(wl)
 #!             except:
 #!                 continue
 #!             ar[ri,wi] = wl
 #!     return ar
 
 
-def wavelength_offsets(records):
+def _wavelength_offsets(records):
     # sorted list of wavelengths from ALL records
     window = sorted(
         set(records[0].wavelength).union(*[r.wavelength for r in records[1:]]))
     # offsets[ri] = index into WINDOW
     offsets = {ri: window.index(rec.wavelength[0])
                for ri, rec in enumerate(records)}
     return(window, offsets)
 
 
-def validate_wavelength_alignment(records, window, offsets, precision=None):
+def _validate_wavelength_alignment(records, window, offsets, precision=None):
     PLACES = Decimal(10) ** -precision if precision is not None else None
     #! print(f'DBG: PLACES={PLACES}')
     # Given an exact wavelength match between first wl (wavelength) in a rec
     # and the wl at its offset of WINDOW, ensure all the remaning wls
     # in rec match the next N wls of WINDOW.
     for ri, rec in enumerate(records):
         for wi, rwl in enumerate(rec.wavelength):  # wi=recwavelengthIndex
@@ -96,39 +99,39 @@
 
 
 # We want to align a bunch of records by wavelength into a single
 # 2d numpy array (record vs wavelength).  In general, we
 # are not guaranteed that this is possible -- even if using only
 # records from a single DataSet. So validate it first.
 # (If not valid, allowing wavelength slop might help.)
-def align_wavelengths(records):
+def _align_wavelengths(records):
     window, offsets = wavelength_offsets(records)
-    validate_wavelength_alignment(records, window, offsets)
+    _validate_wavelength_alignment(records, window, offsets)
     ar = np.ones([len(records), len(window)])
     for ri, r in enumerate(records):
         for wi, wl in enumerate(r.wavelength):
             ar[ri, offsets[ri + wi]] = wl  # @@@WRONG!!! We want FLUX
     return ar
 
 
-def tt1(numrecs=20, dr='BOSS-DR16'):
+def _tt1(numrecs=20, dr='BOSS-DR16'):
     client = sparcl.client.SparclClient()
     found = client.find(constraints=dict(data_release=[dr]),
                         limit=numrecs)
     got = client.retrieve(found.ids)
     records = got.records
     window, offsets = wavelength_offsets(records)
     print(f'Built window len={len(window)}; offsets={offsets}')
     #return records, window, offsets
-    ar = align_wavelengths(records)
+    ar = _align_wavelengths(records)
     return ar
 
 
 # precision:: number of decimal places
-def wavelength_grid_offsets(records, precision=11):
+def _wavelength_grid_offsets(records, precision=11):
     PLACES = Decimal(10) ** -precision
 
     # set of wavelengths from ALL records. Quantized to precision
     gset = set()  # Grid SET
     for r in records:
         gset.update([Decimal(w).quantize(PLACES) for w in r.wavelength])
     grid = sorted(gset)  # 1D sorted list of wavelengths (bigger than any rec)
@@ -137,37 +140,107 @@
     offsets = {ri: grid.index(Decimal(rec.wavelength[0]).quantize(PLACES))
                for ri, rec in enumerate(records)}
     return(grid, offsets)
 
 
 # return 2D numpy array of FLUX values that is aligned to wavelength GRID.
 # GRID is generally wider than flux for single record. Pad with NaN.
-def flux_grid(records, grid, offsets, precision=None):
-    validate_wavelength_alignment(records, grid, offsets, precision=precision)
+def _flux_grid(records, grid, offsets, precision=None):
+    _validate_wavelength_alignment(records, grid, offsets, precision=precision)
     ar = np.full([len(records), len(grid)], np.nan)
     for ri, r in enumerate(records):
         for fi, flux in enumerate(r.flux):
             ar[ri, offsets[ri] + fi] = flux
     return ar
 
+# RETURN 2D nparray(records,wavelengthGrid) = fieldValue
+def _field_grid(records, fieldName, grid, offsets, precision=None):
+    ar = np.full([len(records), len(grid)], np.nan)
+    for ri, r in enumerate(records):
+        for fi, fieldValue in enumerate(r[fieldName]):
+            ar[ri, offsets[ri] + fi] = fieldValue
+    return ar  # (wavelengthGrid, records)
+
+# RETURN 2D nparray(fields,wavelengthGrid) = fieldValue
+#! def rec_grid(rec, fields, grid, offsets, precision=None):
+#!     ar = np.full([len(fields), len(grid)], np.nan)
+#!     ri = 0
+#!     for fi, fieldValue in enumerate(r[fieldName]):
+#!         ar[ri, offsets[ri] + fi] = fieldValue
+#!     return ar  # (wavelengthGrid, fields)
+
+
+# Align flux from records into one array using quantization
+#! def flux_records(records, precision=None):
+#!     grid, offsets = wavelength_grid_offsets(records, precision=precision)
+#!     ar = _flux_grid(records, grid, offsets, precision=precision)
+#!     return ar, np.array([float(x) for x in grid])
+
+# TOP level: Intended for access from Jupyter NOTEBOOK.
+# Align spectra related field from records into one array using quantization.
+def align_records(records, fields=None, precision=7):
+    """Align given spectra-type fields to a common wavelength grid.
+
+    Args:
+        records (list): List of dictionaries. The keys for all these dictionaries
+            are Science Field Names.
+
+        fields (:obj:`list`, optional): List of Science Field Names of
+            spectra related fields to align and include in the results.
+
+        precision (:obj:`int`, optional): Number of decimal points to use for
+            quantizing wavelengths into a grid. Default=7
+
+    Returns:
+        tuple containing:
+        - ar_dict(dict): Dictionary of 2D numpy arrays keyed by Field Name.
+              Each array is shape: (numRecs, numzGridWavelengths)
+        - grid(ndarray): 1D numpy array containing wavelength values.
+
+    Example:
+        >>> client = sparcl.client.SparclClient()
+        >>> specflds = ['wavelength', 'flux', 'ivar', 'mask', 'model']
+        >>> cons = {"data_release": ['BOSS-DR16']}
+        >>> found = client.find(constraints=cons, limit=21)
+        >>> got = client.retrieve(found.ids, include=specflds)
+        >>> ar_dict, grid = align_records(got.records, fields=specflds)
+        >>> ar_dict['model'].shape
+        (21, 4670)
+
+    """
+    grid, offsets = _wavelength_grid_offsets(records, precision=precision)
+    _validate_wavelength_alignment(records, grid, offsets, precision=precision)
+
+    # One slice for each record; each slice a 2darray(wavelength, fieldName)=fldVal
+    #! slices = list()
+    #! for rec in records:
+    #!     ar = rec_grid(rec, fields, grid, offsets, precision=None):
+    #!     slices.append(ar)
+
+    # One slice for each field; each slice a 2darray(wavelength, record)=fldVal
+    adict = dict()
+    for fld in fields:
+        ar = _field_grid(records, fld, grid, offsets, precision=None)
+        adict[fld] = ar
 
-def flux_records(records, precision=None):
-    grid, offsets = wavelength_grid_offsets(records, precision=precision)
-    ar = flux_grid(records, grid, offsets, precision=precision)
-    return ar, grid
+    return adict, np.array([float(x) for x in grid])
 
 
-def tt(numrecs=9, dr='BOSS-DR16', precision=7):
+def _tt(numrecs=9, dr='BOSS-DR16', precision=7):
     # Get sample of NUMRECS records from DR DataSet.
     client = sparcl.client.SparclClient()
     found = client.find(constraints=dict(data_release=[dr]),
                         limit=numrecs)
     got = client.retrieve(found.ids)
     records = got.records
 
-    #! grid, offsets = wavelength_grid_offsets(records, precision=precision)
+    #! grid, offsets = _wavelength_grid_offsets(records, precision=precision)
     #! print(f'Built grid len={len(grid)} '
     #!       f'offsets({len(offsets)})[:5]={list(offsets.values())[:5]}')
-    #! ar = flux_grid(records, grid, offsets, precision=precision)
+    #! ar = _flux_grid(records, grid, offsets, precision=precision)
     ar, grid = flux_records(records, precision=precision)
     return ar, grid  # ar (numRecs,len(grid))
 # with np.printoptions(threshold=np.inf, linewidth=210, formatter=dict(float=lambda v: f'{v: > 7.3f}')): print(ar.T)  # noqa: E501
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

## sparcl/utils.py

```diff
@@ -1,12 +1,12 @@
 # Python library
-#!import os
 import datetime
 import time
 import socket
+import itertools
 # External packages
 #   none
 # LOCAL packages
 #   none
 
 
 # data = {
@@ -138,7 +138,26 @@
         tree = {showname: type(obj).__name__}
     return(tree)
 
 
 def invLUT(lut):
     """Given dict[k]=v, Return dict[v]=k"""
     return {v: k for k, v in lut.items()}
+
+def count_values(recs):
+    """Count number of non-None values in a list of dictionaries.
+    A key that exists with a value of None is treated the same as a
+    key that does not exist at all. i.e. It does not add to the count.
+
+    Args:
+       recs (:obj:`list`): ('records') List of dictionaries.
+
+    Returns:
+        A dictionary. Keys are the full list of keys available in any
+        of the recs.  Values are the count of occurances of non-None values
+        for that key.
+
+    >>> count_values([dict(a=None, b=3), dict(a=1, b=2), dict(a=None, b=2)])
+    {'a': 1, 'b': 3}
+    """
+    allkeys = set(list(itertools.chain(*recs)))
+    return {k: sum(x.get(k) is not None for x in recs) for k in allkeys}
```

## Comparing `sparclclient-1.2.0b3.dev8.dist-info/LICENSE` & `sparclclient-1.2.0b3.dev9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparclclient-1.2.0b3.dev8.dist-info/METADATA` & `sparclclient-1.2.0b3.dev9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparclclient
-Version: 1.2.0b3.dev8
+Version: 1.2.0b3.dev9
 Summary: A client for getting spectra data from NOIRLab.
 Home-page: https://github.com/astro-datalab/sparclclient
 Author: NOIRLab DataLab
 Author-email: datalab-spectro@noirlab.edu
 Project-URL: Documentation, https://sparclclient.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
```

