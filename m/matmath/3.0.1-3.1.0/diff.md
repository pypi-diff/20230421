# Comparing `tmp/matmath-3.0.1.tar.gz` & `tmp/matmath-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matmath-3.0.1.tar", last modified: Fri Apr  1 13:17:02 2022, max compression
+gzip compressed data, was "matmath-3.1.0.tar", max compression
```

## Comparing `matmath-3.0.1.tar` & `matmath-3.1.0.tar`

### file list

```diff
@@ -1,21 +1,7 @@
-drwxrwxrwx   0        0        0        0 2022-04-01 13:17:02.413802 matmath-3.0.1/
--rw-rw-rw-   0        0        0     1072 2021-10-11 03:16:42.000000 matmath-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     7949 2022-04-01 13:17:02.409805 matmath-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6679 2022-02-25 12:25:16.000000 matmath-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-04-01 13:17:02.377802 matmath-3.0.1/matmath/
--rw-rw-rw-   0        0        0       87 2022-02-12 10:10:48.000000 matmath-3.0.1/matmath/__init__.py
--rw-rw-rw-   0        0        0    17032 2022-04-01 03:13:28.000000 matmath-3.0.1/matmath/matrices.py
--rw-rw-rw-   0        0        0        0 2022-02-03 16:49:05.000000 matmath-3.0.1/matmath/py.typed
--rw-rw-rw-   0        0        0     9166 2022-04-01 03:09:09.000000 matmath-3.0.1/matmath/vectors.py
-drwxrwxrwx   0        0        0        0 2022-04-01 13:17:02.401868 matmath-3.0.1/matmath.egg-info/
--rw-rw-rw-   0        0        0     7949 2022-04-01 13:17:01.000000 matmath-3.0.1/matmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-04-01 13:17:02.000000 matmath-3.0.1/matmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-01 13:17:01.000000 matmath-3.0.1/matmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-04-01 13:17:02.000000 matmath-3.0.1/matmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-11 12:37:27.000000 matmath-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-01 13:17:02.413802 matmath-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1403 2022-04-01 13:16:10.000000 matmath-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-01 13:17:02.409805 matmath-3.0.1/test/
--rw-rw-rw-   0        0        0        0 2021-12-04 04:01:58.000000 matmath-3.0.1/test/__init__.py
--rw-rw-rw-   0        0        0      284 2022-03-20 11:42:49.000000 matmath-3.0.1/test/test_matrix.py
--rw-rw-rw-   0        0        0     3153 2022-02-15 11:37:21.000000 matmath-3.0.1/test/test_vectors.py
+-rw-r--r--   0        0        0     1072 2022-07-05 06:12:14.501665 matmath-3.1.0/LICENSE
+-rw-r--r--   0        0        0      110 2023-04-21 08:21:19.171129 matmath-3.1.0/matmath/__init__.py
+-rw-r--r--   0        0        0    20038 2023-04-21 08:19:25.715900 matmath-3.1.0/matmath/matrices.py
+-rw-r--r--   0        0        0        0 2022-07-05 10:29:36.433485 matmath-3.1.0/matmath/py.typed
+-rw-r--r--   0        0        0    10217 2023-04-21 08:15:16.270345 matmath-3.1.0/matmath/vectors.py
+-rw-r--r--   0        0        0      656 2023-04-21 08:21:09.587687 matmath-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 matmath-3.1.0/PKG-INFO
```

### Comparing `matmath-3.0.1/LICENSE` & `matmath-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matmath-3.0.1/matmath/matrices.py` & `matmath-3.1.0/matmath/matrices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-def zero(n, m=None):
+from typing import Optional
+
+
+def zero(n: int, m: Optional[int] = None):
     """Creates a 2D array of size n x m."""
     if m is None:
         m = n
     return [[0] * m] * n
 
 
-def identity(n):
+def identity(n: int):
     """Creates a 2D array of size n x m with 1s on the diagonal."""
     return [[int(i == j) for i in range(n)] for j in range(n)]
 
 
 # ------------------------------------------------------------------------------
 class Matrix:
     def __init__(self, *matrix):
@@ -25,28 +28,24 @@
                 # Check if rows are lists or tuples
                 if not isinstance(row, (list, tuple)):
                     raise ValueError(f"Matrix must contain list/tuples not {type(row)}")
                 iter_check = iter(row)
                 # Confirm that elements are numbers.
                 for element in iter_check:
                     if not isinstance(element, (int, float, complex)):
