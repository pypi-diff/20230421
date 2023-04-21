# Comparing `tmp/synapgrad-0.2.8-py3-none-any.whl.zip` & `tmp/synapgrad-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 22499 bytes, number of entries: 19
+Zip file size: 28868 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
--rw-rw-rw-  2.0 fat    21680 b- defN 23-Apr-12 10:56 synapgrad/engine.py
--rw-rw-rw-  2.0 fat      340 b- defN 23-Apr-13 21:18 synapgrad/nn/__init__.py
--rw-rw-rw-  2.0 fat     4883 b- defN 23-Apr-13 00:43 synapgrad/nn/activations.py
--rw-rw-rw-  2.0 fat     2174 b- defN 23-Apr-13 13:34 synapgrad/nn/layers.py
--rw-rw-rw-  2.0 fat     8087 b- defN 23-Apr-13 00:32 synapgrad/nn/losses.py
--rw-rw-rw-  2.0 fat     2477 b- defN 23-Apr-11 18:04 synapgrad/nn/modules.py
--rw-rw-rw-  2.0 fat     2150 b- defN 23-Apr-11 00:40 synapgrad/nn/neurons.py
+-rw-rw-rw-  2.0 fat    30875 b- defN 23-Apr-21 09:11 synapgrad/engine.py
+-rw-rw-rw-  2.0 fat      420 b- defN 23-Apr-21 10:37 synapgrad/nn/__init__.py
+-rw-rw-rw-  2.0 fat     3538 b- defN 23-Apr-20 01:42 synapgrad/nn/activations.py
+-rw-rw-rw-  2.0 fat     7831 b- defN 23-Apr-19 17:14 synapgrad/nn/functional.py
+-rw-rw-rw-  2.0 fat     2879 b- defN 23-Apr-20 12:52 synapgrad/nn/initializations.py
+-rw-rw-rw-  2.0 fat    13895 b- defN 23-Apr-21 10:27 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-20 01:41 synapgrad/nn/losses.py
+-rw-rw-rw-  2.0 fat     2654 b- defN 23-Apr-19 20:19 synapgrad/nn/modules.py
+-rw-rw-rw-  2.0 fat      997 b- defN 23-Apr-20 12:59 synapgrad/nn/neurons.py
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
--rw-rw-rw-  2.0 fat     5290 b- defN 23-Apr-13 12:38 synapgrad/optim/optimizers.py
+-rw-rw-rw-  2.0 fat     5293 b- defN 23-Apr-20 01:43 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
--rw-rw-rw-  2.0 fat     1272 b- defN 23-Apr-11 01:07 synapgrad/utils/graph.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-21 08:50 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4700 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1525 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/RECORD
-19 files, 70029 bytes uncompressed, 20025 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4488 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1696 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/RECORD
+21 files, 98171 bytes uncompressed, 26128 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -6,14 +6,20 @@
 
 Filename: synapgrad/nn/__init__.py
 Comment: 
 
 Filename: synapgrad/nn/activations.py
 Comment: 
 
+Filename: synapgrad/nn/functional.py
+Comment: 
+
+Filename: synapgrad/nn/initializations.py
+Comment: 
+
 Filename: synapgrad/nn/layers.py
 Comment: 
 
 Filename: synapgrad/nn/losses.py
 Comment: 
 
 Filename: synapgrad/nn/modules.py
@@ -36,23 +42,23 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.2.8.dist-info/LICENSE
+Filename: synapgrad-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.2.8.dist-info/METADATA
+Filename: synapgrad-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.2.8.dist-info/WHEEL
+Filename: synapgrad-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.2.8.dist-info/top_level.txt
+Filename: synapgrad-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.2.8.dist-info/RECORD
+Filename: synapgrad-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/engine.py

