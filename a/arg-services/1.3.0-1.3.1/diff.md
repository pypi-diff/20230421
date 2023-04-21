# Comparing `tmp/arg_services-1.3.0.tar.gz` & `tmp/arg_services-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.3.0.tar", max compression
+gzip compressed data, was "arg_services-1.3.1.tar", max compression
```

## Comparing `arg_services-1.3.0.tar` & `arg_services-1.3.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1067 2023-04-09 09:56:51.694542 arg_services-1.3.0/LICENSE
--rw-r--r--   0        0        0      657 2023-04-09 09:56:51.694542 arg_services-1.3.0/README.md
--rw-r--r--   0        0        0      671 2023-04-09 09:57:28.058345 arg_services-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7288 2023-04-09 09:57:27.274349 arg_services-1.3.0/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     6996 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12124 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3416 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2519 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     8286 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    15179 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     4628 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0     1252 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.258350 arg_services-1.3.0/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.258350 arg_services-1.3.0/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    11861 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      151 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.262349 arg_services-1.3.0/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     5028 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1237 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     6102 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     8973 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     4721 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1298 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4150 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3812 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      856 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2930 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0      821 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.266349 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3371 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0      916 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4502 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3857 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      960 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     9005 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27846 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.270349 arg_services-1.3.0/src/google/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 09:57:27.274349 arg_services-1.3.0/src/google/api/__init__.py
--rw-r--r--   0        0        0     1813 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2631 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18295 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-04-09 09:57:27.250350 arg_services-1.3.0/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 09:06:53.310260 arg_services-1.3.1/LICENSE
+-rw-r--r--   0        0        0      657 2023-04-21 09:06:53.310260 arg_services-1.3.1/README.md
+-rw-r--r--   0        0        0      671 2023-04-21 09:07:30.726636 arg_services-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7288 2023-04-21 09:07:29.786626 arg_services-1.3.1/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     7099 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12424 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3416 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2519 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8286 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     1252 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.766626 arg_services-1.3.1/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    11861 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      151 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5028 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1237 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6102 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     8973 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     4721 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1298 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4150 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3812 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      856 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2930 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0      821 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.778626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3371 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0      916 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4502 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3857 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      960 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.778626 arg_services-1.3.1/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9005 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1813 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2631 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.1/PKG-INFO
```

### Comparing `arg_services-1.3.0/LICENSE` & `arg_services-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/README.md` & `arg_services-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/pyproject.toml` & `arg_services-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.3.0"
+version = "1.3.1"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
```

### Comparing `arg_services-1.3.0/src/arg_services/__init__.py` & `arg_services-1.3.1/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,47 +14,47 @@
 from arg_services.cbr.v1beta import model_pb2 as arg__services_dot_cbr_dot_v1beta_dot_model__pb2
 from arg_services.cbr.v1beta import retrieval_pb2 as arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2
 from arg_services.nlp.v1 import nlp_pb2 as arg__services_dot_nlp_dot_v1_dot_nlp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/cbr/v1beta/adaptation.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\'arg_services/cbr/v1beta/retrieval.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xae\x03\n\x0c\x41\x64\x61ptRequest\x12\x46\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x30.arg_services.cbr.v1beta.AdaptRequest.CasesEntryR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12@\n\tdirection\x18\x06 \x01(\x0e\x32\".arg_services.cbr.v1beta.DirectionR\tdirection\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x65\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32+.arg_services.cbr.v1beta.AdaptedCaseRequestR\x05value:\x02\x38\x01\"\xf1\x01\n\rAdaptResponse\x12G\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x31.arg_services.cbr.v1beta.AdaptResponse.CasesEntryR\x05\x63\x61ses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x66\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x42\n\x05value\x18\x02 \x01(\x0b\x32,.arg_services.cbr.v1beta.AdaptedCaseResponseR\x05value:\x02\x38\x01\"\xdc\x01\n\x12\x41\x64\x61ptedCaseRequest\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12\x33\n\x05rules\x18\x02 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x05rules\x12H\n\x07mapping\x18\x03 \x01(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingH\x00R\x07mapping\x88\x01\x01\x42\n\n\x08_mapping\"\xd2\x03\n\x13\x41\x64\x61ptedCaseResponse\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12O\n\x12\x65xtracted_concepts\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x65xtractedConcepts\x12O\n\x12\x64iscarded_concepts\x18\x03 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x64iscardedConcepts\x12\x42\n\rapplied_rules\x18\x04 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0c\x61ppliedRules\x12\x46\n\x0f\x64iscarded_rules\x18\x05 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0e\x64iscardedRules\x12P\n\x0frule_candidates\x18\x06 \x03(\x0b\x32\'.arg_services.cbr.v1beta.RuleCandidatesR\x0eruleCandidates\"z\n\x04Rule\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target\"e\n\x07\x43oncept\x12\x14\n\x05lemma\x18\x01 \x01(\tR\x05lemma\x12.\n\x03pos\x18\x02 \x01(\x0e\x32\x1c.arg_services.cbr.v1beta.PosR\x03pos\x12\x14\n\x05score\x18\x03 \x01(\x01R\x05score\"\x84\x01\n\x0eRuleCandidates\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target*z\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x44IRECTION_GENERALIZATION\x10\x01\x12\x1c\n\x18\x44IRECTION_SPECIALIZATION\x10\x02\x12\x16\n\x12\x44IRECTION_COMBINED\x10\x03*Y\n\x03Pos\x12\x13\n\x0fPOS_UNSPECIFIED\x10\x00\x12\x0c\n\x08POS_NOUN\x10\x01\x12\x0c\n\x08POS_VERB\x10\x02\x12\x11\n\rPOS_ADJECTIVE\x10\x03\x12\x0e\n\nPOS_ADVERB\x10\x04\x32\x89\x01\n\x11\x41\x64\x61ptationService\x12t\n\x05\x41\x64\x61pt\x12%.arg_services.cbr.v1beta.AdaptRequest\x1a&.arg_services.cbr.v1beta.AdaptResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/cbr/v1beta/adaptB\xa8\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0f\x41\x64\x61ptationProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/cbr/v1beta/adaptation.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\'arg_services/cbr/v1beta/retrieval.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xae\x03\n\x0c\x41\x64\x61ptRequest\x12\x46\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x30.arg_services.cbr.v1beta.AdaptRequest.CasesEntryR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12@\n\tdirection\x18\x06 \x01(\x0e\x32\".arg_services.cbr.v1beta.DirectionR\tdirection\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x65\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32+.arg_services.cbr.v1beta.AdaptedCaseRequestR\x05value:\x02\x38\x01\"\xf1\x01\n\rAdaptResponse\x12G\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x31.arg_services.cbr.v1beta.AdaptResponse.CasesEntryR\x05\x63\x61ses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x66\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x42\n\x05value\x18\x02 \x01(\x0b\x32,.arg_services.cbr.v1beta.AdaptedCaseResponseR\x05value:\x02\x38\x01\"\xdc\x01\n\x12\x41\x64\x61ptedCaseRequest\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12\x33\n\x05rules\x18\x02 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x05rules\x12H\n\x07mapping\x18\x03 \x01(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingH\x00R\x07mapping\x88\x01\x01\x42\n\n\x08_mapping\"\x9a\x04\n\x13\x41\x64\x61ptedCaseResponse\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12O\n\x12\x65xtracted_concepts\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x65xtractedConcepts\x12O\n\x12\x64iscarded_concepts\x18\x03 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x64iscardedConcepts\x12\x42\n\rapplied_rules\x18\x04 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0c\x61ppliedRules\x12\x46\n\x0f\x64iscarded_rules\x18\x05 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0e\x64iscardedRules\x12\x46\n\x0fgenerated_rules\x18\x07 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0egeneratedRules\x12P\n\x0frule_candidates\x18\x06 \x03(\x0b\x32\'.arg_services.cbr.v1beta.RuleCandidatesR\x0eruleCandidates\"z\n\x04Rule\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target\"e\n\x07\x43oncept\x12\x14\n\x05lemma\x18\x01 \x01(\tR\x05lemma\x12.\n\x03pos\x18\x02 \x01(\x0e\x32\x1c.arg_services.cbr.v1beta.PosR\x03pos\x12\x14\n\x05score\x18\x03 \x01(\x01R\x05score\"\x84\x01\n\x0eRuleCandidates\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target*z\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x44IRECTION_GENERALIZATION\x10\x01\x12\x1c\n\x18\x44IRECTION_SPECIALIZATION\x10\x02\x12\x16\n\x12\x44IRECTION_COMBINED\x10\x03*Y\n\x03Pos\x12\x13\n\x0fPOS_UNSPECIFIED\x10\x00\x12\x0c\n\x08POS_NOUN\x10\x01\x12\x0c\n\x08POS_VERB\x10\x02\x12\x11\n\rPOS_ADJECTIVE\x10\x03\x12\x0e\n\nPOS_ADVERB\x10\x04\x32\x89\x01\n\x11\x41\x64\x61ptationService\x12t\n\x05\x41\x64\x61pt\x12%.arg_services.cbr.v1beta.AdaptRequest\x1a&.arg_services.cbr.v1beta.AdaptResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/cbr/v1beta/adaptB\xa8\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0f\x41\x64\x61ptationProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.adaptation_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.arg_services.cbr.v1betaB\017AdaptationProtoP\001\242\002\003ACX\252\002\026ArgServices.Cbr.V1beta\312\002\026ArgServices\\Cbr\\V1beta\342\002\"ArgServices\\Cbr\\V1beta\\GPBMetadata\352\002\030ArgServices::Cbr::V1beta'
   _ADAPTREQUEST_CASESENTRY._options = None
   _ADAPTREQUEST_CASESENTRY._serialized_options = b'8\001'
   _ADAPTRESPONSE_CASESENTRY._options = None
   _ADAPTRESPONSE_CASESENTRY._serialized_options = b'8\001'
   _ADAPTATIONSERVICE.methods_by_name['Adapt']._options = None
   _ADAPTATIONSERVICE.methods_by_name['Adapt']._serialized_options = b'\202\323\344\223\002\026:\001*\"\021/cbr/v1beta/adapt'
