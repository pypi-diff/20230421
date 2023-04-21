# Comparing `tmp/ekonlpy-1.1.4.tar.gz` & `tmp/ekonlpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekonlpy-1.1.4.tar", max compression
+gzip compressed data, was "ekonlpy-1.1.5.tar", max compression
```

## Comparing `ekonlpy-1.1.4.tar` & `ekonlpy-1.1.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1071 2023-04-08 00:00:22.710246 ekonlpy-1.1.4/LICENSE
--rw-r--r--   0        0        0     8716 2023-04-08 00:00:22.710246 ekonlpy-1.1.4/README.md
--rw-r--r--   0        0        0     3577 2023-04-08 00:00:55.690322 ekonlpy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-08 00:00:55.634322 ekonlpy-1.1.4/src/ekonlpy/_version.py
--rw-r--r--   0        0        0       31 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/__init__.py
--rw-r--r--   0        0        0      514 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ADJECTIVES.txt
--rw-r--r--   0        0        0      108 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ADVERBS.txt
--rw-r--r--   0        0        0     2583 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/COUNTRY.txt
--rw-r--r--   0        0        0       17 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/CURRENCY.txt
--rw-r--r--   0        0        0    47727 2023-04-08 00:00:22.794246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
--rw-r--r--   0        0        0   475773 2023-04-08 00:00:22.802246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ECON_TERMS.txt
--rwxr-xr-x   0        0        0    77542 2023-04-08 00:00:22.802246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ENTITY.txt
--rw-r--r--   0        0        0     9629 2023-04-08 00:00:22.802246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
--rw-r--r--   0        0        0     2077 2023-04-08 00:00:22.802246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/GENERIC.txt
--rw-r--r--   0        0        0    35442 2023-04-08 00:00:22.802246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
--rw-r--r--   0        0        0    69192 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/INSTITUTION.txt
--rw-r--r--   0        0        0    20594 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/LEMMA.txt
--rw-r--r--   0        0        0     2072 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/NAMES.txt
--rw-r--r--   0        0        0      687 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/NOUNS.txt
--rw-r--r--   0        0        0    10396 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
--rw-r--r--   0        0        0    12378 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
--rw-r--r--   0        0        0    14928 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SECTOR.txt
--rw-r--r--   0        0        0     6456 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS.txt
--rwxr-xr-x   0        0        0      260 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
--rw-r--r--   0        0        0     5788 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
--rwxr-xr-x   0        0        0      598 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
--rw-r--r--   0        0        0    33685 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM.txt
--rw-r--r--   0        0        0      300 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
--rw-r--r--   0        0        0     5329 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
--rw-r--r--   0        0        0    27207 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
--rw-r--r--   0        0        0       87 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
--rw-r--r--   0        0        0       69 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/UNIT.txt
--rw-r--r--   0        0        0       40 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/dictionary/VERBS.txt
--rwxr-xr-x   0        0        0     1677 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Currencies.txt
--rwxr-xr-x   0        0        0      724 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/DatesandNumbers.txt
--rwxr-xr-x   0        0        0     1798 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Generic.txt
--rwxr-xr-x   0        0        0     1622 2023-04-08 00:00:22.806246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Geographic.txt
--rwxr-xr-x   0        0        0  2903900 2023-04-08 00:00:22.814246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/HIV-4.csv
--rwxr-xr-x   0        0        0  8373373 2023-04-08 00:00:22.858246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/LM.csv
--rwxr-xr-x   0        0        0    93474 2023-04-08 00:00:22.858246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Names.txt
--rw-r--r--   0        0        0  3047832 2023-04-08 00:00:22.874246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
--rw-r--r--   0        0        0  2362210 2023-04-08 00:00:22.886246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
--rwxr-xr-x   0        0        0   778128 2023-04-08 00:00:22.890246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
--rwxr-xr-x   0        0        0   661841 2023-04-08 00:00:22.890246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/intensity.csv
--rwxr-xr-x   0        0        0   659879 2023-04-08 00:00:22.894246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/polarity.csv
--rw-r--r--   0        0        0  3226022 2023-04-08 00:00:22.910246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
--rw-r--r--   0        0        0  3832440 2023-04-08 00:00:22.930246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
--rw-r--r--   0        0        0  2735025 2023-04-08 00:00:22.946246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
--rw-r--r--   0        0        0  3749409 2023-04-08 00:00:22.962246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
--rw-r--r--   0        0        0  2835691 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
--rw-r--r--   0        0        0    36419 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
--rw-r--r--   0        0        0   281858 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/data/model/MPKC.nbc
--rw-r--r--   0        0        0    15644 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/data/tagset.py
--rw-r--r--   0        0        0       33 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/etag/__init__.py
--rw-r--r--   0        0        0     4210 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/etag/_template.py
--rwxr-xr-x   0        0        0       63 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/mecab/__init__.py
--rw-r--r--   0        0        0     5687 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/mecab/_mecab.py
--rw-r--r--   0        0        0     4529 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/mecab/_userdic.py
--rw-r--r--   0        0        0        0 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/py.typed
--rwxr-xr-x   0        0        0      236 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/__init__.py
--rwxr-xr-x   0        0        0     4149 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/base.py
--rwxr-xr-x   0        0        0     1741 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/euko.py
--rwxr-xr-x   0        0        0     1010 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/hiv4.py
--rw-r--r--   0        0        0     5936 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/kosac.py
--rwxr-xr-x   0        0        0     1054 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/lm.py
--rw-r--r--   0        0        0    16118 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/mpck.py
--rwxr-xr-x   0        0        0     1840 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/mpko.py
--rwxr-xr-x   0        0        0     9268 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/sentiment/utils.py
--rw-r--r--   0        0        0       66 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/tag/__init__.py
--rw-r--r--   0        0        0    10630 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/tag/_mecab.py
--rw-r--r--   0        0        0     2172 2023-04-08 00:00:22.974246 ekonlpy-1.1.4/src/ekonlpy/tag/_postprocess.py
--rwxr-xr-x   0        0        0        0 2023-04-08 00:00:22.978246 ekonlpy-1.1.4/src/ekonlpy/utils/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-08 00:00:22.978246 ekonlpy-1.1.4/src/ekonlpy/utils/dictionary.py
--rw-r--r--   0        0        0     6668 2023-04-08 00:00:22.978246 ekonlpy-1.1.4/src/ekonlpy/utils/io.py
--rw-r--r--   0        0        0     9613 1970-01-01 00:00:00.000000 ekonlpy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 10:55:46.882415 ekonlpy-1.1.5/LICENSE
+-rw-r--r--   0        0        0     8562 2023-04-21 10:55:46.882415 ekonlpy-1.1.5/README.md
+-rw-r--r--   0        0        0     3617 2023-04-21 10:56:16.467097 ekonlpy-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-21 10:56:16.407096 ekonlpy-1.1.5/src/ekonlpy/_version.py
+-rw-r--r--   0        0        0       31 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/__init__.py
+-rw-r--r--   0        0        0      514 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ADJECTIVES.txt
+-rw-r--r--   0        0        0      108 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ADVERBS.txt
+-rw-r--r--   0        0        0     2583 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/COUNTRY.txt
+-rw-r--r--   0        0        0       17 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/CURRENCY.txt
+-rw-r--r--   0        0        0    47727 2023-04-21 10:55:46.962417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
+-rw-r--r--   0        0        0   475773 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ECON_TERMS.txt
+-rwxr-xr-x   0        0        0    77542 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ENTITY.txt
+-rw-r--r--   0        0        0     9629 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
+-rw-r--r--   0        0        0     2077 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/GENERIC.txt
+-rw-r--r--   0        0        0    35442 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
+-rw-r--r--   0        0        0    69192 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/INSTITUTION.txt
+-rw-r--r--   0        0        0    20594 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/LEMMA.txt
+-rw-r--r--   0        0        0     2072 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/NAMES.txt
+-rw-r--r--   0        0        0      687 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/NOUNS.txt
+-rw-r--r--   0        0        0    10396 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
+-rw-r--r--   0        0        0    12378 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
+-rw-r--r--   0        0        0    14928 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SECTOR.txt
+-rw-r--r--   0        0        0     6456 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS.txt
+-rwxr-xr-x   0        0        0      260 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
+-rw-r--r--   0        0        0     5788 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
+-rwxr-xr-x   0        0        0      598 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
+-rw-r--r--   0        0        0    33685 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM.txt
+-rw-r--r--   0        0        0      300 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
+-rw-r--r--   0        0        0     5329 2023-04-21 10:55:46.970417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
+-rw-r--r--   0        0        0    27207 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
+-rw-r--r--   0        0        0       87 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
+-rw-r--r--   0        0        0       69 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/UNIT.txt
+-rw-r--r--   0        0        0       40 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/dictionary/VERBS.txt
+-rwxr-xr-x   0        0        0     1677 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Currencies.txt
+-rwxr-xr-x   0        0        0      724 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/DatesandNumbers.txt
+-rwxr-xr-x   0        0        0     1798 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Generic.txt
+-rwxr-xr-x   0        0        0     1622 2023-04-21 10:55:46.974417 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Geographic.txt
+-rwxr-xr-x   0        0        0  2903900 2023-04-21 10:55:46.982417 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/HIV-4.csv
+-rwxr-xr-x   0        0        0  8373373 2023-04-21 10:55:47.022418 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/LM.csv
+-rwxr-xr-x   0        0        0    93474 2023-04-21 10:55:47.022418 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Names.txt
+-rw-r--r--   0        0        0  3047832 2023-04-21 10:55:47.038419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
+-rw-r--r--   0        0        0  2362210 2023-04-21 10:55:47.046419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
+-rwxr-xr-x   0        0        0   778128 2023-04-21 10:55:47.050419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
+-rwxr-xr-x   0        0        0   661841 2023-04-21 10:55:47.054419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/intensity.csv
+-rwxr-xr-x   0        0        0   659879 2023-04-21 10:55:47.054419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/polarity.csv
+-rw-r--r--   0        0        0  3226022 2023-04-21 10:55:47.070419 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
+-rw-r--r--   0        0        0  3832440 2023-04-21 10:55:47.090420 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
+-rw-r--r--   0        0        0  2735025 2023-04-21 10:55:47.102420 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
+-rw-r--r--   0        0        0  3749409 2023-04-21 10:55:47.118420 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
+-rw-r--r--   0        0        0  2835691 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
+-rw-r--r--   0        0        0    36419 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
+-rw-r--r--   0        0        0   281858 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/data/model/MPKC.nbc
+-rw-r--r--   0        0        0    15644 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/data/tagset.py
+-rw-r--r--   0        0        0       33 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/etag/__init__.py
+-rw-r--r--   0        0        0     4210 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/etag/_template.py
+-rwxr-xr-x   0        0        0       63 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/mecab/__init__.py
+-rw-r--r--   0        0        0     5687 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/mecab/_mecab.py
+-rw-r--r--   0        0        0     4529 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/mecab/_userdic.py
+-rw-r--r--   0        0        0        0 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/py.typed
+-rwxr-xr-x   0        0        0      236 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/__init__.py
+-rwxr-xr-x   0        0        0     4149 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/base.py
+-rwxr-xr-x   0        0        0     1741 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/euko.py
+-rwxr-xr-x   0        0        0     1010 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/hiv4.py
+-rw-r--r--   0        0        0     5936 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/kosac.py
+-rwxr-xr-x   0        0        0     1054 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/lm.py
+-rw-r--r--   0        0        0    16118 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/mpck.py
+-rwxr-xr-x   0        0        0     1840 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/mpko.py
+-rwxr-xr-x   0        0        0     9268 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/sentiment/utils.py
+-rw-r--r--   0        0        0       66 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/tag/__init__.py
+-rw-r--r--   0        0        0    10630 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/tag/_mecab.py
+-rw-r--r--   0        0        0     2172 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/tag/_postprocess.py
+-rwxr-xr-x   0        0        0        0 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/utils/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/utils/dictionary.py
+-rw-r--r--   0        0        0     6668 2023-04-21 10:55:47.130421 ekonlpy-1.1.5/src/ekonlpy/utils/io.py
+-rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 ekonlpy-1.1.5/PKG-INFO
```

### Comparing `ekonlpy-1.1.4/LICENSE` & `ekonlpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/README.md` & `ekonlpy-1.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # eKoNLPy: Korean NLP Python Library for Economic Analysis
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
+[![pypi-downloads-image]][pypi-url]
 [![license-image]][license-url]
