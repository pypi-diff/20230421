# Comparing `tmp/tnsu-1.0.2.tar.gz` & `tmp/tnsu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/royelkabetz/Git/tensor_networks_simple_update/dist/tmp06hynyy4/tnsu-1.0.2.tar", last modified: Sun Jul 17 20:40:21 2022, max compression
+gzip compressed data, was "/Users/royelkabetz/Git/tensor_networks_simple_update/dist/.tmp-5b48f9g3/tnsu-1.0.3.tar", last modified: Fri Apr 21 20:09:41 2023, max compression
```

## Comparing `tnsu-1.0.2.tar` & `tnsu-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2022-07-17 20:40:21.985280 tnsu-1.0.2/
--rw-r--r--   0 royelkabetz   (502) staff       (20)     1072 2022-07-17 13:15:41.000000 tnsu-1.0.2/LICENSE.txt
--rw-r--r--   0 royelkabetz   (502) staff       (20)    15999 2022-07-17 20:40:21.985408 tnsu-1.0.2/PKG-INFO
--rw-r--r--   0 royelkabetz   (502) staff       (20)    15253 2022-07-17 20:27:36.000000 tnsu-1.0.2/README.md
--rw-r--r--   0 royelkabetz   (502) staff       (20)       84 2022-07-17 13:15:41.000000 tnsu-1.0.2/pyproject.toml
--rw-r--r--   0 royelkabetz   (502) staff       (20)      986 2022-07-17 20:40:21.987616 tnsu-1.0.2/setup.cfg
-drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2022-07-17 20:40:21.921136 tnsu-1.0.2/src/
-drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2022-07-17 20:40:21.936245 tnsu-1.0.2/src/tnsu/
--rw-r--r--   0 royelkabetz   (502) staff       (20)        0 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/__init__.py
--rw-r--r--   0 royelkabetz   (502) staff       (20)     6064 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/examples.py
--rw-r--r--   0 royelkabetz   (502) staff       (20)    11620 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/ncon.py
-drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2022-07-17 20:40:21.979400 tnsu-1.0.2/src/tnsu/networks/
--rw-r--r--   0 royelkabetz   (502) staff       (20)   778332 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/networks/AFH_10x10_obc_D_4.pkl
--rw-r--r--   0 royelkabetz   (502) staff       (20)  5378915 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/networks/AFH_20x20_obc_D_4.pkl
--rw-r--r--   0 royelkabetz   (502) staff       (20)  5984087 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/networks/AFH_20x20_pbc_D_4.pkl
--rw-r--r--   0 royelkabetz   (502) staff       (20)    30005 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/simple_update.py
--rw-r--r--   0 royelkabetz   (502) staff       (20)     5831 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/structure_matrix_constructor.py
--rw-r--r--   0 royelkabetz   (502) staff       (20)     9244 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/tensor_network.py
--rw-r--r--   0 royelkabetz   (502) staff       (20)     2611 2022-07-17 13:15:41.000000 tnsu-1.0.2/src/tnsu/utils.py
-drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2022-07-17 20:40:21.944273 tnsu-1.0.2/src/tnsu.egg-info/
--rw-r--r--   0 royelkabetz   (502) staff       (20)    15999 2022-07-17 20:40:21.000000 tnsu-1.0.2/src/tnsu.egg-info/PKG-INFO
--rw-r--r--   0 royelkabetz   (502) staff       (20)      523 2022-07-17 20:40:21.000000 tnsu-1.0.2/src/tnsu.egg-info/SOURCES.txt
--rw-r--r--   0 royelkabetz   (502) staff       (20)        1 2022-07-17 20:40:21.000000 tnsu-1.0.2/src/tnsu.egg-info/dependency_links.txt
--rw-r--r--   0 royelkabetz   (502) staff       (20)       37 2022-07-17 20:40:21.000000 tnsu-1.0.2/src/tnsu.egg-info/requires.txt
--rw-r--r--   0 royelkabetz   (502) staff       (20)        5 2022-07-17 20:40:21.000000 tnsu-1.0.2/src/tnsu.egg-info/top_level.txt
--rw-r--r--   0 royelkabetz   (502) staff       (20)        1 2022-07-17 18:06:49.000000 tnsu-1.0.2/src/tnsu.egg-info/zip-safe
+drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2023-04-21 20:09:41.748892 tnsu-1.0.3/
+-rw-r--r--   0 royelkabetz   (502) staff       (20)     1072 2022-07-17 13:15:41.000000 tnsu-1.0.3/LICENSE.txt
+-rw-r--r--   0 royelkabetz   (502) staff       (20)    16179 2023-04-21 20:09:41.749043 tnsu-1.0.3/PKG-INFO
+-rw-r--r--   0 royelkabetz   (502) staff       (20)    15433 2023-04-21 19:13:34.000000 tnsu-1.0.3/README.md
+-rw-r--r--   0 royelkabetz   (502) staff       (20)       84 2022-07-17 13:15:41.000000 tnsu-1.0.3/pyproject.toml
+-rw-r--r--   0 royelkabetz   (502) staff       (20)      986 2023-04-21 20:09:41.750033 tnsu-1.0.3/setup.cfg
+drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2023-04-21 20:09:41.717939 tnsu-1.0.3/src/
+drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2023-04-21 20:09:41.726303 tnsu-1.0.3/src/tnsu/
+-rw-r--r--   0 royelkabetz   (502) staff       (20)        0 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/__init__.py
+-rw-r--r--   0 royelkabetz   (502) staff       (20)     6067 2022-07-24 07:07:56.000000 tnsu-1.0.3/src/tnsu/examples.py
+-rw-r--r--   0 royelkabetz   (502) staff       (20)    11620 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/ncon.py
+drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2023-04-21 20:09:41.742422 tnsu-1.0.3/src/tnsu/networks/
+-rw-r--r--   0 royelkabetz   (502) staff       (20)   778332 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/networks/AFH_10x10_obc_D_4.pkl
+-rw-r--r--   0 royelkabetz   (502) staff       (20)  5378915 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/networks/AFH_20x20_obc_D_4.pkl
+-rw-r--r--   0 royelkabetz   (502) staff       (20)  5984087 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/networks/AFH_20x20_pbc_D_4.pkl
+-rw-r--r--   0 royelkabetz   (502) staff       (20)    30039 2023-04-21 18:52:19.000000 tnsu-1.0.3/src/tnsu/simple_update.py
+-rw-r--r--   0 royelkabetz   (502) staff       (20)     5831 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/structure_matrix_constructor.py
+-rw-r--r--   0 royelkabetz   (502) staff       (20)     9244 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/tensor_network.py
+-rw-r--r--   0 royelkabetz   (502) staff       (20)     2611 2022-07-17 13:15:41.000000 tnsu-1.0.3/src/tnsu/utils.py
+drwxr-xr-x   0 royelkabetz   (502) staff       (20)        0 2023-04-21 20:09:41.730461 tnsu-1.0.3/src/tnsu.egg-info/
+-rw-r--r--   0 royelkabetz   (502) staff       (20)    16179 2023-04-21 20:09:41.000000 tnsu-1.0.3/src/tnsu.egg-info/PKG-INFO
+-rw-r--r--   0 royelkabetz   (502) staff       (20)      523 2023-04-21 20:09:41.000000 tnsu-1.0.3/src/tnsu.egg-info/SOURCES.txt
+-rw-r--r--   0 royelkabetz   (502) staff       (20)        1 2023-04-21 20:09:41.000000 tnsu-1.0.3/src/tnsu.egg-info/dependency_links.txt
+-rw-r--r--   0 royelkabetz   (502) staff       (20)       37 2023-04-21 20:09:41.000000 tnsu-1.0.3/src/tnsu.egg-info/requires.txt
+-rw-r--r--   0 royelkabetz   (502) staff       (20)        5 2023-04-21 20:09:41.000000 tnsu-1.0.3/src/tnsu.egg-info/top_level.txt
+-rw-r--r--   0 royelkabetz   (502) staff       (20)        1 2022-07-17 18:06:49.000000 tnsu-1.0.3/src/tnsu.egg-info/zip-safe
```

### Comparing `tnsu-1.0.2/LICENSE.txt` & `tnsu-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/PKG-INFO` & `tnsu-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsu
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for Tensor-Networks Simple-Update simulations of quantum wave functions representations
 Home-page: https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update
 Author: Roy Elkabetz
 Author-email: elkabetzroy@gmail.com
 Keywords: Tensor-Networks,Simple-Update,Quantum-Information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,32 +40,32 @@
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/imaginary_time_evolution_operator.png?raw=true" width="300" height="">
 
 where finally,
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ITE_local_gate.png?raw=true" width="200" height="">
 
