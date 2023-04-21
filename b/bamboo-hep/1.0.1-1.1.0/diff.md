# Comparing `tmp/bamboo-hep-1.0.1.tar.gz` & `tmp/bamboo-hep-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/cp3-cms/bamboo/dist/tmp1n4hn8vo/bamboo-hep-1.0.1.tar", last modified: Mon Feb 28 10:13:26 2022, max compression
+gzip compressed data, was "/builds/cp3-cms/bamboo/dist/tmpdprpj_3e/bamboo-hep-1.1.0.tar", last modified: Fri Apr 21 08:49:18 2023, max compression
```

## Comparing `bamboo-hep-1.0.1.tar` & `bamboo-hep-1.1.0.tar`

### file list

```diff
@@ -1,150 +1,159 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:26.000000 bamboo-hep-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      839 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1810 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      529 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)     4282 2022-02-28 10:13:26.000000 bamboo-hep-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4996 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_plots_nano.py
--rw-r--r--   0 root         (0) root         (0)    24470 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_jmesystcalc.py
--rw-r--r--   0 root         (0) root         (0)     1213 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_lumi_mask.py
--rwxr-xr-x   0 root         (0) root         (0)     4593 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/diffHistsAndFiles.py
--rw-r--r--   0 root         (0) root         (0)     1149 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_libtorcheval_nn.py
--rw-r--r--   0 root         (0) root         (0)     1469 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_postprocnanodeco.py
--rw-r--r--   0 root         (0) root         (0)     6760 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_plots_postprocnano.py
--rw-r--r--   0 root         (0) root         (0)     2935 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_plotswithreference.py
--rw-r--r--   0 root         (0) root         (0)      152 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2502 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_rochester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:26.000000 bamboo-hep-1.0.1/tests/data/
--rw-r--r--   0 root         (0) root         (0)    12358 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/Electron_EGamma_SF2D_loose_moriond17.json
--rw-r--r--   0 root         (0) root         (0)     5127 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/BTagging_loose_bjets_comb_DeepJet_2016Legacy.json
--rw-r--r--   0 root         (0) root         (0)  2161128 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/RoccoR2016.txt
--rw-r--r--   0 root         (0) root         (0)   386217 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DY_M50_2016postproc_JMEKin_bTagShape_puWeight.root
--rw-r--r--   0 root         (0) root         (0)     2544 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/nn1.pb
--rw-r--r--   0 root         (0) root         (0)    12017 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt
--rw-r--r--   0 root         (0) root         (0)     6130 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/nn1.pt
--rw-r--r--   0 root         (0) root         (0)   343170 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DY_M50_2016postproc_FatJetKin.root
--rw-r--r--   0 root         (0) root         (0)   428591 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DY_M50_2018postproc_hemfix.root
--rw-r--r--   0 root         (0) root         (0)     1620 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/nn1.onnx
--rw-r--r--   0 root         (0) root         (0)     5129 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/BTagging_loose_cjets_comb_DeepJet_2016Legacy.json
--rw-r--r--   0 root         (0) root         (0)     6911 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/nn1_lwtnn.json
--rw-r--r--   0 root         (0) root         (0)   427701 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DY_M50_2017postproc_JMEKin_METFixEE2017.root
--rw-r--r--   0 root         (0) root         (0)     9800 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/puweights.json
--rw-r--r--   0 root         (0) root         (0)   267881 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DY_M50_2016.root
--rw-r--r--   0 root         (0) root         (0)     1584 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/samples.txt
--rw-r--r--   0 root         (0) root         (0)      954 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/BTagging_loose_lightjets_incl_DeepJet_2016Legacy.json
--rw-r--r--   0 root         (0) root         (0)   192702 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/data/DoubleMuon_2016Gpostproc_JMEKin.root
--rw-r--r--   0 root         (0) root         (0)     1746 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_lwtnneval_nn.py
--rw-r--r--   0 root         (0) root         (0)     1665 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3670 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_sfweights.py
--rw-r--r--   0 root         (0) root         (0)     3708 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_nanodeco.py
--rw-r--r--   0 root         (0) root         (0)     3199 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_bamboorun.py
--rw-r--r--   0 root         (0) root         (0)     1706 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_tensorflowceval_nn.py
--rw-r--r--   0 root         (0) root         (0)     1518 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/tests/test_onnxruntimeeval.py
--rw-r--r--   0 root         (0) root         (0)     1325 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)    11597 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      135 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      501 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/zenodo_meta.json
--rw-r--r--   0 root         (0) root         (0)      341 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/AUTHORS
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/bamboo/
--rw-r--r--   0 root         (0) root         (0)    13887 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/batch_slurm.py
--rw-r--r--   0 root         (0) root         (0)    56355 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/dataframebackend.py
--rw-r--r--   0 root         (0) root         (0)    43743 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/analysismodules.py
--rw-r--r--   0 root         (0) root         (0)    40000 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/workflow.py
--rw-r--r--   0 root         (0) root         (0)    34046 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/treedecorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/bamboo/scripts/
--rw-r--r--   0 root         (0) root         (0)     2721 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/scripts/bambooRun.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25372 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/scripts/makePUReWeightJSON.py
--rw-r--r--   0 root         (0) root         (0)     1392 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/utils.py
--rw-r--r--   0 root         (0) root         (0)      197 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66690 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/treeoperations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/bamboo/data/
--rw-r--r--   0 root         (0) root         (0)     8085 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/data/FindFilesystem.cmake
--rw-r--r--   0 root         (0) root         (0)      761 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/data/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5575 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/data/main.cc
--rw-r--r--   0 root         (0) root         (0)    73073 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/analysisutils.py
--rw-r--r--   0 root         (0) root         (0)    48396 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/plots.py
--rw-r--r--   0 root         (0) root         (0)    15943 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/batch.py
--rw-r--r--   0 root         (0) root         (0)    27652 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/treeproxies.py
--rw-r--r--   0 root         (0) root         (0)    37757 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/treefunctions.py
--rw-r--r--   0 root         (0) root         (0)    15256 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/batch_htcondor.py
--rw-r--r--   0 root         (0) root         (0)    28883 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/scalefactors.py
--rw-r--r--   0 root         (0) root         (0)     8382 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/bamboo/root.py
--rw-r--r--   0 root         (0) root         (0)     2312 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/examples/
--rw-r--r--   0 root         (0) root         (0)      927 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/analysis1.yml
--rw-r--r--   0 root         (0) root         (0)     8587 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/adl_benchmarks.py
--rw-r--r--   0 root         (0) root         (0)    19148 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/nanozmumu.py
--rw-r--r--   0 root         (0) root         (0)      638 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/test_skim.yml
--rw-r--r--   0 root         (0) root         (0)    12017 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt
--rw-r--r--   0 root         (0) root         (0)      217 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/test1.yml
--rw-r--r--   0 root         (0) root         (0)    20133 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/preselectskim.py
--rw-r--r--   0 root         (0) root         (0)      333 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/df_ttW.py
--rw-r--r--   0 root         (0) root         (0)      304 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/cern.ini
--rw-r--r--   0 root         (0) root         (0)      196 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/adl_benchmarks.yml
--rw-r--r--   0 root         (0) root         (0)     1846 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/analysis_zmm.yml
--rw-r--r--   0 root         (0) root         (0)      579 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/cmsPhase2Sim_test.yml
--rw-r--r--   0 root         (0) root         (0)     3103 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/analysis_eletnp.yml
--rw-r--r--   0 root         (0) root         (0)     5054 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/cmsPhase2Sim.py
--rw-r--r--   0 root         (0) root         (0)      415 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/ingrid.ini
--rw-r--r--   0 root         (0) root         (0)     4434 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/eletnp.py
--rw-r--r--   0 root         (0) root         (0)     9732 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/examples/df_nano.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/cpp/
--rw-r--r--   0 root         (0) root         (0)     2379 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/cpp/bamboohelpers.h
--rw-r--r--   0 root         (0) root         (0)     1510 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/cpp/printprogress.h
--rw-r--r--   0 root         (0) root         (0)     8386 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/cpp/scalefactors.h
--rw-r--r--   0 root         (0) root         (0)    10185 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/cpp/range.h
--rw-r--r--   0 root         (0) root         (0)     4740 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/doc/
--rw-r--r--   0 root         (0) root         (0)       82 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/rtd-environment.yml
--rw-r--r--   0 root         (0) root         (0)    11969 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/advanced.rst
--rw-r--r--   0 root         (0) root         (0)     5898 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     4693 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1977 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/treefunctions.rst
--rw-r--r--   0 root         (0) root         (0)    11447 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/hacking.rst
--rw-r--r--   0 root         (0) root         (0)    26754 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/userguide.rst
--rw-r--r--   0 root         (0) root         (0)      993 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/apiref.rst
--rw-r--r--   0 root         (0) root         (0)    53648 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/recipes.rst
--rw-r--r--   0 root         (0) root         (0)    18790 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/doc/install.rst
--rw-r--r--   0 root         (0) root         (0)     1827 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/ext/
--rw-r--r--   0 root         (0) root         (0)       74 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/Config.cmake.in
--rwxr-xr-x   0 root         (0) root         (0)      901 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/install_lwtnn.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/ext/include/
--rw-r--r--   0 root         (0) root         (0)      963 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/bambootorch.h
--rw-r--r--   0 root         (0) root         (0)      127 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/BinnedValuesJSONParser.h
--rw-r--r--   0 root         (0) root         (0)      653 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/bamboolwtnn.h
--rw-r--r--   0 root         (0) root         (0)    11878 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/Histogram.h
--rw-r--r--   0 root         (0) root         (0)      255 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/bamboorandom.h
--rw-r--r--   0 root         (0) root         (0)     1556 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/LumiMask.h
--rw-r--r--   0 root         (0) root         (0)     5028 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/bambooonnxruntime.h
--rw-r--r--   0 root         (0) root         (0)      548 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/kinematicvariations.h
--rw-r--r--   0 root         (0) root         (0)     4795 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/BTagCalibrationStandalone.h
--rw-r--r--   0 root         (0) root         (0)      971 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/RochesterCorrectionCalculator.h
--rw-r--r--   0 root         (0) root         (0)     4855 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/RoccoR.h
--rw-r--r--   0 root         (0) root         (0)     7628 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/BinnedValues.h
--rw-r--r--   0 root         (0) root         (0)     4289 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/include/bambootensorflowc.h
--rw-r--r--   0 root         (0) root         (0)     5504 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/ext/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/ext/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      890 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/cmake/modules/FindONNXRuntime.cmake
--rw-r--r--   0 root         (0) root         (0)     1034 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/cmake/modules/FindTensorflowC.cmake
--rwxr-xr-x   0 root         (0) root         (0)      728 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/install_tensorflow-c.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 10:13:25.000000 bamboo-hep-1.0.1/ext/src/
--rw-r--r--   0 root         (0) root         (0)      304 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/bamboorandom.cc
--rw-r--r--   0 root         (0) root         (0)     2434 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/BinnedValues.cc
--rw-r--r--   0 root         (0) root         (0)     1157 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/bamboolwtnn.cc
--rw-r--r--   0 root         (0) root         (0)     1396 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/LumiMask.cc
--rw-r--r--   0 root         (0) root         (0)    20087 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/BTagCalibrationStandalone.cpp
--rw-r--r--   0 root         (0) root         (0)     1077 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/bambootorch.cc
--rw-r--r--   0 root         (0) root         (0)     7285 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/BinnedValuesJSONParser.cc
--rw-r--r--   0 root         (0) root         (0)     2733 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/bambooonnxruntime.cc
--rw-r--r--   0 root         (0) root         (0)     9647 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/RoccoR.cc
--rw-r--r--   0 root         (0) root         (0)     6046 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/bambootensorflowc.cc
--rw-r--r--   0 root         (0) root         (0)      664 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/tester_fatjets.cc
--rw-r--r--   0 root         (0) root         (0)     2960 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/ext/src/RochesterCorrectionCalculator.cc
--rw-r--r--   0 root         (0) root         (0)    35149 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/COPYING
--rw-r--r--   0 root         (0) root         (0)      787 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     2988 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     4424 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/publish_release_to_zenodo.py
--rw-r--r--   0 root         (0) root         (0)      179 2022-02-28 10:11:51.000000 bamboo-hep-1.0.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      839 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/.readthedocs.yml
+-rw-r--r--   0 root         (0) root         (0)     4282 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_plots_nano.py
+-rw-r--r--   0 root         (0) root         (0)    24533 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_jmesystcalc.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_lumi_mask.py
+-rwxr-xr-x   0 root         (0) root         (0)     4593 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/diffHistsAndFiles.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_libtorcheval_nn.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_postprocnanodeco.py
+-rw-r--r--   0 root         (0) root         (0)     6760 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_plots_postprocnano.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_plotswithreference.py
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_rochester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/tests/data/
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/Electron_EGamma_SF2D_loose_moriond17.json
+-rw-r--r--   0 root         (0) root         (0)     5127 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/BTagging_loose_bjets_comb_DeepJet_2016Legacy.json
+-rw-r--r--   0 root         (0) root         (0)  2161128 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/RoccoR2016.txt
+-rw-r--r--   0 root         (0) root         (0)   386217 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DY_M50_2016postproc_JMEKin_bTagShape_puWeight.root
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/nn1.pb
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/nn1.pt
+-rw-r--r--   0 root         (0) root         (0)   343170 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DY_M50_2016postproc_FatJetKin.root
+-rw-r--r--   0 root         (0) root         (0)   428591 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DY_M50_2018postproc_hemfix.root
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/nn1.onnx
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/BTagging_loose_cjets_comb_DeepJet_2016Legacy.json
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/nn1_lwtnn.json
+-rw-r--r--   0 root         (0) root         (0)   427701 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DY_M50_2017postproc_JMEKin_METFixEE2017.root
+-rw-r--r--   0 root         (0) root         (0)     9800 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/puweights.json
+-rw-r--r--   0 root         (0) root         (0)   267881 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DY_M50_2016.root
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/samples.txt
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/BTagging_loose_lightjets_incl_DeepJet_2016Legacy.json
+-rw-r--r--   0 root         (0) root         (0)   192702 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/data/DoubleMuon_2016Gpostproc_JMEKin.root
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_sofie_nn.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_lwtnneval_nn.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3670 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_sfweights.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_nanodeco.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_bamboorun.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_tensorflowceval_nn.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/tests/test_onnxruntimeeval.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)    11597 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/zenodo_meta.json
+-rw-r--r--   0 root         (0) root         (0)      341 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/AUTHORS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo/
+-rw-r--r--   0 root         (0) root         (0)    13887 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/batch_slurm.py
+-rw-r--r--   0 root         (0) root         (0)    56355 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/dataframebackend.py
+-rw-r--r--   0 root         (0) root         (0)    43743 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/analysismodules.py
+-rw-r--r--   0 root         (0) root         (0)    40000 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    34078 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/treedecorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo/scripts/
+-rw-r--r--   0 root         (0) root         (0)     2721 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/scripts/bambooRun.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25372 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/scripts/makePUReWeightJSON.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/utils.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66693 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/treeoperations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo/data/
+-rw-r--r--   0 root         (0) root         (0)     8085 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/data/FindFilesystem.cmake
+-rw-r--r--   0 root         (0) root         (0)      761 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/data/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5575 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/data/main.cc
+-rw-r--r--   0 root         (0) root         (0)    74071 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/analysisutils.py
+-rw-r--r--   0 root         (0) root         (0)    48600 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/plots.py
+-rw-r--r--   0 root         (0) root         (0)    15943 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/batch.py
+-rw-r--r--   0 root         (0) root         (0)    30380 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/treeproxies.py
+-rw-r--r--   0 root         (0) root         (0)    39137 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/treefunctions.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/batch_htcondor.py
+-rw-r--r--   0 root         (0) root         (0)    45244 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/scalefactors.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/bamboo/root.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/CONTRIBUTING.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/examples/
+-rw-r--r--   0 root         (0) root         (0)      927 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/analysis1.yml
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/adl_benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)    19281 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/nanozmumu.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/test_skim.yml
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/test1.yml
+-rw-r--r--   0 root         (0) root         (0)    20133 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/preselectskim.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/df_ttW.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/cern.ini
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/adl_benchmarks.yml
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/analysis_zmm.yml
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/cmsPhase2Sim_test.yml
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/analysis_eletnp.yml
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/cmsPhase2Sim.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/ingrid.ini
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/eletnp.py
+-rw-r--r--   0 root         (0) root         (0)     9732 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/examples/df_nano.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/cpp/
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/cpp/bamboohelpers.h
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/cpp/printprogress.h
+-rw-r--r--   0 root         (0) root         (0)     8386 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/cpp/scalefactors.h
+-rw-r--r--   0 root         (0) root         (0)    10185 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/cpp/range.h
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/doc/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/rtd-environment.yml
+-rw-r--r--   0 root         (0) root         (0)    12028 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/advanced.rst
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/treefunctions.rst
+-rw-r--r--   0 root         (0) root         (0)    11447 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/hacking.rst
+-rw-r--r--   0 root         (0) root         (0)    26754 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/userguide.rst
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/apiref.rst
+-rw-r--r--   0 root         (0) root         (0)    55331 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/recipes.rst
+-rw-r--r--   0 root         (0) root         (0)    18663 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/doc/install.rst
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/ext/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/Config.cmake.in
+-rwxr-xr-x   0 root         (0) root         (0)      901 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/install_lwtnn.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/ext/include/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bambootorch.h
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/BinnedValuesJSONParser.h
+-rw-r--r--   0 root         (0) root         (0)      653 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bamboolwtnn.h
+-rw-r--r--   0 root         (0) root         (0)    11878 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/Histogram.h
+-rw-r--r--   0 root         (0) root         (0)      255 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bamboorandom.h
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/LumiMask.h
+-rw-r--r--   0 root         (0) root         (0)     5028 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bambooonnxruntime.h
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bamboosofie.h
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/kinematicvariations.h
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/BTagCalibrationStandalone.h
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/RochesterCorrectionCalculator.h
+-rw-r--r--   0 root         (0) root         (0)     4855 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/RoccoR.h
+-rw-r--r--   0 root         (0) root         (0)     7628 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/BinnedValues.h
+-rw-r--r--   0 root         (0) root         (0)     4289 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/include/bambootensorflowc.h
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/ext/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/ext/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/cmake/modules/FindONNXRuntime.cmake
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/cmake/modules/FindTensorflowC.cmake
+-rwxr-xr-x   0 root         (0) root         (0)      728 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/install_tensorflow-c.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/ext/src/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/bamboorandom.cc
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/BinnedValues.cc
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/bamboolwtnn.cc
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/LumiMask.cc
+-rw-r--r--   0 root         (0) root         (0)    20087 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/BTagCalibrationStandalone.cpp
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/bambootorch.cc
+-rw-r--r--   0 root         (0) root         (0)     7285 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/BinnedValuesJSONParser.cc
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/bambooonnxruntime.cc
+-rw-r--r--   0 root         (0) root         (0)     9647 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/RoccoR.cc
+-rw-r--r--   0 root         (0) root         (0)     6046 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/bambootensorflowc.cc
+-rw-r--r--   0 root         (0) root         (0)      664 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/tester_fatjets.cc
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/ext/src/RochesterCorrectionCalculator.cc
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/CHANGELOG.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     4282 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 08:49:18.000000 bamboo-hep-1.1.0/bamboo_hep.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/publish_release_to_zenodo.py
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-21 08:47:29.000000 bamboo-hep-1.1.0/.gitignore
```

### Comparing `bamboo-hep-1.0.1/NOTICE` & `bamboo-hep-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/.pre-commit-config.yaml` & `bamboo-hep-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/.readthedocs.yml` & `bamboo-hep-1.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/PKG-INFO` & `bamboo-hep-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-hep
-Version: 1.0.1
+Version: 1.1.0
 Summary: A high-level HEP analysis library for ROOT::RDataFrame
 Home-page: https://gitlab.cern.ch/cp3-cms/bamboo
 Author: Pieter David
 Author-email: pieter.david@cern.ch
 License: GPL-3.0-or-later
 Keywords: ROOT,RDataFrame
 Platform: UNKNOWN