```diff
@@ -42,29 +42,44 @@
 
 def tensor(data, requires_grad=False, dtype=None) -> 'Tensor':
     return Tensor(data, requires_grad=requires_grad, dtype=dtype)
 
 
 class Tensor:
     
-    def __init__(self, data, _children=(), _operation=None, requires_grad=False, dtype=None) -> None:
+    def __init__(self, data, _children=(), _operation=None, requires_grad=False, dtype=None, name=None) -> None:
+        """
+        Creates a Tensor object from the given data, which is always transformed internally into a numpy array.
+
+        Args:
+            data (number or iterable): data of the tensor, must be convertible into a numpy.array().
+            _children (tuple, optional): tensors which produced this tensor as a result of an operation. Defaults to ().
+            _operation (str, optional): string that represents the operation that created this tensor. Defaults to None.
+            requires_grad (bool, optional): whether this tensor requieres gradients or not. Defaults to False.
+            dtype (type, optional): numpy type of this tensor data. Defaults to None.
+            
+        """
         if not isinstance(data, np.ndarray):
             data = np.array(data, dtype=default_type__)
         if dtype is not None and data.dtype != dtype: data = data.astype(dtype)
         assert isinstance(data, np.ndarray), "data must be a list or numpy array"
         
         self.data = data
         # Internal variables used for autograd graph construction
         self._grad = None
         self._grad_fn = None
-        self._requires_grad = requires_grad and gradient__
+        req_grad = requires_grad and gradient__
+        if req_grad and not self.is_floating_point(data):
+            raise RuntimeError("Only floating point Tensors can require gradients")
+        self._requires_grad = req_grad
         self._is_leaf = True
         self._retain_grad = False
         self._children = _children
-        self._operation = _operation # Operation that produced this node, for graphviz / debugging         
+        self._operation = _operation # Operation that produced this node, for graphviz / debugging
+        self._name = name        
     
     
     @staticmethod
     def __add_grad(tensor:'Tensor', grad:np.ndarray):
         """Function that ensures that the gradient that wants to be added is compatible
         with the tensor gradient. It is a useful function for operations like __add__ and __mul__
         when opertions like v1:(3,) (+ or *) v2:(2,3) pop up. In this case the incomming gradient
@@ -74,15 +89,14 @@
         Args:
             tensor (Tensor): Tensor whose gradient is going to be updated
             grad (np.ndarray): Gradient array to add
         """
         def get_incompatible_dims(tensor_shape, grad_shape) -> tuple:
             not_compatible_dims = []
             for i, (tdim, gdim) in enumerate(zip(tensor_shape[::-1], grad_shape[::-1])):
-                print(tdim, gdim)
                 if gdim != 1 and tdim != gdim:
                     not_compatible_dims.append(len(grad_shape)-1-i)
             not_compatible_dims = tuple(not_compatible_dims)
             return not_compatible_dims
             
         
         if len(tensor.data.squeeze().shape) == 0:
@@ -92,15 +106,15 @@
         tensor_shape = tensor.data.shape; grad_shape = grad.data.shape
         diff_axis = len(grad_shape)-len(tensor_shape)
         sum_axis = None if diff_axis <= 0 else tuple(np.arange(abs(diff_axis), dtype=np.int8).tolist())
         
         if tensor.grad.matches_shape(grad) or sum_axis is None: 
             if sum_axis is None and not tensor.grad.matches_shape(grad):
                 not_compatible_dims = get_incompatible_dims(tensor_shape, grad_shape)
-                tensor += grad.sum(axis=not_compatible_dims, keepdims=True)
+                tensor._grad += grad.sum(axis=not_compatible_dims, keepdims=True)
             else:
                 tensor._grad += grad
         else:
             tensor._grad += grad.sum(axis=sum_axis)
     
     
     def __add__(self, summand:'Tensor') -> 'Tensor':
@@ -142,18 +156,21 @@
         tensor = tensor if isinstance(tensor, Tensor) else Tensor(tensor)
         r_grad = self.requires_grad or tensor.requires_grad
         assert len(self.data.shape) > 1 and len(tensor.data.shape) > 1, "Both inputs should have dimension > 1"
         out = Tensor(self.data @ tensor.data, (self, tensor), '<Matmul>', requires_grad=r_grad)
         
         def _backward():
             if self.requires_grad:
-                self._grad += np.dot(tensor.data, out._grad.T).T
+                grad = out._grad @ np.moveaxis(tensor.data, -2, -1)
+                self.__add_grad(self, grad)
             
             if tensor.requires_grad:
-                tensor._grad += np.dot(self.data.T, out._grad)
+                grad = np.moveaxis(out._grad, -2,-1) @ self.data
+                grad = np.moveaxis(grad, -2,-1)
+                self.__add_grad(tensor, grad)
                     
         out._backward = _backward
         
         return out
     
     
     def __rmatmul__(self, tensor:'Tensor') -> 'Tensor':
@@ -261,30 +278,27 @@
                 tensor._grad += grad
 
         out._backward = _backward
         
         return out
     
     
-    @staticmethod
-    def add(t1:'Tensor', t2:'Tensor') -> 'Tensor':
-        return t1 + t2
+    def add(self, t2:'Tensor') -> 'Tensor':
+        return self + t2
     
     
-    @staticmethod
-    def mul(t1:'Tensor', t2:'Tensor') -> 'Tensor':
-        return t1 * t2
+    def mul(self, t2:'Tensor') -> 'Tensor':
+        return self * t2
     
     
-    @staticmethod
-    def matmul(t1:'Tensor', t2:'Tensor') -> 'Tensor':
-        return t1 @ t2
+    def matmul(self, t2:'Tensor') -> 'Tensor':
+        return self @ t2
     
     
-    def view(self, shape:tuple) -> 'Tensor':
+    def view(self, *shape:tuple) -> 'Tensor':
         out = Tensor(self.data.reshape(shape), (self,), '<View>', requires_grad=self.requires_grad)
         
         def _backward():
             if self.requires_grad:
                 self._grad += out._grad.reshape(self.shape)
             
         out._backward = _backward
@@ -324,36 +338,254 @@
                 self._grad += np.squeeze(out._grad, dim)
             
         out._backward = _backward
         
         return out
     
     
+    def unfold(self, dimension:int, size:int, step:int) -> 'Tensor':
+        """
+        Unfold a tensor along a specified dimension.
+
+        Parameters
+        ----------
+        tensor : Tensor
+            The tensor to unfold.
+        dimension : int
+            The dimension to unfold.
+        size : int
+            The size of the unfolding window.
+        step : int
+            The step between each unfolding window.
+
+        Returns
+        -------
+        Tensor
+            The unfolding result.
+
+        Raises
+        ------
+        ValueError
+            If the specified dimension is invalid, if the size or step are not positive integers, or if the size is
+            larger than the size of the specified dimension.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> a = np.arange(10)
+        >>> unfold(a, 0, 3, 1)
+        array([[[0, 1, 2],
+                [3, 4, 5],
+                [6, 7, 8]],
+            
+               [[9, 0, 1],
+                [2, 3, 4],
+                [5, 6, 7]]])
+        """
+        tensor = self.data
+        # check that the specified dimension is valid
+        if dimension >= tensor.ndim or dimension < -tensor.ndim:
+            raise ValueError(f"Dimension out of range for tensor with {tensor.ndim} dimensions: {dimension}")
+        if dimension < 0:
+            dimension += tensor.ndim
+        # check that the size and step are positive integers
+        if not isinstance(size, int) or size <= 0:
+            raise ValueError(f"Invalid size: {size}")
+        if not isinstance(step, int) or step <= 0:
+            raise ValueError(f"Invalid step: {step}")
+        # get the size of the specified dimension
+        dim_size = tensor.shape[dimension]
+        # check that the size is smaller than or equal to the size of the dimension
+        if size > dim_size:
+            raise ValueError(f"Size ({size}) must be smaller than or equal to the size of the specified dimension ({dim_size})")
+        # calculate the size of the output dimension
+        out_size = int((dim_size - size) / step) + 1
+        # create an output array with the appropriate shape
+        out_shape = list(tensor.shape)
+        out_shape[dimension] = out_size
+        out_shape.append(size)
+        out_array = np.zeros(out_shape, dtype=tensor.dtype)
+        # fill the output array with the unfolded slices
+        for i in range(out_size):
+            start = i * step
+            end = start + size
+            window = np.take(tensor, np.arange(start, end), axis=dimension)
+            window = np.moveaxis(window, dimension, -1)
+            out_array = np.delete(out_array, i, axis=dimension)
+            out_array = np.insert(out_array, i, window, axis=dimension)
+        
+        out = Tensor(out_array, (self,), f'<UnfoldDim{dimension}>', requires_grad=self.requires_grad)
+        
+        def _backward():
+            if self.requires_grad:
+                folded = np.zeros_like(tensor)
+                for i in range(out._grad.shape[dimension]):
+                    start = i * step
+                    end = start + size
+                    s1 = [slice(None)] * (dimension + 1); s1[dimension] = slice(start, end)
+                    s2 = [slice(None)] * (dimension + 1); s2[dimension] = i
+                    s1 = tuple(s1); s2 = tuple(s2)
+                    folded[s1] += np.moveaxis(out._grad[s2], -1, dimension).reshape(folded[s1].shape)
+                
+                self._grad += folded 
+            
+        out._backward = _backward
+
+        return out
+    
+    
+    def contiguous(self) -> 'Tensor':
+        """
+        Returns a contiguous tensor.
+
+        Returns
+        -------
+        Tensor
+            The contiguous tensor.
+        """
+        out = Tensor(np.ascontiguousarray(self.data), (self,), '<Contiguous>', requires_grad=self.requires_grad)
+        
+        def _backward():
+            if self.requires_grad:
+                self._grad += out._grad
+            
+        out._backward = _backward
+        
+        return out
+    
+    
+    @staticmethod
+    def __get_selected_from_indices(values:np.ndarray, indices:np.ndarray, dim) -> np.ndarray:
+        """
+        Returns a boolean array of the same shape as the input array, where each element is True if the corresponding
+        element in the input array is the selected value in the corresponding dimension.
+
+        Parameters
+        ----------
+        values : np.ndarray
+            The values in the input array.
+        indices : np.ndarray
+            The indices of the selected values in the input array.
+        dim : int
+            The dimension of the input array.
+
+        Returns
+        -------
+        np.ndarray
+            The boolean array.
+        """
+        def get_indices(array, dim):
+            indices = []
+            if dim == -1: dim = array.ndim - 1
+            for i in range(dim):
+                s = [None,] * dim
+                s[i] = slice(None)
+                s = tuple(s)
+                #print(s)
+                indices.append(np.arange(array.shape[i])[s])
+            return tuple(indices)
+    
+        selected = np.zeros_like(values)
+        
+        if dim is not None:
+            slices = get_indices(values, dim)
+            slices = list(slices)
+            slices.append(indices)
+            slices = tuple(slices)
+        else:
+            slices = np.unravel_index(indices, values.shape)
+
+        selected[slices] = 1
+        
+        return selected
+    
+    
     def sum(self, dim:int=None, keepdims=False) -> 'Tensor':
         out = Tensor(self.data.sum(axis=dim, keepdims=keepdims), (self,), '<Sum>', requires_grad=self.requires_grad)
         
         def _backward():
             if self.requires_grad:
                 self._grad += out._grad
             
         out._backward = _backward
         
         return out
     
     
-    def mean(self, dim:int=None) -> 'Tensor':
-        out = Tensor(self.data.mean(axis=dim), (self,), '<Mean>', requires_grad=self.requires_grad)
+    def mean(self, dim:int=None, keepdims=False) -> 'Tensor':
+        out = Tensor(self.data.mean(axis=dim, keepdims=keepdims), (self,), '<Mean>', requires_grad=self.requires_grad)
         
         def _backward():
             if self.requires_grad:
-                self._grad += (np.ones(self.shape) / self.data.size) * out._grad
+                if dim is None:
+                    size = self.data.size
+                elif isinstance(dim, int):
+                    size = self.data.shape[dim]
+                elif isinstance(dim, tuple):
+                    size = 1
+                    for d in dim: size *= self.data.shape[d]
+                self._grad += (np.ones(self.shape) / size) * out._grad
             
         out._backward = _backward
         
         return out
+
+    
+    def max(self, dim:int=None, keepdims=False, return_indices=None, return_selected=False) -> tuple['Tensor',...]:
+        max_values = self.data.max(axis=dim, keepdims=keepdims)
+        max_indices = self.data.argmax(axis=dim)
+        selected = self.__get_selected_from_indices(self.data, max_indices, dim)
+        
+        out = Tensor(max_values, (self,), '<Max>', requires_grad=self.requires_grad)
+        
+        def _backward():
+            if self.requires_grad:
+                grad = out._grad
+                if not keepdims and dim is not None:
+                    grad = np.expand_dims(grad, axis=dim)
+                self._grad += selected * grad
+            
+        out._backward = _backward
+        
+        out_tuple = (out,)
+        
+        if return_indices is not False and dim is not None:
+            out_tuple += (max_indices,)
+        
+        if return_selected:
+            out_tuple += (selected,)
+        
+        return out_tuple if len(out_tuple) > 1 else out_tuple[0]
+    
+    
+    def min(self, dim:int=None, keepdims=False, return_indices=None, return_selected=False) -> tuple['Tensor',...]:
+        min_values = self.data.min(axis=dim, keepdims=keepdims)
+        min_indices = self.data.argmin(axis=dim)
+        selected = self.__get_selected_from_indices(self.data, min_indices, dim)
+        
+        out = Tensor(min_values, (self,), '<Min>', requires_grad=self.requires_grad)
+        
+        def _backward():
+            if self.requires_grad:
+                grad = out._grad
+                if not keepdims and dim is not None:
+                    grad = np.expand_dims(grad, axis=dim)
+                self._grad += selected * grad
+            
+        out._backward = _backward
+        
+        out_tuple = (out,)
+        
+        if return_indices is not False and dim is not None:
+            out_tuple += (min_indices,)
+        
+        if return_selected:
+            out_tuple += (selected,)
+        
+        return out_tuple if len(out_tuple) > 1 else out_tuple[0]
     
     
     def transpose(self, dim0:int, dim1:int) -> 'Tensor':
         """ Transpose tensor, dim0 and dim1 are swapped (0, 1 for 2D tensor)"""
         out = Tensor(self.data.swapaxes(dim0, dim1), (self,), '<Transpose>', requires_grad=self.requires_grad)
         
         def _backward():
@@ -408,28 +640,33 @@
                 self._grad += out._grad / (2 * out.data)
                 
         out._backward = _backward
         
         return out
     
     
+    @staticmethod
+    def is_floating_point(array) -> bool:
+        return array.dtype == np.float16 or array.dtype == np.float32 or array.dtype == np.float64
+    
+    
     def backward(self, grad:np.ndarray=None):
         if not self.requires_grad:
             raise RuntimeError("Trying to call backward on Tensor with requires_grad=False")
 
         if grad is None:
             if self.data.size > 1:
                 raise RuntimeError("grad must be specified for non-scalar tensors")
             else:
                 grad = np.array(1.0, dtype=self.data.dtype)
-                
+        
+        assert self.is_floating_point(grad), "expected float dtype for grad, got %s" % grad.dtype
+          
         if not isinstance(grad, np.ndarray):
             raise ValueError("Gradient parameter must be a numpy array")
-                
-        self._is_leaf = True
         
         # Topological order all of the children in the graph 
         # (init gradients for those who are going to need it)
         ordered_nodes = []
         visited_nodes = set()
         def visit_node(node):
             if node not in visited_nodes:
@@ -481,15 +718,21 @@
         if len(self.shape) != len(tensor.shape):
             return False
         
         for n1, n2 in zip(self.shape, tensor.shape):
             if n1 != n2: return False
         
         return True
-                
+        
+        
+    @property
+    def name(self) -> str:
+        return "" if self._name is None else str(self._name)
+        
+        
     @property
     def shape(self) -> tuple:
         return self.data.shape
     
     @property
     def dtype(self) -> np.dtype:
         return self.data.dtype
@@ -508,15 +751,18 @@
     
     @requires_grad.setter
     def requires_grad(self, value:bool):
         if not self.is_leaf:
             raise RuntimeError("you can only change requires_grad flags of leaf variables. " + 
                     "If you want to use a computed variable in a subgraph that doesn't require " + 
                     "differentiation use var_no_grad = var.detach()")
-            
+        
+        if value and not self.is_floating_point(self.data):
+            raise RuntimeError("Only floating point Tensors can require gradients")
+        
         self._requires_grad = value
     
     @property
     def grad(self) -> 'Tensor':
         if not self._is_leaf and not self._retain_grad:
             print("\n[!] WARNING: The .grad attribute of a Tensor that is not a " + 
                   "leaf Tensor is being accessed. Its .grad attribute won't be populated " + 
@@ -567,40 +813,34 @@
     def __truediv__(self, other) -> 'Tensor': # self / other
         return self * other**-1
 
     def __rtruediv__(self, other) -> 'Tensor': # other / self
         return other * self**-1
     
     @staticmethod
-    def pretty_numpy(array:np.ndarray, decimals=5) -> str:
-        def truncate(f, n):
-            return np.floor(f * 10 ** n) / 10 ** n
-        rounded_data = array.copy().round(decimals=decimals)
-        #rounded_data += 0. # Remove -0.0 values (just 0.0)
-        str_to_rm = "array("
-        data_str = repr(rounded_data).replace(str_to_rm, "")
-        crop_index = (len(data_str)) - data_str[::-1].find("]")
-        cropped = data_str[:crop_index]
-        
-        braces_padd = (len(array.shape)-1)
-        no_padding = cropped.replace("\n" + " "*(braces_padd+len(str_to_rm)), "\n" + " "*braces_padd)
-        return no_padding
+    def pretty_numpy(array:np.ndarray, precision=4, separator=',') -> str: 
+        data_str = np.array2string(array, precision=precision, separator=separator)
+        return data_str
         
     def __repr__(self) -> str:
         pretty_data_str = self.pretty_numpy(self.data)
         beggining = "Tensor("
         data_str = ""
         for i, line in enumerate(pretty_data_str.splitlines(keepends=True)):
             if i != 0:
-                line = " "*len(beggining) + line  
+                line = " "*len(beggining) + line
             data_str += line
         string = f"{beggining}{data_str}, shape={self.shape}"
         
         if self.requires_grad:
             string += f", req_grad={self.requires_grad}"
             
         if self._operation is not None:
-            string += f", op={self._operation})"
+            string += f", op={self._operation}"
+            
+        if self._name is not None:
+            string += f", name={self._operation}"
+            
             
-        string += ")"
+        string += f", dtype={self.dtype})"
             
         return string
```

