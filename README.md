# 🌾 AgriCast – Blockchain Prediction Market for Agriculture

AgriCast is a blockchain-powered prediction market platform for farmers, traders, and organizations to forecast crop yields, food prices, and climate risks.  
Built on BlockDAG’s fast, scalable EVM-compatible network, AgriCast empowers agricultural communities with transparent, decentralized risk management.

---

## 🌍 Problem

Agriculture faces volatility from climate change, unpredictable markets, and price swings.  
- Farmers suffer from inaccurate forecasts.
- Smallholders lack affordable risk management.
- NGOs and governments need real-time food security intelligence.

---

## 💡 Solution

AgriCast provides a community-driven prediction market:
- **Market Creation:** Farmers/traders create yes/no forecast markets (e.g., “Will maize prices rise next month?”).
- **Staking:** Users stake BDAG tokens on outcomes.
- **Transparent Resolution:** Outcomes are resolved on-chain; winnings are distributed automatically.
- **Advanced Payouts:** Winners receive their stake plus a proportional share of the losing pool.

**New Smart Contract Features:**
- **Claim Winnings:** Winners claim their stake and a share of the opposing pool.  
- **Market Getter:** Retrieve market details (question, pools, outcome) in a single call.  
- **Claim Status:** Check if a user has already claimed winnings for a market.  
- **Ownership Transfer:** Enables future upgrades or community governance.  
- **ETH Fallback:** Contract accepts ETH for flexible funding.

---

## 🛠 Technology Stack

| Component       | Technology |
|-----------------|------------|
| Blockchain      | BlockDAG (EVM-compatible) |
| Smart Contracts | Solidity + Hardhat |
| Frontend        | React + Ethers.js |
| Wallet          | MetaMask |
| Backend (optional) | Node.js / Express |
| Oracles (future) | Weather & crop price APIs |

---

## 📖 How It Works

1. **Create Market:** Define a yes/no agricultural forecast.
2. **Stake Tokens:** Place BDAG tokens on your chosen outcome.
3. **Resolve Outcome:** Verified on-chain (future support for oracles).
4. **Claim Winnings:**  
   - Winners claim their original stake plus a proportional share of the losing pool.  
   - Use the smart contract’s `claimWinnings()` function.
5. **Check Status:**  
   - Use `hasClaimed()` to confirm if winnings have been claimed.
   - Use `getMarket()` to view market details.
6. **Ownership Transfer:**  
   - Contract owner can transfer control for upgrades or decentralization.

---

## AGRICAST ARCHITECTURE

![AgriCast Architecture](assets/agricast-architecture.png)

---

## 📦 Installation & Setup

### Prerequisites
- [Node.js](https://nodejs.org/) v18+
- [MetaMask](https://metamask.io/) with BlockDAG testnet
- [Hardhat](https://hardhat.org/)

### Setup Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/agricast.git
    cd agricast
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Configure environment (`.env`):
    ```env
    PRIVATE_KEY=your_metamask_private_key
    ```
4. Compile contracts:
    ```bash
    npx hardhat compile
    ```
5. Deploy contracts:
    ```bash
    npx hardhat run scripts/deploy.js --network blockdag
    ```

---

## 🚀 Demo Usage

1. Start frontend (React):
    ```bash
    cd frontend
    npm install
    npm start
    ```
2. Connect MetaMask to BlockDAG.
3. Create a market (e.g., “Will Kano receive above-average rainfall?”).
4. Place predictions with BDAG tokens.
5. Resolve market and claim winnings using the smart contract.
6. Use `getMarket()` and `hasClaimed()` methods for market info and claim status.

---

## 🗝 Key Features

- Decentralized, blockchain-secured prediction markets
- Hedging against climate and market volatility
- Transparent and automated payouts
- Advanced payout logic for fair distribution
- Getter and claim status utility functions
- Ownership transfer for future upgrades
- Accepts ETH for flexible funding
- Community-driven forecasting

---

## 💎 Value Proposition

- **Farmers:** Affordable, blockchain-based risk management
- **Traders:** Data-driven agricultural market insights
- **NGOs/Governments:** Real-time food security intelligence
- **Investors:** Access to a $3T+ agriculture sector

---

## 👥 Team Roles

- Smart Contract Development – Solidity, Hardhat, BlockDAG
- Frontend Development – React, Ethers.js, UI/UX
- Backend & Oracles – Weather/price APIs
- Business & Strategy – Partnerships, investor relations

---

## 🏆 Why AgriCast Stands Out

- First blockchain prediction market focused on agriculture
- Addresses global food security
- Built on BlockDAG for speed, low fees, scalability
- Technical innovation with social impact
- Unique crowdsourced agricultural data

---

AgriCast is not only a hackathon project — it's built for real-world impact.