-When performing the ITE scheme, the TN virtual bond dimension increases, therefore, after every few ITE iterations we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
+When performing the ITE scheme, the TN virtual bond dimension increases. Therefore, after every few ITE iterations, we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/simple_update_algorithm.png?raw=true" width="1000" height="">
 
 For a more comprehensive explanation of the algorithm, the interested reader should check out [1].
 
 ## The Code
 
 
 The [`src.tnsu`](/src/tnsu) folder contains the source code for this project
 
 | #   | file                                         | Subject             | 
 |:----:|------------------------------------------------|:-----------------:|
-| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights and their connectivity| 
-| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and perform a simple-update run on it using Imaginary Time Evolution. | 
+| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights, and their connectivity| 
+| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and performs a simple-update run on it using Imaginary Time Evolution. | 
 | 3  | `structure_matrix_constructor.py`         | Contains a dictionary of common iPEPS structure matrices and also functionality construction of 2D square and rectangular lattices structure matrices (**still in progress**).
 | 4  | `examples.py`         | Few scripts for loading a tensor network state from memory and a full Antiferromagnetic Heisenberg model PEPS experiment.|
-| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) github repository.|
+| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) GitHub repository.|
 | 6  | `utils.py`         | A general utility module.|
 
 
 
 ## Examples
 
 ### Example 1: Spin 1/2 2D star lattice iPEPS Antiferromagnetic Heisenberg model simulation
