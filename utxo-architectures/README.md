# The UTXO Model

The **Unspent Transaction Output (UTXO)** model is Bitcoin's foundational data structure for tracking ownership. Instead of maintaining account balances (like a bank), UTXO-based blockchains track individual "coins" — discrete outputs of previous transactions that haven't yet been spent.

Since Bitcoin, a rich variety of UTXO variants have emerged. The **UTXO Alliance** brings these projects together to advance the model. This section is a visual and technical guide to every major UTXO flavor, adapted from the Alliance's official [UTXO Model Flavors Handbook](https://github.com/UTXO-Alliance/handbooks).

---

## How UTXO Works

A transaction *consumes* one or more existing UTXOs (inputs) and *creates* one or more new UTXOs (outputs). The sum of inputs must equal or exceed the sum of outputs; any excess goes to the miner as a fee.

This is fundamentally different from the account model (used by Ethereum), where transactions modify balances in a global state. The UTXO model provides natural parallelism (transactions that consume different UTXOs are independent), enhanced privacy (each output is a distinct "coin"), and straightforward auditability (the entire supply is the set of all unspent outputs).

## The Flavors

Each chain in this section takes the basic UTXO concept and extends it:

| Chain | UTXO Variant | Key Innovation |
|---|---|---|
| **Bitcoin** | Classic UTXO | The original — Script-based locking |
| **Cardano** | Extended UTXO (eUTXO) | Datum + redeemer for smart contracts |
| **Ergo** | ErgoScript UTXO | Registers for rich data, sigma protocols |
| **Nervos** | Cell Model | Generalized UTXO with arbitrary state |
| **Alephium** | Sharded UTXO | Stateful UTXO across sharded groups |
| **Quai Network** | Hierarchical UTXO | Multi-chain UTXO with merged mining |
| **DigiByte** | Multi-Algorithm UTXO | Five PoW algorithms for decentralization |
| **Hathor** | DAG-Based UTXO | UTXO on a directed acyclic graph |

## Visual Guide

Architecture diagrams for each chain are available on the [thermoeconomics.info](https://thermoeconomics.info) landing page — click any chain name in the UTXO section to see its diagram from the Alliance handbook.

---

*Content adapted from the [UTXO Alliance Handbook v2.2](https://github.com/UTXO-Alliance/handbooks) · [utxoa.org](https://www.utxoa.org/)*
