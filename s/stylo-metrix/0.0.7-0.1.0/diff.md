# Comparing `tmp/stylo_metrix-0.0.7.tar.gz` & `tmp/stylo_metrix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylo_metrix-0.0.7.tar", last modified: Fri Sep  2 09:01:06 2022, max compression
+gzip compressed data, was "stylo_metrix-0.1.0.tar", last modified: Fri Apr 21 09:57:38 2023, max compression
```

## Comparing `stylo_metrix-0.0.7.tar` & `stylo_metrix-0.1.0.tar`

### file list

```diff
@@ -1,71 +1,92 @@
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.468601 stylo_metrix-0.0.7/
--rw-rw-rw-   0        0        0    33095 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/LICENSE
--rw-rw-rw-   0        0        0        0 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    10970 2022-09-02 09:01:06.470623 stylo_metrix-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10491 2022-08-22 11:59:37.000000 stylo_metrix-0.0.7/README.md
--rw-rw-rw-   0        0        0      772 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      719 2022-09-02 09:01:06.477925 stylo_metrix-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.021093 stylo_metrix-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.094498 stylo_metrix-0.0.7/src/stylo_metrix/
--rw-rw-rw-   0        0        0     1135 2022-08-24 12:57:39.000000 stylo_metrix-0.0.7/src/stylo_metrix/__init__.py
--rw-rw-rw-   0        0        0     3895 2022-09-02 08:48:12.000000 stylo_metrix-0.0.7/src/stylo_metrix/functions.py
--rw-rw-rw-   0        0        0     1629 2022-08-22 11:57:19.000000 stylo_metrix-0.0.7/src/stylo_metrix/logger.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.140028 stylo_metrix-0.0.7/src/stylo_metrix/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-24 08:51:58.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.185814 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/
--rw-rw-rw-   0        0        0     1229 2022-06-20 20:11:11.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/__init__.py
--rw-rw-rw-   0        0        0      809 2022-08-24 10:21:54.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/en.py
--rw-rw-rw-   0        0        0    14131 2022-08-24 10:27:22.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/grammatical_forms.py
--rw-rw-rw-   0        0        0    15495 2022-08-24 10:26:59.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/lexical_en.py
--rw-rw-rw-   0        0        0     4145 2022-08-24 10:23:15.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/parts_of_speech_en.py
--rw-rw-rw-   0        0        0     5656 2022-08-24 10:27:32.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/syntactic_en.py
--rw-rw-rw-   0        0        0    12452 2022-08-24 10:21:09.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/verb_tenses_en.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.262413 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/
--rw-rw-rw-   0        0        0     1877 2022-08-12 11:38:33.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/__init__.py
--rw-rw-rw-   0        0        0     2760 2022-08-24 10:54:12.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/grammatical_forms.py
--rw-rw-rw-   0        0        0    17227 2022-08-24 10:54:28.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/inflection.py
--rw-rw-rw-   0        0        0     6787 2022-08-24 10:54:50.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/lexical.py
--rw-rw-rw-   0        0        0      808 2022-08-24 10:21:54.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/pl.py
--rw-rw-rw-   0        0        0     7734 2022-08-24 10:54:12.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/psycholinguistic.py
--rw-rw-rw-   0        0        0     4865 2022-08-24 10:31:40.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/syntactic.py
--rw-rw-rw-   0        0        0     6140 2022-08-24 10:54:33.000000 stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/word_formation.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.278199 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/
--rw-rw-rw-   0        0        0        0 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.326180 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/
--rw-rw-rw-   0        0        0      980 2022-09-02 08:47:31.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/__init__.py
--rw-rw-rw-   0        0        0     1097 2022-08-22 11:56:11.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/custom_preprocessing.py
--rw-rw-rw-   0        0        0     2961 2022-06-18 11:38:39.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/dictionary_en.py
--rw-rw-rw-   0        0        0    52326 2022-08-22 11:55:27.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/grammar.py
--rw-rw-rw-   0        0        0     1497 2022-09-02 08:47:47.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/metrics.py
--rw-rw-rw-   0        0        0     1821 2022-08-22 11:57:15.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/params.py
--rw-rw-rw-   0        0        0     2495 2022-08-22 11:57:15.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/pos_tagger.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.365778 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/
--rw-rw-rw-   0        0        0     1176 2022-09-02 08:47:31.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/__init__.py
--rw-rw-rw-   0        0        0     1449 2022-09-02 08:47:43.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/metrics.py
--rw-rw-rw-   0        0        0     1931 2022-08-15 16:13:35.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/params.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.387980 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/
--rw-rw-rw-   0        0        0        0 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/__init__.py
--rw-rw-rw-   0        0        0     4284 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py
--rw-rw-rw-   0        0        0     6232 2022-06-03 12:43:58.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/pos.py
--rw-rw-rw-   0        0        0     3892 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pos_tagger.py
--rw-rw-rw-   0        0        0     1286 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/psycholinguistic.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.403766 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/resources/
--rw-rw-rw-   0        0        0        0 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/resources/__init__.py
--rw-rw-rw-   0        0        0   290924 2022-06-03 12:43:58.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/resources/experimental_data.py
--rw-rw-rw-   0        0        0     1155 2022-05-20 11:35:36.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/sentence_segmenter.py
--rw-rw-rw-   0        0        0     2119 2022-09-02 08:48:17.000000 stylo_metrix-0.0.7/src/stylo_metrix/pipeline/stylo_metrix_pipe.py
--rw-rw-rw-   0        0        0     2716 2022-08-15 17:06:59.000000 stylo_metrix-0.0.7/src/stylo_metrix/reader.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.463609 stylo_metrix-0.0.7/src/stylo_metrix/structures/
--rw-rw-rw-   0        0        0      890 2022-06-18 12:45:13.000000 stylo_metrix-0.0.7/src/stylo_metrix/structures/__init__.py
--rw-rw-rw-   0        0        0     2413 2022-08-24 11:52:17.000000 stylo_metrix-0.0.7/src/stylo_metrix/structures/errors.py
--rw-rw-rw-   0        0        0     3263 2022-08-24 10:55:53.000000 stylo_metrix-0.0.7/src/stylo_metrix/structures/metric.py
--rw-rw-rw-   0        0        0     4161 2022-09-02 08:56:33.000000 stylo_metrix-0.0.7/src/stylo_metrix/structures/metrics_group.py
--rw-rw-rw-   0        0        0     1991 2022-08-24 11:13:31.000000 stylo_metrix-0.0.7/src/stylo_metrix/structures/stylo_metrix_vector.py
--rw-rw-rw-   0        0        0     2168 2022-08-22 11:55:27.000000 stylo_metrix-0.0.7/src/stylo_metrix/utils.py
--rw-rw-rw-   0        0        0     2175 2022-09-02 08:58:54.000000 stylo_metrix-0.0.7/src/stylo_metrix/writer.py
-drwxrwxrwx   0        0        0        0 2022-09-02 09:01:06.134870 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/
--rw-rw-rw-   0        0        0    10970 2022-09-02 09:01:05.000000 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2220 2022-09-02 09:01:06.000000 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-02 09:01:05.000000 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-09-02 09:01:05.000000 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-09-02 09:01:05.000000 stylo_metrix-0.0.7/src/stylo_metrix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.387712 stylo_metrix-0.1.0/
+-rw-rw-rw-   0        0        0    33095 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10974 2023-04-21 09:57:38.387712 stylo_metrix-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10491 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/README.md
+-rw-rw-rw-   0        0        0      772 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      798 2023-04-21 09:57:38.392846 stylo_metrix-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:37.979828 stylo_metrix-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.018828 stylo_metrix-0.1.0/src/stylo_metrix/
+-rw-rw-rw-   0        0        0      847 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.038836 stylo_metrix-0.1.0/src/stylo_metrix/metrics/
+-rw-rw-rw-   0        0        0      758 2023-03-15 13:04:26.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.097836 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/
+-rw-rw-rw-   0        0        0     1157 2023-03-10 20:11:10.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/__init__.py
+-rw-rw-rw-   0        0        0     5113 2023-03-15 13:30:46.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/distance_en.py
+-rw-rw-rw-   0        0        0     1971 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/figures_of_speech.py
+-rw-rw-rw-   0        0        0    13569 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/grammatical_forms.py
+-rw-rw-rw-   0        0        0    16796 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/lexical_en.py
+-rw-rw-rw-   0        0        0     4081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/parts_of_speech_en.py
+-rw-rw-rw-   0        0        0     4464 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/psycholinguistics.py
+-rw-rw-rw-   0        0        0     8324 2023-03-29 12:59:55.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/social_media.py
+-rw-rw-rw-   0        0        0     7885 2023-03-29 12:59:55.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/syntactic_en.py
+-rw-rw-rw-   0        0        0     4223 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/text_statistics.py
+-rw-rw-rw-   0        0        0    12004 2023-04-06 13:12:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/verb_tenses_en.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.188389 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/
+-rw-rw-rw-   0        0        0     1059 2023-03-10 19:52:40.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/descriptive.py
+-rw-rw-rw-   0        0        0     5229 2023-04-06 13:10:29.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/grammatical_forms.py
+-rw-rw-rw-   0        0        0     1336 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/graphical.py
+-rw-rw-rw-   0        0        0    19983 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/inflection.py
+-rw-rw-rw-   0        0        0     6373 2023-03-10 20:11:05.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/lexical.py
+-rw-rw-rw-   0        0        0     6066 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/psycholinguistic.py
+-rw-rw-rw-   0        0        0     2330 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/punctuation.py
+-rw-rw-rw-   0        0        0     7377 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/syntactic.py
+-rw-rw-rw-   0        0        0     5788 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/word_formation.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.210918 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/
+-rw-rw-rw-   0        0        0      944 2023-03-15 13:04:46.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/__init__.py
+-rw-rw-rw-   0        0        0    17631 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/lexical_ukr.py
+-rw-rw-rw-   0        0        0     4040 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py
+-rw-rw-rw-   0        0        0     6598 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/syntactic_ukr.py
+-rw-rw-rw-   0        0        0    10724 2023-03-28 08:06:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/verb_forms_ukr.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.216917 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/
+-rw-rw-rw-   0        0        0       23 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.300474 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/
+-rw-rw-rw-   0        0        0      987 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/custom_preprocessing.py
+-rw-rw-rw-   0        0        0     8872 2023-03-10 19:46:18.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/dictionary_en.py
+-rw-rw-rw-   0        0        0    44832 2023-04-06 13:12:03.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/grammar.py
+-rw-rw-rw-   0        0        0     1909 2023-03-10 19:53:28.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/params.py
+-rw-rw-rw-   0        0        0     3065 2023-03-29 12:59:55.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/pos_tagger.py
+-rw-rw-rw-   0        0        0     3402 2023-03-10 19:46:18.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/psycholinguistics.py
+-rw-rw-rw-   0        0        0     5020 2023-03-29 12:59:55.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/stylistic.py
+-rw-rw-rw-   0        0        0     2157 2023-04-17 09:17:44.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/new_pipe.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.320874 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/
+-rw-rw-rw-   0        0        0     1206 2023-03-15 11:55:34.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/__init__.py
+-rw-rw-rw-   0        0        0     2213 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/matcher_component.py
+-rw-rw-rw-   0        0        0     1931 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/params.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.332543 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/__init__.py
+-rw-rw-rw-   0        0        0     4284 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py
+-rw-rw-rw-   0        0        0     6232 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/pos.py
+-rw-rw-rw-   0        0        0     3892 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pos_tagger.py
+-rw-rw-rw-   0        0        0     1286 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/psycholinguistic.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.338543 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/resources/__init__.py
+-rw-rw-rw-   0        0        0   290924 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/resources/experimental_data.py
+-rw-rw-rw-   0        0        0     1155 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/sentence_segmenter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.363712 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/
+-rw-rw-rw-   0        0        0      833 2023-03-15 11:56:59.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-03-15 10:11:22.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/custom_preprocessing.py
+-rw-rw-rw-   0        0        0     1128 2023-03-15 10:11:22.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/dictionary_ukr.py
+-rw-rw-rw-   0        0        0     4715 2023-03-15 10:11:22.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/grammar_ukr.py
+-rw-rw-rw-   0        0        0     1753 2023-03-15 10:11:22.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/params.py
+-rw-rw-rw-   0        0        0     2232 2023-03-15 10:11:22.000000 stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.380712 stylo_metrix-0.1.0/src/stylo_metrix/structures/
+-rw-rw-rw-   0        0        0      812 2023-03-10 19:12:54.000000 stylo_metrix-0.1.0/src/stylo_metrix/structures/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-03-10 19:54:10.000000 stylo_metrix-0.1.0/src/stylo_metrix/structures/category.py
+-rw-rw-rw-   0        0        0     2826 2023-03-10 19:54:30.000000 stylo_metrix-0.1.0/src/stylo_metrix/structures/language.py
+-rw-rw-rw-   0        0        0     2691 2023-03-10 19:54:39.000000 stylo_metrix-0.1.0/src/stylo_metrix/structures/metric.py
+-rw-rw-rw-   0        0        0     2605 2023-03-10 19:55:00.000000 stylo_metrix-0.1.0/src/stylo_metrix/structures/metrics_group.py
+-rw-rw-rw-   0        0        0     3654 2023-04-06 11:39:35.000000 stylo_metrix-0.1.0/src/stylo_metrix/stylo_metrix.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.386712 stylo_metrix-0.1.0/src/stylo_metrix/tools/
+-rw-rw-rw-   0        0        0       26 2023-03-10 19:46:18.000000 stylo_metrix-0.1.0/src/stylo_metrix/tools/__init__.py
+-rw-rw-rw-   0        0        0     1830 2023-03-10 19:55:48.000000 stylo_metrix-0.1.0/src/stylo_metrix/tools/metric_tools.py
+-rw-rw-rw-   0        0        0     2175 2023-03-10 19:48:40.000000 stylo_metrix-0.1.0/src/stylo_metrix/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:57:38.035829 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/
+-rw-rw-rw-   0        0        0    10974 2023-04-21 09:57:37.000000 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3067 2023-04-21 09:57:37.000000 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:57:37.000000 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-04-21 09:57:37.000000 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 09:57:37.000000 stylo_metrix-0.1.0/src/stylo_metrix.egg-info/top_level.txt
```

### Comparing `stylo_metrix-0.0.7/LICENSE` & `stylo_metrix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/PKG-INFO` & `stylo_metrix-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: stylo_metrix
-Version: 0.0.7
+Version: 0.1.0
 Summary: StyloMetrix tool
 Home-page: https://github.com/ZILiAT-NASK/StyloMetrix
-Author: ZILiAT-NASK, Anna Zawadzka
-Author-email: anna.zawadzka@nask.pl
+Author: ZILiAT-NASK, Adam Nowakowski
+Author-email: adam.nowakowski@nask.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: stylo_metrix Version: 0.0.7 Summary: StyloMetrix
+Metadata-Version: 2.1 Name: stylo_metrix Version: 0.1.0 Summary: StyloMetrix
 tool Home-page: https://github.com/ZILiAT-NASK/StyloMetrix Author: ZILiAT-NASK,
-Anna Zawadzka Author-email: anna.zawadzka@nask.pl Classifier: Programming
+Adam Nowakowski Author-email: adam.nowakowski@nask.pl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # StyloMetrix [StyloMetrix][NASK] ZakÅad InÅ¼ynierii Lingwistycznej i
 Anailzy Tekstu, NASK PIB ## ð Quick ð¡ Stylometry tool in beta version for
 **Polish** and **English** language, distributed as a **Python package** ð¡
 [Tutorial notebook](examples/Quick%20Tutorial.ipynb) ð¡ List of built-in
```

### Comparing `stylo_metrix-0.0.7/README.md` & `stylo_metrix-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/pyproject.toml` & `stylo_metrix-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/setup.cfg` & `stylo_metrix-0.1.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7479 6c6f 5f6d 6574 7269 780d   = stylo_metrix.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e37  .version = 0.0.7
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
 00000030: 0d0a 6175 7468 6f72 203d 205a 494c 6941  ..author = ZILiA