```

### Comparing `bamboo-hep-1.0.1/tests/test_plots_nano.py` & `bamboo-hep-1.1.0/tests/test_plots_nano.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     plots.append(Plot.make1D(
         "nElectrons", op.rng_len(electrons), noSel, EqBin(10, 0., 10.),
         title="Number of electrons", xTitle="N_{e}"))
     hasMuon = noSel.refine("hasMuon", cut=(op.rng_len(muons) > 0))
     plots.append(Plot.make1D(
         "hasMuon_leadMuPT", muons[0].pt, hasMuon, EqBin(50, 0., 100.),
         title="Leading muon PT", xTitle="p_{T}(mu_{1})"))
-    forceDefine(tup._Jet.calcProd, noSel)
+    for calcProd in tup._Jet.calcProds:
+        forceDefine(calcProd, noSel)
     jets = op.select(tup.Jet, lambda j: op.AND(j.pt > 20., op.abs(j.eta) < 2.4, j.jetId & 2))
     cleanedJets = op.select(jets, lambda j: op.AND(
         op.NOT(op.rng_any(electrons, lambda ele: op.deltaR(j.p4, ele.p4) < 0.3)),
         op.NOT(op.rng_any(muons, lambda mu: op.deltaR(j.p4, mu.p4) < 0.3))))
     plots.append(Plot.make1D(
         "nCleanedJets", op.rng_len(cleanedJets), noSel, EqBin(10, 0., 10.),
         title="Number of cleaned jets", xTitle="N_{j}"))
```

### Comparing `bamboo-hep-1.0.1/tests/test_jmesystcalc.py` & `bamboo-hep-1.1.0/tests/test_jmesystcalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,24 @@
             toRVecFloat(tup.Jet_chEmEF),
         ]
     if not (forMET and isMETFixEE2017):
         args.append(toRVecInt(tup.Jet_jetId if addHEM2018Issue else []))
     args.append(tup.fixedGridRhoFastjetAll)
     if isMC:
         args += [
+            toRVecInt(tup.Jet_partonFlavour),
             ((tup.run << 20) + (tup.luminosityBlock << 10) + tup.event
              + 1 + (int(tup.Jet_eta[0] / .01) if tup.nJet != 0 else 0)),
             toRVecFloat(tup.GenJet_pt),
             toRVecFloat(tup.GenJet_eta),
             toRVecFloat(tup.GenJet_phi),
             toRVecFloat(tup.GenJet_mass)
         ]
     else:
