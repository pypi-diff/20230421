# Comparing `tmp/finalynx-1.7.0.tar.gz` & `tmp/finalynx-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalynx-1.7.0.tar", max compression
+gzip compressed data, was "finalynx-1.8.0.tar", max compression
```

## Comparing `finalynx-1.7.0.tar` & `finalynx-1.8.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    35149 2023-04-20 08:07:53.173183 finalynx-1.7.0/LICENSE
--rw-r--r--   0        0        0     6652 2023-04-20 08:07:53.173183 finalynx-1.7.0/README.md
--rw-r--r--   0        0        0     1340 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/__init__.py
--rw-r--r--   0        0        0      770 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/__main__.py
--rw-r--r--   0        0        0      662 2023-04-20 08:07:54.501173 finalynx-1.7.0/finalynx/__meta__.py
--rw-r--r--   0        0        0      993 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/analyzer.py
--rw-r--r--   0        0        0     3187 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/asset_class.py
--rw-r--r--   0        0        0     2398 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/envelopes.py
--rw-r--r--   0        0        0     2858 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/investment_state.py
--rw-r--r--   0        0        0     5506 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/assistant.py
--rw-r--r--   0        0        0      273 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/console.py
--rw-r--r--   0        0        0      424 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/copilot/__init__.py
--rw-r--r--   0        0        0      593 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/copilot/copilot.py
--rw-r--r--   0        0        0      427 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/dashboard/__init__.py
--rw-r--r--   0        0        0    11345 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/dashboard/dashboard.py
--rw-r--r--   0        0        0      891 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/fetch.py
--rw-r--r--   0        0        0    16256 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/fetch_finary.py
--rw-r--r--   0        0        0       47 2023-04-20 08:07:53.689179 finalynx-1.7.0/finalynx/finary_api/.git
--rw-r--r--   0        0        0      222 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/.github/dependabot.yml
--rw-r--r--   0        0        0     1905 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/.gitignore
--rw-r--r--   0        0        0     1064 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/LICENSE
--rw-r--r--   0        0        0     5099 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/README.md
--rwxr-xr-x   0        0        0      170 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/check.sh
--rw-r--r--   0        0        0       32 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/credentials.json.tpl
--rw-r--r--   0        0        0      691 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/__init__.py
--rw-r--r--   0        0        0    15625 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/__main__.py
--rw-r--r--   0        0        0      323 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/auth.py
--rw-r--r--   0        0        0      694 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/bank_account_types.py
--rw-r--r--   0        0        0      118 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/constants.py
--rw-r--r--   0        0        0      241 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/crypto_chains.py
--rw-r--r--   0        0        0      824 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/currencies.py
--rw-r--r--   0        0        0      308 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/institutions.py
--rw-r--r--   0        0        0      511 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/precious_metals.py
--rw-r--r--   0        0        0      494 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/scpis.py
--rw-r--r--   0        0        0     3276 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/securities.py
--rw-r--r--   0        0        0     2308 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/signin.py
--rw-r--r--   0        0        0     4177 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_cryptos.py
--rw-r--r--   0        0        0      246 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_me.py
--rw-r--r--   0        0        0     1670 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_portfolio.py
--rw-r--r--   0        0        0     1865 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_precious_metals.py
--rw-r--r--   0        0        0      222 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_real_estates.py
--rw-r--r--   0        0        0      208 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_scpis.py
--rw-r--r--   0        0        0     5680 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_securities.py
--rw-r--r--   0        0        0      221 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_startups.py
--rw-r--r--   0        0        0      196 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/utils.py
--rw-r--r--   0        0        0     3253 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/views.py
--rw-r--r--   0        0        0      478 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/mypy.ini
--rw-r--r--   0        0        0      195 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/requirements-tests.txt
--rw-r--r--   0        0        0       60 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/requirements.txt
--rw-r--r--   0        0        0      224 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/setup.cfg
--rw-r--r--   0        0        0       50 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/cryptos.csv
--rw-r--r--   0        0        0      172 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/stocks.csv
--rw-r--r--   0        0        0      340 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/stocks.json
--rw-r--r--   0        0        0      153 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/__init__.py
--rw-r--r--   0        0        0      739 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/json.py
--rw-r--r--   0        0        0     1007 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/parser.py
--rw-r--r--   0        0        0     2016 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/bucket.py
--rw-r--r--   0        0        0      860 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/constants.py
--rw-r--r--   0        0        0     2133 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/envelope.py
--rw-r--r--   0        0        0     6934 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/folder.py
--rw-r--r--   0        0        0      422 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/hierarchy.py
--rw-r--r--   0        0        0     2436 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/line.py
--rw-r--r--   0        0        0     6833 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/node.py
--rw-r--r--   0        0        0     1195 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/portfolio.py
--rw-r--r--   0        0        0     3529 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/render.py
--rw-r--r--   0        0        0    11163 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/targets.py
--rw-r--r--   0        0        0      419 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/simulator/__init__.py
--rw-r--r--   0        0        0     2262 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/simulator/simulator.py
--rw-r--r--   0        0        0     1705 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/usage.py
--rw-r--r--   0        0        0     1713 2023-04-20 08:07:54.501173 finalynx-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     7539 1970-01-01 00:00:00.000000 finalynx-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 16:02:25.589810 finalynx-1.8.0/LICENSE
+-rw-r--r--   0        0        0     6652 2023-04-21 16:02:25.589810 finalynx-1.8.0/README.md
+-rw-r--r--   0        0        0     1345 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/__init__.py
+-rw-r--r--   0        0        0      770 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/__main__.py
+-rw-r--r--   0        0        0      662 2023-04-21 16:02:26.777826 finalynx-1.8.0/finalynx/__meta__.py
+-rw-r--r--   0        0        0      993 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3187 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/asset_class.py
+-rw-r--r--   0        0        0     2398 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/envelopes.py
+-rw-r--r--   0        0        0     2858 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/analyzer/investment_state.py
+-rw-r--r--   0        0        0     5557 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/assistant.py
+-rw-r--r--   0        0        0      273 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/console.py
+-rw-r--r--   0        0        0      424 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/copilot/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/copilot/copilot.py
+-rw-r--r--   0        0        0      427 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/dashboard/__init__.py
+-rw-r--r--   0        0        0    11713 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/dashboard/dashboard.py
+-rw-r--r--   0        0        0      891 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/fetch.py
+-rw-r--r--   0        0        0    16256 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/fetch/fetch_finary.py
+-rw-r--r--   0        0        0       47 2023-04-21 16:02:25.933815 finalynx-1.8.0/finalynx/finary_api/.git
+-rw-r--r--   0        0        0      222 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/.github/dependabot.yml
+-rw-r--r--   0        0        0     1905 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/LICENSE
+-rw-r--r--   0        0        0     5099 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/README.md
+-rwxr-xr-x   0        0        0      170 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/check.sh
+-rw-r--r--   0        0        0       32 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/credentials.json.tpl
+-rw-r--r--   0        0        0      691 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/__init__.py
+-rw-r--r--   0        0        0    15625 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/__main__.py
+-rw-r--r--   0        0        0      323 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/auth.py
+-rw-r--r--   0        0        0      694 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/bank_account_types.py
+-rw-r--r--   0        0        0      118 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/constants.py
+-rw-r--r--   0        0        0      241 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/crypto_chains.py
+-rw-r--r--   0        0        0      824 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/currencies.py
+-rw-r--r--   0        0        0      308 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/institutions.py
+-rw-r--r--   0        0        0      511 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/precious_metals.py
+-rw-r--r--   0        0        0      494 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/scpis.py
+-rw-r--r--   0        0        0     3276 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/securities.py
+-rw-r--r--   0        0        0     2308 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/signin.py
+-rw-r--r--   0        0        0     4177 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_cryptos.py
+-rw-r--r--   0        0        0      246 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_me.py
+-rw-r--r--   0        0        0     1670 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_real_estates.py
+-rw-r--r--   0        0        0      208 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_scpis.py
+-rw-r--r--   0        0        0     5680 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_securities.py
+-rw-r--r--   0        0        0      221 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/user_startups.py
+-rw-r--r--   0        0        0      196 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/finary_api/views.py
+-rw-r--r--   0        0        0      478 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/mypy.ini
+-rw-r--r--   0        0        0      195 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/requirements.txt
+-rw-r--r--   0        0        0      224 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/setup.cfg
+-rw-r--r--   0        0        0       50 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/cryptos.csv
+-rw-r--r--   0        0        0      172 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/stocks.csv
+-rw-r--r--   0        0        0      340 2023-04-21 16:02:25.941815 finalynx-1.8.0/finalynx/finary_api/tests/data/stocks.json
+-rw-r--r--   0        0        0      153 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/json.py
+-rw-r--r--   0        0        0     1007 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/parse/parser.py
+-rw-r--r--   0        0        0     2016 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/bucket.py
+-rw-r--r--   0        0        0      860 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/constants.py
+-rw-r--r--   0        0        0     2427 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/envelope.py
+-rw-r--r--   0        0        0     7451 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/folder.py
+-rw-r--r--   0        0        0      422 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/hierarchy.py
+-rw-r--r--   0        0        0     2436 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/line.py
+-rw-r--r--   0        0        0     8141 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/node.py
+-rw-r--r--   0        0        0     1195 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/portfolio.py
+-rw-r--r--   0        0        0     3624 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/render.py
+-rw-r--r--   0        0        0    11976 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/portfolio/targets.py
+-rw-r--r--   0        0        0      419 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/simulator/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/simulator/simulator.py
+-rw-r--r--   0        0        0     1705 2023-04-21 16:02:25.605810 finalynx-1.8.0/finalynx/usage.py
+-rw-r--r--   0        0        0     1713 2023-04-21 16:02:26.777826 finalynx-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7539 1970-01-01 00:00:00.000000 finalynx-1.8.0/PKG-INFO
```

### Comparing `finalynx-1.7.0/LICENSE` & `finalynx-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/README.md` & `finalynx-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/__init__.py` & `finalynx-1.8.0/finalynx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Add finary_api submodule to path to allow imports to work
 sys.path.append(os.path.join(os.path.dirname(__file__), "finary_api"))
 
 # Portfolio
 from .portfolio import TargetRange, TargetMin, TargetMax, TargetRatio, TargetGlobalRatio
 from .portfolio import Line, Folder, Bucket, SharedFolder, Portfolio, FolderDisplay
 from .portfolio import AssetClass, EnvelopeClass