@@ -133,97 +133,97 @@
 ```
 
 and run the algorithm
 ```python
 star_su.run()
 ```
 
-It is also possible to compute a single and double site expectation values like energy, magnetizatoin etc, with the following
+It is also possible to compute single and double-site expectation values like energy, magnetization etc, with the following
 ```python
 energy_per_site = star_su.energy_per_site()
 z_magnetization_per_site = star_su.expectation_per_site(operator=pauli_z / 2)
 ```
 
-or manually calculating single and double site reduced-density matrices and expectations following the next few lines of code
+or manually calculating single and double-site reduced-density matrices and expectations following the next few lines of code
 ```python
 tensor = 0
 edge = 1
 tensor_pair_operator = np.reshape(np.kron(pauli_z / 2, pauli_z / 2), (2, 2, 2, 2))
 star_su.tensor_rdm(tensor_index=tensor)
 star_su.tensor_pair_rdm(common_edge=edge)
 star_su.tensor_expectation(tensor_index=tensor, operator=pauli_z / 2)
 star_su.tensor_pair_expectation(common_edge=edge, operator=tensor_pair_operator)
 ```
 
 ### Example 2: The Trivial Simple-Update Algorithm
-The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor networks with no loops (tree-like topology) each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into to distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), where it is used as an approximated inference tool. For a detailed description about the duality between the trivial-Simple-Update and the Belief Propagation algorithm see Refs [3][4].
+The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting the ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor network with no loops (tree-like topology), each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), which is used as an approximated inference tool. For a detailed description of the duality between the trivial-Simple-Update and the Belief Propagation algorithm, see Refs [3][4].
 
-In order to implement the trivial-SU algorithm we can initialize the simple update class with zero time step as follows
+In order to implement the trivial-SU algorithm, we can initialize the simple update class with zero time step as follows
 ```python
 su.SimpleUpdate(tensor_network=tensornet, 
                 dts=[0], 
                 j_ij=j_ij, 
                 h_k=0, 
                 s_i=s, 
                 s_j=s, 
                 s_k=s_k, 
                 d_max=d_max, 
                 max_iterations=1000, 
                 convergence_error=1e-6, 
                 log_energy=False,
                 print_process=False)
 ```
-then, the algorithm will run 1000 iteration or until the maximal L2 distance between temporal consecutive weight vectors will be smaller then 1e-6.
+then, the algorithm will run 1000 iterations or until the maximal L2 distance between temporal consecutive weight vectors is smaller than 1e-6.
 
 
 There are more fully-written examples in the [`notebooks`](/notebooks) folder.
 
 ### List of Notebooks
-The notebooks below are not part of the package, they can be found in the `tnsu` github repository under `/notebooks`. You can run them locally with jupyter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
+The notebooks below are not part of the package, they can be found in the `tnsu` GitHub repository under `/notebooks`. You can run them locally with Jupiter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
 
 | #   | file            | Subject                                         | Colab             | Nbviewer               |
 |:----:|:--------------:|:------------------------------------------------:|:-----------------:|:---------------------:|
 | 1   | `ipeps_energy_simulations.ipynb` | Computing ground-state energies of iPEPS Tensor Networks   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)|
 | 2   | `Quantum_Ising_Model_Phase_Transition.ipynb` | Simulating the phase transition of the Quantum Transverse Field Ising model  | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)|
 | 3   | `Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb` | Spin-1 BLBQ tringular 2D lattice phase transition   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)|
 
 
 ## Simulations
 ### Spin-1/2 Antiferromagnetic Heisenberg (AFH) model
 
-Below are some result of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS and Cube tensor networks. The AFH Hamiltonian is given by
+Below are some results of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS, and Cube tensor networks. The AFH Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/hamiltonian_eq.png?raw=true" width="" height="60">
 
-In the case of the Star tensor network lattice the AFH Hamiltonian is composite of two parts which corresponds to different type of edges (see [1]).
-The Chain, Star, PEPS and Cube infinite tensor networks are illustrated in the next figure.
+In the case of the Star tensor network lattice, the AFH Hamiltonian consists of two parts that correspond to different types of edges (see [1]).
+The Chain, Star, PEPS, and Cube infinite tensor networks are illustrated in the next figure.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Tensor_Networks_diagrams.png?raw=true" width="1000" height=""> 
 
 
-Here are the ground-state energy per-site vs inverse virtual bond-dimension simulations for the tensor networks diagrams above
+Here is the ground-state energy per-site vs. inverse virtual bond-dimension simulations for the tensor networks diagrams above
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/chain_star_peps_cube_plots.png?raw=true" width="1000" height="">
 
 ### Quantum Ising Model on a 2D Spin-1/2 Lattice
 Next, we simulated the quantum Ising model on a 2D lattice with a transverse magnetic field. Its Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ising_transverse_field.png?raw=true" width="" height="100">
 
-In the plots below one can see the simulated x, z magnetization (per-site) along with the simulated energy (per-site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
+In the plots below, one can see the simulated x and z magnetization (per site) along with the simulated energy (per site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Ising_model.png?raw=true" width="1000" height="">
 
 ### Spin-1 Simulation of a Bilinear-Biquadratic Heisenberg model on a star 2D lattice
 
-Finally we simulated the BLBQ Hamiltonian which is given by the next equation
+Finally, we simulated the BLBQ Hamiltonian, which is given by the next equation
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_hamiltonian.png?raw=true" width="300" height="">
 
-notice that for 0 radian angle, this model coincides with the original AFH model. The energy, magnetization and Q-norm as a function of the angle for different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time to trace all the phase transitions of this model. However, we notice that for larger bond dimensions it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice see Ref [2])
+notice that for the 0-radian angle, this model coincides with the original AFH model. The energy, magnetization, and Q-norm as a function of the angle for a different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time tracing all the phase transitions of this model. However, we notice that for larger bond dimensions, it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice, see Ref [2])
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_model_simulation_star.png?raw=true" width="1000" height="">
 
 ## References
 - [[1]](https://arxiv.org/abs/1808.00680) Saeed S. Jahromi, and Roman Orus - "A universal tensor network algorithm for any infinite lattice" (2019)
 - [[2]](https://arxiv.org/abs/1805.00354) Ido Niesen, Philippe Corboz - "A ground state study of the spin-1 bilinear-biquadratic Heisenberg model on the triangular lattice using tensor networks" (2018)
 - [[3]](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.023073) Roy Alkabetz and Itai Arad - "Tensor networks contraction and the belief propagation algorithm" (2020)
@@ -232,18 +232,19 @@
 
 ## Contact
 
 Roy Elkabetz - [elkabetzroy@gmail.com](mailto:elkabetzroy@gmail.com)
 
 ## Citation
 
-To cite this repository in academic works or any other purpose, please use the following BibTeX citation:
-```Latex
-@software{tnsu,
-    author = {Elkabetz, Roy},
-    title = {{tnsu: A python package for Tensor Networks Simple-Update simulations}},
-    url = {https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update},
-    version = {1.0.2},
-    year = {2022}
+To cite this repository in academic works or for any other purpose, please use the following BibTeX citation:
+```
+@misc{tnsu,
+    author = "Elkabetz, Roy",
+    title = "Python Package for Universal Tensor-Networks Simple-Update Simulations",
+    howpublished = "\url{https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update}",
+    url = "https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/tnsu__A_python_package_for_Tensor_Networks_Simple_Update_simulations.pdf",
+    year = "2022",
+    type = "Python package"
 }
 ```
```

### Comparing `tnsu-1.0.2/README.md` & `tnsu-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,32 @@
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/imaginary_time_evolution_operator.png?raw=true" width="300" height="">
 
 where finally,
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ITE_local_gate.png?raw=true" width="200" height="">
 
-When performing the ITE scheme, the TN virtual bond dimension increases, therefore, after every few ITE iterations we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
+When performing the ITE scheme, the TN virtual bond dimension increases. Therefore, after every few ITE iterations, we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/simple_update_algorithm.png?raw=true" width="1000" height="">
 
 For a more comprehensive explanation of the algorithm, the interested reader should check out [1].
 
 ## The Code
 
 
 The [`src.tnsu`](/src/tnsu) folder contains the source code for this project
 
 | #   | file                                         | Subject             | 
 |:----:|------------------------------------------------|:-----------------:|
-| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights and their connectivity| 
-| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and perform a simple-update run on it using Imaginary Time Evolution. | 
+| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights, and their connectivity| 
+| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and performs a simple-update run on it using Imaginary Time Evolution. | 
 | 3  | `structure_matrix_constructor.py`         | Contains a dictionary of common iPEPS structure matrices and also functionality construction of 2D square and rectangular lattices structure matrices (**still in progress**).
 | 4  | `examples.py`         | Few scripts for loading a tensor network state from memory and a full Antiferromagnetic Heisenberg model PEPS experiment.|
-| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) github repository.|
+| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) GitHub repository.|
 | 6  | `utils.py`         | A general utility module.|
 
 
 
 ## Examples
 
 ### Example 1: Spin 1/2 2D star lattice iPEPS Antiferromagnetic Heisenberg model simulation
