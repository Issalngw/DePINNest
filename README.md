# DePINNest

# Decentralized EV Charging Network on Solana

> Powering Africa’s Electric Future, One Charge at a Time.


## Overview

**DePINNest** is a decentralized EV charging network built on **Solana**, connecting IoT-powered charging stations with on-chain smart contracts, NFT Smart Wallets, and Solana Pay.  
Each charging node operates as a tokenized infrastructure asset — trackable, ownable, and reward-generating — enabling transparent, instant, and community-driven electric vehicle charging.

## The Problem

- EV charging infrastructure in Africa is centralized, expensive, and unevenly distributed.  
- Small operators and communities lack tools for transparent revenue tracking or on-chain payments.  
- Web3 users can’t easily participate in or invest in real-world clean energy systems.
- 

## The Solution

**DePINNest** introduces a *DePIN (Decentralized Physical Infrastructure Network)* model for EV charging — powered by **Solana’s speed, scalability, and efficiency**.  
Each charging node becomes an on-chain asset using IoT integration and Solana smart contracts to manage:

- Real-time energy tracking  
- Instant payments (USDC/SOL via Solana Pay)  
- NFT Smart Wallets for ownership and rewards  
- Cross-chain coordination via Axelar GMP  

**Components:**
- **IoT meters:** Measure and push real-time energy usage to the Solana blockchain.  
- **Solana Smart Contracts:** Verify transactions, manage energy credits, and split payments.  
- **NFT Smart Wallets:** Represent ownership of physical charging nodes, storing performance and payout data.  
- **Axelar Integration:** Enables data and reward synchronization across other chains or regions.  
- **Solana Pay:** Processes instant microtransactions between users and operators.

## Core Features

✅ **IoT-Enabled Real-Time Tracking** — Every watt used is logged on Solana for transparency.  
✅ **Instant Payments** — Microtransactions settled via Solana Pay in USDC or SOL.  
✅ **NFT Ownership Layer** — Charging stations represented as NFT Smart Wallets.  
✅ **Revenue Splitting** — On-chain automated distribution to community operators, investors, and maintenance teams.  
✅ **Cross-Chain Interoperability** — Powered by Axelar GMP for future expansion.  
✅ **Security First** — Escrow-based contracts and planned audit with Halborn/OpenZeppelin.

## Tech Stack

- **Blockchain:** Solana  
- **Payments:** Solana Pay  
- **Interoperability:** Axelar GMP  
- **Frontend:** React / Next.js  
- **Smart Contracts:** Anchor Framework  
- **IoT Devices:** ESP32/Arduino + REST API to Solana RPC  
- **Database (optional):** IPFS or Supabase for off-chain metadata  
- **NFTs:** Metaplex for asset tokenization  

## Roadmap

### **Q4 2025**
- Deploy 10 IoT-enabled EV charging nodes (pilot)
- Launch NFT Smart Wallet dashboard
- Integrate Solana Pay for instant settlements

### **Q1 2026**
- Smart contract audit (Halborn or OpenZeppelin)
- Expand to 5 new communities
- Implement Axelar GMP for multi-region data sync

### **Q2 2026**
- Scale to 3 new African countries
- Launch Charge-to-Earn system
- Begin DePINNest Africa Initiative

## Deployment & Usage

This section outlines how to set up and interact with the **DePINNest** prototype using the Solana and Anchor frameworks.  
*(Note: The commands below are placeholders and can be updated with actual paths and program IDs once the smart contracts are ready.)*

### Prerequisites
Before deployment, ensure you have the following installed:
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli) (v1.18 or higher)
- [Anchor Framework](https://book.anchor-lang.com/chapter_2/installation.html)
- Node.js (v18 or higher)
- npm or yarn

### Setup Instructions

```bash
# Clone the repository
git clone https://github.com/<yourusername>/DePINNest.git

# Navigate into the project directory
cd DePINNest

# Install dependencies
npm install
```

### Build and Deploy Smart Contracts

```bash
# Build smart contracts using Anchor
anchor build

# Deploy program to Solana Devnet
anchor deploy

# (Optional) View your deployed program ID
solana address -k target/deploy/depinnest-keypair.json
```

### Run the Frontend Locally

```bash
# Start the Next.js frontend in development mode
npm run dev
```

### Interacting with the Prototype

1. Connect your Solana wallet (e.g., Phantom) to the Devnet network.  
2. Load test tokens using:  
   ```bash
   solana airdrop 2
   ```  
3. Use the dashboard to simulate EV charging, view real-time IoT data, and send payments using Solana Pay.  
4. Monitor on-chain logs and events via Solana Explorer.  

### Notes
- Replace placeholder program IDs and RPC URLs once your on-chain contract is finalized.  
- Always test on **Devnet** before deploying to **Mainnet**.  
- Consider integrating **Axelar GMP** in later versions for multi-chain data sync.
- 
