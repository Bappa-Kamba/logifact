# 🚚 LogiFact

**Decentralized Invoice Factoring on the Stellar Network.**

LogiFact is a liquidity protocol that bridges the cash-flow gap for SME logistics. By tokenizing unpaid invoices using **Soroban Smart Contracts**, we allow drivers to receive immediate USDC advances from a global pool of investors.

[![Ecosystem: Stellar](https://img.shields.io/badge/Ecosystem-Stellar-blue)](https://stellar.org)
[![Contracts: Soroban/Rust](https://img.shields.io/badge/Contracts-Soroban%2FRust-orange)](https://soroban.stellar.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## 🏗️ Tech Stack

- **Frontend:** Next.js 15 (App Router), Tailwind CSS, Shadcn/UI
- **Backend:** NestJS (Node.js Enterprise Framework)
- **Database:** PostgreSQL + TypeORM (Strict Schema Enforcement)
- **Blockchain:** Soroban (Rust SDK)
- **Identity:** Stellar Wallet (Freighter/Albedo) + Stellar Passkeys

## 🚀 Quick Start

### Prerequisites
- [Rust & Cargo](https://rustup.rs/)
- [Stellar CLI](https://developers.stellar.org/docs/build/smart-contracts/getting-started/setup#install-the-stellar-cli)
- Node.js v20+ & pnpm

### Setup
1. **Clone the Repo:**
   ```bash
   git clone [https://github.com/Bappa-Kamba/LogiFact.git](https://github.com/Bappa-Kamba/LogiFact.git)
   cd LogiFact
   ```
2. **Smart Contracts:**
   ```bash
   cd contracts
   stellar contract build
   cargo test
   ```
3. **Backend:**
   ```bash
   cd server
   yarn install
   yarn run start:dev
   ```
4. **Frontend:**
   ```bash
   cd client
   yarn install
   yarn run dev
