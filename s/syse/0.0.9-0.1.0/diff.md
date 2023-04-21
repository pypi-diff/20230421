# Comparing `tmp/syse-0.0.9.tar.gz` & `tmp/syse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syse-0.0.9.tar", last modified: Mon Apr 17 18:15:40 2023, max compression
+gzip compressed data, was "syse-0.1.0.tar", last modified: Fri Apr 21 21:44:43 2023, max compression
```

## Comparing `syse-0.0.9.tar` & `syse-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.476316 syse-0.0.9/
--rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     3006 2023-04-17 18:15:40.475316 syse-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-04-17 16:57:47.000000 syse-0.0.9/README.md
--rw-rw-rw-   0        0        0      751 2023-04-17 16:58:23.000000 syse-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 18:15:40.476316 syse-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-17 16:58:23.000000 syse-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.460905 syse-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.468317 syse-0.0.9/src/syse/
--rw-rw-rw-   0        0        0       47 2023-03-20 22:23:59.000000 syse-0.0.9/src/syse/__init__.py
--rw-rw-rw-   0        0        0    49035 2023-04-17 18:08:26.000000 syse-0.0.9/src/syse/_syse.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.474316 syse-0.0.9/src/syse.egg-info/
--rw-rw-rw-   0        0        0     3006 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 21:44:43.412018 syse-0.1.0/
+-rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2894 2023-04-21 21:44:43.411018 syse-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2023-04-21 21:42:49.000000 syse-0.1.0/README.md
+-rw-rw-rw-   0        0        0      751 2023-04-21 21:42:49.000000 syse-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 21:44:43.412018 syse-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-21 21:42:49.000000 syse-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 21:44:43.394019 syse-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 21:44:43.404018 syse-0.1.0/src/syse/
+-rw-rw-rw-   0        0        0       47 2023-04-17 18:21:04.000000 syse-0.1.0/src/syse/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-04-21 21:40:27.000000 syse-0.1.0/src/syse/_syse.py
+drwxrwxrwx   0        0        0        0 2023-04-21 21:44:43.410018 syse-0.1.0/src/syse.egg-info/
+-rw-rw-rw-   0        0        0     2894 2023-04-21 21:44:43.000000 syse-0.1.0/src/syse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-21 21:44:43.000000 syse-0.1.0/src/syse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 21:44:43.000000 syse-0.1.0/src/syse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 21:44:43.000000 syse-0.1.0/src/syse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 21:44:43.000000 syse-0.1.0/src/syse.egg-info/top_level.txt
```

### Comparing `syse-0.0.9/LICENSE` & `syse-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syse-0.0.9/PKG-INFO` & `syse-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.0.9
+Version: 0.1.0
 Summary: Systems & Industrial Engineering Python Package
 Home-page: https://github.com/apexpromgt/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
@@ -54,11 +54,9 @@
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
 **Notes:**
 
-* This project is being worked on, but I am very busy. 
-* The declining depreciation functions will be fixed.
 * The linear optimization function is extremely limited, and will be worked on.
 * For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

### Comparing `syse-0.0.9/README.md` & `syse-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,9 @@
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
 **Notes:**
 
-* This project is being worked on, but I am very busy. 
-* The declining depreciation functions will be fixed.
 * The linear optimization function is extremely limited, and will be worked on.
 * For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

### Comparing `syse-0.0.9/pyproject.toml` & `syse-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syse"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Jonathon Nicholson", email="Jonathon@apexpromgt.com" },
 ]
 description = "Systems & Industrial Engineering Python Package"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `syse-0.0.9/setup.py` & `syse-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "syse",
-    version = "0.0.9",
+    version = "0.1.0",
     author = "Jonathon Nicholson",
     author_email = "Jonathon@apexpromgt.com",
     description = "Systems & Industrial Engineering Python Package",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/apexpromgt/SysE",
     project_urls = {
```

### Comparing `syse-0.0.9/src/syse/_syse.py` & `syse-0.1.0/src/syse/_syse.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,32 +78,43 @@
                       pv*(1+rate)**nper +
                       pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) == 0
            or, when ``rate == 0``::
                       fv + pv + pmt * nper == 0
 
 
 
-    Examples:
+    Example 1:
     ---------
-    What is the future value after 10 years of saving $100 now, with
-    an additional monthly savings of $100.  Assume the interest rate is
-    5% (annually) compounded monthly?
+    You invest $20,000 in a retirement account and expect to earn a 10% annual return. How much do you expect to be in
+    the account after 20 years?
     ::