## synapgrad/nn/__init__.py

```diff
@@ -1,6 +1,8 @@
 
 from .modules import Module, Sequential
 from .neurons import Neuron
-from .layers import Linear, Flatten #, Conv2D, BatchNorm2d, MaxPool2D
+from .layers import Linear, Flatten, Unfold, Fold, Conv2d, MaxPool2d, Dropout# , BatchNorm2d
 from .losses import Loss, MSELoss, CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss
-from .activations import relu_fn, ReLU, Tanh, tanh_fn, sigmoid_fn, Sigmoid, softmax_fn, Softmax, LogSoftmax
+from .activations import relu_fn, ReLU, Tanh, tanh_fn, sigmoid_fn, Sigmoid, softmax_fn, Softmax, LogSoftmax
+from . import functional
+from . import initializations
```

## synapgrad/nn/activations.py

```diff
@@ -1,47 +1,17 @@
 import numpy as np
 from .. import Tensor, nn
+from .functional import relu_fn, tanh_fn, sigmoid_fn, softmax_fn,  log_softmax_fn, epsilon
 
 
-# ---------------------------- Functions ----------------------------
-# -------------------------------------------------------------------
-def relu_fn(data:np.ndarray) -> np.ndarray:
-    return np.maximum(0, data)
-
-
-def tanh_fn(data:np.ndarray) -> np.ndarray:
-    return np.tanh(data)
-
-
-def sigmoid_fn(data:np.ndarray) -> np.ndarray:
-    return 1/(1 + np.exp(-data))
-
-
-def softmax_fn(data:np.ndarray, dim:int) -> np.ndarray:
-    # Shift to make it numerically stable (with large values 'inf' appears)
-    shiftx = data - data.max(axis=dim, keepdims=True) 
-    exps = np.exp(shiftx)
-    exp_sums = exps.sum(axis=dim, keepdims=True)
-    return exps / exp_sums
-
-def log_softmax_fn(data:np.ndarray, dim:int) -> np.ndarray:
-    # Using log-sum-exp trick for numerical stability
-    max_val = data.max(axis=dim, keepdims=True)
-    substract = data - max_val
-    exp = np.exp(substract)
-    lse = max_val + np.log(exp.sum(axis=dim, keepdims=True))
-    log_softmax = data - lse
-    return log_softmax
-
 # ----------------------------- Modules -----------------------------
 # -------------------------------------------------------------------
 class ReLU(nn.Module):
     
     def forward(self, x:Tensor) -> Tensor:
-        assert isinstance(x, Tensor), "Input must be a Tensor" 
         relu = relu_fn(x.data)
         out = Tensor(relu, (x,), '<ReLU>', requires_grad=x.requires_grad)
 
         def _backward():
             if x.requires_grad:
                 x._grad += (out.data > 0) * out._grad
         
@@ -50,15 +20,14 @@
         return out
 
 
 class Tanh(nn.Module):
     """ np.sinh(x)/np.cosh(x) or -1j * np.tan(1j*x) """
     
     def forward(self, x:Tensor) -> Tensor:
-        assert isinstance(x, Tensor), "Input must be a Tensor"
         tanh = tanh_fn(x.data)
         out = Tensor(tanh, (x,), '<Tanh>', requires_grad=x.requires_grad)
     
         def _backward():
             if x.requires_grad:
                 x_grad = 1 - tanh**2
                 x._grad += x_grad * out._grad
@@ -67,42 +36,39 @@
         
         return out
 
 
 class Sigmoid(nn.Module):
     
     def forward(self, x:Tensor) -> Tensor:
-        # Returning (1/(1 + np.e**-x)) should be enough, but defining explicit 
-        # grad function should be faster
-        assert isinstance(x, Tensor), "Input must be a Tensor"
         sigmoid = sigmoid_fn(x.data)
         out = Tensor(sigmoid, (x,), '<Sigmoid>', requires_grad=x.requires_grad)
     
         def _backward():
             if x.requires_grad:
                 x_grad = sigmoid * (1 - sigmoid)
                 x._grad += x_grad * out._grad
             
         out._backward = _backward
         
         return out
 
     
 class Softmax(nn.Module):
-    """ References: 
-            https://eli.thegreenplace.net/2016/the-softmax-function-and-its-derivative/
-            https://aimatters.wordpress.com/2019/06/17/the-softmax-function-derivative/
+    """ 
+    References: 
+        https://eli.thegreenplace.net/2016/the-softmax-function-and-its-derivative/
+        https://aimatters.wordpress.com/2019/06/17/the-softmax-function-derivative/
     """
     
     def __init__(self, dim) -> None:
         super().__init__()
         self.dim = dim
     
     def forward(self, x: Tensor) -> Tensor:
-        assert isinstance(x, Tensor), "Input must be a Tensor"
         softmax = softmax_fn(x.data, self.dim)
         out = Tensor(softmax, (x,), '<Softmax>', requires_grad=x.requires_grad)
     
         def _backward():
             # Hand made derivation
             if x.requires_grad:
                 jacobians = np.stack([np.diag(y) - np.outer(y, y) for y in softmax])
@@ -111,32 +77,34 @@
             
         out._backward = _backward
         
         return out
 
     
 class LogSoftmax(nn.Module):
-    """ Same as Softmax(dim=self.dim)(x).log() but more numerically stable due to the log-sum-exp trick
-            Reference to log-sum-exp trick: https://en.wikipedia.org/wiki/LogSumExp 
+    """ 
+    Same as Softmax(dim=self.dim)(x).log() but more numerically stable due to the log-sum-exp trick
+            
+    Reference to log-sum-exp trick: 
+        https://en.wikipedia.org/wiki/LogSumExp 
     """
     
     def __init__(self, dim) -> None:
         super().__init__()
         self.dim = dim
     
     def forward(self, x: Tensor) -> Tensor:
-        assert isinstance(x, Tensor), "Input must be a Tensor"
         log_softmax = log_softmax_fn(x.data, self.dim)
         out = Tensor(log_softmax, (x,), '<LogSoftmax>', requires_grad=x.requires_grad)
     
         def _backward():
             if x.requires_grad:
                 softmax = np.exp(log_softmax)
                 jacobians = np.stack([np.diag(y) - np.outer(y, y) for y in softmax])
-                dlog_dsoftmax = (1/softmax) * out._grad
+                dlog_dsoftmax = (1/(softmax + epsilon)) * out._grad
                 dlog_dsoftmax = np.expand_dims(dlog_dsoftmax, axis=self.dim)
                 x._grad += (dlog_dsoftmax @ jacobians).sum(axis=self.dim)
             
         out._backward = _backward
         
         return out
```

