# Victor Chang

Senior Full-Stack Engineer building real-time, fintech, and Web3 systems.

`Go` · `TypeScript` · `React` · `Node.js` · `PostgreSQL` · `AWS`

I design and build production-oriented systems involving real-time market data, asset accounting, distributed workflows, and blockchain infrastructure. Focused on backend correctness, deterministic execution, and clean, responsive interfaces.

---

## Featured Projects

### [Matchbook](https://github.com/outsider987/matchbook)

Cryptocurrency exchange infrastructure built from scratch.

`Go` · `React 19` · `TypeScript` · `WebSocket` · `PostgreSQL` · `Solidity` · `Docker`

* **High-Performance Matching Engine:** Single-writer in-memory order book implementing price-time priority (~430k matches/s, ~2.3µs order-to-trade latency benchmarked on single symbol).
* **Exchange Semantics & Accounting:** Fixed-point integer money (`int64` scaled by 1e8, 128-bit intermediate math, zero floats), available/locked balance ledger with per-fill price-improvement refunds, and Binance-compatible REST/WebSocket endpoints.
* **On-Chain Asset Gateway:** EVM deposit/withdrawal pipeline with HD wallet derivation, confirmation-depth block scanning that makes shallow reorgs structurally invisible, and nonce-managed crash-safe broadcasting.
* **Post-FTX Proof of Reserves:** Per-asset Merkle sum tree committed on-chain each epoch; users verify cryptographic balance inclusion via their own RPC against verified Solidity contracts.
* **Trading Terminal & Market Maker:** Full React 19 trading interface with real-time candles, cumulative depth ladders, tape, and a bot mirroring live Binance price feeds and taker flow.

[View Repository →](https://github.com/outsider987/matchbook)

---

### [HoldBook — Hedera RWA Secondary Market](https://github.com/outsider987/hedera-rwa-secondary-market)

ATS-first secondary market prototype for tokenized equity on Hedera Testnet.

`TypeScript` · `React` · `Go` · `PostgreSQL` · `Solidity` · `Hedera SDK`

* **Signed Order Matching:** Off-chain Go matching engine with EIP-712 signature verification, price-time priority book, and durable PostgreSQL state recovery.
* **Atomic Settlement (DvP):** Custom Solidity escrow contract executing ATS Holds and HBAR payment atomically in a single transaction (Delivery vs. Payment).
* **Verifiable Compliance Lifecycle:** Verifiable Credential verification, on-chain KYC gating, and guarded hold execution/release.
* **Audit & Evidence:** Prototype on Hedera Testnet with verifiable on-chain settlement receipts, structured architecture documentation, and recorded execution evidence.

[Live Demo →](https://outsider987.github.io/hedera-rwa-secondary-market/) · [View Repository →](https://github.com/outsider987/hedera-rwa-secondary-market)

---

### [Portfolio](https://github.com/outsider987/victor-site)

Personal engineering portfolio and systems case study index.

`Next.js 16` · `React 19` · `TypeScript` · `Motion`

* Case study index documenting engineering decisions across real-time operations, healthcare workflows, and Web3 transaction UX.
* Fully typed Next.js App Router implementation with bilingual support (EN/ZH), Swiss typography, and static export deployed via GitHub Actions.

[Live Portfolio →](https://outsider987.github.io/victor-site/) · [View Repository →](https://github.com/outsider987/victor-site)

---

## Open Source

### [SUSE Harvester / Rancher UI](https://github.com/harvester/harvester-ui-extension)

Contributing upstream bug fixes to the Harvester UI Extension (open-source hyperconverged infrastructure management based on Kubernetes, KubeVirt, and Longhorn):

* [PR #1146](https://github.com/harvester/harvester-ui-extension/pull/1146) — `fix: bind bulk VM disk deletion checkbox to checkAll` *(Open / Under review)*
  Resolved an issue where bulk VM deletion incorrectly inherited global deletion flags, ensuring disk retention preferences are preserved across batch operations.
* [PR #1138](https://github.com/harvester/harvester-ui-extension/pull/1138) — `fix: require names for cloud configuration templates` *(Open / Under review)*
  Enforced mandatory name validation when creating or cloning Cloud Configuration Templates to prevent invalid unnamed resource creation.

---

## Engineering Focus

* **Real-Time & Event-Driven Systems:** In-memory matching engines, LMAX-style single-writer goroutines, low-latency WebSocket push feeds, and event journaling.
* **Fintech & Asset Accounting:** Fixed-point integer money, balance ledgers with available/locked accounting, per-fill price-improvement refunds, and trade journals.
* **Backend Architecture & APIs:** High-throughput REST and WebSocket services in Go and Node.js/TypeScript, PostgreSQL schema design, and Docker containerization.
* **Web3 & Blockchain Infrastructure:** On-chain Proof of Reserves (Merkle sum trees), reorg-safe transaction scanning, nonce-managed hot wallets, and atomic DvP smart contracts.

---

## Contact

* **Location:** Taiwan (UTC+8) · Open to remote & international engineering roles
* **GitHub:** [@outsider987](https://github.com/outsider987)
* **Portfolio:** [outsider987.github.io/victor-site](https://outsider987.github.io/victor-site/)
* **LinkedIn:** [linkedin.com/in/yao-hsien-chang](https://linkedin.com/in/yao-hsien-chang)
* **Email:** [t790219520@gmail.com](mailto:t790219520@gmail.com)
