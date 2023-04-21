# Comparing `tmp/bsmschema-0.0.4.tar.gz` & `tmp/bsmschema-0.1.0.tar.gz`

## Comparing `bsmschema-0.0.4.tar` & `bsmschema-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bsmschema-0.0.4/bsmschema/__init__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 bsmschema-0.0.4/bsmschema/__main__.py
--rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 bsmschema-0.0.4/bsmschema/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bsmschema-0.0.4/bsmschema/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bsmschema-0.0.4/.gitignore
--rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 bsmschema-0.0.4/LICENSE
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 bsmschema-0.0.4/README.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bsmschema-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    14534 2020-02-02 00:00:00.000000 bsmschema-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bsmschema-0.1.0/bsmschema/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 bsmschema-0.1.0/bsmschema/__main__.py
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 bsmschema-0.1.0/bsmschema/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bsmschema-0.1.0/bsmschema/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bsmschema-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 bsmschema-0.1.0/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 bsmschema-0.1.0/README.md
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bsmschema-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14534 2020-02-02 00:00:00.000000 bsmschema-0.1.0/PKG-INFO
```

### Comparing `bsmschema-0.0.4/bsmschema/models.py` & `bsmschema-0.1.0/bsmschema/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,19 +76,23 @@
 ]
 
 # Aliases
 Filter = Dict[StrictStr, List[Any]]
 VariableList = List[Union[Literal[1], StrictStr]]
 Weights = List[Union[StrictInt, StrictFloat, StrictStr]]
 
+# Python 3.10 at least weirdly annotates "X: Optional[X] = None" as NoneType
+OptionalFilter = Optional[Filter]
+OptionalAggregate = Optional[Aggregate]
+
 
 class _BSMBase(BaseModel):
     # Docstring missing to avoid polluting every object description with this field
     # This permits users to write comments on objects.
-    Description: Optional[str]
+    Description: Optional[str] = None
 
     class Config:
         extra = Extra.forbid
 
 
 class Edge(_BSMBase):
     r"""An Edge connects two :py:class:`Node`\s, indicating the outputs (contrasts) of
@@ -119,15 +123,15 @@
     Source: StrictStr
     """Name of :py:class:`Node`. The outputs of this node are passed to :py:attr:`Destination`."""
     Destination: StrictStr
     """Name of :py:class:`Node`. The outputs of :py:attr:`Source` are passed to this node.
 
     If :py:attr:`Filter` is defined,
     The outputs of the Source node are the inputs of the Destination node, after filtering (if any)."""
-    Filter: Optional[Filter]
+    Filter: OptionalFilter = None
     """Maps a grouping variable to a list of values to pass to Destination.
     If multiple grouping variables are passed, the result is the conjunction of filters."""
 
 
 class Transformations(_BSMBase):
     """Transformations describe modifications of variables to prepare a design matrix.
 
@@ -162,14 +166,18 @@
     Transformer: TransformerID
     """Name of the specification of an instruction set."""
     Instructions: List[Any]
     """Sequence of instructions to pass to an implementation of :py:attr:`Transformer`.
     The format of these instructions is determined by the :py:attr:`Transformer`."""
 
 
+# Python annotation hack
+OptionalTransformations = Optional[Transformations]
+
+
 class HRF(_BSMBase):
     """Specification of a hemodynamic response function (HRF) model.
 
     Most design matrix constructors permit sparse events of the form
     (onset, duration, amplitude) to be convolved by a named HRF,
     possibly with some parameters.
     Some may permit dense time series to be convolved as well.
@@ -208,48 +216,57 @@
     * ``"glover + derivative + dispersion"``
     * ``"afni"``
     * ``"fir"``
 
     The list of supported models is expandable and limited by the estimator, not the specification.
     Note that ``"glover"`` is the default "Gamma" HRF in FSL.
     """
-    Parameters: Optional[Dict[str, Any]]
+    Parameters: Optional[Dict[str, Any]] = None
     """Parameters to the hemodynamic model.
 
     Options will be software specific and are not controlled.
     For ``"fir"``, the parameter ``"fir_delays"`` is required.
     """
 
 
+# Python annotation hack
+OptionalHRF = Optional[HRF]
+
+
 class Options(_BSMBase):
     """Estimation options that are common to multiple estimation packages."""
