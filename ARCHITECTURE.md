# LogiFact Architecture

## The "Triangle of Trust" Flow
1. **The Driver** uploads an NRS-certified e-invoice via the **Next.js** frontend.
2. **NestJS** parses the XML, validates the IRN, and caches the metadata in **PostgreSQL**.
3. **The Driver** signs a transaction to the **Soroban Smart Contract**, which mints an `InvoiceToken`.
4. **The Investor** sends USDC to the contract's escrow.
5. **The Contract** releases the advance to the Driver, minus the **0.5% flat platform fee**.

## Folder Structure
- `/contracts`: Rust-based Soroban contracts.
- `/server`: NestJS backend and TypeORM entities.
- `/client`: Next.js frontend and Shadcn/UI components.
- `/common`: Shared Typescript interfaces and constants.
