# Comparing `tmp/calorine-1.5.tar.gz` & `tmp/calorine-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calorine-1.5.tar", last modified: Mon Mar 13 20:46:51 2023, max compression
+gzip compressed data, was "calorine-1.6.tar", last modified: Fri Apr 21 19:05:46 2023, max compression
```

## Comparing `calorine-1.5.tar` & `calorine-1.6.tar`

### file list

```diff
@@ -1,156 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.269684 calorine-1.5/
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-03-13 20:46:37.000000 calorine-1.5/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-13 20:46:37.000000 calorine-1.5/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-13 20:46:37.000000 calorine-1.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3169 2023-03-13 20:46:37.000000 calorine-1.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-03-13 20:46:37.000000 calorine-1.5/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-03-13 20:46:37.000000 calorine-1.5/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    16725 2023-03-13 20:46:37.000000 calorine-1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1265 2023-03-13 20:46:51.269684 calorine-1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-03-13 20:46:37.000000 calorine-1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.225680 calorine-1.5/calorine/
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-03-13 20:46:37.000000 calorine-1.5/calorine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.227680 calorine-1.5/calorine/calculators/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-03-13 20:46:37.000000 calorine-1.5/calorine/calculators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-03-13 20:46:37.000000 calorine-1.5/calorine/calculators/cpunep.py
--rw-rw-rw-   0 root         (0) root         (0)    11345 2023-03-13 20:46:37.000000 calorine-1.5/calorine/calculators/gpunep.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.228680 calorine-1.5/calorine/gpumd/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-03-13 20:46:37.000000 calorine-1.5/calorine/gpumd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7717 2023-03-13 20:46:37.000000 calorine-1.5/calorine/gpumd/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.230680 calorine-1.5/calorine/nep/
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-03-13 20:46:37.000000 calorine-1.5/calorine/nep/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12927 2023-03-13 20:46:37.000000 calorine-1.5/calorine/nep/io.py
--rw-rw-rw-   0 root         (0) root         (0)     6922 2023-03-13 20:46:37.000000 calorine-1.5/calorine/nep/nep.py
--rw-rw-rw-   0 root         (0) root         (0)    14972 2023-03-13 20:46:37.000000 calorine-1.5/calorine/nep/potential.py
--rw-rw-rw-   0 root         (0) root         (0)     4779 2023-03-13 20:46:37.000000 calorine-1.5/calorine/nep/training_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.231680 calorine-1.5/calorine/tools/
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-03-13 20:46:37.000000 calorine-1.5/calorine/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2023-03-13 20:46:37.000000 calorine-1.5/calorine/tools/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2023-03-13 20:46:37.000000 calorine-1.5/calorine/tools/phonons.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2023-03-13 20:46:37.000000 calorine-1.5/calorine/tools/stiffness.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2023-03-13 20:46:37.000000 calorine-1.5/calorine/tools/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.227680 calorine-1.5/calorine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1265 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4391 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-13 20:46:51.000000 calorine-1.5/calorine.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.234681 calorine-1.5/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.235681 calorine-1.5/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-03-13 20:46:37.000000 calorine-1.5/doc/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-03-13 20:46:37.000000 calorine-1.5/doc/_static/logo.ico
--rw-rw-rw-   0 root         (0) root         (0)    18405 2023-03-13 20:46:37.000000 calorine-1.5/doc/_static/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.236681 calorine-1.5/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-03-13 20:46:37.000000 calorine-1.5/doc/_templates/breadcrumbs.html
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-03-13 20:46:37.000000 calorine-1.5/doc/_templates/page.html
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-03-13 20:46:37.000000 calorine-1.5/doc/_templates/versions.html
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-03-13 20:46:37.000000 calorine-1.5/doc/calculators.rst
--rw-rw-rw-   0 root         (0) root         (0)     2799 2023-03-13 20:46:37.000000 calorine-1.5/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-13 20:46:37.000000 calorine-1.5/doc/genindex.rst
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-13 20:46:37.000000 calorine-1.5/doc/gpumd.rst
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-03-13 20:46:37.000000 calorine-1.5/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-03-13 20:46:37.000000 calorine-1.5/doc/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-03-13 20:46:37.000000 calorine-1.5/doc/nep.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-03-13 20:46:37.000000 calorine-1.5/doc/tools.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.239681 calorine-1.5/doc/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    27771 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/calculators.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4391 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/nep_descriptors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   707350 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/nep_model_inspection.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   216024 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/phonons.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    35580 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/structure_relaxation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   299814 2023-03-13 20:46:37.000000 calorine-1.5/doc/tutorials/visualize_descriptor_space_with_pca.ipynb
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 20:46:51.269684 calorine-1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-03-13 20:46:37.000000 calorine-1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.219679 calorine-1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.241681 calorine-1.5/src/nepy/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-03-13 20:46:37.000000 calorine-1.5/src/nepy/README.md
--rw-rw-rw-   0 root         (0) root         (0)    75546 2023-03-13 20:46:37.000000 calorine-1.5/src/nepy/nep.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-03-13 20:46:37.000000 calorine-1.5/src/nepy/nep.h
--rw-rw-rw-   0 root         (0) root         (0)     5004 2023-03-13 20:46:37.000000 calorine-1.5/src/nepy/nepy.cpp
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-03-13 20:46:37.000000 calorine-1.5/src/nepy/nepy.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.246682 calorine-1.5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.249682 calorine-1.5/tests/example_files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.250682 calorine-1.5/tests/example_files/fcp/
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/fcp/fcp.txt
--rw-rw-rw-   0 root         (0) root         (0)     4988 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/fcp/fcs_order2.in
--rw-rw-rw-   0 root         (0) root         (0)     2376 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/fcp/r0.in
--rw-rw-rw-   0 root         (0) root         (0)     5520 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/hac.out
--rw-rw-rw-   0 root         (0) root         (0)     5520 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/hac_nan.out
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/kappa.out
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/kappa_nan.out
--rw-rw-rw-   0 root         (0) root         (0)    11400 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/loss.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.250682 calorine-1.5/tests/example_files/md_no_velocities_or_forces/
--rw-rw-rw-   0 root         (0) root         (0)     6001 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/md_no_velocities_or_forces/dump.xyz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.251682 calorine-1.5/tests/example_files/md_velocities_and_forces/
--rw-rw-rw-   0 root         (0) root         (0)     9605 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/md_velocities_and_forces/dump.xyz
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/nep.in
--rw-rw-rw-   0 root         (0) root         (0)    21699 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/nep.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/run.in
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/thermo_ortho_v3.2.out
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_files/thermo_tri_v3.2.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.257683 calorine-1.5/tests/example_output/
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CON_NEP2_dummy_CON_3atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CON_NEP2_dummy_CON_3atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CO_NEP2_dummy_CO_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/CO_NEP2_dummy_CO_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/C_NEP2_dummy_C_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/C_NEP2_dummy_C_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)   145555 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)    13930 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)    41677 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_virial.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.259683 calorine-1.5/tests/example_structures/
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_structures/CON_3atom.in
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_structures/CO_2atom.in
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_structures/C_2atom.in
--rw-rw-rw-   0 root         (0) root         (0)    20588 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_structures/PbTe_250atom.in
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-13 20:46:37.000000 calorine-1.5/tests/example_structures/PbTe_2atom.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.263683 calorine-1.5/tests/nep_models/
--rw-rw-rw-   0 root         (0) root         (0)    28522 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/CON_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    26644 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/CO_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    26642 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/C_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    52623 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/CsPbI3-SCAN.txt
--rw-rw-rw-   0 root         (0) root         (0)    26647 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/PbTe_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/README.md
--rw-rw-rw-   0 root         (0) root         (0)    21670 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt
--rw-rw-rw-   0 root         (0) root         (0)    21687 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt
--rw-rw-rw-   0 root         (0) root         (0)    37053 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/nep4_PbTe.txt
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-03-13 20:46:37.000000 calorine-1.5/tests/nep_models/update_expted_descriptors.py
--rw-rw-rw-   0 root         (0) root         (0)     5445 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    16212 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_cpunep.py
--rw-rw-rw-   0 root         (0) root         (0)    11285 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_gpumd_io.py
--rw-rw-rw-   0 root         (0) root         (0)    17572 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_gpunep.py
--rw-rw-rw-   0 root         (0) root         (0)     3743 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_nep3_execution.py
--rw-rw-rw-   0 root         (0) root         (0)     3743 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_nep4_execution.py
--rw-rw-rw-   0 root         (0) root         (0)    14638 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_nep_io.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_nep_nep.py
--rw-rw-rw-   0 root         (0) root         (0)     5690 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_nep_potential.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_phonons.py
--rw-rw-rw-   0 root         (0) root         (0)     5360 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_setup_training.py
--rw-rw-rw-   0 root         (0) root         (0)     6833 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_stiffness.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-03-13 20:46:37.000000 calorine-1.5/tests/test_structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.267684 calorine-1.5/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    52623 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/CsPbI3-SCAN.txt
--rw-rw-rw-   0 root         (0) root         (0)    21687 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/PbTe_NEP3.txt
--rw-rw-rw-   0 root         (0) root         (0)    27771 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/calculators.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    49025 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/elastic_stiffness_tensor.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4391 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/nep_descriptors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   707350 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/nep_model_inspection.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 20:46:51.269684 calorine-1.5/tutorials/perovskite-structures/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/perovskite-structures/CsPbI3-cubic-Pm-3m.xyz
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz
--rw-rw-rw-   0 root         (0) root         (0)   216024 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/phonons.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    35580 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/structure_relaxation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   299814 2023-03-13 20:46:37.000000 calorine-1.5/tutorials/visualize_descriptor_space_with_pca.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.497277 calorine-1.6/
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-04-21 19:05:34.000000 calorine-1.6/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-21 19:05:34.000000 calorine-1.6/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-04-21 19:05:34.000000 calorine-1.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-21 19:05:34.000000 calorine-1.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-04-21 19:05:34.000000 calorine-1.6/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2023-04-21 19:05:34.000000 calorine-1.6/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    16725 2023-04-21 19:05:34.000000 calorine-1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-21 19:05:46.497277 calorine-1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-04-21 19:05:34.000000 calorine-1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.447273 calorine-1.6/calorine/
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-21 19:05:34.000000 calorine-1.6/calorine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.450273 calorine-1.6/calorine/calculators/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6498 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/cpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)    11345 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/gpunep.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.451274 calorine-1.6/calorine/gpumd/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-21 19:05:34.000000 calorine-1.6/calorine/gpumd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7717 2023-04-21 19:05:34.000000 calorine-1.6/calorine/gpumd/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.453274 calorine-1.6/calorine/nep/
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     9877 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/nep.py
+-rw-rw-rw-   0 root         (0) root         (0)    14972 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/potential.py
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/training_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.454274 calorine-1.6/calorine/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/phonons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/stiffness.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.449273 calorine-1.6/calorine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.457274 calorine-1.6/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.458274 calorine-1.6/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/logo.ico
+-rw-rw-rw-   0 root         (0) root         (0)    18405 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.459274 calorine-1.6/doc/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/breadcrumbs.html
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/page.html
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/versions.html
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-21 19:05:34.000000 calorine-1.6/doc/calculators.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-21 19:05:34.000000 calorine-1.6/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-21 19:05:34.000000 calorine-1.6/doc/genindex.rst
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-21 19:05:34.000000 calorine-1.6/doc/gpumd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-21 19:05:34.000000 calorine-1.6/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 19:05:34.000000 calorine-1.6/doc/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-21 19:05:34.000000 calorine-1.6/doc/nep.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-21 19:05:34.000000 calorine-1.6/doc/tools.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.463274 calorine-1.6/doc/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    48216 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/calculators.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    48910 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/elastic_stiffness_tensor.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    57668 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/nep_descriptors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   707350 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/nep_model_inspection.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   215886 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/phonons.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    35580 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/structure_relaxation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   162489 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/thermal_conductivity_from_bte.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   299804 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/visualize_descriptor_space_with_pca.ipynb
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 19:05:46.497277 calorine-1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-04-21 19:05:34.000000 calorine-1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.441273 calorine-1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.465275 calorine-1.6/src/nepy/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    81016 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nep.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nep.h
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nepy.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nepy.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.470275 calorine-1.6/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.473275 calorine-1.6/tests/example_files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.474275 calorine-1.6/tests/example_files/dipole/
+-rw-rw-rw-   0 root         (0) root         (0)    31383 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/dipole/dipole_test.out
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/dipole/test.xyz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/fcp/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/fcp.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4988 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/fcs_order2.in
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/r0.in
+-rw-rw-rw-   0 root         (0) root         (0)     5520 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/hac.out
+-rw-rw-rw-   0 root         (0) root         (0)     5520 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/hac_nan.out
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/kappa.out
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/kappa_nan.out
+-rw-rw-rw-   0 root         (0) root         (0)    11400 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/loss.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/md_no_velocities_or_forces/
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/md_no_velocities_or_forces/dump.xyz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/md_velocities_and_forces/
+-rw-rw-rw-   0 root         (0) root         (0)     9605 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/md_velocities_and_forces/dump.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/nep.in
+-rw-rw-rw-   0 root         (0) root         (0)    21699 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/nep.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/run.in
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/thermo_ortho_v3.2.out
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/thermo_tri_v3.2.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.482276 calorine-1.6/tests/example_output/
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)   145555 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)    13930 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)    41677 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_virial.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.483276 calorine-1.6/tests/example_structures/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/CON_3atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/CO_2atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/C_2atom.in
+-rw-rw-rw-   0 root         (0) root         (0)    20588 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/PbTe_250atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/PbTe_2atom.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.488276 calorine-1.6/tests/nep_models/
+-rw-rw-rw-   0 root         (0) root         (0)    28522 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CON_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26644 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CO_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26642 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/C_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    52623 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CsPbI3-SCAN.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26647 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/PbTe_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    21670 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21687 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt
+-rw-rw-rw-   0 root         (0) root         (0)    37053 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep4_PbTe.txt
+-rw-rw-rw-   0 root         (0) root         (0)   381233 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep4_dipole_Christian.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/update_expted_descriptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5445 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    17089 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_cpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)    11285 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_gpumd_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    17572 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_gpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep3_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep4_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)    14638 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11387 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_nep.py
+-rw-rw-rw-   0 root         (0) root         (0)     5690 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_potential.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_phonons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5360 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_setup_training.py
+-rw-rw-rw-   0 root         (0) root         (0)     6833 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_stiffness.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.495277 calorine-1.6/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    52623 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/CsPbI3-SCAN.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21687 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/PbTe_NEP3.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48216 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/calculators.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    48910 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/elastic_stiffness_tensor.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    44098 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep-graphite.txt
+-rw-rw-rw-   0 root         (0) root         (0)   381233 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep4_dipole.txt
+-rw-rw-rw-   0 root         (0) root         (0)    57668 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep_descriptors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   707350 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep_model_inspection.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.497277 calorine-1.6/tutorials/perovskite-structures/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-cubic-Pm-3m.xyz
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz
+-rw-rw-rw-   0 root         (0) root         (0)   215886 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/phonons.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/prim-graphite.xyz
+-rw-rw-rw-   0 root         (0) root         (0)    35580 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/structure_relaxation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/structure_with_dipole.xyz
+-rw-rw-rw-   0 root         (0) root         (0)   162489 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/thermal_conductivity_from_bte.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   299804 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/visualize_descriptor_space_with_pca.ipynb
```

### Comparing `calorine-1.5/.coveragerc` & `calorine-1.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `calorine-1.5/.gitignore` & `calorine-1.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # data files that should not be included
 log.*
 *.traj
 reference-data/
 *.npy
 benchmark/logs*
 *.fcp
+phono3py_workdir
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `calorine-1.5/.gitlab-ci.yml` & `calorine-1.6/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   tags:
     - linux
     - GPU
   needs:
     - build:linux
   script:
     - cd tutorials