-    HighPassFilterCutoffHz: Optional[float]
+
+    HighPassFilterCutoffHz: Optional[float] = None
     """The cutoff frequency, in Hz, for a high-pass filter."""
-    LowPassFilterCutoffHz: Optional[float]
+    LowPassFilterCutoffHz: Optional[float] = None
     """The cutoff frequency, in Hz, for a low-pass filter."""
-    ReplaceVariables: Optional[Dict[StrictStr, Any]]
+    ReplaceVariables: Optional[Dict[StrictStr, Any]] = None
     """Allows a specification of design matrix columns that are to be replaced by the estimating software.
     Keys are the names of columns to replace; values are unconstrained,
     and can be anything that helps the receiving software understand what is intended.
     For example, it is relatively common to want to include a voxel-specific timecourse as a covariate.
     In this case, the expectation is that the user will have constructed a dummy column as a placeholder
     (e.g., by adding a constant column to events.tsv files), and then indicate (via ReplaceVariables)
     how the receiving software should inject new values."""
-    Mask: Optional[Filter]
+    Mask: Optional[Filter] = None
     """BIDS entities specifying a mask file from the input dataset.
     For example, {"desc": "brain", "suffix": "mask"}."""
-    Aggregate: Optional[Aggregate]
+    Aggregate: OptionalAggregate = None
     """Method of combining time series within each value in the Mask.
     The following values are valid: "none", "mean", "pca".
     "none" (the default) indicates no dimensionality reduction; a separate timecourse is returned for each voxel
     that contains at least one non-zero value in its timecourse.
     "mean" returns the average of all voxels within each discrete non-zero value found in the image.
     "pca" returns the first principal component of all voxels within each discrete non-zero value found in the image."""
 
 
+# Python annotation hack
+OptionalOptions = Optional[Options]
+
+
 class Contrast(_BSMBase):
     r"""Contrasts are weighted sums of parameter estimates (betas) generated by a model fit.
 
     ``Contrast`` defines the structure of the elements of the :py:attr:`Node.Contrasts` list.
 
     Along with :py:class:`DummyContrasts`, Contrasts define the outputs of a :py:class:`Node`.
 
@@ -330,27 +347,31 @@
             {"Name": "A", "ConditionList": ["A"], "Weights": [1], "Test": "t"}
             {"Name": "B", "ConditionList": ["B"], "Weights": [1], "Test": "t"}
         ]
 
     While ``"t"`` and ``"pass"`` contrasts are passed as inputs to the next node, ``"F"``
     contrasts are terminal and are not passed as inputs to following :py:class:`Node`\s.
     """
-    Contrasts: Optional[VariableList]
+    Contrasts: Optional[VariableList] = None
     """A list of variables to construct DummyContrasts for.
     Must be a strict subset of ``Model.X``.
     If absent, then dummy contrasts for all variables are constructed."""
     # Note: Keep Test synced with Contrast.Test, including docstring and type
     Test: StatisticalTest
     r"""The type of test statistic to compute on the contrast.
     The special value "pass" indicates that no statistical test is to be performed.
 
     Note that ``"F"`` contrasts are terminal and not passed as inputs to following
     :py:class:`Node`\s."""
 
 
+# Python annotation hack
+OptionalDummyContrasts = Optional[DummyContrasts]
+
+
 class Model(_BSMBase):
     """The model to fit to the collection of input images.
 
     This section defines the design matrix construction, estimator type,
     and additional options needed to estimate the model parameters.
     """
     Type: ModelType
