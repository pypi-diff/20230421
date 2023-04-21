# Comparing `tmp/finalynx-1.8.0.tar.gz` & `tmp/finalynx-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalynx-1.8.0.tar", max compression
+gzip compressed data, was "finalynx-1.8.1.tar", max compression
```

## Comparing `finalynx-1.8.0.tar` & `finalynx-1.8.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    35149 2023-04-21 16:02:25.589810 finalynx-1.8.0/LICENSE
--rw-r--r--   0        0        0     6652 2023-04-21 16:02:25.589810 finalynx-1.8.0/README.md
--rw-r--r--   0        0        0     1345 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/__init__.py
--rw-r--r--   0        0        0      770 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/__main__.py
--rw-r--r--   0        0        0      662 2023-04-21 16:02:26.777826 finalynx-1.8.0/finalynx/__meta__.py
--rw-r--r--   0        0        0      993 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/analyzer.py
--rw-r--r--   0        0        0     3187 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/asset_class.py
--rw-r--r--   0        0        0     2398 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/envelopes.py
--rw-r--r--   0        0        0     2858 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/investment_state.py
--rw-r--r--   0        0        0     5557 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/assistant.py
--rw-r--r--   0        0        0      273 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/console.py
--rw-r--r--   0        0        0      424 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/copilot/__init__.py
--rw-r--r--   0        0        0      593 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/copilot/copilot.py
--rw-r--r--   0        0        0      427 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/dashboard/__init__.py
--rw-r--r--   0        0        0    11713 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/dashboard/dashboard.py
--rw-r--r--   0        0        0      891 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/fetch.py
--rw-r--r--   0        0        0    16256 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/fetch_finary.py
--rw-r--r--   0        0        0       47 2023-04-21 16:02:25.933815 finalynx-1.8.0/finalynx/finary_api/.git
--rw-r--r--   0        0        0      222 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/.github/dependabot.yml
--rw-r--r--   0        0        0     1905 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/.gitignore
--rw-r--r--   0        0        0     1064 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/LICENSE
--rw-r--r--   0        0        0     5099 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/README.md
--rwxr-xr-x   0        0        0      170 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/check.sh
--rw-r--r--   0        0        0       32 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/credentials.json.tpl
--rw-r--r--   0        0        0      691 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/__init__.py
--rw-r--r--   0        0        0    15625 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/__main__.py
--rw-r--r--   0        0        0      323 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/auth.py
--rw-r--r--   0        0        0      694 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/bank_account_types.py
--rw-r--r--   0        0        0      118 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/constants.py
--rw-r--r--   0        0        0      241 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/crypto_chains.py
--rw-r--r--   0        0        0      824 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/currencies.py
--rw-r--r--   0        0        0      308 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/institutions.py
--rw-r--r--   0        0        0      511 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/precious_metals.py
--rw-r--r--   0        0        0      494 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/scpis.py
--rw-r--r--   0        0        0     3276 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/securities.py
--rw-r--r--   0        0        0     2308 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/signin.py
--rw-r--r--   0        0        0     4177 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_cryptos.py
--rw-r--r--   0        0        0      246 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_me.py
--rw-r--r--   0        0        0     1670 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_portfolio.py
--rw-r--r--   0        0        0     1865 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_precious_metals.py
--rw-r--r--   0        0        0      222 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_real_estates.py
--rw-r--r--   0        0        0      208 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_scpis.py
--rw-r--r--   0        0        0     5680 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_securities.py
--rw-r--r--   0        0        0      221 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_startups.py
--rw-r--r--   0        0        0      196 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/utils.py
--rw-r--r--   0        0        0     3253 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/views.py
--rw-r--r--   0        0        0      478 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/mypy.ini
--rw-r--r--   0        0        0      195 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/requirements-tests.txt
--rw-r--r--   0        0        0       60 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/requirements.txt
--rw-r--r--   0        0        0      224 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/setup.cfg
--rw-r--r--   0        0        0       50 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/cryptos.csv
--rw-r--r--   0        0        0      172 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/stocks.csv
--rw-r--r--   0        0        0      340 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/stocks.json
--rw-r--r--   0        0        0      153 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/__init__.py
--rw-r--r--   0        0        0      739 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/json.py
--rw-r--r--   0        0        0     1007 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/parser.py
--rw-r--r--   0        0        0     2016 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/bucket.py
--rw-r--r--   0        0        0      860 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/constants.py
--rw-r--r--   0        0        0     2427 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/envelope.py
--rw-r--r--   0        0        0     7451 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/folder.py
--rw-r--r--   0        0        0      422 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/hierarchy.py
--rw-r--r--   0        0        0     2436 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/line.py
--rw-r--r--   0        0        0     8141 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/node.py
--rw-r--r--   0        0        0     1195 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/portfolio.py
--rw-r--r--   0        0        0     3624 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/render.py
--rw-r--r--   0        0        0    11976 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/targets.py
--rw-r--r--   0        0        0      419 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/simulator/__init__.py
--rw-r--r--   0        0        0     2385 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/simulator/simulator.py
--rw-r--r--   0        0        0     1705 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/usage.py
--rw-r--r--   0        0        0     1713 2023-04-21 16:02:26.777826 finalynx-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     7539 1970-01-01 00:00:00.000000 finalynx-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 17:47:02.702652 finalynx-1.8.1/LICENSE
+-rw-r--r--   0        0        0     6890 2023-04-21 17:47:02.702652 finalynx-1.8.1/README.md
+-rw-r--r--   0        0        0     1345 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/__init__.py
+-rw-r--r--   0        0        0      770 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/__main__.py
+-rw-r--r--   0        0        0      662 2023-04-21 17:47:04.138664 finalynx-1.8.1/finalynx/__meta__.py
+-rw-r--r--   0        0        0      993 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/analyzer/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3187 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/analyzer/asset_class.py
+-rw-r--r--   0        0        0     2398 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/analyzer/envelopes.py
+-rw-r--r--   0        0        0     2858 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/analyzer/investment_state.py
+-rw-r--r--   0        0        0     6022 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/assistant.py
+-rw-r--r--   0        0        0      273 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/console.py
+-rw-r--r--   0        0        0      424 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/copilot/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/copilot/copilot.py
+-rw-r--r--   0        0        0      427 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/dashboard/__init__.py
+-rw-r--r--   0        0        0    11713 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/dashboard/dashboard.py
+-rw-r--r--   0        0        0      891 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/fetch/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/fetch/fetch.py
+-rw-r--r--   0        0        0    16256 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/fetch/fetch_finary.py
+-rw-r--r--   0        0        0       47 2023-04-21 17:47:03.262657 finalynx-1.8.1/finalynx/finary_api/.git
+-rw-r--r--   0        0        0      222 2023-04-21 17:47:03.266657 finalynx-1.8.1/finalynx/finary_api/.github/dependabot.yml
+-rw-r--r--   0        0        0     1905 2023-04-21 17:47:03.266657 finalynx-1.8.1/finalynx/finary_api/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-21 17:47:03.266657 finalynx-1.8.1/finalynx/finary_api/LICENSE
+-rw-r--r--   0        0        0     5099 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/README.md
+-rwxr-xr-x   0        0        0      170 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/check.sh
+-rw-r--r--   0        0        0       32 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/credentials.json.tpl
+-rw-r--r--   0        0        0      691 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/__init__.py
+-rw-r--r--   0        0        0    15625 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/__main__.py
+-rw-r--r--   0        0        0      323 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/auth.py
+-rw-r--r--   0        0        0      694 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/bank_account_types.py
+-rw-r--r--   0        0        0      118 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/constants.py
+-rw-r--r--   0        0        0      241 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/crypto_chains.py
+-rw-r--r--   0        0        0      824 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/currencies.py
+-rw-r--r--   0        0        0      308 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/institutions.py
+-rw-r--r--   0        0        0      511 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/precious_metals.py
+-rw-r--r--   0        0        0      494 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/scpis.py
+-rw-r--r--   0        0        0     3276 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/securities.py
+-rw-r--r--   0        0        0     2308 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/signin.py
+-rw-r--r--   0        0        0     4177 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_cryptos.py
+-rw-r--r--   0        0        0      246 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_me.py
+-rw-r--r--   0        0        0     1670 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_real_estates.py
+-rw-r--r--   0        0        0      208 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_scpis.py
+-rw-r--r--   0        0        0     5680 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_securities.py
+-rw-r--r--   0        0        0      221 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/user_startups.py
+-rw-r--r--   0        0        0      196 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/finary_api/views.py
+-rw-r--r--   0        0        0      478 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/mypy.ini
+-rw-r--r--   0        0        0      195 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/requirements.txt
+-rw-r--r--   0        0        0      224 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/setup.cfg
+-rw-r--r--   0        0        0       50 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/tests/data/cryptos.csv
+-rw-r--r--   0        0        0      172 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/tests/data/stocks.csv
+-rw-r--r--   0        0        0      340 2023-04-21 17:47:03.270657 finalynx-1.8.1/finalynx/finary_api/tests/data/stocks.json
+-rw-r--r--   0        0        0      153 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/parse/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/parse/json.py
+-rw-r--r--   0        0        0     1007 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/parse/parser.py
+-rw-r--r--   0        0        0     2016 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/bucket.py
+-rw-r--r--   0        0        0      860 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/constants.py
+-rw-r--r--   0        0        0     2427 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/envelope.py
+-rw-r--r--   0        0        0     7451 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/folder.py
+-rw-r--r--   0        0        0      422 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/hierarchy.py
+-rw-r--r--   0        0        0     2436 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/line.py
+-rw-r--r--   0        0        0     8332 2023-04-21 17:47:02.718652 finalynx-1.8.1/finalynx/portfolio/node.py
+-rw-r--r--   0        0        0     1195 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/portfolio/portfolio.py
+-rw-r--r--   0        0        0     3624 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/portfolio/render.py
+-rw-r--r--   0        0        0    11976 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/portfolio/targets.py
+-rw-r--r--   0        0        0      419 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/simulator/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/simulator/simulator.py
+-rw-r--r--   0        0        0     2086 2023-04-21 17:47:02.722652 finalynx-1.8.1/finalynx/usage.py
+-rw-r--r--   0        0        0     1713 2023-04-21 17:47:04.138664 finalynx-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 finalynx-1.8.1/PKG-INFO
```

### Comparing `finalynx-1.8.0/LICENSE` & `finalynx-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/README.md` & `finalynx-1.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 from finalynx import Portfolio, Assistant
 portfolio = Portfolio()  # <- your custom configuration here
 Assistant(portfolio).run()
 ```
 
 You can now populate the `Portfolio` class with your own custom hierarchy by taking inspiration from the [`demo.py`](https://github.com/MadeInPierre/finalynx/blob/main/examples/demo.py) example or by reading the [Getting Started](https://finalynx.readthedocs.io/en/latest/tutorials/getting_started.html) guide in the documentation. For additional details, checkout the full [API Reference](https://finalynx.readthedocs.io/en/latest/apidocs/index.html) or [ask a question](https://github.com/MadeInPierre/finalynx/discussions/new?category=q-a).
 
+Once you have a fully defined portfolio tree with sensible targets, you can display how much you need to invest in each line using:
+
+```sh
+python your_config.py delta  # type --help for other options, like launching a web dashboard!
+```
+
 ## 👨‍💻 Feedback & Contributions
 This repository is at a very early stage. Unfortunately, I won't have time to make this tool work for everyone by default, but you are welcome to extend this project (or [hire me](https://www.buymeacoffee.com/MadeInPierre/commissions) if you can't develop it yourself). Pull requests, [issues](https://github.com/MadeInPierre/finalynx/issues/new) (🇬🇧 preferably) and [open discussions](https://github.com/MadeInPierre/finalynx/discussions/new) (🇬🇧/🇫🇷) are warmly welcome!
 
 If you would like to contribute to this project, welcome on board and thanks for your interest! 🎉 Please read the [contribution guidelines](https://github.com/MadeInPierre/finalynx/blob/main/CONTRIBUTING.md) to setup the project on your machine and agree on common conventions.
 
 ## 📄 License
 This project is under the [GPLv3 License](https://github.com/MadeInPierre/finalynx/blob/main/LICENSE) meaning anyone can use, share, extend, and contribute to this project as long as their changes are integrated to this repo or also published using GPLv3. Please contact me for any specific licensing requests.
```