-        args += [0, toRVecFloat([]), toRVecFloat([]), toRVecFloat([]), toRVecFloat([])]
+        args += [toRVecInt([]), 0, toRVecFloat([]), toRVecFloat([]), toRVecFloat([]), toRVecFloat([])]
     if forMET:
         args += [tup.RawMET_phi, tup.RawMET_pt]
         if not isMETFixEE2017:
             args += [tup.MET_MetUnclustEnUpDeltaX, tup.MET_MetUnclustEnUpDeltaY]
         else:
             args += [tup.METFixEE2017_MetUnclustEnUpDeltaX, tup.METFixEE2017_MetUnclustEnUpDeltaY]
         args += [toRVecFloat(getattr(tup, f"CorrT1METJet_{varNm}"))
@@ -192,15 +193,15 @@
     config.puppi_resol_for = puppiResolFwd
 
 
 @pytest.fixture(scope="module")
 def nanojetargsMC16():
     from bamboo.root import gbl
     f = gbl.TFile.Open(os.path.join(testData, "DY_M50_2016.root"))
-    for tup in getEventWith(f, (lambda tup: tup.nJet >= 5)):
+    for tup in getEventWith(f, (lambda tup_: tup_.nJet >= 5)):
         yield getJetMETArgs(tup, isMC=True, forMET=False)
 
 
 @pytest.fixture(scope="module")
 def nanojetargsMC16_postvalues():
     from bamboo.root import gbl
     f = gbl.TFile.Open(os.path.join(testData, "DY_M50_2016postproc_JMEKin_bTagShape_puWeight.root"))
```

### Comparing `bamboo-hep-1.0.1/tests/test_lumi_mask.py` & `bamboo-hep-1.1.0/tests/test_lumi_mask.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/diffHistsAndFiles.py` & `bamboo-hep-1.1.0/tests/diffHistsAndFiles.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_libtorcheval_nn.py` & `bamboo-hep-1.1.0/tests/test_libtorcheval_nn.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_postprocnanodeco.py` & `bamboo-hep-1.1.0/tests/test_postprocnanodeco.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_plots_postprocnano.py` & `bamboo-hep-1.1.0/tests/test_plots_postprocnano.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_plotswithreference.py` & `bamboo-hep-1.1.0/tests/test_plotswithreference.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_rochester.py` & `bamboo-hep-1.1.0/tests/test_rochester.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/Electron_EGamma_SF2D_loose_moriond17.json` & `bamboo-hep-1.1.0/tests/data/Electron_EGamma_SF2D_loose_moriond17.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/BTagging_loose_bjets_comb_DeepJet_2016Legacy.json` & `bamboo-hep-1.1.0/tests/data/BTagging_loose_bjets_comb_DeepJet_2016Legacy.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/RoccoR2016.txt` & `bamboo-hep-1.1.0/tests/data/RoccoR2016.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DY_M50_2016postproc_JMEKin_bTagShape_puWeight.root` & `bamboo-hep-1.1.0/tests/data/DY_M50_2016postproc_JMEKin_bTagShape_puWeight.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/nn1.pb` & `bamboo-hep-1.1.0/tests/data/nn1.pb`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt` & `bamboo-hep-1.1.0/tests/data/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/nn1.pt` & `bamboo-hep-1.1.0/tests/data/nn1.pt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DY_M50_2016postproc_FatJetKin.root` & `bamboo-hep-1.1.0/tests/data/DY_M50_2016postproc_FatJetKin.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DY_M50_2018postproc_hemfix.root` & `bamboo-hep-1.1.0/tests/data/DY_M50_2018postproc_hemfix.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/nn1.onnx` & `bamboo-hep-1.1.0/tests/data/nn1.onnx`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/BTagging_loose_cjets_comb_DeepJet_2016Legacy.json` & `bamboo-hep-1.1.0/tests/data/BTagging_loose_cjets_comb_DeepJet_2016Legacy.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/nn1_lwtnn.json` & `bamboo-hep-1.1.0/tests/data/nn1_lwtnn.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DY_M50_2017postproc_JMEKin_METFixEE2017.root` & `bamboo-hep-1.1.0/tests/data/DY_M50_2017postproc_JMEKin_METFixEE2017.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/puweights.json` & `bamboo-hep-1.1.0/tests/data/puweights.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DY_M50_2016.root` & `bamboo-hep-1.1.0/tests/data/DY_M50_2016.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/samples.txt` & `bamboo-hep-1.1.0/tests/data/samples.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/BTagging_loose_lightjets_incl_DeepJet_2016Legacy.json` & `bamboo-hep-1.1.0/tests/data/BTagging_loose_lightjets_incl_DeepJet_2016Legacy.json`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/data/DoubleMuon_2016Gpostproc_JMEKin.root` & `bamboo-hep-1.1.0/tests/data/DoubleMuon_2016Gpostproc_JMEKin.root`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_lwtnneval_nn.py` & `bamboo-hep-1.1.0/tests/test_lwtnneval_nn.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/conftest.py` & `bamboo-hep-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_sfweights.py` & `bamboo-hep-1.1.0/tests/test_sfweights.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_nanodeco.py` & `bamboo-hep-1.1.0/tests/test_nanodeco.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_bamboorun.py` & `bamboo-hep-1.1.0/tests/test_bamboorun.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_tensorflowceval_nn.py` & `bamboo-hep-1.1.0/tests/test_tensorflowceval_nn.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/tests/test_onnxruntimeeval.py` & `bamboo-hep-1.1.0/tests/test_onnxruntimeeval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os.path
 
 import pytest
 
 from bamboo.root import findLibrary
+from bamboo.root import _rootVersion_split
 from helpers import isclose_float
 
 onnxRuntime_found = findLibrary("libonnxruntime")
 if not onnxRuntime_found and "VIRTUAL_ENV" in os.environ:
     ortlib_guessed_path = os.path.join(os.environ["VIRTUAL_ENV"], "lib", "libonnxruntime.so")
     if os.path.exists(ortlib_guessed_path):
         onnxRuntime_found = ortlib_guessed_path
-pytestmark = pytest.mark.skipif(not onnxRuntime_found, reason="ONNX Runtime not found")
+# workaround for https://github.com/root-project/root/issues/11581
+pytestmark = pytest.mark.skipif(
+    (not onnxRuntime_found) or (_rootVersion_split[0] == 6 and _rootVersion_split[1] == 26),
+    reason="ONNX Runtime not found; bug in ROOT 6.26")
 
 testData = os.path.join(os.path.dirname(__file__), "data")
 
 
 @pytest.fixture(scope="module")
 def onnxruntime_nn1():
     from bamboo.root import gbl, loadONNXRuntime
```

### Comparing `bamboo-hep-1.0.1/setup.py` & `bamboo-hep-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/LICENSE` & `bamboo-hep-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/batch_slurm.py` & `bamboo-hep-1.1.0/bamboo/batch_slurm.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/dataframebackend.py` & `bamboo-hep-1.1.0/bamboo/dataframebackend.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/analysismodules.py` & `bamboo-hep-1.1.0/bamboo/analysismodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,21 +56,21 @@
         if isinstance(action, argparse._StoreTrueAction):
             if getattr(args, action.dest):
                 argv.append(action.option_strings[0])
         elif isinstance(action, argparse._AppendAction):
             items = getattr(args, action.dest)
             if items:
                 for item in items:
-                    argv.append(f"{action.option_strings[0]}={item}")
+                    argv.append(f"{action.option_strings[0]} {item}")
         elif isinstance(action, argparse._StoreAction):
             val = getattr(args, action.dest)
             if isinstance(val, list):
-                argv.append(f"{action.option_strings[0]}=" + " ".join(str(v) for v in val))
+                argv.append(f"{action.option_strings[0]} " + " ".join(str(v) for v in val))
             elif val is not None:
-                argv.append(f"{action.option_strings[0]}={val}")
+                argv.append(f"{action.option_strings[0]} {val}")
         else:
             raise RuntimeError(f"Reconstruction of action {action} not supported")
     return argv
 
 
 def parseRunRange(rrStr):
     return tuple(int(t.strip()) for t in rrStr.split(","))
```

### Comparing `bamboo-hep-1.0.1/bamboo/workflow.py` & `bamboo-hep-1.1.0/bamboo/workflow.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/treedecorators.py` & `bamboo-hep-1.1.0/bamboo/treedecorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     :py:class:`~.NanoSystematicVarSpec` for on-the-fly corrections
         and systematic variation calculation
     """
     def __init__(self, nomName="nominal", origName="raw", exclVars=None, changes=None, **colsAndAttrs):
         super().__init__(
             nomName=nomName, origName=origName, isCalc=True,
             exclVars=(exclVars if exclVars is not None else (origName,)))
-        self.colsAndAttrs = dict()
+        self.colsAndAttrs = dict()  # e.g. "Jet" -> ("pt", "mass")
         for colgrp, attrs in colsAndAttrs.items():
             if isinstance(attrs, str):
                 attrs = (attrs,)
             self.colsAndAttrs[colgrp] = attrs
         self.changes = (changes if changes is not None else dict())
 
     def appliesTo(self, name):
```

### Comparing `bamboo-hep-1.0.1/bamboo/scripts/bambooRun.py` & `bamboo-hep-1.1.0/bamboo/scripts/bambooRun.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/scripts/makePUReWeightJSON.py` & `bamboo-hep-1.1.0/bamboo/scripts/makePUReWeightJSON.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/utils.py` & `bamboo-hep-1.1.0/bamboo/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/treeoperations.py` & `bamboo-hep-1.1.0/bamboo/treeoperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1695,14 +1695,14 @@
 
 def collectSystVars(exprs):
     # { varName : { expr : [ nodes to change ] } }
     systVars = defaultdict(dict)
     for expr in exprs:
         toChangeForThis = defaultdict(list)
         for nd in set(collectNodes(expr,
-                                   select=(lambda nd: isinstance(nd, OpWithSyst) and nd.variations),
+                                   select=(lambda nd_: isinstance(nd_, OpWithSyst) and nd_.variations),
                                    defCache=VisitOnceAndStopAt())):
             for vari in nd.variations:
                 toChangeForThis[vari].append(nd)
         for vari, variNodes in toChangeForThis.items():
             systVars[vari][expr] = variNodes
     return systVars
```

### Comparing `bamboo-hep-1.0.1/bamboo/data/FindFilesystem.cmake` & `bamboo-hep-1.1.0/bamboo/data/FindFilesystem.cmake`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/data/CMakeLists.txt` & `bamboo-hep-1.1.0/bamboo/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/data/main.cc` & `bamboo-hep-1.1.0/bamboo/data/main.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/analysisutils.py` & `bamboo-hep-1.1.0/bamboo/analysisutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,40 +802,46 @@
                 if ln.startswith("[") and ln.endswith("]"):
                     readSources.append(ln[1:-1])
         logger.debug(f"Found {len(readSources):d} JES uncertainty sources in {plf}: {', '.join(readSources)}")
         sources = readSources
     return plf, sources
 
 
-def _enableCalcSystematics(variProxy, enableSystematics=None, default=True, name=""):
+def _filterCalcSystematics(variProxy, calcHandle, enableSystematics=None, default=True, name=""):
     if enableSystematics is None:
         if default:
             def enableSystematics(x):
                 return True
         else:
             def enableSystematics(x):
                 return False
     elif (not callable(enableSystematics)) and hasattr(enableSystematics, "__contains__"):
         enableSystematics = enableSystematics.__contains__
     all_enabled = set()
     all_avail = set()
     for attN, opWithSyst in variProxy.brMapMap[variProxy.withSystName].items():
-        enable = []
-        for vari in variProxy._available(attN):
+        # variations provided by this calculator
+        calc_vars = variProxy.availableVariations(attN, calcHandle)
+        # variations registered with this collection that are provided by others...
+        other_vars = set(opWithSyst.variations).difference(calc_vars)
+        # ...and keep those
+        enable = set(other_vars)
+        all_avail.update(opWithSyst.variations)
+        for vari in calc_vars:
             if vari != "nominal":
                 all_avail.add(vari)
                 vari_c = vari
                 if vari.endswith("up"):
                     vari_c = vari[:-2]
                 elif vari.endswith("down"):
                     vari_c = vari[:-4]
                 if enableSystematics(vari) or enableSystematics(vari_c):
-                    enable.append(vari)
+                    enable.add(vari)
         if enable or opWithSyst.variations:
-            opWithSyst.variations = tuple(enable)  # fine, just (re)created by _initFromCalc
+            opWithSyst.variations = tuple(enable)
             all_enabled.update(enable)
     if all_enabled:
         logger.debug("Enabled systematic variations for {}: {}".format(
             name, " ".join(all_enabled)))
     if len(all_enabled) != len(all_avail):
         logger.debug("Disabled systematic variations for {}: {}".format(
             name, " ".join(all_avail.difference(all_enabled))))
@@ -947,42 +953,47 @@
         (returned from :py:meth:`~bamboo.analysismodules.HistogramsModule.prepareTree`)
     :param uName: [deprecated, ignored]
         unique name for the correction calculator (sample name is a safe choice)
     """
     if uName != "":
         warnings.warn("Passing uName to configureJets"
                       "is not necessary anymore (and ignored), please update",
-                      DeprecationWarning)
+                      DeprecationWarning, stacklevel=1)
     from . import treefunctions as op  # first to load default headers/libs, if still needed
     from .treefunctions import _to, _tp  # treeoperations and treeproxies
     from itertools import repeat
     isFat = jetType.startswith("AK8")
     aJet = variProxy.orig[0]
     if isFat and subjets is None:
         evt = variProxy._parent
         subjets = evt.SubJet