-        import numpy as np
-        import syse as syse
-        syse.fv(0.05/12, 10*12, -100, -100)
-        Output = 15692.928894335748
-    By convention, the negative sign represents cash flow out (i.e. money not
-    available today).  Thus, saving $100 a month at 5% annual interest leads
-    to $15,692.93 available to spend in 10 years.
-    If any input is array_like, returns an array of equal shape.  Let's
-    compare different interest rates from the example above::
-        a = np.array((0.05, 0.06, 0.07))/12
-        syse.fv(a, 10*12, -100, -100)
-        Output = array([ 15692.92889434,  16569.87435405,  17509.44688102]) # may vary
+           import numpy as np
+           import syse as syse
+
+           account_value = syse.fv(0.1,20,0,20000)
+
+           print(f"Account Value = ${abs(account_value):,.2f}")
+
+           Account Value = $134,550.00
+
+
+    Example 2:
+    ----------
+    You are planning for your retirement and will be investing $250/month into an IRA. You expect a monthly return of
+    1% and are 45 years from your expected retirement date. Given this information, how much do you expect to be in your
+    retirement account when you retire?
+    ::
+           import numpy as np
+           import syse as syse
+
+           ira_value = syse.fv(0.01,12*45,250,0)
+
+           print(f"IRA Value = ${abs(Q5):,.2f}")
+
+           IRA Value = $5,363,673.26
     """
     when = _convert_when(when)
     rate, nper, pmt, pv, when = np.broadcast_arrays(rate, nper, pmt, pv, when)
 
     fv_array = np.empty_like(rate)
     zero = rate == 0
     nonzero = ~zero
@@ -430,34 +441,39 @@
             fv + pv*(1 + rate)**nper + pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) = 0
         or, when ``rate = 0``::
             fv + pv + pmt * nper = 0
         for `pv`, which is then returned.
 
     Examples:
     ---------
-    What is the present value (e.g., the initial investment)
-    of an investment that needs to total $15692.93
-    after 10 years of saving $100 every month?  Assume the
-    interest rate is 5% (annually) compounded monthly::
+    A German bond that pays annual coupons of 4.5%, has a par value of €1,000, and a YTM of 3.9%.
+    Assuming there are 19 years until maturity, what is the current price of this bond?
+    ::
+        import numpy as np
+        import syse as syse
+        face_value=1000
+        coupon_value=4.5
+        num_coupons=19
+        ytm=3.9
+        current_price = syse.pv(0.039, 19, 45, 1000)
+        print(f"Current price = €{abs(current_price):,.2f}")
+        Output = Current price = €1,079.48
+
+    Gruber Corp. pays a constant $9 dividend on its stock. The company will maintain this dividend for the next 12
+    years and will then cease paying dividends forever (you should assume the company disappears with no extra payouts).
+    If the required return on this stock is 10%, what is the current share price?
+    ::
         import numpy as np
         import syse as syse
-        syse.pv(0.05/12, 10*12, -100, 15692.93)
-        Output = -100.00067131625819
-    By convention, the negative sign represents cash flow out
-    (i.e., money not available today).  Thus, to end up with
-    $15,692.93 in 10 years saving $100 a month at 5% annual
-    interest, one's initial deposit should also be $100.
-    If any input is array_like, ``pv`` returns an array of equal shape.
-    Let's compare different interest rates in the example above::
-        a = np.array((0.05, 0.04, 0.03))/12
-        syse.pv(a, 10*12, -100, 15692.93)
-        array([ -100.00067132,  -649.26771385, -1273.78633713]) # may vary
-    So, to end up with the same $15692.93 under the same $100 per month
-    "savings plan," for annual interest rates of 4% and 3%, one would
-    need initial investments of $649.27 and $1273.79, respectively.
+        rate = 0.10
+        nper = 12
+        pmt = 9
+        share_price = syse.pv(0.10, 12, 9)
+        print(f"Share Price = ${abs(share_price):.2f}")
+        Output = Share Price = $61.32
     """
     when = _convert_when(when)
     (rate, nper, pmt, fv, when) = map(np.asarray, [rate, nper, pmt, fv, when])
     temp = (1+rate)**nper
     fact = np.where(rate == 0, nper, (1+rate*when)*(temp-1)/rate)
     return -(fv + pmt*fact)/temp
 