#### html2text {}

```diff
@@ -43,15 +43,18 @@
 You can now populate the `Portfolio` class with your own custom hierarchy by
 taking inspiration from the [`demo.py`](https://github.com/MadeInPierre/
 finalynx/blob/main/examples/demo.py) example or by reading the [Getting
 Started](https://finalynx.readthedocs.io/en/latest/tutorials/
 getting_started.html) guide in the documentation. For additional details,
 checkout the full [API Reference](https://finalynx.readthedocs.io/en/latest/
 apidocs/index.html) or [ask a question](https://github.com/MadeInPierre/
-finalynx/discussions/new?category=q-a). ## ð¨âð» Feedback & Contributions
+finalynx/discussions/new?category=q-a). Once you have a fully defined portfolio
+tree with sensible targets, you can display how much you need to invest in each
+line using: ```sh python your_config.py delta # type --help for other options,
+like launching a web dashboard! ``` ## ð¨âð» Feedback & Contributions
 This repository is at a very early stage. Unfortunately, I won't have time to
 make this tool work for everyone by default, but you are welcome to extend this
 project (or [hire me](https://www.buymeacoffee.com/MadeInPierre/commissions) if
 you can't develop it yourself). Pull requests, [issues](https://github.com/
 MadeInPierre/finalynx/issues/new) (ð¬ð§ preferably) and [open discussions]
 (https://github.com/MadeInPierre/finalynx/discussions/new) (ð¬ð§/ð«ð·)
 are warmly welcome! If you would like to contribute to this project, welcome on
```