@@ -368,29 +389,29 @@
     Any available variables that are not explicitly named in X will be omitted from the model.
     Partial matching is supported and can be specified using wildcard characters;
     for example, use "aroma_motion_*" to specify all of the aroma components found in the confounds file.
     Following standard Unix-style glob rules,
     "*" is interpreted to match 0 or more alphanumeric characters, and
     "?" is interpreted to match exactly one alphanumeric character.
     """
-    Formula: Optional[StrictStr]
+    Formula: Optional[StrictStr] = None
     """Wilkinson notation specification of a transformation of the design matrix X.
     A 1 or 0 term MUST be present to explicitly include or exclude, respectively, an intercept variable,
     to ensure consistent handling across formula interpreters."""
-    HRF: Optional[HRF]
+    HRF: OptionalHRF = None
     """A specification of the hemodynamic response function (HRF) that should be applied
     to variables by implementing software."""
     ## These are very likely getting pulled out.
     # VarianceComponents: Optional[List[Dict[str, Any]]]
     # """A specification of the variance components to include in the model."""
     # ErrorDistribution: Optional[Dict[str, Any]]
     # """Specifies how to model the error."""
-    Options: Optional[Options]
+    Options: OptionalOptions = None
     """Estimation options that are common to multiple estimation packages."""
-    Software: Optional[Dict[StrictStr, Dict[StrictStr, Any]]]
+    Software: Optional[Dict[StrictStr, Dict[StrictStr, Any]]] = None
     """This section allows one to specify any software-specific estimation parameters.
     Each key in the object is the name of the software package (FSL, SPM, etc.),
     and the value is an object containing software-specific parameters.
     The BIDS Stats Models spec makes no attempt to control the vocabulary available for
     use in any particular software package;
     we expect that the developers of each package will, over time, fill in these specifications."""
 
@@ -409,22 +430,22 @@
     """
     GroupBy: List[StrictStr]
     """The output statistical maps received from the input node are split along
     unique combinations of the grouping variables and passed to the model as subsets.
     If empty, all inputs are passed to a single model to fit.
     Reserved strings include: "run", "session", "subject", and "contrast".
     Any metadata field may be used as a grouping variable."""
-    Transformations: Optional[Transformations]
+    Transformations: OptionalTransformations = None
     """Specification of transformations to be applied to variables before the construction of the model."""
     Model: Model
     """What model parameters should be included, and how the errors are specified."""
-    Contrasts: Optional[List[Contrast]]
+    Contrasts: Optional[List[Contrast]] = None
     """How to linearly weight/combine design matrix columns
     to generate contrast maps and (optionally) run statistical tests."""
-    DummyContrasts: Optional[DummyContrasts]
+    DummyContrasts: OptionalDummyContrasts = None
     """A convenient shortcut for specifying contrasts;
     allows automatic creation of indicator contrasts
     for either all variables in the design matrix, or all named variables."""
 
 
 class BIDSStatsModel(_BSMBase):
     """A BIDS Stats Model is a JSON file that defines one or more hierarchical models
@@ -443,24 +464,24 @@
     (i.e., if a single BIDS project contains multiple model specifications in different files and/or folders,
     care should be taken to ensure that each model has a unique name)."""
 
     BIDSModelVersion: StrictStr
     """A string identifying the version of the specification adhered to.
     Note this is different from BIDSVersion"""
 
-    Description: Optional[StrictStr]
+    Description: Optional[StrictStr] = None
     """A concise verbal description of the model."""
 
-    Input: Optional[Filter]
+    Input: Optional[Filter] = None
     """Dictionary specification of input images"""
 
     Nodes: List[Node]
     """A list of analysis nodes. The ordering of this list is significant if Edges is absent."""
 
-    Edges: Optional[List[Edge]]
+    Edges: Optional[List[Edge]] = None
     """A list of edges between analysis nodes. If absent, the nodes are connected in the sequence presented in Nodes."""
 
 
 class ExplainerModel(BaseModel):
     """This is an example model.
 
     In schema terms, the structure that defines a JSON object is a "model". To avoid
@@ -574,15 +595,15 @@
         {"UnionField": 1}
         {"UnionField": "stringval"}
 
     Invalid examples::
 
         {"UnionField": 2.0}
     """
-    OptionalField: Optional[str]
+    OptionalField: Optional[str] = None
     """``OptionalField`` could be present or absent.
 
     Up to now, all fields have been required. If a field is optional, its type will be
     wrapped in ``Optional[]`` and will not have ``[Required]`` in its signature.
     """
     ListOrListOfLists: Union[List[int], List[List[int]]]
     """A 1- or 2D array of integers.
```

### Comparing `bsmschema-0.0.4/LICENSE` & `bsmschema-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsmschema-0.0.4/README.md` & `bsmschema-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bsmschema-0.0.4/pyproject.toml` & `bsmschema-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bsmschema-0.0.4/PKG-INFO` & `bsmschema-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsmschema
-Version: 0.0.4
+Version: 0.1.0
 Summary: A Pydantic schema for BIDS Stats Models
 Project-URL: Homepage, https://bids-standard.github.io/stats-models/
 Project-URL: Source code, https://github.com/bids-standard/stats-models
 Author-email: BIDS Contributors <bids.maintenance@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

