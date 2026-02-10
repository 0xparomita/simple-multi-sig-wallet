# Simple Multi-Sig Wallet

This repository provides a high-quality, secure Multi-Signature (Multi-Sig) wallet. It is designed for teams or DAOs that require multiple individuals to authorize a transaction before it is executed on the blockchain.

## How it Works
1. **Submission:** Any owner can submit a transaction (destination, value, and data).
2. **Confirmation:** Other owners review and "confirm" the transaction.
3. **Execution:** Once the required threshold (e.g., 2 out of 3) is met, any owner can trigger the execution.



## Security Features
- **Immutable Owners:** The list of owners and the required threshold are set at deployment to prevent takeover.
- **Reentrancy Protection:** Follows the checks-effects-interactions pattern to ensure funds are safe.
- **Data Transparency:** All proposed transactions and their confirmation status are visible on-chain.

## Tech Stack
- **Solidity ^0.8.20**
- **Foundry** (Testing & Deployment)
