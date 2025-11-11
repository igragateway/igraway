# IgraWay Contracts (Hyperlane  Based)

This repository contains the full set of **Hyperlane smart contracts**, preserved in their entirety,
and serves as the foundational base for **IgraWay’s cross-chain arbitration and validator research**.

---

## 📦 Source & License

**Upstream source:**  
[https://github.com/hyperlane-xyz/hyperlane-monorepo](https://github.com/hyperlane-xyz/hyperlane-monorepo)

**Original authors:**  
[Hyperlane Labs (Abacus Works)](https://hyperlane.xyz)

**License:**  
Dual-licensed under **MIT OR Apache-2.0**, exactly as the upstream repository.  
All SPDX license identifiers remain intact.

> © Hyperlane Labs — retained and reused in compliance with MIT OR Apache-2.0 license terms.

---

## 🧱 Repository Description

This repository keeps the full set of Hyperlane contract modules intact, preserving their original structure and content.
The core cross-chain and mailbox logic remains unmodified and cryptographically consistent with the upstream implementation.


| Directory | Description |
|------------|-------------|
| `avs/` | Active Verification Service modules (experimental validator off-chain service interface) |
| `client/` | Core message router abstractions (`Router.sol`, `GasRouter.sol`, `TokenRouter.sol`) |
| `hooks/` | Post-dispatch hooks and metadata definitions |
| `interfaces/` | Public interfaces for routers, ISMs, and hooks |
| `isms/` | The current implementation uses Multisig ISM (Interchain Security Module),which verifies cross-chain messages through m-of-n validator signatures on-chain. |
| `libs/` | Shared utility libraries (Message, TypeCasts, MerkleLib, etc.) |
| `mailbox/` | Core message dispatch and processing contracts |
| `middleware/` | Middleware extension layer for optional message handling logic |
| `mock/` | Mock and testing contracts used in simulations |
| `token/` | Hyperlane token bridges and HypERC20 series contracts |
| `upgrade/` | Proxy upgrade framework for upgradable deployments |



---

## 🧩 Purpose

IgraWay uses this repository as a **research and development base** for:
- Building arbitration-augmented ISMs (Interchain Security Modules);
- Experimenting with validator coordination mechanisms;
- Integrating flexible governance and cross-chain message filtering;
- Developing prototype cross-chain asset and message validation frameworks.