-    args = [getattr(aJet, comp).op.arg for comp in ("pt", "eta", "phi", "mass", "rawFactor", "area")]
+    args = [getattr(aJet, comp).op.arg for comp in ("pt", "eta", "phi", "mass",
+                                                    "rawFactor", "area")]
     if isFat:
         args.append(aJet.msoftdrop.op.arg)
         args += [getattr(aJet, f"subJet{iSJ:d}").idx.op.arg for iSJ in range(1, 3)]
         args += [getattr(subjets[0], comp).op.arg for comp in ("pt", "eta", "phi", "mass")]
     args.append(aJet.jetId.op.arg)
     args.append(_to.GetColumn("Float_t", "fixedGridRhoFastjetAll"))
     if isMC:
+        if not isFat:
+            args.append(aJet.partonFlavour.op.arg)
         evt = variProxy._parent
         args.append((evt.run << 20) + (evt.luminosityBlock << 10) + evt.event + 1 + op.static_cast("unsigned",
                     op.switch(op.rng_len(variProxy.orig) != 0, variProxy.orig[0].eta / .01, op.c_float(0.))))
         aGJet = evt.GenJet[0]
         if isFat:
             aGJet = evt.GenJetAK8[0]
         args += [getattr(aGJet, comp).op.arg for comp in ("pt", "eta", "phi", "mass")]
         if isFat:
             aGSJet = evt.SubGenJetAK8[0]
             args += [getattr(aGSJet, comp).op.arg for comp in ("pt", "eta", "phi", "mass")]
     else:
+        if not isFat:
+            args.append(_to.ExtVar("ROOT::VecOps::RVec<int>", "ROOT::VecOps::RVec<int>{}"))
         args.append(_tp.makeConst(0, "unsigned"))  # no seed
         args += list(repeat(_to.ExtVar(
             "ROOT::VecOps::RVec<float>", "ROOT::VecOps::RVec<float>{}"),
             (8 if isFat else 4)))
     # fill configuration
     from CMSJMECalculators import config as calcConfigs
     config = (calcConfigs.JetVariations() if not isFat else calcConfigs.FatJetVariations())
@@ -1073,18 +1084,19 @@
         config.puppi_resol_cen = fatjet_puppi_msd_params["resol_cen"]
         config.puppi_resol_for = fatjet_puppi_msd_params["resol_fwd"]
 
     # define calculator and initialize
     from .root import loadJMESystematicsCalculators, gbl
     loadJMESystematicsCalculators(backend=backend)
     jetcalcName = backend.symbol(f"const auto <<name>> = {config.cppConstruct};")
-    variProxy._initCalc(op.extVar(config.calcClass, jetcalcName),
-                        calcHandle=getattr(gbl, jetcalcName), args=args)
-    variProxy._initFromCalc()
-    _enableCalcSystematics(variProxy, enableSystematics=enableSystematics, default=isMC, name="Jet")
+    calcHandle = getattr(gbl, jetcalcName)
+    variProxy.addCalculator(op.extVar(config.calcClass, jetcalcName),
+                            calcHandle=calcHandle, args=args)
+    _filterCalcSystematics(variProxy, calcHandle,
+                           enableSystematics=enableSystematics, default=isMC, name="Jet")
 
 
 def configureType1MET(
         variProxy, jec=None, smear=None, isT1Smear=False,
         useGenMatch=True, genMatchDR=0.2, genMatchDPt=3.,
         jesUncertaintySources=None, regroupTag="",
         splitJER=False, addHEM2018Issue=False, enableSystematics=None,
@@ -1126,41 +1138,44 @@
     :param uName: [deprecated, ignored]
         unique name for the correction calculator (sample name is a safe choice)
     :param isMC: MC or not
     """
     if uName != "":
         warnings.warn("Passing uName to configureType1MET"
                       "is not necessary anymore (and ignored), please update",
-                      DeprecationWarning)
+                      DeprecationWarning, stacklevel=1)
     isFixEE2017 = variProxy.orig.pt.op.name.startswith("METFixEE2017_")
     isPuppi = ("Puppi" in variProxy.orig.pt.op.name)
     from . import treefunctions as op  # first to load default headers/libs, if still needed
     from .treefunctions import _to, _tp  # treeoperations and treeproxies
     from itertools import repeat
     evt = variProxy._parent
     jets = evt._Jet.orig if hasattr(evt, "_Jet") else evt.Jet[0]
     args = [getattr(jets[0], comp).op.arg for comp in (
-        "pt", "eta", "phi", "mass", "rawFactor", "area", "muonSubtrFactor", "neEmEF", "chEmEF")]
+        "pt", "eta", "phi", "mass", "rawFactor", "area",
+        "muonSubtrFactor", "neEmEF", "chEmEF")]
     if addHEM2018Issue:
         if isFixEE2017:
             raise RuntimeError(
                 "You can either use the EE 2017 fix, or the 2018 HEM issue variation, "
                 "but not both at a time, for the MET")
         args.append(jets[0].jetId.op.arg)
     else:
         if not isFixEE2017:
             args.append(_to.ExtVar("ROOT::VecOps::RVec<int>", "ROOT::VecOps::RVec<int>{}"))
     args.append(_to.GetColumn("Float_t", "fixedGridRhoFastjetAll"))
     evt = variProxy._parent
     if isMC:
+        args.append(jets[0].partonFlavour.op.arg)
         args.append((evt.run << 20) + (evt.luminosityBlock << 10) + evt.event + 1 + op.static_cast(
             "unsigned", op.switch(op.rng_len(jets) != 0, jets[0].eta / .01, op.c_float(0.))))
         aGJet = evt.GenJet[0]
         args += [getattr(aGJet, comp).op.arg for comp in ("pt", "eta", "phi", "mass")]
     else:
+        args.append(_to.ExtVar("ROOT::VecOps::RVec<int>", "ROOT::VecOps::RVec<int>{}"))
         args.append(_tp.makeConst(0, "unsigned"))  # no seed
         args += list(repeat(_to.ExtVar("ROOT::VecOps::RVec<float>", "ROOT::VecOps::RVec<float>{}"), 4))
     if isPuppi:
         args += [evt.RawPuppiMET.phi, evt.RawPuppiMET.pt]
     else:
         args += [evt.RawMET.phi, evt.RawMET.pt]
     args += [variProxy.orig.MetUnclustEnUpDeltaX, variProxy.orig.MetUnclustEnUpDeltaY]
@@ -1225,18 +1240,19 @@
                     config.jesUncertainties = [(src, plf) for src in jesUncertaintySources]
     if jec is None and jesUncertaintySources:
         logger.error("JES uncertainty specified, but no JEC tag; none will be evaluated")
     # define calculator and initialize
     from .root import loadJMESystematicsCalculators, gbl
     loadJMESystematicsCalculators(backend=backend)
     metcalcName = backend.symbol(f"const auto <<name>> = {config.cppConstruct};")
-    variProxy._initCalc(op.extVar(config.calcClass, metcalcName),
-                        calcHandle=getattr(gbl, metcalcName), args=args)
-    variProxy._initFromCalc()
-    _enableCalcSystematics(variProxy, enableSystematics=enableSystematics, default=isMC, name="MET")
+    calcHandle = getattr(gbl, metcalcName)
+    variProxy.addCalculator(op.extVar(config.calcClass, metcalcName),
+                            calcHandle=calcHandle, args=args)
+    _filterCalcSystematics(variProxy, calcHandle,
+                           enableSystematics=enableSystematics, default=isMC, name="MET")
 
 
 def splitVariation(variProxy, variation, regions, nomName="nom"):
     """
     Split a systematic variation between (kinematic) regions (to decorrelate the nuisance parameter)
 
     :param variProxy: jet variations proxy, e.g. ``tree._Jet``
@@ -1274,15 +1290,16 @@
                     regSel, origAtt, attN)
                 )) for attN, origAtt in origBrMap.items()}
             else:  # non-collection
                 regBrMap = {
                     attN: adaptArg(op.switch(regSel, origAtt, getattr(nomProxy, attN)))
                     for attN, origAtt in origBrMap.items()}
             variProxy.brMapMap[f"{variation}{regNm}{direction}"] = regBrMap
-    # adjust varMap and enabled variations for with-syst ops (as in initFromCalc and configure* above)
+    # adjust varMap and enabled variations for with-syst ops
+    # (as in CalcVariationsBase.addCalculator and configure* above)
     origVarNames = tuple(f"{variation}{direction}" for direction in ("up", "down"))
     newVarNames = tuple(f"{variation}{regNm}{direction}"
                         for regNm in regions.keys() for direction in ("up", "down"))
     for attN, opWithSyst in variProxy.brMapMap[getattr(variProxy, "withSystName", "nomWithSyst")].items():
         if opWithSyst._cache:
             raise RuntimeError(
                 "Expression has already been used, changing now would lead to undefined behaviour")
