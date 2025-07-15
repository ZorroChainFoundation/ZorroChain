

# 🧠 ZorroChain V2 — Modular Codex Overview

ZorroChain is a post-quantum sovereign consensus framework with layered entropy, decentralized vaults, and governance by civic quorum.  
Each folder in this repo is a standalone module, defined and sealed per Epoch under Codex rules.

---

## 📦 Repository Layout Overview

Modules are versioned and linked through `/docs/codex_structure.md`.  
Codex builds are auto-generated via Doxygen (`doxygen Doxyfile`).

---

### ⚙️ Core Protocol Modules
- `core/` — Execution engine: epoch state, tx logic, entropy ops  
- `vault/` — Civic-secure identity vaults, Shamir, snapshot, zk-hardened recovery  
- `wallet/` — Sovereign shell: biometrics, staking, sync, proposal tooling  
- `genesis/` — Epoch 0 init logic: roles, permissions, DAO start curve  
- `sync/` — Epoch replay, ZK sync guards, state convergence

---

### 🧠 Governance & Mutation
- `dao/` — Proposal lifecycle, allocation, validator score tracking  
- `evolve/` — Simulation engine, mutation watchdog, proposal modeling  
- `genome/` — Civic fork lineage, trait divergence, zk DAG ancestry  
- `egraal/` — Reflexive zk mutation governor (Epoch 100+)  
- `audit/` — Civic deviation tracking, rollback logging, ethics scoring  
- `autonomy/` — Entropy-energy survival scoring, uptime fallback
- `zorroculture/` — Digital cultural anchoring; non-financial artifact minting and memory registry

---

### 🌐 Network, Mesh & Resilience
- `mirror/` — Fallback replay and snapshot mirror topology  
- `network/` — Sync stack: LORA, QR, NFC, GNSS, offline media  
- `satlink/` — Orbital uplink relay + GNSS sync fallback  
- `reentry/` — Stateless rejoin logic and fork ancestry check  
- `civicmesh/` — Offline civic quorum injection: QR, LoRa, analog ballots
- `sentinelwave/` — Proximity anomaly detection via LoRa echo-mapping; security presence heuristic

---

### 📊 Economic Feeds & Pegs
- `pegfeed/` — Entropy-weighted oracle aggregator: sync cost, index price  
- `pegfeed-api/` — API gateway for peg consensus + regional feed access  
- `gnosis/` — Forecast entropy collapse, civic quorum fracture detection

---

### 🔗 L2 Coordination & Execution
- `contracts/` — Proposal execution logic, trigger hooks, vault binding  
- `bridge/` — L2↔L2 sync coordination, ZK boundary proof, state mirror

---

### 🛰️ Public Interfaces & Documentation
- `public/` — Stateless civic endpoint layer (QR voting, proposal readout)  
- `docs/` — Codex spec, amendment processes, whitepapers, index  

---

### 🛠 Utilities
- `tools/` — Flash booters, QR keygen, mesh relay tests, entropy probes  

---

## 🚀 Epoch 0 — Bootstrapping Sequence

To initialize a sovereign Genesis set, use the following:

### ✅ Minimum Required
- `core/`  
- `vault/`  
- `wallet/`  
- `genesis/`  
- `sync/`

### 🔄 Recommended
- `dao/`  
- `pegfeed/`  
- `public/`

### 🧪 Optional / Post-Boot
- `contracts/`, `bridge/`, `tools/`, `mirror/`, `satlink/`  
- `audit/`, `evolve/`, `autonomy/`, `genome/`, `civicmesh/`

---

## 🔑 Core Design Principles

- 🧬 **Modular Isolation** — Every module sealed, testable, entropy-signed  
- 🔐 **Entropy Anchoring** — Chain state driven by civic randomness and vault proof  
- 🧠 **Governance = Runtime** — DAO defines mutation paths per Epoch  
- 🔁 **Stateless Reentry** — Any node can rejoin after blackout or exile  
- 🛰️ **Offline Durability** — Mesh sync, QR, NFC fallback, GNSS redundancy  
- ⚖️ **ZK Trust Layer** — zkID signatures and zero-knowledge runtime guards

---

## 🛠 Developer Quickstart

```bash
# Rebuild Codex Docs (HTML)
cd docs/codex
doxygen Doxyfile
start docs_output/index.html