-    - pytest --nbmake --nbmake-timeout=3600 *.ipynb
+    - pytest --nbmake --nbmake-timeout=3600 $(find . -name '*.ipynb' | grep -v thermal_conductivity_from_bte)
 
 test_tutorials:manual:
   extends: .test_tutorials
   when: manual
 
 test_tutorials:schedules:
   extends: .test_tutorials
```

### Comparing `calorine-1.5/CONTRIBUTING.md` & `calorine-1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `calorine-1.5/Dockerfile` & `calorine-1.6/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     pybind11 \
     scikit-learn \
     seekpath
 
 # Packages for building documentation
 RUN \
   pip3 install --upgrade \
+    sphinx==5.3.0 \
     sphinx_autodoc_typehints \
     sphinx-rtd-theme \
     sphinx_sitemap \
     sphinxcontrib-bibtex \
     cloud_sptheme \
     nbsphinx \
   && \
```

### Comparing `calorine-1.5/LICENSE` & `calorine-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calorine-1.5/PKG-INFO` & `calorine-1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: calorine
-Version: 1.5
+Version: 1.6
 Summary: A Python library for building and sampling NEP models via GPUMD simulations.
 Home-page: http://calorine.materialsmodeling.org/
 Author: calorine developer group
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: calorine
         ========
```

### Comparing `calorine-1.5/calorine/calculators/cpunep.py` & `calorine-1.6/calorine/calculators/cpunep.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     -------
 
     >>> calc = CPUNEP('nep.txt')
     >>> atoms.calc = calc
     >>> atoms.get_potential_energy()
     """
 
-    implemented_properties = ['energy', 'energies', 'forces', 'stress']
+    implemented_properties = ['energy', 'energies', 'forces', 'stress', 'dipole']
     debug = False
     nepy = None
 
     def __init__(self,
                  potential_filename: str,
                  atoms: Atoms | None = None,
                  label: str | None = None,
@@ -136,15 +136,15 @@
             self.atoms.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
         self.nepy.set_positions(positions)
 
     def calculate(self,
                   atoms: Atoms = None,
                   properties: List[str] = None,
                   system_changes: List[str] = all_changes):
-        """Calculate energy, per atom energies and forces.
+        """Calculate energy, per atom energies, forces, stress and dipole.
 
         Parameters
         ----------
         atoms : Atoms, optional
             System for which to calculate properties, by default None
         properties : List[str], optional
             Properties to calculate, by default None
@@ -172,10 +172,13 @@
         energies_per_atom = np.array(energies)
         energy = energies_per_atom.sum()
         forces_per_atom = np.array(forces).reshape(-1, self.N_atoms).T
         virials_per_atom = np.array(virials).reshape(-1, self.N_atoms).T
         stress = -(np.sum(virials_per_atom, axis=0) / atoms.get_volume()).reshape((3, 3))
         stress = full_3x3_to_voigt_6_stress(stress)
 
+        dipole = np.array(self.nepy.get_dipole())
+
         self.results['energy'] = energy
         self.results['forces'] = forces_per_atom
         self.results['stress'] = stress
+        self.results['dipole'] = dipole
```

### Comparing `calorine-1.5/calorine/calculators/gpunep.py` & `calorine-1.6/calorine/calculators/gpunep.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/gpumd/io.py` & `calorine-1.6/calorine/gpumd/io.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/nep/__init__.py` & `calorine-1.6/calorine/nep/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 from .io import (read_loss,
                  read_nepfile,
                  read_structures,
                  write_nepfile,
                  write_structures,
                  get_parity_data)
 from .nep import (get_descriptors,
+                  get_dipole,
+                  get_latent_space,
                   get_potential_forces_and_virials)
 from .potential import read_potential
 from .training_factory import setup_training
 
 __all__ = ['read_loss',
            'read_nepfile',
            'read_potential',
            'read_structures',
            'get_parity_data',
            'get_descriptors',
+           'get_dipole',
+           'get_latent_space',
            'get_potential_forces_and_virials',
            'setup_training',
            'write_nepfile',
            'write_structures']
```

### Comparing `calorine-1.5/calorine/nep/io.py` & `calorine-1.6/calorine/nep/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,49 +161,50 @@
     if not exists(path):
         raise ValueError(f'Directory {path} does not exist')
 
     structures = {}
 
     for stype in ['train', 'test']:
         structures[stype] = read(join_path(dirname, f'{stype}.xyz'), format='extxyz', index=':')
-        n_atoms = [len(atom) for atom in structures[stype]]
-        cells = [atom.cell for atom in structures[stype]]
-        n_structures = len(structures[stype])
 
         ts, ps = _read_data_file(path, f'energy_{stype}.out')
+        n_structures = len(structures[stype])
         assert len(ts) == n_structures, \
             f'Number of structures in energy_{stype}.out ({len(ts)})' \
             f' and {stype}.xyz ({n_structures}) inconsistent'
-        for k, t, p in zip(range(n_structures), ts, ps):
-            structures[stype][k].info['energy_target'] = t
-            structures[stype][k].info['energy_predicted'] = p
+        for structure, t, p in zip(structures[stype], ts, ps):
+            structure.info['energy_target'] = t
+            structure.info['energy_predicted'] = p
 
         ts, ps = _read_data_file(path, f'force_{stype}.out')
-        assert len(ts) == sum(n_atoms), \
+        n_atoms_total = sum([len(s) for s in structures[stype]])
+        assert len(ts) == n_atoms_total, \
             f'Number of structures in force_{stype}.out ({len(ts)})' \
             f' and {stype}.xyz ({n_structures}) inconsistent'
         n = 0
-        for k, nat in zip(range(n_structures), n_atoms):
-            structures[stype][k].info['force_target'] = np.array(ts[n:n+nat]).reshape(nat, 3)
-            structures[stype][k].info['force_predicted'] = np.array(ps[n:n+nat]).reshape(nat, 3)
+        for structure in structures[stype]:
+            nat = len(structure)
+            structure.info['force_target'] = np.array(ts[n:n+nat]).reshape(nat, 3)
+            structure.info['force_predicted'] = np.array(ps[n:n+nat]).reshape(nat, 3)
             n += nat
 
         ts, ps = _read_data_file(path, f'virial_{stype}.out')
         assert len(ts) == 6 * n_structures, \
             f'Number of structures in virial_{stype}.out ({len(ts)})' \
             f' and {stype}.xyz ({n_structures}) inconsistent'
         ts = np.array(ts).reshape((6, n_structures)).T
         ps = np.array(ps).reshape((6, n_structures)).T
-        for k, nat, cell, t, p in zip(range(n_structures), n_atoms, cells, ts, ps):
+        for structure, t, p in zip(structures[stype], ts, ps):
             assert np.shape(t) == (6,)
-            structures[stype][k].info['virial_target'] = t
-            structures[stype][k].info['virial_predicted'] = p
-            conv = nat / np.linalg.det(cell) / GPa
-            structures[stype][k].info['stress_target'] = t * conv
-            structures[stype][k].info['stress_predicted'] = p * conv
+            structure.info['virial_target'] = t
+            structure.info['virial_predicted'] = p
+            conv = len(structure) / structure.get_volume() / GPa
+            structure.info['stress_target'] = t * conv
+            structure.info['stress_predicted'] = p * conv
+
     return structures['train'], structures['test']
 
 
 def _read_data_file(dirname: str,
                     fname: str):
     """Private function that parses energy/force/virial_*.out files and
     returns their content for further processing.
```

### Comparing `calorine-1.5/calorine/nep/nep.py` & `calorine-1.6/calorine/nep/nep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import contextlib
 import shutil
 import tempfile
-from typing import List, Tuple
 import warnings
+from typing import List, Tuple, Union, Optional
 import numpy as np
-import _nepy
 from ase import Atoms
+import _nepy
 
 
 def _create_dummy_nep2(potential_filename: str, symbols: List[str]) -> None:
     """Create a dummy NEP2 model, i.e., a model for which there are no descriptor parameters.
     This is to be used when one wants descriptors not pertaining to a specific NEP3 model.
 
     Parameters
@@ -71,14 +71,85 @@
     ----------
     directory
         Path to temporary directory
     """
     shutil.rmtree(directory)
 
 
