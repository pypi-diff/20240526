# Comparing `tmp/solathon-1.0.1.tar.gz` & `tmp/solathon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solathon-1.0.1.tar", max compression
+gzip compressed data, was "solathon-1.0.2.tar", max compression
```

## Comparing `solathon-1.0.1.tar` & `solathon-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1050 2024-04-16 13:48:37.758737 solathon-1.0.1/LICENSE
--rw-r--r--   0        0        0     1428 2024-04-16 14:15:10.734716 solathon-1.0.1/README.md
--rw-r--r--   0        0        0     1135 2024-04-30 07:31:50.886527 solathon-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      213 2024-04-30 07:31:33.987671 solathon-1.0.1/solathon/__init__.py
--rw-r--r--   0        0        0    18172 2024-04-16 14:31:07.234418 solathon-1.0.1/solathon/async_client.py
--rw-r--r--   0        0        0    26868 2024-04-30 07:30:12.369363 solathon-1.0.1/solathon/client.py
--rw-r--r--   0        0        0       20 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/__init__.py
--rw-r--r--   0        0        0     3004 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/http.py
--rw-r--r--   0        0        0     5146 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/instructions.py
--rw-r--r--   0        0        0     3040 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/layouts.py
--rw-r--r--   0        0        0     6280 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/message.py
--rw-r--r--   0        0        0     4602 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/account_info.py
--rw-r--r--   0        0        0     6787 2024-04-30 07:30:30.435210 solathon-1.0.1/solathon/core/types/block.py
--rw-r--r--   0        0        0      778 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/cluster_node.py
--rw-r--r--   0        0        0     1426 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/epoch.py
--rw-r--r--   0        0        0     1750 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/inflation.py
--rw-r--r--   0        0        0     2395 2024-04-16 14:28:08.682787 solathon-1.0.1/solathon/keypair.py
--rw-r--r--   0        0        0     1222 2024-04-16 14:21:14.602960 solathon-1.0.1/solathon/publickey.py
--rw-r--r--   0        0        0      286 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/create_qr.py
--rw-r--r--   0        0        0     5128 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/create_transfer.py
--rw-r--r--   0        0        0     3129 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/encode_url.py
--rw-r--r--   0        0        0     3044 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/fetch_transaction.py
--rw-r--r--   0        0        0     1148 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/find_reference.py
--rw-r--r--   0        0        0     2592 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/parse_url.py
--rw-r--r--   0        0        0     3053 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/qr-logo.png
--rw-r--r--   0        0        0      914 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/types.py
--rw-r--r--   0        0        0     3507 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/validate_transfer.py
--rw-r--r--   0        0        0    11293 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/transaction.py
--rw-r--r--   0        0        0     2150 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/utils.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 solathon-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-04-16 13:48:37.758737 solathon-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1428 2024-04-16 14:15:10.734716 solathon-1.0.2/README.md
+-rw-r--r--   0        0        0     1135 2024-05-26 12:37:47.179514 solathon-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-05-26 12:37:50.785489 solathon-1.0.2/solathon/__init__.py
+-rw-r--r--   0        0        0    18172 2024-04-16 14:31:07.234418 solathon-1.0.2/solathon/async_client.py
+-rw-r--r--   0        0        0    26901 2024-05-26 12:37:38.586572 solathon-1.0.2/solathon/client.py
+-rw-r--r--   0        0        0       20 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/__init__.py
+-rw-r--r--   0        0        0     3004 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/http.py
+-rw-r--r--   0        0        0     5146 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/instructions.py
+-rw-r--r--   0        0        0     3040 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/layouts.py
+-rw-r--r--   0        0        0     6280 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/message.py
+-rw-r--r--   0        0        0     4602 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/types/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-16 13:48:37.765736 solathon-1.0.2/solathon/core/types/account_info.py
+-rw-r--r--   0        0        0     8509 2024-05-26 12:37:38.586572 solathon-1.0.2/solathon/core/types/block.py
+-rw-r--r--   0        0        0      969 2024-05-26 12:37:38.586572 solathon-1.0.2/solathon/core/types/cluster_node.py
+-rw-r--r--   0        0        0     1803 2024-05-26 12:37:38.587572 solathon-1.0.2/solathon/core/types/epoch.py
+-rw-r--r--   0        0        0     2448 2024-05-26 12:37:38.587572 solathon-1.0.2/solathon/core/types/inflation.py
+-rw-r--r--   0        0        0     2395 2024-04-16 14:28:08.682787 solathon-1.0.2/solathon/keypair.py
+-rw-r--r--   0        0        0     1222 2024-04-16 14:21:14.602960 solathon-1.0.2/solathon/publickey.py
+-rw-r--r--   0        0        0      286 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/create_qr.py
+-rw-r--r--   0        0        0     5128 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/create_transfer.py
+-rw-r--r--   0        0        0     3129 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/encode_url.py
+-rw-r--r--   0        0        0     3044 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/fetch_transaction.py
+-rw-r--r--   0        0        0     1148 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/find_reference.py
+-rw-r--r--   0        0        0     2592 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/parse_url.py
+-rw-r--r--   0        0        0     3053 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/qr-logo.png
+-rw-r--r--   0        0        0      914 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/types.py
+-rw-r--r--   0        0        0     3507 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/solana_pay/validate_transfer.py
+-rw-r--r--   0        0        0    11293 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/transaction.py
+-rw-r--r--   0        0        0     2150 2024-04-16 13:48:37.766737 solathon-1.0.2/solathon/utils.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 solathon-1.0.2/PKG-INFO
```

### Comparing `solathon-1.0.1/LICENSE` & `solathon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/README.md` & `solathon-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/pyproject.toml` & `solathon-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solathon"
-version = "1.0.1"
+version = "1.0.2"
 description = "High performance, easy to use and feature-rich Solana SDK for Python."
 license = "MIT"
 authors = ["GitBolt"]
 readme = "README.md"
 repository = "https://github.com/GitBolt/solathon"
 keywords = ["solana", "web3", "sdk", "blockchain", "crypto"]
 classifiers = [
```

### Comparing `solathon-1.0.1/solathon/async_client.py` & `solathon-1.0.2/solathon/async_client.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/client.py` & `solathon-1.0.2/solathon/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,17 +98,17 @@
             public_key (PublicKey | str): The public key of the account.
             commitment (Commitment, optional): The level of commitment desired when querying state.
 
         Returns:
             RPCResponse: The response from the RPC endpoint.
         """
         commitment = validate_commitment(commitment) if commitment else None
-        response = self.build_and_send_request(
-            "getAccountInfo", [public_key, commitment]
-        )
+        response = self.build_and_send_request("getAccountInfo", [public_key, {
+            "encoding": "base64"
+        }])
         if self.clean_response:
             if response["value"] == None:
                 raise RPCRequestError(f"Account details not found: {public_key}")
             return AccountInfo(response["value"])
         return response
 
     def get_balance(
@@ -549,17 +549,17 @@
         if self.clean_response:
             return [RecentPerformanceSamples(sample) for sample in response]
         return response
 
     def get_signatures_for_address(
         self,
         acct_address: Text,
-        limit: Optional[Text],
-        before: Optional[Text],
-        until: Optional[Text],
+        limit: Optional[Text] = None,
+        before: Optional[Text] = None,
+        until: Optional[Text] = None,
     ) -> RPCResponse[List[TransactionSignatureType]] | List[TransactionSignature]:
         """
         Returns the signatures for the specified account address.
 
         Args:
             acct_address (str): The account address.
```

### Comparing `solathon-1.0.1/solathon/core/http.py` & `solathon-1.0.2/solathon/core/http.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/instructions.py` & `solathon-1.0.2/solathon/core/instructions.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/layouts.py` & `solathon-1.0.2/solathon/core/layouts.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/message.py` & `solathon-1.0.2/solathon/core/message.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/types/__init__.py` & `solathon-1.0.2/solathon/core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/types/account_info.py` & `solathon-1.0.2/solathon/core/types/account_info.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/core/types/block.py` & `solathon-1.0.2/solathon/core/types/block.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,292 @@
 from solathon.core.message import Message as CoreMessage, MessageHeader
 from typing import Any, List, TypedDict, Union
 
+
 class HeaderType(TypedDict):
     '''
     JSON Response type of Header Information received by RPC
     '''
     numReadonlySignedAccounts: int
     numReadonlyUnsignedAccounts: int
     numRequiredSignatures: int
 
+
 class Header:
 
     def __init__(self, response: HeaderType) -> None:
         self.num_readonly_signed_accounts = response['numReadonlySignedAccounts']
         self.num_readonly_unsigned_accounts = response['numReadonlyUnsignedAccounts']
         self.num_required_signatures = response['numRequiredSignatures']
 
+    def __repr__(self) -> str:
+        return f"Header(num_required_signatures={self.num_required_signatures!r}, num_readonly_signed_accounts={self.num_readonly_signed_accounts!r}, num_readonly_unsigned_accounts={self.num_readonly_unsigned_accounts!r})"
+
+
 class InstructionType(TypedDict):
     '''
     JSON Response type of Instruction Information received by RPC
     '''
     accounts: List[int]
     data: str
     programIdIndex: int
 
+
 class Instruction:
     '''
     Convert Instruction JSON to Class
     '''
+
     def __init__(self, response: InstructionType) -> None:
         self.accounts = response['accounts']
         self.data = response['data']
         self.program_id_index = response['programIdIndex']
 
+    def __repr__(self) -> str:
+        return f"Instruction(num_accounts={len(self.accounts)!r}, program_id_index={self.program_id_index!r})"
+
+
 class MessageType(TypedDict):
     '''
     JSON Response type of Message Information received by RPC
     '''
     accountKeys: List[str]
     header: HeaderType
     instructions: List[InstructionType]
     recentBlockhash: str
 
+
 class Message:
     '''
     Convert Message JSON to Class
     '''
+
     def __init__(self, response: MessageType) -> None:
         self.account_keys = response['accountKeys']
         header = Header(response['header'])
         self.header = MessageHeader(
             num_required_signatures=header.num_required_signatures,
             num_readonly_signed_accounts=header.num_readonly_signed_accounts,
             num_readonly_unsigned_accounts=header.num_readonly_unsigned_accounts
         )
-        self.instructions = [Instruction(instruction) for instruction in response['instructions']]
+        self.instructions = [Instruction(instruction)
+                             for instruction in response['instructions']]
         self.recent_blockhash = response['recentBlockhash']
 
+    def __repr__(self) -> str:
+        return f"Message(header={self.header!r}, num_instructions={len(self.instructions)!r}, recent_blockhash={self.recent_blockhash!r})"
+
 
 class TransactionType(TypedDict):
     '''
     JSON Response type of Transaction Information received by RPC
     '''
     message: MessageType
     signatures: List[str]
 
+
 class Transaction:
     '''
     Convert Transaction JSON to Class
     '''
+
     def __init__(self, response: TransactionType) -> None:
         message = Message(response['message'])
         self.message = CoreMessage(
             header=message.header,
             account_keys=message.account_keys,
             instructions=message.instructions,
             recent_blockhash=message.recent_blockhash
         )
         self.signatures = response['signatures']
 
+    def __repr__(self) -> str:
+        return f"Transaction(message={self.message!r}, signatures={self.signatures!r})"
+
+
 class MetaType(TypedDict):
     '''
     JSON Response type of Meta Information received by RPC
     '''
     err: Union[Any, None]
     fee: int
     innerInstructions: List[Any]
     logMessages: List[Any]
     postBalances: List[int]
     postTokenBalances: List[Any]
     preBalances: List[int]
     preTokenBalances: List[Any]
     rewards: Union[Any, None]
 
+
 class Meta:
     '''
     Convert Meta JSON to Class
     '''
+
     def __init__(self, response: MetaType) -> None:
         self.err = response['err']
         self.fee = response['fee']
         self.inner_instructions = response['innerInstructions']
         self.log_messages = response['logMessages']
         self.post_balances = response['postBalances']
         self.post_token_balances = response['postTokenBalances']
         self.pre_balances = response['preBalances']
         self.pre_token_balances = response['preTokenBalances']
         self.rewards = response['rewards']
 
+    def __repr__(self) -> str:
+        return f"Meta(err={self.err!r}, fee={self.fee!r}, num_inner_instructions={len(self.inner_instructions)!r})"
+
+
 class TransactionElementType(TypedDict):
     '''
     JSON Response type of Transaction Information received by RPC
     '''
     meta: MetaType
     transaction: TransactionType
 
+
 class TransactionElement:
     '''
     Convert Transaction JSON to Class
     '''
+
     def __init__(self, response: TransactionElementType) -> None:
         self.meta = Meta(response['meta'])
         self.transaction = Transaction(response['transaction'])
 
     def __repr__(self) -> str:
         return f"TransactionElement(signatures={self.transaction.signatures!r})"
 
-    
+
 class BlockType(TypedDict):
     '''
     JSON Response type of Block Information received by RPC
     '''
     blockHeight: int
     blockTime: None
     blockhash: str
     parentSlot: int
     previousBlockhash: str
     transactions: List[TransactionElementType]
 
+
 class Block:
     '''
     Convert Block JSON to Class
     '''
 
     def __init__(self, response: BlockType) -> None:
         self.block_height = response['block_height']
         self.block_time = response['block_time']
         self.blockhash = response['blockhash']
         self.parent_slot = response['parent_slot']
         self.previous_blockhash = response['previous_blockhash']
-        self.transactions = [TransactionElement(transaction) for transaction in response['transactions']]
+        self.transactions = [TransactionElement(
+            transaction) for transaction in response['transactions']]
+
+    def __repr__(self) -> str:
+        return f"Block(block_height={self.block_height!r}, block_time={self.block_time!r}, blockhash={self.blockhash!r},num_transactions={len(self.transactions)!r})"
+
 
 class RangeType(TypedDict):
     '''
     JSON Response type of Range Information received by RPC
     '''
     firstSlot: int
     lastSlot: int
 
+
 class Range:
     '''
     Convert Range JSON to Class
     '''
+
     def __init__(self, response: RangeType) -> None:
         self.first_slot = response['firstSlot']
         self.last_slot = response['lastSlot']
 
+    def __repr__(self) -> str:
+        return f"Range(first_slot={self.first_slot!r}, last_slot={self.last_slot!r})"
+
+
 class BlockProductionType(TypedDict):
     '''
     JSON Response type of Block Production Information received by RPC
     '''
     byIdentity: dict[str, Any]
     range: RangeType
 
+
 class BlockProduction:
     '''
     Convert Block Production JSON to Class
     '''
+
     def __init__(self, response: BlockProductionType) -> None:
         self.by_identity = response['byIdentity']
         self.range = Range(response['range'])
 
+    def __repr__(self) -> str:
+        return f"BlockProduction(by_identity={self.by_identity!r}, range={self.range!r})"
+
+
 class BlockCommitmentType(TypedDict):
     '''
     JSON Response type of Block Commitment Information received by RPC
     '''
     commitment: List[int]
     totalStake: int
 
+
 class BlockCommitment:
     '''
     Convert Block Commitment JSON to Class
     '''
-    
+
     def __init__(self, response: BlockCommitmentType) -> None:
         self.commitment = response['commitment']
         self.total_stake = response['totalStake']
 
+    def __repr__(self) -> str:
+        return f"BlockCommitment(commitment={self.commitment!r}, total_stake={self.total_stake!r})"
+
+
 class FeeCalculatorType(TypedDict):
     '''
     JSON Response type of Fee Calculator Information received by RPC
     '''
     lamportsPerSignature: int
 
-class BlockHashType(TypedDict):
-    '''
-    JSON Response type of Block Hash Information received by RPC
-    '''
-    blockhash: str
-    feeCalculator: FeeCalculatorType
 
 class FeeCalculator:
     '''
     Convert Fee Calculator JSON to Class
     '''
 
     def __init__(self, response: FeeCalculatorType) -> None:
         self.lamports_per_signature = response['lamportsPerSignature']
 
+    def __repr__(self) -> str:
+        return f"FeeCalculator(lamports_per_signature={self.lamports_per_signature!r})"
+
+
+class BlockHashType(TypedDict):
+    '''
+    JSON Response type of Block Hash Information received by RPC
+    '''
+    blockhash: str
+    feeCalculator: FeeCalculatorType
+
+
 class BlockHash:
     '''
     Convert Block Hash JSON to Class
     '''
+
     def __init__(self, response: BlockHashType) -> None:
         self.blockhash = response['blockhash']
-        self.fee_calculator = FeeCalculator(response['feeCalculator'])
+        self.fee_calculator = FeeCalculator(response['feeCalculator'])
+
+    def __repr__(self) -> str:
+        return f"BlockHash(blockhash={self.blockhash!r}, fee_calculator={self.fee_calculator!r})"
```

### Comparing `solathon-1.0.1/solathon/core/types/cluster_node.py` & `solathon-1.0.2/solathon/core/types/cluster_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import Optional, TypedDict
 
+
 class ClusterNodeType(TypedDict):
     '''
     JSON Response type of Cluster Node Information received by RPC
     '''
     pubkey: str
     gossip: Optional[str]
     tpu: Optional[str]
     rpc: Optional[str]
     version: Optional[str]
     featureSet: Optional[int]
     shredVersion: Optional[int]
 
+
 class ClusterNode:
     '''
     Convert Cluster Node Information JSON to Class
     '''
+
     def __init__(self, response: ClusterNodeType) -> None:
         self.pubkey = response['pubkey']
         self.gossip = response['gossip']
         self.tpu = response['tpu']
         self.rpc = response['rpc']
         self.version = response['version']
         self.feature_set = response['featureSet']
-        self.shred_version = response['shredVersion']
+        self.shred_version = response['shredVersion']
+
+    def __repr__(self) -> str:
+        return f"ClusterNode(pubkey={self.pubkey!r}, tpu={self.tpu!r}, rpc={self.rpc!r}, version={self.version!r},, shred_version={self.shred_version!r})"
```

### Comparing `solathon-1.0.1/solathon/core/types/epoch.py` & `solathon-1.0.2/solathon/core/types/epoch.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,40 +8,50 @@
     epoch: int
     absoluteSlot: int
     blockHeight: int
     slotIndex: int
     slotsInEpoch: int
     transactionCount: Optional[int]
 
+
 class Epoch:
     '''
     Convert Epoch Information JSON to Class
     '''
+
     def __init__(self, response: EpochType) -> None:
         self.epoch = response['epoch']
         self.absolute_slot = response['absoluteSlot']
         self.block_height = response['blockHeight']
         self.slot_index = response['slotIndex']
         self.slots_in_epoch = response['slotsInEpoch']
         self.transaction_count = response['transactionCount']
 
+    def __repr__(self) -> str:
+        return f"Epoch(epoch={self.epoch!r}, absolute_slot={self.absolute_slot!r}, block_height={self.block_height!r}, slot_index={self.slot_index!r})"
+
+
 class EpochScheduleType(TypedDict):
     '''
     JSON Response type of Epoch Schedule Information received by RPC
     '''
     slotsPerEpoch: int
     leaderScheduleSlotOffset: int
     warmup: bool
     firstNormalEpoch: int
     firstNormalSlot: int
 
+
 class EpochSchedule:
     '''
     Convert Epoch Schedule Information JSON to Class
     '''
+
     def __init__(self, response: EpochScheduleType) -> None:
         self.slots_per_epoch = response['slotsPerEpoch']
         self.leader_schedule_slot_offset = response['leaderScheduleSlotOffset']
         self.warmup = response['warmup']
         self.first_normal_epoch = response['firstNormalEpoch']
         self.first_normal_slot = response['firstNormalSlot']
-        
+
+    def __repr__(self) -> str:
+        return f"EpochSchedule(slots_per_epoch={self.slots_per_epoch!r}, leader_schedule_slot_offset={self.leader_schedule_slot_offset!r}, warmup={self.warmup!r})"
```

### Comparing `solathon-1.0.1/solathon/core/types/inflation.py` & `solathon-1.0.2/solathon/core/types/inflation.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,55 +7,74 @@
     '''
     foundation: float
     foundationTerm: int
     initial: float
     taper: float
     terminal: float
 
+
 class InflationGovernor:
     '''
     Convert Inflation Governer Information JSON to Class
     '''
+
     def __init__(self, response: InflationGovernorType) -> None:
         self.foundation = response['foundation']
         self.foundation_term = response['foundationTerm']
         self.initial = response['initial']
         self.taper = response['taper']
         self.terminal = response['terminal']
 
+    def __repr__(self) -> str:
+        return f"InflationGovernor(foundation={self.foundation!r}, foundation_term={self.foundation_term!r}, initial={self.initial!r}, taper={self.taper!r}, terminal={self.terminal!r})"
+
+
 class InflationRateType(TypedDict):
     '''
     JSON Response type of Inflation Rate Information received by RPC
     '''
     epoch: int
     foundation: float
     validator: float
     total: float
 
+
 class InflationRate:
 
     def __init__(self, response: InflationRateType) -> None:
         self.epoch = response['epoch']
         self.foundation = response['foundation']
         self.validator = response['validator']
         self.total = response['total']
 
+    def __repr__(self) -> str:
+        return f"InflationRate(epoch={self.epoch!r}, foundation={self.foundation!r}, validator={self.validator!r}, total={self.total!r})"
+
+
 class InflationRewardType(TypedDict):
     '''
     JSON Response type of Inflation Reward Information received by RPC
     '''
     epoch: int
     effectiveSlot: int
     amount: int
     postBalance: int
     commission: Optional[int]
 
+    def __repr__(self) -> str:
+        return f"InflationReward(epoch={self.epoch!r}, effectiveSlot={self.effectiveSlot!r}, amount={self.amount!r})"
+
+
 class InflationReward:
     '''
     Convert Inflation Reward Information JSON to Class
     '''
+
     def __init__(self, response: InflationRewardType) -> None:
         self.epoch = response['epoch']
         self.effective_slot = response['effectiveSlot']
         self.amount = response['amount']
         self.post_balance = response['postBalance']
-        self.commission = response['commission']
+        self.commission = response['commission']
+
+    def __repr__(self) -> str:
+        return f"InflationReward(epoch={self.epoch!r}, effective_slot={self.effective_slot!r}, amount={self.amount!r})"
```

### Comparing `solathon-1.0.1/solathon/keypair.py` & `solathon-1.0.2/solathon/keypair.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/publickey.py` & `solathon-1.0.2/solathon/publickey.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/create_qr.py` & `solathon-1.0.2/solathon/solana_pay/create_qr.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/create_transfer.py` & `solathon-1.0.2/solathon/solana_pay/create_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/encode_url.py` & `solathon-1.0.2/solathon/solana_pay/encode_url.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/fetch_transaction.py` & `solathon-1.0.2/solathon/solana_pay/fetch_transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/find_reference.py` & `solathon-1.0.2/solathon/solana_pay/find_reference.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/parse_url.py` & `solathon-1.0.2/solathon/solana_pay/parse_url.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/qr-logo.png` & `solathon-1.0.2/solathon/solana_pay/qr-logo.png`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/types.py` & `solathon-1.0.2/solathon/solana_pay/types.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/solana_pay/validate_transfer.py` & `solathon-1.0.2/solathon/solana_pay/validate_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/transaction.py` & `solathon-1.0.2/solathon/transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/solathon/utils.py` & `solathon-1.0.2/solathon/utils.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.1/PKG-INFO` & `solathon-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solathon
-Version: 1.0.1
+Version: 1.0.2
 Summary: High performance, easy to use and feature-rich Solana SDK for Python.
 Home-page: https://github.com/GitBolt/solathon
 License: MIT
 Keywords: solana,web3,sdk,blockchain,crypto
 Author: GitBolt
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solathon Version: 1.0.1 Summary: High performance,
+Metadata-Version: 2.1 Name: solathon Version: 1.0.2 Summary: High performance,
 easy to use and feature-rich Solana SDK for Python. Home-page: https://
 github.com/GitBolt/solathon License: MIT Keywords:
 solana,web3,sdk,blockchain,crypto Author: GitBolt Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

