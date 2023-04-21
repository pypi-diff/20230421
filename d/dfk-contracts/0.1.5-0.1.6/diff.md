# Comparing `tmp/dfk_contracts-0.1.5.tar.gz` & `tmp/dfk_contracts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfk_contracts-0.1.5.tar", max compression
+gzip compressed data, was "dfk_contracts-0.1.6.tar", max compression
```

## Comparing `dfk_contracts-0.1.5.tar` & `dfk_contracts-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0   509023 2023-02-24 21:13:22.305257 dfk_contracts-0.1.5/dfk_contracts/DFK_ABIS.json
--rw-r--r--   0        0        0     6165 2023-02-24 21:13:22.167936 dfk_contracts-0.1.5/dfk_contracts/abi_contract_wrapper.py
--rw-r--r--   0        0        0     1285 2023-02-24 21:13:22.168696 dfk_contracts-0.1.5/dfk_contracts/abi_multi_contract_wrapper.py
--rw-r--r--   0        0        0     5224 2023-02-24 21:13:22.304926 dfk_contracts-0.1.5/dfk_contracts/all_dfk_contracts.py
--rw-r--r--   0        0        0     6443 2023-02-24 21:13:22.175233 dfk_contracts-0.1.5/dfk_contracts/contracts/airdrop_claim.py
--rw-r--r--   0        0        0     7938 2023-02-24 21:13:22.178331 dfk_contracts-0.1.5/dfk_contracts/contracts/alchemist.py
--rw-r--r--   0        0        0    11346 2023-02-24 21:13:22.183735 dfk_contracts-0.1.5/dfk_contracts/contracts/assisting_auction.py
--rw-r--r--   0        0        0    28633 2023-02-24 21:13:22.196371 dfk_contracts-0.1.5/dfk_contracts/contracts/atonement_crystal.py
--rw-r--r--   0        0        0     5368 2023-02-24 21:13:22.198536 dfk_contracts-0.1.5/dfk_contracts/contracts/banker.py
--rw-r--r--   0        0        0     9787 2023-02-24 21:13:22.201541 dfk_contracts-0.1.5/dfk_contracts/contracts/birthday_cake.py
--rw-r--r--   0        0        0     8977 2023-02-24 21:13:22.204595 dfk_contracts-0.1.5/dfk_contracts/contracts/charity_fund.py
--rw-r--r--   0        0        0    13451 2023-02-24 21:13:22.208716 dfk_contracts-0.1.5/dfk_contracts/contracts/crystal_core.py
--rw-r--r--   0        0        0    25794 2023-02-24 21:13:22.220662 dfk_contracts-0.1.5/dfk_contracts/contracts/dark_summoning.py
--rw-r--r--   0        0        0    55830 2023-02-24 21:13:22.228939 dfk_contracts-0.1.5/dfk_contracts/contracts/dfk_duel_s2.py
--rw-r--r--   0        0        0    14296 2023-02-24 21:13:22.231587 dfk_contracts-0.1.5/dfk_contracts/contracts/duel_rank_claim.py
--rw-r--r--   0        0        0     8728 2023-02-24 21:13:22.233302 dfk_contracts-0.1.5/dfk_contracts/contracts/erc20.py
--rw-r--r--   0        0        0     7483 2023-02-24 21:13:22.234552 dfk_contracts-0.1.5/dfk_contracts/contracts/gen0_airdrop.py
--rw-r--r--   0        0        0    25083 2023-02-24 21:13:22.236693 dfk_contracts-0.1.5/dfk_contracts/contracts/gen0_reroll.py
--rw-r--r--   0        0        0    16211 2023-02-24 21:13:22.239464 dfk_contracts-0.1.5/dfk_contracts/contracts/hero_auction.py
--rw-r--r--   0        0        0    10449 2023-02-24 21:13:22.241594 dfk_contracts-0.1.5/dfk_contracts/contracts/hero_bridge.py
--rw-r--r--   0        0        0    30987 2023-02-24 21:13:22.244572 dfk_contracts-0.1.5/dfk_contracts/contracts/hero_core.py
--rw-r--r--   0        0        0    28714 2023-02-24 21:13:22.248582 dfk_contracts-0.1.5/dfk_contracts/contracts/hero_summoning.py
--rw-r--r--   0        0        0    12535 2023-02-24 21:13:22.249412 dfk_contracts-0.1.5/dfk_contracts/contracts/item_consumer.py
--rw-r--r--   0        0        0     6871 2023-02-24 21:13:22.250582 dfk_contracts-0.1.5/dfk_contracts/contracts/item_gold_trader_v2.py
--rw-r--r--   0        0        0    26862 2023-02-24 21:13:22.254712 dfk_contracts-0.1.5/dfk_contracts/contracts/jewel_token.py
--rw-r--r--   0        0        0    15192 2023-02-24 21:13:22.256918 dfk_contracts-0.1.5/dfk_contracts/contracts/land_auction.py
--rw-r--r--   0        0        0    18105 2023-02-24 21:13:22.259522 dfk_contracts-0.1.5/dfk_contracts/contracts/land_core.py
--rw-r--r--   0        0        0    30381 2023-02-24 21:13:22.264360 dfk_contracts-0.1.5/dfk_contracts/contracts/master_gardener.py
--rw-r--r--   0        0        0    25321 2023-02-24 21:13:22.267569 dfk_contracts-0.1.5/dfk_contracts/contracts/meditation_circle.py
--rw-r--r--   0        0        0     7278 2023-02-24 21:13:22.268743 dfk_contracts-0.1.5/dfk_contracts/contracts/pasture.py
--rw-r--r--   0        0        0    15191 2023-02-24 21:13:22.272888 dfk_contracts-0.1.5/dfk_contracts/contracts/pet_auction.py
--rw-r--r--   0        0        0    20801 2023-02-24 21:13:22.275312 dfk_contracts-0.1.5/dfk_contracts/contracts/pet_core.py
--rw-r--r--   0        0        0     9676 2023-02-24 21:13:22.276954 dfk_contracts-0.1.5/dfk_contracts/contracts/pet_exchange.py
--rw-r--r--   0        0        0    19016 2023-02-24 21:13:22.279512 dfk_contracts-0.1.5/dfk_contracts/contracts/pet_hatching.py
--rw-r--r--   0        0        0    20106 2023-02-24 21:13:22.215040 dfk_contracts-0.1.5/dfk_contracts/contracts/power_token.py
--rw-r--r--   0        0        0    33463 2023-02-24 21:13:22.283436 dfk_contracts-0.1.5/dfk_contracts/contracts/power_up_manager.py
--rw-r--r--   0        0        0    14471 2023-02-24 21:13:22.285695 dfk_contracts-0.1.5/dfk_contracts/contracts/profiles.py
--rw-r--r--   0        0        0    20908 2023-02-24 21:13:22.288118 dfk_contracts-0.1.5/dfk_contracts/contracts/quest_core.py
--rw-r--r--   0        0        0    23204 2023-02-24 21:13:22.291697 dfk_contracts-0.1.5/dfk_contracts/contracts/raffle_master.py
--rw-r--r--   0        0        0     9787 2023-02-24 21:13:22.293355 dfk_contracts-0.1.5/dfk_contracts/contracts/raffle_ticket.py
--rw-r--r--   0        0        0     9147 2023-02-24 21:13:22.294801 dfk_contracts-0.1.5/dfk_contracts/contracts/stone_carver.py
--rw-r--r--   0        0        0     6206 2023-02-24 21:13:22.295858 dfk_contracts-0.1.5/dfk_contracts/contracts/stylist.py
--rw-r--r--   0        0        0     7897 2023-02-24 21:13:22.297056 dfk_contracts-0.1.5/dfk_contracts/contracts/token_disburse.py
--rw-r--r--   0        0        0     4541 2023-02-24 21:13:22.297929 dfk_contracts-0.1.5/dfk_contracts/contracts/uniswap_v2_factory.py
--rw-r--r--   0        0        0    21550 2023-02-24 21:13:22.301811 dfk_contracts-0.1.5/dfk_contracts/contracts/uniswap_v2_router.py
--rw-r--r--   0        0        0    18537 2023-02-24 21:13:22.304386 dfk_contracts-0.1.5/dfk_contracts/contracts/validator_fund.py
--rw-r--r--   0        0        0     1140 2023-02-24 21:13:22.166848 dfk_contracts-0.1.5/dfk_contracts/credentials.py
--rw-r--r--   0        0        0      779 2023-02-24 21:13:22.166233 dfk_contracts-0.1.5/dfk_contracts/solidity_types.py
--rw-r--r--   0        0        0      365 2023-02-27 16:16:41.451346 dfk_contracts-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 dfk_contracts-0.1.5/setup.py
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 dfk_contracts-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0   584106 2023-04-20 16:46:33.470587 dfk_contracts-0.1.6/dfk_contracts/DFK_ABIS.json
+-rw-r--r--   0        0        0     6165 2023-04-20 16:46:33.331337 dfk_contracts-0.1.6/dfk_contracts/abi_contract_wrapper.py
+-rw-r--r--   0        0        0     1285 2023-04-20 16:46:33.332783 dfk_contracts-0.1.6/dfk_contracts/abi_multi_contract_wrapper.py
+-rw-r--r--   0        0        0     5782 2023-04-20 16:46:33.470192 dfk_contracts-0.1.6/dfk_contracts/all_dfk_contracts.py
+-rw-r--r--   0        0        0     6443 2023-04-20 16:46:33.340389 dfk_contracts-0.1.6/dfk_contracts/contracts/airdrop_claim.py
+-rw-r--r--   0        0        0     7938 2023-04-20 16:46:33.344692 dfk_contracts-0.1.6/dfk_contracts/contracts/alchemist.py
+-rw-r--r--   0        0        0    11346 2023-04-20 16:46:33.348522 dfk_contracts-0.1.6/dfk_contracts/contracts/assisting_auction.py
+-rw-r--r--   0        0        0    28633 2023-04-20 16:46:33.352611 dfk_contracts-0.1.6/dfk_contracts/contracts/atonement_crystal.py
+-rw-r--r--   0        0        0     5368 2023-04-20 16:46:33.354351 dfk_contracts-0.1.6/dfk_contracts/contracts/banker.py
+-rw-r--r--   0        0        0     9787 2023-04-20 16:46:33.356980 dfk_contracts-0.1.6/dfk_contracts/contracts/birthday_cake.py
+-rw-r--r--   0        0        0     8977 2023-04-20 16:46:33.359385 dfk_contracts-0.1.6/dfk_contracts/contracts/charity_fund.py
+-rw-r--r--   0        0        0    13451 2023-04-20 16:46:33.362195 dfk_contracts-0.1.6/dfk_contracts/contracts/crystal_core.py
+-rw-r--r--   0        0        0    25794 2023-04-20 16:46:33.370883 dfk_contracts-0.1.6/dfk_contracts/contracts/dark_summoning.py
+-rw-r--r--   0        0        0    55830 2023-04-20 16:46:33.378548 dfk_contracts-0.1.6/dfk_contracts/contracts/dfk_duel_s2.py
+-rw-r--r--   0        0        0    14296 2023-04-20 16:46:33.380876 dfk_contracts-0.1.6/dfk_contracts/contracts/duel_rank_claim.py
+-rw-r--r--   0        0        0     8728 2023-04-20 16:46:33.382521 dfk_contracts-0.1.6/dfk_contracts/contracts/erc20.py
+-rw-r--r--   0        0        0     5901 2023-04-20 16:46:33.383672 dfk_contracts-0.1.6/dfk_contracts/contracts/flag_storage_v2.py
+-rw-r--r--   0        0        0     7483 2023-04-20 16:46:33.384912 dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_airdrop.py
+-rw-r--r--   0        0        0    25083 2023-04-20 16:46:33.386922 dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_reroll.py
+-rw-r--r--   0        0        0    40923 2023-04-20 16:46:33.388869 dfk_contracts-0.1.6/dfk_contracts/contracts/gene_reroll.py
+-rw-r--r--   0        0        0    16211 2023-04-20 16:46:33.391435 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_auction.py
+-rw-r--r--   0        0        0    10449 2023-04-20 16:46:33.393291 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_bridge.py
+-rw-r--r--   0        0        0    30987 2023-04-20 16:46:33.401862 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_core.py
+-rw-r--r--   0        0        0    28714 2023-04-20 16:46:33.405713 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_summoning.py
+-rw-r--r--   0        0        0    24467 2023-04-20 16:46:33.409796 dfk_contracts-0.1.6/dfk_contracts/contracts/item_bridge.py
+-rw-r--r--   0        0        0    12535 2023-04-20 16:46:33.410594 dfk_contracts-0.1.6/dfk_contracts/contracts/item_consumer.py
+-rw-r--r--   0        0        0    11557 2023-04-20 16:46:33.412092 dfk_contracts-0.1.6/dfk_contracts/contracts/item_gold_trader_v2.py
+-rw-r--r--   0        0        0    26862 2023-04-20 16:46:33.416170 dfk_contracts-0.1.6/dfk_contracts/contracts/jewel_token.py
+-rw-r--r--   0        0        0    15192 2023-04-20 16:46:33.418435 dfk_contracts-0.1.6/dfk_contracts/contracts/land_auction.py
+-rw-r--r--   0        0        0    18105 2023-04-20 16:46:33.420950 dfk_contracts-0.1.6/dfk_contracts/contracts/land_core.py
+-rw-r--r--   0        0        0    30381 2023-04-20 16:46:33.425186 dfk_contracts-0.1.6/dfk_contracts/contracts/master_gardener.py
+-rw-r--r--   0        0        0    25321 2023-04-20 16:46:33.427296 dfk_contracts-0.1.6/dfk_contracts/contracts/meditation_circle.py
+-rw-r--r--   0        0        0     9664 2023-04-20 16:46:33.428542 dfk_contracts-0.1.6/dfk_contracts/contracts/multicall3.py
+-rw-r--r--   0        0        0     7278 2023-04-20 16:46:33.429480 dfk_contracts-0.1.6/dfk_contracts/contracts/pasture.py
+-rw-r--r--   0        0        0    15191 2023-04-20 16:46:33.431774 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_auction.py
+-rw-r--r--   0        0        0     9508 2023-04-20 16:46:33.433482 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_bridge.py
+-rw-r--r--   0        0        0    20801 2023-04-20 16:46:33.440079 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_core.py
+-rw-r--r--   0        0        0     9676 2023-04-20 16:46:33.441798 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_exchange.py
+-rw-r--r--   0        0        0    19016 2023-04-20 16:46:33.444778 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_hatching.py
+-rw-r--r--   0        0        0    20106 2023-04-20 16:46:33.366801 dfk_contracts-0.1.6/dfk_contracts/contracts/power_token.py
+-rw-r--r--   0        0        0    33463 2023-04-20 16:46:33.448757 dfk_contracts-0.1.6/dfk_contracts/contracts/power_up_manager.py
+-rw-r--r--   0        0        0    14471 2023-04-20 16:46:33.450982 dfk_contracts-0.1.6/dfk_contracts/contracts/profiles.py
+-rw-r--r--   0        0        0    20908 2023-04-20 16:46:33.453862 dfk_contracts-0.1.6/dfk_contracts/contracts/quest_core.py
+-rw-r--r--   0        0        0    23204 2023-04-20 16:46:33.457090 dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_master.py
+-rw-r--r--   0        0        0     9787 2023-04-20 16:46:33.458656 dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_ticket.py
+-rw-r--r--   0        0        0     9147 2023-04-20 16:46:33.460218 dfk_contracts-0.1.6/dfk_contracts/contracts/stone_carver.py
+-rw-r--r--   0        0        0     6206 2023-04-20 16:46:33.461272 dfk_contracts-0.1.6/dfk_contracts/contracts/stylist.py
+-rw-r--r--   0        0        0     7897 2023-04-20 16:46:33.462407 dfk_contracts-0.1.6/dfk_contracts/contracts/token_disburse.py
+-rw-r--r--   0        0        0     4541 2023-04-20 16:46:33.463269 dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_factory.py
+-rw-r--r--   0        0        0    21550 2023-04-20 16:46:33.467047 dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_router.py
+-rw-r--r--   0        0        0    18537 2023-04-20 16:46:33.469549 dfk_contracts-0.1.6/dfk_contracts/contracts/validator_fund.py
+-rw-r--r--   0        0        0     2008 2023-04-20 16:46:33.329270 dfk_contracts-0.1.6/dfk_contracts/credentials.py
+-rw-r--r--   0        0        0      779 2023-04-20 16:46:33.326875 dfk_contracts-0.1.6/dfk_contracts/solidity_types.py
+-rw-r--r--   0        0        0      365 2023-04-21 15:18:44.353200 dfk_contracts-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 dfk_contracts-0.1.6/PKG-INFO
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/DFK_ABIS.json` & `dfk_contracts-0.1.6/dfk_contracts/DFK_ABIS.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821596771484155%*

 * *Differences: {"'CONTRACTS'": "{'ItemGoldTraderV2': {'ABI': {0: {'name': 'Initialized', 'inputs': {0: {'name': "*

 * *                "'version', 'type': 'uint8', 'internalType': 'uint8'}, delete: [1, 0]}}, 1: "*

 * *                "{'name': 'ItemAdded', 'inputs': {0: {'name': 'item'}, 2: {'name': "*

 * *                "'playerSellPrice', 'type': 'uint256', 'internalType': 'uint256'}, 3: {'name': "*

 * *                "'minPrice'}, 4: {'name': 'deltaPriceIncrease', 'type': 'uint256', 'internalType': "*

 * *                "'uint256'}, 5: {'na […]*

```diff
@@ -10462,14 +10462,295 @@
                 }
             ],
             "ADDRESS": {
                 "cv": null,
                 "sd": null
             }
         },
+        "FlagStorageV2": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint32",
+                                    "name": "levelCarryover",
+                                    "type": "uint32"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct DarkSummoning",
+                            "name": "values",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "DarkSummoningStorageSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "values",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "Gen0RerollSDStorageSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "owner_",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_access",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setModerator",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_access",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setUpdater",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getDarkSummoningStorage",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint32",
+                                    "name": "levelCarryover",
+                                    "type": "uint32"
+                                }
+                            ],
+                            "internalType": "struct DarkSummoning",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint32",
+                            "name": "_value",
+                            "type": "uint32"
+                        }
+                    ],
+                    "name": "setLevelCarryover",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getGen0RerollSDStorage",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "_reroll",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "setGen0RerollSDStorage",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x75d8ba2E4725633FcdcC165332dCA04c107915cA",
+                "sd": "0xeb9ff38209dCC4236DBFb3C275c0AAeEBf0B92Cf"
+            }
+        },
         "Gen0Airdrop": {
             "ABI": [
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_heroCoreAddress",
@@ -12462,14 +12743,3002 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0x74934378840D77E36AeF1f031D301549b4e1a225",
                 "sd": "0x0000000000000000000000000000000000000000"
             }
         },
+        "GeneReroll": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "afterHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bool",
+                            "name": "craftingGenesRerolled",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "CraftingGenesRerolled",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "HeroRerollStarted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "heroBefore",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "heroAfter",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "HeroRerolled",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "stat",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "increase",
+                            "type": "uint8"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "updateType",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "StatUp",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "afterHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8[]",
+                            "name": "geneIndex",
+                            "type": "uint8[]"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8[]",
+                            "name": "rankType",
+                            "type": "uint8[]"
+                        }
+                    ],
+                    "name": "TaintedGenesRerolled",
+                    "type": "event"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "cancelReroll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "endRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "heroToRerollData",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "seedblock",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "finishTime",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "rerollStarted",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "multiEndRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "multiStartRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "startRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x4b98f4C73fadA8E9C3f573502713FCebfA5a98AC",
+                "sd": "0xD0E292bAfBB1F691fEAFa7ddE1050EAEa923b2e3"
+            }
+        },
         "HeroAuction": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
                             "indexed": false,
@@ -17115,14 +20384,1102 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0xBc36D18662Bb97F9e74B1EAA1B752aA7A44595A7",
                 "sd": "0xb086584f476Ad21B40aF0672f385a67334A0b294"
             }
         },
+        "ItemBridge": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "receiver",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "item",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "ERC1155Received",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "bytes32",
+                            "name": "identifier",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "contractAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "ItemMapped",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "receiver",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "item",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "ItemReceived",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "MessageFailed",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Paused",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "SetTrustedRemote",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Unpaused",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "FUNCTION_TYPE_SEND",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "NO_EXTRA_GAS",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_lzEndpoint",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "__NonblockingLzAppUpgradeable_init",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "__NonblockingLzAppUpgradeable_init_unchained",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_useZro",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC1155",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC1155",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC20",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_useZro",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC20",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "failedMessages",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "forceResumeReceive",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_version",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_chainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_configType",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getConfig",
+                    "outputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "getGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "gasLimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "pure",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_lzEndpoint",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_itemMinter",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "initialize",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "isTrustedRemote",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "itemAddresses",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "itemIdentifiers",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "lzEndpoint",
+                    "outputs": [
+                        {
+                            "internalType": "contract ILayerZeroEndpointUpgradeable",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "lzReceive",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "string",
+                            "name": "_identifier",
+                            "type": "string"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_contractAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "mapItem",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "minDstGasLookup",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "nonblockingLzReceive",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "pause",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "paused",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "renounceOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "retryMessage",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_zroPaymentAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "sendERC1155",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "sendERC1155",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_zroPaymentAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "sendERC20",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "sendERC20",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_version",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_chainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_configType",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_config",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "setConfig",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_type",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_dstGasAmount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setMinDstGasLookup",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_version",
+                            "type": "uint16"
+                        }
+                    ],
+                    "name": "setReceiveVersion",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_version",
+                            "type": "uint16"
+                        }
+                    ],
+                    "name": "setSendVersion",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "setTrustedRemote",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "_useCustomAdapterParams",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setUseCustomAdapterParams",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
+                        }
+                    ],
+                    "name": "trustedRemoteLookup",
+                    "outputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "unpause",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "useCustomAdapterParams",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x501CdC4ef10b63219704Bf6aDb785dfccb06deE2",
+                "sd": "0x6d5B86EaC9097EA4a94B2b69Cd4854678B89f839"
+            }
+        },
         "ItemConsumer": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
                             "indexed": false,
@@ -17992,30 +22349,67 @@
         },
         "ItemGoldTraderV2": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": true,
                             "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "startingPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "playerSellPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "minPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "deltaPriceIncrease",
                             "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
                         }
                     ],
                     "name": "ItemAdded",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
@@ -18062,75 +22456,93 @@
                             "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "currentPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "playerSellPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
-                            "internalType": "uint8",
-                            "name": "status",
-                            "type": "uint8"
-                        }
-                    ],
-                    "name": "ItemUpdated",
-                    "type": "event"
-                },
-                {
-                    "anonymous": false,
-                    "inputs": [
+                            "internalType": "uint256",
+                            "name": "minPrice",
+                            "type": "uint256"
+                        },
                         {
                             "indexed": false,
-                            "internalType": "address",
-                            "name": "account",
-                            "type": "address"
-                        }
-                    ],
-                    "name": "Paused",
-                    "type": "event"
-                },
-                {
-                    "anonymous": false,
-                    "inputs": [
+                            "internalType": "uint256",
+                            "name": "deltaPriceIncrease",
+                            "type": "uint256"
+                        },
                         {
                             "indexed": false,
-                            "internalType": "address",
-                            "name": "account",
-                            "type": "address"
+                            "internalType": "uint256",
+                            "name": "decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "status",
+                            "type": "uint8"
                         }
                     ],
-                    "name": "Unpaused",
+                    "name": "ItemUpdated",
                     "type": "event"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_buyPrice",
+                            "name": "_startingPrice",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_sellPrice",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_minPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_deltaPriceIncrease",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_priceIncreaseDecay",
+                            "type": "uint64"
                         }
                     ],
                     "name": "addTradeItem",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
@@ -18160,82 +22572,252 @@
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_quantity",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_maxPrice",
+                            "type": "uint256"
                         }
                     ],
                     "name": "buyItem",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "getTradeItems",
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_itemAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_quantity",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getNextPrice",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getTradeItem",
                     "outputs": [
                         {
                             "components": [
                                 {
                                     "internalType": "uint256",
                                     "name": "id",
                                     "type": "uint256"
                                 },
                                 {
-                                    "internalType": "contract IInventoryItem",
+                                    "internalType": "address",
                                     "name": "item",
                                     "type": "address"
                                 },
                                 {
                                     "internalType": "uint256",
-                                    "name": "buyPrice",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
                                     "type": "uint256"
                                 },
                                 {
                                     "internalType": "uint256",
-                                    "name": "sellPrice",
+                                    "name": "decreaseRate",
                                     "type": "uint256"
                                 },
                                 {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
                                     "internalType": "uint8",
                                     "name": "status",
                                     "type": "uint8"
                                 }
                             ],
-                            "internalType": "struct ItemGoldTrader.TradeItem[]",
+                            "internalType": "struct TraderTypes.TradeItem",
                             "name": "",
-                            "type": "tuple[]"
+                            "type": "tuple"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "address",
-                            "name": "_dfkGoldAddress",
+                            "name": "_itemAddress",
                             "type": "address"
                         }
                     ],
-                    "name": "initialize",
-                    "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "name": "getTradeItemByAddress",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "item",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "decreaseRate",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint8",
+                                    "name": "status",
+                                    "type": "uint8"
+                                }
+                            ],
+                            "internalType": "struct TraderTypes.TradeItem",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [],
-                    "name": "paused",
+                    "name": "getTradeItems",
                     "outputs": [
                         {
-                            "internalType": "bool",
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "item",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "decreaseRate",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint8",
+                                    "name": "status",
+                                    "type": "uint8"
+                                }
+                            ],
+                            "internalType": "struct TraderTypes.TradeItem[]",
                             "name": "",
-                            "type": "bool"
+                            "type": "tuple[]"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
@@ -18267,29 +22849,54 @@
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "id",
                             "type": "uint256"
                         },
                         {
-                            "internalType": "contract IInventoryItem",
+                            "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "currentPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "playerSellPrice",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "minPrice",
                             "type": "uint256"
                         },
                         {
+                            "internalType": "uint256",
+                            "name": "deltaPriceIncrease",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "lastPurchaseTimestamp",
+                            "type": "uint64"
+                        },
+                        {
                             "internalType": "uint8",
                             "name": "status",
                             "type": "uint8"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
@@ -18299,23 +22906,43 @@
                         {
                             "internalType": "address",
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_buyPrice",
+                            "name": "_currentPrice",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_sellPrice",
                             "type": "uint256"
                         },
                         {
+                            "internalType": "uint256",
+                            "name": "_minPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_deltaPriceIncrease",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
                             "internalType": "uint8",
                             "name": "_status",
                             "type": "uint8"
                         }
                     ],
                     "name": "updateTradeItem",
                     "outputs": [],
@@ -23938,14 +28565,460 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0xD507b6b299d9FC835a0Df92f718920D13fA49B47",
                 "sd": "0xdbEE8C336B06f2d30a6d2bB3817a3Ae0E34f4900"
             }
         },
+        "Multicall3": {
+            "ABI": [
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes[]",
+                            "name": "returnData",
+                            "type": "bytes[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "allowFailure",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call3[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate3",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "allowFailure",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "value",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call3Value[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate3Value",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "blockAndAggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getBasefee",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "basefee",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getBlockHash",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getBlockNumber",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getChainId",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "chainid",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockCoinbase",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "coinbase",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockDifficulty",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "difficulty",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "gaslimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockTimestamp",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "timestamp",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "addr",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "getEthBalance",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "balance",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getLastBlockHash",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "requireSuccess",
+                            "type": "bool"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "tryAggregate",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "requireSuccess",
+                            "type": "bool"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "tryBlockAndAggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0xcA11bde05977b3631167028862bE2a173976CA11",
+                "sd": "0xcA11bde05977b3631167028862bE2a173976CA11"
+            }
+        },
         "Pasture": {
             "ABI": [
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_petCore",
@@ -25027,14 +30100,428 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0x72F860bF73ffa3FC42B97BbcF43Ae80280CFcdc3",
                 "sd": "0x7aB1C574A8762bEde901F32670481c0427DdF626"
             }
         },
+        "PetBridge": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "previousAdmin",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "newAdmin",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "AdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "implementation",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Upgraded",
+                    "type": "event"
+                },
+                {
+                    "stateMutability": "payable",
+                    "type": "fallback"
+                },
+                {
+                    "inputs": [],
+                    "name": "admin",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newAdmin",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "changeAdmin",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "implementation",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newImplementation",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "upgradeTo",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newImplementation",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "data",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "upgradeToAndCall",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "stateMutability": "payable",
+                    "type": "receive"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "arrivalChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "PetArrived",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "arrivalChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "PetSent",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "SetTrustedRemote",
+                    "type": "event"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_message",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_executor",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "executeMessage",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_chainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getTrustedRemote",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "trustedRemote",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_messageBus",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_pets",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "initialize",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "messageBus",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "msgGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "pets",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "renounceOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_dstChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "sendPet",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_messageBus",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setMessageBus",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_msgGasLimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setMsgGasLimit",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "setTrustedRemote",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "initialLogic",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "initialAdmin",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_data",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "payable",
+                    "type": "constructor"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x36829ba54e6A0f11fB6e5A45aC5aD2742ec86a0B",
+                "sd": "0x5EcB820B32b60cCEd4506bd3b06C80BaFb879446"
+            }
+        },
         "PetCore": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
                             "indexed": true,
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/abi_contract_wrapper.py` & `dfk_contracts-0.1.6/dfk_contracts/abi_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/abi_multi_contract_wrapper.py` & `dfk_contracts-0.1.6/dfk_contracts/abi_multi_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/all_dfk_contracts.py` & `dfk_contracts-0.1.6/dfk_contracts/all_dfk_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 from .contracts.charity_fund import CharityFund
 from .contracts.crystal_core import CrystalCore
 from .contracts.power_token import PowerToken
 from .contracts.dark_summoning import DarkSummoning
 from .contracts.dfk_duel_s2 import DFKDuelS2
 from .contracts.duel_rank_claim import DuelRankClaim
 from .contracts.erc20 import ERC20
+from .contracts.flag_storage_v2 import FlagStorageV2
 from .contracts.gen0_airdrop import Gen0Airdrop
 from .contracts.gen0_reroll import Gen0Reroll
+from .contracts.gene_reroll import GeneReroll
 from .contracts.hero_auction import HeroAuction
 from .contracts.hero_bridge import HeroBridge
 from .contracts.hero_core import HeroCore
 from .contracts.hero_summoning import HeroSummoning
+from .contracts.item_bridge import ItemBridge
 from .contracts.item_consumer import ItemConsumer
 from .contracts.item_gold_trader_v2 import ItemGoldTraderV2
 from .contracts.jewel_token import JewelToken
 from .contracts.land_auction import LandAuction
 from .contracts.land_core import LandCore
 from .contracts.master_gardener import MasterGardener
 from .contracts.meditation_circle import MeditationCircle
+from .contracts.multicall3 import Multicall3
 from .contracts.pasture import Pasture
 from .contracts.pet_auction import PetAuction
+from .contracts.pet_bridge import PetBridge
 from .contracts.pet_core import PetCore
 from .contracts.pet_exchange import PetExchange
 from .contracts.pet_hatching import PetHatching
 from .contracts.power_up_manager import PowerUpManager
 from .contracts.profiles import Profiles
 from .contracts.quest_core import QuestCore
 from .contracts.raffle_master import RaffleMaster
@@ -64,29 +69,34 @@
         self.charity_fund = CharityFund(self.chain_key, self.rpc)
         self.crystal_core = CrystalCore(self.chain_key, self.rpc)
         self.power_token = PowerToken(self.chain_key, self.rpc)
         self.dark_summoning = DarkSummoning(self.chain_key, self.rpc)
         self.dfk_duel_s2 = DFKDuelS2(self.chain_key, self.rpc)
         self.duel_rank_claim = DuelRankClaim(self.chain_key, self.rpc)
         self.erc20 = ERC20(self.rpc)
+        self.flag_storage_v2 = FlagStorageV2(self.chain_key, self.rpc)
         self.gen0_airdrop = Gen0Airdrop(self.chain_key, self.rpc)
         self.gen0_reroll = Gen0Reroll(self.chain_key, self.rpc)
+        self.gene_reroll = GeneReroll(self.chain_key, self.rpc)
         self.hero_auction = HeroAuction(self.chain_key, self.rpc)
         self.hero_bridge = HeroBridge(self.chain_key, self.rpc)
         self.hero_core = HeroCore(self.chain_key, self.rpc)
         self.hero_summoning = HeroSummoning(self.chain_key, self.rpc)
+        self.item_bridge = ItemBridge(self.chain_key, self.rpc)
         self.item_consumer = ItemConsumer(self.chain_key, self.rpc)
         self.item_gold_trader_v2 = ItemGoldTraderV2(self.chain_key, self.rpc)
         self.jewel_token = JewelToken(self.chain_key, self.rpc)
         self.land_auction = LandAuction(self.chain_key, self.rpc)
         self.land_core = LandCore(self.chain_key, self.rpc)
         self.master_gardener = MasterGardener(self.chain_key, self.rpc)
         self.meditation_circle = MeditationCircle(self.chain_key, self.rpc)
+        self.multicall3 = Multicall3(self.chain_key, self.rpc)
         self.pasture = Pasture(self.chain_key, self.rpc)
         self.pet_auction = PetAuction(self.chain_key, self.rpc)
+        self.pet_bridge = PetBridge(self.chain_key, self.rpc)
         self.pet_core = PetCore(self.chain_key, self.rpc)
         self.pet_exchange = PetExchange(self.chain_key, self.rpc)
         self.pet_hatching = PetHatching(self.chain_key, self.rpc)
         self.power_up_manager = PowerUpManager(self.chain_key, self.rpc)
         self.profiles = Profiles(self.chain_key, self.rpc)
         self.quest_core = QuestCore(self.chain_key, self.rpc)
         self.raffle_master = RaffleMaster(self.chain_key, self.rpc)
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/airdrop_claim.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/airdrop_claim.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/alchemist.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/alchemist.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/assisting_auction.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/assisting_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/atonement_crystal.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/atonement_crystal.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/banker.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/banker.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/birthday_cake.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/birthday_cake.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/charity_fund.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/charity_fund.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/crystal_core.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/crystal_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/dark_summoning.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/dark_summoning.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/dfk_duel_s2.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/dfk_duel_s2.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/duel_rank_claim.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/duel_rank_claim.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/erc20.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/gen0_airdrop.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_airdrop.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/gen0_reroll.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_reroll.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/hero_auction.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/hero_bridge.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_bridge.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/hero_core.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/hero_summoning.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_summoning.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/item_consumer.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/item_consumer.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/item_gold_trader_v2.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pasture.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 
 from ..abi_contract_wrapper import ABIContractWrapper
 from ..solidity_types import *
 from ..credentials import Credentials
 
 CONTRACT_ADDRESS =     {
-    "cv": "0x0f85fdf6c561C42d6b46d0E27ea6Aa9Bf9476B3f",
-    "sd": "0x3Eab8a8F71dDA3e6c907C74302B734805C4f3278"
+    "cv": "0xE959cbddB8616BDFFa5464279664CCbb9EA10317",
+    "sd": "0x4aBb1cDe7a0C55850495E80E1806993b1B92F742"
 }
 
 ABI = """[
-    {"name": "ItemAdded", "type": "event", "inputs": [{"name": "item", "type": "address", "indexed": true, "internalType": "address"}, {"name": "buyPrice", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "sellPrice", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
-    {"name": "ItemTraded", "type": "event", "inputs": [{"name": "player", "type": "address", "indexed": true, "internalType": "address"}, {"name": "boughtItem", "type": "address", "indexed": false, "internalType": "address"}, {"name": "boughtQty", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "soldItem", "type": "address", "indexed": false, "internalType": "address"}, {"name": "soldQty", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
-    {"name": "ItemUpdated", "type": "event", "inputs": [{"name": "item", "type": "address", "indexed": true, "internalType": "address"}, {"name": "buyPrice", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "sellPrice", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "status", "type": "uint8", "indexed": false, "internalType": "uint8"}], "anonymous": false},
-    {"name": "Paused", "type": "event", "inputs": [{"name": "account", "type": "address", "indexed": false, "internalType": "address"}], "anonymous": false},
-    {"name": "Unpaused", "type": "event", "inputs": [{"name": "account", "type": "address", "indexed": false, "internalType": "address"}], "anonymous": false},
-    {"name": "addTradeItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_buyPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_sellPrice", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "addressToTradeItemId", "type": "function", "inputs": [{"name": "", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "buyItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_quantity", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "getTradeItems", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "tuple[]", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "item", "type": "address", "internalType": "contract IInventoryItem"}, {"name": "buyPrice", "type": "uint256", "internalType": "uint256"}, {"name": "sellPrice", "type": "uint256", "internalType": "uint256"}, {"name": "status", "type": "uint8", "internalType": "uint8"}], "internalType": "struct ItemGoldTrader.TradeItem[]"}], "stateMutability": "view"},
-    {"name": "initialize", "type": "function", "inputs": [{"name": "_dfkGoldAddress", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "paused", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "bool", "internalType": "bool"}], "stateMutability": "view"},
-    {"name": "sellItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_quantity", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "tradeItems", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "item", "type": "address", "internalType": "contract IInventoryItem"}, {"name": "buyPrice", "type": "uint256", "internalType": "uint256"}, {"name": "sellPrice", "type": "uint256", "internalType": "uint256"}, {"name": "status", "type": "uint8", "internalType": "uint8"}], "stateMutability": "view"},
-    {"name": "updateTradeItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_buyPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_sellPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_status", "type": "uint8", "internalType": "uint8"}], "outputs": [], "stateMutability": "nonpayable"}
+    {"type": "constructor", "inputs": [{"name": "_petCore", "type": "address", "internalType": "address"}], "stateMutability": "nonpayable"},
+    {"name": "PetReleased", "type": "event", "inputs": [{"name": "petId", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "releaseReason", "type": "string", "indexed": true, "internalType": "string"}, {"name": "releaseTime", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
+    {"name": "getProfileReleasedPet", "type": "function", "inputs": [{"name": "_profile", "type": "address", "internalType": "address"}, {"name": "_index", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "tuple", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet"}], "stateMutability": "view"},
+    {"name": "getProfileReleasedPets", "type": "function", "inputs": [{"name": "_profile", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "tuple[]", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet[]"}], "stateMutability": "view"},
+    {"name": "getReleasedPet", "type": "function", "inputs": [{"name": "_petId", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "tuple", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet"}], "stateMutability": "view"},
+    {"name": "getReleasedPets", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "tuple[]", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet[]"}], "stateMutability": "view"},
+    {"name": "petCore", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "contract IPetCore"}], "stateMutability": "view"},
+    {"name": "petToReleasedPet", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "profileReleasedPets", "type": "function", "inputs": [{"name": "", "type": "address", "internalType": "address"}, {"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "stateMutability": "view"},
+    {"name": "releasePet", "type": "function", "inputs": [{"name": "_holder", "type": "address", "internalType": "address"}, {"name": "_petId", "type": "uint256", "internalType": "uint256"}, {"name": "_releaseReason", "type": "string", "internalType": "string"}, {"name": "_previousOwner", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "releasedPets", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "stateMutability": "view"}
 ]
 """     
 
-class ItemGoldTraderV2(ABIContractWrapper):
+class Pasture(ABIContractWrapper):
     def __init__(self, chain_key:str, rpc:str):
         contract_address = CONTRACT_ADDRESS[chain_key]
         super().__init__(contract_address=contract_address, abi=ABI, rpc=rpc)
 
-    def add_trade_item(self, cred:Credentials, _item_address:address, _buy_price:uint256, _sell_price:uint256) -> TxReceipt:
-        tx = self.contract.functions.addTradeItem(_item_address, _buy_price, _sell_price)
-        return self.send_transaction(tx, cred)
+    def get_profile_released_pet(self, _profile:address, _index:uint256, block_identifier:BlockIdentifier = 'latest') -> tuple:
+        return self.contract.functions.getProfileReleasedPet(_profile, _index).call(block_identifier=block_identifier)
 
-    def address_to_trade_item_id(self, a:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.addressToTradeItemId(a).call(block_identifier=block_identifier)
+    def get_profile_released_pets(self, _profile:address, block_identifier:BlockIdentifier = 'latest') -> List[tuple]:
+        return self.contract.functions.getProfileReleasedPets(_profile).call(block_identifier=block_identifier)
 
-    def buy_item(self, cred:Credentials, _item_address:address, _quantity:uint256) -> TxReceipt:
-        tx = self.contract.functions.buyItem(_item_address, _quantity)
-        return self.send_transaction(tx, cred)
+    def get_released_pet(self, _pet_id:uint256, block_identifier:BlockIdentifier = 'latest') -> tuple:
+        return self.contract.functions.getReleasedPet(_pet_id).call(block_identifier=block_identifier)
 
-    def get_trade_items(self, block_identifier:BlockIdentifier = 'latest') -> List[tuple]:
-        return self.contract.functions.getTradeItems().call(block_identifier=block_identifier)
+    def get_released_pets(self, block_identifier:BlockIdentifier = 'latest') -> List[tuple]:
+        return self.contract.functions.getReleasedPets().call(block_identifier=block_identifier)
 
-    def initialize(self, cred:Credentials, _dfk_gold_address:address) -> TxReceipt:
-        tx = self.contract.functions.initialize(_dfk_gold_address)
-        return self.send_transaction(tx, cred)
+    def pet_core(self, block_identifier:BlockIdentifier = 'latest') -> address:
+        return self.contract.functions.petCore().call(block_identifier=block_identifier)
 
-    def paused(self, block_identifier:BlockIdentifier = 'latest') -> bool:
-        return self.contract.functions.paused().call(block_identifier=block_identifier)
+    def pet_to_released_pet(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.petToReleasedPet(a).call(block_identifier=block_identifier)
 
-    def sell_item(self, cred:Credentials, _item_address:address, _quantity:uint256) -> TxReceipt:
-        tx = self.contract.functions.sellItem(_item_address, _quantity)
-        return self.send_transaction(tx, cred)
+    def profile_released_pets(self, a:address, b:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, uint256, uint64, string, address]:
+        return self.contract.functions.profileReleasedPets(a, b).call(block_identifier=block_identifier)
 
-    def trade_items(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, address, uint256, uint256, uint8]:
-        return self.contract.functions.tradeItems(a).call(block_identifier=block_identifier)
+    def release_pet(self, cred:Credentials, _holder:address, _pet_id:uint256, _release_reason:string, _previous_owner:address) -> TxReceipt:
+        tx = self.contract.functions.releasePet(_holder, _pet_id, _release_reason, _previous_owner)
+        return self.send_transaction(tx, cred)
 
-    def update_trade_item(self, cred:Credentials, _item_address:address, _buy_price:uint256, _sell_price:uint256, _status:uint8) -> TxReceipt:
-        tx = self.contract.functions.updateTradeItem(_item_address, _buy_price, _sell_price, _status)
-        return self.send_transaction(tx, cred)
+    def released_pets(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, uint256, uint64, string, address]:
+        return self.contract.functions.releasedPets(a).call(block_identifier=block_identifier)
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/jewel_token.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/jewel_token.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/land_auction.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/land_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/land_core.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/land_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/master_gardener.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/master_gardener.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/meditation_circle.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/meditation_circle.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/pasture.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/token_disburse.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 
 from ..abi_contract_wrapper import ABIContractWrapper
 from ..solidity_types import *
 from ..credentials import Credentials
 
 CONTRACT_ADDRESS =     {
-    "cv": "0xE959cbddB8616BDFFa5464279664CCbb9EA10317",
-    "sd": "0x4aBb1cDe7a0C55850495E80E1806993b1B92F742"
+    "cv": "0x123165B3a30fdA3655B30cfC10135C1CA3C21bFC",
+    "sd": "0x0000000000000000000000000000000000000000"
 }
 
 ABI = """[
-    {"type": "constructor", "inputs": [{"name": "_petCore", "type": "address", "internalType": "address"}], "stateMutability": "nonpayable"},
-    {"name": "PetReleased", "type": "event", "inputs": [{"name": "petId", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "releaseReason", "type": "string", "indexed": true, "internalType": "string"}, {"name": "releaseTime", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
-    {"name": "getProfileReleasedPet", "type": "function", "inputs": [{"name": "_profile", "type": "address", "internalType": "address"}, {"name": "_index", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "tuple", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet"}], "stateMutability": "view"},
-    {"name": "getProfileReleasedPets", "type": "function", "inputs": [{"name": "_profile", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "tuple[]", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet[]"}], "stateMutability": "view"},
-    {"name": "getReleasedPet", "type": "function", "inputs": [{"name": "_petId", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "tuple", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet"}], "stateMutability": "view"},
-    {"name": "getReleasedPets", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "tuple[]", "components": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "internalType": "struct ReleasedPet[]"}], "stateMutability": "view"},
-    {"name": "petCore", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "contract IPetCore"}], "stateMutability": "view"},
-    {"name": "petToReleasedPet", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "profileReleasedPets", "type": "function", "inputs": [{"name": "", "type": "address", "internalType": "address"}, {"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "stateMutability": "view"},
-    {"name": "releasePet", "type": "function", "inputs": [{"name": "_holder", "type": "address", "internalType": "address"}, {"name": "_petId", "type": "uint256", "internalType": "uint256"}, {"name": "_releaseReason", "type": "string", "internalType": "string"}, {"name": "_previousOwner", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "releasedPets", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "petId", "type": "uint256", "internalType": "uint256"}, {"name": "releaseTime", "type": "uint64", "internalType": "uint64"}, {"name": "releaseReason", "type": "string", "internalType": "string"}, {"name": "previousOwner", "type": "address", "internalType": "address"}], "stateMutability": "view"}
+    {"name": "DisbursementAdded", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "recipient", "type": "address", "indexed": false, "internalType": "address"}, {"name": "amount", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "startTime", "type": "uint64", "indexed": false, "internalType": "uint64"}, {"name": "duration", "type": "uint64", "indexed": false, "internalType": "uint64"}], "anonymous": false},
+    {"name": "DisbursementClaim", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "recipient", "type": "address", "indexed": false, "internalType": "address"}, {"name": "amount", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
+    {"name": "DisbursementUpdated", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "reduction", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "startTime", "type": "uint64", "indexed": false, "internalType": "uint64"}, {"name": "duration", "type": "uint64", "indexed": false, "internalType": "uint64"}], "anonymous": false},
+    {"name": "addDisbursement", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}, {"name": "_amount", "type": "uint256", "internalType": "uint256"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}, {"name": "_note", "type": "string", "internalType": "string"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "addDisbursements", "type": "function", "inputs": [{"name": "_recipients", "type": "address[]", "internalType": "address[]"}, {"name": "_amounts", "type": "uint256[]", "internalType": "uint256[]"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}, {"name": "_note", "type": "string", "internalType": "string"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "claim", "type": "function", "inputs": [{"name": "_amount", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "disbursements", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "recipient", "type": "address", "internalType": "address"}, {"name": "note", "type": "string", "internalType": "string"}, {"name": "total", "type": "uint256", "internalType": "uint256"}, {"name": "claimed", "type": "uint256", "internalType": "uint256"}, {"name": "balance", "type": "uint256", "internalType": "uint256"}, {"name": "createdTime", "type": "uint64", "internalType": "uint64"}, {"name": "startTime", "type": "uint64", "internalType": "uint64"}, {"name": "duration", "type": "uint64", "internalType": "uint64"}], "stateMutability": "view"},
+    {"name": "getDisbursementIds", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256[]", "internalType": "uint256[]"}], "stateMutability": "view"},
+    {"name": "initialize", "type": "function", "inputs": [{"name": "_tokenAddress", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "reservedToken", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "totalClaimed", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "totalUnvested", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "totalVested", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "updateDisbursement", "type": "function", "inputs": [{"name": "_disbursementId", "type": "uint256", "internalType": "uint256"}, {"name": "_reduction", "type": "uint256", "internalType": "uint256"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}], "outputs": [], "stateMutability": "nonpayable"}
 ]
 """     
 
-class Pasture(ABIContractWrapper):
+class TokenDisburse(ABIContractWrapper):
     def __init__(self, chain_key:str, rpc:str):
         contract_address = CONTRACT_ADDRESS[chain_key]
         super().__init__(contract_address=contract_address, abi=ABI, rpc=rpc)
 
-    def get_profile_released_pet(self, _profile:address, _index:uint256, block_identifier:BlockIdentifier = 'latest') -> tuple:
-        return self.contract.functions.getProfileReleasedPet(_profile, _index).call(block_identifier=block_identifier)
+    def add_disbursement(self, cred:Credentials, _recipient:address, _amount:uint256, _start_time:uint64, _duration:uint64, _note:string) -> TxReceipt:
+        tx = self.contract.functions.addDisbursement(_recipient, _amount, _start_time, _duration, _note)
+        return self.send_transaction(tx, cred)
 
-    def get_profile_released_pets(self, _profile:address, block_identifier:BlockIdentifier = 'latest') -> List[tuple]:
-        return self.contract.functions.getProfileReleasedPets(_profile).call(block_identifier=block_identifier)
+    def add_disbursements(self, cred:Credentials, _recipients:Sequence[address], _amounts:Sequence[uint256], _start_time:uint64, _duration:uint64, _note:string) -> TxReceipt:
+        tx = self.contract.functions.addDisbursements(_recipients, _amounts, _start_time, _duration, _note)
+        return self.send_transaction(tx, cred)
 
-    def get_released_pet(self, _pet_id:uint256, block_identifier:BlockIdentifier = 'latest') -> tuple:
-        return self.contract.functions.getReleasedPet(_pet_id).call(block_identifier=block_identifier)
+    def claim(self, cred:Credentials, _amount:uint256) -> TxReceipt:
+        tx = self.contract.functions.claim(_amount)
+        return self.send_transaction(tx, cred)
 
-    def get_released_pets(self, block_identifier:BlockIdentifier = 'latest') -> List[tuple]:
-        return self.contract.functions.getReleasedPets().call(block_identifier=block_identifier)
+    def disbursements(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, address, string, uint256, uint256, uint256, uint64, uint64, uint64]:
+        return self.contract.functions.disbursements(a).call(block_identifier=block_identifier)
 
-    def pet_core(self, block_identifier:BlockIdentifier = 'latest') -> address:
-        return self.contract.functions.petCore().call(block_identifier=block_identifier)
+    def get_disbursement_ids(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> List[uint256]:
+        return self.contract.functions.getDisbursementIds(_recipient).call(block_identifier=block_identifier)
 
-    def pet_to_released_pet(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.petToReleasedPet(a).call(block_identifier=block_identifier)
+    def initialize(self, cred:Credentials, _token_address:address) -> TxReceipt:
+        tx = self.contract.functions.initialize(_token_address)
+        return self.send_transaction(tx, cred)
 
-    def profile_released_pets(self, a:address, b:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, uint256, uint64, string, address]:
-        return self.contract.functions.profileReleasedPets(a, b).call(block_identifier=block_identifier)
+    def reserved_token(self, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.reservedToken().call(block_identifier=block_identifier)
 
-    def release_pet(self, cred:Credentials, _holder:address, _pet_id:uint256, _release_reason:string, _previous_owner:address) -> TxReceipt:
-        tx = self.contract.functions.releasePet(_holder, _pet_id, _release_reason, _previous_owner)
-        return self.send_transaction(tx, cred)
+    def total_claimed(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.totalClaimed(_recipient).call(block_identifier=block_identifier)
+
+    def total_unvested(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.totalUnvested(_recipient).call(block_identifier=block_identifier)
+
+    def total_vested(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.totalVested(_recipient).call(block_identifier=block_identifier)
 
-    def released_pets(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, uint256, uint64, string, address]:
-        return self.contract.functions.releasedPets(a).call(block_identifier=block_identifier)
+    def update_disbursement(self, cred:Credentials, _disbursement_id:uint256, _reduction:uint256, _start_time:uint64, _duration:uint64) -> TxReceipt:
+        tx = self.contract.functions.updateDisbursement(_disbursement_id, _reduction, _start_time, _duration)
+        return self.send_transaction(tx, cred)
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/pet_auction.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/pet_core.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/pet_exchange.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_exchange.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/pet_hatching.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_hatching.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/power_token.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/power_token.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/power_up_manager.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/power_up_manager.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/profiles.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/profiles.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/quest_core.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/quest_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/raffle_master.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_master.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/raffle_ticket.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_ticket.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/stone_carver.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/stone_carver.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/stylist.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/stylist.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/token_disburse.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_bridge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,112 @@
 
 from ..abi_contract_wrapper import ABIContractWrapper
 from ..solidity_types import *
 from ..credentials import Credentials
 
 CONTRACT_ADDRESS =     {
-    "cv": "0x123165B3a30fdA3655B30cfC10135C1CA3C21bFC",
-    "sd": "0x0000000000000000000000000000000000000000"
+    "cv": "0x36829ba54e6A0f11fB6e5A45aC5aD2742ec86a0B",
+    "sd": "0x5EcB820B32b60cCEd4506bd3b06C80BaFb879446"
 }
 
 ABI = """[
-    {"name": "DisbursementAdded", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "recipient", "type": "address", "indexed": false, "internalType": "address"}, {"name": "amount", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "startTime", "type": "uint64", "indexed": false, "internalType": "uint64"}, {"name": "duration", "type": "uint64", "indexed": false, "internalType": "uint64"}], "anonymous": false},
-    {"name": "DisbursementClaim", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "recipient", "type": "address", "indexed": false, "internalType": "address"}, {"name": "amount", "type": "uint256", "indexed": false, "internalType": "uint256"}], "anonymous": false},
-    {"name": "DisbursementUpdated", "type": "event", "inputs": [{"name": "id", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "reduction", "type": "uint256", "indexed": false, "internalType": "uint256"}, {"name": "startTime", "type": "uint64", "indexed": false, "internalType": "uint64"}, {"name": "duration", "type": "uint64", "indexed": false, "internalType": "uint64"}], "anonymous": false},
-    {"name": "addDisbursement", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}, {"name": "_amount", "type": "uint256", "internalType": "uint256"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}, {"name": "_note", "type": "string", "internalType": "string"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "addDisbursements", "type": "function", "inputs": [{"name": "_recipients", "type": "address[]", "internalType": "address[]"}, {"name": "_amounts", "type": "uint256[]", "internalType": "uint256[]"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}, {"name": "_note", "type": "string", "internalType": "string"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "claim", "type": "function", "inputs": [{"name": "_amount", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "disbursements", "type": "function", "inputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "id", "type": "uint256", "internalType": "uint256"}, {"name": "recipient", "type": "address", "internalType": "address"}, {"name": "note", "type": "string", "internalType": "string"}, {"name": "total", "type": "uint256", "internalType": "uint256"}, {"name": "claimed", "type": "uint256", "internalType": "uint256"}, {"name": "balance", "type": "uint256", "internalType": "uint256"}, {"name": "createdTime", "type": "uint64", "internalType": "uint64"}, {"name": "startTime", "type": "uint64", "internalType": "uint64"}, {"name": "duration", "type": "uint64", "internalType": "uint64"}], "stateMutability": "view"},
-    {"name": "getDisbursementIds", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256[]", "internalType": "uint256[]"}], "stateMutability": "view"},
-    {"name": "initialize", "type": "function", "inputs": [{"name": "_tokenAddress", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
-    {"name": "reservedToken", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "totalClaimed", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "totalUnvested", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "totalVested", "type": "function", "inputs": [{"name": "_recipient", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
-    {"name": "updateDisbursement", "type": "function", "inputs": [{"name": "_disbursementId", "type": "uint256", "internalType": "uint256"}, {"name": "_reduction", "type": "uint256", "internalType": "uint256"}, {"name": "_startTime", "type": "uint64", "internalType": "uint64"}, {"name": "_duration", "type": "uint64", "internalType": "uint64"}], "outputs": [], "stateMutability": "nonpayable"}
+    {"name": "AdminChanged", "type": "event", "inputs": [{"name": "previousAdmin", "type": "address", "internalType": "address", "indexed": false}, {"name": "newAdmin", "type": "address", "internalType": "address", "indexed": false}], "anonymous": false},
+    {"name": "Upgraded", "type": "event", "inputs": [{"name": "implementation", "type": "address", "internalType": "address", "indexed": true}], "anonymous": false},
+    {"type": "fallback", "stateMutability": "payable"},
+    {"name": "admin", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "address"}], "stateMutability": "nonpayable"},
+    {"name": "changeAdmin", "type": "function", "inputs": [{"name": "newAdmin", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "implementation", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "address"}], "stateMutability": "nonpayable"},
+    {"name": "upgradeTo", "type": "function", "inputs": [{"name": "newImplementation", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "upgradeToAndCall", "type": "function", "inputs": [{"name": "newImplementation", "type": "address", "internalType": "address"}, {"name": "data", "type": "bytes", "internalType": "bytes"}], "outputs": [], "stateMutability": "payable"},
+    {"type": "receive", "stateMutability": "payable"},
+    {"name": "OwnershipTransferred", "type": "event", "inputs": [{"name": "previousOwner", "type": "address", "internalType": "address", "indexed": true}, {"name": "newOwner", "type": "address", "internalType": "address", "indexed": true}], "anonymous": false},
+    {"name": "PetArrived", "type": "event", "inputs": [{"name": "petId", "type": "uint256", "internalType": "uint256", "indexed": true}, {"name": "arrivalChainId", "type": "uint256", "internalType": "uint256", "indexed": false}], "anonymous": false},
+    {"name": "PetSent", "type": "event", "inputs": [{"name": "petId", "type": "uint256", "internalType": "uint256", "indexed": true}, {"name": "arrivalChainId", "type": "uint256", "internalType": "uint256", "indexed": false}], "anonymous": false},
+    {"name": "SetTrustedRemote", "type": "event", "inputs": [{"name": "_srcChainId", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "_srcAddress", "type": "bytes32", "internalType": "bytes32", "indexed": false}], "anonymous": false},
+    {"name": "executeMessage", "type": "function", "inputs": [{"name": "_srcAddress", "type": "bytes32", "internalType": "bytes32"}, {"name": "_srcChainId", "type": "uint256", "internalType": "uint256"}, {"name": "_message", "type": "bytes", "internalType": "bytes"}, {"name": "_executor", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "getTrustedRemote", "type": "function", "inputs": [{"name": "_chainId", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "trustedRemote", "type": "bytes32", "internalType": "bytes32"}], "stateMutability": "view"},
+    {"name": "initialize", "type": "function", "inputs": [{"name": "_messageBus", "type": "address", "internalType": "address"}, {"name": "_pets", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "messageBus", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "address"}], "stateMutability": "view"},
+    {"name": "msgGasLimit", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
+    {"name": "owner", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "address"}], "stateMutability": "view"},
+    {"name": "pets", "type": "function", "inputs": [], "outputs": [{"name": "", "type": "address", "internalType": "address"}], "stateMutability": "view"},
+    {"name": "renounceOwnership", "type": "function", "inputs": [], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "sendPet", "type": "function", "inputs": [{"name": "_petId", "type": "uint256", "internalType": "uint256"}, {"name": "_dstChainId", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "payable"},
+    {"name": "setMessageBus", "type": "function", "inputs": [{"name": "_messageBus", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "setMsgGasLimit", "type": "function", "inputs": [{"name": "_msgGasLimit", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "setTrustedRemote", "type": "function", "inputs": [{"name": "_srcChainId", "type": "uint256", "internalType": "uint256"}, {"name": "_srcAddress", "type": "bytes32", "internalType": "bytes32"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"name": "transferOwnership", "type": "function", "inputs": [{"name": "newOwner", "type": "address", "internalType": "address"}], "outputs": [], "stateMutability": "nonpayable"},
+    {"type": "constructor", "inputs": [{"name": "initialLogic", "type": "address", "internalType": "address"}, {"name": "initialAdmin", "type": "address", "internalType": "address"}, {"name": "_data", "type": "bytes", "internalType": "bytes"}], "stateMutability": "payable"}
 ]
 """     
 
-class TokenDisburse(ABIContractWrapper):
+class PetBridge(ABIContractWrapper):
     def __init__(self, chain_key:str, rpc:str):
         contract_address = CONTRACT_ADDRESS[chain_key]
         super().__init__(contract_address=contract_address, abi=ABI, rpc=rpc)
 
-    def add_disbursement(self, cred:Credentials, _recipient:address, _amount:uint256, _start_time:uint64, _duration:uint64, _note:string) -> TxReceipt:
-        tx = self.contract.functions.addDisbursement(_recipient, _amount, _start_time, _duration, _note)
+    def admin(self, cred:Credentials) -> TxReceipt:
+        tx = self.contract.functions.admin()
         return self.send_transaction(tx, cred)
 
-    def add_disbursements(self, cred:Credentials, _recipients:Sequence[address], _amounts:Sequence[uint256], _start_time:uint64, _duration:uint64, _note:string) -> TxReceipt:
-        tx = self.contract.functions.addDisbursements(_recipients, _amounts, _start_time, _duration, _note)
+    def change_admin(self, cred:Credentials, new_admin:address) -> TxReceipt:
+        tx = self.contract.functions.changeAdmin(new_admin)
         return self.send_transaction(tx, cred)
 
-    def claim(self, cred:Credentials, _amount:uint256) -> TxReceipt:
-        tx = self.contract.functions.claim(_amount)
+    def implementation(self, cred:Credentials) -> TxReceipt:
+        tx = self.contract.functions.implementation()
         return self.send_transaction(tx, cred)
 
-    def disbursements(self, a:uint256, block_identifier:BlockIdentifier = 'latest') -> Tuple[uint256, address, string, uint256, uint256, uint256, uint64, uint64, uint64]:
-        return self.contract.functions.disbursements(a).call(block_identifier=block_identifier)
+    def upgrade_to(self, cred:Credentials, new_implementation:address) -> TxReceipt:
+        tx = self.contract.functions.upgradeTo(new_implementation)
+        return self.send_transaction(tx, cred)
+
+    def upgrade_to_and_call(self, cred:Credentials, new_implementation:address, data:bytes) -> TxReceipt:
+        tx = self.contract.functions.upgradeToAndCall(new_implementation, data)
+        return self.send_transaction(tx, cred)
+
+    def execute_message(self, cred:Credentials, _src_address:bytes32, _src_chain_id:uint256, _message:bytes, _executor:address) -> TxReceipt:
+        tx = self.contract.functions.executeMessage(_src_address, _src_chain_id, _message, _executor)
+        return self.send_transaction(tx, cred)
 
-    def get_disbursement_ids(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> List[uint256]:
-        return self.contract.functions.getDisbursementIds(_recipient).call(block_identifier=block_identifier)
+    def get_trusted_remote(self, _chain_id:uint256, block_identifier:BlockIdentifier = 'latest') -> bytes32:
+        return self.contract.functions.getTrustedRemote(_chain_id).call(block_identifier=block_identifier)
 
-    def initialize(self, cred:Credentials, _token_address:address) -> TxReceipt:
-        tx = self.contract.functions.initialize(_token_address)
+    def initialize(self, cred:Credentials, _message_bus:address, _pets:address) -> TxReceipt:
+        tx = self.contract.functions.initialize(_message_bus, _pets)
         return self.send_transaction(tx, cred)
 
-    def reserved_token(self, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.reservedToken().call(block_identifier=block_identifier)
+    def message_bus(self, block_identifier:BlockIdentifier = 'latest') -> address:
+        return self.contract.functions.messageBus().call(block_identifier=block_identifier)
+
+    def msg_gas_limit(self, block_identifier:BlockIdentifier = 'latest') -> uint256:
+        return self.contract.functions.msgGasLimit().call(block_identifier=block_identifier)
 
-    def total_claimed(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.totalClaimed(_recipient).call(block_identifier=block_identifier)
+    def owner(self, block_identifier:BlockIdentifier = 'latest') -> address:
+        return self.contract.functions.owner().call(block_identifier=block_identifier)
 
-    def total_unvested(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.totalUnvested(_recipient).call(block_identifier=block_identifier)
+    def pets(self, block_identifier:BlockIdentifier = 'latest') -> address:
+        return self.contract.functions.pets().call(block_identifier=block_identifier)
+
+    def renounce_ownership(self, cred:Credentials) -> TxReceipt:
+        tx = self.contract.functions.renounceOwnership()
+        return self.send_transaction(tx, cred)
 
-    def total_vested(self, _recipient:address, block_identifier:BlockIdentifier = 'latest') -> uint256:
-        return self.contract.functions.totalVested(_recipient).call(block_identifier=block_identifier)
+    def send_pet(self, cred:Credentials, _pet_id:uint256, _dst_chain_id:uint256) -> TxReceipt:
+        tx = self.contract.functions.sendPet(_pet_id, _dst_chain_id)
+        return self.send_transaction(tx, cred)
+
+    def set_message_bus(self, cred:Credentials, _message_bus:address) -> TxReceipt:
+        tx = self.contract.functions.setMessageBus(_message_bus)
+        return self.send_transaction(tx, cred)
+
+    def set_msg_gas_limit(self, cred:Credentials, _msg_gas_limit:uint256) -> TxReceipt:
+        tx = self.contract.functions.setMsgGasLimit(_msg_gas_limit)
+        return self.send_transaction(tx, cred)
+
+    def set_trusted_remote(self, cred:Credentials, _src_chain_id:uint256, _src_address:bytes32) -> TxReceipt:
+        tx = self.contract.functions.setTrustedRemote(_src_chain_id, _src_address)
+        return self.send_transaction(tx, cred)
 
-    def update_disbursement(self, cred:Credentials, _disbursement_id:uint256, _reduction:uint256, _start_time:uint64, _duration:uint64) -> TxReceipt:
-        tx = self.contract.functions.updateDisbursement(_disbursement_id, _reduction, _start_time, _duration)
+    def transfer_ownership(self, cred:Credentials, new_owner:address) -> TxReceipt:
+        tx = self.contract.functions.transferOwnership(new_owner)
         return self.send_transaction(tx, cred)
```

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/uniswap_v2_factory.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_factory.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/uniswap_v2_router.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_router.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/contracts/validator_fund.py` & `dfk_contracts-0.1.6/dfk_contracts/contracts/validator_fund.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.5/dfk_contracts/solidity_types.py` & `dfk_contracts-0.1.6/dfk_contracts/solidity_types.py`

 * *Files identical despite different names*