### Comparing `finalynx-1.8.0/finalynx/__init__.py` & `finalynx-1.8.1/finalynx/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/__main__.py` & `finalynx-1.8.1/finalynx/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/__meta__.py` & `finalynx-1.8.1/finalynx/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ```{warning}
 Do not manually change this information.
 ```
 
 Metadata information about Finalynx. This file is used by Fynalinx and updated by the CI/CD pipeline.
 """
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 __author__ = "Pierre Laclau (MadeInPierre)"
 
 __copyright__ = """
 Copyright (c) 2023, MadeInPierre
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
```

### Comparing `finalynx-1.8.0/finalynx/analyzer/__init__.py` & `finalynx-1.8.1/finalynx/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/analyzer/analyzer.py` & `finalynx-1.8.1/finalynx/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/analyzer/asset_class.py` & `finalynx-1.8.1/finalynx/analyzer/asset_class.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/analyzer/envelopes.py` & `finalynx-1.8.1/finalynx/analyzer/envelopes.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/analyzer/investment_state.py` & `finalynx-1.8.1/finalynx/analyzer/investment_state.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/assistant.py` & `finalynx-1.8.1/finalynx/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         copilot: Optional[Copilot] = None,
         ignore_orphans: bool = False,
         clear_cache: bool = False,
         force_signin: bool = False,
         hide_amounts: bool = False,
         hide_root: bool = False,
         show_data: bool = False,