@@ -1366,25 +1383,28 @@
     :param puWeights: path of the JSON file with weights (binned in NumTrueInteractions)
         for cp3-llbb JSON, or tuple of JSON path and correction name (correctionlib JSON)
     :param numTrueInteractions: expression to get the number of true interactions
         (Poissonian expectation value for an event)
     :param systName: name of the associated systematic nuisance parameter
     :param sel: a selection in the current graph (only used to retrieve a pointer to the backend)
     """
+
     from . import treefunctions as op
     if isinstance(puWeights, tuple):
         from .scalefactors import get_correction
         expr = get_correction(
             puWeights[0], puWeights[1],
             params={"NumTrueInteractions": numTrueInteractions},
             systParam="weights", systNomName="nominal", systVariations=("up", "down"),
             systName=systName,  # will enable or disable systematic variations
             sel=sel, defineOnFirstUse=defineOnFirstUse
         )(None)
     else:
+        logger.warning("Using makePileupWeight() with 'llbb' JSONs is deprecated!"
+                       "Use correctionlib JSONs and get_correction() instead")
         paramVType = "Parameters::value_type::value_type"
         puArgs = op.construct(
             "Parameters", (op.initList(
                 f"std::initializer_list<{paramVType}>", paramVType,
                 (op.initList(paramVType, "float", (op.extVar(
                     "int", "BinningVariable::NumTrueInteractions"), numTrueInteractions)),)),))
         puWFun = op.define("ILeptonScaleFactor",
@@ -1465,15 +1485,15 @@
         (returned from :py:meth:`~bamboo.analysismodules.HistogramsModule.prepareTree`)
     :param uName: [deprecated, ignored]
         unique name for the correction calculator (sample name is a safe choice)
     """
     if uName != "":
         warnings.warn("Passing uName to configureRochesterCorrection "
                       "is not necessary anymore (and ignored), please update",
-                      DeprecationWarning)
+                      DeprecationWarning, stacklevel=1)
     from bamboo.treefunctions import _to, _tp
     aMu = variProxy.orig[0]
     args = [getattr(aMu, comp).op.arg for comp in (
         "pt", "eta", "phi", "mass", "charge", "nTrackerLayers")]
     if isMC:
         args += [aMu.genPart._idx.arg, variProxy._parent.GenPart[0].pt.op.arg]
         evt = variProxy._parent
@@ -1488,12 +1508,11 @@
     from .root import loadRochesterCorrectionCalculator, gbl
     loadRochesterCorrectionCalculator(backend=backend)
     if not os.path.exists(paramsFile):
         raise ValueError(f"File {paramsFile} not found")
     # define calculator and initialize
     roccorName = backend.symbol(
         f'RochesterCorrectionCalculator <<name>>{{"{paramsFile}"}};')
-    variProxy._initCalc(op.extVar("RochesterCorrectionCalculator", roccorName),
-                        calcHandle=getattr(gbl, roccorName),
-                        args=args)
-    variProxy._initFromCalc()
-    assert variProxy.calcProd
+    calcHandle = getattr(gbl, roccorName)
+    calcProd = op.extVar("RochesterCorrectionCalculator", roccorName)
+    variProxy.addCalculator(calcProd, calcHandle, args=args)
+    assert variProxy.calcWithProd[calcHandle]
```

### Comparing `bamboo-hep-1.0.1/bamboo/plots.py` & `bamboo-hep-1.1.0/bamboo/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,18 @@
     """ Variable-sized binning """
     __slots__ = ("__weakref__", "binEdges")
 
     def __init__(self, binEdges):
         """
         :param binEdges: iterable with the edges. There will be ``len(binEges)-1`` bins
         """
-        self.binEdges = list(binEdges)
+        binEdges = list(binEdges)
+        if any(binEdges[i + 1] <= binEdges[i] for i in range(len(binEdges) - 1)):
+            raise ValueError(f"Variable bin edges should be strictly increasing: {binEdges}")
+        self.binEdges = binEdges
 
     @property
     def N(self):
         return len(self.binEdges) - 1
 
     @property
     def minimum(self):
```

### Comparing `bamboo-hep-1.0.1/bamboo/batch.py` & `bamboo-hep-1.1.0/bamboo/batch.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/treeproxies.py` & `bamboo-hep-1.1.0/bamboo/treeproxies.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 to allow easy constructing the expression tree for the backend.
 As an example: 'myTreeProxy.event_id' will return an integer proxy,
 with as 'op' attribute a 'GetColumn(tree, "event_id")' operation.
 """
 
 import functools
 import re
+import logging
 
 from . import treeoperations as top
 from .treeoperations import SizeType, TupleBaseProxy, adaptArg
 
+logger = logging.getLogger(__name__)
+
 _boolTypes = {"bool", "Bool_t"}
 _integerTypes = {
     "Int_t", "UInt_t", "Char_t", "UChar_t", "ULong64_t", "int", "unsigned", "unsigned short",
     "char", "signed char", "unsigned char", "long", "Short_t", "size_t", "std::size_t",
     "unsigned short", "unsigned long"}
 _floatTypes = {"Float_t", "Double_t", "float", "double"}
 # TODO lists are probably not complete
@@ -351,17 +354,18 @@
                     else getattr(typ, name).__class__.__name__ == "CPPOverload")
                 or ((hasattr(gbl, "TemplateProxy") and isinstance(getattr(typ, name), gbl.TemplateProxy))
                     or (type(getattr(typ, name)).__name__ == "TemplateProxy"))):
             return ObjectMethodProxy(self, name)
         else:
             return top.GetDataMember(self, name, byPointer=self._isPointer).result
 
-    def __call__(self, *args):
+    def __call__(self, *args, **kwargs):
         if callable(self._typ):
-            return top.CallMemberMethod(self, "__call__", args, byPointer=self._isPointer).result
+            return top.CallMemberMethod(self, "__call__", args, byPointer=self._isPointer,
+                                        returnType=kwargs.get("returnType")).result
         else:
             raise RuntimeError(f"No operator() for type {self._typeName}")
 
     def __repr__(self):
         return f"ObjectProxy({self._parent!r})"
 
 
@@ -606,15 +610,15 @@
         return f"{self.__class__.__name__}({self._parent!r}, {self.brMap!r})"
 
 
 class AltCollectionVariations(TupleBaseProxy):
     """ Set of collections with alternative names for some branches """
     def __init__(self, parent, orig, brMapMap, altItemType=None):
         self.orig = orig
-        self.brMapMap = brMapMap
+        self.brMapMap = brMapMap  # variation name -> attribute name -> operation
         self.altItemType = altItemType if altItemType else orig.valueType
         super().__init__(parent)
 
     @property
     def _typeName(self):
         return None
 
@@ -656,45 +660,91 @@
         return self.orig.__len__()
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._parent!r}, {self.brMap!r}, {self.itemType!r})"
 
 
 class CalcVariationsBase:
-    """ extra base class for AltCollectionVariations or AltLeafGroupVariations with calculator """
+    """ extra base class for AltCollectionVariations or AltLeafGroupVariations with calculators """
     def __init__(self, withSystName=None):
-        self.calc = None
-        self.calcProd = None
-        self.withSystName = withSystName
+        self.calcWithProd = {}  # dict of calc handle -> product proxy)
+        self.withSystName = withSystName  # typically "nomWithSyst"
+
+    def addCalculator(self, calcProxy, calcHandle, args=None):
+        """Add a calculator for on-the-fly corrections or variations to this collection.
 
-    def _initCalc(self, calcProxy, calcHandle=None, args=None):
-        self.calc = calcHandle  # handle to the actual module object
+        :param calcProxy: the bamboo proxy wrapping the calculator
+                (e.g. returned by :py:method:`bamboo.treefunctions.extVar`)
+        :param calcHandle: the (pyROOT) handle to the calculator instance
+        :param args: the arguments to pass to the calculator's ``produce()`` method
+
+        :Example:
+
+        >>> calcName = backend.symbol("MyCalcClass <<name>>;")
+        >>> calcHandle = getattr(ROOT, calcName)
+        >>> calcProd = op.extVar("MyCalcClass", calcName)
+        >>> aJet = tree._Jet.orig[0]
+        >>> args = [getattr(aJet, attr).op.arg for attr in ["pt", "mass"]]
+        >>> tree._Jet.addCalculator(calcProd, calcHandle, args=args)
+        """
         import bamboo.treefunctions as op
         # define on-demand (does nothing if done explicitly) to limit worst-case behaviour
-        self.calcProd = op.defineOnFirstUse(calcProxy.produce(*args))
+        calcProd = op.defineOnFirstUse(calcProxy.produce(*args))
+        self.calcWithProd[calcHandle] = calcProd
 
-    def _available(self, att=""):
-        return list(str(iav) for iav in self.calc.available(att))
-
-    def _initFromCalc(self):
+        # create the ops for the individual variations, for this calculator
         for attN in self.brMapMap[self.withSystName].keys():
-            for i, nm in enumerate(self._available(attN)):
+            for iVar, nm in enumerate(calcHandle.available(attN)):
+                nm = str(nm)
                 if nm not in self.brMapMap:
                     self.brMapMap[nm] = dict()
+                elif attN in self.brMapMap[nm]:
+                    logger.warning(f"Variation {nm} for attribute {attN} "
+                                   f"of calculator {calcHandle} of collection "
+                                   f"{self.orig._prefix} was already present, replacing it.")
                 self.brMapMap[nm][attN] = adaptArg(
-                    getattr(self.calcProd, attN)(
-                        top.Parameter(SizeType, f"{i:d}ul").result))
+                    getattr(calcProd, attN)(
+                        top.Parameter(SizeType, f"{iVar:d}ul").result))
+
+        # Update the OpWithSyst wrapping all the variations inside the nominal,
+        # with the variations added by this calculator
         nonVarNames = (self.withSystName, "nominal", "raw")
         for attN in self.brMapMap[self.withSystName].keys():
+            # we should already have a SystAltOp at this point
+            theAltOp = self.brMapMap[self.withSystName][attN]
+            if theAltOp._cache:
+                raise RuntimeError(
+                    "Expression has already been used, changing now would lead to undefined behaviour")
+            assert(isinstance(theAltOp, top.SystAltOp))
+            existingVars = theAltOp.variations
+            varMap = theAltOp.varMap
+            varsToAdd = set((str(nm) for nm in calcHandle.available(attN))).difference(nonVarNames)
+            for var in varsToAdd:
+                varMap[var] = self.brMapMap[var][attN]
+            # recreate the op with the new variation map and new nominal wrapped op
             self.brMapMap[self.withSystName][attN] = top.SystAltOp(
                 self.brMapMap["nominal"][attN],
-                {var: brMap[attN] for var, brMap in self.brMapMap.items()
-                 if var not in nonVarNames and attN in brMap},
-                valid=[vr for vr in self.brMapMap.keys()
-                       if vr not in nonVarNames])
+                varMap,
+                valid=tuple(varsToAdd.union(existingVars)))
+
+    @property
+    def calcProds(self):
+        """Returns iterable with all calculator products"""
+        return self.calcWithProd.values()
+
+    def availableVariations(self, att="", calcHandle=None):
+        """Obtain list of available variations for a given attribute of the collection items.
+
+        :param att: the attribute, e.g. ``pt``
+        :param calcHandle: the handle of the calculator for which to get the variation list.
+                            If not specified, return variations for all calculators.
+        :returns: the list of variations, e.g. ``["jesTotalup", "jesTotalDown"]``
+        """
+        return list(str(iav) for calc, _ in self.calcWithProd.items()
+                    for iav in calc.available(att) if (not calcHandle or calc is calcHandle))
 
 
 class CalcLeafGroupVariations(AltLeafGroupVariations, CalcVariationsBase):
     """ Set of groups with alternative names for some branches, with calculator """
     def __init__(self, parent, orig, brMapMap, altProxyType, withSystName=None):
         super().__init__(parent, orig, brMapMap, altProxyType)
         CalcVariationsBase.__init__(self, withSystName=withSystName)
```

### Comparing `bamboo-hep-1.0.1/bamboo/treefunctions.py` & `bamboo-hep-1.1.0/bamboo/treefunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -974,41 +974,45 @@
             nd.changeVariation(varName)
         nd.variations = tuple()  # no hash collision because of different wrapped op
     return newExpr.result
 
 
 class MVAEvaluator:
     """ Small wrapper to make sure MVA evaluation is cached """
-    def __init__(self, evaluate, returnType=None, toArray=False):
+    def __init__(self, evaluate, returnType=None, toArray=False, toVector=True,
+                 useSlots=False):
         self.evaluate = evaluate
         self.returnType = returnType
         self.toArray = toArray
+        self.toVector = toVector
+        self.useSlots = useSlots
 
     def __call__(self, *inputs, **kwargs):
         evalArgs = inputs
         if all(isinstance(iin, _tp.NumberProxy) for iin in inputs):
             if self.toArray:
                 evalArgs = (array("float", *(static_cast("float", iin) for iin in inputs)),)
-            else:  # like before
+            elif self.toVector:
                 evalArgs = (initList("std::vector<float>", "float",
                                      (static_cast("float", iin) for iin in inputs)),)
-        else:
-            evalArgs = inputs
+        if self.useSlots:
+            evalArgs = (extVar("unsigned int", "rdfslot_"),) + evalArgs
         mvaOut = self.evaluate(*evalArgs, returnType=self.returnType)
         if kwargs.get("defineOnFirstUse", True):
             mvaOut = defineOnFirstUse(mvaOut)
         return mvaOut
 
 
 _mvaExtMap = {
     "TMVA": [".xml"],
     "Tensorflow": [".pb"],
     "Torch": [".pt"],
     "lwtnn": [".json"],
-    "ONNXRuntime": [".onnx"]
+    "ONNXRuntime": [".onnx"],
+    "SOFIE": [".hxx"]
 }
 
 
 def mvaEvaluator(fileName, mvaType=None, otherArgs=None, nameHint=None):
     """ Declare and initialize an MVA evaluator
 
     The C++ object is defined (with :py:meth:`bamboo.treefunctions.define`),