@@ -814,99 +830,96 @@
         accumulated_depreciation += depreciation.astype(np.float64)
 
     return accumulated_depreciation
 
 
 # Declining Balance Method:
 
-def decline(cost: float, salvage_value: float, useful_life: int, rate: float) -> float:
+def decline(cost: np.ndarray, salvage_value: np.ndarray, useful_life: int, rate: float) -> np.ndarray:
     """
-    Compute the depreciation for an asset using the declining balance method.
+    Compute the accumulated depreciation for an asset using the declining balance method.
 
     Parameters:
-        cost (float): The cost of the asset.
-        salvage_value (float): The salvage value of the asset.
+        cost (np.ndarray): The cost of the asset.
+        salvage_value (np.ndarray): The salvage value of the asset.
         useful_life (int): The useful life of the asset.
         rate (float): The depreciation rate, expressed as a fraction of 1.
 
     Returns:
-        float: The depreciation for the asset.
+        np.ndarray: The depreciation for the asset.
 
     .. Note::
         The function takes as input the cost of the asset, the salvage_value of the asset at the end of its useful
         life, the useful_life of the asset in years, and the rate of depreciation as a fraction of 1. It computes the
         depreciation for the asset using the declining balance method, which assumes that the asset depreciates by a
         fixed percentage of its remaining book value each year.
 
     Examples:
     ---------
     Suppose a company purchases a delivery truck for $50,000, with an expected salvage value of $5,000 after 5 years.
     The company expects to use the truck for 5 years. The depreciation rate for the truck is 30% per year using the
     declining balance method. We can compute the depreciation for the truck using the
-    decline function::
+    decline function
+    ::
         depreciation = syse.decline(cost=50000, salvage_value=5000, useful_life=5, rate=0.3)
-        print(f"The annual depreciation for the truck is ${depreciation/5:.2f}.")
-        Output = The annual depreciation for the truck is $10717.15.
-    This means that the company can deduct $10,717.15 each year for 5 years as a depreciation expense for tax purposes.
-    At the end of 5 years, the book value of the truck will be $5,000, which is the expected salvage value.
+        print(f"The accumulated depreciation for the truck is ${depreciation:.2f}.")
+        Output = The accumulated depreciation for the truck is $41,596.50
     """
-    accumulated_depreciation = 0.0
-    book_value = cost
+    accumulated_depreciation = np.zeros_like(cost, dtype=np.float64)
+    book_value = np.array(cost, dtype=np.float64)
 
     for year in range(1, useful_life + 1):
         depreciation = book_value * rate
-        if book_value - depreciation < salvage_value:
-            depreciation = book_value - salvage_value
-        accumulated_depreciation += depreciation
-        book_value -= depreciation
+        depreciation = np.minimum(depreciation, book_value - salvage_value)
+        accumulated_depreciation += depreciation.astype(np.float64)
+        book_value = (book_value - depreciation).astype(np.float64)
 
     return accumulated_depreciation
 
 
 # Double Declining Balance Method:
 
-def double(cost: float, salvage_value: float, useful_life: int, rate: float) -> float:
+def double(cost: np.ndarray, salvage_value: np.ndarray, useful_life: int, rate: float) -> np.ndarray:
     """
     Compute the depreciation for an asset using the double declining balance method.
 
     Parameters:
-        cost (float): The cost of the asset.
-        salvage_value (float): The salvage value of the asset.
+        cost (np.ndarray): The cost of the asset.
+        salvage_value (np.ndarray): The salvage value of the asset.
         useful_life (int): The useful life of the asset.
         rate (float): The depreciation rate, expressed as a fraction of 1.
 
     Returns:
-        float: The depreciation for the asset.
+        np.ndarray: The depreciation for the asset.
 
     .. Note::
         The function takes the same inputs as the declining_balance_method function, but computes the depreciation
         using the double declining balance method. The double declining balance method assumes that the asset
         depreciates by a fixed percentage of its remaining book value each year, but that the rate of depreciation is
         twice the straight-line rate.
 
     Examples:
     ---------
     Suppose a company purchases a printing press for $100,000, with an expected salvage value of $10,000 after 4 years.
     The company expects to use the printing press for 4 years. The depreciation rate for the printing press is 50% per
     year using the double declining balance method. We can compute the depreciation for the printing press using the
-    double function::
+    double function
+    ::
         depreciation = syse.double(cost=100000, salvage_value=10000, useful_life=4, rate=0.5)
         print(f"The total depreciation for the printing press over 4 years is ${depreciation:.2f}.")
-        Output = The total depreciation for the printing press over 4 years is $102000.00.
-    This means that the company can deduct $102,000 as a depreciation expense over the 4-year life of the printing
+        Output = The total depreciation for the printing press over 4 years is $90,000.00.
+    This means that the company can deduct $90,000 as a depreciation expense over the 4-year life of the printing
     press for tax purposes. At the end of 4 years, the book value of the printing press will be $10,000, which is the
     expected salvage value.
     """