+def _get_cell_symbols_position(structure: Atoms) -> Tuple[List[float], List[str], List[float]]:
+    """Fetches cell, symbols and positions for a structure. Since NEP_CPU requires a cell, if the
+    structure has no cell a default cubic cell with a side of 100 Å will be used.
+
+    Parameters
+    ----------
+    structure
+        Atoms object representing the structure.
+
+    Returns
+    -------
+    List[float]
+        Cell vectors
+    List[str]
+        Atomic species
+    List[float]
+        Atom positions
+    """
+    if structure.cell.rank == 0:
+        warnings.warn('Using default unit cell (cubic with side 100 Å).')
+        set_default_cell(structure)
+
+    c = structure.get_cell(complete=True).flatten()
+    cell = [c[0], c[3], c[6], c[1], c[4], c[7], c[2], c[5], c[8]]
+
+    symbols = structure.get_chemical_symbols()
+    positions = list(structure.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
+
+    return cell, symbols, positions
+
+
+def _setup_nepy(
+        potential_filename: str,
+        N_atoms: int,
+        cell: List[float],
+        symbols: List[str],
+        positions: List[float],
+        debug: bool) -> _nepy.NEPY:
+    """Sets up an instance of the NEPY pybind11 interface to NEP_CPU.
+
+    Parameters
+    ----------
+    potential_filename
+        Path to potential.
+    N_atoms:
+        Number of atoms in the structure.
+    cell:
+        Cell vectors.
+    symbols:
+        Atom species.
+    positions:
+        Atom positions.
+    debug:
+        Flag to control if the output from NEP_CPU will be printed.
+
+    Returns
+    -------
+    NEPY
+        NEPY interface
+    """
+    # Disable output from C++ code by default
+    if debug:
+        nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
+    else:
+        with open(os.devnull, 'w') as f:
+            with contextlib.redirect_stdout(f):
+                with contextlib.redirect_stderr(f):
+                    nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
+    return nepy
+
+
 def set_default_cell(structure: Atoms, box_length: float = 100):
     """Adds a cubic box to an Atoms object. Atoms object is edited in-place.
 
     Parameters
     ----------
     structure
         Structure to add box to
@@ -86,15 +157,15 @@
         Cubic box side length in Å, by default 100
     """
     structure.set_cell([[box_length, 0, 0], [0, box_length, 0], [0, 0, box_length]])
     structure.center()
 
 
 def get_descriptors(structure: Atoms,
-                    potential_filename: str = None,
+                    potential_filename: Optional[str] = None,
                     debug: bool = False) -> np.ndarray:
     """Calculates the NEP descriptors for a given structure. A NEP model defined by a nep.txt
     can additionally be provided to get the NEP3 model specific descriptors. If no model is
     provided, a dummy NEP2 model suitable for the provided structure will be created and used.
 
     Parameters
     ----------
@@ -104,56 +175,106 @@
         Path to NEP potential. Defaults to None.
     debug
         Flag to toggle debug mode. Makes the generated dummy NEP2 model available
         in a local tmp directory, as well as prints GPUMD output. Defaults to False.
 
     Returns
     -------
-        Descriptors for the supplied structure, with shape (N_atoms, descriptor components)
+    Descriptors for the supplied structure, with shape (N_atoms, descriptor components)
     """
     local_structure = structure.copy()
-    if local_structure.cell.rank == 0:
-        warnings.warn('Using default unit cell (cubic with side 100 Å).')
-        set_default_cell(local_structure)
-
     N_atoms = len(local_structure)
-    c = local_structure.get_cell(complete=True).flatten()
-    cell = [c[0], c[3], c[6], c[1], c[4], c[7], c[2], c[5], c[8]]
-
-    symbols = local_structure.get_chemical_symbols()
-    positions = list(local_structure.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
+    cell, symbols, positions = _get_cell_symbols_position(local_structure)
 
     use_dummy_nep2_potential = potential_filename is None
     if use_dummy_nep2_potential:
         tmp_dir = _create_tmp_dir(debug)
         potential_filename = f'{tmp_dir}/nep.txt'
         _create_dummy_nep2(potential_filename, symbols)
-
-    # Disable output from C++ code by default
-    if debug:
-        nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
     else:
-        with open(os.devnull, 'w') as f:
-            with contextlib.redirect_stdout(f):
-                with contextlib.redirect_stderr(f):
-                    nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
+        tmp_dir = None
 
+    nepy = _setup_nepy(potential_filename, N_atoms, cell, symbols, positions, debug)
     all_descriptors = nepy.get_descriptors()
     descriptors_per_atom = np.array(all_descriptors).reshape(-1, N_atoms).T
 
-    if use_dummy_nep2_potential and not debug:
+    if use_dummy_nep2_potential and tmp_dir and not debug:
         _clean_tmp_dir(tmp_dir)
-    if use_dummy_nep2_potential and debug:
+    if use_dummy_nep2_potential and tmp_dir and debug:
         print(f'DEBUG - Directory containing dummy nep.in: {tmp_dir}')
     return descriptors_per_atom
 
 
+def get_dipole(structure: Atoms,
+               potential_filename: Optional[str] = None,
+               debug: bool = False) -> np.ndarray:
+    """Calculates the dipole for a given structure. A NEP model defined by a
+    `nep.txt` file needs to be provided.
+
+    Parameters
+    ----------
+    structure
+        Input structure
+    potential_filename
+        Path to NEP potential. Defaults to None.
+    debug
+        Flag to toggle debug mode. Prints GPUMD output. Defaults to False.
+
+    Returns
+    -------
+    dipole with shape `(3,)`
+    """
+    if potential_filename is None:
+        raise ValueError('Potential must be defined!')
+    local_structure = structure.copy()
+    N_atoms = len(local_structure)
+    cell, symbols, positions = _get_cell_symbols_position(local_structure)
+
+    nepy = _setup_nepy(potential_filename, N_atoms, cell, symbols, positions, debug)
+    dipole = nepy.get_dipole()
+    return np.array(dipole)
+
+
+def get_latent_space(structure: Atoms,
+                     potential_filename: Union[str, None] = None,
+                     debug: bool = False) -> np.ndarray:
+    """Calculates the latent space representation of a structure, i.e, the activiations in
+    the hidden layer. A NEP model defined by a `nep.txt` file needs to be provided.
+
+    Parameters
+    ----------
+    structure
+        Input structure
+    potential_filename
+        Path to NEP potential. Defaults to None.
+    debug
+        Flag to toggle debug mode. Prints GPUMD output. Defaults to False.
+
+    Returns
+    -------
+    Activation with shape `(N_atoms, N_neurons)`
+    """
+    if potential_filename is None:
+        raise ValueError('Potential must be defined!')
+    local_structure = structure.copy()
+    N_atoms = len(local_structure)
+    cell, symbols, positions = _get_cell_symbols_position(local_structure)
+
+    nepy = _setup_nepy(potential_filename, N_atoms, cell, symbols, positions, debug)
+
+    latent = nepy.get_latent_space()
+    latent = np.array(latent).reshape(N_atoms, -1)
+    return latent
+
+
 def get_potential_forces_and_virials(structure: Atoms,
-                                     potential_filename: str = None,
-                                     debug: bool = False) -> Tuple[np.ndarray]:
+                                     potential_filename: Optional[str] = None,
+                                     debug: bool = False) -> Tuple[np.ndarray,
+                                                                   np.ndarray,
+                                                                   np.ndarray]:
     """Calculates the per-atom potential, forces and virials for a given structure.
     A NEP model defined by a `nep.txt` file needs to be provided.
 
     Parameters
     ----------
     structure
         Input structure
@@ -167,31 +288,16 @@
     potential with shape `(N_atoms,)`
     forces with shape `(N_atoms, 3)`
     virials with shape `(N_atoms, 9)`
     """
     if potential_filename is None:
         raise ValueError('Potential must be defined!')
     local_structure = structure.copy()
-    if local_structure.cell.rank == 0:
-        warnings.warn('Using default unit cell (cubic with side 100 Å).')
-        set_default_cell(local_structure)
-
     N_atoms = len(local_structure)
-    c = local_structure.get_cell(complete=True).flatten()
-    cell = [c[0], c[3], c[6], c[1], c[4], c[7], c[2], c[5], c[8]]
+    cell, symbols, positions = _get_cell_symbols_position(local_structure)
 
-    symbols = local_structure.get_chemical_symbols()
-    positions = list(local_structure.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
-
-    # Disable output from C++ code by default
-    if debug:
-        nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
-    else:
-        with open(os.devnull, 'w') as f:
-            with contextlib.redirect_stdout(f):
-                with contextlib.redirect_stderr(f):
-                    nepy = _nepy.NEPY(potential_filename, N_atoms, cell, symbols, positions)
+    nepy = _setup_nepy(potential_filename, N_atoms, cell, symbols, positions, debug)
 
     energies, forces, virials = nepy.get_potential_forces_and_virials()
     forces_per_atom = np.array(forces).reshape(-1, N_atoms).T
     virials_per_atom = np.array(virials).reshape(-1, N_atoms).T
     return np.array(energies), forces_per_atom, virials_per_atom
```

### Comparing `calorine-1.5/calorine/nep/potential.py` & `calorine-1.6/calorine/nep/potential.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/nep/training_factory.py` & `calorine-1.6/calorine/nep/training_factory.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/tools/__init__.py` & `calorine-1.6/calorine/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/tools/analysis.py` & `calorine-1.6/calorine/tools/analysis.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/tools/phonons.py` & `calorine-1.6/calorine/tools/phonons.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     supercell_matrix
         specification of supercell size handed over to phonopy;
         should be a tuple of three values or a matrix
     kwargs_phonopy
         *Expert option*:
         keyword arguments used when initializing the `Phonopy` object;
         this includes, e.g., the tolerance used when determining the symmetry (`symprec`) and
-        [parameters for the non-analytical
-        corrections](https://phonopy.github.io/phonopy/phonopy-module.html#non-analytical-term-correction)
+        `parameters for the non-analytical corrections
+        <https://phonopy.github.io/phonopy/phonopy-module.html#non-analytical-term-correction>`_
         (`nac_params`)
     kwargs_generate_displacements
         *Expert option*:
         keyword arguments to be handed over to the `generate_displacements` method;
-        this includes in particular the `displacement` keyword, which specifies the
+        this includes in particular the `distance` keyword, which specifies the
         magnitude of the atomic displacement imposed when calculating the force constant matrix
     """
 
     # prepare primitive unit cell for phonopy
     structure_ph = PhonopyAtoms(symbols=structure.symbols,
                                 cell=structure.cell,
                                 scaled_positions=structure.get_scaled_positions(),
```

### Comparing `calorine-1.5/calorine/tools/stiffness.py` & `calorine-1.6/calorine/tools/stiffness.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine/tools/structures.py` & `calorine-1.6/calorine/tools/structures.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/calorine.egg-info/PKG-INFO` & `calorine-1.6/calorine.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: calorine
-Version: 1.5
+Version: 1.6
 Summary: A Python library for building and sampling NEP models via GPUMD simulations.
 Home-page: http://calorine.materialsmodeling.org/
 Author: calorine developer group
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: calorine
         ========
```

### Comparing `calorine-1.5/calorine.egg-info/SOURCES.txt` & `calorine-1.6/calorine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -40,18 +40,20 @@
 doc/_static/custom.css
 doc/_static/logo.ico
 doc/_static/logo.png
 doc/_templates/breadcrumbs.html
 doc/_templates/page.html
 doc/_templates/versions.html
 doc/tutorials/calculators.ipynb
+doc/tutorials/elastic_stiffness_tensor.ipynb
 doc/tutorials/nep_descriptors.ipynb
 doc/tutorials/nep_model_inspection.ipynb
 doc/tutorials/phonons.ipynb
 doc/tutorials/structure_relaxation.ipynb
+doc/tutorials/thermal_conductivity_from_bte.ipynb
 doc/tutorials/visualize_descriptor_space_with_pca.ipynb
 src/nepy/README.md
 src/nepy/nep.cpp
 src/nepy/nep.h
 src/nepy/nepy.cpp
 src/nepy/nepy.h
 tests/test_analysis.py
@@ -73,14 +75,16 @@
 tests/example_files/kappa_nan.out
 tests/example_files/loss.out
 tests/example_files/nep.in
 tests/example_files/nep.txt
 tests/example_files/run.in
 tests/example_files/thermo_ortho_v3.2.out
 tests/example_files/thermo_tri_v3.2.out
+tests/example_files/dipole/dipole_test.out
+tests/example_files/dipole/test.xyz
 tests/example_files/fcp/fcp.txt
 tests/example_files/fcp/fcs_order2.in
 tests/example_files/fcp/r0.in
 tests/example_files/md_no_velocities_or_forces/dump.xyz
 tests/example_files/md_velocities_and_forces/dump.xyz
 tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out
 tests/example_output/CON_NEP2_dummy_CON_3atom_force.out
@@ -110,22 +114,28 @@
 tests/nep_models/C_NEP2_dummy.txt
 tests/nep_models/CsPbI3-SCAN.txt
 tests/nep_models/PbTe_NEP2_dummy.txt
 tests/nep_models/README.md
 tests/nep_models/nep3_v3.2_PbTe_Fan22.txt
 tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt
 tests/nep_models/nep4_PbTe.txt
+tests/nep_models/nep4_dipole_Christian.txt
 tests/nep_models/update_expted_descriptors.py
 tutorials/CsPbI3-SCAN.txt
 tutorials/PbTe_NEP3.txt
 tutorials/calculators.ipynb
 tutorials/elastic_stiffness_tensor.ipynb
+tutorials/nep-graphite.txt
+tutorials/nep4_dipole.txt
 tutorials/nep_descriptors.ipynb
 tutorials/nep_model_inspection.ipynb
 tutorials/phonons.ipynb
+tutorials/prim-graphite.xyz
 tutorials/structure_relaxation.ipynb
+tutorials/structure_with_dipole.xyz
+tutorials/thermal_conductivity_from_bte.ipynb
 tutorials/visualize_descriptor_space_with_pca.ipynb
 tutorials/perovskite-structures/CsPbI3-cubic-Pm-3m.xyz
 tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz
 tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz
 tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz
 tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz
```

### Comparing `calorine-1.5/doc/_static/custom.css` & `calorine-1.6/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/_static/logo.ico` & `calorine-1.6/doc/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/_static/logo.png` & `calorine-1.6/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/_templates/page.html` & `calorine-1.6/doc/_templates/page.html`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/_templates/versions.html` & `calorine-1.6/doc/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/calculators.rst` & `calorine-1.6/doc/calculators.rst`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/conf.py` & `calorine-1.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/index.rst` & `calorine-1.6/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 .. toctree::
    :maxdepth: 2
    :caption: Tutorials
 
    tutorials/calculators
    tutorials/nep_descriptors
    tutorials/nep_model_inspection
+   tutorials/visualize_descriptor_space_with_pca
    tutorials/structure_relaxation
    tutorials/phonons
-   tutorials/visualize_descriptor_space_with_pca
+   tutorials/elastic_stiffness_tensor
+   tutorials/thermal_conductivity_from_bte
 
 .. toctree::
    :maxdepth: 2
    :caption: Function reference
 
    calculators
    gpumd
```

### Comparing `calorine-1.5/doc/installation.rst` & `calorine-1.6/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/tutorials/nep_model_inspection.ipynb` & `calorine-1.6/doc/tutorials/nep_model_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/tutorials/phonons.ipynb` & `calorine-1.6/doc/tutorials/phonons.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976004464285715%*

 * *Differences: {"'cells'": "{0: {'source': ['# Phonon properties']}, 2: {'source': {insert: [(1, 'First, we "*

 * *            'compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> '*

 * *            'described by a neuroevolution potential using the `get_force_constants()` convenience '*

 * *            'function from `calorine`, which wraps functionality from the [phonopy '*

 * *            "package](https://phonopy.github.io/phonopy).\\n'), (2, 'To set the path through the "*

 * *            'Brillouin zone we use the [ […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "6373958f-5692-4b03-8d83-7f01b751bbe5",
             "metadata": {},
             "source": [
-                "# Phonon dispersions and density of states"
+                "# Phonon properties"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "7e813f1b-45db-404e-82eb-eb974b25da0a",
             "metadata": {},
@@ -27,16 +27,16 @@
         },
         {
             "cell_type": "markdown",
             "id": "d089b4ae-a518-4a80-85e8-637dffdc1de8",
             "metadata": {},
             "source": [
                 "In this tutorial we illustrate the calculation of phonon dispersions and densities of states.\n",
-                "First, we compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> described by a neuroevolution potential using the [`get_phonon_dispersion()` convenience function](../tools.html#calorine.tools.get_phonon_dispersion) from `calorine`, which wraps functionality from the [`phonopy` package](https://phonopy.github.io/phonopy/).\n",
-                "To set the path through the Brillouin zone we use the [`seekpath` package](https://www.materialscloud.org/work/tools/seekpath).\n",
+                "First, we compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> described by a neuroevolution potential using the `get_force_constants()` convenience function from `calorine`, which wraps functionality from the [phonopy package](https://phonopy.github.io/phonopy).\n",
+                "To set the path through the Brillouin zone we use the [seekpath package](https://www.materialscloud.org/work/tools/seekpath).\n",
                 "\n",
                 "Then we demonstrate how to use the Python API of `phonopy` directly to compute the phonon density of states."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f2cc4a4a-7e74-47de-9b6d-f66607d89687",
@@ -64,15 +64,15 @@
             "cell_type": "markdown",
             "id": "c2715f08-e76e-4012-b9b9-b08133ceb32e",
             "metadata": {},
             "source": [
                 "## Compute force constants\n",
                 "\n",
                 "Next we prepare the force constants from which we can then obtain, for example, the phonon dispersion and the phonon density of states as shown below.\n",
-                "To this end, we use the [`get_force_constants` function](../tools.html#calorine.tools.get_force_constants).\n",
+                "To this end, we use the `get_force_constants()` function.\n",
                 "Note that the third argument of this function specifies the supercell that is being used for computing the force constant matrix.\n",
                 "Here, we simply use a $2\\times2\\times2$ supercell.\n",
                 "In general you need to ensure that the results are converged with respect to the supercell size."
             ]
         },
         {
             "cell_type": "code",
@@ -85,26 +85,26 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37dc4a23-da5f-4a8a-bb95-01ee5cca3515",
             "metadata": {},
             "source": [
-                "The `get_force_constants` function returns a [`Phonopy` object](https://phonopy.github.io/phonopy/phonopy-module.html), which provides methods for calculating various derived quantities, including but not limited to the phonon dispersion and density of states."
+                "The `get_force_constants` function returns a [Phonopy object](https://phonopy.github.io/phonopy/phonopy-module.html), which provides methods for calculating various derived quantities, including but not limited to the phonon dispersion and density of states."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0c331069-e206-434f-acd0-a5c2b13a58af",
             "metadata": {},
             "source": [
                 "## Phonon dispersion\n",
                 "\n",
                 "We now need to specify the path through the Brillouin zone along which the phonon dispersion is to be calculated.\n",
-                "To this end, we use the [`seekpath` package](https://www.materialscloud.org/work/tools/seekpath), which provides a standardized way for generating such paths.\n",
+                "To this end, we use the [seekpath package](https://www.materialscloud.org/work/tools/seekpath), which provides a standardized way for generating such paths.\n",
                 "It is also possible to set up suitable paths also \"manually\" by stringing together a list of $\\boldsymbol{q}$-points.\n",
                 "\n",
                 "In the following, we first prepare the structure in the format expected by `seekpath` and then call the `get_explicit_k_path` function."
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `calorine-1.5/doc/tutorials/structure_relaxation.ipynb` & `calorine-1.6/doc/tutorials/structure_relaxation.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.5/doc/tutorials/visualize_descriptor_space_with_pca.ipynb` & `calorine-1.6/doc/tutorials/visualize_descriptor_space_with_pca.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Descriptor space analysis\\n')], delete: [0]}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "46ee7988",
             "metadata": {},
             "source": [
-                "# Visualize descriptor space with PCA\n",
+                "# Descriptor space analysis\n",
                 "This notebook demonstrates how to visualize the descriptor space for a collection of structures using principal component Analysis (PCA) as implemented in [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "84538df3",
             "metadata": {},
```

### Comparing `calorine-1.5/setup.py` & `calorine-1.6/setup.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/src/nepy/nep.cpp` & `calorine-1.6/src/nepy/nep.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,40 @@
   f *= d12inv;
   double fc, fcp;
   find_fc_and_fcp_zbl(rc_inner, rc_outer, d12, fc, fcp);
   fp = fp * fc + f * fcp;
   f *= fc;
 }
 
+void find_f_and_fp_zbl(
+  double* zbl_para,
+  double zizj,
+  double a_inv,
+  double rc_inner,
+  double rc_outer,
+  double d12,
+  double d12inv,
+  double& f,
+  double& fp)
+{
+  double x = d12 * a_inv;
+  f = fp = 0.0f;
+  find_phi_and_phip_zbl(zbl_para[0], zbl_para[1], x, f, fp);
+  find_phi_and_phip_zbl(zbl_para[2], zbl_para[3], x, f, fp);
+  find_phi_and_phip_zbl(zbl_para[4], zbl_para[5], x, f, fp);
+  f *= zizj;
+  fp *= zizj * a_inv;
+  fp = fp * d12inv - f * d12inv * d12inv;
+  f *= d12inv;
+  double fc, fcp;
+  find_fc_and_fcp_zbl(rc_inner, rc_outer, d12, fc, fcp);
+  fp = fp * fc + f * fcp;
+  f *= fc;
+}
+
 void find_fn(const int n, const double rcinv, const double d12, const double fc12, double& fn)
 {
   if (n == 0) {
     fn = fc12;
   } else if (n == 1) {
     double x = 2.0 * (d12 * rcinv - 1.0) * (d12 * rcinv - 1.0) - 1.0;
     fn = (x + 1.0) * 0.5 * fc12;
@@ -902,14 +928,15 @@
         g_Fp[d * N + n1] = Fp[d] * paramb.q_scaler[d];
       }
     }
   }
 }
 
 void find_force_radial_small_box(
+  const bool is_dipole,
   NEP3::ParaMB& paramb,
   NEP3::ANN& annmb,
   const int N,
   const int* g_NN,
   const int* g_NL,
   const int* g_type,
   const double* g_x12,
@@ -960,34 +987,42 @@
           double tmp12 = g_Fp[n1 + n * N] * gnp12 * d12inv;
           for (int d = 0; d < 3; ++d) {
             f12[d] += tmp12 * r12[d];
           }
         }
       }
 
-      g_fx[n1] += f12[0];
-      g_fy[n1] += f12[1];
-      g_fz[n1] += f12[2];
-      g_fx[n2] -= f12[0];
-      g_fy[n2] -= f12[1];
-      g_fz[n2] -= f12[2];
-      g_virial[n2 + 0 * N] -= r12[0] * f12[0];
-      g_virial[n2 + 1 * N] -= r12[0] * f12[1];
-      g_virial[n2 + 2 * N] -= r12[0] * f12[2];
-      g_virial[n2 + 3 * N] -= r12[1] * f12[0];
-      g_virial[n2 + 4 * N] -= r12[1] * f12[1];
-      g_virial[n2 + 5 * N] -= r12[1] * f12[2];
-      g_virial[n2 + 6 * N] -= r12[2] * f12[0];
-      g_virial[n2 + 7 * N] -= r12[2] * f12[1];
-      g_virial[n2 + 8 * N] -= r12[2] * f12[2];
+      if (!is_dipole) {
+        g_fx[n1] += f12[0];
+        g_fy[n1] += f12[1];
+        g_fz[n1] += f12[2];
+        g_fx[n2] -= f12[0];
+        g_fy[n2] -= f12[1];
+        g_fz[n2] -= f12[2];
+        g_virial[n2 + 0 * N] -= r12[0] * f12[0];
+        g_virial[n2 + 1 * N] -= r12[0] * f12[1];
+        g_virial[n2 + 2 * N] -= r12[0] * f12[2];
+        g_virial[n2 + 3 * N] -= r12[1] * f12[0];
+        g_virial[n2 + 4 * N] -= r12[1] * f12[1];
+        g_virial[n2 + 5 * N] -= r12[1] * f12[2];
+        g_virial[n2 + 6 * N] -= r12[2] * f12[0];
+        g_virial[n2 + 7 * N] -= r12[2] * f12[1];
+        g_virial[n2 + 8 * N] -= r12[2] * f12[2];
+      } else {
+        double r12_square = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
+        g_virial[n2 + 0 * N] -= r12_square * f12[0];
+        g_virial[n2 + 1 * N] -= r12_square * f12[1];
+        g_virial[n2 + 2 * N] -= r12_square * f12[2];
+      }
     }
   }
 }
 
 void find_force_angular_small_box(
+  const bool is_dipole,
   NEP3::ParaMB& paramb,
   NEP3::ANN& annmb,
   const int N,
   const int* g_NN_angular,
   const int* g_NL_angular,
   const int* g_type,
   const double* g_x12,
@@ -1058,29 +1093,37 @@
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           } else {
             accumulate_f12_with_5body(
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           }
         }
       }
-      g_fx[n1] += f12[0];
-      g_fy[n1] += f12[1];
-      g_fz[n1] += f12[2];
-      g_fx[n2] -= f12[0];
-      g_fy[n2] -= f12[1];
-      g_fz[n2] -= f12[2];
-      g_virial[n2 + 0 * N] -= r12[0] * f12[0];
-      g_virial[n2 + 1 * N] -= r12[0] * f12[1];
-      g_virial[n2 + 2 * N] -= r12[0] * f12[2];
-      g_virial[n2 + 3 * N] -= r12[1] * f12[0];
-      g_virial[n2 + 4 * N] -= r12[1] * f12[1];
-      g_virial[n2 + 5 * N] -= r12[1] * f12[2];
-      g_virial[n2 + 6 * N] -= r12[2] * f12[0];
-      g_virial[n2 + 7 * N] -= r12[2] * f12[1];
-      g_virial[n2 + 8 * N] -= r12[2] * f12[2];
+
+      if (!is_dipole) {
+        g_fx[n1] += f12[0];
+        g_fy[n1] += f12[1];
+        g_fz[n1] += f12[2];
+        g_fx[n2] -= f12[0];
+        g_fy[n2] -= f12[1];
+        g_fz[n2] -= f12[2];
+        g_virial[n2 + 0 * N] -= r12[0] * f12[0];
+        g_virial[n2 + 1 * N] -= r12[0] * f12[1];
+        g_virial[n2 + 2 * N] -= r12[0] * f12[2];
+        g_virial[n2 + 3 * N] -= r12[1] * f12[0];
+        g_virial[n2 + 4 * N] -= r12[1] * f12[1];
+        g_virial[n2 + 5 * N] -= r12[1] * f12[2];
+        g_virial[n2 + 6 * N] -= r12[2] * f12[0];
+        g_virial[n2 + 7 * N] -= r12[2] * f12[1];
+        g_virial[n2 + 8 * N] -= r12[2] * f12[2];
+      } else {
+        double r12_square = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
+        g_virial[n2 + 0 * N] -= r12_square * f12[0];
+        g_virial[n2 + 1 * N] -= r12_square * f12[1];
+        g_virial[n2 + 2 * N] -= r12_square * f12[2];
+      }
     }
   }
 }
 
 void find_force_ZBL_small_box(
   const int N,
   const NEP3::ZBL& zbl,
@@ -1093,27 +1136,48 @@
   double* g_fx,
   double* g_fy,
   double* g_fz,
   double* g_virial,
   double* g_pe)
 {
   for (int n1 = 0; n1 < N; ++n1) {
-    double zi = zbl.atomic_numbers[g_type[n1]];
+    int type1 = g_type[n1];
+    double zi = zbl.atomic_numbers[type1];
     double pow_zi = pow(zi, 0.23);
     for (int i1 = 0; i1 < g_NN[n1]; ++i1) {
       int index = i1 * N + n1;
       int n2 = g_NL[index];
       double r12[3] = {g_x12[index], g_y12[index], g_z12[index]};
       double d12 = sqrt(r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2]);
       double d12inv = 1.0 / d12;
       double f, fp;
-      double zj = zbl.atomic_numbers[g_type[n2]];
+      int type2 = g_type[n2];
+      double zj = zbl.atomic_numbers[type2];
       double a_inv = (pow_zi + pow(zj, 0.23)) * 2.134563;
       double zizj = K_C_SP * zi * zj;
-      find_f_and_fp_zbl(zizj, a_inv, zbl.rc_inner, zbl.rc_outer, d12, d12inv, f, fp);
+      if (zbl.flexibled) {
+        int t1, t2;
+        if (type1 < type2) {
+          t1 = type1;
+          t2 = type2;
+        } else {
+          t1 = type2;
+          t2 = type1;
+        }
+        int zbl_index = t1 * zbl.num_types - (t1 * (t1 - 1)) / 2 + (t2 - t1);
+        double rc_inner = zbl.rc_flexible_inner[zbl_index];
+        double rc_outer = zbl.rc_flexible_outer[zbl_index];
+        double ZBL_para[6];
+        for (int i = 0; i < 6; ++i) {
+          ZBL_para[i] = zbl.para[6 * zbl_index + i];
+        }
+        find_f_and_fp_zbl(ZBL_para, zizj, a_inv, rc_inner, rc_outer, d12, d12inv, f, fp);
+      } else {
+        find_f_and_fp_zbl(zizj, a_inv, zbl.rc_inner, zbl.rc_outer, d12, d12inv, f, fp);
+      }
       double f2 = fp * d12inv * 0.5;
       double f12[3] = {r12[0] * f2, r12[1] * f2, r12[2] * f2};
       g_fx[n1] += f12[0];
       g_fy[n1] += f12[1];
       g_fz[n1] += f12[2];
       g_fx[n2] -= f12[0];
       g_fy[n2] -= f12[1];
@@ -1474,33 +1538,55 @@
   double g_total_virial[6],
   double** g_virial,
   double& g_total_potential,
   double* g_potential)
 {
   for (int ii = 0; ii < N; ++ii) {
     int n1 = g_ilist[ii];
-    double zi = zbl.atomic_numbers[g_type[n1] - 1]; // from LAMMPS to NEP convention
+    int type1 = g_type[n1] - 1;
+    double zi = zbl.atomic_numbers[type1]; // from LAMMPS to NEP convention
     double pow_zi = pow(zi, 0.23);
     for (int i1 = 0; i1 < g_NN[n1]; ++i1) {
       int n2 = g_NL[n1][i1];
       double r12[3] = {
         g_pos[n2][0] - g_pos[n1][0], g_pos[n2][1] - g_pos[n1][1], g_pos[n2][2] - g_pos[n1][2]};
 
       double d12sq = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
-      if (d12sq >= zbl.rc_outer * zbl.rc_outer) {
+      double max_rc_outer = 2.5;
+      if (d12sq >= max_rc_outer * max_rc_outer) {
         continue;
       }
       double d12 = sqrt(d12sq);
 
       double d12inv = 1.0 / d12;
       double f, fp;
-      double zj = zbl.atomic_numbers[g_type[n2] - 1]; // from LAMMPS to NEP convention
+      int type2 = g_type[n2] - 1;
+      double zj = zbl.atomic_numbers[type2]; // from LAMMPS to NEP convention
       double a_inv = (pow_zi + pow(zj, 0.23)) * 2.134563;
       double zizj = K_C_SP * zi * zj;
-      find_f_and_fp_zbl(zizj, a_inv, zbl.rc_inner, zbl.rc_outer, d12, d12inv, f, fp);
+      if (zbl.flexibled) {
+        int t1, t2;
+        if (type1 < type2) {
+          t1 = type1;
+          t2 = type2;
+        } else {
+          t1 = type2;
+          t2 = type1;
+        }
+        int zbl_index = t1 * zbl.num_types - (t1 * (t1 - 1)) / 2 + (t2 - t1);
+        double rc_inner = zbl.rc_flexible_inner[zbl_index];
+        double rc_outer = zbl.rc_flexible_outer[zbl_index];
+        double ZBL_para[6];
+        for (int i = 0; i < 6; ++i) {
+          ZBL_para[i] = zbl.para[6 * zbl_index + i];
+        }
+        find_f_and_fp_zbl(ZBL_para, zizj, a_inv, rc_inner, rc_outer, d12, d12inv, f, fp);
+      } else {
+        find_f_and_fp_zbl(zizj, a_inv, zbl.rc_inner, zbl.rc_outer, d12, d12inv, f, fp);
+      }
       double f2 = fp * d12inv * 0.5;
       double f12[3] = {r12[0] * f2, r12[1] * f2, r12[2] * f2};
       g_force[n1][0] += f12[0]; // accumulation here
       g_force[n1][1] += f12[1];
       g_force[n1][2] += f12[2];
       g_force[n2][0] -= f12[0];
       g_force[n2][1] -= f12[1];
@@ -1710,15 +1796,15 @@
     std::istream_iterator<std::string>{iss}, std::istream_iterator<std::string>{}};
   return tokens;
 }
 
 void print_tokens(const std::vector<std::string>& tokens)
 {
   std::cout << "Line:";
-  for(const auto& token : tokens) {
+  for (const auto& token : tokens) {
     std::cout << " " << token;
   }
   std::cout << std::endl;
 }
 
 int get_int_from_token(const std::string& token, const char* filename, const int line)
 {
@@ -1793,15 +1879,15 @@
   paramb.num_types = get_int_from_token(tokens[1], __FILE__, __LINE__);
   if (tokens.size() != 2 + paramb.num_types) {
     print_tokens(tokens);
     std::cout << "The first line of nep.txt should have " << paramb.num_types << " atom symbols."
               << std::endl;
     exit(1);
   }
-  
+
   element_list.resize(paramb.num_types);
   for (int n = 0; n < paramb.num_types; ++n) {
     int atomic_number = 0;
     element_list[n] = tokens[2 + n];
     for (int m = 0; m < NUM_ELEMENTS; ++m) {
       if (tokens[2 + n] == ELEMENTS[m]) {
         atomic_number = m + 1;
@@ -1817,14 +1903,17 @@
     if (tokens.size() != 3) {
       print_tokens(tokens);
       std::cout << "This line should be zbl rc_inner rc_outer." << std::endl;
       exit(1);
     }
     zbl.rc_inner = get_double_from_token(tokens[1], __FILE__, __LINE__);
     zbl.rc_outer = get_double_from_token(tokens[2], __FILE__, __LINE__);
+    if (zbl.rc_inner == 0 && zbl.rc_outer == 0) {
+      zbl.flexibled = true;
+    }
   }
 
   // cutoff 4.2 3.7 80 47
   tokens = get_tokens(input);
   if (tokens.size() != 3 && tokens.size() != 5) {
     print_tokens(tokens);
     std::cout << "This line should be cutoff rc_radial rc_angular [MN_radial] [MN_angular].\n";
@@ -1861,15 +1950,15 @@
   if (paramb.version == 2) {
     if (tokens.size() != 2) {
       print_tokens(tokens);
       std::cout << "This line should be l_max l_max_3body." << std::endl;
       exit(1);
     }
   } else {
-    if (tokens.size() != 4) { 
+    if (tokens.size() != 4) {
       print_tokens(tokens);
       std::cout << "This line should be l_max l_max_3body l_max_4body l_max_5body." << std::endl;
       exit(1);
     }
   }
 
   paramb.L_max = get_int_from_token(tokens[1], __FILE__, __LINE__);
@@ -1926,34 +2015,56 @@
   }
   update_potential(parameters.data(), annmb);
   for (int d = 0; d < annmb.dim; ++d) {
     tokens = get_tokens(input);
     paramb.q_scaler[d] = get_double_from_token(tokens[0], __FILE__, __LINE__);
   }
 
+  // flexible zbl potential parameters if (zbl.flexibled)
+  if (zbl.flexibled) {
+    int num_type_zbl = (paramb.num_types * (paramb.num_types + 1)) / 2;
+    for (int d = 0; d < num_type_zbl; ++d) {
+      tokens = get_tokens(input);
+      zbl.rc_flexible_inner[d] = get_double_from_token(tokens[0], __FILE__, __LINE__);
+    }
+    for (int d = 0; d < num_type_zbl; ++d) {
+      tokens = get_tokens(input);
+      zbl.rc_flexible_outer[d] = get_double_from_token(tokens[0], __FILE__, __LINE__);
+    }
+    for (int d = 0; d < 6 * num_type_zbl; ++d) {
+      tokens = get_tokens(input);
+      zbl.para[d] = get_double_from_token(tokens[0], __FILE__, __LINE__);
+    }
+    zbl.num_types = paramb.num_types;
+  }
   input.close();
 
   // only report for rank_0
   if (is_rank_0) {
 
     if (paramb.num_types == 1) {
       std::cout << "Use the NEP" << paramb.version << " potential with " << paramb.num_types
                 << " atom type.\n";
     } else {
       std::cout << "Use the NEP" << paramb.version << " potential with " << paramb.num_types
                 << " atom types.\n";
     }
 
     for (int n = 0; n < paramb.num_types; ++n) {
-      std::cout << "    type " << n << "( " << element_list[n] << " with Z = " << zbl.atomic_numbers[n] << ").\n";
+      std::cout << "    type " << n << "( " << element_list[n]
+                << " with Z = " << zbl.atomic_numbers[n] << ").\n";
     }
 
     if (zbl.enabled) {
-      std::cout << "    has ZBL with inner cutoff " << zbl.rc_inner << " A and outer cutoff "
-                << zbl.rc_outer << " A.\n";
+      if (zbl.flexibled) {
+        std::cout << "    has flexible ZBL.\n";
+      } else {
+        std::cout << "    has universal ZBL with inner cutoff " << zbl.rc_inner
+                  << " A and outer cutoff " << zbl.rc_outer << " A.\n";
+      }
     }
     std::cout << "    radial cutoff = " << paramb.rc_radial << " A.\n";
     std::cout << "    angular cutoff = " << paramb.rc_angular << " A.\n";
     std::cout << "    n_max_radial = " << paramb.n_max_radial << ".\n";
     std::cout << "    n_max_angular = " << paramb.n_max_angular << ".\n";
     if (paramb.version >= 3) {
       std::cout << "    basis_size_radial = " << paramb.basis_size_radial << ".\n";
@@ -2049,22 +2160,22 @@
   find_descriptor_small_box(
     true, false, false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
     r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
     sum_fxyz.data(), potential.data(), nullptr, nullptr);
 
   find_force_radial_small_box(
-    paramb, annmb, N, NN_radial.data(), NL_radial.data(), type.data(), r12.data(),
+    false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), type.data(), r12.data(),
     r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(), force.data(), force.data() + N,
     force.data() + N * 2, virial.data());
 
   find_force_angular_small_box(
-    paramb, annmb, N, NN_angular.data(), NL_angular.data(), type.data(), r12.data() + size_x12 * 3,
-    r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(), sum_fxyz.data(), force.data(),
-    force.data() + N, force.data() + N * 2, virial.data());
+    false, paramb, annmb, N, NN_angular.data(), NL_angular.data(), type.data(),
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
+    sum_fxyz.data(), force.data(), force.data() + N, force.data() + N * 2, virial.data());
 
   if (zbl.enabled) {
     find_force_ZBL_small_box(
       N, zbl, NN_angular.data(), NL_angular.data(), type.data(), r12.data() + size_x12 * 3,
       r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, force.data(), force.data() + N,
       force.data() + N * 2, virial.data(), potential.data());
   }
@@ -2128,14 +2239,67 @@
   find_descriptor_small_box(
     false, false, true, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
     r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
     sum_fxyz.data(), nullptr, nullptr, latent_space.data());
 }
 
+void NEP3::find_dipole(
+  const std::vector<int>& type,
+  const std::vector<double>& box,
+  const std::vector<double>& position,
+  std::vector<double>& dipole)
+{
+  const int N = type.size();
+  const int size_x12 = N * MN;
+
+  if (N * 3 != position.size()) {
+    std::cout << "Type and position sizes are inconsistent.\n";
+    exit(1);
+  }
+
+  allocate_memory(N);
+  std::vector<double> potential(N);  // not used but needed for find_descriptor_small_box
+  std::vector<double> virial(N * 3); // need the 3 diagonal components only
+
+  for (int n = 0; n < potential.size(); ++n) {
+    potential[n] = 0.0;
+  }
+  for (int n = 0; n < virial.size(); ++n) {
+    virial[n] = 0.0;
+  }
+
+  find_neighbor_list_small_box(
+    paramb.rc_radial, paramb.rc_angular, N, box, position, num_cells, ebox, NN_radial, NL_radial,
+    NN_angular, NL_angular, r12);
+
+  find_descriptor_small_box(
+    true, false, false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
+    NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
+    sum_fxyz.data(), potential.data(), nullptr, nullptr);
+
+  find_force_radial_small_box(
+    true, paramb, annmb, N, NN_radial.data(), NL_radial.data(), type.data(), r12.data(),
+    r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(), nullptr, nullptr, nullptr,
+    virial.data());
+
+  find_force_angular_small_box(
+    true, paramb, annmb, N, NN_angular.data(), NL_angular.data(), type.data(),
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
+    sum_fxyz.data(), nullptr, nullptr, nullptr, virial.data());
+
+  for (int d = 0; d < 3; ++d) {
+    dipole[d] = 0.0;
+    for (int n = 0; n < N; ++n) {
+      dipole[d] += virial[d * N + n];
+    }
+  }
+}
+
 void NEP3::compute_for_lammps(
   int N,
   int* ilist,
   int* NN,
   int** NL,
   int* type,
   double** pos,
```

### Comparing `calorine-1.5/src/nepy/nep.h` & `calorine-1.6/src/nepy/nep.h`

 * *Files 6% similar despite different names*

```diff
@@ -39,26 +39,31 @@
     double q_scaler[140];
   };
 
   struct ANN {
     int dim = 0;
     int num_neurons1 = 0;
     int num_para = 0;
-    const double* w0[100];
-    const double* b0[100];
-    const double* w1[100];
+    const double* w0[103];
+    const double* b0[103];
+    const double* w1[103];
     const double* b1;
     const double* c;
   };
 
   struct ZBL {
     bool enabled = false;
+    bool flexibled = false;
+    int num_types;
     double rc_inner = 1.0;
     double rc_outer = 2.0;
-    double atomic_numbers[10];
+    double atomic_numbers[103];
+    double rc_flexible_inner[55];
+    double rc_flexible_outer[55];
+    double para[330];
   };
 
   NEP3();
   NEP3(const std::string& potential_filename);
 
   void init_from_file(const std::string& potential_filename, const bool is_rank_0);
 
@@ -88,14 +93,21 @@
 
   void find_latent_space(
     const std::vector<int>& type,
     const std::vector<double>& box,
     const std::vector<double>& position,
     std::vector<double>& latent_space);
 
+  void find_dipole(
+    const std::vector<int>& type,
+    const std::vector<double>& box,
+    const std::vector<double>& position,
+    std::vector<double>& dipole // 3 components, for the whole box
+  );
+
   void compute_for_lammps(
     int inum,                // list->inum
     int* ilist,              // list->ilist
     int* numneigh,           // list->numneigh
     int** firstneigh,        // list->firstneigh
     int* type,               // atom->type
     double** x,              // atom->x
```

### Comparing `calorine-1.5/src/nepy/nepy.h` & `calorine-1.6/src/nepy/nepy.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "nep.h"
+using namespace std;
 
 // Local struct to hold an atomic configuration.
 struct Atom
 {
     int N;
     std::vector<int> type;
     std::vector<double> cell, position;
@@ -14,14 +15,16 @@
     NEP3 nep;
     struct Atom atom;
     std::string potential_filename;
 
 public:
     NEPY(const std::string &potential_filename, int N_atoms, std::vector<double> box, std::vector<std::string> atom_symbols, std::vector<double> positions);
     std::vector<double> getDescriptors();
+    std::vector<double> getDipole();
+    std::vector<double> getLatentSpace();
     std::tuple<std::vector<double>, std::vector<double>, std::vector<double>> getPotentialForcesAndVirials();
     std::vector<std::string> _getAtomSymbols(std::string potential_filename);
     void _convertAtomTypeNEPIndex(int N, std::vector<std::string> atom_symbols, std::vector<std::string> model_atom_symbols, std::vector<int> &type);
     void setPositions(std::vector<double> positions);
     void setCell(std::vector<double> cell);
     void setSymbols(std::vector<std::string> atom_symbols);
-};
+};
```

### Comparing `calorine-1.5/tests/example_files/fcp/fcs_order2.in` & `calorine-1.6/tests/example_files/fcp/fcs_order2.in`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/fcp/r0.in` & `calorine-1.6/tests/example_files/fcp/r0.in`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/hac.out` & `calorine-1.6/tests/example_files/hac.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/hac_nan.out` & `calorine-1.6/tests/example_files/hac_nan.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/kappa.out` & `calorine-1.6/tests/example_files/kappa.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/loss.out` & `calorine-1.6/tests/example_files/loss.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/md_no_velocities_or_forces/dump.xyz` & `calorine-1.6/tests/example_files/md_no_velocities_or_forces/dump.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/md_velocities_and_forces/dump.xyz` & `calorine-1.6/tests/example_files/md_velocities_and_forces/dump.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/nep.txt` & `calorine-1.6/tests/example_files/nep.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/thermo_ortho_v3.2.out` & `calorine-1.6/tests/example_files/thermo_ortho_v3.2.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_files/thermo_tri_v3.2.out` & `calorine-1.6/tests/example_files/thermo_tri_v3.2.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out` & `calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out` & `calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out` & `calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out` & `calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out` & `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out` & `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out` & `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out` & `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/example_structures/PbTe_250atom.in` & `calorine-1.6/tests/example_structures/PbTe_250atom.in`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/CON_NEP2_dummy.txt` & `calorine-1.6/tests/nep_models/CON_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/CO_NEP2_dummy.txt` & `calorine-1.6/tests/nep_models/CO_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/C_NEP2_dummy.txt` & `calorine-1.6/tests/nep_models/C_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/CsPbI3-SCAN.txt` & `calorine-1.6/tests/nep_models/CsPbI3-SCAN.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/PbTe_NEP2_dummy.txt` & `calorine-1.6/tests/nep_models/PbTe_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt` & `calorine-1.6/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt` & `calorine-1.6/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/nep4_PbTe.txt` & `calorine-1.6/tests/nep_models/nep4_PbTe.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/nep_models/update_expted_descriptors.py` & `calorine-1.6/tests/nep_models/update_expted_descriptors.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_analysis.py` & `calorine-1.6/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_cpunep.py` & `calorine-1.6/tests/test_cpunep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,56 @@
 import contextlib
 import numpy as np
 import pytest
 from ase import Atoms
+from ase.io import read
 from ase.build import bulk
 from ase.stress import full_3x3_to_voigt_6_stress
 from ase.db import connect
 from calorine.calculators import CPUNEP, GPUNEP
 
 
 # Use same volume as in PbTe_2atom.in, C_2atom.in etc.
 vacuum_cell = ([100, 0, 0], [0, 100, 0], [0, 0, 100])
-PbTe = Atoms('TePb', positions=[(0, 0, 0), (0, 0.0, 1.1)],
-             cell=vacuum_cell)
-C = Atoms('C', positions=[(0, 0, 0)],
-          cell=vacuum_cell)
-CO = Atoms('CO', positions=[(0, 0, 0), (0, 0.0, 1.1)],
-           cell=vacuum_cell)
-CC = Atoms('CC', positions=[(0, 0, 0), (0, 0.0, 1.1)],
-           cell=vacuum_cell)
-CON = Atoms('CON', positions=[(0, 0, 0), (0, 0.0, 1.1), (0, 0.0, 2.2)],
-            cell=vacuum_cell)
-PbTeBulk = bulk('PbTe', crystalstructure='rocksalt', a=4)
-PbTeBulk[0].position += np.array([0.03, 0.02, 0])
+
+
+@pytest.fixture
+def PbTe():
+    return Atoms('TePb', positions=[(0, 0, 0), (0, 0.0, 1.1)],
+                 cell=vacuum_cell)
+
+
+@pytest.fixture
+def C():
+    return Atoms('C', positions=[(0, 0, 0)], cell=vacuum_cell)
+
+
+@pytest.fixture
+def CC():
+    return Atoms('CC', positions=[(0, 0, 0), (0, 0.0, 1.1)],
+                 cell=vacuum_cell)
+
+
+@pytest.fixture
+def CO():
+    return Atoms('CO', positions=[(0, 0, 0), (0, 0.0, 1.1)],
+                 cell=vacuum_cell)
+
+
+@pytest.fixture
+def CON():
+    return Atoms('CON', positions=[(0, 0, 0), (0, 0.0, 1.1), (0, 0.0, 2.2)],
+                 cell=vacuum_cell)
+
+
+@pytest.fixture
+def PbTeBulk():
+    PbTeBulk = bulk('PbTe', crystalstructure='rocksalt', a=4)
+    PbTeBulk[0].position += np.array([0.03, 0.02, 0])
+    return PbTeBulk
 
 
 @pytest.fixture
 def NEP3CPUNEP():
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
     return calc
@@ -40,15 +65,15 @@
     stress = (np.sum(-np.loadtxt(path), axis=0) / volume).reshape((3, 3))
     if voigt:
         return full_3x3_to_voigt_6_stress(stress)
     return stress
 
 
 # --- get_potential_forces_and_virials ---
-def test_get_potential_forces_and_stress_NEP3():
+def test_get_potential_forces_and_stress_NEP3(PbTe):
     """NEP3 model supplied. Compares results to output from `nep_cpu`"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
     PbTe.calc = calc
     energy = PbTe.get_potential_energy()
     forces = PbTe.get_forces()
     stress = PbTe.get_stress()
@@ -62,15 +87,15 @@
     assert forces.shape == (2, 3)
     assert stress.shape == (6,)
     assert np.allclose(forces[0, :], -forces[1, :], atol=1e-12, rtol=0)  # Newton III
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_set_atoms_constructor():
+def test_get_potential_forces_and_stress_set_atoms_constructor(PbTe):
     """Set atoms directly when creating the calculator"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     CPUNEP(nep3, atoms=PbTe)
     energy = PbTe.get_potential_energy()
     forces = PbTe.get_forces()
     stress = PbTe.get_stress()
 
@@ -83,15 +108,15 @@
     assert forces.shape == (2, 3)
     assert stress.shape == (6,)
     assert np.allclose(forces[0, :], -forces[1, :], atol=1e-12, rtol=0)  # Newton III
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_set_atoms_calculate():
+def test_get_potential_forces_and_stress_set_atoms_calculate(PbTe):
     """Set atoms directly when calling calculate on the calculator"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
     calc.calculate(atoms=PbTe)
     results = calc.results
     energy = results['energy']
     forces, stress = results['forces'], results['stress']
@@ -105,15 +130,15 @@
     assert forces.shape == (2, 3)
     assert stress.shape == (6, )
     assert np.allclose(forces[0, :], -forces[1, :], atol=1e-12, rtol=0)  # Newton III
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_NEP3_debug(tmpdir):
+def test_get_potential_forces_and_stress_NEP3_debug(tmpdir, PbTe):
     """Compares result with debug flag enabled."""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3, debug=True)
     p = tmpdir.join('nep_out.tmp')
     with open(p, 'w') as f:
         with contextlib.redirect_stdout(f):
             with contextlib.redirect_stderr(f):
@@ -123,28 +148,28 @@
                 PbTe.get_stress()
     with open(p, 'r') as f:
         lines = p.readlines()
         assert lines[0] == 'Use the NEP3 potential with 2 atom types.\n'
         assert len(lines) == 16
 
 
-def test_get_tress_non_voigt_NEP3():
+def test_get_tress_non_voigt_NEP3(PbTe):
     """NEP3 model supplied. Compares results to output from `nep_cpu`"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
     PbTe.calc = calc
     stress = PbTe.get_stress(voigt=False)
     expected_stress = get_expected_stress(
         'tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_virial.out', voigt=False)
 
     assert stress.shape == (3, 3)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_dummy_NEP2():
+def test_get_potential_forces_and_stress_dummy_NEP2(CO):
     """Dummy NEP2 model supplied. Compares results to output from `nep_cpu` for another system"""
     nep2 = 'tests/nep_models/CO_NEP2_dummy.txt'
     calc = CPUNEP(nep2)
     CO.calc = calc
     energy = CO.get_potential_energy()
     forces = CO.get_forces()
     stress = CO.get_stress()
@@ -158,15 +183,15 @@
     assert forces.shape == (2, 3)
     assert stress.shape == (6,)
     assert np.allclose(forces[0, :], -forces[1, :], atol=1e-12, rtol=0)  # Newton III
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_several_different_species():
+def test_get_potential_forces_and_stress_several_different_species(CON):
     """Check that forces and stress are correct for a CON system.
     Note that these forces/stress should be exactly zero for this system
     since the NEP2 dummy potential treats all atom species as identical atm."""
     nep2 = 'tests/nep_models/CON_NEP2_dummy.txt'
     calc = CPUNEP(nep2)
     CON.calc = calc
     energy = CON.get_potential_energy()
@@ -184,15 +209,15 @@
     assert np.allclose(forces[0, :], -forces[1, :], atol=1e-12, rtol=0)  # Newton III
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(forces, np.zeros((3, 3)), atol=1e-12, rtol=0)
     assert np.allclose(stress, expected_stress, atol=1e-12, rtol=0)
     assert np.allclose(stress, np.zeros((6,)), atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_dummy_NEP2_independent_of_species():
+def test_get_potential_forces_and_stress_dummy_NEP2_independent_of_species(PbTe, CO):
     """Dummy NEP2 energies, forces and stress should be independent of atom species"""
     nep2 = 'tests/nep_models/PbTe_NEP2_dummy.txt'
     calc = CPUNEP(nep2)
     PbTe.calc = calc
     PbTe_energy = PbTe.get_potential_energy()
     PbTe_forces = PbTe.get_forces()
     PbTe_stress = PbTe.get_stress()
@@ -212,15 +237,15 @@
     assert np.allclose(PbTe_energy, CO_energy, atol=1e-12, rtol=0)
     assert np.allclose(PbTe_forces, CO_forces, atol=1e-12, rtol=0)
     assert np.allclose(PbTe_stress, CO_stress, atol=1e-12, rtol=0)
     assert np.allclose(CO_forces, expected_forces_CO, atol=1e-12, rtol=0)
     assert np.allclose(CO_stress, expected_stress_CO, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_stress_update_positions():
+def test_get_potential_forces_and_stress_update_positions(PbTe):
     """Update the positions and make sure that the energies, forces and stress are also updated"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
 
     copy = PbTe.copy()
     copy.calc = calc
     energy_initial = copy.get_potential_energy()
@@ -238,15 +263,15 @@
     diff_stress = stress_initial - stress_after
 
     assert np.isclose(diff_energy, 1.80751674, atol=1e-12, rtol=1e-6)
     assert np.allclose(diff_force, [[0, 0, 4.65672972], [0, 0, -4.65672972]], atol=1e-12, rtol=1e-6)
     assert np.allclose(diff_stress, [0, 0, 7.13057884e-06, 0, 0, 0], atol=1e-12, rtol=1e-6)
 
 
-def test_get_potential_forces_and_stress_update_cell():
+def test_get_potential_forces_and_stress_update_cell(PbTe):
     """Update the cell and make sure that the energies, forces and stress are still the same"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
 
     copy = PbTe.copy()
     copy.calc = calc
     energy_initial = copy.get_potential_energy()
@@ -264,15 +289,15 @@
     stress_after = copy.get_stress()
 
     assert np.isclose(energy_initial, energy_after, atol=1e-12, rtol=1e-6)
     assert np.allclose(forces_initial, forces_after, atol=1e-12, rtol=1e-6)
     assert np.allclose(stress_initial, stress_after / volume_factor, atol=1e-12, rtol=1e-6)
 
 
-def test_get_potential_forces_and_stress_update_numbers():
+def test_get_potential_forces_and_stress_update_numbers(PbTe):
     """Update the atom numbers (species) and make sure that the
     energies, forces and stress are also updated.
     """
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
 
     copy = PbTe.copy()
@@ -292,15 +317,15 @@
     diff_force = forces_initial - forces_after
     diff_stress = stress_initial - stress_after
     assert np.isclose(diff_energy, 1.86577361, atol=1e-12, rtol=1e-6)
     assert np.allclose(diff_force, [[0, 0, 1.07038059], [0, 0, -1.07038059]], atol=1e-12, rtol=1e-6)
     assert np.allclose(diff_stress, [0, 0, 1.17741865e-06, 0, 0, 0], atol=1e-12, rtol=1e-6)
 
 
-def test_reset_calculator_on_atoms_change():
+def test_reset_calculator_on_atoms_change(PbTe):
     """Reset the calculator when changing the system.
     """
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
 
     copy = PbTe.copy()
     copy.calc = calc
@@ -313,15 +338,15 @@
     original_cell = copy.cell.copy()
     atoms_copy.calc = calc
 
     assert calc.results == {}
     assert calc.nepy is None
 
     # Scale cell
-    atoms_copy.set_cell(1.1*original_cell, scale_atoms=True)
+    atoms_copy.set_cell(1.1 * original_cell, scale_atoms=True)
     energy_after = atoms_copy.get_potential_energy()
     forces_after = atoms_copy.get_forces()
     stress_after = atoms_copy.get_stress()
 
     diff_energy = np.abs(energy_after - energy_initial)
     diff_force = forces_initial - forces_after
     diff_stress = stress_initial - stress_after
@@ -353,15 +378,15 @@
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     calc = CPUNEP(nep3)
     with pytest.raises(ValueError)as e:
         calc.calculate()
     assert 'Atoms must be defined to get energies and forces.' in str(e)
 
 
-def test_CPU_GPU_equivalent():
+def test_CPU_GPU_equivalent(PbTe):
     """Assert that the CPU and GPU implementation are equivalent
     """
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     # CPU
     PbTe.calc = CPUNEP(nep3)
     cpu_energy = PbTe.get_potential_energy()
     cpu_forces = PbTe.get_forces()
@@ -373,15 +398,15 @@
     gpu_stress = PbTe.get_stress()
     assert np.isclose(cpu_energy, gpu_energy, atol=1e-12, rtol=1e-5)
     # GPUMD forces are in single precision, meaning errors can add up to 1e-6
     assert np.allclose(cpu_forces, gpu_forces, atol=1e-12, rtol=1e-5)
     assert np.allclose(cpu_stress, gpu_stress, atol=1e-12, rtol=1e-5)
 
 
-def test_CPU_GPU_equivalent_bulk():
+def test_CPU_GPU_equivalent_bulk(PbTeBulk):
     """Assert that the CPU and GPU implementation are equivalent for a bulk PbTE system
     """
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     print(PbTeBulk.get_volume())
     # CPU
     PbTeBulk.calc = CPUNEP(nep3)
     cpu_energy = PbTeBulk.get_potential_energy()
@@ -407,20 +432,37 @@
 
 
 def test_cpunep_tostr(NEP3CPUNEP):
     s = str(NEP3CPUNEP)
     assert 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt' in s
 
 
-def test_cpunep_readwrite_db(tmpdir, NEP3CPUNEP):
+def test_cpunep_readwrite_db(tmpdir, NEP3CPUNEP, PbTeBulk):
     PbTeBulk.calc = NEP3CPUNEP
     with connect(f'{tmpdir}/db.db') as db:
         db.write(PbTeBulk)
     atoms = None
     with connect(f'{tmpdir}/db.db') as db:
         for row in db.select():
             atoms = row.toatoms()
             atoms.calc = CPUNEP(**row.calculator_parameters)
     assert atoms == PbTeBulk
     assert atoms.calc is not None
     all_keys = ['potential_filename']
     assert all([getattr(atoms.calc, key) == getattr(NEP3CPUNEP, key) for key in all_keys])
+
+# ---- get_dipole() ----
+
+
+def test_get_dipole_NEP3():
+    """NEP3 model supplied. Compares results to output from DFT."""
+    nep3 = 'tests/nep_models/nep4_dipole_Christian.txt'
+    calc = CPUNEP(nep3)
+    structure = read('tests/example_files/dipole/test.xyz')
+    structure.calc = calc
+
+    dipole = structure.get_dipole_moment()
+    dft_dipole = structure.info['dipole']
+    delta = dipole - dft_dipole
+
+    assert dipole.shape == (3,)
+    assert np.allclose([-0.07468218, -0.03891397, -0.11160894], delta, atol=1e-12, rtol=1e-5)
```

### Comparing `calorine-1.5/tests/test_gpumd_io.py` & `calorine-1.6/tests/test_gpumd_io.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_gpunep.py` & `calorine-1.6/tests/test_gpunep.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_nep3_execution.py` & `calorine-1.6/tests/test_nep3_execution.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_nep4_execution.py` & `calorine-1.6/tests/test_nep4_execution.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_nep_io.py` & `calorine-1.6/tests/test_nep_io.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_nep_nep.py` & `calorine-1.6/tests/test_nep_nep.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 import pytest
 import numpy as np
 from ase import Atoms
-from calorine.nep.nep import get_descriptors, get_potential_forces_and_virials, _clean_tmp_dir
+from ase.io import read
+from calorine.nep.nep import get_descriptors, get_dipole, get_latent_space, \
+        get_potential_forces_and_virials, _clean_tmp_dir
 
-PbTe = Atoms('TePb', positions=[(0, 0, 0), (0, 0.0, 1.1)],
-             cell=([100, 0, 0], [0, 100, 0], [0, 0, 100]))
-C = Atoms('C', positions=[(0, 0, 0)])
-CO = Atoms('CO', positions=[(0, 0, 0), (0, 0.0, 1.1)])
-CC = Atoms('CC', positions=[(0, 0, 0), (0, 0.0, 1.1)])
-CON = Atoms('CON', positions=[(0, 0, 0), (0, 0.0, 1.1), (0, 0.0, 2.2)])
+
+@pytest.fixture
+def PbTe():
+    return Atoms('TePb', positions=[(0, 0, 0), (0, 0.0, 1.1)],
+                 cell=([100, 0, 0], [0, 100, 0], [0, 0, 100]))
+
+
+@pytest.fixture
+def C():
+    return Atoms('C', positions=[(0, 0, 0)])
+
+
+@pytest.fixture
+def CC():
+    return Atoms('CC', positions=[(0, 0, 0), (0, 0.0, 1.1)])
+
+
+@pytest.fixture
+def CO():
+    return Atoms('CO', positions=[(0, 0, 0), (0, 0.0, 1.1)])
+
+
+@pytest.fixture
+def CON():
+    return Atoms('CON', positions=[(0, 0, 0), (0, 0.0, 1.1), (0, 0.0, 2.2)])
 
 
 def get_expected(path):
     """Load forces or virials from file"""
     return np.loadtxt(path)
 
 
@@ -31,50 +52,50 @@
     """
     with open(file, 'r') as f:
         model = f.read()
     return model
 
 
 # --- get_descriptors ---
-def test_get_descriptors_setup_dummy_NEP2_model():
+def test_get_descriptors_setup_dummy_NEP2_model(PbTe):
     """Verifies the dummy NEP model is properly formatted."""
     get_descriptors(PbTe, debug=True)
     tmp_dir = './tmp_nepy/'
     PbTe_dummy = _load_nep_from_file(f'{tmp_dir}/nep.txt')
     _clean_tmp_dir(tmp_dir)
     expected_PbTe_dummy = _load_nep_from_file(
         'tests/nep_models/PbTe_NEP2_dummy.txt')
     assert PbTe_dummy == expected_PbTe_dummy
 
 
-def test_get_descriptors_no_cell():
+def test_get_descriptors_no_cell(CO):
     """Should get descriptors for atoms without a specified cell, and raise a warning."""
     with pytest.warns(UserWarning) as record:
         descriptors = get_descriptors(CO)
     assert len(record) == 1
     assert record[0].message.args[0] == 'Using default unit cell (cubic with side 100 Å).'
     assert descriptors.shape == (2, 52)
 
 
-def test_get_descriptors_NEP2_independent_of_species():
+def test_get_descriptors_NEP2_independent_of_species(PbTe, CO):
     """NEP2 should give the same descriptors regardless of atom species."""
     descriptors_PbTe = get_descriptors(PbTe)
     descriptors_CO = get_descriptors(CO)
     assert np.allclose(descriptors_CO, descriptors_PbTe, atol=1e-12, rtol=0)
 
 
-def test_get_descriptors_NEP2_several_atoms_same_species():
+def test_get_descriptors_NEP2_several_atoms_same_species(CC):
     """NEP2 should get the descritors for a single component system"""
     descriptors_CC = get_descriptors(CC)
     assert descriptors_CC.shape == (2, 52)
     assert descriptors_CC.dtype == np.float64
     assert not np.all(np.isclose(descriptors_CC, 0))
 
 
-def test_get_descriptors_dummy_NEP2_several_atom_species():
+def test_get_descriptors_dummy_NEP2_several_atom_species(C, CO, CON):
     """Verifies the dummy NEP model has the correct number of parameters."""
     # C
     get_descriptors(C, debug=True)
     tmp_dir = './tmp_nepy/'
     C_dummy_parameters = _load_nep_from_file(f'{tmp_dir}/nep.txt').split('\n')[6:]
     _clean_tmp_dir(tmp_dir)
     assert len(C_dummy_parameters) == 1698
@@ -88,54 +109,54 @@
     get_descriptors(CON, debug=True)
     tmp_dir = './tmp_nepy/'
     CON_dummy_parameters = _load_nep_from_file(f'{tmp_dir}/nep.txt').split('\n')[6:]
     _clean_tmp_dir(tmp_dir)
     assert len(CON_dummy_parameters) == 1898
 
 
-def test_get_descriptors_NEP2_dummy():
+def test_get_descriptors_NEP2_dummy(PbTe):
     """Case: No NEP model supplied; using dummy NEP2 model.
        Compares results to output from `nep_cpu`
     """
     descriptors_PbTe = get_descriptors(PbTe)
     expected_PbTe = np.loadtxt(
         'tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out')
     assert np.allclose(descriptors_PbTe, expected_PbTe, atol=1e-12, rtol=0)
 
 
-def test_get_descriptors_NEP3():
+def test_get_descriptors_NEP3(PbTe):
     """Case: NEP3 model supplied. Compares results to output from `nep_cpu`"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     descriptors_PbTe = get_descriptors(PbTe, potential_filename=nep3)
     expected_PbTe = np.loadtxt(
         'tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out')
     assert np.allclose(descriptors_PbTe, expected_PbTe, atol=1e-12, rtol=0)
 
 
-def test_get_descriptors_debug():
+def test_get_descriptors_debug(PbTe):
     """Check that the generated files are accessible in the debug directory"""
     get_descriptors(PbTe, debug=True)
     tmp_dir = './tmp_nepy/'
     PbTe_dummy = _load_nep_from_file(f'{tmp_dir}/nep.txt')
     _clean_tmp_dir(tmp_dir)
     assert 'nep 2 Te Pb' in PbTe_dummy
 
 
-def test_get_descriptors_debug_directory_exists():
+def test_get_descriptors_debug_directory_exists(PbTe):
     """Should fail if debug directory already exists from an earlier calculation"""
     get_descriptors(PbTe, debug=True)
     tmp_dir = './tmp_nepy/'
     with pytest.raises(FileExistsError)as e:
         get_descriptors(PbTe, debug=True)
     assert 'Please delete or move the conflicting directory' in str(e)
     _clean_tmp_dir(tmp_dir)
 
 
 # --- get_potential_forces_and_virials ---
-def test_get_potential_forces_and_virials_NEP3():
+def test_get_potential_forces_and_virials_NEP3(PbTe):
     """Case: NEP3 model supplied. Compares results to output from `nep_cpu`"""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     energies, forces, virials = get_potential_forces_and_virials(
         PbTe, potential_filename=nep3)
 
     expected_forces = get_expected(
         'tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out')
@@ -145,15 +166,15 @@
     assert energies.shape == (2,)
     assert forces.shape == (2, 3)
     assert virials.shape == (2, 9)
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_NEP3_debug():
+def test_get_potential_forces_and_virials_NEP3_debug(PbTe):
     """Compares result with debug flag enabled."""
     nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
     energies, forces, virials = get_potential_forces_and_virials(
         PbTe, potential_filename=nep3, debug=True)
 
     expected_forces = get_expected(
         'tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out')
@@ -163,15 +184,15 @@
     assert energies.shape == (2,)
     assert forces.shape == (2, 3)
     assert virials.shape == (2, 9)
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_dummy_NEP2():
+def test_get_potential_forces_and_virials_dummy_NEP2(CO):
     """Dummy NEP2 model supplied. Compares results to output from `nep_cpu` for another system"""
     nep2_dummy = 'tests/nep_models/CO_NEP2_dummy.txt'
     energies, forces, virials = get_potential_forces_and_virials(
         CO, potential_filename=nep2_dummy)
 
     expected_forces = get_expected('tests/example_output/CO_NEP2_dummy_CO_2atom_force.out')
     expected_virials = get_expected('tests/example_output/CO_NEP2_dummy_CO_2atom_virial.out')
@@ -179,15 +200,15 @@
     assert energies.shape == (2,)
     assert forces.shape == (2, 3)
     assert virials.shape == (2, 9)
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_no_cell():
+def test_get_potential_forces_and_virials_no_cell(CO):
     """Should work with default cell if no cell is supplied"""
     nep2_dummy = 'tests/nep_models/CO_NEP2_dummy.txt'
     with pytest.warns(UserWarning) as record:
         energies, forces, virials = get_potential_forces_and_virials(
             CO, potential_filename=nep2_dummy)
 
     expected_forces = get_expected('tests/example_output/CO_NEP2_dummy_CO_2atom_force.out')
@@ -198,15 +219,15 @@
     assert energies.shape == (2,)
     assert forces.shape == (2, 3)
     assert virials.shape == (2, 9)
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_several_of_same_species():
+def test_get_potential_forces_and_virials_several_of_same_species(CC):
     """Check that forces are correct for a CC system"""
     nep = 'tests/nep_models/C_NEP2_dummy.txt'
     energies, forces, virials = get_potential_forces_and_virials(
         CC, potential_filename=nep)
 
     expected_forces = get_expected('tests/example_output/C_NEP2_dummy_C_2atom_force.out')
     expected_virials = get_expected('tests/example_output/C_NEP2_dummy_C_2atom_virial.out')
@@ -214,15 +235,15 @@
     assert energies.shape == (2,)
     assert forces.shape == (2, 3)
     assert virials.shape == (2, 9)
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_several_different_species():
+def test_get_potential_forces_and_virials_several_different_species(CON):
     """Check that forces are correct for a CON system.
     Note that these forces should be exactly zero for this system
     since the NEP2 dummy potential treats all atom species as identical atm.
     """
     nep = 'tests/nep_models/CON_NEP2_dummy.txt'
     energies, forces, virials = get_potential_forces_and_virials(
         CON, potential_filename=nep)
@@ -236,12 +257,47 @@
 
     assert np.allclose(forces, expected_forces, atol=1e-12, rtol=0)
     assert np.allclose(forces, np.zeros((3, 3)), atol=1e-12, rtol=0)
     assert np.allclose(virials, expected_virials, atol=1e-12, rtol=0)
     assert np.allclose(virials, np.zeros((3, 9)), atol=1e-12, rtol=0)
 
 
-def test_get_potential_forces_and_virials_no_potential():
+def test_get_potential_forces_and_virials_no_potential(PbTe):
     """Tries to get potentials, forces and virials without specifying potential"""
     with pytest.raises(ValueError)as e:
         get_potential_forces_and_virials(PbTe)
     assert 'Potential must be defined!' in str(e)
+
+
+# --- get_dipole ---
+def test_get_dipole_NEP3():
+    """Case: NEP3 model supplied. Compares results to output from DFT."""
+    nep3 = 'tests/nep_models/nep4_dipole_Christian.txt'
+    structure = read('tests/example_files/dipole/test.xyz')
+
+    dipole = get_dipole(structure, potential_filename=nep3)
+    dft_dipole = structure.info['dipole']
+    delta = dipole - dft_dipole
+    assert dipole.shape == (3,)
+    assert np.allclose([-0.07468218, -0.03891397, -0.11160894], delta, atol=1e-12, rtol=1e-5)
+
+
+def test_get_dipole_no_potential(PbTe):
+    """Tries to get dipole without specifying potential"""
+    with pytest.raises(ValueError)as e:
+        get_dipole(PbTe)
+    assert 'Potential must be defined!' in str(e)
+
+
+# --- get_latent_space ---
+def test_get_latent_space_NEP3(PbTe):
+    """Case: NEP3 model supplied. Returns a latent space with expected shape."""
+    nep3 = 'tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt'
+    latent = get_latent_space(PbTe, potential_filename=nep3)
+    assert latent.shape == (2, 30)
+
+
+def test_get_latent_space_no_potential(PbTe):
+    """Tries to get latent space without specifying potential"""
+    with pytest.raises(ValueError)as e:
+        get_latent_space(PbTe)
+    assert 'Potential must be defined!' in str(e)
```

### Comparing `calorine-1.5/tests/test_nep_potential.py` & `calorine-1.6/tests/test_nep_potential.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_phonons.py` & `calorine-1.6/tests/test_phonons.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_setup_training.py` & `calorine-1.6/tests/test_setup_training.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_stiffness.py` & `calorine-1.6/tests/test_stiffness.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tests/test_structures.py` & `calorine-1.6/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/CsPbI3-SCAN.txt` & `calorine-1.6/tutorials/CsPbI3-SCAN.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/PbTe_NEP3.txt` & `calorine-1.6/tutorials/PbTe_NEP3.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/elastic_stiffness_tensor.ipynb` & `calorine-1.6/doc/tutorials/elastic_stiffness_tensor.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(0, 'The elastic stiffness tensor $c_{ij}$ can then be "*

 * *            "readily calculated using the `get_elastic_stiffness_tensor` function.\\n')], delete: "*

 * *            "[0]}}, 9: {'source': {insert: [(0, 'We compute the force constants using the "*

 * *            '`get_force_constants` function and then use methods of the [Phonopy '*

 * *            'object](https://phonopy.github.io/phonopy/phonopy-module.html) returned by the latter '*

 * *            'to calculate the group veloc […]*

```diff
@@ -64,15 +64,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e8fa677a-303c-452a-84ca-f943ea96b219",
             "metadata": {},
             "source": [
-                "The elastic stiffness tensor $c_{ij}$ can then be readily calculated using the [`get_elastic_stiffness_tensor` function](../tools.html#calorine.tools.get_elastic_stiffness_tensor).\n",
+                "The elastic stiffness tensor $c_{ij}$ can then be readily calculated using the `get_elastic_stiffness_tensor` function.\n",
                 "The latter applies a series of deformations to the cell and fits the resulting strain energy to a Taylor expansion in strain, in which the components of the elastic stiffness tensor appear as expansion coefficients."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "86b5bb00-2e5b-42ae-9f43-3203e5287c20",
@@ -129,15 +129,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "07274b4b-73ec-4b5c-ace7-21ee662687bd",
             "metadata": {},
             "source": [
-                "We compute the force constants using the [`get_force_constants` function](../tools.html#calorine.tools.get_force_constants) and then use methods of the [`Phonopy` object](https://phonopy.github.io/phonopy/phonopy-module.html) returned by the latter to calculate the group velocities at $\\boldsymbol{q}=(\\delta, 0, 0)$ with $\\delta = 0.01$.\n",
+                "We compute the force constants using the `get_force_constants` function and then use methods of the [Phonopy object](https://phonopy.github.io/phonopy/phonopy-module.html) returned by the latter to calculate the group velocities at $\\boldsymbol{q}=(\\delta, 0, 0)$ with $\\delta = 0.01$.\n",
                 "This $\\boldsymbol{q}$-point lies along $\\left<100\\right>$ and the small $\\delta$-value mimics the long-wavelength limit, i.e., $\\boldsymbol{q} \\rightarrow 0$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "0102bb7b-e7b2-44be-8d85-a7b55eb349a7",
```

### Comparing `calorine-1.5/tutorials/nep_model_inspection.ipynb` & `calorine-1.6/tutorials/nep_model_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz` & `calorine-1.6/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz` & `calorine-1.6/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz` & `calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz` & `calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/phonons.ipynb` & `calorine-1.6/tutorials/phonons.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976004464285715%*

 * *Differences: {"'cells'": "{0: {'source': ['# Phonon properties']}, 2: {'source': {insert: [(1, 'First, we "*

 * *            'compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> '*

 * *            'described by a neuroevolution potential using the `get_force_constants()` convenience '*

 * *            'function from `calorine`, which wraps functionality from the [phonopy '*

 * *            "package](https://phonopy.github.io/phonopy).\\n'), (2, 'To set the path through the "*

 * *            'Brillouin zone we use the [ […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "6373958f-5692-4b03-8d83-7f01b751bbe5",
             "metadata": {},
             "source": [
-                "# Phonon dispersions and density of states"
+                "# Phonon properties"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "7e813f1b-45db-404e-82eb-eb974b25da0a",
             "metadata": {},
@@ -27,16 +27,16 @@
         },
         {
             "cell_type": "markdown",
             "id": "d089b4ae-a518-4a80-85e8-637dffdc1de8",
             "metadata": {},
             "source": [
                 "In this tutorial we illustrate the calculation of phonon dispersions and densities of states.\n",
-                "First, we compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> described by a neuroevolution potential using the [`get_phonon_dispersion()` convenience function](../tools.html#calorine.tools.get_phonon_dispersion) from `calorine`, which wraps functionality from the [`phonopy` package](https://phonopy.github.io/phonopy/).\n",
-                "To set the path through the Brillouin zone we use the [`seekpath` package](https://www.materialscloud.org/work/tools/seekpath).\n",
+                "First, we compute the phonon dispersion of the orthorhombic phase of CsPbI<sub>3</sub> described by a neuroevolution potential using the `get_force_constants()` convenience function from `calorine`, which wraps functionality from the [phonopy package](https://phonopy.github.io/phonopy).\n",
+                "To set the path through the Brillouin zone we use the [seekpath package](https://www.materialscloud.org/work/tools/seekpath).\n",
                 "\n",
                 "Then we demonstrate how to use the Python API of `phonopy` directly to compute the phonon density of states."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f2cc4a4a-7e74-47de-9b6d-f66607d89687",
@@ -64,15 +64,15 @@
             "cell_type": "markdown",
             "id": "c2715f08-e76e-4012-b9b9-b08133ceb32e",
             "metadata": {},
             "source": [
                 "## Compute force constants\n",
                 "\n",
                 "Next we prepare the force constants from which we can then obtain, for example, the phonon dispersion and the phonon density of states as shown below.\n",
-                "To this end, we use the [`get_force_constants` function](../tools.html#calorine.tools.get_force_constants).\n",
+                "To this end, we use the `get_force_constants()` function.\n",
                 "Note that the third argument of this function specifies the supercell that is being used for computing the force constant matrix.\n",
                 "Here, we simply use a $2\\times2\\times2$ supercell.\n",
                 "In general you need to ensure that the results are converged with respect to the supercell size."
             ]
         },
         {
             "cell_type": "code",
@@ -85,26 +85,26 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37dc4a23-da5f-4a8a-bb95-01ee5cca3515",
             "metadata": {},
             "source": [
-                "The `get_force_constants` function returns a [`Phonopy` object](https://phonopy.github.io/phonopy/phonopy-module.html), which provides methods for calculating various derived quantities, including but not limited to the phonon dispersion and density of states."
+                "The `get_force_constants` function returns a [Phonopy object](https://phonopy.github.io/phonopy/phonopy-module.html), which provides methods for calculating various derived quantities, including but not limited to the phonon dispersion and density of states."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0c331069-e206-434f-acd0-a5c2b13a58af",
             "metadata": {},
             "source": [
                 "## Phonon dispersion\n",
                 "\n",
                 "We now need to specify the path through the Brillouin zone along which the phonon dispersion is to be calculated.\n",
-                "To this end, we use the [`seekpath` package](https://www.materialscloud.org/work/tools/seekpath), which provides a standardized way for generating such paths.\n",
+                "To this end, we use the [seekpath package](https://www.materialscloud.org/work/tools/seekpath), which provides a standardized way for generating such paths.\n",
                 "It is also possible to set up suitable paths also \"manually\" by stringing together a list of $\\boldsymbol{q}$-points.\n",
                 "\n",
                 "In the following, we first prepare the structure in the format expected by `seekpath` and then call the `get_explicit_k_path` function."
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `calorine-1.5/tutorials/structure_relaxation.ipynb` & `calorine-1.6/tutorials/structure_relaxation.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.5/tutorials/visualize_descriptor_space_with_pca.ipynb` & `calorine-1.6/tutorials/visualize_descriptor_space_with_pca.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Descriptor space analysis\\n')], delete: [0]}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "46ee7988",
             "metadata": {},
             "source": [
-                "# Visualize descriptor space with PCA\n",
+                "# Descriptor space analysis\n",
                 "This notebook demonstrates how to visualize the descriptor space for a collection of structures using principal component Analysis (PCA) as implemented in [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "84538df3",
             "metadata": {},
```