-00000040: 542d 4e41 534b 2c20 416e 6e61 205a 6177  T-NASK, Anna Zaw
-00000050: 6164 7a6b 610d 0a61 7574 686f 725f 656d  adzka..author_em
-00000060: 6169 6c20 3d20 616e 6e61 2e7a 6177 6164  ail = anna.zawad
-00000070: 7a6b 6140 6e61 736b 2e70 6c0d 0a64 6573  zka@nask.pl..des
-00000080: 6372 6970 7469 6f6e 203d 2053 7479 6c6f  cription = Stylo
-00000090: 4d65 7472 6978 2074 6f6f 6c0d 0a6c 6f6e  Metrix tool..lon
-000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000b0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-000000c0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000d0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000e0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000100: 7468 7562 2e63 6f6d 2f5a 494c 6941 542d  thub.com/ZILiAT-
-00000110: 4e41 534b 2f53 7479 6c6f 4d65 7472 6978  NASK/StyloMetrix
-00000120: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000130: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000140: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000150: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-00000160: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000170: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
-00000180: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
-00000190: 3320 2847 504c 7633 290d 0a09 4f70 6572  3 (GPLv3)...Oper
-000001a0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001b0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000001c0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-000001d0: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
-000001e0: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
-000001f0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000200: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-00000210: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000220: 203d 200d 0a09 7365 7475 7074 6f6f 6c73   = ...setuptools
-00000230: 3e3d 3439 2e32 2e30 0d0a 096e 756d 7079  >=49.2.0...numpy
-00000240: 3e3d 312e 3137 2e30 0d0a 0970 616e 6461  >=1.17.0...panda
-00000250: 733e 3d31 2e30 2e35 0d0a 0973 7061 6379  s>=1.0.5...spacy
-00000260: 0d0a 0973 7061 6379 2d73 796c 6c61 626c  ...spacy-syllabl
-00000270: 6573 3d3d 332e 302e 310d 0a0d 0a5b 6f70  es==3.0.1....[op
-00000280: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000290: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000002a0: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-000002b0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000002c0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000040: 542d 4e41 534b 2c20 4164 616d 204e 6f77  T-NASK, Adam Now
+00000050: 616b 6f77 736b 690d 0a61 7574 686f 725f  akowski..author_
+00000060: 656d 6169 6c20 3d20 6164 616d 2e6e 6f77  email = adam.now
+00000070: 616b 6f77 736b 6940 6e61 736b 2e70 6c0d  akowski@nask.pl.
+00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2053  .description = S
+00000090: 7479 6c6f 4d65 7472 6978 2074 6f6f 6c0d  tyloMetrix tool.
+000000a0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000b0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000c0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000d0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000e0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000f0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+00000100: 2f2f 6769 7468 7562 2e63 6f6d 2f5a 494c  //github.com/ZIL
+00000110: 6941 542d 4e41 534b 2f53 7479 6c6f 4d65  iAT-NASK/StyloMe
+00000120: 7472 6978 0d0a 636c 6173 7369 6669 6572  trix..classifier
+00000130: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+00000140: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000150: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
+00000160: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000170: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000180: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000190: 7365 2076 3320 2847 504c 7633 290d 0a09  se v3 (GPLv3)...
+000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001c0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
+000001d0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+000001e0: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+000001f0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000200: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000210: 2e36 0d0a 696e 7374 616c 6c5f 7265 7175  .6..install_requ
+00000220: 6972 6573 203d 200d 0a09 7365 7475 7074  ires = ...setupt
+00000230: 6f6f 6c73 3e3d 3439 2e32 2e30 0d0a 096e  ools>=49.2.0...n
+00000240: 756d 7079 3e3d 312e 3137 2e30 0d0a 0970  umpy>=1.17.0...p
+00000250: 616e 6461 733e 3d31 2e30 2e35 0d0a 0973  andas>=1.0.5...s
+00000260: 6369 6b69 742d 6c65 6172 6e0d 0a09 7370  cikit-learn...sp
+00000270: 6163 790d 0a09 7370 6163 792d 7379 6c6c  acy...spacy-syll
+00000280: 6162 6c65 733d 3d33 2e30 2e31 0d0a 0976  ables==3.0.1...v
+00000290: 6164 6572 5365 6e74 696d 656e 740d 0a09  aderSentiment...
+000002a0: 7370 6163 792d 7472 616e 7366 6f72 6d65  spacy-transforme
+000002b0: 7273 0d0a 096d 6f72 6665 7573 7a32 0d0a  rs...morfeusz2..
+000002c0: 0970 6578 7065 6374 0d0a 0d0a 5b6f 7074  .pexpect....[opt
+000002d0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000002e0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+000002f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000300: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000310: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/en.py` & `stylo_metrix-0.1.0/src/stylo_metrix/structures/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,11 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
-
-from stylo_metrix.structures import Metric
-
-
-class EnglishMetric(Metric, ABC):
-    lang = "en"
+from .language import Lang
+from .category import Category
+from .metric import Metric
+from .metrics_group import MetricGroup
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/grammatical_forms.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/grammatical_forms.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,453 +10,443 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
+from stylo_metrix.structures import Metric, Category
 
-from stylo_metrix.metrics.en.en import EnglishMetric
-from stylo_metrix.structures import Metric, MetricsGroup
 from stylo_metrix.utils import incidence
 
 
-class GrammaticalForms(EnglishMetric, ABC):
-    category_en = "Grammatical Forms"
-    category_id = 2
+class GrammaticalForms(Category):
+    lang = 'en'
+    name_en = "Grammatical Forms"
 
+class G_WOULD(Metric):
+    category = GrammaticalForms
+    name_en = "Would verb simple"
 
-class G_WOULD(GrammaticalForms):
-    name_en = "Would Simple Incidence"
-    metric_id =1
-
-    def count(self, doc):
-        search = [token for token in doc if token._.modal_verbs == "would_ind_activ"]
+    def count(doc):
+        search = [token for token in doc if token._.modal_verbs == "would_ind_active"]
         result = incidence(doc, search)
-        return result, {"G_WLD": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_WOULD_PASSIVE(GrammaticalForms):
-    name_en = "Would Passive Incidence"
-    metric_id = 2
+class G_WOULD_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Would verb passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "would_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_WLD_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_WOULD_PROGRESSIVE(GrammaticalForms):
-    name_en = "Would Continuous Incidence"
-    metric_id = 3
+class G_WOULD_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Would verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "would_cont"]
         result = incidence(doc, search)
-        return result, {"G_WLD_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_WOULD_PERFECT(GrammaticalForms):
-    name_en = "Would Perfect Incidence"
-    metric_id = 4
+class G_WOULD_PERFECT(Metric):
+    category = GrammaticalForms
+    name_en = "Would verb perfect"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "would_perf_active"]
         result = incidence(doc, search)
-        return result, {"G_WLD_PRF": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_WOULD_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "Would Perfect Passive Incidence"
-    metric_id = 5
+class G_WOULD_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Would verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "would_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_WLD_P_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHOULD(GrammaticalForms):
-    name_en = "Should Simple Incidence"
-    metric_id = 6
+class G_SHOULD(Metric):
+    category = GrammaticalForms
+    name_en = "Should verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "should_ind_active"]
         result = incidence(doc, search)
-        return result, {"G_SHLD": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHOULD_PASSIVE(GrammaticalForms):
-    name_en = "Should Simple Passive Incidence"
-    metric_id = 7
+class G_SHOULD_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Should verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "should_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_SHLD_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHALL(GrammaticalForms):
-    name_en = "Shall Simple Incidence"
-    metric_id = 8
+class G_SHALL(Metric):
+    category = GrammaticalForms
+    name_en = "Shall verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "shall_ind_active"]
         result = incidence(doc, search)
-        return result, {"G_SHLL": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHALL_PASSIVE(GrammaticalForms):
-    name_en = "Shall Simple Passive Incidence"
-    metric_id = 9
+class G_SHALL_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Shall verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "shall_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_SHLL_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHOULD_PROGRESSIVE(GrammaticalForms):
-    name_en = "Should Continuous Incidence"
-    metric_id = 10
+class G_SHOULD_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Should verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "should_cont"]
         result = incidence(doc, search)
-        return result, {"G_SHLD_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHOULD_PERFECT(GrammaticalForms):
-    name_en = "Should Perfect Incidence"
-    metric_id = 11
+class G_SHOULD_PERFECT(Metric):
+    category = GrammaticalForms
+    name_en = "Should verb perfect"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "should_perf_active"]
         result = incidence(doc, search)
-        return result, {"G_SHLD_PRF": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_SHOULD_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "Should Perfect Passive Incidence"
-    metric_id = 12
+class G_SHOULD_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Should verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "should_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_SHLD_P_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MUST(GrammaticalForms):
-    name_en = "Must Simple Incidence"
-    metric_id = 13
+class G_MUST(Metric):
+    category = GrammaticalForms
+    name_en = "Must verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "must_ind_active"]
         result = incidence(doc, search)
-        return result, {"G_MST": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MUST_PASSIVE(GrammaticalForms):
-    name_en = "Must Simple Passive Incidence"
-    metric_id = 14
+class G_MUST_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Must verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "must_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_MST_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MUST_PROGRESSIVE(GrammaticalForms):
-    name_en = "Must Continuous Incidence"
-    metric_id = 15
+class G_MUST_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Must verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "must_cont"]
         result = incidence(doc, search)
-        return result, {"G_MST_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MUST_PERFECT(GrammaticalForms):
-    name_en = "Must Perfect Incidence"
-    metric_id = 16
+class G_MUST_PERFECT(Metric):
+    category = GrammaticalForms
+    name_en = "Must verb perfect"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "must_perf_active"]
         result = incidence(doc, search)
-        return result, {"G_MST_PRF": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MST_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "Must Perfect Passive Incidence"
-    metric_id = 17
+class G_MST_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Must verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "must_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_MST_P_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_CAN(GrammaticalForms):
-    name_en = "Can Simple Incidence"
-    metric_id = 18
+class G_CAN(Metric):
+    category = GrammaticalForms
+    name_en = "Can verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "can_ind"]
         result = incidence(doc, search)
-        return result, {"G_CAN": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_CAN_PASSIVE(GrammaticalForms):
-    name_en = "Can Simple Passive Incidence"
-    metric_id = 19
+class G_CAN_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Can verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "can_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_CAN_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_COULD(GrammaticalForms):
-    name_en = "Could Simple Incidence"
-    metric_id = 20
+class G_COULD(Metric):
+    category = GrammaticalForms
+    name_en = "Could verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "could_ind"]
         result = incidence(doc, search)
-        return result, {"G_CLD": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_COULD_PASSIVE(GrammaticalForms):
-    name_en = "Could Simple Passive Incidence"
-    metric_id = 21
+class G_COULD_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Could verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "could_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_CLD_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_CAN_PROGRESSIVE(GrammaticalForms):
-    name_en = "Can Continuous Incidence"
-    metric_id = 22
+class G_CAN_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Can verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "can_cont"]
         result = incidence(doc, search)
-        return result, {"G_CAN_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_COULD_PROGRESSIVE(GrammaticalForms):
-    name_en = "Could Continuous Incidence"
-    metric_id = 23
+class G_COULD_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Could verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "could_cont"]
         result = incidence(doc, search)
-        return result, {"G_CLD_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_COULD_PERFECT(GrammaticalForms):
-    name_en = "Could Perfect Incidence"
-    metric_id = 24
+class G_COULD_PERFECT(Metric):
+    category = GrammaticalForms
+    name_en = "Could verb perfect"
 
-    def count(self, doc):
-        search = [token for token in doc if token._.modal_verbs == "could_perf"]
+    def count(doc):
+        search = [token.text for token in doc if token._.modal_verbs == "could_perf"]
         result = incidence(doc, search)
-        return result, {"G_CLD_PRF": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_COULD_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "Could Perfect Passive Incidence"
-    metric_id = 25
+class G_COULD_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Could verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "could_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_CLD_P_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MAY(GrammaticalForms):
-    name_en = "May Simple Incidence"
-    metric_id = 26
+class G_MAY(Metric):
+    category = GrammaticalForms
+    name_en = "May verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "may_ind"]
         result = incidence(doc, search)
-        return result, {"G_MAY": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MAY_PASSIVE(GrammaticalForms):
-    name_en = "May Simple Passive Incidence"
-    metric_id = 27
+class G_MAY_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "May verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "may_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_MAY_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MIGHT(GrammaticalForms):
-    name_en = "Might Simple Incidence"
-    metric_id = 28
+class G_MIGHT(Metric):
+    category = GrammaticalForms
+    name_en = "Might verb simple"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "might_ind"]
         result = incidence(doc, search)
-        return result, {"G_MGHT": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MIGHT_PASSIVE(GrammaticalForms):
-    name_en = "Might Simple Passive Incidence"
-    metric_id = 29
+class G_MIGHT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Might verb simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "might_ind_passive"]
         result = incidence(doc, search)
-        return result, {"G_MGHT_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MAY_PROGRESSIVE(GrammaticalForms):
-    name_en = "May Continuous Incidence"
-    metric_id = 30
+class G_MAY_PROGRESSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "May verb continuous"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "may_cont"]
         result = incidence(doc, search)
-        return result, {"G_MAY_CON": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MIGTH_PERFECT(GrammaticalForms):
-    name_en = "Might Perfect Incidence"
-    metric_id = 31
+class G_MIGTH_PERFECT(Metric):
+    category = GrammaticalForms
+    name_en = "Might verb perfect"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "might_perf"]
         result = incidence(doc, search)
-        return result, {"G_MGTH_PRF": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-#
-class G_MIGHT_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "Might Perfect Passive Incidence"
-    metric_id = 32
+class G_MIGHT_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Might verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "might_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_MGHT_PRF_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_MAY_PERFECT_PASSIVE(GrammaticalForms):
-    name_en = "May Perfect Passive Incidence"
-    metric_id = 33
+class G_MAY_PERFECT_PASSIVE(Metric):
+    category = GrammaticalForms
+    name_en = "May verb perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.modal_verbs == "may_perf_passive"]
         result = incidence(doc, search)
-        return result, {"G_MAY_PRF_P": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADJ_POSITIVE(GrammaticalForms):
-    name_en = "Adjectives Positive Degree Incidence"
-    metric_id = 34
+class G_ADJ_POSITIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adjectives in positive degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adjectives == "positive_adjective"]
         result = incidence(doc, search)
-        return result, {"G_ADJ_POS": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADJ_COMPARATIVE(GrammaticalForms):
-    name_en = "Adjectives Comparative Degree Incidence"
-    metric_id = 35
+class G_ADJ_COMPARATIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adjectives in comparative degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adjectives == "comparative_adjective"]
         result = incidence(doc, search)
-        return result, {"G_ADJ_COMP": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADJ_SUPERLATIVE(GrammaticalForms):
-    name_en = "Adjectives Superlative Degree Incidence"
-    metric_id = 36
+class G_ADJ_SUPERLATIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adjectives in superlative degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adjectives == "superlative_adjective"]
         result = incidence(doc, search)
-        return result, {"G_ADJ_SUP": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADV_POSITIVE(GrammaticalForms):
-    name_en = "Adverbs Positive Degree Incidence"
-    metric_id = 37
+class G_ADV_POSITIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adverbs in positive degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adverbs == "positive_adverb"]
         result = incidence(doc, search)
-        return result, {"G_ADV_POS": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADV_COMPARATIVE(GrammaticalForms):
-    name_en = "Adverbs Comparative Degree Incidence"
-    metric_id = 38
+class G_ADV_COMPARATIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adverbs in comparative degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adverbs == "comparative_adverb"]
         result = incidence(doc, search)
-        return result, {"G_ADV_COMP": search}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class G_ADV_SUPERLATIVE(GrammaticalForms):
-    name_en = "Adverbs Superlative Degree Incidence"
-    metric_id = 39
+class G_ADV_SUPERLATIVE(Metric):
+    category = GrammaticalForms
+    name_en = "Adverbs in superlative degree"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.adverbs == "superlative_adverb"]
         result = incidence(doc, search)
-        return result, {"G_ADV_SUP": search}
-
-
-GRAMMATICAL_FORMS = [
-    G_WOULD,
-    G_WOULD_PASSIVE,
-    G_WOULD_PROGRESSIVE,
-    G_WOULD_PERFECT,
-    G_WOULD_PERFECT_PASSIVE,
-    G_SHOULD,
-    G_SHOULD_PASSIVE,
-    G_SHALL,
-    G_SHALL_PASSIVE,
-    G_SHOULD_PROGRESSIVE,
-    G_SHOULD_PERFECT,
-    G_SHOULD_PERFECT_PASSIVE,
-    G_MUST,
-    G_MUST_PASSIVE,
-    G_MUST_PROGRESSIVE,
-    G_MUST_PERFECT,
-    G_MST_PERFECT_PASSIVE,
-    G_CAN,
-    G_CAN_PASSIVE,
-    G_COULD,
-    G_COULD_PASSIVE,
-    G_CAN_PROGRESSIVE,
-    G_COULD_PROGRESSIVE,
-    G_COULD_PERFECT,
-    G_COULD_PERFECT_PASSIVE,
-    G_MAY,
-    G_MAY_PASSIVE,
-    G_MIGHT,
-    G_MIGHT_PASSIVE,
-    G_MAY_PROGRESSIVE,
-    G_MIGTH_PERFECT,
-    G_MIGHT_PERFECT_PASSIVE,
-    G_MAY_PERFECT_PASSIVE,
-    G_ADJ_POSITIVE,
-    G_ADJ_COMPARATIVE,
-    G_ADJ_SUPERLATIVE,
-    G_ADV_POSITIVE,
-    G_ADV_COMPARATIVE,
-    G_ADV_SUPERLATIVE,
-]
-
-grammatical_forms_group = MetricsGroup([m() for m in GRAMMATICAL_FORMS])
+        debug = {'TOKENS': search}
+        return result, debug
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/parts_of_speech_en.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,143 +10,134 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
-
-from stylo_metrix.metrics.en.en import EnglishMetric
-from stylo_metrix.structures import MetricsGroup
+from stylo_metrix.structures import Category, Metric
 from stylo_metrix.utils import incidence
 
 
-class Part_of_speech(EnglishMetric, ABC):
-    category_en = "Parts of speech"
-    category_id = 1
+class PartOfSpeech(Category):
+    lang = 'ukr'
+    name_en = "Parts of speech"
 
 
-class POS_VERB(Part_of_speech):
+class POS_VERB(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Verbs"
-    metric_id = 1
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "v"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_NOUN(Part_of_speech):
+class POS_NOUN(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Nouns"
-    metric_id = 2
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "n"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_ADJ(Part_of_speech):
+class POS_ADJ(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Adjectives"
-    metric_id = 3
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "adj"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_ADV(Part_of_speech):
+class POS_ADV(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Adverbs"
-    metric_id = 4
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "adv"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_DET(Part_of_speech):
+class POS_DET(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Determiners"
-    metric_id = 5
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "det"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_INTJ(Part_of_speech):
+class POS_INTJ(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Interjections"
-    metric_id = 6
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "intj"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_CONJ(Part_of_speech):
+class POS_CONJ(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Conjunctions"
-    metric_id = 7
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "conj"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_PART(Part_of_speech):
+class POS_PART(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Particles"
-    metric_id = 8
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "part"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_NUM(Part_of_speech):
+class POS_NUM(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Numerals"
-    metric_id = 9
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "num"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_PREP(Part_of_speech):
+class POS_PREP(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Prepositions"
-    metric_id = 10
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc._.words if token._.pos == "prep"]
         result = incidence(doc, search)
         return result, {}
 
 
-class POS_PRO(Part_of_speech):
+class POS_PRO(Metric):
+    category = PartOfSpeech
     name_en = "Incidence of Pronouns"
-    metric_id = 11
 
-    def count(self, doc):
-        search = [token for token in doc._.words if token._.pos == "prep"]
+    def count(doc):
+        search = [token for token in doc._.words if token._.pos == "pro"]
         result = incidence(doc, search)
         return result, {}
 
-PART_OF_SPEECH = [
-    POS_VERB,
-    POS_NOUN,
-    POS_ADJ,
-    POS_ADV,
-    POS_DET,
-    POS_INTJ,
-    POS_CONJ,
-    POS_PART,
-    POS_NUM,
-    POS_PREP,
-]
 
+class POS_OTHER(Metric):
+    category = PartOfSpeech
+    name_en = "Incidence of Code-Switching"
 
-parts_of_speech = MetricsGroup([m() for m in PART_OF_SPEECH])
+    def count(doc):
+        search = [token for token in doc._.words if token._.pos == "other"]
+        result = incidence(doc, search)
+        return result, {}
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/syntactic_en.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/ukr/syntactic_ukr.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,152 +10,182 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
-import itertools
-
-from stylo_metrix.metrics.en.en import EnglishMetric
-from stylo_metrix.structures import MetricsGroup
+from spacy.matcher import Matcher
+from stylo_metrix.structures import Category, Metric
 from stylo_metrix.utils import incidence, ratio, start_end_quote
-from spacy.tokens import Span
-
-
-class Syntactic(EnglishMetric, ABC):
-    category_en = "Syntactic"
-    category_id = 5
+import itertools
 
+class Syntactic(Category):
+    lang = 'ukr'
+    name_en = "Syntactic"
 
-class SY_QUESTION(Syntactic):
-    name_en = "Words in questions incidence"
-    metric_id = 1
 
-    def count(self, doc):
-        sentence_tokens = [[token for token in sent if '?' in sent.text] for sent in doc.sents]
-        words = sum([[token for token in sent if token._.is_word] for sent in sentence_tokens], [])
-        result = incidence(doc, words)
-        return result, {"QS": sentence_tokens}
+class SY_DIRECT_SPEECH(Metric):
+    category = Syntactic
+    name_en = "Number of words in direct speech"
 
+    def count(doc):
+        start, end = start_end_quote(doc)
+        if (start and end) != None:
+            span = doc[start:end]
+            span_words = [token for token in span if token._.is_word]
+            result = incidence(doc, span_words)
+            return result, {"Direct Speech": span_words}
+        else:
+            result = ratio(len(doc), 0)
+            return result, {}
 
-class SY_EXCLAMATION(Syntactic):
-    name_en = "Words in exclamatory sentences incidence"
-    metric_id = 2
 
-    def count(self, doc):
-        sentence_tokens = [[token for token in sent if '!' in sent.text] for sent in doc.sents]
-        words = sum([[token for token in sent if token._.is_word] for sent in sentence_tokens], [])
-        result = incidence(doc, words)
+class SY_NEGATIVE(Metric):
+    category = Syntactic
+    name_en = "Number of words in negative sentences"
+
+    def count(doc):
+        neg = set([sent for sent in doc.sents for token in sent if "Polarity=Neg" in token.morph])
+        flatten = [token for i in neg for token in i]
+        result = incidence(doc, flatten)
         return result, {}
 
 
-class SY_IMPERATIVE(Syntactic):
-    name_en = "Words in imperative sentences incidence"
-    metric_id = 3
-
-    def count(self, doc):
-        sentence_tokens = [[token for token in sent] for sent in doc.sents if
-                           "VerbForm=Inf" in sent[0].morph and sent[0].pos_ == "VERB"]
-        words = sum([[token for token in sent if token._.is_word] for sent in sentence_tokens], [])
-        result = incidence(doc, words)
+# https://universaldependencies.org/u/dep/parataxis.html?
+class SY_PARATAXIS(Metric):
+    category = Syntactic
+    name_en = "Number of words in parataxis sentences"
+
+    def count(doc):
+        prt = set([sent for sent in doc.sents for token in sent if "parataxis" in token.dep_])
+        tokens = [token for i in prt for token in i]
+        result = incidence(doc, tokens)
         return result, {}
 
+class SY_NON_FINITE(Metric):
+    category = Syntactic
+    name_en = "Number of words in sentences without any verbs"
+
+    def count(doc):
+        sent = [sent for sent in doc.sents if not any(token for token in sent if token.pos_ == "VERB")]
+        result = incidence(doc, sent)
+        return result, {}
 
-class SY_SUBORD_SENT(Syntactic):
-    name_en = "Words in subordinate sentences incidence"
-    metric_id = 4
-
-    def count(self, doc):
-        subord_sentences = [sent for sent in doc.sents if any(token.pos_ == "SCONJ" for token in sent)]
-        join_sents = itertools.chain(*subord_sentences)
-        sent_tok = [tkn for tkn in join_sents if tkn.pos_ != "PUNCT"]
-
-        result = incidence(doc, sent_tok)
-        return result, {"SUBORD_SENT": sent_tok}
-
-
-class SY_SUBORD_SENT_PUNCT(Syntactic):
-    name_en = "Punctuation in subordinate sentences incidence"
-    metric_id = 5
-
-    def count(self, doc):
-        sub_sent_punct = [sent for sent in doc.sents if any(token.pos_ == "SCONJ" for token in sent)]
-        join_sents = itertools.chain(*sub_sent_punct)
-        sent_tok = [tkn for tkn in join_sents if tkn.pos_ in "PUNCT"]
-
-        result = incidence(doc, sent_tok)
-        return result, {"SUBORD_SENT_PUNCT": sent_tok}
 
+class SY_QUOTATIONS(Metric):
+    category = Syntactic
+    name_en = "Number of words in sentences with quotation marks"
+
+    def count(doc):
+        sent = [sent for sent in doc.sents for token in sent if token.text == '"' or token.text == "'"]
+        result = incidence(doc, sent)
+        return result, {}
 
-class SY_COORD_SENT(Syntactic):
-    name_en = "Words in coordinate sentences incidence"
-    metric_id = 6
 
-    def count(self, doc):
-        coord_sentences = [sent for sent in doc.sents if any(token.pos_ == "CCONJ" for token in sent)]
-        join_sents = itertools.chain(*coord_sentences)
-        sent_tok = [tkn for tkn in join_sents if tkn.pos_ != "PUNCT"]
+class SY_EXCLAMATION(Metric):
+    category = Syntactic
+    name_en = "Number of words in exclamatory sentences"
+
+    def count(doc):
+        sent = [sent for sent in doc.sents for token in sent if token.text == "!"]
+        result = incidence(doc, sent)
+        return result, {}
 
-        result = incidence(doc, sent_tok)
-        return result, {"COORD": sent_tok}
 
+class SY_QUESTION(Metric):
+    category = Syntactic
+    name_en = "Number of words in interrogative sentences"
+
+    def count(doc):
+        sent = [sent for sent in doc.sents for token in sent if token.text == "?"]
+        result = incidence(doc, sent)
+        return result, {}
 
-class SY_COORD_SENT_PUNCT(Syntactic):
-    name_en = "Punctuation in coordinate sentences incidence"
-    metric_id = 7
+class SY_ELLIPSES(Metric):
+    category = Syntactic
+    name_en = "Number of words in elliptic sentences"
+
+    def count(doc):
+        sents = [sent for sent in doc.sents for token in sent if token.dep_ == "orphan"]
+        result = incidence(doc, sents)
+        return result, {}
 
-    def count(self, doc):
-        coord_sent_punct = [sent for sent in doc.sents if any(token.pos_ == "CCONJ" for token in sent)]
-        join_sents = itertools.chain(*coord_sent_punct)
-        sent_tok = [tkn for tkn in join_sents if tkn.pos_ in "PUNCT"]
 
-        result = incidence(doc, sent_tok)
-        return result, {"COORD_PUNCT": sent_tok}
+class SY_POSITIONING(Metric):
+    category = Syntactic
+    name_en = "Number of positionings (прикладка)"
+
+    def count(doc):
+        tokens = []
+        matcher = Matcher(doc.vocab)
+        pattern = [{"POS": "ADJ"}, {"MORPH": {"IS_SUBSET": ["PunctType=Dash"]}}, {"POS": "NOUN"}]
+        matcher.add("positioning", [pattern])
+        matches = matcher(doc)
+        for match_id, start, end in matches:
+            tokens.append(doc[start:end])
+        result = incidence(doc, tokens)
+        return result, {}
 
 
-class SY_SIMPLE_SENT(Syntactic):
-    name_en = "Tokens in simple sentences incidence"
-    metric_id = 8
+class SY_CONDITIONAL(Metric):
+    category = Syntactic
+    name_en = "Number of words in conditional sentences"
+
+    def count(doc):
+        tokens = [[token, token.head] for token in doc if token.dep_ == "aux" and "Mood=Cnd" in token.morph]
+        flatten = [token for i in tokens for token in i]
+        result = incidence(doc, flatten)
+        return result, {}
 
-    def count(self, doc):
-        sentence_tokens = [[sent for token in sent if token.pos_ == "SCONJ" or token.pos_ == "CCONJ"] for sent in
-                           doc.sents]
-        flattened = [val for sublist in sentence_tokens for val in sublist]
-        simple_sent = [[token for token in sent] for sent in doc.sents if
-                       sent not in flattened]
-        flattened_simple = [val for sublist in simple_sent for val in sublist]
 
-        result = incidence(doc, flattened_simple)
+class SY_IMPERATIVE(Metric):
+    category = Syntactic
+    name_en = "Number of words in imperative sentences"
+
+    def count(doc):
+        tokens = [sent for sent in doc.sents for token in sent if "Mood=Imp" in token.morph and token.pos_ == "VERB"]
+        result = incidence(doc, tokens)
         return result, {}
 
 
-class SY_DIRECT_SPEECH(Syntactic):
-    name_en = "Number of words in direct speech"
-    metric_id = 9
-
-    def count(self, doc):
-        start, end = start_end_quote(doc)
-        if (start and end) != None:
-            span = doc[start:end]
-            span_words = [token for token in span]
-            result = incidence(doc, span_words)
-            return result, {"Direct Speech": span_words}
-        else:
-            result = ratio(len(doc), 0)
-            return result, {}
+class SY_AMPLIFIED_SENT(Metric):
+    category = Syntactic
+    name_en = "Number of words in amplified sentences"
+
+    def count(doc):
+        tokens = [sent for sent in doc.sents if sent.text[-2:] == "?!"]
+        result = incidence(doc, tokens)
+        return result, {}
 
 
-SYNTACTIC = [
-    SY_QUESTION,
-    SY_EXCLAMATION,
-    SY_IMPERATIVE,
-    SY_SUBORD_SENT,
-    SY_SUBORD_SENT_PUNCT,
-    SY_COORD_SENT,
-    SY_COORD_SENT_PUNCT,
-    SY_SIMPLE_SENT,
-    SY_DIRECT_SPEECH,
-]
+class SY_NOUN_PHRASES(Metric):
+    category = Syntactic
+    name_en = "Number of noun phrases"
+
+    def count(doc):
+        tags_ = ["NOUN", "PROPN"]
+        dep = ["nmod", "amod", "discourse", "case"]
+        noun_phrases = []
+
+        for sent in doc.sents:
+            # noun phrases without any modifiers
+            subjects = [noun_phrases.append([[token.text]]) for token in sent if token.dep_ in ["nsubj", "nsubjpass"] and len([*token.children]) == 0]
+            # noun phrases with modifiers
+            chunks = []
+            for token in sent:
+                if token.pos_ in tags_ and len([*token.children]) > 0:
+                    ph = []
+                    for child in token.children:
+                        if child.dep_ in dep and child.head.text not in ph:
+                            ph.append(child.head.text)
+                            ph.append(child.text)
+                        elif child.dep_ in dep and child.head.text in ph:
+                            ph.append(child.text)
+                            
+                    chunks.append(ph)
+            noun_phrases.append(chunks)
+        flatten_np = list(itertools.chain(*noun_phrases))
+        result = ratio(len(flatten_np), len(doc))
+        debug = {"Noun Phrases": flatten_np}
 
-syntactic_group = MetricsGroup([m() for m in SYNTACTIC])
+        return result, debug
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/en/verb_tenses_en.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/en/verb_tenses_en.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,384 +10,364 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
+from stylo_metrix.structures import Metric, Category
 
-from stylo_metrix.metrics.en.en import EnglishMetric
-from stylo_metrix.structures import MetricsGroup
 from stylo_metrix.utils import incidence
 
 
-class Verb_Tenses(EnglishMetric, ABC):
-    category_en = "Verbs Tenses"
-    category_id = 3
+class VerbTenses(Category):
+    lang = 'en'
+    name_en = "Verbs Tenses"
 
 
-class VT_PRESENT_ACTIVE(Verb_Tenses):
-    name_en = "Present Tenses Active"
-    metric_id = 1
+class VT_PRESENT_ACTIVE(Metric):
+    category = VerbTenses
+    name_en = "Present tenses active"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["present_simple", "present_ind_3p",
                       "present_cont", "present_perfect",
                       "present_perfect_cont"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_PASSIVE(Verb_Tenses):
-    name_en = "Present Tenses Passive"
-    metric_id = 2
+class VT_PRESENT_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present tenses passive"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["present_ind_passive", "present_cont_passive",
                       "present_perfect_passive"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_ACTIVE(Verb_Tenses):
-    name_en = "Past Tenses Active"
-    metric_id = 3
+class VT_PAST_ACTIVE(Metric):
+    category = VerbTenses
+    name_en = "Past tenses active"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["past_simple", "past_ind_be",
                       "past_cont", "past_perf", "past_perf_cont"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_PASSIVE(Verb_Tenses):
-    name_en = "Past Tenses Passive"
-    metric_id = 4
+class VT_PAST_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Past tenses passive"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["past_ind_passive", "past_cont_passive", "past_perf_passive"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_ACTIVE(Verb_Tenses):
-    name_en = "Future Tenses Active"
-    metric_id = 5
+class VT_FUTURE_ACTIVE(Metric):
+    category = VerbTenses
+    name_en = "Future tenses active"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["future_simple", "future_progr", "future_perfect", "future_perfect_cont"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PASSIVE(Verb_Tenses):
-    name_en = "Future Tenses Passive"
-    metric_id = 6
+class VT_FUTURE_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Future tenses passive"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["future_simple_passive", "future_progr_passive", "future_perf_passive"]
         search = [token for token in doc if token._.verb_tense in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_MODALS_ACTIVE(Verb_Tenses):
-    name_en = "Modal Verbs Active"
-    metric_id = 7
+class VT_MODALS_ACTIVE(Metric):
+    category = VerbTenses
+    name_en = "Modal verbs active"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["would_ind_active", "would_cont", "would_perf_active",
                       "should_ind_active", "shall_ind_active", "should_cont", "should_perf_active",
                       "must_ind_active", "must_cont", "must_perf_active", "can_ind", "could_ind",
                       "can_cont", "could_cont", "could_perf", "may_ind", "might_ind", "may_cont",
                       "might_perf"]
         search = [token for token in doc if token._.modal_verbs in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_MODALS_PASSIVE(Verb_Tenses):
-    name_en = "Modal Verbs Active"
-    metric_id = 8
+class VT_MODALS_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Modal verbs active"
 
-    def count(self, doc):
+    def count(doc):
         label_list = ["would_ind_passive", "would_perf_passive", "should_ind_passive",
                       "shall_ind_passive", "should_perf_passive", "must_ind_passive",
                       "must_perf_passive", "can_ind_passive", "could_ind_passive", "could_perf_passive",
                       "may_ind_passive", "might_ind_passive", "might_perf_passive", "may_perf_passive"]
         search = [token for token in doc if token._.modal_verbs in label_list]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_SIMPLE(Verb_Tenses):
-    name_en = "Present Simple Tense Incidence"
-    metric_id = 9
+class VT_PRESENT_SIMPLE(Metric):
+    category = VerbTenses
+    name_en = "Present Simple tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_simple"]
         result = incidence(doc, search)
+        debug = {'TOKENS': search}
+        return result, debug
 
-        return result, {}
 
+class VT_PRESENT_PROGRESSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present Continuous tense"
 
-class VT_PRESENT_SIMPLE_3DPERSN(Verb_Tenses):
-    name_en = "Present Simple 3rd Person Incidence"
-    metric_id = 10
-
-    def count(self, doc):
-        search = [token for token in doc if token._.verb_tense == "present_ind_3p"]
-        result = incidence(doc, search)
-        return result, {}
-
-
-class VT_PRESENT_PROGRESSIVE(Verb_Tenses):
-    name_en = "Present Continuous Tense Incidence"
-    metric_id = 11
-
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_cont"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_PERFECT(Verb_Tenses):
-    name_en = "Present Perfect Tense Incidence"
-    metric_id = 12
+class VT_PRESENT_PERFECT(Metric):
+    category = VerbTenses
+    name_en = "Present Perfect tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_perfect"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_PERFECT_PROGR(Verb_Tenses):
-    name_en = "Present Prefect Continuous Tense Incidence"
-    metric_id = 13
+class VT_PRESENT_PERFECT_PROGR(Metric):
+    category = VerbTenses
+    name_en = "Present Prefect Continuous tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_perfect_cont"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_SIMPLE_PASSIVE(Verb_Tenses):
-    name_en = "Present Simple Passive Incidence"
-    metric_id = 14
+class VT_PRESENT_SIMPLE_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present Simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_ind_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_PROGR_PASSIVE(Verb_Tenses):
-    name_en = "Present Continuous Passive Incidence"
-    metric_id = 15
+class VT_PRESENT_PROGR_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present Continuous passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_cont_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PRESENT_PERFECT_PASSIVE(Verb_Tenses):
-    name_en = "Present Perfect Passive Incidence"
-    metric_id = 16
+class VT_PRESENT_PERFECT_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present Perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "present_perfect_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_SIMPLE(Verb_Tenses):
-    name_en = "Past Simple Tense Incidence"
-    metric_id = 17
+class VT_PAST_SIMPLE(Metric):
+    category = VerbTenses
+    name_en = "Past Simple tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_simple"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_SIMPLE_BE(Verb_Tenses):
-    name_en = "Past Simple  Incidence'to be'"
-    metric_id = 18
+class VT_PAST_SIMPLE_BE(Metric):
+    category = VerbTenses
+    name_en = "Past Simple 'to be' verb"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_ind_be"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_PROGR(Verb_Tenses):
-    name_en = "Past Continuous Tense Incidence"
-    metric_id = 19
+class VT_PAST_PROGR(Metric):
+    category = VerbTenses
+    name_en = "Past Continuous tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_cont"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_PERFECT(Verb_Tenses):
-    name_en = "Past Perfect Tense Incidence"
-    metric_id = 20
+class VT_PAST_PERFECT(Metric):
+    category = VerbTenses
+    name_en = "Past Perfect tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_perf"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_PERFECT_PROGR(Verb_Tenses):
-    name_en = "Past Perfect Continuous Tense Incidence"
-    metric_id = 21
+class VT_PAST_PERFECT_PROGR(Metric):
+    category = VerbTenses
+    name_en = "Past Perfect Continuous tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_perf_cont"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_SIMPLE_PASSIVE(Verb_Tenses):
-    name_en = "Past Simple Passive Incidence"
-    metric_id = 22
+class VT_PAST_SIMPLE_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Past Simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_ind_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_POGR_PASSIVE(Verb_Tenses):
-    name_en = "Past Continuous Passive Incidence"
-    metric_id = 23
+class VT_PAST_POGR_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Past Continuous passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_cont_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_PAST_PERFECT_PASSIVE(Verb_Tenses):
-    name_en = "Past Perfect Passive Incidence"
-    metric_id = 24
+class VT_PAST_PERFECT_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Past Perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "past_perf_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_SIMPLE(Verb_Tenses):
-    name_en = "Future Simple Tense Incidence"
-    metric_id = 25
+class VT_FUTURE_SIMPLE(Metric):
+    category = VerbTenses
+    name_en = "Future Simple tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_simple"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PROGRESSIVE(Verb_Tenses):
-    name_en = "Future Continuous Tense Incidence"
-    metric_id = 26
+class VT_FUTURE_PROGRESSIVE(Metric):
+    category = VerbTenses
+    name_en = "Future Continuous tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_progr"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PERFECT(Verb_Tenses):
-    name_en = "Future Perfect Tense Incidence"
-    metric_id = 27
+class VT_FUTURE_PERFECT(Metric):
+    category = VerbTenses
+    name_en = "Future Perfect tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_perfect"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PERFECT_PROGR(Verb_Tenses):
-    name_en = "Future Perfect Continuous Incidence"
-    metric_id = 28
+class VT_FUTURE_PERFECT_PROGR(Metric):
+    category = VerbTenses
+    name_en = "Future Perfect Continuous tense"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_perfect_cont"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_SIMPLE_PASSIVE(Verb_Tenses):
-    name_en = "Future Simple Passive Incidence"
-    metric_id = 29
+class VT_FUTURE_SIMPLE_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Future Simple passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_simple_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PROGR_PASSIVE(Verb_Tenses):
-    name_en = "Future Continuous Passive Incidence"
-    metric_id = 30
+class VT_FUTURE_PROGR_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Future Continuous passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_progr_passive"]
         result = incidence(doc, search)
-        return result, {}
+        debug = {'TOKENS': search}
+        return result, debug
 
 
-class VT_FUTURE_PERFECT_PASSIVE(Verb_Tenses):
-    name_en = "Present Perfect Passive Incidence"
-    metric_id = 31
+class VT_FUTURE_PERFECT_PASSIVE(Metric):
+    category = VerbTenses
+    name_en = "Present Perfect passive"
 
-    def count(self, doc):
+    def count(doc):
         search = [token for token in doc if token._.verb_tense == "future_perf_passive"]
         result = incidence(doc, search)
-        return result, {}
-
-
-TENSES = [
-    VT_PRESENT_ACTIVE,
-    VT_PRESENT_PASSIVE,
-    VT_PAST_ACTIVE,
-    VT_PAST_PASSIVE,
-    VT_FUTURE_ACTIVE,
-    VT_FUTURE_PASSIVE,
-    VT_MODALS_ACTIVE,
-    VT_MODALS_PASSIVE,
-    VT_PRESENT_SIMPLE,
-    VT_PRESENT_SIMPLE_3DPERSN,
-    VT_PRESENT_PROGRESSIVE,
-    VT_PRESENT_PERFECT,
-    VT_PRESENT_PERFECT_PROGR,
-    VT_PRESENT_SIMPLE_PASSIVE,
-    VT_PRESENT_PROGR_PASSIVE,
-    VT_PRESENT_PERFECT_PASSIVE,
-    VT_PAST_SIMPLE,
-    VT_PAST_SIMPLE_BE,
-    VT_PAST_PROGR,
-    VT_PAST_PERFECT,
-    VT_PAST_PERFECT_PROGR,
-    VT_PAST_SIMPLE_PASSIVE,
-    VT_PAST_POGR_PASSIVE,
-    VT_PAST_PERFECT_PASSIVE,
-    VT_FUTURE_SIMPLE,
-    VT_FUTURE_PROGRESSIVE,
-    VT_FUTURE_PERFECT,
-    VT_FUTURE_PERFECT_PROGR,
-    VT_FUTURE_SIMPLE_PASSIVE,
-    VT_FUTURE_PROGR_PASSIVE,
-    VT_FUTURE_PERFECT_PASSIVE,
-]
-
-verb_tenses_group = MetricsGroup([m() for m in TENSES])
+        debug = {'TOKENS': search}
+        return result, debug
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/inflection.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/inflection.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,601 +10,707 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
+from stylo_metrix.structures import Metric, Category
 
-from stylo_metrix.metrics.pl.pl import PolishMetric
-from stylo_metrix.structures import Metric, MetricsGroup
-from stylo_metrix.utils import incidence, select
+from stylo_metrix.utils import incidence, select, ratio
 
 
-class Inflection(PolishMetric, ABC):
-    category_local = "Inflection"
-    category_en = "Fleksja"
-    category_id = 2
-
-
-class IN_V_INF(Inflection):
-    name_en = "Infinitives incidence"
-    name_local = "Występowanie czasowników w bezokoliczniku"
-    metric_id = 1
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_inflection': 'inf'}))
-        return result, {}
-
-
-class IN_V_INFL(Inflection):
-    name_en = "Inflected verb incidence"
-    name_local = "Występowanie czasowników w formie osobowej"
-    metric_id = 2
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_inflection': 'infl'}))
-        return result, {}
-
-
-VERBS_INFLECTION = [
-    IN_V_INF,
-    IN_V_INFL,
-]
-
-
-class IN_V_1S(Inflection):
-    name_en = "First person singular verb incidence"
-    name_local = "Występowanie czasowników w 1. os. l. poj."
-    metric_id = 3
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 's1'}))
-        return result, {}
-
-
-class IN_V_1P(Inflection):
-    name_en = "First person plural verb incidence"
-    name_local = "Występowanie czasowników w 1. os. l. mn."
-    metric_id = 4
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 'p1'}))
-        return result, {}
-
-
-class IN_V_2S(Inflection):
-    name_en = "Second person singular verb incidence"
-    name_local = "Występowanie czasowników w 2. os. l. poj."
-    metric_id = 5
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 's2'}))
-        return result, {}
-
-
-class IN_V_2P(Inflection):
-    name_en = "Second person plural verb incidence"
-    name_local = "Występowanie czasowników w 2. os. l. mn."
-    metric_id = 6
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 'p2'}))
-        return result, {}
-
-
-class IN_V_3S(Inflection):
-    name_en = "Third person singular verb incidence"
-    name_local = "Występowanie czasowników w 3. os. l. poj."
-    metric_id = 7
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 's3'}))
-        return result, {}
-
-
-class IN_V_3P(Inflection):
-    name_en = "Third person plural verb incidence"
-    name_local = "Występowanie czasowników w 3. os. l. mn."
-    metric_id = 8
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_person': 'p3'}))
-        return result, {}
-
-
-VERBS_PERSONS = [
-    IN_V_1S,
-    IN_V_1P,
-    IN_V_2S,
-    IN_V_2P,
-    IN_V_3S,
-    IN_V_3P,
-]
-
-
-class IN_V_PAST(Inflection):
-    name_en = "Verbs in past tense incidence"
-    name_local = "Występowanie czasowników w czasie przeszłym"
-    metric_id = 9
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_tense': 'past'}))
-        return result, {}
-
-
-class IN_V_PRES(Inflection):
-    name_en = "Verbs in present tense incidence"
-    name_local = "Występowanie czasowników w czasie teraźniejszym"
-    metric_id = 10
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_tense': 'pres'}))
-        return result, {}
-
-
-class IN_V_FUT(Inflection):
-    name_en = "Verbs in future tense incidence"
-    name_local = "Występowanie czasowników w czasie przyszłym"
-    metric_id = 11
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_tense': 'fut'}))
-        return result, {}
-
-
-class IN_V_FUTS(Inflection):
-    name_en = "Verbs in future simple tense incidence"
-    name_local = "Występowanie czasowników w czasie przyszłym prostym"
-    metric_id = 12
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_future': 'futs'}))
-        return result, {}
-
-
-class IN_V_FUTC(Inflection):
-    name_en = "Verbs in future complex tense incidence"
-    name_local = "Występowanie czasowników w czasie przyszłym złożonym"
-    metric_id = 13
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_future': 'futc'}))
-        return result, {}
-
-
-VERBS_TENSES = [
-    IN_V_PAST,
-    IN_V_PRES,
-    IN_V_FUT,
-    IN_V_FUTS,
-    IN_V_FUTC,
-]
-
-
-class IN_V_PERF(Inflection):
-    name_en = "Verbs in perfective aspect incidence"
-    name_local = "Występowanie czasowników w aspekcie dokonanym"
-    metric_id = 14
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_aspect': 'perf'}))
-        return result, {}
-
-
-class IN_V_IMPERF(Inflection):
-    name_en = "Verbs in imperfective aspect incidence"
-    name_local = "Występowanie czasowników w aspekcie niedokonanym"
-    metric_id = 15
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_aspect': 'imperf'}))
-        return result, {}
+class Inflection(Category):
+    lang = 'pl'
+    name_en = "Inflection"
+    name_local = "Fleksja"
+
+
+class IN_V_INF(Metric):
+    category = Inflection
+    name_en = "Infinitives"
+    name_local = "Czasowniki w bezokoliczniku"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_inflection': 'inf'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_INFL(Metric):
+    category = Inflection
+    name_en = "Inflected verbs"
+    name_local = "Czasowniki w formie osobowej"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_inflection': 'infl'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+    
+
+class IN_V_QUASI(Metric):
+    category = Inflection
+    name_en = "Quasi-verbs"
+    name_local = "Quasi-czasowniki"
+
+    def count(doc):
+        quasi = list(token.text for token in doc if str(token.morph.get('VerbType')) =='[\'Quasi\']')
+        result = ratio(len(quasi), doc._.n_tokens)
+        debug = {'TOKENS': quasi}
+        return result, debug
+
+
+# VERBS_INFLECTION = [
+#     IN_V_INF,
+#     IN_V_INFL,
+#     IN_V_QUASI,
+# ]
+
+
+class IN_V_1S(Metric):
+    category = Inflection
+    name_en = "First person singular verbs"
+    name_local = "Czasowniki w 1. os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 's1'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_1P(Metric):
+    category = Inflection
+    name_en = "First person plural verbs"
+    name_local = "Czasowniki w 1. os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 'p1'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_2S(Metric):
+    category = Inflection
+    name_en = "Second person singular verbs"
+    name_local = "Czasowniki w 2. os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 's2'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_2P(Metric):
+    category = Inflection
+    name_en = "Second person plural verbs"
+    name_local = "Czasowniki w 2. os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 'p2'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_3S(Metric):
+    category = Inflection
+    name_en = "Third person singular verbs"
+    name_local = "Czasowniki w 3. os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 's3'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_3P(Metric):
+    category = Inflection
+    name_en = "Third person plural verbs"
+    name_local = "Czasowniki w 3. os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_person': 'p3'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# VERBS_PERSONS = [
+#     IN_V_1S,
+#     IN_V_1P,
+#     IN_V_2S,
+#     IN_V_2P,
+#     IN_V_3S,
+#     IN_V_3P,
+# ]
+
+
+class IN_V_PAST(Metric):
+    category = Inflection
+    name_en = "Verbs in past tense"
+    name_local = "Czasowniki w czasie przeszłym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_tense': 'past'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_PRES(Metric):
+    category = Inflection
+    name_en = "Verbs in present tense"
+    name_local = "Czasowniki w czasie teraźniejszym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_tense': 'pres'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_FUT(Metric):
+    category = Inflection
+    name_en = "Verbs in future tense"
+    name_local = "Czasowniki w czasie przyszłym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_tense': 'fut'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_FUTS(Metric):
+    category = Inflection
+    name_en = "Verbs in future simple tense"
+    name_local = "Czasowniki w czasie przyszłym prostym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_future': 'futs'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_FUTC(Metric):
+    category = Inflection
+    name_en = "Verbs in future complex tense"
+    name_local = "Czasowniki w czasie przyszłym złożonym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_future': 'futc'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# VERBS_TENSES = [
+#     IN_V_PAST,
+#     IN_V_PRES,
+#     IN_V_FUT,
+#     IN_V_FUTS,
+#     IN_V_FUTC,
+# ]
+
+
+class IN_V_PERF(Metric):
+    category = Inflection
+    name_en = "Verbs in perfective aspect"
+    name_local = "Czasowniki w aspekcie dokonanym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_aspect': 'perf'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_IMPERF(Metric):
+    category = Inflection
+    name_en = "Verbs in imperfective aspect"
+    name_local = "Czasowniki w aspekcie niedokonanym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_aspect': 'imperf'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
 
 
 VERBS_ASPECTS = [
     IN_V_PERF,
     IN_V_IMPERF,
 ]
 
 
-class IN_V_IMP(Inflection):
-    name_en = "Verbs in imperative mood incidence"
-    name_local = "Występowanie czasowników w trybie rozkazującym"
-    metric_id = 16
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_voice': 'impt'}))
-        return result, {}
-
-
-class IN_V_COND(Inflection):
-    name_en = "Verbs in conditional mood incidence"
-    name_local = "Występowanie czasowników w trybie przypuszczającym"
-    metric_id = 17
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'verb_voice': 'cond'}))
-        return result, {}
-
-
-VERBS_MOODS = [
-    IN_V_IMP,
-    IN_V_COND,
-]
-
-
-class IN_V_PCON(Inflection):
-    name_en = "Present adverbial participles incidence"
-    name_local = "Występowanie imiesłowów przysłówkowych współczesnych"
-    metric_id = 18
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'participle_type': 'pcon'}))
-        return result, {}
-
-
-class IN_V_PANT(Inflection):
-    name_en = "Perfect adverbial participles incidence"
-    name_local = "Występowanie imiesłowów przysłówkowych uprzednich"
-    metric_id = 19
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'participle_type': 'pant'}))
-        return result, {}
-
-
-class IN_V_PACT(Inflection):
-    name_en = "Active adjectival participles incidence"
-    name_local = "Występowanie imiesłowów przymiotnikowych czynnych"
-    metric_id = 20
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'participle_type': 'pact'}))
-        return result, {}
+class IN_V_IMP(Metric):
+    category = Inflection
+    name_en = "Verbs in imperative mood"
+    name_local = "Czasowniki w trybie rozkazującym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_voice': 'impt'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_COND(Metric):
+    category = Inflection
+    name_en = "Verbs in conditional mood"
+    name_local = "Czasowniki w trybie przypuszczającym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'verb_voice': 'cond'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# VERBS_MOODS = [
+#     IN_V_IMP,
+#     IN_V_COND,
+# ]
+
+class IN_V_ACT(Metric):
+    category = Inflection
+    name_en = "Verbs in active voice"
+    name_local = "Czasowniki w stronie czynnej"
+
+    def count(doc):
+        actives = list(token.text for token in doc if str(token.morph.get('Voice'))=='[\'Act\']')
+        debug = {"VALUES": actives}
+        return ratio(len(actives), doc._.n_tokens), debug
+
+class IN_V_PASS(Metric):
+    category = Inflection
+    name_en = "Verbs in passive voice"
+    name_local = "Czasowniki w stronie biernej"
+
+    def count(doc):
+        passives = list(token.text for token in doc if str(token.morph.get('Voice'))=='[\'Pass\']')
+        debug = {"VALUES": passives}
+        return ratio(len(passives), doc._.n_tokens), debug
+
+# VERBS_VOICES = [
+#     IN_V_ACT,
+#     IN_V_PASS,
+# ]
+
+class IN_V_PCON(Metric):
+    category = Inflection
+    name_en = "Present adverbial participles"
+    name_local = "Imiesłowy przysłówkowe współczesne"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'participle_type': 'pcon'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_PANT(Metric):
+    category = Inflection
+    name_en = "Perfect adverbial participles"
+    name_local = "Imiesłowy przysłówkowe uprzednie"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'participle_type': 'pant'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_PACT(Metric):
+    category = Inflection
+    name_en = "Active adjectival participles"
+    name_local = "Imiesłowy przymiotnikowe czynne"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'participle_type': 'pact'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_V_PPAS(Metric):
+    category = Inflection
+    name_en = "Passive adjectival participles"
+    name_local = "Imiesłowy przymiotnikowe bierne (przeszłe)"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v', 'participle_type': 'ppas'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# VERBS_PARTICIPLES = [
+#     IN_V_PCON,
+#     IN_V_PANT,
+#     IN_V_PACT,
+#     IN_V_PPAS,
+# ]
+
+
+class IN_V_GER(Metric):
+    category = Inflection
+    name_en = "Gerunds"
+    name_local = "Rzeczowniki odczasownikowe"
+
+
+    def count(doc):
+        selection = select(doc, {'pos': 'n', 'noun_type': 'ger'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# VERBS_DERIVATION = [
+#     IN_V_GER,
+# ]
+
+
+class Nouns:
+    @classmethod
+    def count(cls, doc):
+        selection = select(doc, {'pos': 'n', 'case': cls.case})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
 
 
-class IN_V_PPAS(Inflection):
-    name_en = "Passive adjectival participles incidence"
-    name_local = "Występowanie imiesłowów przymiotnikowych biernych (przeszłych)"
-    metric_id = 21
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'v', 'participle_type': 'ppas'}))
-        return result, {}
-
-
-VERBS_PARTICIPLES = [
-    IN_V_PCON,
-    IN_V_PANT,
-    IN_V_PACT,
-    IN_V_PPAS,
-]
-
-
-class IN_V_GER(Inflection):
-    name_en = "Gerunds incidence"
-    name_local = "Występowanie rzeczowników odczasownikowych"
-    metric_id = 22
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'n', 'noun_type': 'ger'}))
-        return result, {}
-
-
-VERBS_DERIVATION = [
-    IN_V_GER,
-]
-
-
-class Nouns(Inflection, ABC):
-    case = ""
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'n', 'case': self.__class__.case}))
-        return result, {}
-
-
-class IN_N_1M(Nouns):
+class IN_N_1M(Metric, Nouns):
+    category = Inflection
     case = "nom"
