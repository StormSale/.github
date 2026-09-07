<div align="center">

<img src="profile/assets/stormsale-hero.svg" alt="StormSale Protocol on Stellar & Soroban" width="100%" />

<br/>

[![Stellar Network](https://img.shields.io/badge/Stellar-Soroban%20Smart%20Contracts-0ea5e9?style=for-the-badge&logo=stellar&logoColor=white)](https://stellar.org)
[![Network: Testnet](https://img.shields.io/badge/Network-Testnet%20Active-6366f1?style=for-the-badge)](https://stellar.expert/explorer/testnet)
[![License: MIT](https://img.shields.io/badge/License-MIT-10b981.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Freighter Wallet](https://img.shields.io/badge/Wallet-Freighter%20v6+-a855f7?style=for-the-badge)](https://www.freighter.app/)
[![SCF](https://img.shields.io/badge/Ecosystem-Stellar%20Community%20Fund-38bdf8?style=for-the-badge)](https://communityfund.stellar.org)

<p align="center">
  <a href="https://github.com/StormSale/Storm-Contract"><b>⚡ Soroban Contracts</b></a> &nbsp;•&nbsp;
  <a href="https://github.com/StormSale/StormSale"><b>💻 Frontend dApp</b></a> &nbsp;•&nbsp;
  <a href="https://github.com/StormSale/StormSale-backend"><b>⚙️ Backend API</b></a> &nbsp;•&nbsp;
  <a href="#-architecture"><b>🏛️ Architecture</b></a> &nbsp;•&nbsp;
  <a href="#-contributing"><b>🤝 Contributing</b></a>
</p>

---

</div>

## 🌐 Protocol Mission

**StormSale** is a decentralized, non-custodial affiliate marketing and merchant escrow clearing protocol built natively for the **Stellar Network** using **Soroban Rust Smart Contracts**.

In traditional Web2 affiliate marketing, merchants and affiliates lose up to **30% in platform fees**, wait **30–60 days for commission payouts**, and suffer from opaque attribution and chargeback fraud. 

StormSale eliminates centralized middlemen by orchestrating deterministic smart-contract escrows, sub-second finality, and cryptographic commission settlement.

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

The protocol is organized into three production-grade, decoupled repositories:

| Repository | Scope | Core Technologies | Health Status |
| :--- | :--- | :--- | :---: |
| [**`Storm-Contract`**](https://github.com/StormSale/Storm-Contract) | Core Soroban Smart Contracts, campaign escrows, affiliate registry, instant XLM payouts | Rust, Soroban SDK v22, WASM, Dalek Crypto | ![Tests](https://img.shields.io/badge/cargo%20test-passing-10b981) |
| [**`StormSale`**](https://github.com/StormSale/StormSale) | Next-Gen Web3 dApp, role dashboards (Advertiser, Affiliate, Auditor), Freighter wallet connection | React 18, Vite, TypeScript, TailwindCSS, `@stellar/freighter-api` | ![Build](https://img.shields.io/badge/vite%20build-passing-0ea5e9) |
| [**`StormSale-backend`**](https://github.com/StormSale/StormSale-backend) | High-speed indexing service, Stellar RFC 4648 Base32 public key validation API | Node.js, Express, TypeScript, Prisma ORM, PostgreSQL | ![Tests](https://img.shields.io/badge/npm%20test-passing-6366f1) |

---

## ⚡ Why Stellar & Soroban?

<table>
  <tr>
    <td width="33%" align="center">
      <br/>
      <h3>⏱️ &lt; 1s Finality</h3>
      <p>Instant commission settlements. No 30-day payout holding periods.</p>
    </td>
    <td width="33%" align="center">
      <br/>
      <h3>💎 $0.00001 Fees</h3>
      <p>Near-zero transaction costs allow micro-affiliate payouts and high-frequency conversion logging.</p>
    </td>
    <td width="33%" align="center">
      <br/>
      <h3>🔒 Non-Custodial</h3>
      <p>Funds remain locked in deterministic Soroban escrow contracts. Zero custodial counterparty risk.</p>
    </td>
  </tr>
</table>

---

## 🚀 Key Technical Highlights

- **Native Stellar Architecture**: Zero legacy EVM baggage. Integrated with `@stellar/stellar-sdk` and `@stellar/freighter-api`.
- **NIST-Level Data Confidentiality**: Proprietary conversion data is encrypted off-chain using AES-GCM/ECIES before on-chain hash attestation.
- **Strict RFC 4648 Base32 Validation**: Rigorous runtime validation on all Stellar account addresses (`G...`) and Soroban contract IDs (`C...`).
- **Complete Contributor Governance**: 100% GitHub Community Standards score across all repositories (MIT License, Contributor Covenant v2.1, and issue/PR templates).

---

## 🤝 Community & Governance

We welcome developers, merchants, and affiliates to build on top of StormSale!

- 📜 **Contributing Guidelines**: [CONTRIBUTING.md](https://github.com/StormSale/StormSale/blob/main/CONTRIBUTING.md)
- 🛡️ **Vulnerability Disclosure**: [SECURITY.md](https://github.com/StormSale/StormSale/blob/main/SECURITY.md)
- 🕊️ **Code of Conduct**: [CODE_OF_CONDUCT.md](https://github.com/StormSale/StormSale/blob/main/CODE_OF_CONDUCT.md)
- 💬 **Direct Contact**: `security@stormsale.xyz`

<br/>

<div align="center">
  <sub>Built with ❤️ for the Stellar Ecosystem • © 2026 StormSale Protocol</sub>
</div>
