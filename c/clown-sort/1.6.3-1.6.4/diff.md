# Comparing `tmp/clown_sort-1.6.3.tar.gz` & `tmp/clown_sort-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.6.3.tar", max compression
+gzip compressed data, was "clown_sort-1.6.4.tar", max compression
```

## Comparing `clown_sort-1.6.3.tar` & `clown_sort-1.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2961 2023-06-02 21:09:30.892923 clown_sort-1.6.3/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.3/LICENSE
--rw-r--r--   0        0        0     8659 2023-05-28 21:20:43.213283 clown_sort-1.6.3/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.3/clown_sort/__init__.py
--rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.3/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.6.3/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.3/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.3/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11399 2023-06-02 21:07:03.088714 clown_sort-1.6.3/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.6.3/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    10043 2023-06-02 07:17:50.864003 clown_sort-1.6.3/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.3/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.3/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.3/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.3/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.3/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.3/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.3/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-06-02 21:09:30.898473 clown_sort-1.6.3/pyproject.toml
--rw-r--r--   0        0        0    10081 1970-01-01 00:00:00.000000 clown_sort-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3134 2023-06-02 22:23:44.794224 clown_sort-1.6.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.4/LICENSE
+-rw-r--r--   0        0        0     8659 2023-05-28 21:20:43.213283 clown_sort-1.6.4/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.4/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.4/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.6.4/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.4/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     2756 2023-06-02 21:34:09.379034 clown_sort-1.6.4/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.6.4/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.6.4/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    10270 2023-06-02 22:21:00.287460 clown_sort-1.6.4/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.4/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.4/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.4/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.6.4/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.4/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.4/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.4/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-06-02 22:23:44.801788 clown_sort-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10081 1970-01-01 00:00:00.000000 clown_sort-1.6.4/PKG-INFO
```

### Comparing `clown_sort-1.6.3/CHANGELOG.md` & `clown_sort-1.6.4/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # NEXT RELEASE
 
+### 1.6.4
+* Crop very long PDF pages when previewing in manual select window
+* Fix regexes for wallet addresses
+* Gracefully handle failures in file timestamp copying call
+
 ### 1.6.3
 * Fix bug with manual folder selection
 * Refactor `move_to_processed_dir()` and call from `sort_selector.py`.
 
 ### 1.6.2
 * Add `--force` and `[gui,pdf]` to the `pipx` installation instructions