-    name_en = "Nouns in nominative case incidence"
-    name_local = "Występowanie rzeczowników w mianowniku"
-    metric_id = 23
+    name_en = "Nouns in nominative case"
+    name_local = "Rzeczowniki w mianowniku"
 
 
-class IN_N_2D(Nouns):
+class IN_N_2D(Metric, Nouns):
+    category = Inflection
     case = "gen"
-    name_en = "Nouns in genitive case incidence"
-    name_local = "Występowanie rzeczowników w dopełniaczu"
-    metric_id = 24
+    name_en = "Nouns in genitive case"
+    name_local = "Rzeczowniki w dopełniaczu"
 
 
-class IN_N_3C(Nouns):
+class IN_N_3C(Metric, Nouns):
+    category = Inflection
     case = "dat"
-    name_en = "Nouns in dative case incidence"
-    name_local = "Występowanie rzeczowników w celowniku"
-    metric_id = 25
+    name_en = "Nouns in dative case"
+    name_local = "Rzeczowniki w celowniku"
 
 
-class IN_N_4B(Nouns):
+class IN_N_4B(Metric, Nouns):
+    category = Inflection
     case = "acc"
-    name_en = "Nouns in accusative case incidence"
-    name_local = "Występowanie rzeczowników w bierniku"
-    metric_id = 26
+    name_en = "Nouns in accusative case"
+    name_local = "Rzeczowniki w bierniku"
 
 
-class IN_N_5MSC(Nouns):
+class IN_N_5MSC(Metric, Nouns):
+    category = Inflection
     case = "inst"
