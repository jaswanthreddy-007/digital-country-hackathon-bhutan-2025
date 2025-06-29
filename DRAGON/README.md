# Dragon Coin 🐉₿

![Dragon Coin Logo](./assets/dragon-coin-logo.png)

**Dragon Coin backed by Bhutan's BTC Reserves**

A revolutionary cryptocurrency project that leverages Bhutan's Bitcoin reserves to create a stable digital currency.

## 🌐 Live Deployment
- **Deployed Token Contract**: [0x432091fca44F8f6e2b20773cb1cA3c4d5a8ED4E8](https://sepolia.etherscan.io/token/0x432091fca44F8f6e2b20773cb1cA3c4d5a8ED4E8) (Sepolia Testnet)
- **Main Application UI**: [https://druk-bitcoin-reserve.lovable.app/](https://druk-bitcoin-reserve.lovable.app/)
- **Dashboard endpoint**: [https://druk-bitcoin-reserve.lovable.app/dashboard](https://druk-bitcoin-reserve.lovable.app/dashboard)

## 🎯 Core Features

- **BTC-Backed Stability**: Dragon Coins are backed by Bhutan's Bitcoin reserves
- **Algorithmic Liquidity**: Dragon Coins are capable of integrating uniswap concentrated liquidity mechanism
- **Dashboard Analytics**: Comprehensive dashboard for monitoring system metrics
- **Real-time Price Feeds**: Live data integration through Chainlink oracles
- **Multi-signature Security**: Enhanced security through multi-sig wallet implementation
- **Reserve Transparency**: Real-time reserve ratio monitoring



## 🚀 Quick Start

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- Git

### Running the Application

#### 1. Clone the Repository
```bash
git clone <repository-url>
cd "DRAGON"
```

#### 2. Setup Local Server for Live Data Feed

Navigate to the server directory:
```bash
cd server
```

**Option A: Using Deploy Script**
```bash
cd scripts
# Run the deploy script (check the deploy script for specific instructions)
```

**Option B: Using Environment Variables**
1. Create a `.env` file in the server directory
2. Add the deployed contract address:
```env
CONTRACT_ADDRESS=0x432091fca44F8f6e2b20773cb1cA3c4d5a8ED4E8
# Add other required environment variables
```

#### 3. Start the API Server

Navigate to the API folder and install dependencies:
```bash
cd api
npm install
npm start
```

🎉 **You're ready!** The local server will now feed live data to the UI, and you can see live update feeds in the deployed application.

## 📁 Project Structure

```
├── README.md
├── server/
│   ├── api/                    # API server for live data feeds
│   ├── contracts/              # Smart contracts
│   ├── scripts/                # Deployment and utility scripts
│   ├── BTC_TEST_NET_WALLET/    # Bitcoin testnet integration
│   └── HEDGE_LORDS_SERVER/     # Optional hedge lords service
├── UI/                         # Frontend applications
│   ├── src/                    # Main UI source code
│   └── HEDGE_LORDS_UI/         # Optional hedge lords UI
└── ...
```

## 🔧 Smart Contracts

### Main Contracts
- **DragonCoin.sol**: Main token contract
- **DragonCoinRates.sol**: Exchange rate management
- **VaultManager.sol**: BTC reserve management
- **BTCDepositVerifier.sol**: Bitcoin deposit verification
- **ChainlinkBTCOracle.sol**: Price oracle integration

### Deployed Contract
- **Network**: Sepolia Testnet
- **Address**: `0x432091fca44F8f6e2b20773cb1cA3c4d5a8ED4E8`
- **Explorer**: [View on Etherscan](https://sepolia.etherscan.io/token/0x432091fca44F8f6e2b20773cb1cA3c4d5a8ED4E8)

## 📊 API Endpoints

The local API server provides the following endpoints for live data:
- Transaction feeds
- Balance information
- Contract status
- Exchange rates
- Reserve ratios

## 🛠️ Development

### Smart Contract Development
```bash
cd server
npm install
npx hardhat compile
npx hardhat test
```

### Frontend Development
```bash
cd UI
npm install
npm run dev
```

## 🔐 Security Features

- Multi-signature wallet implementation
- Chainlink price oracle integration
- BTC deposit verification system
- Collateral ratio monitoring
- Real-time reserve auditing

## 📈 Monitoring & Analytics

The dashboard provides real-time monitoring of:
- Total Dragon Coin supply
- BTC reserve levels
- Collateral ratios
- Transaction volumes
- Price stability metrics


## 🔧 Optional: Hedge Lords Setup

The Hedge Lords UI and service setup is **optional** but provides additional functionality for advanced users who want to explore additional stabilizing features.

### Hedge Lords Server Setup

1. Navigate to the Hedge Lords server directory:
```bash
cd server/HEDGE_LORDS_SERVER
```

2. Install Python dependencies:
```bash
pip install -r requirements.txt
```

3. Run the simulator:
```bash
# On Windows
run_simulator.bat

# Or manually
python -m services.simulator.main
```

### Hedge Lords UI Setup

1. Navigate to the Hedge Lords UI directory:
```bash
cd UI/HEDGE_LORDS_UI
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

**Note**: The Hedge Lords components provide additional trading and hedging functionality but are **completely optional** and not required for the core Dragon Coin application to function.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🆔 Contact & Support

For questions, issues, or support, please refer to the project documentation or create an issue in the repository.

---

**Important Note**: The main application UI is already deployed and accessible via the provided URLs. The local server setup is only required for feeding live data to enhance the user experience with real-time updates.