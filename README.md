# Onchain DAO

A decentralized autonomous organization (DAO) built with Solidity, Foundry, and Next.js. This project enables users to propose, vote, and execute on-chain governance actions.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Technologies Used](#technologies-used)

---

## Overview
This project implements a fully functional DAO on Ethereum with the following key capabilities:
- Users can **create proposals**.
- Members can **vote** on proposals.
- Proposals are executed on-chain after passing.

The frontend (built with Next.js) interacts seamlessly with the smart contracts deployed on Ethereum using libraries like **Wagmi** and **ethers.js**.

---

## Features
- **Proposal Creation:** Users can propose actions to be voted on.
- **Voting System:** Members vote on proposals using on-chain mechanisms.
- **Execution:** Approved proposals trigger smart contract logic.
- **NFT-based Access Control:** Only holders of specific NFTs can vote or create proposals.

---

## Project Structure
```
./onchain-dao
|-- foundry/                # Smart contracts (Solidity)
|   |-- src/                # Contract source code
|   |-- test/               # Tests for smart contracts
|-- frontend/               # Frontend built with Next.js
|   |-- src/                # Next.js components and pages
|   |-- public/             # Static assets
|-- constants/              # ABI and contract addresses
|-- README.md               # Project documentation
|-- package.json            # Dependencies
|-- hardhat.config.js       # Hardhat configuration (if used)
```

---

## Installation
Follow these steps to set up the project locally:

### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v16 or later)
- [Foundry](https://book.getfoundry.sh/) for Solidity development
- [Git](https://git-scm.com/)

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/onchain-dao.git
   cd onchain-dao
   ```

2. **Install Frontend Dependencies:**
   ```bash
   cd frontend
   npm install
   ```

3. **Install Foundry:**
   Follow the Foundry installation guide [here](https://book.getfoundry.sh/getting-started/installation).

4. **Compile Smart Contracts:**
   ```bash
   cd foundry
   forge build
   ```

5. **Run Local Development Server:**
   Navigate to the `frontend` directory and start the Next.js server:
   ```bash
   cd frontend
   npm run dev
   ```
   Your frontend will be live at `http://localhost:3000`.

---

## Usage
### 1. Deploy Contracts
To deploy your smart contracts using Foundry:
```bash
forge script script/Deploy.s.sol --rpc-url <YOUR_RPC_URL> --private-key <YOUR_PRIVATE_KEY>
```

### 2. Interact with Contracts
Update the `constants` folder with:
- **Deployed Contract ABI**
- **Contract Addresses**

### 3. Run the Frontend
Start the Next.js development server:
```bash
npm run dev
```

---

## Technologies Used
- **Solidity**: Smart contract programming
- **Foundry**: Development framework for smart contracts
- **Next.js**: React framework for frontend development
- **Wagmi**: React hooks for Ethereum
- **Ethers.js**: Ethereum interaction library

---

## Contact
For questions or feedback, checkout https://learnweb3.io

---
**Happy Building! 🚀**