-    name_en = "Nouns in instrumental case incidence"
-    name_local = "Występowanie rzeczowników w narzędniku"
-    metric_id = 27
+    name_en = "Nouns in instrumental case"
+    name_local = "Rzeczowniki w narzędniku"
 
 
-class IN_N_6N(Nouns):
+class IN_N_6N(Metric, Nouns):
+    category = Inflection
     case = "loc"
-    name_en = "Nouns in locative case incidence"
-    name_local = "Występowanie rzeczowników w miejscowniku"
-    metric_id = 28
+    name_en = "Nouns in locative case"
+    name_local = "Rzeczowniki w miejscowniku"
 
 
-class IN_N_7W(Nouns):
+class IN_N_7W(Metric, Nouns):
+    category = Inflection
     case = "voc"
-    name_en = "Nouns in vocative case incidence"
-    name_local = "Występowanie rzeczowników w wołaczu"
-    metric_id = 29
-
-
-NOUNS_CASES = [
-    IN_N_1M,
-    IN_N_2D,
-    IN_N_3C,
-    IN_N_4B,
-    IN_N_5MSC,
-    IN_N_6N,
-    IN_N_7W,
-]
+    name_en = "Nouns in vocative case"
+    name_local = "Rzeczowniki w wołaczu"
 
 
-class Pronouns(Inflection, ABC):
-    case = ""
-    name_en = ""
-    name_local = "Zaimki w przypadku " + case
+# NOUNS_CASES = [
+#     IN_N_1M,
+#     IN_N_2D,
+#     IN_N_3C,
+#     IN_N_4B,
+#     IN_N_5MSC,
+#     IN_N_6N,
+#     IN_N_7W,
+# ]
+
+
+class Pronouns:
+    @classmethod
+    def count(cls, doc):
+        selection = select(doc, {'pos': 'pro', 'case': cls.case})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
 
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'case': self.__class__.case}))
-        return result, {}
 
-
-class IN_PRO_1M(Pronouns):
+class IN_PRO_1M(Metric, Pronouns):
+    category = Inflection
     case = "nom"
-    name_en = "Pronouns in nominative case incidence"
-    name_local = "Występowanie zaimków w mianowniku"
-    metric_id = 30
+    name_en = "Pronouns in nominative case"
+    name_local = "Zaimki w mianowniku"
 
 
-class IN_PRO_2D(Pronouns):
+class IN_PRO_2D(Metric, Pronouns):
+    category = Inflection
     case = "gen"
-    name_en = "Pronouns in genitive case incidence"
-    name_local = "Występowanie zaimków w dopełniaczu"
-    metric_id = 31
+    name_en = "Pronouns in genitive case"
+    name_local = "Zaimki w dopełniaczu"
 
 
-class IN_PRO_3C(Pronouns):
+class IN_PRO_3C(Metric, Pronouns):
+    category = Inflection
     case = "dat"
-    name_en = "Pronouns in dative case incidence"
-    name_local = "Występowanie zaimków w celowniku"
-    metric_id = 32
+    name_en = "Pronouns in dative case"
+    name_local = "Zaimki w celowniku"
 
 
-class IN_PRO_4B(Pronouns):
+class IN_PRO_4B(Metric, Pronouns):
+    category = Inflection
     case = "acc"
-    name_en = "Pronouns in accusative case incidence"
-    name_local = "Występowanie zaimków w bierniku"
-    metric_id = 33
+    name_en = "Pronouns in accusative case"
+    name_local = "Zaimki w bierniku"
 
 
-class IN_PRO_5MSC(Pronouns):
+class IN_PRO_5MSC(Metric, Pronouns):
+    category = Inflection
     case = "inst"
-    name_en = "Pronouns in instrumental case incidence"
-    name_local = "Występowanie zaimków w narzędniku"
-    metric_id = 34
+    name_en = "Pronouns in instrumental case"
+    name_local = "Zaimki w narzędniku"
 
 
-class IN_PRO_6N(Pronouns):
+class IN_PRO_6N(Metric, Pronouns):
+    category = Inflection
     case = "loc"
-    name_en = "Pronouns in locative case incidence"
-    name_local = "Występowanie zaimków w miejscowniku"
-    metric_id = 35
+    name_en = "Pronouns in locative case"
+    name_local = "Zaimki w miejscowniku"
 
 
-class IN_PRO_7W(Pronouns):
+class IN_PRO_7W(Metric, Pronouns):
+    category = Inflection
     case = "voc"