-from .portfolio import Envelope, EnvelopeState, PEA, AV, PER
+from .portfolio import Envelope, EnvelopeState, PEA, PEE, AV, PER
 
 # Fetch
 from .fetch import FetchFinary
 
 # Advisor
 from .copilot import Copilot
```

### Comparing `finalynx-1.7.0/finalynx/__main__.py` & `finalynx-1.8.0/finalynx/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/__meta__.py` & `finalynx-1.8.0/finalynx/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ```{warning}
 Do not manually change this information.
 ```
 
 Metadata information about Finalynx. This file is used by Fynalinx and updated by the CI/CD pipeline.
 """
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 __author__ = "Pierre Laclau (MadeInPierre)"
 
 __copyright__ = """
 Copyright (c) 2023, MadeInPierre
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
```

### Comparing `finalynx-1.7.0/finalynx/analyzer/__init__.py` & `finalynx-1.8.0/finalynx/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/analyzer/analyzer.py` & `finalynx-1.8.0/finalynx/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/analyzer/asset_class.py` & `finalynx-1.8.0/finalynx/analyzer/asset_class.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/analyzer/envelopes.py` & `finalynx-1.8.0/finalynx/analyzer/envelopes.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/analyzer/investment_state.py` & `finalynx-1.8.0/finalynx/analyzer/investment_state.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/assistant.py` & `finalynx-1.8.0/finalynx/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from finalynx import Simulator
 from rich import inspect  # noqa F401
 from rich import pretty
 from rich import print  # noqa F401
 from rich import traceback
 from rich.columns import Columns
 from rich.panel import Panel