## synapgrad/nn/layers.py

```diff
@@ -1,69 +1,346 @@
 import numpy as np
 from .. import nn, Tensor
 from .neurons import init_weights
+from .functional import unfold, fold
+from .initializations import init_weights
 
 
 class Linear(nn.Module):
     
-    def __init__(self, input_size:int, output_size:int, weight_init_method='he'):
+    def __init__(self, input_size:int, output_size:int, weight_init_method='he_normal'):
         super().__init__()
         self.input_size = input_size
         self.output_size = output_size
-        # Randomly initialize weights and biases
-        weight_values = [ init_weights(input_size, output_size, weight_init_method).astype(np.float32) for _ in range(output_size) ]
+        
+        self.weight_init_method = weight_init_method
+        weight_values = init_weights((output_size, input_size), weight_init_method).astype(np.float32)
         self.weights = Tensor(weight_values, requires_grad=True)
-        self.biases = Tensor(np.zeros((output_size,), dtype=np.float32), requires_grad=True)
+        self.bias = Tensor(np.zeros((output_size,), dtype=np.float32), requires_grad=True)
         
     def forward(self, x:Tensor) -> Tensor:
         assert x.shape[1] == self.input_size, f"Expected input size '{self.input_size}' but received '{x.shape[1]}'"
 
-        out = (x @ self.weights.transpose(0,-1)) + self.biases
+        out = (x @ self.weights.transpose(0,-1)) + self.bias
         
         return out
     
     def parameters(self) -> list[Tensor]:
-        return [self.weights, self.biases]
+        return [self.weights, self.bias]
     
     def __repr__(self) -> str:
         return f"Linear(input_size={self.input_size}, neurons={len(self.output_size)})"
 
 
 class Flatten(nn.Module):
     
     def __init__(self, start_dim=1, end_dim=-1) -> None:
         super().__init__()
         self.start_dim = start_dim
         self.end_dim = end_dim
     
     def forward(self, x: Tensor) -> Tensor:
         return x.flatten(self.start_dim, self.end_dim)
+    
+    
+class Unfold(nn.Module):
+    """ Check nn.funcional.unfold for more information """
+    
+    def __init__(self, kernel_size, stride=1, padding=0, dilation=1, pad_value=0) -> None:
+        super().__init__()
+        
+        kernel_size = np.broadcast_to(kernel_size, 2)
+        dilation = np.broadcast_to(dilation, 2)
+        padding = np.broadcast_to(padding, 2)
+        stride = np.broadcast_to(stride, 2)
+        
+        self.kernel_size = kernel_size
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
+        self.pad_value = pad_value
+        
+    def forward(self, x: Tensor) -> Tensor:
+        N, C, H, W = x.shape
+        unfolded = unfold(x.data, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
+                           padding=self.padding, pad_value=self.pad_value)
+        
+        out = Tensor(unfolded, (x,), "<Unfold>", requires_grad=x.requires_grad)
+        
+        def _backward():
+            if x.requires_grad:
+                grad = fold(out._grad, (H,W), kernel_size=self.kernel_size, stride=self.stride,
+                     dilation=self.dilation, padding=self.padding)
+
+                x._grad += grad
+                
+        out._backward = _backward
+    
+        return out
+    
+    
+class Fold(nn.Module):
+    """ Check nn.funcional.fold for more information """
+    
+    def __init__(self, output_size, kernel_size, stride=1, padding=0, dilation=1) -> None:
+        super().__init__()
+        
+        output_size = np.broadcast_to(output_size, 2)
+        kernel_size = np.broadcast_to(kernel_size, 2)
+        dilation = np.broadcast_to(dilation, 2)
+        padding = np.broadcast_to(padding, 2)
+        stride = np.broadcast_to(stride, 2)
+        
+        self.output_size = output_size
+        self.kernel_size = kernel_size
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
+        
+    def forward(self, x: Tensor) -> Tensor:
+        folded = fold(x.data, self.output_size, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
+                           padding=self.padding)
+        
+        out = Tensor(folded, (x,), "<Fold>", requires_grad=x.requires_grad)
+        
+        def _backward():
+            if x.requires_grad:
+                grad = unfold(out._grad, kernel_size=self.kernel_size, stride=self.stride,
+                     dilation=self.dilation, padding=self.padding)
 
+                x._grad += grad
+                
+        out._backward = _backward
+    
+        return out
+    
 
-class Conv2D(nn.Module):
+class MaxPool2d(nn.Module):
     
-    def __init__(self, filters, kernel_size, strides=None, padding=None) -> None:
-        self.filters = filters
+    def __init__(self, kernel_size, stride=None, padding=0, dilation=1) -> None:
+        """
+        Applies Max Pooling 2D to a batch of N images with C channels (N, C, H, W).
+        References:
+            https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html
+
+        Args:
+            kernel_size (int or tuple): the size of the sliding blocks
+            stride (int or tuple, optional): the stride of the sliding blocks in the input spatial dimensions. Default: 1
+            padding (int or tuple, optional):  implicit zero padding to be added on both sides of input. Default: 0
+            dilation (int or tuple, optional): a parameter that controls the stride of elements within the neighborhood. Default: 1
+
+        Output:
+            Tensor of shape (N, C, H // stride[0], W // stride[1]).
+        """
+        super().__init__()
+        
+        kernel_size = np.broadcast_to(kernel_size, 2)
+        if stride is None:
+            stride = kernel_size
+        else:
+            stride = np.broadcast_to(stride, 2)
+        padding = np.broadcast_to(padding, 2)
+        dilation = np.broadcast_to(dilation, 2)
+        
         self.kernel_size = kernel_size
-        self.strides = strides
+        self.stride = stride
         self.padding = padding
+        self.dilation = dilation
+        
+    def forward(self, x: Tensor) -> Tensor: 
+        N, C, H, W = x.shape
+        lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
+        lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
+        
+        unfolded = unfold(x.data, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
+                           padding=self.padding, pad_value=-np.inf)
+        
+        N, C_k, L = unfolded.shape
+        split_per_channel = unfolded.reshape(N, C, int(C_k/C), L)
+        
+        unfolded_reorganized = np.moveaxis(split_per_channel, -2, -1).reshape(N, C, lH, lW, -1)
+        pooled, max_indices, selected = Tensor(unfolded_reorganized).max(dim=-1, return_selected=True)
+    
+        out = Tensor(pooled.data, (x,), "<MaxPool2d>", requires_grad=x.requires_grad)
+        
+        def _backward():
+            if x.requires_grad:
+                grad = selected * np.expand_dims(out._grad, axis=-1)
+
+                grad = grad.reshape(N, C, L, int(C_k/C))
+                grad = np.moveaxis(grad, -1, -2)
+                grad = grad.reshape(N, C_k, L)
+                
+                grad = fold(grad, (H,W), kernel_size=self.kernel_size, stride=self.stride,
+                     dilation=self.dilation, padding=self.padding)
+
+                x._grad += grad
+                
+        out._backward = _backward
+        
+        return out
+
+
+class Conv2d(nn.Module):
+    
+    def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, weight_init_method='he_uniform') -> None:
+        """
+        Applies 2D Convolution to a batch of N images with C channels (N, C, H, W).
+        Reference:
+            https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
+
+        Args:
+            in_channels (int): the number of input channels
+            out_channels (int): the number of output channels produced by the convolution
+            kernel_size (int or tuple): the size of the sliding blocks
+            stride (int or tuple, optional): the stride of the sliding blocks in the input spatial dimensions. Default: 1
+            padding (int or tuple, optional):  implicit zero padding to be added on both sides of input. Default: 0
+            dilation (int or tuple, optional): a parameter that controls the stride of elements within the neighborhood. Default: 1
+        """
+        super().__init__()
+        
+        kernel_size = np.broadcast_to(kernel_size, 2)
+        if stride is None:
+            stride = kernel_size
+        else:
+            stride = np.broadcast_to(stride, 2)
+        
+        if padding == 'same':
+            if any(s != 1 for s in stride):
+                raise ValueError("padding='same' is not supported for strided convolutions")
+            padding = int(np.floor(kernel_size[0] / 2))
+        if padding == 'valid':
+            padding = 0
+        padding = np.broadcast_to(padding, 2)
+        dilation = np.broadcast_to(dilation, 2)
+        
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.kernel_size = kernel_size
+        self.stride = stride
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
+        
+        self.weight_init_method = weight_init_method
+        weight_values = init_weights((out_channels, in_channels, *kernel_size), weight_init_method).astype(np.float32)
+        self.weights = Tensor(weight_values, requires_grad=True)
+        self.bias = Tensor(np.zeros((out_channels,), dtype=np.float32), requires_grad=True)
     
     def forward(self, x: Tensor) -> Tensor:
-        return super().forward(x)
+        N, C, H, W = x.shape
+        lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
+        lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
+        
+        unfolded = Unfold(kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
+                           padding=self.padding, pad_value=0)(x)
+        
+        weights = self.weights.view(self.weights.shape[0], -1).transpose(0,1) 
+        mult = unfolded.transpose(1,2) @ weights
+        convolved = (mult) + self.bias
+        out = convolved.transpose(1,2).view(N, self.out_channels, lH, lW)
+
+        return out
+        
+    def parameters(self) -> list['Tensor']:
+        return [self.weights, self.bias]
+    
+    def __repr__(self) -> str:
+        return (f"Conv2d(in_channels={self.in_channels}, out_channels={self.out_channels}, " + 
+                f"kernel_size={self.kernel_size}, stride={self.stride}, padding={self.padding}, " + 
+                f"dilation={self.dilation}")
     
     
 class BatchNorm2d(nn.Module):
-    
-    def __init__(self) -> None:
+    """
+    TODO: This layer is not working properly yet
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
+    """
+    
+    def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
+                 track_running_stats:bool=True) -> None:
+        """
+        Computes the batchnorm2d of a 4-dimensional tensor and its gradient.
+
+        Arguments:
+        x: tensor of shape (N, C, H, W) representing a batch of images.
+        gamma: tensor of shape (C,) representing the normalization scale.
+        beta: tensor of shape (C,) representing the normalization bias.
+        eps: small constant to avoid division by zero in variance computation.
+        momentum: exponential moving average factor for the mean and variance.
+        track_running_stats: 
+        """
         super().__init__()
+        self.num_features = num_features
+        self.eps = eps
+        self.momentum = momentum
+        self.affine = affine
+        self.track_running_stats = track_running_stats
         
+        self.running_mean = None
+        self.running_var = None
+        
+        if affine:
+            self.gamma = Tensor(np.ones(num_features), requires_grad=True, dtype=np.float32, name="gamma")
+            self.beta = Tensor(np.zeros(num_features), requires_grad=True, dtype=np.float32, name="beta")
+            
+            
     def forward(self, x: Tensor) -> Tensor:
-        return super().forward(x)
+        N, C, H, W = x.shape
+        num_examples = N*H*W
+        assert C == self.num_features, f"Expected {self.num_features} channels, got {C}."
+        # Compute the mean of each channel
+        mu = x.mean(dim=(0,2,3), keepdims=True)
+
+        # Compute the variance of each channel
+        var = ((x - mu)**2).mean(dim=(0,2,3), keepdims=True)
+        std = (var + self.eps).sqrt()
+
+        # Update the running average of mean and variance
+        if self.track_running_stats:
+            if self.running_mean is None:
+                self.running_mean = mu
+            else:
+                self.running_mean = (self.momentum * self.running_mean + (1 - self.momentum) * mu)
+            
+            if self.running_var is None:
+                self.running_var = var
+            else:
+                self.running_var = (self.momentum * self.running_var + (1 - self.momentum) * var)
+
+        # Normalize the input tensor
+        x_norm = (x - mu) / std
+
+        # Scale and shift the normalization
+        if self.affine:
+            out = self.gamma.view(1,C,1,1) * x_norm + self.beta.view(1,C,1,1)
+        else:
+            out = x_norm
+        
+        return out
+
+    def parameters(self) -> list[Tensor]:
+        return [self.gamma, self.beta] if self.affine else []    
     
+
+class Dropout(nn.Module):
+    """ 
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html
     
-class MaxPool2D(nn.Module):
+    """
     
-    def __init__(self) -> None:
+    def __init__(self, p=0.5, inplace=False) -> None:
         super().__init__()
+        self.p = p
+        self.inplace = inplace
         
     def forward(self, x: Tensor) -> Tensor:
-        return super().forward(x)
+        if not self.training: return x
+        random_data = np.random.rand(*x.shape)
+        random_data = np.where(random_data <= self.p, 0, 1)
+        if self.p < 1:
+            random_data = random_data / (1-self.p) # scale data
+        random_t = Tensor(random_data)
+        
+        return x*random_t
```