-    name_en = "Pronouns in vocative case incidence"
-    name_local = "Występowanie zaimków w wołaczu"
-    metric_id = 36
-
-
-PRONOUNS_CASES = [
-    IN_PRO_1M,
-    IN_PRO_2D,
-    IN_PRO_3C,
-    IN_PRO_4B,
-    IN_PRO_5MSC,
-    IN_PRO_6N,
-    IN_PRO_7W,
-]
-
-
-class IN_PRO_1S(Inflection):
-    name_en = "First person singular pronoun incidence"
-    name_local = "Występowanie zaimków w 1 os. l. poj."
-    metric_id = 37
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 's1'}))
-        return result, {}
-
-
-class IN_PRO_1P(Inflection):
-    name_en = "First person plural pronoun incidence"
-    name_local = "Występowanie zaimków w 1 os. l. mn."
-    metric_id = 38
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 'p1'}))
-        return result, {}
-
-
-class IN_PRO_2S(Inflection):
-    name_en = "Second person singular pronoun incidence"
-    name_local = "Występowanie zaimków w 2 os. l. poj."
-    metric_id = 39
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 's2'}))
-        return result, {}
-
-
-class IN_PRO_2P(Inflection):
-    name_en = "Second person plural pronoun incidence"
-    name_local = "Występowanie zaimków w 2 os. l. mn."
-    metric_id = 40
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 'p2'}))
-        return result, {}
+    name_en = "Pronouns in vocative case"
+    name_local = "Zaimki w wołaczu"
 
 
-class IN_PRO_3S(Inflection):
-    name_en = "Third person singular pronoun incidence"
-    name_local = "Występowanie zaimków w 3 os. l. poj."
-    metric_id = 41
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 's3'}))
-        return result, {}
-
-
-class IN_PRO_3P(Inflection):
-    name_en = "Third person plural pronoun incidence"
-    name_local = "Występowanie zaimków w 3 os. l. mn."
-    metric_id = 42
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'pro', 'pronoun_type': 'p3'}))
-        return result, {}
-
-
-PRONOUNS_PERSONS = [
-    IN_PRO_1S,
-    IN_PRO_1P,
-    IN_PRO_2S,
-    IN_PRO_2P,
-    IN_PRO_3S,
-    IN_PRO_3P,
-]
-
-
-class IN_ADJ_POS(Inflection):
-    name_en = "Adjectives in positive degree incidence"
-    name_local = "Występowanie przymiotników w stopniu równym"
-    metric_id = 43
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adj', 'adjective_degree': 'pos'}))
-        return result, {}
-
-
-class IN_ADJ_COM(Inflection):
-    name_en = "Adjectives in comparative degree incidence"
-    name_local = "Występowanie przymiotników w stopniu wyższym"
-    metric_id = 44
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adj', 'adjective_degree': 'com'}))
-        return result, {}
-
-
-class IN_ADJ_SUP(Inflection):
-    name_en = "Adjectives in superlative degree incidence"
-    name_local = "Występowanie przymiotników w stopniu najwyższym"
-    metric_id = 45
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adj', 'adjective_degree': 'sup'}))
-        return result, {}
-
-
-ADJECTIVES_DEGREES = [
-    IN_ADJ_POS,
-    IN_ADJ_COM,
-    IN_ADJ_SUP,
-]
-
-
-class IN_ADV_POS(Inflection):
-    name_en = "Adverbs in positive degree incidence"
-    name_local = "Występowanie przysłówków w stopniu równym"
-    metric_id = 46
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adv', 'adverb_degree': 'pos'}))
-        return result, {}
-
-
-class IN_ADV_COM(Inflection):
-    name_en = "Adverbs in comparative degree incidence"
-    name_local = "Występowanie przysłówków w stopniu wyższym"
-    metric_id = 47
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adv', 'adverb_degree': 'com'}))
-        return result, {}
-
-
-class IN_ADV_SUP(Inflection):
-    name_en = "Adverbs in superlative degree incidence"
-    name_local = "Występowanie przysłówków w stopniu najwyższym"
-    metric_id = 48
-
-    def count(self, doc):
-        result = incidence(doc, select(doc, {'pos': 'adv', 'adverb_degree': 'sup'}))
-        return result, {}
-
-
-ADVERBS_DEGREES = [
-    IN_ADV_POS,
-    IN_ADV_COM,
-    IN_ADV_SUP,
-]
-
-verbs_inflection_group = MetricsGroup([m() for m in VERBS_INFLECTION])
-verbs_persons_group = MetricsGroup([m() for m in VERBS_PERSONS])
-verbs_tenses_group = MetricsGroup([m() for m in VERBS_TENSES])
-verbs_aspects_group = MetricsGroup([m() for m in VERBS_ASPECTS])
-verbs_moods_group = MetricsGroup([m() for m in VERBS_MOODS])
-verbs_participles_group = MetricsGroup([m() for m in VERBS_PARTICIPLES])
-verbs_derivation_group = MetricsGroup([m() for m in VERBS_DERIVATION])
-nouns_cases_group = MetricsGroup([m() for m in NOUNS_CASES])
-pronouns_cases_group = MetricsGroup([m() for m in PRONOUNS_CASES])
-pronouns_persons_group = MetricsGroup([m() for m in PRONOUNS_PERSONS])
-adjectives_degrees_group = MetricsGroup([m() for m in ADJECTIVES_DEGREES])
-adverbs_degrees_group = MetricsGroup([m() for m in ADVERBS_DEGREES])
-
-verbs_group = verbs_inflection_group + \
-              verbs_persons_group + \
-              verbs_tenses_group + \
-              verbs_aspects_group + \
-              verbs_moods_group + \
-              verbs_participles_group + \
-              verbs_derivation_group
-nouns_group = nouns_cases_group
-pronouns_group = pronouns_cases_group + \
-                 pronouns_persons_group
-adjectives_group = adjectives_degrees_group
-adverbs_group = adverbs_degrees_group
-inflection_group = verbs_group + \
-                   nouns_group + \
-                   pronouns_group + \
-                   adjectives_group + \
-                   adverbs_group
+# PRONOUNS_CASES = [
+#     IN_PRO_1M,
+#     IN_PRO_2D,
+#     IN_PRO_3C,
+#     IN_PRO_4B,
+#     IN_PRO_5MSC,
+#     IN_PRO_6N,
+#     IN_PRO_7W,
+# ]
+
+
+class IN_PRO_1S(Metric):
+    category = Inflection
+    name_en = "First person singular pronouns"
+    name_local = "Zaimki w 1 os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 's1'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_PRO_1P(Metric):
+    category = Inflection
+    name_en = "First person plural pronouns"
+    name_local = "Zaimki w 1 os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 'p1'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_PRO_2S(Metric):
+    category = Inflection
+    name_en = "Second person singular pronouns"
+    name_local = "Zaimki w 2 os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 's2'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_PRO_2P(Metric):
+    category = Inflection
+    name_en = "Second person plural pronouns"
+    name_local = "Zaimki w 2 os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 'p2'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_PRO_3S(Metric):
+    category = Inflection
+    name_en = "Third person singular pronouns"
+    name_local = "Zaimki w 3 os. l. poj."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 's3'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_PRO_3P(Metric):
+    category = Inflection
+    name_en = "Third person plural pronouns"
+    name_local = "Zaimki w 3 os. l. mn."
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 'p3'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# PRONOUNS_PERSONS = [
+#     IN_PRO_1S,
+#     IN_PRO_1P,
+#     IN_PRO_2S,
+#     IN_PRO_2P,
+#     IN_PRO_3S,
+#     IN_PRO_3P,
+# ]
+
+
+class IN_ADJ_POS(Metric):
+    category = Inflection
+    name_en = "Adjectives in positive degree"
+    name_local = "Przymiotniki w stopniu równym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adj', 'adjective_degree': 'pos'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_ADJ_COM(Metric):
+    category = Inflection
+    name_en = "Adjectives in comparative degree"
+    name_local = "Przymiotniki w stopniu wyższym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adj', 'adjective_degree': 'com'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_ADJ_SUP(Metric):
+    category = Inflection
+    name_en = "Adjectives in superlative degree"
+    name_local = "Przymiotniki w stopniu najwyższym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adj', 'adjective_degree': 'sup'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# ADJECTIVES_DEGREES = [
+#     IN_ADJ_POS,
+#     IN_ADJ_COM,
+#     IN_ADJ_SUP,
+# ]
+
+
+class IN_ADV_POS(Metric):
+    category = Inflection
+    name_en = "Adverbs in positive degree"
+    name_local = "Przysłówki w stopniu równym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adv', 'adverb_degree': 'pos'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_ADV_COM(Metric):
+    category = Inflection
+    name_en = "Adverbs in comparative degree"
+    name_local = "Przysłówki w stopniu wyższym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adv', 'adverb_degree': 'com'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+class IN_ADV_SUP(Metric):
+    category = Inflection
+    name_en = "Adverbs in superlative degree"
+    name_local = "Przysłówki w stopniu najwyższym"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adv', 'adverb_degree': 'sup'})
+        result = incidence(doc, selection)
+        debug = {'TOKENS': selection}
+        return result, debug
+
+
+# ADVERBS_DEGREES = [
+#     IN_ADV_POS,
+#     IN_ADV_COM,
+#     IN_ADV_SUP,
+# ]
+
+# verbs_inflection_group = MetricsGroup([m() for m in VERBS_INFLECTION])
+# verbs_persons_group = MetricsGroup([m() for m in VERBS_PERSONS])
+# verbs_tenses_group = MetricsGroup([m() for m in VERBS_TENSES])
+# verbs_aspects_group = MetricsGroup([m() for m in VERBS_ASPECTS])
+# verbs_moods_group = MetricsGroup([m() for m in VERBS_MOODS])
+# verbs_voices_group = MetricsGroup([m() for m in VERBS_VOICES])
+# verbs_participles_group = MetricsGroup([m() for m in VERBS_PARTICIPLES])
+# verbs_derivation_group = MetricsGroup([m() for m in VERBS_DERIVATION])
+# nouns_cases_group = MetricsGroup([m() for m in NOUNS_CASES])
+# pronouns_cases_group = MetricsGroup([m() for m in PRONOUNS_CASES])
+# pronouns_persons_group = MetricsGroup([m() for m in PRONOUNS_PERSONS])
+# adjectives_degrees_group = MetricsGroup([m() for m in ADJECTIVES_DEGREES])
+# adverbs_degrees_group = MetricsGroup([m() for m in ADVERBS_DEGREES])
+
+# verbs_group = verbs_inflection_group + \
+#               verbs_persons_group + \
+#               verbs_tenses_group + \
+#               verbs_aspects_group + \
+#               verbs_moods_group + \
+#               verbs_voices_group + \
+#               verbs_participles_group + \
+#               verbs_derivation_group
+# nouns_group = nouns_cases_group
+# pronouns_group = pronouns_cases_group + \
+#                  pronouns_persons_group
+# adjectives_group = adjectives_degrees_group
+# adverbs_group = adverbs_degrees_group
+# inflection_group = verbs_group + \
+#                    nouns_group + \
+#                    pronouns_group + \
+#                    adjectives_group + \
+#                    adverbs_group
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/pl.py` & `stylo_metrix-0.1.0/src/stylo_metrix/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-
-from abc import ABC
-
-from stylo_metrix.structures import Metric
-
-
-class PolishMetric(Metric, ABC):
-    lang = "pl"
+from .stylo_metrix import StyloMetrix
+from .tools.metric_tools import get_all_categories, get_all_metrics, custom_metric
+from .structures import Metric, Category
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/syntactic.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/grammatical_forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,124 +10,164 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
+from stylo_metrix.structures import Metric, Category
 
-from stylo_metrix.metrics.pl.pl import PolishMetric
-from stylo_metrix.structures import MetricsGroup
-from stylo_metrix.utils import incidence
-
-
-class Syntactic(PolishMetric, ABC):
-    category_local = "Syntactic"
-    category_en = "Składniowe"
-    category_id = 3
-
-
-class SY_S_DE(Syntactic):
-    name_en = "Words in declarative sentences incidence"
-    name_local = "Występowanie wyrazów należących do zdań oznajmujących"
-    metric_id = 1
-
-    def count(self, doc):
-        sents = [sent for sent in doc.sents if sent[-1].text in ['.', '…']]
-        words = sum([[token for token in sent if token._.is_word] for sent in sents], [])
-        result = incidence(doc, words)
-        return result, {}
-
-
-class SY_S_IN(Syntactic):
-    name_en = "Words in interrogative sentences incidence"
-    name_local = "Występowanie wyrazów należących do zdań pytających"
-    metric_id = 2
-
-    def count(self, doc):
-        sents = [sent for sent in doc.sents if sent[-1].text in ['?']]
-        words = sum([[token for token in sent if token._.is_word] for sent in sents], [])
-        result = incidence(doc, words)
-        return result, {}
-
-
-class SY_S_EX(Syntactic):
-    name_en = "Words in exclamative sentences incidence"
-    name_local = "Występowanie wyrazów należących do zdań rozkazujących"
-    metric_id = 3
-
-    def count(self, doc):
-        sents = [sent for sent in doc.sents if sent[-1].text in ['!']]
-        words = sum([[token for token in sent if token._.is_word] for sent in sents], [])
-        result = incidence(doc, words)
-        return result, {}
-
-
-class SY_S_INIT(Syntactic):
-    name_en = "Words being initial word in sentence incidence"
-    name_local = "Występowanie wyrazów będących pierwszym wyrazem zdania"
-    metric_id = 4
-
-    def count(self, doc):
-        words = [sent[0] for sent in doc.sents]
-        result = incidence(doc, words)
-        return result, {}
-
-
-class SY_NPHR(Syntactic):
-    name_en = "Words in nominal phrases incidence"
-    name_local = "Występowanie wyrazów wchodzących w skład fraz nominalnych"
-    metric_id = 5
-
-    def count(self, doc):
-        nouns = [token for token in doc if token.pos_ == 'NOUN']
-        nouns_not_part_of_subtree = []
-        for noun in nouns:
-            list_without_current = [n for n in nouns if n is not noun]
-            subtrees = [list(noun.subtree) for noun in list_without_current]
-            subtrees_list = sum(subtrees, [])
-            if noun not in subtrees_list:
-                nouns_not_part_of_subtree.append(noun)
-        subtrees = [[word for word in list(noun.subtree) if word._.is_word] for noun in nouns_not_part_of_subtree]
-        sum_subtrees = sum(subtrees, [])
-        result = incidence(doc, sum_subtrees)
-        return result, {
-            "[SUBTREES]": subtrees,
-        }
-
-
-class SY_MOD(Syntactic):
-    name_en = "Words in modifiers incidence"
-    name_local = "Występowanie wyrazów wchodzących w skład przydawek"
-    metric_id = 6
-
-    def count(self, doc):
-        mod_tags = ['amod', 'nmod', 'nmod:arg', 'acl']
-        nouns = [token for token in doc if token.pos_ == "NOUN"]
-        children_mods = [[ch for ch in list(noun.children) if ch.dep_ in mod_tags] for noun in nouns]
-        mods_heads = sum(children_mods, [])
-        mods_not_part_of_subtree = []
-        for mod in mods_heads:
-            list_without_current = [m for m in mods_heads if m is not mod]
-            subtrees = [list(mod.subtree) for mod in list_without_current]
-            subtrees_list = sum(subtrees, [])
-            if mod not in subtrees_list:
-                mods_not_part_of_subtree.append(mod)
-        subtrees = [[el for el in list(head.subtree) if el._.is_word] for head in mods_not_part_of_subtree]
-        sum_subtrees = sum(subtrees, [])
-        result = incidence(doc, sum_subtrees)
-        return result, {
-            "[SUBTREES]": subtrees
-        }
-
-
-SYNTACTIC = [
-    SY_S_DE,
-    SY_S_IN,
-    SY_S_EX,
-    SY_S_INIT,
-    SY_NPHR,
-    SY_MOD,
-]
+from stylo_metrix.utils import incidence, select, ratio
 
-syntactic_group = MetricsGroup([m() for m in SYNTACTIC])
+
+class GrammaticalForms(Category):
+    lang = 'pl'
+    name_en = "Grammatical Forms"
+    name_local = "Formy gramatyczne"
+
+
+class G_V(Metric):
+    category = GrammaticalForms
+    name_en = "Verb"
+    name_local = "Czasowniki"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'v'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+
+
+class G_N(Metric):
+    category = GrammaticalForms
+    name_en = "Nouns"
+    name_local = "Rzeczowniki"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'n'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+
+
+class G_ADJ(Metric):
+    category = GrammaticalForms
+    name_en = "Adjectives"
+    name_local = "Przymiotniki"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adj'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+
+
+class G_ADV(Metric):
+    category = GrammaticalForms
+    name_en = "Adverbs"
+    name_local = "Przysłówki"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'adv'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+
+
+class G_PRO(Metric):
+    category = GrammaticalForms
+    name_en = "Pronouns"
+    name_local = "Zaimki"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+
+
+class G_PRO_DEM(Metric):
+    category = GrammaticalForms
+    name_en = "Demonstrative pronouns"
+    name_local = "Zaimki wskazujące"
+
+    def count(doc):
+        selection = select(doc, {'pos': 'pro', 'pronoun_type': 'dem'})
+        result = incidence(doc, selection)
+        debug = {'VALUES': selection}
+        return result, debug
+    
+
+class APOSTROFA_ADJ(Metric):
+    category = GrammaticalForms
+    name_en = "Descriptive apostrophe"
+    name_local = "Apostrofa opisowa"
+
+    def count(doc):
+        c = 0
+        results = []
+        dets = ["det", "amod"]
+        for sent in doc.sents:
+            inn7w = list(
+                token.text
+                for token in sent
+                if token.pos_ == "NOUN" and str(token.morph.get("Case")) == "['Voc']"
+            )
+            pron = [
+                token.text
+                for token in sent
+                if token.dep_ in dets and token.head.text in inn7w
+            ]
+            if inn7w and pron:
+                results.append(sent)
+                c = c + len(inn7w) + len(pron)
+        debug = {"FOUND": results}
+        return ratio(c, doc._.n_tokens), debug
+    
+
+class APOSTROFA_VERB(Metric):
+    category = GrammaticalForms
+    name_en = "Apostrophe together with a verb"
+    name_local = "Apostrofa wraz z czasownikiem"
+
+    def count(doc):
+        c = 0
+        results = []
+        dets = ["det", "amod"]
+        for sent in doc.sents:
+            inn7w = list(
+                token.text
+                for token in sent
+                if token.pos_ == "NOUN" and str(token.morph.get("Case")) == "['Voc']"
+            )
+            pron = [
+                token.text
+                for token in sent
+                if token.pos_ == "VERB" and str(token.morph.get("Person")) == "['2']"
+            ]
+            if inn7w and pron:
+                results.append(sent)
+                c = c + len(inn7w) + len(pron)
+        debug = {"FOUND": results}
+        return ratio(c, doc._.n_tokens), debug
+    
+
+class VOC_CONTENT(Metric):
+    category = GrammaticalForms
+    name_en = "Apostrophe and amount of content words"
+    name_local = "Apostrofa i ilość content words"
+
+    def count(doc):
+        c = 0
+        results = []
+        for sent in doc.sents:
+            inn7w = list(
+                token.text
+                for token in sent
+                if token.pos_ == "NOUN" and str(token.morph.get("Case")) == "['Voc']"
+            )
+            pron = [token.text for token in sent if token._.content_word == "cont"]
+            if inn7w and pron:
+                results.append(sent)
+                c = c + len(inn7w) + len(pron)
+        debug = {"FOUND": results}
+        return ratio(c, doc._.n_tokens), debug
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/metrics/pl/word_formation.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/word_formation.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,179 +10,174 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from abc import ABC
+from stylo_metrix.structures import Metric, Category
 
-from stylo_metrix.metrics.pl.pl import PolishMetric
-from stylo_metrix.structures import MetricsGroup
 from stylo_metrix.utils import incidence
 
 
