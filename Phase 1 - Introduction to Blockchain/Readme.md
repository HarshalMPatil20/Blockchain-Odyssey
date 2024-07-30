# Phase 1: Introduction to Blockchain

## Module 1: What is Blockchain?

### Introduction to Blockchain

#### 1. Definition and Overview 
__Blockchain Technology Defined:__\
Blockchain technology is a decentralized digital ledger that records transactions across a network of computers. Each transaction, or "block," is securely linked to the previous one, forming a "chain." This structure ensures that the information stored in the blockchain is immutable and transparent.

__Core Components:__

- Blocks: Each block contains a list of transactions, a timestamp, and a reference to the previous block's hash.
- Chain: Blocks are connected in a sequential manner, forming a chain of blocks.
- Nodes: These are individual computers that participate in the blockchain network. Each node maintains a copy of the blockchain ledger.
- Consensus Mechanism: A protocol used by nodes to agree on the validity of transactions and blocks. Common mechanisms include Proof of Work (PoW) and Proof of Stake (PoS).

```sql
+---------------------+      +---------------------+     +---------------------+     
|     Node A          |      |     Node B          |     |     Node C          |
| +-----------------+ |      | +-----------------+ |     | +-----------------+ |
| |  Blockchain     | |      | |  Blockchain     | |     | |  Blockchain     | |
| |  Ledger         | |      | |  Ledger         | |     | |  Ledger         | |
| | +-------------+ | |      | | +-------------+ | |     | | +-------------+ | |
| | | Block 1     | | |      | | | Block 1     | | |     | | | Block 1     | | |
| | |-------------| | |      | | |-------------| | |     | | |-------------| | |
| | | Transactions| | |      | | | Transactions| | |     | | | Transactions| | |
| | | Timestamp   | | |      | | | Timestamp   | | |     | | | Timestamp   | | |
| | | Prev. Hash  | | |      | | | Prev. Hash  | | |     | | | Prev. Hash  | | |
| | +-------------+ | |      | | +-------------+ | |     | | +-------------+ | |
| | +-------------+ | |      | | +-------------+ | |     | | +-------------+ | |
| | | Block 2     | | |      | | | Block 2     | | |     | | | Block 2     | | |
| | |-------------| | |      | | |-------------| | |     | | |-------------| | |
| | | Transactions| | |      | | | Transactions| | |     | | | Transactions| | |
| | | Timestamp   | | |      | | | Timestamp   | | |     | | | Timestamp   | | |
| | | Prev. Hash  | | |      | | | Prev. Hash  | | |     | | | Prev. Hash  | | |
| | +-------------+ | |      | | +-------------+ | |     | | +-------------+ | |
| +-----------------+ |      | +-----------------+ |     | +-----------------+ |
+---------------------+      +---------------------+     +---------------------+
                                 
                                                                    |
                                                                    |
                                                                    v
                                                         +---------------------+
                                                         | Consensus Mechanism |
                                                         | (e.g., PoW, PoS)    |
                                                         +---------------------+

```

__How Blockchain Works:__

1. Transaction Initiation: A user initiates a transaction, which is then broadcasted to the network.
2. Transaction Verification: Nodes validate the transaction using consensus mechanisms.
3. Block Creation: Verified transactions are grouped into a block.
4. Block Addition: The new block is added to the blockchain, and the ledger is updated across all nodes.
5. Immutability: Once added, the block cannot be altered, ensuring data integrity.

```sql
                   +---------------------------+
                   | 1. Transaction Initiation |
                   +---------------------------+
                                 |
                                 v
                   +-----------------------------+
                   | 2. Transaction Verification |
                   | - Broadcast to Network      |
                   | - Nodes Validate            |
                   | - Consensus Mechanism       |
                   +-----------------------------+
                                 |
                                 v
                   +---------------------------+
                   | 3. Block Creation         |
                   | - Group Transactions      |
                   | - Create New Block        |
                   +---------------------------+
                                 |
                                 v
                   +---------------------------+
                   | 4. Block Addition         |
                   | - Add Block to Blockchain |
                   | - Update Ledger Across    |
                   |   All Nodes               |
                   +---------------------------+
                                 |
                                 v
                   +---------------------------+
                   | 5. Immutability           |
                   | - Block Cannot Be Altered |
                   | - Ensures Data Integrity  |
                   +---------------------------+
```