+        hide_deltas: bool = False,
         launch_dashboard: bool = False,
         output_format: str = "[console]",
     ):
         self.portfolio = portfolio
         self.scenario = scenario if scenario else Simulator()  # TODO Coming soon
         self.copilot = copilot if copilot else Copilot()  # TODO Coming soon
 
@@ -64,22 +65,22 @@
         self.clear_cache = clear_cache
         self.force_signin = force_signin
         self.hide_amounts = hide_amounts
         self.hide_root = hide_root
         self.show_data = show_data
         self.launch_dashboard = launch_dashboard
         self.output_format = output_format
+        self.hide_deltas = hide_deltas
 
         self._parse_args()
 
     def _parse_args(self) -> None:
         """Internal method that parses the command-line options and activates the options
         in the corresponding modules.
         """
-
         args = docopt(__doc__, version=__version__)
         if args["--ignore-orphans"]:
             self.ignore_orphans = True
         if args["--clear-cache"]:
             self.clear_cache = True
         if args["--force-signin"]:
             self.clear_cache = True
@@ -90,14 +91,24 @@
             self.hide_root = True
         if args["--show-data"]:
             self.show_data = True
         if args["dashboard"]:
             self.launch_dashboard = True
         if args["--format"]:
             self.output_format = args["--format"]