-class WordFormation(PolishMetric, ABC):
-    category_local = "Word Formation"
-    category_en = "Słowotwórcze"
-    affixes = ""
-    category_id = -1
-
-    def find_words_affix(self, doc, affixes, starts, pos):
-        affixes = affixes.split(", ")
-        data = [token for token in doc if token._.pos == pos] if pos else doc
+class WordFormation(Category):
+    lang = 'pl'
+    name_en = "Word Formation"
+    name_local = "Słowotwórcze"
+
+
+class Affixes:
+    @classmethod
+    def count(cls, doc):
+        affixes = cls.affixes.split(", ")
+        data = [token for token in doc if token._.pos == cls.pos] if cls.pos else doc
         search = [token for token in data if
-                  any([token.lemma_.startswith(e) if starts else token.lemma_.endswith(e)
+                  any([token.lemma_.startswith(e) if cls.starts else token.lemma_.endswith(e)
                        for e in affixes]) and token.lemma_ not in affixes]
         result = incidence(doc, search)
         return result, {}
 
 
-class NounsEnd(WordFormation, ABC):
-    affixes = ""
+class NounsEnd(Affixes):
+    starts = False
+    pos = 'n'
 
-    def count(self, doc):
-        result, debug = self.find_words_affix(doc, affixes=self.__class__.affixes, starts=False, pos='n')
-        return result, debug
 
-
-class WF_NE_OSC(NounsEnd):
+class WF_NE_OSC(Metric, NounsEnd):
     """ przyrostek bardzo częsty, tworzy pojęcia abstrakcyjne """
+    category = WordFormation
     name_en = "Incidence od nouns ending with ość"
     name_local = "Występowanie rzeczowników zakończonych na ość"
     affixes = "ość"
 
 
-class WF_NE_IK(NounsEnd):
+class WF_NE_IK(Metric, NounsEnd):
     """ zdrobnienia - częste w tekstach potocznych, internetowych """
+    category = WordFormation
     name_en = "Incidence od nouns ending with ik"
     name_local = "Występowanie rzeczowników zakończonych na ik"
     affixes = "ik"
 
 
-class WF_NE_EK(NounsEnd):
+class WF_NE_EK(Metric, NounsEnd):
     """ zdrobnienia - częste w tekstach potocznych, internetowych """
+    category = WordFormation
     name_en = "Incidence od nouns ending with ek"
     name_local = "Występowanie rzeczowników zakończonych na ek"
     affixes = "ek"
 
 
-class WF_NE_KA(NounsEnd):
+class WF_NE_KA(Metric, NounsEnd):
     """ zdrobnienia - częste w tekstach potocznych, internetowych """
+    category = WordFormation
     name_en = "Incidence od nouns ending with ka"
     name_local = "Występowanie rzeczowników zakończonych na ka"
     affixes = "ka"
 
 
-class WF_NE_KO(NounsEnd):
+class WF_NE_KO(Metric, NounsEnd):
     """ zdrobnienia - częste w tekstach potocznych, internetowych """
+    category = WordFormation
     name_en = "Incidence od nouns ending with ko"
     name_local = "Występowanie rzeczowników zakończonych na ko"
     affixes = "ko"
 
 
-class WF_NE_IYCIEL(NounsEnd):
+class WF_NE_IYCIEL(Metric, NounsEnd):
     """ wykonawcy czynności i nosiciele cech """
+    category = WordFormation
     name_en = "Incidence od nouns ending with iciel, yciel"
     name_local = "Występowanie rzeczowników zakończonych na iciel, yciel"
     affixes = "iciel, yciel"
 
 
-class WF_NE_OWIEC(NounsEnd):
+class WF_NE_OWIEC(Metric, NounsEnd):
     """ wykonawcy czynności i nosiciele cech """
+    category = WordFormation
     name_en = "Incidence od nouns ending with owiec"
     name_local = "Występowanie rzeczowników zakończonych na owiec"
     affixes = "owiec"
 
 
-class WF_NE_ARZ(NounsEnd):
+class WF_NE_ARZ(Metric, NounsEnd):
     """ wykonawcy czynności i nosiciele cech """
+    category = WordFormation
     name_en = "Incidence od nouns ending with arz"
     name_local = "Występowanie rzeczowników zakończonych na arz"
     affixes = "arz"
 
 
-class WF_NE_OWICZ(NounsEnd):
+class WF_NE_OWICZ(Metric, NounsEnd):
     """ wykonawcy czynności i nosiciele cech """
+    category = WordFormation
     name_en = "Incidence od nouns ending with owicz"
     name_local = "Występowanie rzeczowników zakończonych na owicz"
     affixes = "owicz"
 
 
 # -----------------------------------------------------------------
 
-class AdjectivesStart(WordFormation, ABC):
-    affixes = ""
-    name_en = ""
-    name_local = "Występowanie przymiotników rozpoczynających się na "
-    languages = "pl" + affixes
-
-    def count(self, doc):
-        result, debug = self.find_words_affix(doc, affixes=self.__class__.affixes, starts=True, pos='adj')
-        return result, debug
-
+class AdjectivesStart(Affixes):
+    starts = True
+    pos = 'adj'
 
 # -----------------------------------------------------------------
 
 
-class AdjectivesEnd(WordFormation, ABC):
-    affixes = ""
-    name_en = ""
-    name_local = "Występowanie przymiotników zakończonych na "
-    languages = "pl" + affixes
-
-    def count(self, doc):
-        result, debug = self.find_words_affix(doc, affixes=self.__class__.affixes, starts=False, pos='adj')
-        return result, debug
+class AdjectivesEnd(Affixes):
+    starts = False
+    pos = 'adj'
 
 
-class WF_ADJE_OWY(AdjectivesEnd):
+class WF_ADJE_OWY(Metric, AdjectivesEnd):
     """ najczęstsze przyrostki przymiotnikowe """
+    category = WordFormation
     name_en = "Incidence od adjectives ending with owy"
     name_local = "Występowanie przymiotników zakończonych na owy"
     affixes = "owy"
 
 
-class WF_ADJE_SKI(AdjectivesEnd):
+class WF_ADJE_SKI(Metric, AdjectivesEnd):
     """ najczęstsze przyrostki przymiotnikowe """
+    category = WordFormation
     name_en = "Incidence od adjectives ending with ski"
     name_local = "Występowanie przymiotników zakończonych na ski"
     affixes = "ski"
 
 
-class WF_ADJE_LIWY(AdjectivesEnd):
+class WF_ADJE_LIWY(Metric, AdjectivesEnd):
     """ najczęstsze przyrostki przymiotnikowe """
+    category = WordFormation
     name_en = "Incidence od adjectives ending with liwy"
     name_local = "Występowanie przymiotników zakończonych na liwy"
     affixes = "liwy"
 
 
 # ----------------------------------------------------
 
 
-class AllStart(WordFormation, ABC):
-    affixes = ""
-    name_en = ""
-    name_local = "Występowanie wyrazów rozpoczynających się na "
-    languages = "pl" + affixes
-
-    def count(self, doc):
-        result, debug = self.find_words_affix(doc, affixes=self.__class__.affixes, starts=True, pos=None)
-        return result, debug
-
-
-WORD_FORMATION = [
-    WF_NE_OSC,
-    WF_NE_IK,
-    WF_NE_EK,
-    WF_NE_KA,
-    WF_NE_KO,
-    WF_NE_IYCIEL,
-    WF_NE_OWIEC,
-    WF_NE_ARZ,
-    WF_NE_OWICZ,
-    WF_ADJE_OWY,
-    WF_ADJE_SKI,
-    WF_ADJE_LIWY,
-]
+# class AllStart(Metric, Affixes):
+#     affixes = ""
+#     name_en = ""
+#     name_local = "Występowanie wyrazów rozpoczynających się na "
+
+#     def count(self, doc):
+#         result, debug = self.find_words_affix(doc, affixes=self.__class__.affixes, starts=True, pos=None)
+#         return result, debug
+
+
+# WORD_FORMATION = [
+#     WF_NE_OSC,
+#     WF_NE_IK,
+#     WF_NE_EK,
+#     WF_NE_KA,
+#     WF_NE_KO,
+#     WF_NE_IYCIEL,
+#     WF_NE_OWIEC,
+#     WF_NE_ARZ,
+#     WF_NE_OWICZ,
+#     WF_ADJE_OWY,
+#     WF_ADJE_SKI,
+#     WF_ADJE_LIWY,
+# ]
 
-word_formation_group = MetricsGroup([m() for m in WORD_FORMATION])
+# word_formation_group = MetricsGroup([m() for m in WORD_FORMATION])
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/__init__.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from spacy_syllables import SpacySyllables
 from stylo_metrix.pipeline.en.pos_tagger import POSTagger
 from stylo_metrix.pipeline.en.params import Params
-from stylo_metrix.pipeline.en.metrics import Metrics
+# from stylo_metrix.pipeline.en.metrics import Metrics
 
-COMPONENTS = [
+en_components = [
     SpacySyllables,
     POSTagger,
     Params,
-    Metrics,
+    # Metrics,
 ]
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/custom_preprocessing.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/custom_preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-import spacy
 import unicodedata
 
 
-class CustomPreprocessing():
+class CustomPreprocessing:
     def __init__(self, tokenizer):
         self.tokenizer = tokenizer
 
     def __call__(self, string):
         right_quote = unicodedata.lookup('RIGHT DOUBLE QUOTATION MARK')
         left_quote = unicodedata.lookup('LEFT DOUBLE QUOTATION MARK')
         return self.tokenizer(string.replace(right_quote, '\"').replace(left_quote, '\"'))
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/grammar.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/grammar.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from stylo_metrix.pipeline.en.dictionary_en import TAGS_DICT, WORDS_POS, FUNCTION_WORDS
-
+import itertools
 
 def classify_pos(token):
     for custom_pos, pos in TAGS_DICT.items():
         if token.pos_ in pos:
             return custom_pos
 
 
@@ -39,636 +39,296 @@
 
 """GRAMMATICAL TENSES"""
 
 """ METRICS FOR THE PRESENT TENSES [PASSIVE & ACTIVE VOICE]"""
 
 
 def present_simple(doc):
-    present_simple = set()
     label = "present_simple"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.tag_ == "VBP" and [child.pos_ != "AUX" for child in token.children]:
-            present_simple.add(token)
-
-    for token in doc:
-        if token.lemma_ == "do" and (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VB":
-            head = token.head
-            present_simple.add(head)
-            present_simple.add(token)
-
-            for t in head.subtree:
-                if t.tag_ == "VB" and t.dep_ == "conj":
-                    present_simple.add(t)
-    return present_simple, ext, label
-
-
-def present_ind_3p(doc):
-    present_ind_3p = set()
-    label = "present_ind_3p"
-    ext = "verb_tense"
-
-    for token in doc:
-        if token.tag_ == "VBZ" and [child.pos_ != "AUX" for child in token.children]:
-            present_ind_3p.add(token)
-
-    return present_ind_3p, ext, label
+    negative = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.lemma_ == "do" and "Tense=Pres" in token.morph
+                                                   and "VerbForm=Inf" in token.head.morph]))
+    tokens = [token for token in doc if (token.tag_ == "VBZ" or token.tag_ == "VBP") and "Tense=Pres" in token.morph and "VerbForm=Fin" and token.dep_ != "aux" and token.dep_ != "auxpass"]
+    general = tokens + negative
+    return general, ext, label
 
 
 def present_cont(doc):
-    present_cont = set()
+
     label = "present_cont"
     ext = "verb_tense"
-
-    for token in doc:
-
-        if token.lemma_ == "be" and (
-                token.tag_ == "VBZ" or token.tag_ == "VBP") and token.dep_ == "aux" and token.head.tag_ == "VBG":
-            head = token.head
-            present_cont.add(head)
-            present_cont.add(token)
-
-            for t in head.subtree:
-                if t.tag_ == "VBG" and t.dep_ == "conj":
-                    present_cont.add(t)
-
-    return present_cont, ext, label
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.lemma_ == "be" and "Tense=Pres" in token.morph and
+              token.head.tag_ == "VBG" and not [child for child in token.head.children if child.text == "have"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.tag_ == "VBG" and token.head in tokens]
+    general = tokens + conj
+    return general, ext, label
 
 
 def present_perfect_cont(doc):
-    present_perfect_cont = set()
     label = "present_perfect_cont"
     ext = "verb_tense"
+    aux_have = ["have", "'s", "'ve", "’s", "’ve"]
+    aux_been = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.lemma_ in aux_have and "Tense=Pres" in token.morph and 
+              token.head.tag_ == "VBG" and [aux_been.append(child) for child in token.head.lefts if child.text == "been" and child.dep_ == "aux"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.head in tokens]
+    general = tokens + aux_been + conj
 
-    for token in doc:
-        if token.dep_ == "auxpass" and (token.text == "'s" or token.text == "’s") and token.head.tag_ == "VBG":
-            head = token.head
-
-            for t in head.subtree:
-                if t.text == "been" and t.dep_ == "aux":
-                    present_perfect_cont.add(head)
-                    present_perfect_cont.add(token)
-                    present_perfect_cont.add(t)
-
-                for i in head.subtree:
-                    if i.tag_ == "VBG" and i.dep_ == "conj":
-                        present_perfect_cont.add(i)
+    return general, ext, label
 
-        if token.dep_ == "aux" and token.lemma_ == "'ve" and token.head.tag_ == "VBG":
-            head = token.head
-
-            for tok in head.subtree:
-                if tok.text == "been" and tok.dep_ == "aux":
-                    present_perfect_cont.add(head)
-                    present_perfect_cont.add(token)
-                    present_perfect_cont.add(tok)
-
-            for j in head.subtree:
-                if j.tag_ == "VBG" and j.dep_ == "conj":
-                    present_perfect_cont.add(j)
-
-        if token.lemma_ == "have" and (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VBG":
-            head = token.head
 
-            for tkn in head.subtree:
-                if tkn.text == "been" and tkn.dep_ == "aux":
-                    present_perfect_cont.add(head)
-                    present_perfect_cont.add(token)
-                    present_perfect_cont.add(tkn)
-
-            for l in head.subtree:
-                if l.tag_ == "VBG" and l.dep_ == "conj":
-                    present_perfect_cont.add(l)
-
-    return present_perfect_cont, ext, label
-
-
-def present_ind_pas(doc):
-    present_ind_pas = set()
+def present_simple_passive(doc):
     label = "present_ind_passive"
     ext = "verb_tense"
+    aux = ["is", "am", "are", "'re", "'m", "'s", "’re", "’m", "’s"]
 
-    for token in doc:
-        if (
-                token.tag_ == "VBP" or token.tag_ == "VBZ") and token.dep_ == "auxpass" and token.lemma_ == 'be' and token.head.tag_ == "VBN":
-            head = token.head
-            present_ind_pas.add(head)
-
-            for child in head.subtree:
-                if child.text == "been" and child.dep_ == "auxpass" and head in present_ind_pas:
-                    present_ind_pas.remove(head)
-                if child.text == "been" and child.dep_ == "ROOT" and head in present_ind_pas:
-                    present_ind_pas.remove(head)
-            if head in present_ind_pas:
-                present_ind_pas.add(token)
-            for t in head.children:
-                if t.tag_ == "VBN" and t.dep_ == "conj" and head in present_ind_pas:
-                    present_ind_pas.add(t)
-    return present_ind_pas, ext, label
+    roots = [token for token in doc if "Aspect=Perf" in token.morph  and "Tense=Past" in token.morph  and "VerbForm=Part" in token.morph and\
+             [child for child in token.lefts if child.dep_ == "auxpass" and child.text in aux]]
+    aux = [token for token in doc if token in [*token.head.lefts] and token.head in roots and token.text in aux]
+    conj = [token for token in doc if token.tag_ == "VBN" and token.dep_ == "conj" and token.head in roots]
+    general = roots + aux + conj
+    return general, ext, label
 
 
-def present_cont_pas(doc):
-    present_cont_pas = set()
+def present_progressive_passive(doc):
     label = "present_cont_passive"
     ext = "verb_tense"
-
-    for token in doc:
-        if (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.lemma_ == "be" and token.dep_ == "aux":
-            head = token.head
-
-            for t in head.subtree:
-                if t.text == "being" and t.dep_ == "auxpass" and head not in present_cont_pas:
-                    present_cont_pas.add(head)
-                    present_cont_pas.add(t)
-                    present_cont_pas.add(token)
-
-                    if t.tag_ == "VBN" and t.dep_ == "conj":
-                        present_cont_pas.add(t)
-    return present_cont_pas, ext, label
+    aux = ["is", "am", "are", "'re", "'m", "'s", "’re", "’m", "’s"]
+    
+    roots = [token for token in doc if "Aspect=Perf" in token.morph and "Tense=Past" in token.morph and "VerbForm=Part" in token.morph and\
+             [child for child in token.lefts if child.dep_ == "aux" and child.text in aux] and [t for t in token.lefts if t.dep_ == "auxpass" and t.text == "being"]]
+    aux = [token for token in doc if token in [*token.head.lefts] and token.head in roots and token.text in aux]
+    auxpass = [token for token in doc if token in [*token.head.lefts] and token.head in roots and token.text == "being"]
+    conj = [token for token in doc if token.tag_ == "VBN" and token.dep_ == "conj" and token.head in roots]
+    general = roots + aux + auxpass + conj
+    return general, ext, label
 
 
 def present_perfect_passive(doc):
-    present_perfect_passive = set()
     label = "present_perfect_passive"
     ext = "verb_tense"
+    aux = ["have", "'s", "'ve", "’s", "’ve"]
+    auxpass = []
 
-    for token in doc:
-        if token.lemma_ == "have" and (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VBN":
-            head = token.head
-
-            for t in head.subtree:
-                if t.text == "been" and t.dep_ == "auxpass" and head not in present_perfect_passive:
-                    present_perfect_passive.add(head)
-                    present_perfect_passive.add(token)
-                    present_perfect_passive.add(t)
-
-            for tok in head.children:
-                if tok.tag_ == "VBN" and tok.dep_ == "conj" and head in present_perfect_passive:
-                    present_perfect_passive.add(tok)
-
-        if (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VBN":
-            head = token.head
-
-            for j in head.subtree:
-                if j.text == "been" and j.dep_ == "auxpass" and head not in present_perfect_passive:
-                    present_perfect_passive.add(head)
-                    present_perfect_passive.add(token)
-                    present_perfect_passive.add(j)
-
-            for tkn in head.children:
-                if tkn.tag_ == "VBN" and tkn.dep_ == "conj" and head in present_perfect_passive:
-                    present_perfect_passive.add(tkn)
-
-    return present_perfect_passive, ext, label
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.lemma_ in aux and "Tense=Pres" in token.morph
+                                                 and token.head.tag_ == "VBN" and [auxpass.append(child) for child in token.head.lefts if child.dep_ == "auxpass" and child.text == "been"]]))
+    conj = [token for token in doc if token in [*token.head.rights] and token.dep_ == "conj" and token.head in tokens]
+    general = tokens + conj + auxpass
+    return general, ext, label
 
 
 def present_perfect(doc):
-    present_perfect = []
     label = "present_perfect"
     ext = "verb_tense"
 
-    verbs_perfect_passive, _, _ = present_perfect_passive(doc)
-    verbs_ind_pas, _, _ = present_ind_pas(doc)
-    verbs_cont_pas, _, _ = present_cont_pas(doc)
-
-    for token in doc:
-
-        if token.lemma_ == "have" and (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VBN":
-            head = token.head
-            present_perfect.append(head)
-            present_perfect.append(token)
-
-            for key in verbs_perfect_passive:
-                for verb in present_perfect:
-                    if key == verb:
-                        present_perfect.remove(head)
-                        present_perfect.remove(token)
-
-            for tok in head.subtree:
-                if head in present_perfect:
-                    if tok.tag_ == "VBN" and tok.dep_ == "conj":
-                        present_perfect.append(tok)
-
-        if (token.tag_ == "VBZ" or token.tag_ == "VBP") and token.head.tag_ == "VBN":
-            head = token.head
-            present_perfect.append(head)
-
-            for key in verbs_perfect_passive:
-                for verb in present_perfect:
-                    if head in present_perfect and key == verb:
-                        present_perfect.remove(head)
-
-            for key in verbs_ind_pas:
-                for verb in present_perfect:
-                    if head in present_perfect and key == verb:
-                        present_perfect.remove(head)
-
-            for key in verbs_cont_pas:
-                for verb in present_perfect:
-                    if head in present_perfect and key == verb:
-                        present_perfect.remove(head)
-
-            for tok in head.subtree:
-                if head in present_perfect:
-                    if tok.tag_ == "VBN" and tok.dep_ == "conj" and head in present_perfect and tok not in present_perfect:
-                        present_perfect.append(tok)
-
-    present_perfect_ = set(present_perfect)
-    return present_perfect_, ext, label
+    aux = ["have", "'ve", "'s", "’ve", "’s"]
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.lemma_ in aux and "Tense=Pres" in token.morph
+                                                 and token.head.tag_ == "VBN" and not any(child for child in token.head.lefts if child.dep_ == "auxpass" or child.dep_ == "nsubjpass")]))
+    conj = [token for token in doc if token in [*token.head.rights] and token.dep_ == "conj" and token.head in tokens]
+    general = tokens + conj 
+    return general, ext, label
 
 
 """ METRICS FOR THE PAST TENSES [PASSIVE & ACTIVE VOICE]"""
 
 
 def past_simple_passive(doc):
