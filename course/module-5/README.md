# Module 5: Core Ingredients

A detailed examination of the building blocks: encryption schemes, UTXO models, transaction structures, network designs, and blockchain specifications.

🔗 **[Interactive Blockchain Demo →](https://andersbrownworth.com/blockchain/)**

---

## Key Concepts

**UTXO vs. Account models** — Two fundamentally different ways of tracking ownership on a blockchain. UTXO (Unspent Transaction Output) tracks individual coins; Account model tracks balances. Bitcoin, Quai, Cardano, Ergo, and others use UTXO variants.

**Transaction structure** — Inputs, outputs, signatures, and metadata. How value moves through the system. The structure of a transaction determines what the blockchain can express.

**Network design** — Peer-to-peer gossip protocols, block propagation, mempool management, and fee markets. The engineering that connects individual nodes into a coherent network.

**Blockchain specifications** — Block size, block time, difficulty adjustment period, emission schedule, signature scheme, address format. The parameter choices that define a specific chain's character.

## Connection to Thermoeconomics

The UTXO model is particularly important for thermoeconomics because each UTXO is a discrete, verifiable unit of value created by a specific block — traceable back to the mining event that created it. This creates a direct link between the thermodynamic work of mining and the economic objects in circulation.

## Further Resources

- [Proof of Work](../foundations/proof-of-work/README.md)
- [Quai Network — Dual Currency](../quai/qi-quai-dual-currency.md)