+from rich.text import Text
 
 from .__meta__ import __version__
 from .console import console
 from .usage import __doc__
 
 # Enable rich's features
 
@@ -109,33 +110,34 @@
 
         # Simulate the portolio's evolution through the years by auto-investing each month
         simulation = self.scenario.rich_simulation(self.portfolio)  # noqa TODO
 
         # Get recommendations for immediate investment operations
         recommentations = self.copilot.rich_recommendations(self.portfolio)  # noqa TODO
 
-        # Final set of results to be displayed
-        panels = [
-            Panel(
-                self.portfolio.tree(
-                    output_format=self.output_format,
-                    hide_root=self.hide_root,
-                    hide_amounts=self.hide_amounts,
-                ),
-                title=self.portfolio.name,
-                padding=(1, 4),
+        # Items to be rendered as a row
+        render = [
+            self.portfolio.tree(
+                output_format=self.output_format,
+                hide_root=self.hide_root,
+                hide_amounts=self.hide_amounts,
             ),
-            # Panel(simulation, title='Simulation'),   # TODO Coming soon
-            # Panel(recommendations, title='Advisor'), # TODO Coming soon
         ]
 
+        # Display deltas only if not already printed in the main tree
+        if "delta" not in self.output_format:
+            render.append(self.portfolio.tree_delta())
+
+        # Final set of results to be displayed
+        panels = [Columns([Text("  ")] + render)]  # type: ignore
+
         # Show the data fetched from Finary if specified
         if self.show_data:
-            panels.append(Panel(finary_tree, title="Finary data"))
+            panels.append(Panel(finary_tree, title="Finary data"))  # type: ignore
 
         # Display the entire portfolio and associated recommendations
-        console.print("\n", Columns(panels, padding=(2, 10)))
+        console.print("\n", Columns(panels, padding=(2, 10)), "\n")
 
         # Host a local webserver with the running dashboard
         if self.launch_dashboard:
             console.log("Launching dashboard.")
             Dashboard().run(portfolio=self.portfolio)
```

### Comparing `finalynx-1.7.0/finalynx/copilot/copilot.py` & `finalynx-1.8.0/finalynx/copilot/copilot.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/dashboard/dashboard.py` & `finalynx-1.8.0/finalynx/dashboard/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,89 +96,100 @@
                     ui.toggle({1: "Finalynx", 2: "Finary"}, value=1, on_change=_on_select_color_map)
 
         # with ui.right_drawer(fixed=False).style('background-color: #ebf1fa').props('bordered') as right_drawer:
         #     ui.label('RIGHT DRAWER')
         # with ui.footer(value=True).style('background-color: #3874c8'):
         #     ui.label('FOOTER')
 
-        with ui.tabs() as tabs:
-            ui.tab("Portfolio", icon="home")
-            ui.tab("Analysis", icon="info")
-
-        with ui.tab_panels(tabs, value="Portfolio"):
-            with ui.tab_panel("Portfolio"):
-                self.portfolio_dict = self._convert_rich_tree_to_nicegui(portfolio)
-                max_id = self._add_ids_to_tree(self.portfolio_dict)
-
-                # with ui.card_section().style("padding: 20px 40px"):
-                #     ui.markdown(f"#### {self.portfolio_dict['label']}").classes("text-center").style(
-                #         "padding: 0 0 10px 0"
-                #     )
-                #     tree = ui.tree(
-                #         self.portfolio_dict["children"],
-                #         on_expand=self._on_tree_expand,
-                #         on_select=self._on_tree_select,
-                #         on_tick=self._on_tree_tick,
-                #     ).props("selected-color=secondary")
-                #     tree._props["expanded"] = list(range(max_id))
-
-                ui.markdown(f"#### {portfolio.render('[dashboard_tree]')}").classes("text-center")
-
-                with ui.tree(
-                    self.portfolio_dict["children"],
-                    on_select=self._on_tree_select,
-                ) as tree:
-                    tree._props["expanded"] = list(range(max_id))
-                    tree.props("dense")
-
-                    tree.add_slot(
-                        "default-header",
-                        """
-                            <q-icon v-if="props.node.icon !== 'menu'" v-bind="{ name: props.node.icon, color: props.node.color }" size="20px"/>
-                            <span :props="props">
-                                <strong>
-                                    <span :style="{ color: props.node.color }">&nbsp;{{ props.node.amount }} €</span>
-                                </strong>
-                                <strong v-if="props.node.is_folder">
-                                    <span style="color: #455A64">&nbsp;{{ props.node.name }}</span>
-                                </strong>
-                                <span v-else style="color: black">&nbsp;{{ props.node.name }}</span>
-                                <span style="color: grey">&nbsp;{{ props.node.hint }}</span>
-                            </span>
+        # with ui.tabs() as tabs:
+        #     ui.tab("Portfolio", icon="home")
+        #     ui.tab("Analysis", icon="info")
+
+        # with ui.tab_panels(tabs, value="Portfolio"):
+        #     with ui.tab_panel("Portfolio"):
+        #         pass
+        #     with ui.tab_panel("Analysis"):
+        #         pass
+
+        with ui.column():
+            self.hey = ui.markdown(f"#### {self.selected_node.name}").classes("text-center")
+
+            with ui.splitter(value=50).classes("w-full") as splitter:
+                with splitter.before:
+                    self.portfolio_dict = self._convert_rich_tree_to_nicegui(portfolio)
+                    max_id = self._add_ids_to_tree(self.portfolio_dict)
+
+                    # with ui.card_section().style("padding: 20px 40px"):
+                    #     ui.markdown(f"#### {self.portfolio_dict['label']}").classes("text-center").style(
+                    #         "padding: 0 0 10px 0"
+                    #     )
+                    #     tree = ui.tree(
+                    #         self.portfolio_dict["children"],
+                    #         on_expand=self._on_tree_expand,
+                    #         on_select=self._on_tree_select,
+                    #         on_tick=self._on_tree_tick,
+                    #     ).props("selected-color=secondary")
+                    #     tree._props["expanded"] = list(range(max_id))
+
+                    # ui.markdown(f"#### {portfolio.render('[dashboard_tree]')}").classes("text-center")
+
+                    with ui.tree(
+                        self.portfolio_dict["children"],
+                        on_select=self._on_tree_select,
+                    ) as tree:
+                        tree._props["expanded"] = list(range(max_id))
+                        tree.props("dense")
+
+                        tree.add_slot(
+                            "default-header",
+                            """
+                                <q-icon v-if="props.node.icon !== 'menu'" v-bind="{ name: props.node.icon, color: props.node.color }" size="20px"/>
+                                <span :props="props">
+                                    <strong>
+                                        <span :style="{ color: props.node.color }">&nbsp;{{ props.node.amount }} €</span>
+                                    </strong>
+                                    <strong v-if="props.node.is_folder">
+                                        <span style="color: #455A64">&nbsp;{{ props.node.name }}</span>
+                                    </strong>
+                                    <span v-else style="color: black">&nbsp;{{ props.node.name }}</span>
+                                    <span style="color: grey">&nbsp;{{ props.node.hint }}</span>
+                                </span>
+                            """,
+                        )
+
+                        tree.add_slot(
+                            "default-body",
+                            """
+                            <span v-if="props.node.newline == true" :props="props">&nbsp;</span>
                         """,
-                    )
+                        )
 
-                    tree.add_slot(
-                        "default-body",
-                        """
-                        <span v-if="props.node.newline == true" :props="props">&nbsp;</span>
-                    """,
-                    )
-
-                # dashboard_console = Console(record=True)
-                # dashboard_console.print(portfolio.tree(output_format="[dashboard_console]", hide_root=True))
-                # ui.html(dashboard_console.export_html())
-
-            with ui.tab_panel("Analysis"):
-                self.hey = ui.markdown(f"#### {self.selected_node.name}")
-                with ui.column():
-                    self.chart_simulator = ui.chart(Simulator().chart(portfolio))
-                    self.chart_asset_classes = ui.chart(AnalyzeAssetClasses(self.selected_node).chart(self.color_map))
-                    self.chart_envelope_states = ui.chart(
-                        AnalyzeInvestmentStates(self.selected_node).chart(date.today())
-                    )
-                    self.chart_envelopes = ui.chart(AnalyzeEnvelopes(self.selected_node).chart())
-
-        # with ui.splitter(value=40).classes("w-full") as splitter:
-        #     with splitter.before:
-        #         ui.label("This is the first tab")
-        #     with splitter.after:
-        #         ui.label("This is the second tab")
-
-        ui.run(title="Finalynx Dashboard", favicon=self._url_logo, reload=True, show=True, host="0.0.0.0")
+                    # dashboard_console = Console(record=True)
+                    # dashboard_console.print(portfolio.tree(output_format="[dashboard_console]", hide_root=True))
+                    # ui.html(dashboard_console.export_html())
+
+                with splitter.after:
+                    with ui.column():
+                        self.chart_simulator = ui.chart(Simulator().chart(portfolio))
+                        self.chart_asset_classes = ui.chart(
+                            AnalyzeAssetClasses(self.selected_node).chart(self.color_map)
+                        )
+                        self.chart_envelope_states = ui.chart(
+                            AnalyzeInvestmentStates(self.selected_node).chart(date.today())
+                        )
+                        self.chart_envelopes = ui.chart(AnalyzeEnvelopes(self.selected_node).chart())
+
+        ui.run(
+            title="Finalynx Dashboard",
+            favicon=self._url_logo,
+            reload=False,
+            show=False,
+            host="0.0.0.0",
+            native=False,
+        )
 
     def _on_tree_expand(self, event: Any) -> None:
         console.log(event)
 
     def _on_tree_select(self, event: Any) -> None:
         node_id = event.value if event.value else 1
         node = self._get_node_from_id(node_id, self.portfolio_dict)
```

### Comparing `finalynx-1.7.0/finalynx/fetch/__init__.py` & `finalynx-1.8.0/finalynx/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/fetch/fetch.py` & `finalynx-1.8.0/finalynx/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/fetch/fetch_finary.py` & `finalynx-1.8.0/finalynx/fetch/fetch_finary.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/.gitignore` & `finalynx-1.8.0/finalynx/finary_api/.gitignore`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/LICENSE` & `finalynx-1.8.0/finalynx/finary_api/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/README.md` & `finalynx-1.8.0/finalynx/finary_api/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/__init__.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/__main__.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/bank_account_types.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/currencies.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/currencies.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/cryptocom.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/securities.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/signin.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/signin.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_cryptos.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_generic_assets.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_holdings_accounts.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_portfolio.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_precious_metals.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/user_securities.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/user_securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/finary_api/finary_api/views.py` & `finalynx-1.8.0/finalynx/finary_api/finary_api/views.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/parse/json.py` & `finalynx-1.8.0/finalynx/parse/json.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/parse/parser.py` & `finalynx-1.8.0/finalynx/parse/parser.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/__init__.py` & `finalynx-1.8.0/finalynx/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/bucket.py` & `finalynx-1.8.0/finalynx/portfolio/bucket.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/constants.py` & `finalynx-1.8.0/finalynx/portfolio/constants.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/envelope.py` & `finalynx-1.8.0/finalynx/portfolio/envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,21 @@
 
 class PEA(Envelope):
     def __init__(self, name: str, code: str, date_created: date):
         date_unlock = date_created + relativedelta(years=5)
         super().__init__(name, code, date_created, date_unlock, date_unlock)
 
 
+class PEE(Envelope):
+    def __init__(self, name: str, code: str, date_created: date, date_unlock: Optional[date] = None):
+        if not date_unlock:
+            date_unlock = date_created + relativedelta(years=5)
+        super().__init__(name, code, date_created, date_unlock, date_unlock)
+
+
 class AV(Envelope):
     def __init__(self, name: str, code: str, date_created: date):
         date_untax = date_created + relativedelta(years=8)
         super().__init__(name, code, date_created, date_created, date_untax)
 
 
 class PER(Envelope):
```

### Comparing `finalynx-1.7.0/finalynx/portfolio/folder.py` & `finalynx-1.8.0/finalynx/portfolio/folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,28 @@
         render = self.render(output_format, **render_args)
         node = _tree.add(render) if _tree else Tree(render, guide_style="grey42", hide_root=hide_root)
         if self.display == FolderDisplay.EXPANDED:
             for child in self.children:
                 child.tree(output_format=output_format, _tree=node, **render_args)
         return node
 
+    def tree_delta(self, _tree: Optional[Tree] = None) -> Tree:
+        """Generates a tree with delta amounts to be invested to reach the ideal portfolio allocation."""
+        render = self._render_delta() + ("\n" if self.newline else "")
+
+        if not _tree:
+            _tree = Tree(render, hide_root=True)
+        else:
+            _tree.add(render)
+
+        if self.display == FolderDisplay.EXPANDED:
+            for child in self.children:
+                child.tree_delta(_tree=_tree)
+        return _tree
+
     def process(self) -> None:
         """Some `Node` or `Target` objects might need to process some data once the investment
         values have been fetched from Finary. Folders do not have any processing procedure.
         Here, we only call the `process()` method of all children.
         """
         total_ratio = 0.0
```

### Comparing `finalynx-1.7.0/finalynx/portfolio/line.py` & `finalynx-1.8.0/finalynx/portfolio/line.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/node.py` & `finalynx-1.8.0/finalynx/portfolio/node.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,41 +47,52 @@
         if target is not None:
             target.set_parent(self)
 
         # Setup custom aliases for node rendering
         render_aliases: Dict[str, str] = {
             "[text]": "[target_text][prehint] [name] [hint][newline]",
             "[console]": "[target][dim white][prehint][/] [account_code][name_color][name][/] [dim white][hint][/][newline]",
+            "[console_delta]": "[delta][account_code][name_color][name][/] [newline]",
             "[console_targets]": "[bold green][goal][/][account_code][name_color][name][/][newline]",
             "[text_targets]": "[goal][name][newline]",
             "[dashboard_tree]": "[amount] [currency] [name]",
             "[dashboard_console]": "[bold][target][/][bright_black][prehint][/] [name_color][name][/] [bright_black][hint][/][newline]",
             "[target]": "[[target_color]][target_text][/]",
             "[target_text]": "[target_symbol] [amount] [currency]",
         }
         render_agents: Dict[str, Callable[..., str]] = {
             "name": self._render_name,
             "name_color": self._render_name_color,
             "newline": self._render_newline,
             "amount": self._render_amount,
             "goal": self._render_goal,
+            "ideal": self._render_ideal,
+            "delta": self._render_delta,
             "hint": self._render_hint,
             "prehint": self._render_prehint,
             "currency": self._render_currency,
             "target_symbol": self.target._render_target_symbol,
             "target_color": self.target._render_target_color,
         }
         render_aliases.update(aliases if aliases else {})
         render_agents.update(agents if agents else {})
         Render.__init__(self, render_aliases, render_agents)
 
     def get_amount(self) -> float:
         """Virtual method that must be implemented by all subclasses."""
         raise NotImplementedError("Must be implemented by children classes")
 
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested in this node based on surrounding targets."""
+        return self.target.get_ideal()
+
+    def get_delta(self) -> float:
+        """:returns: How much should be invested in this node to reach the ideal amount set by the target."""
+        return self.get_ideal() - self.get_amount()
+
     def tree(
         self,
         output_format: str = "[console]",
         _tree: Optional[Tree] = None,
         hide_root: bool = False,
         **render_args: Any,
     ) -> Tree:
@@ -95,14 +106,19 @@
         :param args: Provide any list of arguments supported by the `Tree` class if this is the root folder in the hierarchy.
         :returns: If the `_tree` argument is empty, the function returns a new `Tree` instance with this node's render.
         Otherwise, it adds this node's render as a child node and returns the `_tree`.
         """
         render = self.render(output_format, **render_args)
         return _tree.add(render) if _tree else Tree(render, hide_root=hide_root)
 
+    def tree_delta(self, _tree: Optional[Tree] = None) -> Tree:
+        """Generates a tree with delta amounts to be invested to reach the ideal portfolio allocation."""
+        render = self._render_delta() + ("\n" if self.newline else "")
+        return _tree.add(render) if _tree else Tree(render, hide_root=True)
+
     def process(self) -> None:
         """Some `Node` or `Target` objects might need to process some data once the investment
         values have been fetched from Finary. Here, this method is left as esmpty but can be
         overridden by subclasses.
         """
         return  # Optional method for subclasses to process after fetch
 
@@ -131,14 +147,26 @@
             else 0
         )
         return "···" if hide_amounts else f"{round(self.get_amount()):>{max_length}}"
 
     def _render_goal(self) -> str:
         return self.target.render_goal()
 
+    def _render_ideal(self) -> str:
+        return self.target.render_ideal()
+
+    def _render_delta(self) -> str:
+        delta, check = round(self.get_delta()), self.target.check()
+        if delta == 0 or check == Target.RESULT_NONE:
+            return ""
+        if check == Target.RESULT_OK:
+            return "[green]✓[/] "
+        color = "green" if delta > 0 else "red"
+        return f"[{color}]{'+' if delta > 0 else ''}{delta} €[/] "
+
     def _render_name(self) -> str:
         """:returns: A formatted rendering of the node name."""
         return self.name
 
     def _render_name_color(self) -> str:
         """:returns: A formatted rendering of the node name."""
         return "[black]"
```

### Comparing `finalynx-1.7.0/finalynx/portfolio/portfolio.py` & `finalynx-1.8.0/finalynx/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/finalynx/portfolio/render.py` & `finalynx-1.8.0/finalynx/portfolio/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     def render(self, output_format: str = "[console]", **args: Dict[str, Any]) -> str:
         """Render the instance as a string by following the output format. See
         [formatting guidelines](https://finalynx.readthedocs.io/en/latest/tutorials/customization.html)
         for more information.
         :returns: A string representation of the instance based on the output format.
         """
 
+        # TODO automatically add a space between components instead of hardcoding everywhere?
+
         # Utility method used below
         def safe_len(obj: Any) -> int:
             return len(obj) if obj else 0
 
         # Recursively replace alias keywords by their correspoding values
         output_format = self._apply_aliases(output_format)
```

### Comparing `finalynx-1.7.0/finalynx/portfolio/targets.py` & `finalynx-1.8.0/finalynx/portfolio/targets.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
     def get_amount(self) -> float:
         """:returns: The amount stored in the target's parent."""
         if self.parent is None:
             raise ValueError("[red]Target has no parent, not allowed.[/]")
         return self.parent.get_amount()
 
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested based on surrounding targets."""
+        return 0.0
+
     def check(self) -> Dict[str, str]:
         """Default behavior to check if the parent's amount respects the target objective.
         This method should be overriden by all subclasses to define custom-tailored logic.
         :returns: A `Target.RESULT_*` object depending on the recommendation to be rendered
         in the output console.
         """
         if self.get_amount() == 0:
@@ -57,19 +61,24 @@
         :returns: A string with a righ-formatted render of the parent's amount based on the target recommendation.
         """
         result = self.check()
         result = result if result != True else Target.RESULT_START  # type: ignore # noqa: E712 TODO weird bug??? Workaround for now
         number = f"{round(self.get_amount()):>{n_characters}}" if not hide_amount else "···"
         return f'[{result["color"]}]{result["symbol"]} {number} €[/][dim white]{self.prehint()}[/]'
 
-    def render_goal(self) -> str:
+    def render_ideal(self) -> str:
         """Ideal amount to be reached based on the current target and node
         position in the tree. Must be overridden by subclasses."""
         return ""
 
+    def render_goal(self) -> str:
+        """Ideal amount or ratio to be reached based on the current target and node
+        position in the tree. Must be overridden by subclasses."""
+        return ""
+
     def _render_target_name(self) -> str:
         """:returns: The name of the target recommentation."""
         return self.check()["name"]
 
     def _render_target_symbol(self) -> str:
         """:returns: The UFT-8 symbol associated to the target recommentation."""
         return self.check()["symbol"]
@@ -105,18 +114,29 @@
             return Target.RESULT_TOLERATED
         elif self._get_variable() <= self.target_max:
             return Target.RESULT_OK
         elif self._get_variable() <= self.target_max + self.tolerance:
             return Target.RESULT_TOLERATED
         return Target.RESULT_DEVEST
 
-    def render_goal(self) -> str:
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested based on surrounding targets."""
+        if self.target_min <= self.get_amount() <= self.target_max:
+            return self.get_amount()
+        elif self.get_amount() < self.target_min:
+            return self.target_min
+        return self.target_max
+
+    def render_ideal(self) -> str:
         """:returns: The average between target boundaries."""
-        goal_amount = round((self.target_min + self.target_max) / 2)
-        return f"{goal_amount} € "
+        return f"{round(self.get_ideal())} € "
+
+    def render_goal(self) -> str:
+        """:returns: Same as ideal amount."""
+        return f"{round(self.get_ideal())} € "
 
     def _get_variable(self) -> float:
         """Internal method that gives the value to be checked (overriden by subclasses)."""
         return self.get_amount()
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
@@ -129,17 +149,17 @@
     def __init__(self, target_max: float, tolerance: float = 0):
         """This target checks if the amount is below a specified threshold (with an optional tolerance).
         :param target_max: Maximum threshold to get a `RESULT_OK`.
         :param tolerance: If the amount is at most `target_max + tolerance`, the check will return a `RESULT_TOLERATED`.
         """
         super().__init__(0, target_max, tolerance)
 
-    def render_goal(self) -> str:
-        """:returns: The maximum target value."""
-        return f"{self.target_max} € "
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested based on surrounding targets."""
+        return self.target_max
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
         return f"- Maximum {self.target_max} €"
 
 
 class TargetMin(TargetRange):
@@ -148,17 +168,17 @@
     def __init__(self, target_min: float, tolerance: float = 0):
         """This target checks if the amount is above a specified threshold (with an optional tolerance).
         :param target_min: Minimum threshold to get a `RESULT_OK`.
         :param tolerance: If the amount is at least `target_min - tolerance`, the check will return a `RESULT_TOLERATED`.
         """
         super().__init__(target_min, np.inf, tolerance)
 
-    def render_goal(self) -> str:
-        """:returns: The minimum target value."""
-        return f"{self.target_min} € "
+    def get_ideal(self) -> float:
+        """:returns: The ideal amount to be invested based on surrounding targets."""
+        return self.target_min
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
         return f"- Minimum {self.target_min} €"
 
 
 class TargetRatio(TargetRange):
```

### Comparing `finalynx-1.7.0/finalynx/simulator/simulator.py` & `finalynx-1.8.0/finalynx/simulator/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         """Dummy output for now, will return a full simulation graph in the future."""
         return "Simulation"
 
     def chart(self, portfolio: Portfolio) -> Dict[str, Any]:
         analyzer = AnalyzeInvestmentStates(portfolio)
         data: Dict[str, List[float]] = {c.value: [] for c in EnvelopeState}
 
-        for year in range(2000, 2100):
+        date_start, date_end = 2022, 2085  # TODO set as parameter in dashboard/options
+
+        for year in range(date_start, date_end):
             result = analyzer.analyze(date(year, 1, 1))
             for key, value in result.items():
                 data[key].append(value)
 
         colors = {
             "Unknown": "#434348",
             "Closed": "#999999",
@@ -47,19 +49,19 @@
             "Free": "#7BB151",
         }
 
         return {
             "chart": {"plotBackgroundColor": None, "plotBorderWidth": None, "plotShadow": False, "type": "area"},
             "title": {"text": "Simulation", "align": "center"},
             "plotOptions": {
-                "series": {"pointStart": 2000},
+                "series": {"pointStart": date_start},
                 "area": {
                     "stacking": "normal",
                     "lineColor": "#666666",
                     "lineWidth": 1,
-                    "marker": {"lineWidth": 1, "lineColor": "#666666"},
+                    "marker": {"lineWidth": 1, "lineColor": "#666666", "enabled": False},
                 },
             },
             "series": [{"name": key, "data": value, "color": colors[key]} for key, value in data.items()],
             "credits": {"enabled": False},
             # "xAxis": {"plotLines": [{"color": "#000000", "width": 2, "value": 2023}]},
         }
```

### Comparing `finalynx-1.7.0/finalynx/usage.py` & `finalynx-1.8.0/finalynx/usage.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.7.0/pyproject.toml` & `finalynx-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finalynx"
-version = "1.7.0"
+version = "1.8.0"
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
-version = "1.7.0"
+version = "1.8.0"
 tag_format = "v$version"
 
 [tool.mypy]
 exclude = [
     "finary_api/*",
     "docs/*",
     "tests/*.py"
```

### Comparing `finalynx-1.7.0/PKG-INFO` & `finalynx-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalynx
-Version: 1.7.0
+Version: 1.8.0
 Summary: A command line investment assistant to organize your portfolio and simulate its future to reach your life goals.
 License: GPLv3
 Author: MadeInPierre
 Author-email: pielaclau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalynx Version: 1.7.0 Summary: A command line
+Metadata-Version: 2.1 Name: finalynx Version: 1.8.0 Summary: A command line
 investment assistant to organize your portfolio and simulate its future to
 reach your life goals. License: GPLv3 Author: MadeInPierre Author-email:
 pielaclau@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2)
```