## synapgrad/nn/losses.py

```diff
@@ -1,47 +1,17 @@
 from typing import Any
 from abc import ABC, abstractmethod
 from .. import Tensor
-from .activations import softmax_fn, relu_fn
+from .functional import (
+    mse_loss, nll_loss, cross_entropy_loss, bce_loss, softmax_fn,
+    bce_with_logits_loss, relu_fn, epsilon
+)
 import numpy as np
 
 
-epsilon = 1e-12
-
-# ---------------------------- Functions ----------------------------
-# -------------------------------------------------------------------
-def mse_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    loss = (y_pred - y_true)**2
-    return loss
-    
-    
-def nll_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    loss = -y_pred[range(len(y_pred)), y_true].reshape((-1, 1))
-    return loss
-
-
-def bce_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    assert y_pred.max() <= 1 and y_pred.min() >= 0, "BCELoss inputs must be between 0 and 1"
-    loss = - (y_true * np.log(y_pred + epsilon) + (1 - y_true) * np.log(1 - y_pred + epsilon))
-    # For compatibility with pytorch (returns 100 when y_pred=0 and y_true=1; vice versa)
-    loss = np.where(loss == -np.log(epsilon), 100, loss) 
-    return loss
-
-
-def bce_with_logits_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    tn = -relu_fn(y_pred)
-    loss = (1-y_true) * y_pred + tn + np.log(np.exp(-tn) + np.exp((-y_pred-tn)))
-    return loss
-
-
-def cross_entropy_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    softmax = np.log(softmax_fn(y_pred, 1) + epsilon)
-    log_likelihood = nll_loss(softmax, y_true)
-    return log_likelihood
-
 # ----------------------------- Modules -----------------------------
 # -------------------------------------------------------------------
 class Loss(ABC):
     
     def __init__(self, reduction='mean') -> None:
         self.reduction = reduction
         
@@ -84,23 +54,25 @@
         
         loss._backward = _backward
         
         return loss
 
 
 class NLLLoss(Loss):
-    """ This class expects y_true to be the probabilities of a LogSoftmax function. Also, y_pred 
-        should be shape=(batch, num_classes). It expects to receive the probability of a sample to be of each class.
-        For binary classification problems, output should not be a scalar value (0 <= x <=1) but an array with 
-        the probability of each class [0.3, 0.7]
-        reference: https://towardsdatascience.com/cross-entropy-negative-log-likelihood-and-all-that-jazz-47a95bd2e81    
+    """ 
+    This class expects y_true to be the probabilities of a LogSoftmax function. Also, y_pred 
+    should be shape=(batch, num_classes). It expects to receive the probability of a sample to be of each class.
+    For binary classification problems, output should not be a scalar value (0 <= x <=1) but an array with 
+    the probability of each class [0.3, 0.7]
+    
+    Reference: 
+        https://towardsdatascience.com/cross-entropy-negative-log-likelihood-and-all-that-jazz-47a95bd2e81    
     """
     
     def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
-        assert isinstance(y_pred, Tensor) and isinstance(y_true, Tensor), "Inputs must be Tensors"
         req_grad = y_pred.requires_grad or y_true.requires_grad
         log_likelihood = nll_loss(y_pred.data, y_true.data)
         loss = Tensor(log_likelihood, (y_pred, y_true), '<NLLLoss>', requires_grad=req_grad)
         
         def _backward():
             # Hand made derivation
             if y_pred.requires_grad:
@@ -131,15 +103,16 @@
         
         loss._backward = _backward
         
         return loss
 
 
 class BCEWithLogitsLoss(Loss):
-    """ This loss combines a Sigmoid layer and the BCELoss in one single class.
+    """ 
+    This loss combines a Sigmoid layer and the BCELoss in one single class.
     This version is more numerically stable than using a plain Sigmoid followed by a BCELoss as,
     by combining the operations into one layer, we take advantage of the log-sum-exp
     trick for numerical stability
     
     References:
         https://pytorch.org/docs/stable/generated/torch.nn.BCEWithLogitsLoss.html
         https://stackoverflow.com/questions/66906884/how-is-pytorchs-class-bcewithlogitsloss-exactly-implemented
@@ -163,16 +136,19 @@
         
         loss._backward = _backward
         
         return loss
     
     
 class CrossEntropyLoss(Loss):
-    """ Same as:\n
-    log_softmax = LogSoftmax(dim=1)(y_pred)\n
+    """ 
+    Same as:
+    
+    log_softmax = LogSoftmax(dim=1)(y_pred)
+    
     loss = NLLLoss(reduction=None)(log_softmax, y_true)
     
     Reference: https://deepnotes.io/softmax-crossentropy#:~:text=Cross%20entropy%20indicates%20the%20distance,used%20alternative%20of%20squared%20error
     """
     
     def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
         """
```

