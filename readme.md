# JUNTA dApp

**JUNTA** is a decentralized ROSCA (Rotating Savings and Credit Association) dApp built on the [Stacks](https://www.stacks.co) blockchain. This application leverages smart contracts and sBTC to facilitate transparent, secure, and trustless community savings pools.

## 📌 Project Overview

JUNTA digitizes the traditional concept of rotating savings and credit associations (ROSCAs), enabling groups of participants to pool funds and take turns receiving the full amount in a secure and automated manner. Using sBTC as the main currency, JUNTA aims to provide access to liquidity and community-driven savings in a decentralized way, all while being secured by the Bitcoin blockchain.

## 💡 Features

- **Secure Fund Pooling**: Contributions are locked in a smart contract and distributed to participants in a predetermined order.
- **Automated Fund Allocation**: The smart contract manages fund allocation and payouts automatically based on predefined rules.
- **Penalty System**: Late contributions or early exits are penalized through a ranking system, ensuring reliability.
- **Reward Mechanism**: Participants and P2P traders earn the native $ROS token as rewards for completing rounds successfully.
- **Integration with sBTC**: sBTC is used for all transactions, enabling the use of Bitcoin's liquidity in the JUNTA dApp.

## ⚙️ Technology Stack

- **Clarity**: Smart contracts are written in Clarity for predictable and secure logic execution.
- **Stacks Blockchain**: Leveraging the Stacks blockchain, all transactions are anchored to Bitcoin for added security.
- **Frontend**: Built with Next.js and React for a seamless user experience.
- **Stacks.js**: Library for interacting with Stacks smart contracts and managing wallet connections.

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/)
- [Clarinet](https://github.com/hirosystems/clarinet)
- [Stacks Wallet](https://www.hiro.so/wallet)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/zuyux/junta.git
   ```
2. Navigate to the project directory and install dependencies:
   ```bash
   cd junta
   npm i
   ```
3. Start the local development server:
   ```bash
   npm run dev
   ```

### Smart Contract Deployment

1. Compile the Clarity contracts:
   ```bash
   clarinet check
   ```
2. Deploy the contracts to the Stacks Testnet:
  ```bash
   clarinet deployment generate --testnet --low-cost
   ``` 
  ```bash
   clarinet deployment apply --testnet
   ```

## 📈 Roadmap

- [x] Design core smart contracts for fund allocation and rewards
- [ ] Implement UI for creating and managing juntas
- [ ] Integration with P2P sBTC exchanges
- [ ] Launch mainnet deployment
- [ ] Implement staking mechanism for $ROS token

## 🛡️ Security

All smart contracts have been written with security in mind. However, an external audit is recommended before deploying to mainnet. Contributions and suggestions are always welcome to improve the security and functionality of the dApp.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🤝 Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## 📧 Contact

For questions or support, reach out at [40230@pm.me].