```

### Comparing `clown_sort-1.6.3/LICENSE` & `clown_sort-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/README.md` & `clown_sort-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/__init__.py` & `clown_sort-1.6.4/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/config.py` & `clown_sort-1.6.4/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/filename_extractor.py` & `clown_sort-1.6.4/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/files/image_file.py` & `clown_sort-1.6.4/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/files/pdf_file.py` & `clown_sort-1.6.4/clown_sort/files/pdf_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Wrapper for PDF files.
 """
+import logging
 from sys import exit
 from typing import Optional
 
 from pypdf import PdfReader
 from pypdf.errors import DependencyError
 
 from clown_sort.config import check_for_pymupdf, log_optional_module_warning
 from clown_sort.util.rich_helper import WARNING, console
 from clown_sort.util.logging import log
 from clown_sort.files.sortable_file import SortableFile
 
+MAX_DISPLAY_HEIGHT = 600
+SCALE_FACTOR = 0.4
+
 
 class PdfFile(SortableFile):
     is_presentable_in_popup = None
 
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
@@ -39,17 +43,28 @@
         self.text_extraction_attempted = True
         return self._extracted_text
 
     def thumbnail_bytes(self) -> bytes:
         """Return bytes for a thumbnail."""
         import fitz
         doc = fitz.open(self.file_path)
-        zoom_matrix = fitz.Matrix(fitz.Identity).prescale(0.4, 0.4)
-        page = doc[0].get_pixmap(matrix=zoom_matrix, alpha=False)
-        return page.tobytes()
+        zoom_matrix = fitz.Matrix(fitz.Identity).prescale(SCALE_FACTOR, SCALE_FACTOR)
+        page = doc[0]
+        bottom_right = page.rect.br
+        page_height = bottom_right[1]
+        page_width = bottom_right[0]
+
+        # Check for PDFs with very long pages and crop them
+        if SCALE_FACTOR * page_height > MAX_DISPLAY_HEIGHT:
+            logging.debug(f"PDF page is {page_height} pixels high so cropping...")
+            clip = fitz.Rect((0, 0), (MAX_DISPLAY_HEIGHT / SCALE_FACTOR, page_width))
+        else:
+            clip = fitz.Rect((0, 0), bottom_right)
+
+        return page.get_pixmap(matrix=zoom_matrix, clip= clip, alpha=False).tobytes()
 
     def _can_be_presented_in_popup(self) -> bool:
         if type(self).is_presentable_in_popup is None:
             type(self).is_presentable_in_popup = check_for_pymupdf()
 
         if not type(self).is_presentable_in_popup:
             console.line()
```

### Comparing `clown_sort-1.6.3/clown_sort/files/sortable_file.py` & `clown_sort-1.6.4/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/sort_selector.py` & `clown_sort-1.6.4/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.6.4/clown_sort/sorting_rules/crypto.csv`

 * *Files 5% similar despite different names*

```diff
@@ -24,41 +24,44 @@
 Bitzlato,Bitzlato
 Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b
 Blockchain8,Blockchain8|tom[-_\s.]*emmer|ritchie[-_\s.]*torres|repritchie|Warren[-_\s.]*Davidson|Byron[-_\s.]*Donalds|Ted[-_\s.]*Budd|Josh[-_\s.]*Gotheimer|Jake[-_\s.]*Auchincloss|Darren[-_\s.]*Soto|ro[-_\s.]*khanna|KMSmithDC|Kristin[-_\s.]*Smith\b|Warren[-_\s.]*Davidson
 Blockchain Capital,Blockchain[-_\s.]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi|Zac[-_\s.]*Prince|Brian[-_\s.]*Oliver
 Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s.]*Ape|yuga[-_\s.]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang
+Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b
 Broettes,Nicole[-_\s.]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s.]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie[-_\s.]*Wood|\bARK(F|G|K|[-_\s.]*Innovation|[-_\s.]*Invest)|\bIZRL
-Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot
+Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot|\bnuke[-_\s.]*gold(stein)?
 China,fentanyl|chin(a|ese)
 Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
+ConsenSys,ConsenSys
 Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b
 Cumberland,cumberland
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
 CUBI,\bCUBI\b|Customers[-_\s.]*Ban(k|corp)
 Custodia,custodia\b|caitlin[-_\s.]*long
 dalle,craiyon|midjourney|\bdall[-_\s.]*e\b
 DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b
 DeFi,\bdefi\b|decentralized[-_\s.]*finance
 Dragonfly Capital,Dragonfly[-_\s.]*Capital
 DWF,DWF|Andrey[-_\s.]*Grachev|\bgrachev\b
+Evolve Bank,getevolved|\bevolve[-_\s.]*bank\b
 Effective Altruism,\bE\.?A\.?\b|effective[-_\s.]*altruism
 El Salvador,El[-_\s.]*Salvador|Bukele|Max[-_\s.]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
+Evertas,\bEvertas\b|Ryan[-_\s.]*Lackey
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker
@@ -90,14 +93,15 @@
 Marathon,\$MARA|marathon
 Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s.]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners
 Mario Nawfal,mario[-_\s.]*nawfal
 Messari,Ryan[-_\s.]*Selkis|twobitidiot|messari|@robustus|Dan[-_\s.]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s.]*Stewart|\bHayner\b
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s.]*(Bank|Commercial)|Mission[-_\s.]*Gateway|Aryeh[-_\s.]*Realty
+Multichain,Multichain\b
 Founders Bank,Michael[-_\s.]*Bianchi|Founders[-_\s.]*Bank
 Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s.]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s.]*seven|kin[-_\s.]*ming[-_\s.]*je|william[-_\s.]*je\b|\bHaoyun\b|\bLi[-_\s.]*You\b
 Miners,bitcoin[-_\s.]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s.]*Scientific|Iris[-_\s.]*Energy|Blockstream
 Moonpay,\bmoonpay
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s.]*bot
 Near Protocol,NEAR[-_\s.]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s.]*Rettig
@@ -109,48 +113,50 @@
 OpenSea,OpenSea
 PAG,\bpag\b|Weijian[-_\s.]*Shan
 Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s.]*(Youssef|Savant)|Artur[-_\s.]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s.]*Network
+Politics,\bted[-_\s.]*cruz
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s.]*Cotten|0xsifu\b|michael[-_\s.]*patryn|wonderland|daniele[-_\s.]*sesta\b
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
-SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
+SEC,\bSEC(\b|Gov)|\bGensler|CFTC|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s.]*Bank|Signet|Scott[-_\s.]*Shay\b|(Joseph|Joe)[-_\s.]*DePaolo|\bKushner\b
 Silicon Valley Bank,si?vb|Silicon[-_\s.]*Valley[-_\s.]*Bank
 Silk Road,Silk[-_\s.]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan[-_\s.]*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s.]*Rettig
 Skrill,\bskrill
 Solana,Solana|Serum
 Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
+Synapse,Synapse(fi|labs|protocol)?\b
 TerraLuna,luna\b|do[-_\s.]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s.]*Foundation\b
 Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Grubacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners
 Tornado Cash,tornado[-_\s.]*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
 Voyager,voyager
 Wallet Addresses BCH,bitcoincash:q.*\b
-Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0–9]{25,39}\b
-Wallet Addresses Cardano,\baddr1[a-z0–9]+\b
-Wallet Addresses Cosmos,\bcosmos[a-zA-Z0–9_.-]{10,}\b
-Wallet Addresses Dash,\bX[1–9A-HJ-NP-Za-km-z]{33}
-Wallet Addresses Doge,\bD[a-zA-Z0–9_.-]{33}
-Wallet Addresses Ethereum,\b0x[a-fA-F0–9]{40}
-Wallet Addresses Monero,\b[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
-Wallet Addresses Polkadot,\b1[0–9a-zA-Z]{47}
-Wallet Addresses Ripple,\br[0–9a-zA-Z]{33}
-Wallet Addresses Stellar,\bG[0–9A-Z]{40,60}\b
+Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39}\b
+Wallet Addresses Cardano,\baddr1[a-z0-9]+\b
+Wallet Addresses Cosmos,\bcosmos[a-zA-Z0-9_.-]{10,}\b
+Wallet Addresses Dash,\bX[1-9A-HJ-NP-Za-km-z]{33}
+Wallet Addresses Doge,\bD[a-zA-Z0-9_.-]{33}
+Wallet Addresses Ethereum,0x[a-fA-F0-9]{40}
+Wallet Addresses Monero,\b[48][0-9AB][1-9A-HJ-NP-Za-km-z]{93}
+Wallet Addresses Polkadot,\b1[0-9a-zA-Z]{47}
+Wallet Addresses Ripple,\br[0-9a-zA-Z]{33}
+Wallet Addresses Stellar,\bG[0-9A-Z]{40,60}\b
 Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s.]*ivanov|boris[-_\s.]*titov|[$#]waves\b
 Wintermute,wintermute|\bbebop\b
 Wirecard,wirecard|\bmarsalek\b|\bBafin\b
 Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `clown_sort-1.6.3/clown_sort/util/argument_parser.py` & `clown_sort-1.6.4/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/util/constants.py` & `clown_sort-1.6.4/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/util/filesystem_helper.py` & `clown_sort-1.6.4/clown_sort/util/filesystem_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from datetime import datetime
 from os import path
 from pathlib import Path
 from typing import List, Optional, Union
 
 from filedate.Utils import Copy
 from filedate import File
+from rich.console import Console
+from rich.text import Text
 
 from clown_sort.util.constants import MAC_SCREENSHOT_REGEX
 
 PDF_EXTENSION = '.pdf'
 IMAGE_FILE_EXTENSIONS = [f".{ext}" for ext in 'tiff jpg jpeg png heic'.split()]
 MOVIE_FILE_EXTENSIONS = ['.mov', '.flv', '.avi']
 SORTABLE_FILE_EXTENSIONS = IMAGE_FILE_EXTENSIONS + [PDF_EXTENSION, '.mov']
@@ -41,15 +43,22 @@
 def timestamp_for_filename() -> str:
     """Returns a string showing current time in a file name friendly format."""
     return datetime.now().strftime("%Y-%m-%dT%H.%M.%S")
 
 
 def copy_file_creation_time(source_file: Path, destination_file: Path) -> None:
     """Copy the file creation timestamp from source_file to destination_file."""
-    Copy(str(source_file), str(destination_file)).all()
+    try:
+        Copy(str(source_file), str(destination_file)).all()
+    except FileNotFoundError:
+        msg = Text("WARNING! couldn't copy file creation timestamp because file does not exist for ")
+        msg.append(f"'{destination_file}'!")
+        Console().print(msg, style='bright_yellow')
+        return
+
     _set_permissions(destination_file)
 
 
 def set_timestamp_based_on_screenshot_filename(file_path: Path) -> None:
     file_timestamp = extract_timestamp_from_filename(str(file_path))
     print(f"Parsed {file_timestamp} from '{file_path.name}'")
     print("    last modified: %s" % time.ctime(os.path.getmtime(file_path)))
```

### Comparing `clown_sort-1.6.3/clown_sort/util/rich_helper.py` & `clown_sort-1.6.4/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/clown_sort/util/string_helper.py` & `clown_sort-1.6.4/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.3/pyproject.toml` & `clown_sort-1.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.6.3"
+version = "1.6.4"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.6.3/PKG-INFO` & `clown_sort-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.6.3
+Version: 1.6.4
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