## synapgrad/nn/modules.py

```diff
@@ -2,25 +2,30 @@
 from .. import Tensor
     
 
 class Module(ABC):
     
     def __init__(self) -> None:
         self.modules = []
-        self.training = False
+        self.training = True
         
     def train(self):
         """ Set module to train mode"""
         self.training = True
+        for m in self.modules:
+            m.train()
         
     def eval(self):
         """ Set module to evaluation mode """
         self.training = False
+        for m in self.modules:
+            m.eval()
         
     def __call__(self, batch:Tensor) -> Tensor:
+        assert isinstance(batch, Tensor), "Input must be a Tensor" 
         if len(batch.shape) <= 1:
             raise ValueError(f"Module '{self.__class__.__name__}' expects a batched input, Shape=(batch_size, *), but received {batch.shape}")
 
         return self.forward(batch)
 
     def zero_grad(self):
         for p in self.parameters():
```

## synapgrad/nn/neurons.py

```diff
@@ -1,68 +1,29 @@
-import math
 import numpy as np
 from .. import Tensor, nn
+from .initializations import init_weights
 
 
-weight_initializers = ['glorot', 'glorot_norm', 'he']
-
 
 class Neuron(nn.Module):
     
-    def __init__(self, inputs:int, weight_init_method='he') -> None:
+    def __init__(self, inputs:int, weight_init_method='he_normal') -> None:
         self.inputs = inputs
+        
         # Randomly initialize weights and bias
-        weight_values = np.expand_dims(init_weights(inputs, 1, weight_init_method), 0).astype(np.float32)
+        self.weight_init_method = weight_init_method
+        weight_values = init_weights((1, inputs), weight_init_method).astype(np.float32)
         self.weights = Tensor(weight_values, requires_grad=True)
         self.bias = Tensor([0], requires_grad=True)
     
     def forward(self, x:Tensor) -> Tensor:
         assert x[0].matches_shape(self.weights[0]), f"Expected input size '{self.weights[0].shape}' but received '{x[0].shape}'"
 
         out = (x @ self.weights.transpose(0,-1)) + self.bias
     
         return out
 
     def parameters(self):
         return [self.weights, self.bias]
 
     def __repr__(self) -> str:
-        return f"Neuron(weights={self.weights}, bias={self.bias})"
-
-
-def init_weights(inputs, outputs, method) -> np.ndarray:
-    if method not in weight_initializers:
-        raise ValueError(f"'{method}' is not a valid weight initializer")
-    
-    if method == 'glorot': return glorot(inputs)
-    elif method == 'glorot_norm': return glorot_norm(inputs, outputs)
-    elif method == 'he': return he(inputs)
-    
-
-def he(nodes) -> np.ndarray:
-    std = math.sqrt(2.0 / nodes)
-    # generate random numbers
-    numbers = np.random.randn(nodes)
-    # scale to the desired range
-    scaled = numbers * std
-    
-    return scaled
-    
-        
-def glorot(nodes) -> np.ndarray:
-    lower = -(1.0 / math.sqrt(nodes))
-    upper = (1.0 / math.sqrt(nodes))
-    numbers = np.random.rand(nodes)
-    scaled = lower + numbers * (upper - lower)
-    
-    return scaled
-
-
-def glorot_norm(nodes_in, nodes_out) -> np.ndarray:
-    lower = -(math.sqrt(6.0) / math.sqrt(nodes_in + nodes_out))
-    upper = (math.sqrt(6.0) / math.sqrt(nodes_in + nodes_out))
-    # generate random numbers
-    numbers = np.random.rand(nodes_in)
-    # scale to the desired range
-    scaled = lower + numbers * (upper - lower)
-    
-    return scaled
+        return f"Neuron(weights={self.weights}, bias={self.bias})"
```

