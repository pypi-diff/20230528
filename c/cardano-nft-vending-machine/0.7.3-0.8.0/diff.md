# Comparing `tmp/cardano-nft-vending-machine-0.7.3.tar.gz` & `tmp/cardano-nft-vending-machine-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-t7tlnj5a/cardano-nft-vending-machine-0.7.3.tar", last modified: Tue May 16 02:11:09 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-k5fu8eyh/cardano-nft-vending-machine-0.8.0.tar", last modified: Sun May 28 19:08:37 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.7.3.tar` & `cardano-nft-vending-machine-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.086012 cardano-nft-vending-machine-0.7.3/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.7.3/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-16 02:11:09.085603 cardano-nft-vending-machine-0.7.3/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12474 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.7.3/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-16 02:11:01.000000 cardano-nft-vending-machine-0.7.3/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-16 02:11:09.086111 cardano-nft-vending-machine-0.7.3/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.075567 cardano-nft-vending-machine-0.7.3/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.077489 cardano-nft-vending-machine-0.7.3/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.3/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.079789 cardano-nft-vending-machine-0.7.3/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5054 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.080670 cardano-nft-vending-machine-0.7.3/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3931 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5630 2023-05-16 02:10:01.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/network.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11029 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.082885 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2511 2023-05-12 17:49:03.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-16 02:11:09.085088 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-16 02:11:09.000000 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-16 02:11:09.000000 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-16 02:11:09.000000 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-16 02:11:09.000000 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-16 02:11:09.000000 cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.781260 cardano-nft-vending-machine-0.8.0/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.8.0/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-05-28 19:08:37.780821 cardano-nft-vending-machine-0.8.0/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12518 2023-05-27 01:38:09.000000 cardano-nft-vending-machine-0.8.0/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-28 02:54:06.000000 cardano-nft-vending-machine-0.8.0/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-28 19:08:37.781411 cardano-nft-vending-machine-0.8.0/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.769776 cardano-nft-vending-machine-0.8.0/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.772053 cardano-nft-vending-machine-0.8.0/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.0/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.774672 cardano-nft-vending-machine-0.8.0/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5058 2023-05-27 01:37:27.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.775566 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3935 2023-05-27 01:21:05.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     6592 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-15 04:03:06.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/network.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    15480 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      888 2023-05-28 00:24:35.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.778161 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2511 2023-05-12 17:49:03.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-28 19:08:37.780333 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13178 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-28 19:08:37.000000 cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.7.3/LICENSE` & `cardano-nft-vending-machine-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.3/PKG-INFO` & `cardano-nft-vending-machine-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.7.3
+Version: 0.8.0
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,16 @@
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
     # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    price = Balance(10000000, Balance.LOVELACE_POLICY)