-                        raise ValueError(
-                            f"Matrix must contain only numbers not {type(element)}"
-                        )
+                        raise ValueError(f"Matrix must contain only numbers not {type(element)}")
         except TypeError:
             raise TypeError("Matrix argument should be iteratable.")
         # Check if number of elements in each row is the same.
         no_of_cols = len(matrix[0])
         no_of_rows = 0
         for row in matrix:
             no_of_rows += 1
             if len(row) != no_of_cols:
-                raise ValueError(
-                    "The number of elements in the matrix should be equal."
-                )
+                raise ValueError("The number of elements in the matrix should be equal.")
         # Initialize variables
         self.matrix = [list(row) for row in matrix]
         self.rows = no_of_rows  # Number of rows
         self.cols = no_of_cols  # Number of columns
         self.__index = 0  # Used for iterating over the matrix
 
     def __len__(self):
@@ -60,15 +59,15 @@
     def __next__(self):
         """Returns the next element of the matrix"""
         if self.__index < len(self.matrix):
             self.__index += 1
             return self.matrix[self.__index - 1]
         raise StopIteration
 
-    def __getitem__(self, r, c):
+    def __getitem__(self, r: int, c: int):
         """Returns the element at the specified key"""
         return self.matrix[r][c]
 
     def __str__(self):
         """Returns a string representation of the matrix"""
         length = self.rows
         string = ["| "] * length
@@ -96,120 +95,199 @@
                     return False
         return True
 
     def __ne__(self, other):
         """Checks if the matrix is not equal to another matrix"""
         return not (self.matrix == other.matrix)
 
-    def __add__(self, anotherObj):
+    def __add__(self, other):
         """Returns the sum of the matrices"""
-        if self.order() == anotherObj.order():
+        if self.order() == other.order():
             matrix = []
             for i in range(self.rows):
                 temp = []
                 for j in range(self.cols):
-                    temp.append(self.matrix[i][j] + anotherObj[i][j])
+                    temp.append(self.matrix[i][j] + other[i][j])
                 matrix.append(temp)
             return Matrix(matrix)
         raise ValueError("The 2 matrices do not have the same order.")
 
-    def __sub__(self, anotherObj):
+    def __iadd__(self, other):
+        return self + other
+
+    def __sub__(self, other):
         """Returns the difference of the matrices"""
-        if self.order() == anotherObj.order():
+        if self.order() == other.order():
             matrix = []
             for i in range(self.rows):
                 temp = []
                 for j in range(self.cols):
-                    temp.append(self.matrix[i][j] - anotherObj[i][j])
+                    temp.append(self.matrix[i][j] - other[i][j])
                 matrix.append(temp)
             return Matrix(matrix)
         raise ValueError("The 2 matrices do not have the same order.")
 
-    def __mul__(self, anotherObj):
+    def __isub__(self, other):
+        return self - other
+
+    def __mul__(self, other):
         """Returns the product of a matrix and a number/matrix"""
-        if isinstance(anotherObj, [int, float]):  # Scalar multiplication
-            prod = []
+        if isinstance(other, [int, float]):  # Scalar multiplication
+            result = []
             for row in self.matrix:
-                new_row = [(element * anotherObj) for element in row]
-                prod.append(new_row)
-            return Matrix(prod)
-        elif isinstance(anotherObj, Matrix):
-            matrix = []
-            for i in range(self.rows):
-                temp = []
-                for j in range(self.cols):
-                    temp.append(self.matrix[i][j] * anotherObj[i][j])
-                matrix.append(temp)
-            return matrix
-        raise TypeError(
-            f"Multiplication not supported between type Matrix and type {type(anotherObj)}."
-        )
+                new_row = [(element * other) for element in row]
+                result.append(new_row)
+            return Matrix(result)
+        elif isinstance(other, Matrix):
+            if self.cols == other.cols and self.rows == other.rows:
+                result = []
+                for i in range(self.rows):
+                    temp = []
+                    for j in range(self.cols):
+                        temp.append(self.matrix[i][j] * other[i][j])
+                    result.append(temp)
+                return result
+            raise ValueError("The 2 matrices do not have the same order.")
+        raise TypeError(f"Multiplication not supported between {type(self)} and {type(other)}.")
+
+    def __imul__(self, other):
+        return self * other
+
+    def __truediv__(self, other):
+        """Returns the division of a matrix and a number/matrix"""
+        if isinstance(other, (int, float)):
+            result = []
+            for row in self.matrix:
+                new_row = [(element * other) for element in row]
+                result.append(new_row)
+            return Matrix(result)
+        elif isinstance(other, Matrix):
+            if self.cols == other.cols and self.rows == other.rows:
+                result = []
+                for i in range(self.rows):
+                    temp = []
+                    for j in range(self.cols):
+                        temp.append(self.matrix[i][j] / other[i][j])
+                    result.append(temp)
+                return result
+            raise ValueError("The 2 matrices do not have the same order.")
+        raise TypeError(f"Division not supported between {type(self)} and {type(other)}.")
+
+    def __itruediv__(self, other):
+        return self / other
+
+    def __floordiv__(self, other):
+        """Returns the quotient of a matrix and a number/matrix"""
+        if isinstance(other, (int, float)):
+            result = []
+            for row in self.matrix:
+                new_row = [(element // other) for element in row]
+                result.append(new_row)
+            return Matrix(result)
+        elif isinstance(other, Matrix):
+            if self.cols == other.cols and self.rows == other.rows:
+                result = []
+                for i in range(self.rows):
+                    temp = []
+                    for j in range(self.cols):
+                        temp.append(self.matrix[i][j] // other[i][j])
+                    result.append(temp)
+                return result
+            raise ValueError("The 2 matrices do not have the same order.")
+        raise TypeError(f"Multiplication not supported between {type(self)} and {type(other)}.")
 
-    def __rmul__(self, otherObj):
-        """Returns the product of a matrix and a number/matrix"""
-        return self * otherObj
+    def __ifloordiv__(self, other):
+        return self // other
 
     def __matmul__(self, other):
         """Returns the cross product of two matrices"""
         if isinstance(other, Matrix):  # Matrix multiplication
             arr = []
             for i in range(self.rows):
                 arr.append([])
-                for j in range(other.rows):
+                for j in range(other.cols):
                     total = 0
                     for k in range(self.cols):
                         total += self.matrix[i][k] * other.matrix[k][j]
                     arr[i].append(total)
             return Matrix(arr)
         raise ValueError(f"Passed object is not of {type(self)}")
 
-    def __pow__(self, power=2):
+    def __pow__(self, power: int = 2):
         """Returns the matrix representing the n^th power of matrix A, if mathematically possible."""
         if self.cols == self.rows:
             if isinstance(power, int) and int > 0:
-                matrix = self.matrix
+                matrix = self.copy()
                 for _ in range(power - 1):
                     matrix = matrix * self.matrix
                 return matrix
             elif power == 0:
                 matrix = identity(self.rows)
                 return Matrix(matrix)
             raise ValueError("The power of the matrix must be a natural number")
         raise ValueError("The given matrix is not a square matrix.")
 
+    def identity(self, n: int = 3):
+        """
+        identity _summary_
+
+        Parameters
+        ----------
+        n : int
+            The order of the identity matrix. defaults to 3.
+        """
+        matrix = [[0] * n] * n
+        for i in range(n):
+            matrix[i][i] = 1
+        self.matrix = matrix
+        self.rows = n
+        self.cols = n
+
+    def zero(self, order: tuple):
+        r, c = order
+        self.matrix = [[0] * c] * r
+        self.rows = r
+        self.cols = c
+
+    def fill(self, value: int, order: tuple):
+        r, c = order
+        self.matrix = [[value] * c] * r
+        self.rows = r
+        self.cols = c
+
     def adjoint(self):
         """Returns the adjoint representation of the matrix.
 
         Returns
         -------
-        matrix :
+        Matrix :
             The adjoint representation of the matrix.
         """
         matrix = []
         for i in range(self.rows):
             temp = []
             for j in range(self.cols):
                 temp.append(self.cofactor(i, j))
             matrix.append(temp)
         return Matrix(matrix).transpose()
 
     def cofactor(self, i: int, j: int):
-        """Returns the cofactor representation of the matrix.
+        """Returns the co-factor representation of the matrix.
 
-        Args
-        ----
+        Parameters
+        ----------
         i: int
             The index of the row of the matrix.
         j: int
             The index of the column of the matrix.
 
         Returns
         -------
-        cofactor: float
-            The cofactor representation of the matrix.
+        float :
+            The co-factor representation of the matrix.
         """
         return float((-1) ** (i + j) * self.minor(i, j))
 
     def copy(self):
         """Returns a shallow copy of this matrix.
 
         Returns
@@ -222,52 +300,48 @@
             new_matrix.append(new_row)
         return Matrix(new_matrix)
 
     def cut(self, i=None, j=None):
         """Returns a new matrix after removing the i th row and/or j th column.
         Will remove no row and column (by default).
 
-        Args
-        ----
+        Parameters
+        ----------
         i (int, optional)
             The row to be removed. Starts from 0.
         j (int, optional)
             The column to be removed. Starts from 0.
 
         Returns
         -------
-        Matrix
+        Matrix :
             The matrix after removing the i th row and/or j th column.
 
         Raises
         ------
         ValueError
             Raised if the row or column to be removed is not a natural number.
         """
         if i is None and j is None:
             matrix = self.copy()
             return Matrix(matrix)
-        elif all([i is not None, i >= 0, i < self.rows, j is None]):
+        elif i is not None and j is None:
             matrix = []
             for k in range(self.rows):
                 if k != i:
                     matrix.append(self.matrix[k])
             return Matrix(matrix)
-        elif all([j is not None, j >= 0, j < self.cols, i is None]):
+        elif i is None and j is not None:
             matrix = []
-            for k in range(self.rows):
-                temp = []
-                for l in range(self.cols):
-                    if l != j:
-                        temp.append(self.matrix[k][l])
-                matrix.append(temp)
+            for k in range(self.cols):
+                for l in range(self.rows):
+                    if k != j:
+                        matrix[l].append(self.matrix[l][k])
             return Matrix(matrix)
-        elif all(
-            [i is not None, j is not None, i >= 0, i < self.rows, j >= 0, j < self.cols]
-        ):
+        elif i is not None and j is not None:
             matrix = []
             for k in range(self.rows):
                 if k != i:
                     temp = []
                     for l in range(self.cols):
                         if l != j:
                             temp.append(self.matrix[k][l])
@@ -276,15 +350,15 @@
         raise ValueError("The row or column to be removed is not a natural number.")
 
     def determinant(self):
         """Returns the determinant of this matrix.
 
         Returns
         -------
-        determinant : float
+        float :
             The determinant of this matrix.
         """
         if self.is_square():
             determinant = 1
             A = self.matrix
             for i in range(self.rows):
                 for j in range(i + 1, self.rows):
@@ -299,144 +373,153 @@
         raise ValueError("The given matrix is not a square matrix.")
 
     def inverse(self):
         """Returns the inverse of this matrix
 
         Returns
         -------
-        inv : Matrix
+        Matrix :
             The inverse of this matrix
         """
         if self.is_square():
             determinant = self.determinant()
             if determinant == 0:
                 raise ValueError("The given matrix is not invertible.")
             return (self.adjoint() / determinant).transpose()
         raise ValueError("The given matrix is not a square matrix.")
 
+    @staticmethod
     def is_diagonal(self):
         """Returns True if the matrix is diagonal, False otherwise."""
         if self.cols == self.rows:
             for i in range(self.rows):
                 for j in range(self.cols):
                     if i != j and self.matrix[i][j] != 0:
                         return False
             return True
         return False
 
+    @staticmethod
     def is_identity(self):
         """Returns True if the matrix is identity, False otherwise"""
         for i in range(self.rows):
             for j in range(self.cols):
                 if i == j and self.matrix[i][j] != 1:
                     return False
                 elif i != j and self.matrix[i][j] != 0:
                     return False
         return True
 
+    @staticmethod
     def is_invertible(self):
         """Returns True if the matrix is invertible, False otherwise."""
         return self.det() != 0
 
+    @staticmethod
     def is_lower_triangular(self):
         """Returns True if the matrix is lower triangular, False otherwise."""
         if self.cols == self.rows:
             for i in range(self.rows):
                 for j in range(i + 1, self.cols):
                     if self.matrix[i][j] != 0:
                         return False
             return True
         return False
 
+    @staticmethod
     def is_null(self):
         """Returns True if the matrix is null, False otherwise."""
         for row in self.matrix:
             for item in row:
                 if item != 0:
                     return False
         return True
 
+    @staticmethod
     def is_skew_symmetric(self):
         """Returns True if the matrix is skew-symmetric, False otherwise."""
         if self.cols == self.rows:
             for i in range(self.rows):
                 for j in range(i, self.cols):
                     if self.matrix[i][j] != -self.matrix[j][i]:
                         return False
             return True
         return False
 
+    @staticmethod
     def is_square(self):
         """Returns True if the matrix is square, False otherwise."""
         return self.cols == self.rows
 
+    @staticmethod
     def is_symmetric(self):
         """Returns True if the matrix is symmetric, False otherwise."""
         if self.cols == self.rows:
             for i in range(self.rows):
                 for j in range(i, self.cols):
                     if self.matrix[i][j] != self.matrix[j][i]:
                         return False
             return True
         return False
 
+    @staticmethod
     def is_upper_triangular(self):
         """Returns True if the matrix is upper triangular, False otherwise."""
         if self.cols == self.rows:
             for i in range(self.rows):
                 for j in range(i):
                     if self.matrix[i][j] != 0:
                         return False
             return True
         return False
 
     def minor(self, i, j):
         """Returns the minor of the Aij element in matrix A.
 
-        Args
-        ----
+        Parameters
+        ----------
         i (int, optional)
             The row of the element. Starts from 0.
         j (int, optional)
             The column of the element. Starts from 0.
 
         Returns
         -------
-        Matrix
+        Matrix :
             The minor of the matrix A.
 
         Raises
         ------
         ValueError
             Raised if the row or column to be removed is not a natural number.
         """
         reduced = self.cut(i, j)
         return reduced.determinant()
 
+    @property
     def order(self):
         """Returns the order of the matrix.
 
         Returns
         -------
-        order: tuple
+        tuple :
             The order of the matrix.
         """
         return self.rows, self.cols
 
     def rotate(self, turns=1):
         """Returns the matrix after n rotations.
 
-        Args
-        ----
+        Parameters
         turns (int, optional)
             The number of turns to rotate the matrix in clockwise direction. Defaults to 1.
 
         Returns
         -------
-        rotated: Matrix
+        Matrix :
             The matrix after n rotations.
         """
         if isinstance(turns, int):
             turns = turns % 4
             if turns == 0:
                 return self
             elif turns == 2:
@@ -451,15 +534,15 @@
         raise ValueError("The number of turns is an integer.")
 
     def trace(self):
         """Returns a trace of the matrix.
 
         Returns
         -------
-        total: int/float/complex
+        int/float/complex ;
             The trace of the matrix.
         """
         if self.is_square():
             total = 0
             for i in range(self.rows):
                 total += self.matrix[i][i]
             return total
@@ -476,14 +559,24 @@
         arr = []
         for i in range(self.cols):
             arr.append([])
             for j in range(self.rows):
                 arr[i].append(self.matrix[j][i])
         return Matrix(arr)
 
+    def to_list(self):
+        """Returns the matrix as a list of lists.
+
+        Returns
+        -------
+        list :
+            The matrix as a list of lists.
+        """
+        return self.matrix
+
     # Alias
     adj = adjoint
     det = determinant
     inv = inverse
     is_diagonal_dominant = is_diagonal
     is_upper_hessenberg = is_upper_triangular
     is_lower_hessenberg = is_lower_triangular
```

### Comparing `matmath-3.0.1/matmath/vectors.py` & `matmath-3.1.0/matmath/vectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from math import acos, cos, pi, sin, sqrt
+from typing import List, Union
 
 
 class Vector:
-    def __init__(self, *args):
+    def __init__(self, *args: List[Union[int, float]]):
+        __slots__ = "length", "__index"
         if len(args) == 0:
             self.vector = [0, 0]
         elif len(args) == 1:
             if isinstance(args[0], (int, float)):
                 self.vector = [args[0]]
             else:
                 for arg in args[0]:
@@ -74,27 +76,25 @@
                 new.append(self.vector[i] * other)
             return Vector(new)
         elif isinstance(other, Vector):
             resultantVector = []
             for elem1, elem2 in zip(self.vector, other.vector):
                 resultantVector.append(elem1 * elem2)
             return Vector(resultantVector)
-        raise TypeError(
-            f"Multiplication not supported between type Vector and type {type(other)}."
-        )
+        raise TypeError(f"Multiplication not supported between type Vector and type {type(other)}.")
 
     def __rmul__(self, other):
         """Returns the product of a number and a vector"""
         return self * other
 
     def __matmul__(self, other):
         """Matrix multiplication (cross product) of two vectors"""
         return self.cross_product(other)
 
-    def __truediv__(self, number: float):
+    def __truediv__(self, number: Union[int, float]):
         """Divides the vector with the given number"""
         if isinstance(number, (int, float)):
             divided = [i / number for i in self]
             return Vector(divided)
         raise TypeError("can only divide by numbers.")
 
     def __eq__(self, other):
@@ -104,27 +104,43 @@
                 return False
         return True
 
     def __ne__(self, other):
         """Tells whether the vectors are not equal"""
         return not self.__eq__(other)
 
-    def modulus(self):
+    def __hash__(self):
+        """Returns the hash of the vector"""
+        return hash(tuple(self.vector))
+
+    def __bool__(self):
+        """Returns True if the vector is non-zero"""
+        return sum(map(lambda x: x * x, self.vector)) != 0
+
+    def __abs__(self):
+        """Returns the modulus of the vector"""
+        return self.modulus()
+
+    def copy(self):
+        """Returns a copy of the vector"""
+        return Vector(self.vector)
+
+    @staticmethod
+    def modulus(self) -> float:
         """Returns the modulus (length/magnitude) of the vector
 
         Returns
         -------
         float
             magnitude of the length of the vector.
         """
-        squared = 0
-        for i in self:
-            squared += i**2
-        return sqrt(squared)
+        sum_of_squares = sum(map(lambda x: x * x, self.vector))
+        return sqrt(sum_of_squares)
 
+    @staticmethod
     def argument(self):
         """Returns the argument of the vector
 
         Returns
         -------
         list
             a list containing angle which the vector makes with respect to the axes.
@@ -144,15 +160,15 @@
         UnitVector = []
         if mod == 0:
             return self
         for element in self:
             UnitVector.append(element / mod)
         return Vector(UnitVector)
 
-    def magnify(self, magnification: float = 1):
+    def magnify(self, magnification: Union[int, float] = 1):
         """Returns the scaled-up or scaled-down version of the vector
 
         Parameter
         ---------
         magnification (float, optional)
             The scale of magnification of the vector. Defaults to 1
 
@@ -162,15 +178,15 @@
             A vector (= vector * magnification) in the same direction as the given vector.
         """
         NewVector = []
         for element in self.vector:
             NewVector.append(element * magnification)
         return Vector(NewVector)
 
-    def rotate(self, theta=pi, radians=True):
+    def rotate(self, theta: Union[int, float] = pi, radians: bool = True):
         """Rotates the given vector by the given angle in clockwise direction
 
         Parameters
         ----------
         theta (int/float, optional)
             The angle of rotation (in radians). Defaults to pi.
         radians (bool, optional)
@@ -247,32 +263,47 @@
                 a1, a2, a3 = self
                 b1, b2, b3 = other
                 return Vector([a2 * b3 - a3 * b2, a3 * b1 - a1 * b3, a1 * b2 - a2 * b1])
             elif self.length == 2:
                 a1, a2 = self
                 b1, b2 = other
                 return Vector([0, 0, a1 * b2 - a2 * b1])
-            raise ValueError(
-                "The dimension of the 2 vectors must be less than or equal to 3."
-            )
+            raise ValueError("The dimension of the 2 vectors must be less than or equal to 3.")
         raise ValueError("The dimension of the 2 vectors must be the same.")
 
+    @staticmethod
     def is_unit(self):
         """Tells whether the vector is a unit vector or not"""
         sum_of_squares = 0
         for i in self.vector:
             sum_of_squares += i**2
             if sum_of_squares > 1:
                 return False
         return sum_of_squares == 1
 
+    @staticmethod
     def is_parallel(self, other):
         """Tells whether the vectors are parallel or not"""
         ratio = self[0] / other[0]
         for i, j in zip(self, other):
             if i / j != ratio:
                 return False
         return True
 
+    @staticmethod
+    def is_orthogonal(self, other):
+        """Tells whether the vectors are orthogonal or not"""
+        return self.dot_product(other) == 0
+
+    @staticmethod
+    def to_list(self):
+        """Returns the vector as a list"""
+        return self.vector
+
+    @staticmethod
+    def to_tuple(self):
+        """Returns the vector as a tuple"""
+        return tuple(self.vector)
+
     # Alias
     arg = argument
     mod = modulus
```

