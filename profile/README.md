<div align="center">

# ⚡ StormSale Protocol

**Storm the market. Break the prices.**  
*The Next-Generation Trustless Affiliate & Merchant Escrow Protocol on Stellar & Soroban.*

[![Stellar](https://img.shields.io/badge/Stellar-Soroban%20Smart%20Contracts-black?style=for-the-badge&logo=stellar&logoColor=white)](https://stellar.org)
[![Network](https://img.shields.io/badge/Network-Testnet%20Active-00b4d8?style=for-the-badge)](https://stellar.expert/explorer/testnet)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Community](https://img.shields.io/badge/Community-SCF%20Ready-6366f1?style=for-the-badge)](https://communityfund.stellar.org)

<p align="center">
  <a href="https://github.com/StormSale/Storm-Contract"><b>Soroban Contracts</b></a> •
  <a href="https://github.com/StormSale/StormSale"><b>Frontend dApp</b></a> •
  <a href="https://github.com/StormSale/StormSale-backend"><b>Backend API</b></a> •
  <a href="#-architecture"><b>Architecture</b></a> •
  <a href="#-contributing"><b>Contributing</b></a>
</p>

---

</div>

## 🌐 Overview

**StormSale** is a decentralized, non-custodial affiliate marketing and commission clearing protocol engineered natively for the **Stellar Network** using **Soroban Rust Smart Contracts**.

Traditional affiliate networks suffer from high intermediary fees (15–30%), opaque attribution, multi-week payout delays, and chargeback fraud. StormSale replaces centralized middlemen with **deterministic Soroban escrows**, cryptographic sale validation, and **instant, sub-cent XLM commission payouts**.

```
┌─────────────────┐       Create Campaign & Deposit Escrow       ┌────────────────────────┐
│   Advertiser    │ ───────────────────────────────────────────> │  Soroban Smart Contract │
└─────────────────┘                                              │  (Escrow & Commission) │
                                                                 └───────────┬────────────┘
┌─────────────────┐       Encrypted Tracking / Proof of Sale                 │ Instant XLM
│    Affiliate    │ <────────────────────────────────────────────────────────┘ Distribution
└─────────────────┘
```

---

## 🏛️ Ecosystem Architecture & Repositories

The StormSale organization maintains three decoupled, production-grade repositories:

| Repository | Focus | Tech Stack | Status |
| :--- | :--- | :--- | :---: |
| [**`Storm-Contract`**](https://github.com/StormSale/Storm-Contract) | Core Soroban Smart Contracts, campaign escrows, commission logic, and clearance engine | Rust, Soroban SDK v22, WASM | ![Tests](https://img.shields.io/badge/tests-passing-brightgreen) |
| [**`StormSale`**](https://github.com/StormSale/StormSale) | Modern Web3 dApp, role-based dashboards (Advertiser, Affiliate, Auditor), Freighter wallet integration | React 18, Vite, TypeScript, TailwindCSS, `@stellar/freighter-api` | ![Build](https://img.shields.io/badge/build-passing-brightgreen) |
| [**`StormSale-backend`**](https://github.com/StormSale/StormSale-backend) | High-performance off-chain indexer, metadata storage, and Stellar RFC 4648 Base32 validation API | Node.js, Express, TypeScript, Prisma ORM, PostgreSQL | ![Tests](https://img.shields.io/badge/tests-passing-brightgreen) |

---

## 🚀 Key Technical Highlights

- **Native Stellar & Soroban Architecture**: Zero legacy EVM dependencies. Pure `@stellar/stellar-sdk` and `@stellar/freighter-api` integration.
- **Sub-Second Finality & Micro-Cent Costs**: Leverages Stellar's consensus mechanism for real-time affiliate payout settlements.
- **Cryptographic Attribution**: End-to-end encrypted payload verification for private sale attribution without exposing proprietary customer data.
- **Strict RFC 4648 Base32 Validation**: Rigorous runtime validation on all Stellar account addresses (`G...`) and Soroban contract IDs (`C...`).
- **Comprehensive Contributor Governance**: 100% GitHub Community Standards compliance across all repositories, including MIT licensing, Contributor Covenant v2.1, and standardized PR/issue triage templates.

---

## 📊 Quick Links & Resources

- 📜 **Smart Contract Audit & Standard**: [`repository_standard_audit.md`](https://github.com/StormSale/Storm-Contract/blob/main/README.md)
- 🤝 **Grant Dossier**: Prepared for the [Stellar Community Fund (SCF)](https://communityfund.stellar.org)
- 🛡️ **Security Policy**: Read our [Vulnerability Disclosure Policy](https://github.com/StormSale/StormSale/blob/main/SECURITY.md)
- 💬 **Get in Touch**: Security inquiries at `security@stormsale.xyz`

---

## 🤝 Contributing

We welcome open-source contributions from the Stellar and Web3 developer communities! 
Please review our [Contributing Guidelines](https://github.com/StormSale/StormSale/blob/main/CONTRIBUTING.md) and [Code of Conduct](https://github.com/StormSale/StormSale/blob/main/CODE_OF_CONDUCT.md) before submitting pull requests.

<div align="center">
  <sub>Built with ❤️ for the Stellar Ecosystem • © 2026 StormSale Protocol</sub>
</div>