-  _globals['_DIRECTION']._serialized_start=1969
-  _globals['_DIRECTION']._serialized_end=2091
-  _globals['_POS']._serialized_start=2093
-  _globals['_POS']._serialized_end=2182
+  _globals['_DIRECTION']._serialized_start=2041
+  _globals['_DIRECTION']._serialized_end=2163
+  _globals['_POS']._serialized_start=2165
+  _globals['_POS']._serialized_end=2254
   _globals['_ADAPTREQUEST']._serialized_start=239
   _globals['_ADAPTREQUEST']._serialized_end=669
   _globals['_ADAPTREQUEST_CASESENTRY']._serialized_start=568
   _globals['_ADAPTREQUEST_CASESENTRY']._serialized_end=669
   _globals['_ADAPTRESPONSE']._serialized_start=672
   _globals['_ADAPTRESPONSE']._serialized_end=913
   _globals['_ADAPTRESPONSE_CASESENTRY']._serialized_start=811
   _globals['_ADAPTRESPONSE_CASESENTRY']._serialized_end=913
   _globals['_ADAPTEDCASEREQUEST']._serialized_start=916
   _globals['_ADAPTEDCASEREQUEST']._serialized_end=1136
   _globals['_ADAPTEDCASERESPONSE']._serialized_start=1139