## synapgrad/optim/optimizers.py

```diff
@@ -19,15 +19,16 @@
         
     @abstractmethod
     def step(self):
         self.t += 1
 
 
 class SGD(Optimizer):
-    """Reference: 
+    """
+    Reference: 
         https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
     """
     
     def __init__(self, parameters: list[Tensor], lr=0.001, momentum=0, dampening=0,
                  weight_decay=0, nesterov=False, maximize=False) -> None:
         """
         Implements stochastic gradient descent (optionally with momentum).
@@ -76,19 +77,20 @@
                     else:
                         grad = self.momentum_buffer[i]
                 
                 # Update Parameter
                 if self.maximize:
                     p.data += self.lr*grad
                 else:
-                    p.data -= p.data - self.lr*grad
+                    p.data -= self.lr*grad
         
     
 class Adam(Optimizer):
-    """Reference: 
+    """
+    Reference: 
         https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
     """
     
     def __init__(self, parameters: list[Tensor], lr=0.001, betas=(0.9, 0.999), eps=1e-8,
                     weight_decay=0, maximize=False) -> None:
         """
         Implements Adam algorithm.
```

## synapgrad/utils/graph.py

```diff
@@ -21,17 +21,18 @@
     """
     assert rankdir in ['LR', 'TB']
     nodes, edges = trace(root)
     dot = Digraph(format=format, graph_attr={'rankdir': rankdir}) #, node_attr={'rankdir': 'TB'})
     
     for n in nodes:
         nid = str(id(n))
-        data_str = Tensor.pretty_numpy(n.data, decimals=2)
-        grad_str = 'None' if n._grad is None else Tensor.pretty_numpy(n._grad, decimals=2)
-        dot.node(name=nid, label=f"<<b>Tensor</b> | data={data_str} | req_grad={n.requires_grad}   is_leaf={n.is_leaf} | grad={grad_str}>", shape='record')
+        data_str = Tensor.pretty_numpy(n.data, precision=2)
+        grad_str = 'None' if n._grad is None else Tensor.pretty_numpy(n._grad, precision=2)
+        header = f"Tensor ({n.name})" if n.name != "" else "Tensor"
+        dot.node(name=nid, label=f"<<b>{header}</b> | data={data_str} | req_grad={n.requires_grad}   is_leaf={n.is_leaf} | grad={grad_str}>", shape='record')
         if n._operation:
             dot.node(name=nid + n._operation, label=n._operation)
             dot.edge(nid + n._operation, nid)
     
     for n1, n2 in edges:
         dot.edge(str(id(n1)), str(id(n2)) + n2._operation)
```

## Comparing `synapgrad-0.2.8.dist-info/LICENSE` & `synapgrad-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synapgrad-0.2.8.dist-info/METADATA` & `synapgrad-0.2.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapgrad
-Version: 0.2.8
+Version: 0.2.9
 Summary: An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 Home-page: https://github.com/pgmesa/synapgrad
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -15,16 +15,14 @@
 License-File: LICENSE
 Requires-Dist: numpy (>=1.21.0)
 
 #  SynapGrad
 
 An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 