+    mint = Mint([price], 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -69,15 +70,15 @@
 ### ``main.py``
 There is a sample vending machine script that is included in the ``src/`` directory to show how to invoke the library components.  Use ``-h`` to see detailed help or use a command like below:
 
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
-                [--mint-price <PRICE_LOVELACE> | --free-mint] \
+                (--mint-price <PRICE> <POLICY_ID>)+ \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.3 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.0 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -29,81 +29,81 @@
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
 directory') # The Mint object below represents your Mint and specifies price,
-and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
-'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
-path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
-where the UTXO sent to the payment address came from blockfrost_api =
-BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
-cli command (used as a utility without any interaction with the network)
-cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
-NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
-max) so long as the mint period is open nft_vending_machine = NftVendingMachine
-('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
-blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
-the state of already-completed UTXOs to avoid double spending errors and uses a
-do-wait-check loop already_completed = set() while _program_is_running:
-nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
-'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
-``main.py`` There is a sample vending machine script that is included in the
-``src/`` directory to show how to invoke the library components. Use ``-h`` to
-see detailed help or use a command like below: python3 main.py [validate | run]
-\ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
-addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
-project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
-\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
-unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
-dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
-Installation This package is available from [PyPI](https://pypi.org/) and can
-be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
-pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
-` directory there are several scripts that can be used to help operationalize
-the vending machine. #### initialize_whitelist.py This file should be used
-exactly once to initialize an asset-based whitelist for an existing NFT policy
-with *ALL* of the assets that are currently minted. Note that the
-`CONSUMED_DIR` folder is created but left empty so that the vending machine
-(e.g., started with `main.py`) can use it during running. usage:
-initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
-consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
-whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
-NFT policy optional arguments: -h, --help show this help message and exit --
-blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
-retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
-whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
-initializer against mainnet assets (default is False [preprod]) --policy-id
-POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
-initializer against preview assets (default is False [preprod]) --whitelist-dir
-WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
-EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
-each asset on the whitelist #### upload_wl_usage.py This file should be run
-continuously during a whitelist mint to upload changes in the assets used for
-consumption by external parties. Note that if there are any performance issues
-(e.g., IOPS throughput) with the local vending machine filesystem it is
-recommended you not use this file. It is kept separate from the main vending
-machine operation to avoid any synchronization or performance issues as it is
-not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
-upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
-recently used in the vending machine optional arguments: -h, --help show this
-help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
-that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
-used whitelist information if any changes (can be same as --old-wl-file) --
-whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
-gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
-folder where unused whitelist files are stored to be processed by vending
-machine --credentials CREDENTIALS JSON-formatted application-specific
-credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
-whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
-generated from ``pydoc3``-formatted multi-line strings in the source code. A
-mirror of ``master`` is hosted on [Github Pages](https://
+and developer fee in Lovelace (both can be 0) price = Balance(10000000,
+Balance.LOVELACE_POLICY) mint = Mint([price], 1000000, 'addr1_developer', '/
+path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey',
+whitelist) # Blockfrost is used in the code to validate where the UTXO sent to
+the payment address came from blockfrost_api = BlockfrostApi('', mainnet=True)
+# CardanoCli is a wrapper around the cardano-cli command (used as a utility
+without any interaction with the network) cardano_cli = CardanoCli
+(protocol_params='/path/to/protocol.json') # NftVendingMachine vends NFTs and
+needs to be called repeatedly (with a 25-vend max) so long as the mint period
+is open nft_vending_machine = NftVendingMachine('addr_payment', '/path/to/
+payment.skey', 'addr_profit', 25, mint, blockfrost_api, cardano_cli,
+mainnet=True) # The following simple loop carries the state of already-
+completed UTXOs to avoid double spending errors and uses a do-wait-check loop
+already_completed = set() while _program_is_running: nft_vending_machine.vend
+('/path/to/output/dir', 'locking_subdir_name', 'metadata_subdir_name',
+already_completed) time.sleep(WAIT_TIMEOUT) ### ``main.py`` There is a sample
+vending machine script that is included in the ``src/`` directory to show how
+to invoke the library components. Use ``-h`` to see detailed help or use a
+command like below: python3 main.py [validate | run] \ --payment-addr  \ --
+payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-addr  \ (--mint-price
+)+ \ --mint-script /FULL/PATH/TO/policy.script \ --mint-sign-key /FULL/PATH/TO/
+policy.skey \ --blockfrost-project  \ --metadata-dir metadata/ \ --output-dir
+output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist | \ [--
+single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
+whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
+additional] \ [--mainnet] ## Installation This package is available from [PyPI]
+(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
+currently unsupported at this time. pip3 install cardano-nft-vending-machine
+### Scripts In the `scripts/` directory there are several scripts that can be
+used to help operationalize the vending machine. #### initialize_whitelist.py
+This file should be used exactly once to initialize an asset-based whitelist
+for an existing NFT policy with *ALL* of the assets that are currently minted.
+Note that the `CONSUMED_DIR` folder is created but left empty so that the
+vending machine (e.g., started with `main.py`) can use it during running.
+usage: initialize_whitelist.py [-h] asset --blockfrost-project
+BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
+POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
+whitelist for an existing NFT policy optional arguments: -h, --help show this
+help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
+project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
+folder where consumed whitelist files will go after processing (MUST NOT YET
+EXIST) --mainnet Run the initializer against mainnet assets (default is False
+[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
+preview Run the initializer against preview assets (default is False [preprod])
+--whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
+(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
+available for each asset on the whitelist #### upload_wl_usage.py This file
+should be run continuously during a whitelist mint to upload changes in the
+assets used for consumption by external parties. Note that if there are any
+performance issues (e.g., IOPS throughput) with the local vending machine
+filesystem it is recommended you not use this file. It is kept separate from
+the main vending machine operation to avoid any synchronization or performance
+issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
+OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
+CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
+assets have been recently used in the vending machine optional arguments: -h, -
+-help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
+of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
+store the new used whitelist information if any changes (can be same as --old-
+wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.7.3/README.md` & `cardano-nft-vending-machine-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
     # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    price = Balance(10000000, Balance.LOVELACE_POLICY)
+    mint = Mint([price], 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -54,15 +55,15 @@
 ### ``main.py``
 There is a sample vending machine script that is included in the ``src/`` directory to show how to invoke the library components.  Use ``-h`` to see detailed help or use a command like below:
 
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
-                [--mint-price <PRICE_LOVELACE> | --free-mint] \
+                (--mint-price <PRICE> <POLICY_ID>)+ \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
```

#### html2text {}

```diff
@@ -20,81 +20,81 @@
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
 directory') # The Mint object below represents your Mint and specifies price,
-and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
-'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
-path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
-where the UTXO sent to the payment address came from blockfrost_api =
-BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
-cli command (used as a utility without any interaction with the network)
-cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
-NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
-max) so long as the mint period is open nft_vending_machine = NftVendingMachine
-('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
-blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
-the state of already-completed UTXOs to avoid double spending errors and uses a
-do-wait-check loop already_completed = set() while _program_is_running:
-nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
-'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
-``main.py`` There is a sample vending machine script that is included in the
-``src/`` directory to show how to invoke the library components. Use ``-h`` to
-see detailed help or use a command like below: python3 main.py [validate | run]
-\ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
-addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
-project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
-\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
-unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
-dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
-Installation This package is available from [PyPI](https://pypi.org/) and can
-be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
-pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
-` directory there are several scripts that can be used to help operationalize
-the vending machine. #### initialize_whitelist.py This file should be used
-exactly once to initialize an asset-based whitelist for an existing NFT policy
-with *ALL* of the assets that are currently minted. Note that the
-`CONSUMED_DIR` folder is created but left empty so that the vending machine
-(e.g., started with `main.py`) can use it during running. usage:
-initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
-consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
-whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
-NFT policy optional arguments: -h, --help show this help message and exit --
-blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
-retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
-whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
-initializer against mainnet assets (default is False [preprod]) --policy-id
-POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
-initializer against preview assets (default is False [preprod]) --whitelist-dir
-WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
-EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
-each asset on the whitelist #### upload_wl_usage.py This file should be run
-continuously during a whitelist mint to upload changes in the assets used for
-consumption by external parties. Note that if there are any performance issues
-(e.g., IOPS throughput) with the local vending machine filesystem it is
-recommended you not use this file. It is kept separate from the main vending
-machine operation to avoid any synchronization or performance issues as it is
-not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
-upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
-recently used in the vending machine optional arguments: -h, --help show this
-help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
-that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
-used whitelist information if any changes (can be same as --old-wl-file) --
-whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
-gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
-folder where unused whitelist files are stored to be processed by vending
-machine --credentials CREDENTIALS JSON-formatted application-specific
-credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
-whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
-generated from ``pydoc3``-formatted multi-line strings in the source code. A
-mirror of ``master`` is hosted on [Github Pages](https://
+and developer fee in Lovelace (both can be 0) price = Balance(10000000,
+Balance.LOVELACE_POLICY) mint = Mint([price], 1000000, 'addr1_developer', '/
+path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey',
+whitelist) # Blockfrost is used in the code to validate where the UTXO sent to
+the payment address came from blockfrost_api = BlockfrostApi('', mainnet=True)
+# CardanoCli is a wrapper around the cardano-cli command (used as a utility
+without any interaction with the network) cardano_cli = CardanoCli
+(protocol_params='/path/to/protocol.json') # NftVendingMachine vends NFTs and
+needs to be called repeatedly (with a 25-vend max) so long as the mint period
+is open nft_vending_machine = NftVendingMachine('addr_payment', '/path/to/
+payment.skey', 'addr_profit', 25, mint, blockfrost_api, cardano_cli,
+mainnet=True) # The following simple loop carries the state of already-
+completed UTXOs to avoid double spending errors and uses a do-wait-check loop
+already_completed = set() while _program_is_running: nft_vending_machine.vend
+('/path/to/output/dir', 'locking_subdir_name', 'metadata_subdir_name',
+already_completed) time.sleep(WAIT_TIMEOUT) ### ``main.py`` There is a sample
+vending machine script that is included in the ``src/`` directory to show how
+to invoke the library components. Use ``-h`` to see detailed help or use a
+command like below: python3 main.py [validate | run] \ --payment-addr  \ --
+payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-addr  \ (--mint-price
+)+ \ --mint-script /FULL/PATH/TO/policy.script \ --mint-sign-key /FULL/PATH/TO/
+policy.skey \ --blockfrost-project  \ --metadata-dir metadata/ \ --output-dir
+output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist | \ [--
+single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
+whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
+additional] \ [--mainnet] ## Installation This package is available from [PyPI]
+(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
+currently unsupported at this time. pip3 install cardano-nft-vending-machine
+### Scripts In the `scripts/` directory there are several scripts that can be
+used to help operationalize the vending machine. #### initialize_whitelist.py
+This file should be used exactly once to initialize an asset-based whitelist
+for an existing NFT policy with *ALL* of the assets that are currently minted.
+Note that the `CONSUMED_DIR` folder is created but left empty so that the
+vending machine (e.g., started with `main.py`) can use it during running.
+usage: initialize_whitelist.py [-h] asset --blockfrost-project
+BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
+POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
+whitelist for an existing NFT policy optional arguments: -h, --help show this
+help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
+project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
+folder where consumed whitelist files will go after processing (MUST NOT YET
+EXIST) --mainnet Run the initializer against mainnet assets (default is False
+[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
+preview Run the initializer against preview assets (default is False [preprod])
+--whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
+(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
+available for each asset on the whitelist #### upload_wl_usage.py This file
+should be run continuously during a whitelist mint to upload changes in the
+assets used for consumption by external parties. Note that if there are any
+performance issues (e.g., IOPS throughput) with the local vending machine
+filesystem it is recommended you not use this file. It is kept separate from
+the main vending machine operation to avoid any synchronization or performance
+issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
+OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
+CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
+assets have been recently used in the vending machine optional arguments: -h, -
+-help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
+of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
+store the new used whitelist information if any changes (can be same as --old-
+wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.7.3/pyproject.toml` & `cardano-nft-vending-machine-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.7.3"
+version = "0.8.0"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/blockfrost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import time
 
 from http import HTTPStatus
 
 from cardano.wt import network
-from cardano.wt.utxo import Utxo
+from cardano.wt.utxo import Utxo, Balance
 
 """
 Repreentation of the Blockfrost web API used in retrieving metadata about txn i/o on the chain.
 """
 class BlockfrostApi(object):
 
     PREPROD_MAGIC = network.PREPROD_MAGIC
@@ -112,15 +112,15 @@
         return self.__call_get_api(f"txs/{txn_hash}/metadata")
 
     def get_utxos(self, address, exclusions):
         available_utxos = list()
         for utxo_data in self.__call_paginated_get_api(f"addresses/{address}/utxos"):
             #print('EXCLUSIONS\t', [f'{utxo.hash}#{utxo.ix}' for utxo in exclusions])
             for raw_utxo in utxo_data:
-                balances = [Utxo.Balance(int(balance['quantity']), balance['unit']) for balance in raw_utxo['amount']]
+                balances = [Balance(int(balance['quantity']), balance['unit']) for balance in raw_utxo['amount']]
                 utxo = Utxo(raw_utxo['tx_hash'], raw_utxo['output_index'], balances)
                 if utxo in exclusions or utxo in available_utxos:
                     print(f'Skipping {utxo.hash}#{utxo.ix}')
                     continue
                 available_utxos.append(utxo)
         return available_utxos
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/cardano_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         print(cmd)
         cli_cmd = subprocess.Popen(cmd,  shell=True, text=True, stdout=subprocess.PIPE)
         (out, err) = cli_cmd.communicate()
         print(f'[STDOUT] {out}')
         print(f'[STDERR] {err}')
         return out
 
-    def named_assets_str(nft_policy_map):
+    def __named_assets_str(nft_policy_map):
         named_assets = []
         for policy in nft_policy_map:
             for nft_name in nft_policy_map[policy]:
                 hex_name = nft_name.encode('UTF-8').hex()
                 named_assets.append(f"{policy}.{hex_name}")
         return '+'.join([f"1 {named_asset}" for named_asset in named_assets])
 
@@ -43,15 +43,15 @@
                 {metadata_file_args} --out-file {raw_build_file} {" ".join(addl_args)}'
         )
         return raw_build_file
 
     def build_raw_mint_txn(self, output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, mint, nft_policy_map, scripts_map):
         mint_args = []
         if nft_policy_map:
-            named_asset_str = CardanoCli.named_assets_str(nft_policy_map)
+            named_asset_str = CardanoCli.__named_assets_str(nft_policy_map)
             mint_args.append(f"--mint=\"{named_asset_str}\"")
             mint_args.extend([f"--minting-script-file {scripts_map[script]}" for script in scripts_map if script in nft_policy_map])
         if mint.initial_slot:
             mint_args.append(f"--invalid-before {mint.initial_slot}")
         if mint.expiration_slot:
             mint_args.append(f"--invalid-hereafter {mint.expiration_slot}")
         return self.build_raw_txn(output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, mint_args)
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/mint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import math
 import os
 
-from cardano.wt.utxo import Utxo
+from cardano.wt.utxo import Utxo, Balance
 
 """
 Representation of the current minting process.
 """
 class Mint(object):
 
     _METADATA_KEY = '721'
@@ -37,16 +37,16 @@
             script_json = json.load(script_file)
         if 'scripts' in script_json:
             for validator in script_json['scripts']:
                 if validator['type'] == validation:
                     return validator[key]
         return None
 
-    def __init__(self, price, dev_fee, dev_addr, nfts_dir, scripts, sign_keys, whitelist, bogo=None):
-        self.price = price
+    def __init__(self, prices, dev_fee, dev_addr, nfts_dir, scripts, sign_keys, whitelist, bogo=None):
+        self.prices = prices
         self.dev_fee = dev_fee
         self.dev_addr = dev_addr
         self.nfts_dir = nfts_dir
         self.scripts = scripts
         self.sign_keys = sign_keys
         self.whitelist = whitelist
         self.bogo = bogo
@@ -57,16 +57,28 @@
         self.expiration_slot = min(before_slots) if before_slots else None
 
     def validate(self):
         if self.dev_fee and self.dev_fee < Utxo.MIN_UTXO_VALUE:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but the minUTxO on Cardano is {Utxo.MIN_UTXO_VALUE} lovelace")
         if self.dev_fee and not self.dev_addr:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but you did not provide a dev address")
-        if self.price and self.price < Mint._MIN_PRICE:
-            raise ValueError(f"Minimum mint price is {Mint._MIN_PRICE}, you entered {self.price}")
+        validated_price_policies = []
+        if not self.prices:
+            raise ValueError("Must specify at least one valid mint price, even if 0 ADA for free mint")
+        for price in self.prices:
+            if price.policy != Balance.LOVELACE_POLICY:
+                if len(price.policy) <= Mint._POLICY_LEN or price.policy[Mint._POLICY_LEN] != '.':
+                    raise ValueError(f"Price unit '{price.policy}' does not look like a valid unit name")
+            if price.policy == Balance.LOVELACE_POLICY and price.lovelace and price.lovelace < Mint._MIN_PRICE:
+                raise ValueError(f"Minimum mint price is {Mint._MIN_PRICE}, you entered {price.lovelace} {Balance.LOVELACE_POLICY}")
+            if not price.lovelace and price.policy != Balance.LOVELACE_POLICY:
+                raise ValueError(f"Detected invalid zero price for non-ADA policy '{price.policy}'")
+            if price.policy in validated_price_policies:
+                raise ValueError(f"Duplicate price detected for policy '{price.policy}', aborting")
+            validated_price_policies.append(price.policy)
         validated_names = []
         for filename in os.listdir(self.nfts_dir):
             with open(os.path.join(self.nfts_dir, filename), 'r') as file:
                 print(f"Validating '{filename}'")
                 validated_nfts = self.__validated_nft(json.load(file), validated_names, filename)
                 validated_names.extend(validated_nfts)
         self.validated_names = validated_names
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/nft_vending_machine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import copy
 import json
 import math
 import os
 import random
 import shutil
 import time
 import traceback
 
 from cardano.wt.cardano_cli import CardanoCli
 from cardano.wt.mint import Mint
-from cardano.wt.utxo import Utxo
+from cardano.wt.utxo import Utxo, Balance
 
 class BadUtxoError(ValueError):
 
     def __init__(self, utxo, message):
         super().__init__(message)
         self.utxo = utxo
 
@@ -32,20 +33,24 @@
         self.single_vend_max = single_vend_max
         self.mint = mint
         self.blockfrost_api = blockfrost_api
         self.cardano_cli = cardano_cli
         self.mainnet = mainnet
         self.__is_validated = False
 
-    def __get_tx_out_args(self, input_addr, change, nft_policy_map, total_profit, total_dev_fee):
-        user_tokens = filter(None, [input_addr, str(change), CardanoCli.named_assets_str(nft_policy_map)])
-        user_output = f"--tx-out \"{'+'.join(user_tokens)}\""
-        profit_output = f"--tx-out \"{self.profit_addr}+{total_profit}\"" if total_profit else ''
-        dev_output = f"--tx-out \"{self.mint.dev_addr}+{total_dev_fee}\"" if total_dev_fee else ''
-        return [user_output, profit_output, dev_output]
+    def __get_tx_out_args(self, payees):
+        tx_outs = []
+        for payee in payees:
+            payouts = payees[payee]
+            if not payee or not payouts:
+                continue
+            payout_str = '+'.join([f"{payouts[policy]} {policy}" for policy in payouts if payouts[policy]])
+            if payout_str:
+                tx_outs.append(f'--tx-out "{payee}+{payout_str}"')
+        return tx_outs
 
     def __get_policy_name_map(self, metadata_file):
         nft_names = {}
         with open(metadata_file, 'r') as metadata_filehandle:
             cip25_metadata = json.load(metadata_filehandle)['721']
             for policy in cip25_metadata:
                 if policy == 'version':
@@ -70,91 +75,176 @@
             mint_metadata_locked = os.path.join(output_dir, locked_subdir, mint_metadata_filename)
             shutil.move(mint_metadata_orig, mint_metadata_locked)
         combined_output_path = os.path.join(output_dir, metadata_subdir, f"{txn_id}.json")
         with open(combined_output_path, 'w') as combined_metadata_handle:
             json.dump({'721': combined_nft_metadata }, combined_metadata_handle)
         return combined_output_path
 
+    def __calculate_num_mints_requested(self, mint_req):
+        num_mints_requested = 0
+        for balance in mint_req.balances:
+            mint_rate = [price for price in self.mint.prices if self.__normalized_unit(balance.policy) == price.policy]
+            if not mint_rate:
+                continue
+            num_mints_requested += math.floor(balance.lovelace / mint_rate[0].lovelace) if mint_rate[0].lovelace else self.single_vend_max
+        return num_mints_requested
+
+    def __normalized_unit(self, policy):
+        if policy == Balance.LOVELACE_POLICY:
+            return policy
+        return f"{policy[0:Mint._POLICY_LEN]}.{policy[Mint._POLICY_LEN:]}"
+
+    def __get_pricing_breakdown(self, input_addr, num_mints, nft_policy_map, mint_req, fee):
+        payees = {input_addr: {}, self.profit_addr: {}, self.mint.dev_addr: {}}
+
+        # GET A COPY OF THE UTXOs TO TRACK THE PAYOUTS (PUT LOVELACE BEFORE NATIVE ASSETS)
+        print(f"Building pricing breakdown for {num_mints} NFTs being paid from {mint_req}")
+        remaining = copy.deepcopy(mint_req.balances)
+        remaining.sort(key=lambda balance: balance.policy)
+        remaining.reverse()
+        remaining_ada = [balance for balance in remaining if balance.policy == Balance.LOVELACE_POLICY][0]
+
+        # PAY THE CREATOR
+        remaining_to_payout = num_mints
+        for remainder in remaining:
+            unit = self.__normalized_unit(remainder.policy)
+            if not remaining_to_payout:
+                break
+            matching_price = [price for price in self.mint.prices if price.policy == unit]
+            if not matching_price:
+                continue
+            if not matching_price[0].lovelace:
+                num_paid_for = num_mints
+            else:
+                num_paid_for = min(remaining_to_payout, math.floor(remainder.lovelace / matching_price[0].lovelace))
+            total_paid = (num_paid_for * matching_price[0].lovelace)
+            print(f"Paid for {num_paid_for} NFTs using {total_paid} {unit}")
+            if not num_paid_for:
+                continue
+            remaining_to_payout -= num_paid_for
+            remainder.lovelace -= total_paid
+            if not unit in payees[self.profit_addr]:
+                payees[self.profit_addr][unit] = 0
+            payees[self.profit_addr][unit] += total_paid
+        if not Balance.LOVELACE_POLICY in payees[self.profit_addr]:
+            if payees[self.profit_addr]:
+                token_types = set([unit[0:Mint._POLICY_LEN] for unit in payees[self.profit_addr].keys()])
+                all_tokens = [bytes.fromhex(unit[(Mint._POLICY_LEN + 1):]).decode('UTF-8') for unit in payees[self.profit_addr].keys()]
+                total_token_chars = sum([len(token) for token in all_tokens])
+                profit_rebate = Mint.RebateCalculator.calculate_rebate_for(len(token_types), len(all_tokens), total_token_chars)
+                payees[self.profit_addr][Balance.LOVELACE_POLICY] = profit_rebate
+                remaining_ada.lovelace -= profit_rebate
+            else:
+                payees[self.profit_addr][Balance.LOVELACE_POLICY] = 0
+        profit_ada = payees[self.profit_addr][Balance.LOVELACE_POLICY]
+        if remaining_to_payout:
+            raise ValueError(f"Unable to match UTxO to payment for {num_mints} NFTs")
+
+        # PAY THE USER THE NFTs NEXT
+        for policy in nft_policy_map:
+            for nft_name in nft_policy_map[policy]:
+                hex_name = nft_name.encode('UTF-8').hex()
+                asset_name = f"{policy}.{hex_name}"
+                if not asset_name in payees[input_addr]:
+                    payees[input_addr][asset_name] = 0
+                payees[input_addr][asset_name] += 1
+
+        # PAY THE USER'S REBATE AFTER NFTs CALCULATED
+        all_names = [name for name_lst in nft_policy_map.values() for name in name_lst]
+        total_name_chars = sum([len(name) for name in all_names])
+        user_rebate = Mint.RebateCalculator.calculate_rebate_for(len(nft_policy_map.keys()), len(all_names), total_name_chars)
+        print(f"Minimum rebate to user is {user_rebate}")
+
+        # DEDUCT REBATES AND FEES FROM PROFIT IF ADA-ONLY MINT, OTHERWISE FROM USER
+        payees[input_addr][Balance.LOVELACE_POLICY] = user_rebate
+        if profit_ada and len(payees[self.profit_addr]) == 1:
+            payees[self.profit_addr][Balance.LOVELACE_POLICY] -= (user_rebate + fee)
+        elif user_rebate > remaining_ada.lovelace:
+            raise ValueError(f"USER SENT {remaining_ada.lovelace} WHICH CAN'T COVER REBATE OF {user_rebate} (FREE MINT?)")
+        else:
+            remaining_ada.lovelace -= (user_rebate + fee)
+
+        # PAY THE DEVELOPER (ADA ONLY)
+        if self.mint.dev_fee:
+            expected_dev_fee = num_mints * self.mint.dev_fee
+            if len(payees[self.profit_addr]) == 1:
+                actual_dev_fee = min([expected_dev_fee, profit_ada])
+                print(f"Paying developer {actual_dev_fee} lovelace")
+                dev_fee_diff = expected_dev_fee - actual_dev_fee
+                if dev_fee_diff:
+                    print(f"SOMETHING IS OFF: Expected dev fee ({expected_dev_fee}) greater than actual ({actual_dev_fee}) by {dev_fee_diff} lovelace")
+                payees[self.mint.dev_addr][Balance.LOVELACE_POLICY] = actual_dev_fee
+                payees[self.profit_addr][Balance.LOVELACE_POLICY] -= actual_dev_fee
+            else:
+                print(f"NATIVE TOKEN WARNING: Cannot pay dev fee for native token, need to credit {expected_dev_fee} lovelace ({num_mints} mints)")
+
+        # DRAIN THE REMAINDER TO THE USER
+        for remainder in remaining:
+            unit = self.__normalized_unit(remainder.policy)
+            if not remainder.lovelace:
+                continue
+            if not unit in payees[input_addr]:
+                payees[input_addr][unit] = 0
+            payees[input_addr][unit] += remainder.lovelace
+            remainder.lovelace = 0
+        return payees
+
     def __do_vend(self, mint_req, output_dir, locked_subdir, metadata_subdir):
         available_mints = sorted(os.listdir(self.mint.nfts_dir))
         if not available_mints:
             print("WARNING: Metadata directory is empty, please restock the vending machine...")
         elif self.vend_randomly:
             random.shuffle(available_mints)
 
-        non_lovelace_bals = [balance for balance in mint_req.balances if balance.policy != Utxo.Balance.LOVELACE_POLICY]
-        if non_lovelace_bals:
-            raise BadUtxoError(mint_req, f"Cannot accept non-lovelace balances as payment")
-
-        lovelace_bals = [balance for balance in mint_req.balances if balance.policy == Utxo.Balance.LOVELACE_POLICY]
-        if len(lovelace_bals) != 1:
-            raise BadUtxoError(mint_req, f"Found too many/few lovelace balances for UTXO {mint_req}")
-
-        lovelace_bal = lovelace_bals.pop()
-        num_mints_requested = math.floor(lovelace_bal.lovelace / self.mint.price) if self.mint.price else self.single_vend_max
-        if not num_mints_requested:
-            raise BadUtxoError(mint_req, f"User intentionally sent too little lovelace, avoiding txn processing to avoid DDoS")
+        num_mints_requested = self.__calculate_num_mints_requested(mint_req)
 
         utxos = self.blockfrost_api.get_tx_utxos(mint_req.hash)
         utxo_inputs = utxos['inputs']
         utxo_outputs = utxos['outputs']
         input_addrs = set([utxo_input['address'] for utxo_input in utxo_inputs if not utxo_input['reference']])
         if len(input_addrs) < 1:
             raise BadUtxoError(mint_req, f"Txn hash {txn_hash} has no valid addresses ({utxo_inputs}), aborting...")
         input_addr = input_addrs.pop()
 
         wl_resources = self.mint.whitelist.required_info(mint_req, utxos, self.blockfrost_api)
         wl_availability = self.mint.whitelist.available(wl_resources)
         num_mints = min(self.single_vend_max, len(available_mints), num_mints_requested, wl_availability)
 
-        if not self.mint.price and self.max_rebate > lovelace_bal.lovelace:
-            print(f"Payment of {lovelace_bal.lovelace} might cause minUTxO error for {num_mints} NFTs, refunding instead...")
-            num_mints = 0
-
-        gross_profit = num_mints * self.mint.price
-        dev_fee = num_mints * self.mint.dev_fee
-        change = lovelace_bal.lovelace - gross_profit
-
+        bonuses = 0
         if self.mint.bogo:
-            bonuses = self.mint.bogo.determine_bonuses(num_mints_requested)
-            print(f"Bonus of {bonuses} NFTs determined based on {num_mints_requested}")
-            num_mints = min(self.single_vend_max, len(available_mints), (num_mints + bonuses))
+            eligible_bonuses = self.mint.bogo.determine_bonuses(num_mints_requested)
+            num_mints_plus_bonus = min(self.single_vend_max, len(available_mints), (num_mints + eligible_bonuses))
+            print(f"Bonus of {eligible_bonuses} NFTs determined based on {num_mints_requested} (can mint {num_mints_plus_bonus} in total)")
+            bonuses = num_mints_plus_bonus - num_mints
+            num_mints += bonuses
 
         print(f"Beginning to mint {num_mints} NFTs to send to address {input_addr}")
         txn_id = int(time.time())
         nft_metadata_file = self.__lock_and_merge(available_mints, num_mints, output_dir, locked_subdir, metadata_subdir, txn_id)
         nft_policy_map = self.__get_policy_name_map(nft_metadata_file)
 
-        all_names = [name for name_lst in nft_policy_map.values() for name in name_lst]
-        total_name_chars = sum([len(name) for name in all_names])
-        user_rebate = Mint.RebateCalculator.calculate_rebate_for(len(nft_policy_map.keys()), len(all_names), total_name_chars) if self.mint.price else 0
-        net_profit = gross_profit - dev_fee - user_rebate
-        print(f"Minimum rebate to user is {user_rebate}, net profit to vault is {net_profit}")
+        fee = 0
+        pricing_breakdown = self.__get_pricing_breakdown(input_addr, (num_mints - bonuses), nft_policy_map, mint_req, fee)
+        print(f"Anticipated pricing breakdown: {pricing_breakdown}")
 
         tx_ins = [f"--tx-in {mint_req.hash}#{mint_req.ix}"]
-        tx_outs = self.__get_tx_out_args(input_addr, user_rebate + change, nft_policy_map, net_profit, dev_fee)
+        tx_outs = self.__get_tx_out_args(pricing_breakdown)
         mint_build_tmp = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, 0, nft_metadata_file, self.mint, nft_policy_map, self.script_map)
 
         tx_in_count = len(tx_ins)
         tx_out_count = len([tx_out for tx_out in tx_outs if tx_out])
         signers = [self.payment_sign_key]
         if num_mints:
             signers.extend(self.mint.sign_keys)
         fee = self.cardano_cli.calculate_min_fee(mint_build_tmp, tx_in_count, tx_out_count, len(signers))
 
-        if net_profit:
-            net_profit = net_profit - fee
-        else:
-            change = change - fee
-
-        final_change = user_rebate + change
-        if (final_change and (final_change < Utxo.MIN_UTXO_VALUE)) or (net_profit and (net_profit < Utxo.MIN_UTXO_VALUE)):
-            raise BadUtxoError(mint_req, f"UTxO left change of {change}, and net_profit of {net_profit}, causing a minUTxO error")
+        pricing_breakdown = self.__get_pricing_breakdown(input_addr, (num_mints - bonuses), nft_policy_map, mint_req, fee)
+        print(f"Final pricing breakdown: {pricing_breakdown}")
 
-        tx_outs = self.__get_tx_out_args(input_addr, final_change, nft_policy_map, net_profit, dev_fee)
+        tx_outs = self.__get_tx_out_args(pricing_breakdown)
         mint_build = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, fee, nft_metadata_file, self.mint, nft_policy_map, self.script_map)
         mint_signed = self.cardano_cli.sign_txn(signers, mint_build)
         self.mint.whitelist.consume(wl_resources, num_mints)
         self.blockfrost_api.submit_txn(mint_signed)
 
     def vend(self, output_dir, locked_subdir, metadata_subdir, exclusions):
         if not self.__is_validated:
@@ -164,25 +254,26 @@
             exclusions.add(mint_req)
             try:
                 self.__do_vend(mint_req, output_dir, locked_subdir, metadata_subdir)
             except BadUtxoError as e:
                 print(f"UNRECOVERABLE UTXO ERROR\n{e.utxo}\n^--- REQUIRES INVESTIGATION")
                 print(traceback.format_exc())
             except Exception as e:
-                print(f"WARNING: Uncaught exception for {mint_req}, added to exclusions (RETRY WILL NOT BE ATTEMPTED)")
+                print(f"ERROR: Uncaught exception for {mint_req}, added to exclusions (RETRY WILL NOT BE ATTEMPTED)")
                 print(traceback.format_exc())
                 time.sleep(NftVendingMachine.__ERROR_WAIT)
 
     def validate(self):
         self.mint.validate()
         if self.payment_addr == self.profit_addr:
             raise ValueError(f"Payment address and profit address ({self.payment_addr}) cannot be the same!")
         self.max_rebate = self.__max_rebate_for(self.mint.validated_names)
-        if self.mint.price and self.mint.price < (self.max_rebate + self.mint.dev_fee + Utxo.MIN_UTXO_VALUE):
-            raise ValueError(f"Price of {self.mint.price} with dev fee of {self.mint.dev_fee} could lead to a minUTxO error due to rebates")
+        for price in self.mint.prices:
+            if price.lovelace and price.policy == Balance.LOVELACE_POLICY and price.lovelace < (self.max_rebate + self.mint.dev_fee + Utxo.MIN_UTXO_VALUE):
+                raise ValueError(f"Price of {price.lovelace} lovelace with dev fee of {self.mint.dev_fee} could lead to a minUTxO error due to rebates")
         if not os.path.exists(self.payment_sign_key):
             raise ValueError(f"Payment signing key file '{self.payment_sign_key}' not found on filesystem")
         expected_payment_addr = self.cardano_cli.build_addr(self.payment_sign_key, self.mainnet)
         if not expected_payment_addr == self.payment_addr:
             raise ValueError(f"Could not match {self.payment_addr} to signature at '{self.payment_sign_key}' (expected {expected_payment_addr})")
         self.script_map = {}
         for policy in self.mint.policies:
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/utxo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import re
 
 """
-Simple UTXO object to strengthen the type of CLI-returned strings
+A unit/policy identifier combination representing a Cardano asset balance.
 """
-class Utxo(object):
+class Balance(object):
 
-    MIN_UTXO_VALUE = 1000000
+    LOVELACE_POLICY = 'lovelace'
 
-    class Balance(object):
-        LOVELACE_POLICY = 'lovelace'
+    def __init__(self, lovelace, policy):
+        self.lovelace = lovelace
+        self.policy = policy if policy else Balance.LOVELACE_POLICY
 
-        def __init__(self, lovelace, policy):
-            self.lovelace = lovelace
-            self.policy = policy if policy else Utxo.Balance.LOVELACE_POLICY
+    def __repr__(self):
+        return f"{self.lovelace} {self.policy}"
 
-        def __repr__(self):
-            return f"{self.lovelace} {self.policy}"
+"""
+Simple UTXO object to strengthen the type of CLI-returned strings
+"""
+class Utxo(object):
 
+    MIN_UTXO_VALUE = 1000000
 
     def __init__(self, hash, ix, balances):
         self.hash = hash
         self.ix = ix
         self.balances = balances
 
     def __eq__(self, other):
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.8.0/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.7.3
+Version: 0.8.0
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,16 @@
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
     # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    price = Balance(10000000, Balance.LOVELACE_POLICY)
+    mint = Mint([price], 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -69,15 +70,15 @@
 ### ``main.py``
 There is a sample vending machine script that is included in the ``src/`` directory to show how to invoke the library components.  Use ``-h`` to see detailed help or use a command like below:
 
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
-                [--mint-price <PRICE_LOVELACE> | --free-mint] \
+                (--mint-price <PRICE> <POLICY_ID>)+ \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.3 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.8.0 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -29,81 +29,81 @@
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
 directory') # The Mint object below represents your Mint and specifies price,
-and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
-'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
-path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
-where the UTXO sent to the payment address came from blockfrost_api =
-BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
-cli command (used as a utility without any interaction with the network)
-cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
-NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
-max) so long as the mint period is open nft_vending_machine = NftVendingMachine
-('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
-blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
-the state of already-completed UTXOs to avoid double spending errors and uses a
-do-wait-check loop already_completed = set() while _program_is_running:
-nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
-'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
-``main.py`` There is a sample vending machine script that is included in the
-``src/`` directory to show how to invoke the library components. Use ``-h`` to
-see detailed help or use a command like below: python3 main.py [validate | run]
-\ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
-addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
-project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
-\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
-unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
-dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
-Installation This package is available from [PyPI](https://pypi.org/) and can
-be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
-pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
-` directory there are several scripts that can be used to help operationalize
-the vending machine. #### initialize_whitelist.py This file should be used
-exactly once to initialize an asset-based whitelist for an existing NFT policy
-with *ALL* of the assets that are currently minted. Note that the
-`CONSUMED_DIR` folder is created but left empty so that the vending machine
-(e.g., started with `main.py`) can use it during running. usage:
-initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
-consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
-whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
-NFT policy optional arguments: -h, --help show this help message and exit --
-blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
-retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
-whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
-initializer against mainnet assets (default is False [preprod]) --policy-id
-POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
-initializer against preview assets (default is False [preprod]) --whitelist-dir
-WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
-EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
-each asset on the whitelist #### upload_wl_usage.py This file should be run
-continuously during a whitelist mint to upload changes in the assets used for
-consumption by external parties. Note that if there are any performance issues
-(e.g., IOPS throughput) with the local vending machine filesystem it is
-recommended you not use this file. It is kept separate from the main vending
-machine operation to avoid any synchronization or performance issues as it is
-not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
-upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
-recently used in the vending machine optional arguments: -h, --help show this
-help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
-that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
-used whitelist information if any changes (can be same as --old-wl-file) --
-whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
-gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
-folder where unused whitelist files are stored to be processed by vending
-machine --credentials CREDENTIALS JSON-formatted application-specific
-credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
-whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
-generated from ``pydoc3``-formatted multi-line strings in the source code. A
-mirror of ``master`` is hosted on [Github Pages](https://
+and developer fee in Lovelace (both can be 0) price = Balance(10000000,
+Balance.LOVELACE_POLICY) mint = Mint([price], 1000000, 'addr1_developer', '/
+path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey',
+whitelist) # Blockfrost is used in the code to validate where the UTXO sent to
+the payment address came from blockfrost_api = BlockfrostApi('', mainnet=True)
+# CardanoCli is a wrapper around the cardano-cli command (used as a utility
+without any interaction with the network) cardano_cli = CardanoCli
+(protocol_params='/path/to/protocol.json') # NftVendingMachine vends NFTs and
+needs to be called repeatedly (with a 25-vend max) so long as the mint period
+is open nft_vending_machine = NftVendingMachine('addr_payment', '/path/to/
+payment.skey', 'addr_profit', 25, mint, blockfrost_api, cardano_cli,
+mainnet=True) # The following simple loop carries the state of already-
+completed UTXOs to avoid double spending errors and uses a do-wait-check loop
+already_completed = set() while _program_is_running: nft_vending_machine.vend
+('/path/to/output/dir', 'locking_subdir_name', 'metadata_subdir_name',
+already_completed) time.sleep(WAIT_TIMEOUT) ### ``main.py`` There is a sample
+vending machine script that is included in the ``src/`` directory to show how
+to invoke the library components. Use ``-h`` to see detailed help or use a
+command like below: python3 main.py [validate | run] \ --payment-addr  \ --
+payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-addr  \ (--mint-price
+)+ \ --mint-script /FULL/PATH/TO/policy.script \ --mint-sign-key /FULL/PATH/TO/
+policy.skey \ --blockfrost-project  \ --metadata-dir metadata/ \ --output-dir
+output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist | \ [--
+single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
+whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
+additional] \ [--mainnet] ## Installation This package is available from [PyPI]
+(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
+currently unsupported at this time. pip3 install cardano-nft-vending-machine
+### Scripts In the `scripts/` directory there are several scripts that can be
+used to help operationalize the vending machine. #### initialize_whitelist.py
+This file should be used exactly once to initialize an asset-based whitelist
+for an existing NFT policy with *ALL* of the assets that are currently minted.
+Note that the `CONSUMED_DIR` folder is created but left empty so that the
+vending machine (e.g., started with `main.py`) can use it during running.
+usage: initialize_whitelist.py [-h] asset --blockfrost-project
+BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
+POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
+whitelist for an existing NFT policy optional arguments: -h, --help show this
+help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
+project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
+folder where consumed whitelist files will go after processing (MUST NOT YET
+EXIST) --mainnet Run the initializer against mainnet assets (default is False
+[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
+preview Run the initializer against preview assets (default is False [preprod])
+--whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
+(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
+available for each asset on the whitelist #### upload_wl_usage.py This file
+should be run continuously during a whitelist mint to upload changes in the
+assets used for consumption by external parties. Note that if there are any
+performance issues (e.g., IOPS throughput) with the local vending machine
+filesystem it is recommended you not use this file. It is kept separate from
+the main vending machine operation to avoid any synchronization or performance
+issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
+OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
+CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
+assets have been recently used in the vending machine optional arguments: -h, -
+-help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
+of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
+store the new used whitelist information if any changes (can be same as --old-
+wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.7.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.8.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