+        if args["delta"]:
+            self.output_format = "[console_delta]"
+        if args["targets"]:
+            self.output_format = "[console_targets]"
+            self.hide_deltas = True
+        if args["text"]:
+            self.output_format = "[text]"
+            self.hide_deltas = True
+        if args["--hide-deltas"]:
+            self.hide_deltas = True
 
     def run(self) -> None:
         """Main function to run once your configuration is fully defined.
 
         This function will fetch the data from your Finary account, process the thr targets in the portfolio tree,
         run your simulation, generate recommendations, and format the output nicely to the console.
         """
@@ -120,15 +131,15 @@
                 output_format=self.output_format,
                 hide_root=self.hide_root,
                 hide_amounts=self.hide_amounts,
             ),
         ]
 
         # Display deltas only if not already printed in the main tree
-        if "delta" not in self.output_format:
+        if not self.hide_deltas and "delta" not in self.output_format:
             render.append(self.portfolio.tree_delta())
 
         # Final set of results to be displayed
         panels = [Columns([Text("  ")] + render)]  # type: ignore
 
         # Show the data fetched from Finary if specified
         if self.show_data:
```

### Comparing `finalynx-1.8.0/finalynx/copilot/copilot.py` & `finalynx-1.8.1/finalynx/copilot/copilot.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/dashboard/dashboard.py` & `finalynx-1.8.1/finalynx/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/fetch/__init__.py` & `finalynx-1.8.1/finalynx/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/fetch/fetch.py` & `finalynx-1.8.1/finalynx/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/fetch/fetch_finary.py` & `finalynx-1.8.1/finalynx/fetch/fetch_finary.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/.gitignore` & `finalynx-1.8.1/finalynx/finary_api/.gitignore`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/LICENSE` & `finalynx-1.8.1/finalynx/finary_api/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/README.md` & `finalynx-1.8.1/finalynx/finary_api/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/__init__.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/__main__.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/bank_account_types.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/currencies.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/currencies.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/cryptocom.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/securities.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/signin.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/signin.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_cryptos.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_generic_assets.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_holdings_accounts.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_portfolio.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_precious_metals.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/user_securities.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/user_securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/finary_api/finary_api/views.py` & `finalynx-1.8.1/finalynx/finary_api/finary_api/views.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/parse/json.py` & `finalynx-1.8.1/finalynx/parse/json.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/parse/parser.py` & `finalynx-1.8.1/finalynx/parse/parser.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/__init__.py` & `finalynx-1.8.1/finalynx/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/bucket.py` & `finalynx-1.8.1/finalynx/portfolio/bucket.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/constants.py` & `finalynx-1.8.1/finalynx/portfolio/constants.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/envelope.py` & `finalynx-1.8.1/finalynx/portfolio/envelope.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/folder.py` & `finalynx-1.8.1/finalynx/portfolio/folder.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/line.py` & `finalynx-1.8.1/finalynx/portfolio/line.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/node.py` & `finalynx-1.8.1/finalynx/portfolio/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         if target is not None:
             target.set_parent(self)
 
         # Setup custom aliases for node rendering
         render_aliases: Dict[str, str] = {
             "[text]": "[target_text][prehint] [name] [hint][newline]",
-            "[console]": "[target][dim white][prehint][/] [account_code][name_color][name][/] [dim white][hint][/][newline]",
+            "[console]": "[target] [account_code][name_color][name][/] [dim white][hint][/][newline]",
             "[console_delta]": "[delta][account_code][name_color][name][/] [newline]",
             "[console_targets]": "[bold green][goal][/][account_code][name_color][name][/][newline]",
             "[text_targets]": "[goal][name][newline]",
             "[dashboard_tree]": "[amount] [currency] [name]",
             "[dashboard_console]": "[bold][target][/][bright_black][prehint][/] [name_color][name][/] [bright_black][hint][/][newline]",
             "[target]": "[[target_color]][target_text][/]",
             "[target_text]": "[target_symbol] [amount] [currency]",
@@ -157,15 +157,20 @@
     def _render_delta(self) -> str:
         delta, check = round(self.get_delta()), self.target.check()
         if delta == 0 or check == Target.RESULT_NONE:
             return ""
         if check == Target.RESULT_OK:
             return "[green]✓[/] "
         color = "green" if delta > 0 else "red"
-        return f"[{color}]{'+' if delta > 0 else ''}{delta} €[/] "
+        max_length = (
+            np.max([len(str(abs(round(c.get_delta())))) for c in self.parent.children])
+            if (self.parent and self.parent.children)
+            else 0
+        )
+        return f"[{color}]{'+' if delta > 0 else '-'}{abs(delta):>{max_length}} €[/] "
 
     def _render_name(self) -> str:
         """:returns: A formatted rendering of the node name."""
         return self.name
 
     def _render_name_color(self) -> str:
         """:returns: A formatted rendering of the node name."""
```