-> :warning: This project is not yet fully completed. Please review the following sections for updates on [next steps](#todo-list). 
-
 ## Technical Description
 This project implements a completely functional engine for tracking operations between Tensors, by dynamically building a Directed Acyclic Graph (DAG), and an automatic backpropagation algorithm (reverse-mode autodiff) over this DAG.
 
 Built on top of the engine, the deep learning library implements the most common functions, layers, losses and optimizers in order to create MLPs and CNNs able to solve AI problems
 
 This library tries to mimic Pytorch in a simplified way, but with similar functions and behaviour. 
 
@@ -62,43 +60,41 @@
 
 out1 = Tensor.stack((a.squeeze(), b.squeeze()))[0]
 out2 = Tensor.concat((a*c, b), dim=1).transpose(0, 1)[0, :]
 out = out1 @ out2.view(3).unsqueeze(1)
 print(out) # outcome of this forward pass
 out.sum().backward()
 
-print(a.grad) # da/dout
-print(c.grad) # dc/dout
+print(a.grad) # dout/da
+print(c.grad) # dout/dc
 ```
 
 ## Training examples using synapgrad
 
 This project comes with 3 jupyter notebooks (in `examples/`) that solve 3 beginner's problems in AI:
 
 - [x] 1. Basic MLP for binary classification (sklearn 'make_moons' toy dataset)
 - [x] 2. MLP for handwritten digits classification (MNIST dataset) 
-- [ ] 3. CNN for handwritten digits classification (MNIST dataset)
-
-> :warning: The 3rd example has not been implemented yet
+- [x] 3. CNN for handwritten digits classification (MNIST dataset)
 
 Example 1 (synapgrad MLP solution)     |  Example 2 and 3
 :-------------------------:|:-------------------------:
 ![Image 1](/assets/example_moons.png) | ![Image 2](/assets/example_mnist.png) 
 
 ## Comparisons with other frameworks
 In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd).
 
 
 | Training Example | synapgrad | torch | micrograd |
 |     :---:        |  :---:  |  :---:  |   :---:   |  
 | 1 | 1.7 s | 1.5 s | 1 min 43 s |
 | 2 | 52 s | 31 s | - |
-| 3 |  -  |  -  | - |
+| 3 |  16 min 7 s  |  1 min 52 s  | - |
 
-As it can be seen, synapgrad is quite fast
+As it can be seen, pytorch is much better optimized for convolutional operations.
 
 ## Graph Visualization
 In the `examples/trace_graph.ipynb` notebook there is an example of how to display the graph that synapgrad creates in the background as operations are chained.
 
 ```python
 import synapgrad
 from synapgrad import nn, utils
@@ -118,10 +114,7 @@
 
 ## Running tests
 To run the unit tests you will have to install PyTorch. In these tests, gradients calculation as well as losses, layers, etc, are assessed with pytorch to check everything is working fine. To run the tests:
 ```bash
 python -m pytest
 ```
 
-## ToDo list
-- Implement training example 3 (Conv2D, MaxPool2D, BatchNorm2D)
-
```

## Comparing `synapgrad-0.2.8.dist-info/RECORD` & `synapgrad-0.2.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 synapgrad/__init__.py,sha256=rzU1koPmJ4_LyMdxWzho4Qd-qWUqh16aKSgmF5HBOEw,72
-synapgrad/engine.py,sha256=eXyXbUrLbujcr3eGt-iQSarPGGzKzVTBuCdeXuFfVSU,21680
-synapgrad/nn/__init__.py,sha256=ZWcUAUrg9znsANp3CW6N0heJkGdYqkKL2w974saqzjM,340
-synapgrad/nn/activations.py,sha256=eopMfwYDloR2jR6UmjYceoQznb2mFC280zu44WLQB8A,4883
-synapgrad/nn/layers.py,sha256=B8lJ6vq07GRAZJ33fUfzmQBBragUdims9VIHHlo02Tg,2174
-synapgrad/nn/losses.py,sha256=KQwCKoKFS6aptCbH3qllsMviNqFZO1o3qlS3VXhrfaw,8087
-synapgrad/nn/modules.py,sha256=Jqw51sbU2S35HR5XpZ1-8ty0rncD25BHbNaDNmshui8,2477
-synapgrad/nn/neurons.py,sha256=zjHsq9Xa61biK3LMkVI21Ca2xJs1E4Aaird2F7MyVg0,2150
+synapgrad/engine.py,sha256=UFwd5mIN1oYTGKGwNlRdd6cbYc4wJYWGXVd19hiMjY0,30875
+synapgrad/nn/__init__.py,sha256=I-NOoUsUEoYP7VlN8IB2BnCGkF3Xruj7X7Dk_BnF4FU,420
+synapgrad/nn/activations.py,sha256=TEUzX6IvnYlnWkmCyLQMxTDENH-cukG8R0R26ikV5QA,3538
+synapgrad/nn/functional.py,sha256=jICas3UKdjRsxh4xZBTl4nNMfswrrEmqRoOKzu4Qgjw,7831
+synapgrad/nn/initializations.py,sha256=WjgU7KfSQh_aMXBXrj5KOyaz6C3y-tPbmsodFiu6uRc,2879
+synapgrad/nn/layers.py,sha256=d5NGI0WbJtI1Z6BZH2laoqpuLwsr62FYixz6vWLj5jI,13895
+synapgrad/nn/losses.py,sha256=N7uLz_ILdv_LQ_MGLH3xCfyC9FPyEWz7zVO51Di0XJY,6809
+synapgrad/nn/modules.py,sha256=y_F6iUE5t0rlXGwvOtsSVttqgJ3OPMkdx5MbDxceVYc,2654
+synapgrad/nn/neurons.py,sha256=_sTmji8gninDkOEqxHL6Q8av7CIu9mK2m9Olz0FG98E,997
 synapgrad/optim/__init__.py,sha256=8X56jD7Dcyw-Hdux1K7_YK9_oc3BuNPk9YwC7gSNWaE,46
-synapgrad/optim/optimizers.py,sha256=cca-em5N6rxG7vqQ3zeAU0sb9g-6RrDoYaTHpvwOGY4,5290
+synapgrad/optim/optimizers.py,sha256=Y5ryseve_Virrpsl2ynSt2npq2O0-kyIj_Tj0jfKko0,5293
 synapgrad/utils/__init__.py,sha256=eCwZrBr9yWO92hufOIWwAFhwrA_JuMCsmHeDL7PSAtE,154
 synapgrad/utils/data.py,sha256=cwSsVZwEbB6BU9tWrf5aIeZo9u5KNgar7rVYa6WV328,3403
-synapgrad/utils/graph.py,sha256=D2e2tdOw9tyRRdc3fR2rs0nh7kEMFGWat-hlNE4NHIs,1272
+synapgrad/utils/graph.py,sha256=FOkPCSYcmOaoPRhdoXweUQRvoxH0n3x4nASGLr7HQjw,1345
 synapgrad/utils/train.py,sha256=V3j4iqSW9sjSfIz9bski95Ni25KuYzIAkjqD4o3-Tjg,10586
-synapgrad-0.2.8.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
-synapgrad-0.2.8.dist-info/METADATA,sha256=u6cIqsLuXJ1aqKqzfWAYWNZaO4pQyZ8I8Kr-Vb5tcaA,4700
-synapgrad-0.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-synapgrad-0.2.8.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
-synapgrad-0.2.8.dist-info/RECORD,,
+synapgrad-0.2.9.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
+synapgrad-0.2.9.dist-info/METADATA,sha256=XeHTUuOhPvWrceJLtuFqH5yPCqe5pBw_M7WaHyAzuU8,4488
+synapgrad-0.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+synapgrad-0.2.9.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
+synapgrad-0.2.9.dist-info/RECORD,,
```