@@ -1030,14 +1034,18 @@
        more than one dimension, or if there are multiple output nodes.
     * .json (``mvaType='lwtnn'``) lwtnn json. The ``otherArgs`` keyword argument should be passed
       the lists of input and output nodes/values, as C++ initializer list strings, e.g.
       ``'{ { "node_0", "variable_0" }, { "node_0", "variable_1" } ... }'`` and
       ``'{ "out_0", "out_1" }'``.
     * .onnx (``mvaType='ONNXRuntime'``) ONNX file, evaluated with ONNX Runtime.
       The ``otherArgs`` keyword argument should the name of the output node (or a list of those)
+    * .hxx (``mvaType='SOFIE'``) ROOT SOFIE generated header file
+      The ``otherArgs`` keyword argument should be the path to the ``.dat`` weights file (if not specified,
+      it will taken by replacing the weight file extension from ``.hxx`` to ``.dat``).
+      Note: only available in ROOT>=6.26.04.
 
     :param fileName: file with MVA weights and structure
     :param mvaType: type of MVA, or library used to evaluate it (Tensorflow, Torch, or lwtnn).
         If absent, this is guessed from the fileName extension
     :param otherArgs: other arguments to construct the MVA evaluator
         (either as a string (safest), or as an iterable)
     :param nameHint: name hint, see :py:meth:`bamboo.treefunctions.define`
@@ -1078,23 +1086,42 @@
     if mvaType is None:
         import os.path
         _, ext = os.path.splitext(fileName)
         try:
             mvaType = next(k for k, v in _mvaExtMap.items() if ext in v)
         except StopIteration:
             raise ValueError(f"Unknown extension {ext!r}, please pass mvaType explicitly")
+
     methodName = "evaluate"  # default, used for wrappers
     isConst = True
     returnType = None
     toArray = False
+    toVector = True
+    useSlots = False  # pass rdfslot_ as first argument to evaluator
+
     if mvaType == "TMVA":
         cppType = "TMVA::Experimental::RReader"
         argStr = f'"{fileName}"'
         methodName = "Compute"
         isConst = False
+    elif mvaType == "SOFIE":
+        from .root import ROOT, getIMTPoolSize, loadHeader, loadBambooSOFIE
+        if not hasattr(ROOT.TMVA.Experimental, "SofieFunctor"):
+            raise RuntimeError(f"SOFIE is not available in this ROOT build")
+        import os
+        modelName = os.path.splitext(os.path.basename(fileName))[0]
+        loadHeader(fileName)
+        loadBambooSOFIE()
+        nSlots = getIMTPoolSize()
+        useSlots = True
+        weightsFile = otherArgs or os.path.join(os.path.dirname(fileName), modelName + ".dat")
+        cppType = f"bamboo::SofieEvaluator<TMVA_SOFIE_{modelName}::Session, float>"
+        argStr = f'{nSlots}, "{weightsFile}"'
+        isConst = False
+        returnType = "vector<float>"
     elif mvaType == "Tensorflow":
         from bamboo.root import loadTensorflowC
         loadTensorflowC()
         cppType = "bamboo::TensorflowCEvaluator"
         if isinstance(otherArgs, str):
             otherArgStr = otherArgs
         else:
@@ -1130,8 +1157,9 @@
         isConst = False
         returnType = "vector<float>"
         toArray = True
     else:
         raise ValueError(f"Unknown MVA type: {ext!r}")
     evaluator = define(cppType, '{const}auto <<name>> = {0}({1});'.format(
         cppType, argStr, const=("const " if isConst else "")), nameHint=nameHint)
-    return MVAEvaluator(getattr(evaluator, methodName), returnType=returnType, toArray=toArray)
+    return MVAEvaluator(getattr(evaluator, methodName),
+                        returnType=returnType, toArray=toArray, toVector=toVector, useSlots=useSlots)
```

### Comparing `bamboo-hep-1.0.1/bamboo/batch_htcondor.py` & `bamboo-hep-1.1.0/bamboo/batch_htcondor.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/bamboo/root.py` & `bamboo-hep-1.1.0/bamboo/root.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,18 @@
         for hdr in asList(headers):
             loadHeader(hdr)
     if bambooLib:
         for lib in asList(bambooLib):
             loadLibrary(f"lib{lib}")
 
 
+def getIMTPoolSize():
+    return ROOT.GetThreadPoolSize() if ROOT.IsImplicitMTEnabled() else 0
+
+
 @contextmanager
 def returnToDirectory():
     gpwd = gbl.gDirectory.GetPath()
     yield
     gbl.gDirectory.cd(gpwd)
 
 
@@ -219,14 +223,21 @@
     loader = backend.addDependency if backend else loadDependency
     loader(bambooLib="BambooONNXRuntime", headers="bambooonnxruntime.h",
            includePath=os.path.dirname(onnx_cxx_hdr),
            dynamicPath=dynPath, libraries="onnxruntime")
 
 
 @once
+def loadBambooSOFIE(backend=None):
+    loadBambooExtensions()
+    loader = backend.addDependency if backend else loadDependency
+    loader(headers="bamboosofie.h")
+
+
+@once
 def loadcorrectionlib(backend=None):
     import os.path
     loader = backend.addDependency if backend else loadDependency
     loader(headers="correction.h",
            includePath=pkg_resources.resource_filename("correctionlib", "include"),
            libraries=pkg_resources.resource_filename(
                "correctionlib", os.path.join("lib", "libcorrectionlib.so"))
```

### Comparing `bamboo-hep-1.0.1/CONTRIBUTING.md` & `bamboo-hep-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/analysis1.yml` & `bamboo-hep-1.1.0/examples/analysis1.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/adl_benchmarks.py` & `bamboo-hep-1.1.0/examples/adl_benchmarks.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,16 @@
                 dilepZ = op.rng_min_element_by(
                     dilep, fun=lambda ll: op.abs(op.invariant_mass(ll[0].p4, ll[1].p4) - 91.2))
                 for tlNm, tlCol in lepColl.items():
                     if tlCol == dlCol:
                         hasTriLep = hasDiLep.refine("hasTrilep{0}{0}{1}".format(dlNm, tlNm),
                                                     cut=(op.rng_len(tlCol) > 2))
                         residLep = op.select(
-                            tlCol, lambda l: op.AND(l.idx != dilepZ[0].idx, l.idx != dilepZ[1].idx))
+                            tlCol, lambda l, _dilepZ=dilepZ: op.AND(l.idx != _dilepZ[0].idx,
+                                                                    l.idx != _dilepZ[1].idx))
                         l3 = op.rng_max_element_by(residLep, lambda l: l.pt)
                     else:
                         hasTriLep = hasDiLep.refine("hasTriLep{0}{0}{1}".format(dlNm, tlNm),
                                                     cut=(op.rng_len(tlCol) > 0))
                         l3 = op.rng_max_element_by(tlCol, lambda l: l.pt)
                     mtPlot = Plot.make1D(
                         "Ex8_3lMT_{0}{0}{1}".format(dlNm, tlNm),
```

### Comparing `bamboo-hep-1.0.1/examples/nanozmumu.py` & `bamboo-hep-1.1.0/examples/nanozmumu.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,18 +235,21 @@
                 }, twoMuSel,
                 keepOriginal=[Skim.KeepRegex("PV_.*"), "nOtherPV", Skim.KeepRegex("OtherPV_.*")]))
 
         # evaluate jet and MET for all events passing twoMuSel
         # more optimization will be needed with systematics etc.
         metName = "METFixEE2017" if era == "2017" else "MET"
         if not self.args.postprocessed:
-            forceDefine(t._Jet.calcProd, twoMuSel)
-            forceDefine(getattr(t, f"_{metName}T1").calcProd, twoMuSel)
+            for calcProd in t._Jet.calcProds:
+                forceDefine(calcProd, twoMuSel)
+            for calcProd in getattr(t, f"_{metName}T1").calcProds:
+                forceDefine(calcProd, twoMuSel)
             if self.isMC(sample):