-    accumulated_depreciation = 0.0
-    book_value = cost
-
+    accumulated_depreciation = np.zeros_like(cost, dtype=np.float64)
+    book_value = np.array(cost, dtype=np.float64)  # Convert cost to numpy array and set dtype to float64
     for year in range(1, useful_life + 1):
-        depreciation = book_value * rate * 2
-        if book_value - depreciation < salvage_value:
-            depreciation = book_value - salvage_value
+        depreciation = book_value * (rate * 2) * 2
+        depreciation = np.minimum(depreciation, book_value - salvage_value)
         accumulated_depreciation += depreciation
         book_value -= depreciation
 
     return accumulated_depreciation
 
 
 # Units of Production Method:
@@ -926,23 +939,24 @@
         float: Depreciation expense in year t
         float: Book value at the end of year t
 
     Examples:
     ---------
     On January 1, Miners, Inc. bought a backhoe for $500,000. They expect to use it for 5,000 hours, about 1,000 per
     year for 5 years, before selling it for $100,000. What is the depreciation expense for the first year if they opt
-    for units-of-production method and used it for 1,500 hours?::
-        cost = 500000
-        salvage = 100000
-        expected_units_lifetime = 5000
-        production_t = np.array([1500])  # Only the first year's usage is given, so the array has one element
-        t = 1
-        # Calculate depreciation expense and book value for the first year
-        syse.units(cost, salvage, expected_units_lifetime, production_t, t)
-        Output = 120000.0
+    for units-of-production method and used it for 1,500 hours?
+    ::
+           cost = 500000
+           salvage = 100000
+           expected_units_lifetime = 5000
+           production_t = np.array([1500])  # Only the first year's usage is given, so the array has one element
+           t = 1
+           # Calculate depreciation expense for the first year
+           syse.units(cost, salvage, expected_units_lifetime, production_t, t)
+           Output = 120000.0
 
 
     """
     # Calculate Depreciation per Unit
     depreciation_per_unit = (cost - salvage) / expected_units_lifetime
     # Calculate Depreciation Expense for each year
     depreciation_expense_t = production_t * depreciation_per_unit
@@ -1130,28 +1144,29 @@
     Calculate the expected time and standard deviation it will take to realistically finish a project using the PERT
     estimate formula: (O +4M + P)/6
 
     Parameters:
            tasks: np.ndarray or list of estimated times for each task
 
     Returns:
-           float: expected time
-           float: standard deviation
+           float: expected time & standard deviation
+
 
     Examples:
     ---------
     You are working on a project to build a new office building.
     You need to estimate the time required to complete the project.
     You have identified the following tasks: **1.** Design the building, **2.** Purchase materials, **3.** Construct the building,
     and **4.** Finish the interior. You can estimate the time required to complete the project using the PERT function::
            # Define the tasks for each stage of the project
            DesignBuilding = [60, 70, 100]
            PurchaseMaterials = [60, 70, 100]
            ConstructBuilding = [60, 70, 100]
            FinishInterior = [60, 70, 100]
+           syse.pert(DesignBuilding, PurchaseMaterials, ConstructBuilding, FinishInterior)
            Output = ([73.33333333, 73.33333333, 73.33333333, 73.33333333]),
                     [6.66666667, 6.66666667, 6.66666667, 6.66666667]))
     """
     # Convert input to NumPy arrays
     tasks = [np.array(task) for task in tasks]
     # Extract the optimistic, most likely, and pessimistic times for each set of tasks
     optimistic_time = [task[0] for task in tasks]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syse-0.0.9/src/syse.egg-info/PKG-INFO` & `syse-0.1.0/src/syse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.0.9
+Version: 0.1.0
 Summary: Systems & Industrial Engineering Python Package
 Home-page: https://github.com/apexpromgt/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
@@ -54,11 +54,9 @@
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
 **Notes:**
 
-* This project is being worked on, but I am very busy. 
-* The declining depreciation functions will be fixed.
 * The linear optimization function is extremely limited, and will be worked on.
 * For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