-    past_ind_passive = set()
     label = "past_ind_passive"
     ext = "verb_tense"
 
-    for token in doc:
-
-        if token.lemma_ == "be" and token.tag_ == "VBD" and token.dep_ == "auxpass" and token.head.tag_ == "VBN":
-            head = token.head
-            past_ind_passive.add(head)
-
-            for child in head.children:
-                if child.text == "been" and child.dep_ == "auxpass":
-                    past_ind_passive.remove(head)
-
-            for tok in head.subtree:
-                if tok.tag_ == "VBN" and tok.dep_ == "conj":
-                    past_ind_passive.add(tok)
-
-            if head in past_ind_passive:
-                past_ind_passive.add(token)
-
-    return past_ind_passive, ext, label
+    tokens = list(itertools.chain.from_iterable([[token, token.head]for token in doc if "Tense=Past" in token.morph and "VerbForm=Fin" in token.morph and token.dep_ == "auxpass" 
+              and "Aspect=Perf" in token.head.morph and "Tense=Past" in token.head.morph and "VerbForm=Part" in token.head.morph]))
+    conj = [token for token in doc if token.tag_ == "VBN" and token.dep_ == "conj" and token.head in tokens]
+    general = tokens + conj
+    return general, ext, label
 
 
 def past_simple(doc):
-    past_ind = set()
     label = "past_simple"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.lemma_ == "be":
-            continue
-        if token.lemma_ == "have" and [child.tag_ == "VBN" for child in token.children]:
-            continue
-        if token.pos_ != "AUX" and token.tag_ == "VBD":
-            past_ind.add(token)
+    indicative = [token for token in doc if "Tense=Past" in token.morph and "VerbForm=Fin" in token.morph and token.text != "was" and token.text != "were"
+                  and [child for child in token.lefts if child.dep_ == "nsubj"]]
+    did_sentences = list(itertools.chain.from_iterable([[token, token.head] for token in doc if "Tense=Past" in token.morph 
+                                                        and "VerbForm=Fin" in token.morph and token.dep_ == "aux" and "VerbForm=Inf" in token.head.morph]))
+    conj = [token for token in doc if token.pos_ == "VERB" and token.dep_ == "conj" and token.head in indicative]
+    conj_neg_inter = [token for token in doc if "VerbForm=Inf" in token.morph and token.dep_ == "conj" and [i for i in token.head.lefts if "Tense=Past" in i.morph 
+                    and "VerbForm=Fin" in i.morph and i.dep_ == "aux"]]
 
-        if token.lemma_ == "do" and token.tag_ == "VBD" and token.head.tag_ == "VB":
-            head = token.head
-            past_ind.add(head)
-            past_ind.add(token)
-            for t in head.subtree:
-                if t.tag_ == "VB" and t.dep_ == "conj":
-                    past_ind.add(t)
+    general = indicative + did_sentences + conj + conj_neg_inter
 
-    return past_ind, ext, label
+    return general, ext, label
 
 
 def past_simple_be(doc):
-    past_ind_be = set()
     label = "past_ind_be"
     ext = "verb_tense"
 
-    for token in doc:
-        for child in token.children:
-            if token.lemma_ == "be" and token.tag_ == "VBD" and child.tag_ != "VBG" and token not in past_ind_be:
-                past_ind_be.add(token)
-
-    return past_ind_be, ext, label
+    tokens = [token for token in doc if token.lemma_ == "be" and token.tag_ == "VBD" and [child for child in token.children if child.tag_ != "VBG"]]
+    return tokens, ext, label
 
 
 def past_cont_passive(doc):
-    past_cont_passive = set()
     label = "past_cont_passive"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.lemma_ == "be" and token.tag_ == "VBD" and token.head.tag_ == "VBN":
-            head = token.head
-
-            for child in head.children:
-                if child.text == "being" and child.tag_ == "VBG":
-                    past_cont_passive.add(head)
-                    past_cont_passive.add(child)
-                    past_cont_passive.add(token)
-
-            for t in head.subtree:
-                if t.tag_ == "VBN" and t.dep_ == "conj" and head in past_cont_passive and t not in past_cont_passive:
-                    past_cont_passive.add(t)
-
-    return past_cont_passive, ext, label
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.text == "being" and "Tense=Past" in token.head.morph and
+                                                 "VerbForm=Part" in token.head.morph and token.head.tag_ == "VBN" and 
+                                                 [aux.append(child) for child in token.head.lefts if child.dep_ == "aux" and child.lemma_ == "be" and "Tense=Past" in child.morph and "VerbForm=Fin" in child.morph]]))
+    conj = [token for token in doc if token.tag_ == "VBN" and token.dep_ == "conj" and token.head in tokens]
+    general = aux + tokens + conj
+    return general, ext, label
 
 
 def past_cont(doc):
-    past_cont = set()
     label = "past_cont"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.lemma_ == "be" and token.tag_ == "VBD" and token.head.tag_ == "VBG":
-            head = token.head
-            past_cont.add(head)
-            past_cont.add(token)
-            for t in head.subtree:
-                if t.tag_ == "VBG" and t.dep_ == "conj" and t not in past_cont:
-                    past_cont.add(t)
-    return past_cont, ext, label
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.lemma_ == "be" and token.tag_ == "VBD" and token.head.tag_ == "VBG" and 
+                                                 not [t for t in token.head.lefts if t.dep_ == "aux" and t.text == "had"]]))
+    conj = [token for token in doc if token.tag_ == "VBG" and token.dep_ == "conj" and token.head in tokens]
+    general = tokens + conj
+
+    return general, ext, label
 
 
 def past_perfect(doc):
-    past_perf = set()
     label = "past_perf"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.tag_ == "VBD" and token.dep_ == "aux" and token.lemma_ == "have" and token.head.tag_ == "VBN":
-            head = token.head
-            past_perf.add(head)
-
-            for child in head.children:
-                if child.text == "been" and child.dep_ == "auxpass":
-                    past_perf.remove(head)
-
-            for t in head.subtree:
-                if t.tag_ == "VBN" and t.dep_ == "conj" and head in past_perf and t not in past_perf:
-                    past_perf.add(t)
-
-        if (token.text == "'d" or token.text == "’d") and (token.head.tag_ == "VBN" or token.head.tag_ == "VBD"):
-            head = token.head
-            past_perf.add(head)
-
-            for child in head.children:
-                if child.lemma_ == "be" and child.dep_ == "auxpass" and head in past_perf:
-                    past_perf.remove(head)
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and "Tense=Past" in token.morph and token.lemma_ != "be"
+              and"Aspect=Perf" in token.head.morph and "Tense=Past" in token.head.morph and
+              not [child for child in token.head.lefts if child.dep_ == "auxpass" and child.lemma_ == "be"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.pos_ == "VERB" and token.head in tokens]
+    general = tokens + conj
 
-            for tok in head.subtree:
-                if tok.tag_ == "VBN" and tok.dep_ == "conj" and head in past_perf and tok not in past_perf:
-                    past_perf.add(tok)
-
-            if head in past_perf:
-                past_perf.add(token)
-
-    return past_perf, ext, label
+    return general, ext, label
 
 
 def past_perf_passive(doc):
-    past_perf_passive = set()
     label = "past_perf_passive"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.tag_ == "VBD" and token.lemma_ == "have" and token.head.tag_ == "VBN":
-            head = token.head
+    auxpass = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and "Tense=Past" in token.morph and token.lemma_ != "be"
+              and"Aspect=Perf" in token.head.morph and "Tense=Past" in token.head.morph and [auxpass.append(child) for child in token.head.lefts if child.dep_ == "auxpass" and child.lemma_ == "be"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.pos_ == "VERB" and token.head in tokens]
+    general =  tokens + conj + auxpass
 
-            for child in head.children:
-                if child.text == "been" and child.dep_ == "auxpass":
-                    past_perf_passive.add(head)
-                    past_perf_passive.add(token)
-                    past_perf_passive.add(child)
-
-            for t in head.subtree:
-                if t.tag_ == "VBN" and t.dep_ == "conj" and head in past_perf_passive and t not in past_perf_passive:
-                    past_perf_passive.add(t)
-
-                    # make sure that no past simple passive verbs are regarded as
-                    # synonyms of the past perfect passive
-                    for ch in t.children:
-                        if ch.lemma_ == "be" and (ch.tag_ == "VBD" or ch.tag_ == "VBG") and t in past_perf_passive:
-                            past_perf_passive.remove(t)
-
-        if (token.text == "'d" or token.text == "’d") and token.head.tag_ == "VBN":
-            head = token.head
-
-            for child in head.children:
-                if child.lemma_ == "be" and child.dep_ == "auxpass":
-                    past_perf_passive.add(head)
-                    past_perf_passive.add(token)
-                    past_perf_passive.add(child)
-
-            for tok in head.subtree:
-                if tok.tag_ == "VBN" and tok.dep_ == "conj" and head in past_perf_passive:
-                    past_perf_passive.add(tok)
-
-                    for chld in tok.children:
-                        if chld.lemma_ == "be" and (
-                                chld.tag_ == "VBD" or chld.tag_ == "VBG") and tok in past_perf_passive:
-                            past_perf_passive.remove(tok)
-
-    return past_perf_passive, ext, label
+    return general, ext, label
 
 
 def past_perfect_cont(doc):
-    past_perfect_cont = set()
     label = "past_perf_cont"
     ext = "verb_tense"
 
-    for token in doc:
-        if token.tag_ == "VBD" and token.lemma_ == "have" and token.head.tag_ == "VBG":
-            head = token.head
-            past_perfect_cont.add(head)
-            past_perfect_cont.add(token)
-
-            for j in head.children:
-                if j.text == "been":
-                    past_perfect_cont.add(j)
-
-            for t in head.subtree:
-                if t.tag_ == "VBG" and t.dep_ == "conj" and t not in past_perfect_cont:
-                    past_perfect_cont.add(t)
-
-    return past_perfect_cont, ext, label
+    aux_been = []
+    aux_have = ["had", "'d", "’d", "Had"]
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if token.dep_ == "aux" and token.text in aux_have and 
+              token.head.tag_ == "VBG" and [aux_been.append(child) for child in token.head.lefts if child.text == "been" and child.dep_ == "aux"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.tag_ == "VBG" and token.head in tokens]
+    general = tokens + conj + aux_been
+    return general, ext, label
 
 
 """ METRICS FOR THE FUTURE TENSES [PASSIVE & ACTIVE VOICE]"""
 
 
 def future_simple(doc):
-    future_simple = set()
     label = "future_simple"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VB" and token.head not in future_simple:
-            head = token.head
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+              and "VerbForm=Inf" in token.head.morph]))
+    conj = [token for token in doc if "VerbForm=Inf" in token.morph and token.dep_ == "conj" and token.head in tokens]
+    general = tokens + conj
 
-            for t in head.subtree:
-                if t.tag_ == "VB" and t.dep_ != "xcomp":
-                    future_simple.add(t)
-                    future_simple.add(token)
-
-    return future_simple, ext, label
+    return general, ext, label
 
 
 def future_simple_passive(doc):
-    future_simple_passive = set()
     label = "future_simple_passive"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[
-            len(str(token)) - 2:] == "ll" or token.lemma_ == "will") and \
-                token.head.tag_ == "VBN" and token.head not in future_simple_passive:
-            head = token.head
-
-            for t in head.children:
-                if t.text == "be" and t.dep_ == "auxpass":
-                    future_simple_passive.add(head)
-                    future_simple_passive.add(token)
-                    future_simple_passive.add(t)
-
-            for child in head.subtree:
-                if child.tag_ == "VBN" and child.dep_ == "conj" and head in future_simple_passive:
-                    future_simple_passive.add(child)
-
-                    for ch in child.children:
-                        if (ch.text == "being" or ch.text == "been") and ch.dep_ == "auxpass" and child in future_simple_passive:
-                            future_simple_passive.remove(child)
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+              and "Tense=Past" in token.head.morph and "VerbForm=Part" in token.head.morph and [aux.append(child) for child in token.head.lefts if child.dep_ == "auxpass" and child.text == "be"]
+              and not [t for t in token.head.lefts if t.text == "being"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.pos_ == "VERB" and "Tense=Past" in token.morph and "VerbForm=Part" in token.morph and token.head in tokens]
+    general = tokens + aux + conj
 
-    return future_simple_passive, ext, label
+    return general, ext, label
 
 
 def future_cont(doc):
-    future_progr = set()
     label = "future_progr"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VBG" and token.head not in future_progr:
-
-            head = token.head
-            future_progr.add(head)
-
-            for t in head.subtree:
-                if t.lemma_ == "have" and head in future_progr:
-                    future_progr.remove(head)
-
-                if t.tag_ == "VBG" and t.dep_ == "conj":
-                    future_progr.add(t)
-
-            if head in future_progr:
-                future_progr.add(token)
-
-            for j in head.children:
-                if j.text == "be":
-                    future_progr.add(j)
-    return future_progr, ext, label
+    aux = []
+    heads = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll") and
+             "Tense=Pres" in token.head.morph and "VerbForm=Part" in token.head.morph and [aux.append(child) for child in token.head.lefts if "VerbForm=Inf" in child.morph and child.lemma_ == "be"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.pos_ == "VERB" and "Tense=Pres" in token.morph and "VerbForm=Part" in token.morph and token.head in heads]
+    general = aux + heads + conj
+    return general, ext, label
 
 
 def future_progr_passive(doc):
-    future_progr_passive = set()
     label = "future_progr_passive"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VBN" and token.head not in future_progr_passive:
-            head = token.head
-
-            for t in head.children:
-                if t.text == "being" and t.dep_ == "auxpass":
-                    future_progr_passive.add(head)
-                    future_progr_passive.add(t)
-                    future_progr_passive.add(token)
-
-                if t.text == "be" and head in future_progr_passive:
-                    future_progr_passive.add(t)
-                if t.tag_ == "VBN" and t.dep_ == "conj" and head in future_progr_passive:
-                    future_progr_passive.add(t)
-
-                    for chld in t.children:
-                        if chld.text == "be" or chld.text == "been" and chld.dep_ == "auxpass" and t in future_progr_passive:
-                            future_progr_passive.remove(t)
-    return future_progr_passive, ext, label
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+              and "Tense=Past" in token.head.morph and "VerbForm=Part" in token.head.morph and [aux.append(child) for child in token.head.lefts if child.dep_ == "aux" and child.text == "be"]
+              and [aux.append(t) for t in token.head.lefts if t.text == "being" and t.dep_ == "auxpass"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and token.pos_ == "VERB" and "Tense=Past" in token.morph and "VerbForm=Part" in token.morph and token.head in tokens]
+    general = tokens + aux + conj
+    return general, ext, label
 
 
 def future_perfect(doc):
-    future_perfect = set()
     label = "future_perfect"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VBN" and token.head not in future_perfect:
-            head = token.head
-
-            for t in head.children:
-                if t.lemma_ == "have" and t.dep_ == "aux":
-                    future_perfect.add(head)
-                if t.text == "been" and t.dep_ == "auxpass" and head in future_perfect:
-                    future_perfect.remove(head)
-
-            for tok in head.subtree:
-                if tok.tag_ == "VBN" and tok.dep_ == "conj" and head in future_perfect:
-                    future_perfect.add(tok)
-
-                for chld in tok.children:
-                    if (chld.text == "being" or chld.text == "be") and tok in future_perfect:
-                        future_perfect.remove(tok)
-
-            if head in future_perfect:
-                for k in head.children:
-                    if k.text == "have":
-                        future_perfect.add(k)
-                    if k.text == "been":
-                        future_perfect.add(k)
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+              and "Tense=Past" in token.head.morph and "VerbForm=Part" in token.head.morph and not [t for t in token.head.lefts if t.text == "been" and t.dep_ == "auxpass"]
+              and [aux.append(child) for child in token.head.lefts if child.dep_ == "aux" and child.text == "have"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and "Tense=Past" in token.morph and "VerbForm=Part" in token.morph and token.head in tokens]
+    general = tokens + aux + conj
 
-    return future_perfect, ext, label
+    return general, ext, label
 
 
 def future_perfect_passive(doc):
-    future_perf_passive = set()
     label = "future_perf_passive"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VBN" and token.head not in future_perf_passive:
-            head = token.head
-
-            for child in head.children:
-                if child.text == "been" and child.dep_ == "auxpass":
-                    future_perf_passive.add(head)
-                    future_perf_passive.add(token)
-                    future_perf_passive.add(child)
-
-            for chld in head.subtree:
-                if chld.tag_ == "VBN" and chld.dep_ == "conj" and head in future_perf_passive:
-                    future_perf_passive.add(chld)
-
-                for t in chld.children:
-                    if (t.text == "be" or t.text == "being") and t.dep_ == "auxpass" and chld in future_perf_passive:
-                        future_perf_passive.remove(chld)
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+              and "Tense=Past" in token.head.morph and "VerbForm=Part" in token.head.morph and [aux.append(t) for t in token.head.lefts if t.text == "been" and t.dep_ == "auxpass"]
+              and [aux.append(child) for child in token.head.lefts if child.dep_ == "aux" and child.text == "have"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and "Tense=Past" in token.morph and "VerbForm=Part" in token.morph and token.head in tokens]
+    general = tokens + aux + conj
 
-    return future_perf_passive, ext, label
+    return general, ext, label
 
 
 def future_perf_cont(doc):
-    future_perfect_cont = set()
     label = "future_perfect_cont"
     ext = "verb_tense"
 
-    for token in doc:
-        if (str(token)[len(str(token)) - 2:] == "ll" or token.lemma_ == "will") \
-                and token.head.tag_ == "VBG" and token.head not in future_perfect_cont:
-            head = token.head
-
-            for t in head.children:
-                if t.tag_ == "VBN" and t.lemma_ == "be":
-                    future_perfect_cont.add(head)
-                    future_perfect_cont.add(t)
-                    future_perfect_cont.add(token)
-    return future_perfect_cont, ext, label
+    aux = []
+    tokens = list(itertools.chain.from_iterable([[token, token.head] for token in doc if (token.lemma_ =="will" or token.lemma_ == "'ll" or token.lemma_ == "’ll")
+                                                 and "Tense=Pres" in token.head.morph and "VerbForm=Part" in token.head.morph and [aux.append(child) for child in token.head.lefts if child.dep_ == "aux" and child.text == "have"]
+                                                 and [aux.append(t) for t in token.head.lefts if t.text == "been" and t.dep_ == "aux"]]))
+    conj = [token for token in doc if token.dep_ == "conj" and "Tense=Pres" in token.morph and "VerbForm=Part" in token.morph and token.head in tokens]
+    general = tokens + aux + conj
+    return general, ext, label
 
 
 """ METRICS FOR MODAL VERBS [PASSIVE & ACTIVE VOICE]"""
 
 
 def would_ind_active(doc):
     would_ind_active = set()
@@ -1021,15 +681,15 @@
                 if (j.tag_ == "VBN" or j.tag_ == "VBD") and j.dep_ == "conj":
                     must_perf_active.add(j)
     return must_perf_active, ext, label
 
 
 def must_perf_passive(doc):
     must_perf_passive = set()
-    label = "could_perf_passive"
+    label = "must_perf_passive"
     ext = "modal_verbs"
 
     for token in doc:
 
         if token.lemma_ == "must" and token.head.tag_ == "VBN":
             head = token.head
 
@@ -1169,40 +829,24 @@
                     for j in head.subtree:
                         if j.tag_ == "VBG" and j.dep_ == "conj":
                             could_cont.add(j)
     return could_cont, ext, label
 
 
 def could_perf_active(doc):
-    could_perf_active = set()
+
     label = "could_perf"
     ext = "modal_verbs"