-  _globals['_ADAPTEDCASERESPONSE']._serialized_end=1605
-  _globals['_RULE']._serialized_start=1607
-  _globals['_RULE']._serialized_end=1729
-  _globals['_CONCEPT']._serialized_start=1731
-  _globals['_CONCEPT']._serialized_end=1832
-  _globals['_RULECANDIDATES']._serialized_start=1835
-  _globals['_RULECANDIDATES']._serialized_end=1967
-  _globals['_ADAPTATIONSERVICE']._serialized_start=2185
-  _globals['_ADAPTATIONSERVICE']._serialized_end=2322
+  _globals['_ADAPTEDCASERESPONSE']._serialized_end=1677
+  _globals['_RULE']._serialized_start=1679
+  _globals['_RULE']._serialized_end=1801
+  _globals['_CONCEPT']._serialized_start=1803
+  _globals['_CONCEPT']._serialized_end=1904
+  _globals['_RULECANDIDATES']._serialized_start=1907
+  _globals['_RULECANDIDATES']._serialized_end=2039
+  _globals['_ADAPTATIONSERVICE']._serialized_start=2257
+  _globals['_ADAPTATIONSERVICE']._serialized_end=2394
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -183,43 +183,47 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CASE_FIELD_NUMBER: builtins.int
     EXTRACTED_CONCEPTS_FIELD_NUMBER: builtins.int
     DISCARDED_CONCEPTS_FIELD_NUMBER: builtins.int
     APPLIED_RULES_FIELD_NUMBER: builtins.int
     DISCARDED_RULES_FIELD_NUMBER: builtins.int
