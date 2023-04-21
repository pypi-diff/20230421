# Comparing `tmp/xyz_py-5.3.1.tar.gz` & `tmp/xyz_py-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.3.1.tar", last modified: Thu Apr 20 18:03:21 2023, max compression
+gzip compressed data, was "xyz_py-5.3.2.tar", last modified: Fri Apr 21 12:40:32 2023, max compression
```

## Comparing `xyz_py-5.3.1.tar` & `xyz_py-5.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.875319 xyz_py-5.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-20 18:02:56.000000 xyz_py-5.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 18:03:21.874319 xyz_py-5.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-20 18:02:56.000000 xyz_py-5.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-20 18:02:56.000000 xyz_py-5.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 18:03:21.875319 xyz_py-5.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-20 18:03:18.000000 xyz_py-5.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.871319 xyz_py-5.3.1/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     8316 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-20 18:03:18.000000 xyz_py-5.3.1/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37690 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.874319 xyz_py-5.3.1/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 12:40:32.665872 xyz_py-5.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-21 12:40:04.000000 xyz_py-5.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-21 12:40:32.663872 xyz_py-5.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-21 12:40:04.000000 xyz_py-5.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-21 12:40:04.000000 xyz_py-5.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 12:40:32.665872 xyz_py-5.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-21 12:40:29.000000 xyz_py-5.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 12:40:32.659872 xyz_py-5.3.2/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-21 12:40:04.000000 xyz_py-5.3.2/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-21 12:40:04.000000 xyz_py-5.3.2/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8316 2023-04-21 12:40:04.000000 xyz_py-5.3.2/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-21 12:40:29.000000 xyz_py-5.3.2/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37714 2023-04-21 12:40:04.000000 xyz_py-5.3.2/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 12:40:32.663872 xyz_py-5.3.2/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-21 12:40:32.000000 xyz_py-5.3.2/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.3.1/LICENSE` & `xyz_py-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.1/PKG-INFO` & `xyz_py-5.3.2/xyz_py.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.3.1
+Name: xyz-py
+Version: 5.3.2
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.3.1/README.md` & `xyz_py-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.1/setup.py` & `xyz_py-5.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.3.1"
+__version__ = "5.3.2"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.3.1/xyz_py/atomic.py` & `xyz_py-5.3.2/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.1/xyz_py/cli.py` & `xyz_py-5.3.2/xyz_py/cli.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.1/xyz_py/xyz_py.py` & `xyz_py-5.3.2/xyz_py/xyz_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -575,15 +575,15 @@
     bonds, _ = find_bonds(
         labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
     )
 
     return bonds
 
 
-def find_bonds(labels, coords, neigh_list=None, verbose=True, style='indices'):
+def find_bonds(labels, coords, neigh_list=None, verbose=True, style='labels'):
     '''
     Calculate list of atoms between which there is a bond.
     Using ASE. Only unique bonds are retained.
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
@@ -603,15 +603,15 @@
             indices : Bond list contains atom number
             labels  : Bond list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique bonds (atom pairs)
-    list[float]
+    np.ndarray
         Bond length in Angstrom
     '''
 
     # Remove labels if present
     labels_nn = remove_label_indices(labels)
 
     # Create molecule object
@@ -644,18 +644,18 @@
         for atom in ibt
     ]
 
     # Count bonds
     n_bonds = len(bonds)
 
     # Calculate actual values
-    values = [
+    values = np.array([
         ana.get_bond_value(0, bond)
         for bond in bonds
-    ]
+    ])
 
     # Set format and convert to atomic labels if requested
     if style == 'labels':
         bonds = [
             [labels[atom1], labels[atom2]]
             for atom1, atom2 in bonds
         ]
@@ -710,15 +710,15 @@
         labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
     )
 
     return angles
 
 
 def find_angles(labels, coords, neigh_list=None, verbose=True,
-                style='indices'):
+                style='labels'):
     '''
     Calculate all angles using ASE. Only unique angles are retained.
     e.g. 0-1-2 but not 2-1-0
 
     Parameters
     ----------
     labels : list
@@ -737,15 +737,15 @@
             indices : Angle labels are atom number
             labels  : Angle labels are atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique angles (atom trios) as labels or indices
-    list[float]
+    np.ndarray
         Angles in degrees
     '''
 
     # Remove labels if present
     labels_nn = remove_label_indices(labels)
 
     # Create molecule object
@@ -776,18 +776,18 @@
         for atoms in ibt:
             angles.append([it, *atoms])
 
     # Count angles
     n_angles = len(angles)
 
     # Calculate actual values
-    values = [
+    values = np.array([
         ana.get_angle_value(0, angle)
         for angle in angles
-    ]
+    ])
 
     # Set format and convert to atomic labels if requested
     if style == 'labels':
         angles = [
             [labels[atom1], labels[atom2], labels[atom3]]
             for atom1, atom2, atom3 in angles
         ]
@@ -841,15 +841,15 @@
         labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
     )
 
     return dihedrals
 
 
 def find_dihedrals(labels, coords, neigh_list=None, verbose=True,
-                   style='indices'):
+                   style='labels'):
     '''
     Calculate and list of atoms between which there is a dihedral.
     Using ASE. Only unique dihedrals are retained.
     e.g. 0-1-2-3 but not 3-2-1-0
 
     Parameters
     ----------
@@ -869,15 +869,15 @@
             indices : Dihedral list contains atom number
             labels  : Dihedral list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique dihedrals (atom quads)
-    list[float]
+    np.ndarray
         Dihedral angles in degrees
     '''
 
     # Remove labels if present
     labels_nn = remove_label_indices(labels)
 
     # Create molecule object
@@ -905,18 +905,18 @@
     # definition to each element of the rhs
     dihedrals = []
     for it, ibt in enumerate(is_dihedraled_to):
         for atoms in ibt:
             dihedrals.append([it, *atoms])
 
     # Calculate actual values
-    values = [
+    values = np.array([
         ana.get_dihedral_value(0, dihedral)
         for dihedral in dihedrals
-    ]
+    ])
 
     # Count dihedrals
     n_dihedrals = len(dihedrals)
 
     # Set format and convert to atomic labels if requested
     if style == 'labels':
         dihedrals = [
```

### Comparing `xyz_py-5.3.1/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.3.1
+Name: xyz_py
+Version: 5.3.2
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