@@ -114,97 +114,97 @@
 ```
 
 and run the algorithm
 ```python
 star_su.run()
 ```
 
-It is also possible to compute a single and double site expectation values like energy, magnetizatoin etc, with the following
+It is also possible to compute single and double-site expectation values like energy, magnetization etc, with the following
 ```python
 energy_per_site = star_su.energy_per_site()
 z_magnetization_per_site = star_su.expectation_per_site(operator=pauli_z / 2)
 ```
 
-or manually calculating single and double site reduced-density matrices and expectations following the next few lines of code
+or manually calculating single and double-site reduced-density matrices and expectations following the next few lines of code
 ```python
 tensor = 0
 edge = 1
 tensor_pair_operator = np.reshape(np.kron(pauli_z / 2, pauli_z / 2), (2, 2, 2, 2))
 star_su.tensor_rdm(tensor_index=tensor)
 star_su.tensor_pair_rdm(common_edge=edge)
 star_su.tensor_expectation(tensor_index=tensor, operator=pauli_z / 2)
 star_su.tensor_pair_expectation(common_edge=edge, operator=tensor_pair_operator)
 ```
 
 ### Example 2: The Trivial Simple-Update Algorithm
-The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor networks with no loops (tree-like topology) each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into to distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), where it is used as an approximated inference tool. For a detailed description about the duality between the trivial-Simple-Update and the Belief Propagation algorithm see Refs [3][4].
+The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting the ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor network with no loops (tree-like topology), each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), which is used as an approximated inference tool. For a detailed description of the duality between the trivial-Simple-Update and the Belief Propagation algorithm, see Refs [3][4].
 
-In order to implement the trivial-SU algorithm we can initialize the simple update class with zero time step as follows
+In order to implement the trivial-SU algorithm, we can initialize the simple update class with zero time step as follows
 ```python
 su.SimpleUpdate(tensor_network=tensornet, 
                 dts=[0], 
                 j_ij=j_ij, 
                 h_k=0, 
                 s_i=s, 
                 s_j=s, 
                 s_k=s_k, 
                 d_max=d_max, 
                 max_iterations=1000, 
                 convergence_error=1e-6, 
                 log_energy=False,
                 print_process=False)
 ```
-then, the algorithm will run 1000 iteration or until the maximal L2 distance between temporal consecutive weight vectors will be smaller then 1e-6.
+then, the algorithm will run 1000 iterations or until the maximal L2 distance between temporal consecutive weight vectors is smaller than 1e-6.
 
 
 There are more fully-written examples in the [`notebooks`](/notebooks) folder.
 
 ### List of Notebooks
-The notebooks below are not part of the package, they can be found in the `tnsu` github repository under `/notebooks`. You can run them locally with jupyter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
+The notebooks below are not part of the package, they can be found in the `tnsu` GitHub repository under `/notebooks`. You can run them locally with Jupiter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
 
 | #   | file            | Subject                                         | Colab             | Nbviewer               |
 |:----:|:--------------:|:------------------------------------------------:|:-----------------:|:---------------------:|
 | 1   | `ipeps_energy_simulations.ipynb` | Computing ground-state energies of iPEPS Tensor Networks   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)|
 | 2   | `Quantum_Ising_Model_Phase_Transition.ipynb` | Simulating the phase transition of the Quantum Transverse Field Ising model  | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)|
 | 3   | `Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb` | Spin-1 BLBQ tringular 2D lattice phase transition   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)|
 
 
 ## Simulations
 ### Spin-1/2 Antiferromagnetic Heisenberg (AFH) model
 
-Below are some result of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS and Cube tensor networks. The AFH Hamiltonian is given by
+Below are some results of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS, and Cube tensor networks. The AFH Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/hamiltonian_eq.png?raw=true" width="" height="60">
 
-In the case of the Star tensor network lattice the AFH Hamiltonian is composite of two parts which corresponds to different type of edges (see [1]).
-The Chain, Star, PEPS and Cube infinite tensor networks are illustrated in the next figure.
+In the case of the Star tensor network lattice, the AFH Hamiltonian consists of two parts that correspond to different types of edges (see [1]).
+The Chain, Star, PEPS, and Cube infinite tensor networks are illustrated in the next figure.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Tensor_Networks_diagrams.png?raw=true" width="1000" height=""> 
 
 
-Here are the ground-state energy per-site vs inverse virtual bond-dimension simulations for the tensor networks diagrams above
+Here is the ground-state energy per-site vs. inverse virtual bond-dimension simulations for the tensor networks diagrams above
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/chain_star_peps_cube_plots.png?raw=true" width="1000" height="">
 
 ### Quantum Ising Model on a 2D Spin-1/2 Lattice
 Next, we simulated the quantum Ising model on a 2D lattice with a transverse magnetic field. Its Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ising_transverse_field.png?raw=true" width="" height="100">
 
-In the plots below one can see the simulated x, z magnetization (per-site) along with the simulated energy (per-site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
+In the plots below, one can see the simulated x and z magnetization (per site) along with the simulated energy (per site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Ising_model.png?raw=true" width="1000" height="">
 
 ### Spin-1 Simulation of a Bilinear-Biquadratic Heisenberg model on a star 2D lattice
 
-Finally we simulated the BLBQ Hamiltonian which is given by the next equation
+Finally, we simulated the BLBQ Hamiltonian, which is given by the next equation
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_hamiltonian.png?raw=true" width="300" height="">
 
-notice that for 0 radian angle, this model coincides with the original AFH model. The energy, magnetization and Q-norm as a function of the angle for different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time to trace all the phase transitions of this model. However, we notice that for larger bond dimensions it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice see Ref [2])
+notice that for the 0-radian angle, this model coincides with the original AFH model. The energy, magnetization, and Q-norm as a function of the angle for a different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time tracing all the phase transitions of this model. However, we notice that for larger bond dimensions, it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice, see Ref [2])
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_model_simulation_star.png?raw=true" width="1000" height="">
 
 ## References
 - [[1]](https://arxiv.org/abs/1808.00680) Saeed S. Jahromi, and Roman Orus - "A universal tensor network algorithm for any infinite lattice" (2019)
 - [[2]](https://arxiv.org/abs/1805.00354) Ido Niesen, Philippe Corboz - "A ground state study of the spin-1 bilinear-biquadratic Heisenberg model on the triangular lattice using tensor networks" (2018)
 - [[3]](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.023073) Roy Alkabetz and Itai Arad - "Tensor networks contraction and the belief propagation algorithm" (2020)
@@ -213,18 +213,19 @@
 
 ## Contact
 
 Roy Elkabetz - [elkabetzroy@gmail.com](mailto:elkabetzroy@gmail.com)
 
 ## Citation
 
-To cite this repository in academic works or any other purpose, please use the following BibTeX citation:
-```Latex
-@software{tnsu,
-    author = {Elkabetz, Roy},
-    title = {{tnsu: A python package for Tensor Networks Simple-Update simulations}},
-    url = {https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update},
-    version = {1.0.2},
-    year = {2022}
+To cite this repository in academic works or for any other purpose, please use the following BibTeX citation:
+```
+@misc{tnsu,
+    author = "Elkabetz, Roy",
+    title = "Python Package for Universal Tensor-Networks Simple-Update Simulations",
+    howpublished = "\url{https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update}",
+    url = "https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/tnsu__A_python_package_for_Tensor_Networks_Simple_Update_simulations.pdf",
+    year = "2022",
+    type = "Python package"
 }
 ```
```

### Comparing `tnsu-1.0.2/setup.cfg` & `tnsu-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tnsu
-version = 1.0.2
+version = 1.0.3
 author = Roy Elkabetz
 author_email = elkabetzroy@gmail.com
 description = A package for Tensor-Networks Simple-Update simulations of quantum wave functions representations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update
 keywords = Tensor-Networks, Simple-Update, Quantum-Information
```

### Comparing `tnsu-1.0.2/src/tnsu/examples.py` & `tnsu-1.0.3/src/tnsu/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,7 +143,10 @@
         if save_network:
             afh_tn.save_network()
 
         # add to networks list
         networks.append(afh_tn)
 
     return networks
+
+
+
```

### Comparing `tnsu-1.0.2/src/tnsu/ncon.py` & `tnsu-1.0.3/src/tnsu/ncon.py`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/networks/AFH_10x10_obc_D_4.pkl` & `tnsu-1.0.3/src/tnsu/networks/AFH_10x10_obc_D_4.pkl`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/networks/AFH_20x20_obc_D_4.pkl` & `tnsu-1.0.3/src/tnsu/networks/AFH_20x20_obc_D_4.pkl`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/networks/AFH_20x20_pbc_D_4.pkl` & `tnsu-1.0.3/src/tnsu/networks/AFH_20x20_pbc_D_4.pkl`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/simple_update.py` & `tnsu-1.0.3/src/tnsu/simple_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,16 +187,16 @@
             tj = self.tensor_dim_permute(tj)
 
             # group all virtual indices em != ek to form pi, pj "mps" tensors.
             pi = self.rank_n_rank_3(ti['tensor'])
             pj = self.rank_n_rank_3(tj['tensor'])
 
             # perform RQ decomposition of pi, pj to obtain ri, qi and rj, qj sub-tensors respectively.
-            ri, qi = linalg.rq(np.reshape(pi, [pi.shape[0] * pi.shape[1], pi.shape[2]]))
-            rj, qj = linalg.rq(np.reshape(pj, [pj.shape[0] * pj.shape[1], pj.shape[2]]))
+            ri, qi = linalg.rq(np.reshape(pi, [pi.shape[0] * pi.shape[1], pi.shape[2]]), mode="economic")
+            rj, qj = linalg.rq(np.reshape(pj, [pj.shape[0] * pj.shape[1], pj.shape[2]]), mode="economic")
 
             # reshape ri and rj into rank 3 tensors with shape (spin_dim, ek_dim, q_(right/left).shape[0]).
             i_physical_dim = ti['tensor'].shape[0]
             j_physical_dim = tj['tensor'].shape[0]
             ri = self.rank_2_rank_3(ri, i_physical_dim)  # (i, ek, qi)
             rj = self.rank_2_rank_3(rj, j_physical_dim)  # (j, ek, qj)
```

### Comparing `tnsu-1.0.2/src/tnsu/structure_matrix_constructor.py` & `tnsu-1.0.3/src/tnsu/structure_matrix_constructor.py`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/tensor_network.py` & `tnsu-1.0.3/src/tnsu/tensor_network.py`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu/utils.py` & `tnsu-1.0.3/src/tnsu/utils.py`

 * *Files identical despite different names*

### Comparing `tnsu-1.0.2/src/tnsu.egg-info/PKG-INFO` & `tnsu-1.0.3/src/tnsu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsu
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for Tensor-Networks Simple-Update simulations of quantum wave functions representations
 Home-page: https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update
 Author: Roy Elkabetz
 Author-email: elkabetzroy@gmail.com
 Keywords: Tensor-Networks,Simple-Update,Quantum-Information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,32 +40,32 @@
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/imaginary_time_evolution_operator.png?raw=true" width="300" height="">
 
 where finally,
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ITE_local_gate.png?raw=true" width="200" height="">
 
-When performing the ITE scheme, the TN virtual bond dimension increases, therefore, after every few ITE iterations we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
+When performing the ITE scheme, the TN virtual bond dimension increases. Therefore, after every few ITE iterations, we need to truncate the bond dimensions so the number of parameters in the tensor network state would stay bounded. The truncation step is implemented via a [Singular Value Decomposition (SVD)](https://en.wikipedia.org/wiki/Singular_value_decomposition) step. A full step-by-step illustrated description of the Simple Update algorithm (which is based on the ITE scheme) is depicted below. 
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/simple_update_algorithm.png?raw=true" width="1000" height="">
 
 For a more comprehensive explanation of the algorithm, the interested reader should check out [1].
 
 ## The Code
 
 
 The [`src.tnsu`](/src/tnsu) folder contains the source code for this project
 
 | #   | file                                         | Subject             | 
 |:----:|------------------------------------------------|:-----------------:|
-| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights and their connectivity| 
-| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and perform a simple-update run on it using Imaginary Time Evolution. | 
+| 1   | `tensor_network.py`                   | a Tensor Network class object which tracks the tensors, weights, and their connectivity| 
+| 2   | `simple_update.py`         | a Tensor Network Simple-Update algorithm class, which gets as an input a `TensorNetwork` object and performs a simple-update run on it using Imaginary Time Evolution. | 
 | 3  | `structure_matrix_constructor.py`         | Contains a dictionary of common iPEPS structure matrices and also functionality construction of 2D square and rectangular lattices structure matrices (**still in progress**).
 | 4  | `examples.py`         | Few scripts for loading a tensor network state from memory and a full Antiferromagnetic Heisenberg model PEPS experiment.|
-| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) github repository.|
+| 5  | `ncon.py`         | A module for tensors contraction in python copied from the [ncon](https://github.com/mhauru/ncon) GitHub repository.|
 | 6  | `utils.py`         | A general utility module.|
 
 
 
 ## Examples
 
 ### Example 1: Spin 1/2 2D star lattice iPEPS Antiferromagnetic Heisenberg model simulation
@@ -133,97 +133,97 @@
 ```
 
 and run the algorithm
 ```python
 star_su.run()
 ```
 
-It is also possible to compute a single and double site expectation values like energy, magnetizatoin etc, with the following
+It is also possible to compute single and double-site expectation values like energy, magnetization etc, with the following
 ```python
 energy_per_site = star_su.energy_per_site()
 z_magnetization_per_site = star_su.expectation_per_site(operator=pauli_z / 2)
 ```
 
-or manually calculating single and double site reduced-density matrices and expectations following the next few lines of code
+or manually calculating single and double-site reduced-density matrices and expectations following the next few lines of code
 ```python
 tensor = 0
 edge = 1
 tensor_pair_operator = np.reshape(np.kron(pauli_z / 2, pauli_z / 2), (2, 2, 2, 2))
 star_su.tensor_rdm(tensor_index=tensor)
 star_su.tensor_pair_rdm(common_edge=edge)
 star_su.tensor_expectation(tensor_index=tensor, operator=pauli_z / 2)
 star_su.tensor_pair_expectation(common_edge=edge, operator=tensor_pair_operator)
 ```
 
 ### Example 2: The Trivial Simple-Update Algorithm
-The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor networks with no loops (tree-like topology) each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into to distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), where it is used as an approximated inference tool. For a detailed description about the duality between the trivial-Simple-Update and the Belief Propagation algorithm see Refs [3][4].
+The trivial SU algorithm is equivalent to the SU algorithm without the ITE and truncation steps; it only consists of consecutive SVD steps over each TN edge (the same as contracting the ITE gate with zero time-step). The trivial-SU algorithm's fixed point corresponds to a canonical representation of the tensor network representations we started with. A tensor network canonical representation is strongly related to the Schmidt Decomposition operation over all the tensor network's edges, where for a tensor network with no loops (tree-like topology), each weight vector in the canonical representation corresponds to the Schmidt values of partitioning the network into two distinct networks along that edge. When the given tensor network has loops in it, it is no longer possible to partition the network along a single edge into distinguished parts. Therefore, the weight vectors are no longer equal to the Schmidt values but rather become some general approximation of the tensors' environments in the network. A very interesting property of the trivial simple update algorithm is that it is identical to the [Belief Propagation (BP)](https://en.wikipedia.org/wiki/Belief_propagation) algorithm. The Belief Propagation (BP) algorithm is a famous iterative-message-passing algorithm in the world of Probabilistic Graphical Models (PGM), which is used as an approximated inference tool. For a detailed description of the duality between the trivial-Simple-Update and the Belief Propagation algorithm, see Refs [3][4].
 
-In order to implement the trivial-SU algorithm we can initialize the simple update class with zero time step as follows
+In order to implement the trivial-SU algorithm, we can initialize the simple update class with zero time step as follows
 ```python
 su.SimpleUpdate(tensor_network=tensornet, 
                 dts=[0], 
                 j_ij=j_ij, 
                 h_k=0, 
                 s_i=s, 
                 s_j=s, 
                 s_k=s_k, 
                 d_max=d_max, 
                 max_iterations=1000, 
                 convergence_error=1e-6, 
                 log_energy=False,
                 print_process=False)
 ```
-then, the algorithm will run 1000 iteration or until the maximal L2 distance between temporal consecutive weight vectors will be smaller then 1e-6.
+then, the algorithm will run 1000 iterations or until the maximal L2 distance between temporal consecutive weight vectors is smaller than 1e-6.
 
 
 There are more fully-written examples in the [`notebooks`](/notebooks) folder.
 
 ### List of Notebooks
-The notebooks below are not part of the package, they can be found in the `tnsu` github repository under `/notebooks`. You can run them locally with jupyter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
+The notebooks below are not part of the package, they can be found in the `tnsu` GitHub repository under `/notebooks`. You can run them locally with Jupiter notebook or in google colab (which is preferable in case you don't want to burn your laptop's mother-board :) )
 
 | #   | file            | Subject                                         | Colab             | Nbviewer               |
 |:----:|:--------------:|:------------------------------------------------:|:-----------------:|:---------------------:|
 | 1   | `ipeps_energy_simulations.ipynb` | Computing ground-state energies of iPEPS Tensor Networks   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/ipeps_energy_simulations.ipynb)|
 | 2   | `Quantum_Ising_Model_Phase_Transition.ipynb` | Simulating the phase transition of the Quantum Transverse Field Ising model  | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Quantum_Ising_Model_Phase_Transition.ipynb)|
 | 3   | `Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb` | Spin-1 BLBQ tringular 2D lattice phase transition   | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)        | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/notebooks/Triangular_2d_lattice_BLBQ_Spin_1_simulation.ipynb)|
 
 
 ## Simulations
 ### Spin-1/2 Antiferromagnetic Heisenberg (AFH) model
 
-Below are some result of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS and Cube tensor networks. The AFH Hamiltonian is given by
+Below are some results of ground-state energy per-site simulated with the Simple Update algorithm over AFH Chain, Star, PEPS, and Cube tensor networks. The AFH Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/hamiltonian_eq.png?raw=true" width="" height="60">
 
-In the case of the Star tensor network lattice the AFH Hamiltonian is composite of two parts which corresponds to different type of edges (see [1]).
-The Chain, Star, PEPS and Cube infinite tensor networks are illustrated in the next figure.
+In the case of the Star tensor network lattice, the AFH Hamiltonian consists of two parts that correspond to different types of edges (see [1]).
+The Chain, Star, PEPS, and Cube infinite tensor networks are illustrated in the next figure.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Tensor_Networks_diagrams.png?raw=true" width="1000" height=""> 
 
 
-Here are the ground-state energy per-site vs inverse virtual bond-dimension simulations for the tensor networks diagrams above
+Here is the ground-state energy per-site vs. inverse virtual bond-dimension simulations for the tensor networks diagrams above
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/chain_star_peps_cube_plots.png?raw=true" width="1000" height="">
 
 ### Quantum Ising Model on a 2D Spin-1/2 Lattice
 Next, we simulated the quantum Ising model on a 2D lattice with a transverse magnetic field. Its Hamiltonian is given by
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/ising_transverse_field.png?raw=true" width="" height="100">
 
-In the plots below one can see the simulated x, z magnetization (per-site) along with the simulated energy (per-site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
+In the plots below, one can see the simulated x and z magnetization (per site) along with the simulated energy (per site). We see that the SU algorithm is able to extract the phase transition of the model around h=3.2.
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/Ising_model.png?raw=true" width="1000" height="">
 
 ### Spin-1 Simulation of a Bilinear-Biquadratic Heisenberg model on a star 2D lattice
 
-Finally we simulated the BLBQ Hamiltonian which is given by the next equation
+Finally, we simulated the BLBQ Hamiltonian, which is given by the next equation
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_hamiltonian.png?raw=true" width="300" height="">
 
-notice that for 0 radian angle, this model coincides with the original AFH model. The energy, magnetization and Q-norm as a function of the angle for different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time to trace all the phase transitions of this model. However, we notice that for larger bond dimensions it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice see Ref [2])
+notice that for the 0-radian angle, this model coincides with the original AFH model. The energy, magnetization, and Q-norm as a function of the angle for a different bond dimension are plotted below. We can see that the simple-update algorithm is having a hard time tracing all the phase transitions of this model. However, we notice that for larger bond dimensions, it seems like it captures the general behavior of the model's phase transition. For a comprehensive explanation and results (for triangular lattice, see Ref [2])
 
 <img src="https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/assets/BLBQ_model_simulation_star.png?raw=true" width="1000" height="">
 
 ## References
 - [[1]](https://arxiv.org/abs/1808.00680) Saeed S. Jahromi, and Roman Orus - "A universal tensor network algorithm for any infinite lattice" (2019)
 - [[2]](https://arxiv.org/abs/1805.00354) Ido Niesen, Philippe Corboz - "A ground state study of the spin-1 bilinear-biquadratic Heisenberg model on the triangular lattice using tensor networks" (2018)
 - [[3]](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.023073) Roy Alkabetz and Itai Arad - "Tensor networks contraction and the belief propagation algorithm" (2020)
@@ -232,18 +232,19 @@
 
 ## Contact
 
 Roy Elkabetz - [elkabetzroy@gmail.com](mailto:elkabetzroy@gmail.com)
 
 ## Citation
 
-To cite this repository in academic works or any other purpose, please use the following BibTeX citation:
-```Latex
-@software{tnsu,
-    author = {Elkabetz, Roy},
-    title = {{tnsu: A python package for Tensor Networks Simple-Update simulations}},
-    url = {https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update},
-    version = {1.0.2},
-    year = {2022}
+To cite this repository in academic works or for any other purpose, please use the following BibTeX citation:
+```
+@misc{tnsu,
+    author = "Elkabetz, Roy",
+    title = "Python Package for Universal Tensor-Networks Simple-Update Simulations",
+    howpublished = "\url{https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update}",
+    url = "https://github.com/RoyElkabetz/Tensor-Networks-Simple-Update/blob/main/tnsu__A_python_package_for_Tensor_Networks_Simple_Update_simulations.pdf",
+    year = "2022",
+    type = "Python package"
 }
 ```
```

### Comparing `tnsu-1.0.2/src/tnsu.egg-info/SOURCES.txt` & `tnsu-1.0.3/src/tnsu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