-
-    for token in doc:
-
-        if token.lemma_ == "could" and token.head.tag_ == "VBN":
-            head = token.head
-
-            for t in head.subtree:
-                if t.lemma_ == "have":
-                    could_perf_active.add(head)
-                    could_perf_active.add(t)
-
-                    for j in head.subtree:
-                        if j.text == "been" and j.dep_ != "ROOT" and (head in could_perf_active):
-                            could_perf_active.remove(head)
-                            could_perf_active.remove(t)
-
-            if head in could_perf_active:
-                could_perf_active.add(token)
-
-            for k in head.subtree:
-                if k.tag_ == "VBN" and k.dep_ == "conj" and head in could_perf_active:
-                    could_perf_active.add(k)
-    return could_perf_active, ext, label
+    sentences = list(itertools.chain.from_iterable([[sent for token in sent if token.dep_ == "ROOT" and doc[token.i-1].text == "have" 
+                  and doc[token.i-1].dep_ == "aux" and [child for child in token.lefts if child.text == "could" and child.dep_ == "aux"]]
+                  for sent in doc.sents]))
+    search = list(itertools.chain.from_iterable([[[token.head, doc[token.head.i-1], token] for 
+                                                  token in sent if token.dep_ == "aux" and token.text == "could"] for sent in sentences]))
+    result = list(itertools.chain.from_iterable(search))
+    return result, ext, label
 
 
 def could_perf_passive(doc):
     could_perf_passive = set()
     label = "could_perf_passive"
     ext = "modal_verbs"
 
@@ -1507,19 +1151,18 @@
             adv[token] = "superlative_adverb"
 
     return adv
 
 
 FUNCTION_LIST = [
     present_simple,
-    present_ind_3p,
     present_cont,
     present_perfect_cont,
-    present_ind_pas,
-    present_cont_pas,
+    present_simple_passive,
+    present_progressive_passive,
     present_perfect_passive,
     present_perfect,
     past_simple_passive,
     past_simple,
     past_simple_be,
     past_cont_passive,
     past_cont,
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/metrics.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/sentence_segmenter.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,33 +10,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from spacy.tokens import Doc
-
-from stylo_metrix.metrics.en import original_group
-from stylo_metrix.structures.stylo_metrix_vector import StyloMetrixVector
-
-
-class Metrics:
+class SentenceSegmenter():
 
     def __init__(self, nlp):
         self.nlp = nlp
-        Doc.set_extension("smv", default=None, force=True)
-        Doc.set_extension("stylo_metrix_vector", default=None, force=True)
-        nlp.metrics_group = original_group
 
     def __call__(self, doc):
-        values = [metric(doc) for metric in self.nlp.metrics_group]
-        vector = StyloMetrixVector(doc._.name, values)
-        doc._.set("smv", vector)
-        doc._.set("stylo_metrix_vector", vector)
-        return doc
+        return self.segment(doc)
 
-    def add_metrics(self, metric): pass
-
-    def set_metrics(self, metrics_group): pass
-
-    def remove_metrics(self, id): pass
+    def segment(self, doc):
+        for token in doc[:-2]:
+            if token.tag_ == 'brev':
+                if doc[token.i + 2].text[0].isupper():
+                    doc[token.i + 2].is_sent_start = True
+                else:
+                    doc[token.i + 2].is_sent_start = False
+        return doc
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/params.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/ukr/params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-# Copyright (C) 2022  NASK PIB
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
-from spacy.tokens import Doc
-
-
-class Params:
-    def __init__(self, nlp):
-        self.nlp = nlp
-        Doc.set_extension("words", default=None, force=True)
-        # Doc.set_extension("content_words", default=None, force=True)
-        # Doc.set_extension("punctuation", default=None, force=True)
-        Doc.set_extension("n_tokens", default=None, force=True)
-        # Doc.set_extension("n_words", default=None, force=True)
-        # Doc.set_extension("n_content_words", default=None, force=True)
-        # Doc.set_extension("n_punctuation", default=None, force=True)
-
-    def __call__(self, doc):
-        doc._.set("words", [token for token in doc if token._.is_word])
-        # doc._.set("content_words", [token for token in doc if token._.content_word == 'cont'])
-        # doc._.set("punctuation", [token for token in doc if token._.is_punctuation])
-        doc._.set("n_tokens", len([token for token in doc]))
-        # doc._.set("n_words", len(doc._.words))
-        # doc._.set("n_content_words", len(doc._.content_words))
-        # doc._.set("n_punctuation", len(doc._.punctuation))
-        return doc
+# Copyright (C) 2022  NASK PIB
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from spacy.tokens import Doc
+
+class Params:
+    def __init__(self, nlp):
+        self.nlp = nlp
+        Doc.set_extension("words", default=None, force=True)
+        Doc.set_extension("content_words", default=None, force=True)
+        Doc.set_extension("punctuation", default=None, force=True)
+        Doc.set_extension("n_tokens", default=None, force=True)
+        Doc.set_extension("n_words", default=None, force=True)
+        Doc.set_extension("n_content_words", default=None, force=True)
+        Doc.set_extension("n_punctuation", default=None, force=True)
+
+    def __call__(self, doc):
+        doc._.set("words", [token for token in doc if token._.is_word])
+        doc._.set("content_words", [token for token in doc if token._.is_content_word])
+        doc._.set("punctuation", [token for token in doc if token._.is_punctuation])
+        doc._.set("n_tokens", len([token for token in doc]))
+        doc._.set("n_words", len(doc._.words))
+        doc._.set("n_content_words", len(doc._.content_words))
+        doc._.set("n_punctuation", len(doc._.punctuation))
+        return doc
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/en/pos_tagger.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/en/pos_tagger.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import stylo_metrix.pipeline.en.grammar as grammar
+import stylo_metrix.pipeline.en.stylistic as stylistic
+import stylo_metrix.pipeline.en.psycholinguistics as psycholinguistics
 from spacy.tokens import Token
 
 
 class POSTagger():
 
     def __init__(self, nlp):
         """
@@ -35,32 +37,41 @@
         Token.set_extension("verb_tense", default=None, force=True)
         Token.set_extension("modal_verbs", default=None, force=True)
         Token.set_extension("adjectives", default=None, force=True)
         Token.set_extension("adverbs", default=None, force=True)
         Token.set_extension("is_word", default=False, force=True)
         Token.set_extension("is_function_word", default=False, force=True)
         Token.set_extension("is_content_word", default=False, force=True)
+        Token.set_extension("stylistic", default=None, force=True)
+        Token.set_extension("linking_words", default=None, force=True)
+        Token.set_extension("syntax", default=None, force=True)
 
     def __call__(self, doc):
         for token in doc:
             token._.set("pos", grammar.classify_pos(token))
             token._.set("is_word", grammar.is_word(token))
             token._.set("is_function_word", grammar.is_function_word(token))
             token._.set("is_content_word", grammar.is_content_word(token))
+        
+        def assign_label(function_list):
+            for function in function_list:
+                lst, extension, label = function(doc)
+                for token in lst:
+                    token._.set(extension, label)
 
         adj = grammar.adjectives(doc)
         for t, label in adj.items():
             t._.set("adjectives", label)
 
         adv = grammar.adverbs(doc)
         for t, label in adv.items():
             t._.set("adverbs", label)
 
-        def assign_label(function_list):
-            for function in function_list:
-                lst, extension, label = function(doc)
-                for token in lst:
-                    token._.set(extension, label)
         assign_label(grammar.FUNCTION_LIST)
+        assign_label(psycholinguistics.FUNCTION_LIST)
+        assign_label(stylistic.FUNCTION_LIST)
 
+        val, extension, label = stylistic.simile(doc)
+        for token in val:
+            token._.set(extension, label)
         return doc
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/__init__.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from spacy_syllables import SpacySyllables
 
-from stylo_metrix.pipeline.pl.metrics import Metrics
+from stylo_metrix.pipeline.pl.matcher_component import MatcherComponent
 from stylo_metrix.pipeline.pl.params import Params
 from stylo_metrix.pipeline.pl.pos_tagger import POSTagger
 from stylo_metrix.pipeline.pl.psycholinguistic import Psycholinguistic
 from stylo_metrix.pipeline.pl.sentence_segmenter import SentenceSegmenter
 
-COMPONENTS = [
+pl_components = [
     SpacySyllables,
     SentenceSegmenter,
     POSTagger,
     Psycholinguistic,
-    Params,
-    Metrics,
+    MatcherComponent,
+    Params
 ]
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/metrics.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/psycholinguistic.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,31 +10,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from spacy.tokens import Doc
+from spacy.tokens import Doc, Token
 
-from stylo_metrix.metrics.pl import original_group
-from stylo_metrix.structures.stylo_metrix_vector import StyloMetrixVector
+from stylo_metrix.pipeline.pl.resources.experimental_data import MEANS, PSYCHOLINGUISTIC_DATA
 
 
-class Metrics:
+class Psycholinguistic():
 
     def __init__(self, nlp):
         self.nlp = nlp
-        Doc.set_extension("smv", default=None, force=True)
-        Doc.set_extension("stylo_metrix_vector", default=None, force=True)
-        nlp.metrics_group = original_group
+        Token.set_extension("affective_norms", default=None, force=True)  # type dict
+        Doc.set_extension("an_means", default=MEANS, force=True)
 
     def __call__(self, doc):
-        values = [metric(doc) for metric in self.nlp.metrics_group]
-        vector = StyloMetrixVector(doc._.name, values)
-        doc._.set("smv", vector)
-        doc._.set("stylo_metrix_vector", vector)
+        for token in doc:
+            if token.lemma_ in PSYCHOLINGUISTIC_DATA.keys():
+                token._.set("affective_norms", PSYCHOLINGUISTIC_DATA[token.lemma_])
         return doc
-
-    @property
-    def n_metrics(self):
-        return len(self.nlp.metrics_group)
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/params.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/params.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pl_nask/pos.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pl_nask/pos.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/pos_tagger.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/pipeline/pl/resources/experimental_data.py` & `stylo_metrix-0.1.0/src/stylo_metrix/pipeline/pl/resources/experimental_data.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/structures/__init__.py` & `stylo_metrix-0.1.0/src/stylo_metrix/metrics/pl/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-# Copyright (C) 2022  NASK PIB
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
-from stylo_metrix.structures.metric import Metric, CustomMetric
-from stylo_metrix.structures.metrics_group import MetricsGroup
-from stylo_metrix.structures.stylo_metrix_vector import StyloMetrixVector
+# Copyright (C) 2022  NASK PIB
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from stylo_metrix.structures import Lang
+
+class PlLang(Lang):
+    definitions = ['polish', 'polski', 'pl', 'pol']
+    spacy_model = 'pl_nask'
+
+from .descriptive import *
+from .grammatical_forms import *
+from .graphical import *
+from .inflection import *
+from .lexical import *
+from .psycholinguistic import *
+from .punctuation import *
+from .syntactic import *
+from .word_formation import *
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix/utils.py` & `stylo_metrix-0.1.0/src/stylo_metrix/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,83 @@
-# Copyright (C) 2022  NASK PIB
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
-import statistics
-
-
-def mean(l: list):
-    try:
-        result = statistics.mean(l)
-    except statistics.StatisticsError:
-        result = 0
-    return result
-
-
-def stdev(lst: list):
-    try:
-        result = statistics.stdev(lst)
-    except statistics.StatisticsError:
-        result = 0
-    return result
-
-
-def median(lst: list):
-    try:
-        result = statistics.median(lst)
-    except statistics.StatisticsError:
-        result = 0
-    return result
-
-
-def ratio(v1: int, v2: int):
-    try:
-        return v1 / v2
-    except ZeroDivisionError:
-        return 0
-
-
-def select(doc, attr_dict):
-    selection = [token for token in doc
-                 if all([getattr(getattr(token, '_'), attr) == value for attr, value in attr_dict.items()])]
-    return selection
-
-
-def incidence(doc, selection):
-    return ratio(len(selection), doc._.n_tokens)
-
-
-def highlight_words(doc, tokens):
-    return "".join(
-        [(str(f"[[[{token}]]]") if token in tokens else str(token)) + token.whitespace_ for token in doc])
-
-
-def start_end_quote(doc):
-    for token in doc:
-        if ("PunctSide=Ini" and "PunctType=Quot") in token.morph:
-            start = token.i+1
-            break
-        else:
-            start = None
-    for token in reversed(doc):
-        if ("PunctSide=Fin" and "PunctType=Quot") in token.morph:
-            end = token.i-1
-            break
-        else:
-            end = None
-    return start, end
+# Copyright (C) 2022  NASK PIB
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+
+import statistics
+
+
+def mean(l: list):
+    try:
+        result = statistics.mean(l)
+    except statistics.StatisticsError:
+        result = 0
+    return result
+
+
+def stdev(lst: list):
+    try:
+        result = statistics.stdev(lst)
+    except statistics.StatisticsError:
+        result = 0
+    return result
+
+
+def median(lst: list):
+    try:
+        result = statistics.median(lst)
+    except statistics.StatisticsError:
+        result = 0
+    return result
+
+
+def ratio(v1: int, v2: int):
+    try:
+        return v1 / v2
+    except ZeroDivisionError:
+        return 0
+
+
+def select(doc, attr_dict):
+    selection = [token for token in doc
+                 if all([getattr(getattr(token, '_'), attr) == value for attr, value in attr_dict.items()])]
+    return selection
+
+
+def incidence(doc, selection):
+    return ratio(len(selection), doc._.n_tokens)
+
+
+def sent_incidence(doc, selection):
+    return ratio(len(selection), doc._.n_sents)
+
+
+def highlight_words(doc, tokens):
+    return "".join(
+        [(str(f"[[[{token}]]]") if token in tokens else str(token)) + token.whitespace_ for token in doc])
+
+
+def start_end_quote(doc):
+    for token in doc:
+        if ("PunctSide=Ini" and "PunctType=Quot") in token.morph:
+            start = token.i+1
+            break
+        else:
+            start = None
+    for token in reversed(doc):
+        if ("PunctSide=Fin" and "PunctType=Quot") in token.morph:
+            end = token.i-1
+            break
+        else:
+            end = None
+    return start, end
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix.egg-info/PKG-INFO` & `stylo_metrix-0.1.0/src/stylo_metrix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: stylo-metrix
-Version: 0.0.7
+Version: 0.1.0
 Summary: StyloMetrix tool
 Home-page: https://github.com/ZILiAT-NASK/StyloMetrix
-Author: ZILiAT-NASK, Anna Zawadzka
-Author-email: anna.zawadzka@nask.pl
+Author: ZILiAT-NASK, Adam Nowakowski
+Author-email: adam.nowakowski@nask.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: stylo-metrix Version: 0.0.7 Summary: StyloMetrix
+Metadata-Version: 2.1 Name: stylo-metrix Version: 0.1.0 Summary: StyloMetrix
 tool Home-page: https://github.com/ZILiAT-NASK/StyloMetrix Author: ZILiAT-NASK,
-Anna Zawadzka Author-email: anna.zawadzka@nask.pl Classifier: Programming
+Adam Nowakowski Author-email: adam.nowakowski@nask.pl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # StyloMetrix [StyloMetrix][NASK] ZakÅad InÅ¼ynierii Lingwistycznej i
 Anailzy Tekstu, NASK PIB ## ð Quick ð¡ Stylometry tool in beta version for
 **Polish** and **English** language, distributed as a **Python package** ð¡
 [Tutorial notebook](examples/Quick%20Tutorial.ipynb) ð¡ List of built-in
```

### Comparing `stylo_metrix-0.0.7/src/stylo_metrix.egg-info/SOURCES.txt` & `stylo_metrix-0.1.0/src/stylo_metrix.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/stylo_metrix/__init__.py
-src/stylo_metrix/functions.py
-src/stylo_metrix/logger.py
-src/stylo_metrix/reader.py
+src/stylo_metrix/stylo_metrix.py
 src/stylo_metrix/utils.py
-src/stylo_metrix/writer.py
 src/stylo_metrix.egg-info/PKG-INFO
 src/stylo_metrix.egg-info/SOURCES.txt
 src/stylo_metrix.egg-info/dependency_links.txt
 src/stylo_metrix.egg-info/requires.txt
 src/stylo_metrix.egg-info/top_level.txt
 src/stylo_metrix/metrics/__init__.py
 src/stylo_metrix/metrics/en/__init__.py
-src/stylo_metrix/metrics/en/en.py
+src/stylo_metrix/metrics/en/distance_en.py
+src/stylo_metrix/metrics/en/figures_of_speech.py
 src/stylo_metrix/metrics/en/grammatical_forms.py
 src/stylo_metrix/metrics/en/lexical_en.py
 src/stylo_metrix/metrics/en/parts_of_speech_en.py
+src/stylo_metrix/metrics/en/psycholinguistics.py
+src/stylo_metrix/metrics/en/social_media.py
 src/stylo_metrix/metrics/en/syntactic_en.py
+src/stylo_metrix/metrics/en/text_statistics.py
 src/stylo_metrix/metrics/en/verb_tenses_en.py
 src/stylo_metrix/metrics/pl/__init__.py
+src/stylo_metrix/metrics/pl/descriptive.py
 src/stylo_metrix/metrics/pl/grammatical_forms.py
+src/stylo_metrix/metrics/pl/graphical.py
 src/stylo_metrix/metrics/pl/inflection.py
 src/stylo_metrix/metrics/pl/lexical.py
-src/stylo_metrix/metrics/pl/pl.py
 src/stylo_metrix/metrics/pl/psycholinguistic.py
+src/stylo_metrix/metrics/pl/punctuation.py
 src/stylo_metrix/metrics/pl/syntactic.py
 src/stylo_metrix/metrics/pl/word_formation.py
+src/stylo_metrix/metrics/ukr/__init__.py
+src/stylo_metrix/metrics/ukr/lexical_ukr.py
+src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py
+src/stylo_metrix/metrics/ukr/syntactic_ukr.py
+src/stylo_metrix/metrics/ukr/verb_forms_ukr.py
 src/stylo_metrix/pipeline/__init__.py
-src/stylo_metrix/pipeline/stylo_metrix_pipe.py
+src/stylo_metrix/pipeline/new_pipe.py
 src/stylo_metrix/pipeline/en/__init__.py
 src/stylo_metrix/pipeline/en/custom_preprocessing.py
 src/stylo_metrix/pipeline/en/dictionary_en.py
 src/stylo_metrix/pipeline/en/grammar.py
-src/stylo_metrix/pipeline/en/metrics.py
 src/stylo_metrix/pipeline/en/params.py
 src/stylo_metrix/pipeline/en/pos_tagger.py
+src/stylo_metrix/pipeline/en/psycholinguistics.py
+src/stylo_metrix/pipeline/en/stylistic.py
 src/stylo_metrix/pipeline/pl/__init__.py
-src/stylo_metrix/pipeline/pl/metrics.py
+src/stylo_metrix/pipeline/pl/matcher_component.py
 src/stylo_metrix/pipeline/pl/params.py
 src/stylo_metrix/pipeline/pl/pos_tagger.py
 src/stylo_metrix/pipeline/pl/psycholinguistic.py
 src/stylo_metrix/pipeline/pl/sentence_segmenter.py
 src/stylo_metrix/pipeline/pl/pl_nask/__init__.py
 src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py
 src/stylo_metrix/pipeline/pl/pl_nask/pos.py
 src/stylo_metrix/pipeline/pl/resources/__init__.py
 src/stylo_metrix/pipeline/pl/resources/experimental_data.py
+src/stylo_metrix/pipeline/ukr/__init__.py
+src/stylo_metrix/pipeline/ukr/custom_preprocessing.py
+src/stylo_metrix/pipeline/ukr/dictionary_ukr.py
+src/stylo_metrix/pipeline/ukr/grammar_ukr.py
+src/stylo_metrix/pipeline/ukr/params.py
+src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py
 src/stylo_metrix/structures/__init__.py
-src/stylo_metrix/structures/errors.py
+src/stylo_metrix/structures/category.py
+src/stylo_metrix/structures/language.py
 src/stylo_metrix/structures/metric.py
 src/stylo_metrix/structures/metrics_group.py
-src/stylo_metrix/structures/stylo_metrix_vector.py
+src/stylo_metrix/tools/__init__.py
+src/stylo_metrix/tools/metric_tools.py
```