-                forceDefine(getattr(t, f"_{metName}T1Smear").calcProd, twoMuSel)
+                for calcProd in getattr(t, f"_{metName}T1Smear").calcProds:
+                    forceDefine(calcProd, twoMuSel)
         else:
             metName += "_"
 
         jets_noclean = op.select(t.Jet, lambda j: op.AND(j.jetId & 0x2, op.abs(j.eta) < 2.4, j.pt > 20.))
         jets = op.sort(
             op.select(jets_noclean, lambda j: op.AND(
                 op.NOT(op.rng_any(muons, lambda l: op.deltaR(l.p4, j.p4) < 0.4)),
```

### Comparing `bamboo-hep-1.0.1/examples/test_skim.yml` & `bamboo-hep-1.1.0/examples/test_skim.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt` & `bamboo-hep-1.1.0/examples/Cert_271036-284044_13TeV_23Sep2016ReReco_Collisions16_JSON.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/preselectskim.py` & `bamboo-hep-1.1.0/examples/preselectskim.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/analysis_zmm.yml` & `bamboo-hep-1.1.0/examples/analysis_zmm.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/cmsPhase2Sim_test.yml` & `bamboo-hep-1.1.0/examples/cmsPhase2Sim_test.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/analysis_eletnp.yml` & `bamboo-hep-1.1.0/examples/analysis_eletnp.yml`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/cmsPhase2Sim.py` & `bamboo-hep-1.1.0/examples/cmsPhase2Sim.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/eletnp.py` & `bamboo-hep-1.1.0/examples/eletnp.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/examples/df_nano.py` & `bamboo-hep-1.1.0/examples/df_nano.py`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/cpp/bamboohelpers.h` & `bamboo-hep-1.1.0/cpp/bamboohelpers.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/cpp/printprogress.h` & `bamboo-hep-1.1.0/cpp/printprogress.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/cpp/scalefactors.h` & `bamboo-hep-1.1.0/cpp/scalefactors.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/cpp/range.h` & `bamboo-hep-1.1.0/cpp/range.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/.gitlab-ci.yml` & `bamboo-hep-1.1.0/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -133,14 +133,48 @@
     - cd tests
     - pytest --junitxml=report_101_clang.xml
   artifacts:
     paths: [tests/report_101_clang.xml]
     reports:
       junit: tests/report_101_clang.xml
 
+build_102: # LCG_102, ROOT 6.26, newest version
+  tags: [cvmfs]
+  stage: build
+  before_script:
+    - yum install -y libgfortran make atlas
+    - source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
+    - python -m venv venv102
+    - source venv102/bin/activate
+  artifacts:
+    paths: [venv102]
+    expire_in: 30min
+  script:
+    # NOTE 'pre-commit -a' can be used (with all the checks) from LCG_102 on
+    # NOTE see https://sft.its.cern.ch/jira/browse/SPI-1978
+    - python -m pip install flake8 flake8-bugbear
+    - flake8 --exclude=venv102/
+    - python -m pip install scikit-build
+    - python -m pip install git+https://gitlab.cern.ch/cp3-cms/CMSJMECalculators.git
+    - python -m pip install . --no-build-isolation # with libtorch
+test_102:
+  tags: [cvmfs]
+  stage: test
+  needs: [build_102]
+  before_script:
+    - source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
+    - source venv102/bin/activate
+  script:
+    - cd tests
+    - pytest --junitxml=report_102.xml
+  artifacts:
+    paths: [tests/report_102.xml]
+    reports:
+      junit: tests/report_102.xml
+
 upload_pypi:
   stage: deploy
   only: [tags]
   before_script:
     - yum install -y python3
     - python3 -m venv release_venv
     - source release_venv/bin/activate
```

### Comparing `bamboo-hep-1.0.1/doc/advanced.rst` & `bamboo-hep-1.1.0/doc/advanced.rst`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,19 @@
 calls, since the default strategy is not to precalculate these because there are
 many more function calls that are not costly.
 A prime example of this is the calculation of modified jet collections with e.g.
 an alternative JEC aplied, which is done in a separate C++ module (see below),
 and is probably the slowest operation in most analysis tasks.
 The definition can be added explicitly under a selection by calling the
 :py:meth:`bamboo.analysisutils.forceDefine` method, e.g. with
-``forceDefine(t._Jet.calcProd, mySelection)``.
+
+.. code-block:: python
+
+    for calcProd in t._Jet.calcProds:
+        forceDefine(calcProd, mySelection)
 
 .. _ugbackends:
 
 Different backends
 ------------------
 
 Different approaches for converting plots and selections to an RDataFrame_
```

### Comparing `bamboo-hep-1.0.1/doc/conf.py` & `bamboo-hep-1.1.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.mathjax',
     'sphinx.ext.viewcode',
+    'sphinxcontrib.jquery',  # see https://github.com/readthedocs/sphinx_rtd_theme/issues/1452
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
```

### Comparing `bamboo-hep-1.0.1/doc/index.rst` & `bamboo-hep-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/doc/treefunctions.rst` & `bamboo-hep-1.1.0/doc/treefunctions.rst`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/doc/hacking.rst` & `bamboo-hep-1.1.0/doc/hacking.rst`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/doc/userguide.rst` & `bamboo-hep-1.1.0/doc/userguide.rst`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/doc/apiref.rst` & `bamboo-hep-1.1.0/doc/apiref.rst`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/doc/recipes.rst` & `bamboo-hep-1.1.0/doc/recipes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,26 @@
 related to automatic systematic uncertainties: the name of a category axis in
 the ``Correction``, the mapping between its categories and systematic variations
 in bamboo, and the name of the nominal category |---| more details and
 a complete example can be found in the reference documentation.
 Please note that this needs the correctionlib package to be installed, see
 :ref:`the installation guide<installbase>` for more details.
 
+Helper methods to configure and combine individual corrections for the purpose
+of applying b-tagging scale factor and uncertainties are provided, see
+:py:meth:`bamboo.scalefactors.makeBtagWeightMeth1a` and
+:py:meth:`bamboo.scalefactors.makeBtagWeightItFit`.
+
 CP3-llbb JSON format
 ''''''''''''''''''''
 
+.. warning:: The CP3-llbb json format and associated Bamboo functionalities
+   are soon going to be deprecated in favour of the central JSON format
+   and correctionlib (see above).
+
 The :py:mod:`bamboo.scalefactors` module provides support for constructing
 such callable objects from the JSON format used in the `CP3-llbb framework`_,
 see some examples
 `here <https://github.com/cp3-llbb/Framework/tree/CMSSW_8_0_6p/data/ScaleFactors>`_
 (these JSON files are produced from the txt or ROOT files provided by the POGs
 using simple python
 `scripts <https://github.com/cp3-llbb/Framework/tree/CMSSW_8_0_6p/scripts>`_).
@@ -131,28 +140,36 @@
                   weight=[ deepBLooseSF(bJets[0]), deepBLooseSF(bJets[1]) ])
 
 Note that the user is responsible for making sure that the weights are only applied to simulated events, and not to real data!
 
 CMS BTV CSV format
 ''''''''''''''''''
 
+.. warning:: The BTV CSV reader and associated Bamboo functionalities
+   are soon going to be deprecated in favour of the central JSON format
+   and correctionlib (see above).
+
 The :py:class:`bamboo.scalefactors.BtagSF` class wraps the
 ``BTagCalibrationReader`` provided by the BTV POG to read the custom CSV
 format for b-tagging scalefactors (more details usage instructions can be
 found in the reference documentation).
 Please note that this will only read the scalefactors, which for most
 `methods for applying b-tagging scalefactors <https://twiki.cern.ch/twiki/bin/viewauth/CMS/BTagSFMethods>`_
 need to be combined with efficiency and mistag probability maps measured
 in simulation in the analysis phase space.
 
 .. _recipepureweighting:
 
 Pileup reweighting
 ------------------
 
+.. warning:: The pileup weights maker and associated Bamboo functionalities
+   are soon going to be deprecated in favour of the central JSON format
+   and correctionlib (see above).
+
 Pileup reweighting to make the pileup distribution in simulation match the one
 in data is very similar to applying a scalefactor, except that the efficiency
 correction is for the whole event or per-object |---| so the same code can be
 used.
 The ``makePUReWeightJSON`` script included in bamboo can be used to make
 a JSON file with weights out of a data pileup profile obtained by running
 ``pileupcalc.py``
@@ -552,15 +569,15 @@
 Evaluate an MVA classifier
 --------------------------
 
 Several external libraries can be used to evaluate the response of MVA
 classifiers inside expressions.
 For convenience, a uniform interface is defined that uses a vector of floats
 as input and output, with implementations available for PyTorch_,
-Tensorflow_, lwtnn_, TMVA_, and `ONNX Runtime`_.
+Tensorflow_, lwtnn_, TMVA_, `ONNX Runtime`_, and `SOFIE`_.
 That works as follows (see the documentation for the
 :py:meth:`bamboo.treefunctions.mvaEvaluator` method for a detailed description,
 additional options may be needed, depending on the type):
 
 .. code-block:: python
 
     mu = tree.Muon[0]
@@ -611,14 +628,25 @@
 For Keras_ models Tensorflow_ is the most natural fit. Please note that the
 frozen graph is needed, see e.g.
 `keras_to_tensorflow <https://github.com/amir-abdi/keras_to_tensorflow>`_,
 `this detailed explanation <https://medium.com/@sebastingarcaacosta/how-to-export-a-tensorflow-2-x-keras-model-to-a-frozen-and-optimized-graph-39740846d9eb>`_,
 and `this script <https://github.com/FlorianBury/HHbbWWAnalysis/blob/master/MachineLearning/HHMachineLearning/KerasToTensorflowModel.py>`_
 for an example of how to do so.
 
+SOFIE_ allows one to evaluate models in ONNX_, `PyTorch`_ or Keras_ format, 
+provided they have been first converted into a header and weight files
+using the helpers available in ROOT 
+(see the ROOT documentation and `tutorials <https://root.cern.ch/doc/master/dir_afb41fc0ce910d0ed999b271277cf431.html>`_ for how to convert models).
+While a limited set of models are supported (only a few types of layers 
+are implemented in SOFIE), if the conversion is possible, model evaluation in 
+SOFIE_ has the potential to be significantly faster than using the ONNX_, 
+Tensorflow_ or `PyTorch`_ APIs.
+Note that SOFIE_ is only supported in ROOT >= 6.26.04 but is not enabled by default,
+so you'll need to make sure that your ROOT build has SOFIE_ enabled.
+
 Testing the evaluation outside RDataFrame
 '''''''''''''''''''''''''''''''''''''''''
 
 MVA inference with all the libraries described above is done by creating
 an instance of an evaluator class, which provides a similar
 RDataFrame-friendly interface: the filename of te saved model and additional
 options are passed to the constructor, and an evaluate method that takes the
@@ -1044,14 +1072,16 @@
 
 .. _TMVA: https://root.cern/manual/tmva/
 
 .. _ONNX: https://onnx.ai
 
 .. _ONNX Runtime: https://www.onnxruntime.ai
 
+.. _SOFIE: https://root.cern/doc/v626/release-notes.html#sofie-code-generation-for-fast-inference-of-deep-learning-models
+
 .. _Keras: https://keras.io
 
 .. _the lwtnn wiki: https://github.com/lwtnn/lwtnn/wiki/Keras-Converter
 
 .. _TorchScript: https://pytorch.org/docs/stable/jit.html
 
 .. _keras2onnx: https://github.com/onnx/keras-onnx
```

### Comparing `bamboo-hep-1.0.1/doc/install.rst` & `bamboo-hep-1.1.0/doc/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 ----------------------------
 
 Bamboo_ only depends on python3 (with pip/setuptools to install PyYAML and
 numpy if needed) and a recent version of ROOT (6.20/00 is the minimum
 supported version, as it introduces some compatibility features for the
 `new PyROOT`_ in 6.22/00).
 
-On ingrid and lxplus (or any machine with cvmfs), an easy way to get such
+On user interface machines (lxplus, ingrid, or any machine with cvmfs), 
+an easy way to get such
 a recent version of ROOT is through a CMSSW release that depends on it,
 or from the `SPI LCG distribution`_, e.g.
 
 .. code-block:: sh
 
-   source /cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc10-opt/setup.sh
+   source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
    python -m venv bamboovenv
    source bamboovenv/bin/activate
 
 (the second command creates a `virtual environment`_
 to install python packages in, after installation it is sufficient to run two
 other commands, to pick up the correct base system and then the installed
 packages).
@@ -52,41 +53,42 @@
 Currently, they include:
 
 - the dasgoclient executable (and a valid grid proxy) for retrieving the list
   of files in samples specified with ``db: das:/X/Y/Z``. Due to some
   interference with the setup script above, the best is to run the cms
   environment scripts first, and also run ``voms-proxy-init`` then (this can
   alternatively also be done from a different shell on the same machine)
-- the SAMADhi_ python library, to retrieve the list of files in samples
-  specified with ``db: SAMADhi:<ID-or-name>`` (not yet integrated)
-- the slurm command-line tools, and CP3SlurmUtils_, which can be loaded with
-  ``module load slurm/slurm_utils`` on the ingrid ui machines
-- the ``makePUReWeightJSON`` script can make a plot of the PU distributions
-  and weights if the ``--makePlot`` option is given, but it needs matplotlib_
-  for that
+- the slurm command-line tools, and CP3SlurmUtils_, which can be installed using `pip`
+  (or loaded with ``module load slurm/slurm_utils`` on the UCLouvain ingrid ui machines)
 - machine learning libraries (libtorch_, Tensorflow-C_, lwtnn_): see
   :ref:`this section<installmachinelearning>` for more information
 - writing out tables in LaTeX format from cutflow reports relies needs
   pyplotit_ (see below)
 
 .. _installbase:
 
 Installation
 ------------
 
 Bamboo_ can (and should, in most cases) be installed in a
-`virtual environment`_ or conda environment (see above) with pip,
-minimally either one of
+`virtual environment`_ or conda environment (see above) with pip:
+
+.. code-block:: sh
+
+    pip install bamboo-hep
+
+Since Bamboo_ is still in heavy development, you may want to fetch the latest
+(unreleased) version using one of:
 
 .. code-block:: sh
 
    pip install git+https://gitlab.cern.ch/cp3-cms/bamboo.git
    pip install git+ssh://git@gitlab.cern.ch:7999/cp3-cms/bamboo.git
 
-but in the current development stage it may be useful to install from
+It may even be useful to install from
 a local clone, such that you can use it to test and propose changes, using
 
 .. code-block:: sh
 
    git clone -o upstream https://gitlab.cern.ch/cp3-cms/bamboo.git /path/to/your/bambooclone
    pip install /path/to/your/bambooclone ## e.g. ./bamboo (not bamboo - a package with that name exists)
 
@@ -131,21 +133,19 @@
 which is used in many analyses, the plotIt_ tool is used.
 It can be installed with cmake, e.g.
 
 .. code-block:: sh
 
    git clone -o upstream https://github.com/cp3-llbb/plotIt.git /path/to/your/plotitclone
    mkdir build-plotit
-   cd build-plotit
-   cmake -DCMAKE_INSTALL_PREFIX=$VIRTUAL_ENV /path/to/your/plotitclone
-   make -j2 install
-   cd -
+   cmake -DCMAKE_INSTALL_PREFIX=$VIRTUAL_ENV -S /path/to/your/plotitclone -B build-plotit
+   cmake --build build-plotit -t install -j 4
 
-where ``-DCMAKE_INSTALL_PREFIX=$VIRTUAL_ENV`` ensures that ``make install``
-will put the ``plotIt`` executable directly in the ``bin`` directory of the
+where ``-DCMAKE_INSTALL_PREFIX=$VIRTUAL_ENV`` ensures that the ``plotIt`` 
+executable will be installed directly in the ``bin`` directory of the
 virtualenv (if not using a virtualenv, its path can be passed to ``bambooRun``
 with the ``--plotIt`` command-line option).
 
 plotIt_ is very efficient at what it does, but not so easy to adapt to producing
 efficiently plots, overlays of differently defined distributions etc.
 Therefore a python implementation of its main functionality was started in the
 pyplotit_ package, which can be installed with
@@ -201,15 +201,15 @@
 #############
 
 .. code-block:: sh
 
    mkdir bamboodev
    cd bamboodev
    # make a virtualenv
-   source /cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc10-opt/setup.sh
+   source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
    python -m venv bamboovenv
    source bamboovenv/bin/activate
    # clone and install bamboo
    git clone -o upstream https://gitlab.cern.ch/cp3-cms/bamboo.git
    pip install ./bamboo
    # clone and install plotIt
    git clone -o upstream https://github.com/cp3-llbb/plotIt.git
@@ -223,15 +223,15 @@
 #################
 
 Once bamboo_ and plotIt have been installed as above, only the following two
 commands are needed to set up the environment in a new shell:
 
 .. code-block:: sh
 
-   source /cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc10-opt/setup.sh
+   source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
    source bamboodev/bamboovenv/bin/activate
 
 Update bamboo
 #############
 
 Assuming the environment is set up as above; this can also be used to test a
 pull request or local modifications to the bamboo_ source code
@@ -268,15 +268,15 @@
 This allows to have e.g. one stable version used for analysis, and another one
 to test experimental changes, or check a new LCG release, without touching a
 known working version.
 
 .. code-block:: sh
 
    cd bamboodev
-   source /cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc10-opt/setup.sh
+   source /cvmfs/sft.cern.ch/lcg/views/LCG_102/x86_64-centos7-gcc11-opt/setup.sh
    python -m venv bamboovenv_X
    source bamboovenv_X/bin/activate
    pip install ./bamboo
    # install plotIt (as in "Update plotIt" above)
    mkdir build-plotit
    cd build-plotit
    cmake -DCMAKE_INSTALL_PREFIX=$VIRTUAL_ENV ../plotIt
```

### Comparing `bamboo-hep-1.0.1/setup.cfg` & `bamboo-hep-1.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -5,59 +5,59 @@
 long_description_content_type = text/markdown
 url = https://gitlab.cern.ch/cp3-cms/bamboo
 author = Pieter David
 author_email = pieter.david@cern.ch
 license = GPL-3.0-or-later
 license_file = LICENSE
 license_files = LICENSE
-classifiers =
-    Development Status :: 4 - Beta
-    Intended Audience :: Developers
-    Intended Audience :: Science/Research
-    License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-    Operating System :: OS Independent
-    Programming Language :: Python :: 3
-    Programming Language :: Python :: 3 :: Only
-    Programming Language :: Python :: 3.6
-    Programming Language :: Python :: 3.7
-    Programming Language :: Python :: 3.8
-    Programming Language :: Python :: 3.9
-    Programming Language :: Python :: 3.10
-    Topic :: Scientific/Engineering :: Information Analysis
-    Topic :: Scientific/Engineering :: Physics
-    Topic :: Software Development :: Libraries :: Python Modules
+classifiers = 
+	Development Status :: 4 - Beta
+	Intended Audience :: Developers
+	Intended Audience :: Science/Research
+	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+	Operating System :: OS Independent
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Topic :: Scientific/Engineering :: Information Analysis
+	Topic :: Scientific/Engineering :: Physics
+	Topic :: Software Development :: Libraries :: Python Modules
 keywords = ROOT, RDataFrame
 
 [options]
-install_requires =
-    PyYAML
-    numpy
-    requests
+install_requires = 
+	PyYAML
+	numpy
+	requests
 python_requires = >=3.6
-setup_requires =
-    pytest-runner
-tests_require =
-    pytest
+setup_requires = 
+	pytest-runner
+tests_require = 
+	pytest
 
 [options.entry_points]
-console_scripts =
-    bambooRun = bamboo.scripts.bambooRun:main
-    makePUReWeightJSON = bamboo.scripts.makePUReWeightJSON:main
-    bambooHTCondorResubmit = bamboo.batch_htcondor:resubmit_cli
+console_scripts = 
+	bambooRun = bamboo.scripts.bambooRun:main
+	makePUReWeightJSON = bamboo.scripts.makePUReWeightJSON:main
+	bambooHTCondorResubmit = bamboo.batch_htcondor:resubmit_cli
 
 [options.extras_require]
-cms =
-    correctionlib
-docs =
-    sphinx
-    sphinx-rtd-theme
-interactive =
-    IPython
-torch =
-    torch>=1.2.0
+cms = 
+	correctionlib
+docs = 
+	sphinx
+	sphinx-rtd-theme
+interactive = 
+	IPython
+torch = 
+	torch>=1.2.0
 
 [options.package_data]
 bamboo = data/*
 
 [bdist_wheel]
 universal = 0
 
@@ -68,7 +68,12 @@
 source-dir = doc
 build-dir = doc/build
 
 [flake8]
 max-line-length = 100
 select = E,F,W,B,B950
 ignore = E501,W503
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

### Comparing `bamboo-hep-1.0.1/ext/install_lwtnn.sh` & `bamboo-hep-1.1.0/ext/install_lwtnn.sh`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/bambootorch.h` & `bamboo-hep-1.1.0/ext/include/bambootorch.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/bamboolwtnn.h` & `bamboo-hep-1.1.0/ext/include/bamboolwtnn.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/Histogram.h` & `bamboo-hep-1.1.0/ext/include/Histogram.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/LumiMask.h` & `bamboo-hep-1.1.0/ext/include/LumiMask.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/bambooonnxruntime.h` & `bamboo-hep-1.1.0/ext/include/bambooonnxruntime.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/kinematicvariations.h` & `bamboo-hep-1.1.0/ext/include/kinematicvariations.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/BTagCalibrationStandalone.h` & `bamboo-hep-1.1.0/ext/include/BTagCalibrationStandalone.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/RochesterCorrectionCalculator.h` & `bamboo-hep-1.1.0/ext/include/RochesterCorrectionCalculator.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/RoccoR.h` & `bamboo-hep-1.1.0/ext/include/RoccoR.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/BinnedValues.h` & `bamboo-hep-1.1.0/ext/include/BinnedValues.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/include/bambootensorflowc.h` & `bamboo-hep-1.1.0/ext/include/bambootensorflowc.h`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/CMakeLists.txt` & `bamboo-hep-1.1.0/ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/cmake/modules/FindONNXRuntime.cmake` & `bamboo-hep-1.1.0/ext/cmake/modules/FindONNXRuntime.cmake`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/cmake/modules/FindTensorflowC.cmake` & `bamboo-hep-1.1.0/ext/cmake/modules/FindTensorflowC.cmake`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/install_tensorflow-c.sh` & `bamboo-hep-1.1.0/ext/install_tensorflow-c.sh`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/BinnedValues.cc` & `bamboo-hep-1.1.0/ext/src/BinnedValues.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/bamboolwtnn.cc` & `bamboo-hep-1.1.0/ext/src/bamboolwtnn.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/LumiMask.cc` & `bamboo-hep-1.1.0/ext/src/LumiMask.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/BTagCalibrationStandalone.cpp` & `bamboo-hep-1.1.0/ext/src/BTagCalibrationStandalone.cpp`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/bambootorch.cc` & `bamboo-hep-1.1.0/ext/src/bambootorch.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/BinnedValuesJSONParser.cc` & `bamboo-hep-1.1.0/ext/src/BinnedValuesJSONParser.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/bambooonnxruntime.cc` & `bamboo-hep-1.1.0/ext/src/bambooonnxruntime.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/RoccoR.cc` & `bamboo-hep-1.1.0/ext/src/RoccoR.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/bambootensorflowc.cc` & `bamboo-hep-1.1.0/ext/src/bambootensorflowc.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/tester_fatjets.cc` & `bamboo-hep-1.1.0/ext/src/tester_fatjets.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/ext/src/RochesterCorrectionCalculator.cc` & `bamboo-hep-1.1.0/ext/src/RochesterCorrectionCalculator.cc`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/COPYING` & `bamboo-hep-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/README.md` & `bamboo-hep-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bamboo-hep-1.0.1/publish_release_to_zenodo.py` & `bamboo-hep-1.1.0/publish_release_to_zenodo.py`

 * *Files identical despite different names*