+    GENERATED_RULES_FIELD_NUMBER: builtins.int
     RULE_CANDIDATES_FIELD_NUMBER: builtins.int
     @property
     def case(self) -> arg_services.cbr.v1beta.model_pb2.AnnotatedGraph: ...
     @property
     def extracted_concepts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Concept]:
         """These are optional and used for further evaluation only"""
     @property
     def discarded_concepts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Concept]: ...
     @property
     def applied_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Rule]: ...
     @property
     def discarded_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Rule]: ...
     @property
+    def generated_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Rule]: ...
+    @property
     def rule_candidates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RuleCandidates]:
         """repeated Path extracted_paths = 6;
         repeated Path adapted_paths = 7;
         """
     def __init__(
         self,
         *,
         case: arg_services.cbr.v1beta.model_pb2.AnnotatedGraph | None = ...,
         extracted_concepts: collections.abc.Iterable[global___Concept] | None = ...,
         discarded_concepts: collections.abc.Iterable[global___Concept] | None = ...,
         applied_rules: collections.abc.Iterable[global___Rule] | None = ...,
         discarded_rules: collections.abc.Iterable[global___Rule] | None = ...,
+        generated_rules: collections.abc.Iterable[global___Rule] | None = ...,
         rule_candidates: collections.abc.Iterable[global___RuleCandidates] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["case", b"case"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["applied_rules", b"applied_rules", "case", b"case", "discarded_concepts", b"discarded_concepts", "discarded_rules", b"discarded_rules", "extracted_concepts", b"extracted_concepts", "rule_candidates", b"rule_candidates"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["applied_rules", b"applied_rules", "case", b"case", "discarded_concepts", b"discarded_concepts", "discarded_rules", b"discarded_rules", "extracted_concepts", b"extracted_concepts", "generated_rules", b"generated_rules", "rule_candidates", b"rule_candidates"]) -> None: ...
 
 global___AdaptedCaseResponse = AdaptedCaseResponse
 
 @typing_extensions.final
 class Rule(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/annotations_pb2.py` & `arg_services-1.3.1/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/annotations_pb2.pyi` & `arg_services-1.3.1/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.3.1/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/http_pb2.py` & `arg_services-1.3.1/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/http_pb2.pyi` & `arg_services-1.3.1/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.3.1/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.0/PKG-INFO` & `arg_services-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.3.0
+Version: 1.3.1
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

