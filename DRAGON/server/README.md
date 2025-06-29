# Dragon Coin (DRGN)

A simple stablecoin POC backed by Bhutan's Bitcoin reserves, deployed on the Sepolia testnet.

## Overview

DragonCoin is an ERC20 token that demonstrates a simple concept of a stablecoin backed by Bhutan's Bitcoin reserves. This POC includes:

- Basic Bitcoin reserves tracking
- Simple minting and burning functionality
- Pausable token transfers for emergency situations
- Role-based access control for administrators and minters

## Getting Started

### Prerequisites

- Node.js (v14+ recommended)
- npm or yarn
- An Ethereum wallet with Sepolia ETH for gas

### Installation

1. Clone the repository
```shell
git clone <repository-url>
cd dragon-coin-sepolia
```

2. Install dependencies
```shell
npm install
```

3. Create a `.env` file with your private key
```
PRIVATE_KEY=your_private_key_without_0x_prefix
```

### Deployment

1. Deploy the DragonCoin contract to Sepolia
```shell
npx hardhat run scripts/deploy.js --network sepolia
```

2. Update the contract address in all scripts after deployment

### Managing the Stablecoin

1. Update Bitcoin reserves
```shell
npx hardhat run scripts/updateReserves.js --network sepolia
```

2. Update BTC/USD exchange rate
```shell
npx hardhat run scripts/updateExchangeRate.js --network sepolia
```

3. Update collateral ratio
```shell
npx hardhat run scripts/updateCollateralRatio.js --network sepolia
```

4. Mint tokens (respecting the collateralization limit)
```shell
npx hardhat run scripts/mintTokens.js --network sepolia
```

5. Check stablecoin status
```shell
npx hardhat run scripts/checkStatus.js --network sepolia
```

6. Grant minter role to another address
```shell
npx hardhat run scripts/grantMinter.js --network sepolia
```

7. Grant oracle role to an address
```shell
npx hardhat run scripts/grantOracle.js --network sepolia
```

8. Revoke minter role from an address
```shell
npx hardhat run scripts/revokeMinter.js --network sepolia
```