-[![codecov](https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg)](https://codecov.io/gh/entelecheia/eKoNLPy)
+[![codecov][codecov-image]][codecov-url]
+[![zenodo-image]][zenodo-url]
 
 <!-- Links: -->
 
 [pypi-image]: https://badge.fury.io/py/ekonlpy.svg
 [pypi-url]: https://badge.fury.io/py/ekonlpy
 [license-image]: https://img.shields.io/github/license/entelecheia/eKoNLPy
 [license-url]: https://github.com/entelecheia/eKoNLPy/blob/master/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/eKoNLPy?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/eKoNLPy
 [release-url]: https://github.com/entelecheia/eKoNLPy/releases
+[pypi-downloads-image]: https://img.shields.io/pypi/dm/ekonlpy
 [codecov-image]: https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg?token=8I4ORHRREL
 [codecov-url]: https://codecov.io/gh/entelecheia/eKoNLPy
-[zeonodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.6497226.svg
-[zendo-url]: https://doi.org/10.5281/zenodo.6497226
+[zenodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.7809447.svg
+[zenodo-url]: https://doi.org/10.5281/zenodo.7809447
 
-[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
-[conventional commits]: https://conventionalcommits.org
 [repo-url]: https://github.com/entelecheia/eKoNLPy
 [pypi-url]: https://pypi.org/project/ekonlpy
 [docs-url]: https://ekonlpy.entelecheia.ai
 [changelog]: https://github.com/entelecheia/eKoNLPy/blob/master/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/eKoNLPy/blob/master/CONTRIBUTING.md
 
 <!-- Links: -->
```

### Comparing `ekonlpy-1.1.4/pyproject.toml` & `ekonlpy-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eKoNLPy"
-version = "1.1.4"
+version = "1.1.5"
 description = "A Korean natural language processing toolkit for economic analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ekonlpy", from = "src" }]
 homepage = "https://ekonlpy.entelecheia.ai/"
 repository = "https://github.com/entelecheia/eKoNLPy"
@@ -135,14 +135,15 @@
 version_variable = "src/ekonlpy/_version.py:__version__"
 version_source = "tag"
 commit_version_number = true                                          # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
+pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github"                                                       # hosting version control system, gitlab is also supported
 
 [build-system]
```

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ADJECTIVES.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ADJECTIVES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/COUNTRY.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/COUNTRY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ECON_PHRASES.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ECON_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ECON_TERMS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ECON_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/ENTITY.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/ENTITY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/GENERIC.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/GENERIC.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/INSTITUTION.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/INSTITUTION.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/LEMMA.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/LEMMA.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/NAMES.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/NAMES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/NOUNS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SECTOR.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SECTOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Currencies.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Currencies.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/DatesandNumbers.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/DatesandNumbers.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Generic.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Generic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Geographic.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Geographic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/HIV-4.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/HIV-4.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/LM.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/LM.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/Names.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/Names.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/expressive-type.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/expressive-type.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/intensity.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/intensity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/kosac/polarity.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/kosac/polarity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt` & `ekonlpy-1.1.5/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/model/MPKC.nbc` & `ekonlpy-1.1.5/src/ekonlpy/data/model/MPKC.nbc`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/data/tagset.py` & `ekonlpy-1.1.5/src/ekonlpy/data/tagset.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/etag/_template.py` & `ekonlpy-1.1.5/src/ekonlpy/etag/_template.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/mecab/_mecab.py` & `ekonlpy-1.1.5/src/ekonlpy/mecab/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/mecab/_userdic.py` & `ekonlpy-1.1.5/src/ekonlpy/mecab/_userdic.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/base.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/base.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/euko.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/euko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/hiv4.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/hiv4.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/kosac.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/kosac.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/lm.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/lm.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/mpck.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/mpck.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/mpko.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/mpko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/sentiment/utils.py` & `ekonlpy-1.1.5/src/ekonlpy/sentiment/utils.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/tag/_mecab.py` & `ekonlpy-1.1.5/src/ekonlpy/tag/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/tag/_postprocess.py` & `ekonlpy-1.1.5/src/ekonlpy/tag/_postprocess.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/utils/dictionary.py` & `ekonlpy-1.1.5/src/ekonlpy/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/src/ekonlpy/utils/io.py` & `ekonlpy-1.1.5/src/ekonlpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.4/PKG-INFO` & `ekonlpy-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekonlpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Korean natural language processing toolkit for economic analysis
 Home-page: https://ekonlpy.entelecheia.ai/
 License: MIT
 Keywords: KoNLPy,Tokenization,Sentiment analysis,Monetary policy
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -22,33 +22,34 @@
 Description-Content-Type: text/markdown
 
 # eKoNLPy: Korean NLP Python Library for Economic Analysis
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
+[![pypi-downloads-image]][pypi-url]
 [![license-image]][license-url]
-[![codecov](https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg)](https://codecov.io/gh/entelecheia/eKoNLPy)
+[![codecov][codecov-image]][codecov-url]
+[![zenodo-image]][zenodo-url]
 
 <!-- Links: -->
 
 [pypi-image]: https://badge.fury.io/py/ekonlpy.svg
 [pypi-url]: https://badge.fury.io/py/ekonlpy
 [license-image]: https://img.shields.io/github/license/entelecheia/eKoNLPy
 [license-url]: https://github.com/entelecheia/eKoNLPy/blob/master/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/eKoNLPy?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/eKoNLPy
 [release-url]: https://github.com/entelecheia/eKoNLPy/releases
+[pypi-downloads-image]: https://img.shields.io/pypi/dm/ekonlpy
 [codecov-image]: https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg?token=8I4ORHRREL
 [codecov-url]: https://codecov.io/gh/entelecheia/eKoNLPy
-[zeonodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.6497226.svg
-[zendo-url]: https://doi.org/10.5281/zenodo.6497226
+[zenodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.7809447.svg
+[zenodo-url]: https://doi.org/10.5281/zenodo.7809447
 
-[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
-[conventional commits]: https://conventionalcommits.org
 [repo-url]: https://github.com/entelecheia/eKoNLPy
 [pypi-url]: https://pypi.org/project/ekonlpy
 [docs-url]: https://ekonlpy.entelecheia.ai
 [changelog]: https://github.com/entelecheia/eKoNLPy/blob/master/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/eKoNLPy/blob/master/CONTRIBUTING.md
 
 <!-- Links: -->
```