### Comparing `finalynx-1.8.0/finalynx/portfolio/portfolio.py` & `finalynx-1.8.1/finalynx/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/render.py` & `finalynx-1.8.1/finalynx/portfolio/render.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/portfolio/targets.py` & `finalynx-1.8.1/finalynx/portfolio/targets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/simulator/simulator.py` & `finalynx-1.8.1/finalynx/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.0/finalynx/usage.py` & `finalynx-1.8.1/finalynx/usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
 # Define the finalynx command-line usage which varies depending on how it's called.
 # When "sys.argv[0]" is the path to a python script, it means the user is using its own script.
 # Otherwise, the user is using
 __doc__ = f"""
 Finalynx command line v{__version__}
 Usage:
-  finalynx {main_filter(main_usage)}[--format=string] [dashboard] [options]
+  finalynx {main_filter(main_usage)}[targets | delta | text | --format=string] [dashboard] [options]
   finalynx (-h | --help)
   finalynx (-v | --version)
 
 Options:
   -h --help            Show this help message and exit
   -v --version         Display the current version and exit
 {main_filter(main_options)}
   dashboard            Launch an interactive web dashboard!
 
+  --hide-deltas        Don't show delta investment recommendations next to the tree
   --format=string      Customize the output format to your own style and information
+  targets              Shortcut to --format="[console_targets]" (show target values instead of amounts)
+  delta                Shortcut to --format="[console_delta]" (show deltas instead of amounts)
+  text                 Shortcut to --format="[console_text]" (no colors)
 
   -i --ignore-orphans  Ignore fetched lines that you didn't reference in your portfolio
   -c --clear-cache     Delete any data from Finary that was cached locally
   -f --force-signin    Clear cache, cookies and credentials files to sign in again
   -a --hide-amounts    Display your portfolio with dots instead of the real values (easier to share)
   -d --show-data       Show what has been fetched online (e.g. from your Finary account)
   -r --hide-root       Display your portfolio without the root (cosmetic preference)
```

### Comparing `finalynx-1.8.0/pyproject.toml` & `finalynx-1.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finalynx"
-version = "1.8.0"
+version = "1.8.1"
 description = "A command line investment assistant to organize your portfolio and simulate its future to reach your life goals."
 authors = ["MadeInPierre <pielaclau@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "finalynx"}]
 include = [{ path = "finalynx/finary_api/**/*" }]
 
@@ -48,15 +48,15 @@
 upload_to_pypi = true
 upload_to_release = true
 commit_subject = "chore(release): auto bump version to {version}"
 build_command = "pip install poetry && poetry build"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.8.0"
+version = "1.8.1"
 tag_format = "v$version"
 
 [tool.mypy]
 exclude = [
     "finary_api/*",
     "docs/*",
     "tests/*.py"
```

### Comparing `finalynx-1.8.0/PKG-INFO` & `finalynx-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalynx
-Version: 1.8.0
+Version: 1.8.1
 Summary: A command line investment assistant to organize your portfolio and simulate its future to reach your life goals.
 License: GPLv3
 Author: MadeInPierre
 Author-email: pielaclau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -82,14 +82,20 @@
 from finalynx import Portfolio, Assistant
 portfolio = Portfolio()  # <- your custom configuration here
 Assistant(portfolio).run()
 ```
 
 You can now populate the `Portfolio` class with your own custom hierarchy by taking inspiration from the [`demo.py`](https://github.com/MadeInPierre/finalynx/blob/main/examples/demo.py) example or by reading the [Getting Started](https://finalynx.readthedocs.io/en/latest/tutorials/getting_started.html) guide in the documentation. For additional details, checkout the full [API Reference](https://finalynx.readthedocs.io/en/latest/apidocs/index.html) or [ask a question](https://github.com/MadeInPierre/finalynx/discussions/new?category=q-a).
 
+Once you have a fully defined portfolio tree with sensible targets, you can display how much you need to invest in each line using:
+
+```sh
+python your_config.py delta  # type --help for other options, like launching a web dashboard!
+```
+
 ## 👨‍💻 Feedback & Contributions
 This repository is at a very early stage. Unfortunately, I won't have time to make this tool work for everyone by default, but you are welcome to extend this project (or [hire me](https://www.buymeacoffee.com/MadeInPierre/commissions) if you can't develop it yourself). Pull requests, [issues](https://github.com/MadeInPierre/finalynx/issues/new) (🇬🇧 preferably) and [open discussions](https://github.com/MadeInPierre/finalynx/discussions/new) (🇬🇧/🇫🇷) are warmly welcome!
 
 If you would like to contribute to this project, welcome on board and thanks for your interest! 🎉 Please read the [contribution guidelines](https://github.com/MadeInPierre/finalynx/blob/main/CONTRIBUTING.md) to setup the project on your machine and agree on common conventions.
 
 ## 📄 License
 This project is under the [GPLv3 License](https://github.com/MadeInPierre/finalynx/blob/main/LICENSE) meaning anyone can use, share, extend, and contribute to this project as long as their changes are integrated to this repo or also published using GPLv3. Please contact me for any specific licensing requests.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalynx Version: 1.8.0 Summary: A command line
+Metadata-Version: 2.1 Name: finalynx Version: 1.8.1 Summary: A command line
 investment assistant to organize your portfolio and simulate its future to
 reach your life goals. License: GPLv3 Author: MadeInPierre Author-email:
 pielaclau@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2)
@@ -55,15 +55,18 @@
 You can now populate the `Portfolio` class with your own custom hierarchy by
 taking inspiration from the [`demo.py`](https://github.com/MadeInPierre/
 finalynx/blob/main/examples/demo.py) example or by reading the [Getting
 Started](https://finalynx.readthedocs.io/en/latest/tutorials/
 getting_started.html) guide in the documentation. For additional details,
 checkout the full [API Reference](https://finalynx.readthedocs.io/en/latest/
 apidocs/index.html) or [ask a question](https://github.com/MadeInPierre/
-finalynx/discussions/new?category=q-a). ## ð¨âð» Feedback & Contributions
+finalynx/discussions/new?category=q-a). Once you have a fully defined portfolio
+tree with sensible targets, you can display how much you need to invest in each
+line using: ```sh python your_config.py delta # type --help for other options,
+like launching a web dashboard! ``` ## ð¨âð» Feedback & Contributions
 This repository is at a very early stage. Unfortunately, I won't have time to
 make this tool work for everyone by default, but you are welcome to extend this
 project (or [hire me](https://www.buymeacoffee.com/MadeInPierre/commissions) if
 you can't develop it yourself). Pull requests, [issues](https://github.com/
 MadeInPierre/finalynx/issues/new) (ð¬ð§ preferably) and [open discussions]
 (https://github.com/MadeInPierre/finalynx/discussions/new) (ð¬ð§/ð«ð·)
 are warmly welcome! If you would like to contribute to this project, welcome on
```

