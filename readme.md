# JUNTA dApp

**JUNTA** is a decentralized ROSCA (Rotating Savings and Credit Association) dApp built on the [Stacks](https://www.stacks.co) blockchain. This application leverages smart contracts and sBTC to facilitate transparent, secure, and trustless community savings pools.

## 📌 Project Overview

JUNTA digitizes the traditional concept of rotating savings and credit associations (ROSCAs), enabling groups of participants to pool funds and take turns receiving the full amount in a secure and automated manner. Using sBTC as the main currency, JUNTA aims to provide access to liquidity and community-driven savings in a decentralized way, all while being secured by the Bitcoin blockchain.

### How JUNTA works

#### 1. **Alice Starts a JUNTA:**
   - Alice creates a new JUNTA with the following parameters:
     - **Number of Participants:** 5
     - **Contribution Amount per Participant:** 100 sBTC
     - **Duration:** 5 months (one round per month)
   - Alice becomes the **leader** of the JUNTA and her information is stored in the smart contract.
   - The contract is deployed, and Alice's JUNTA is open for participants to join.

#### 2. **Bob Joins the JUNTA:**
   - Bob sees Alice's JUNTA listed in the dApp.
   - He decides to join and commits to contributing 100 sBTC every month.
   - Bob’s participation is recorded in the smart contract.
   - The number of participants in the JUNTA now increases to 2.

#### 3. **Charlie, David, and Eve Join the JUNTA:**
   - Charlie, David, and Eve each join the JUNTA.
   - They agree to the same terms and commit 100 sBTC each per month.
   - Now, there are 5 participants, including Alice.
   - The smart contract marks the JUNTA as **full** and the participation phase ends.

#### 4. **First Month Contribution & Allocation:**
   - All participants (Alice, Bob, Charlie, David, and Eve) contribute 100 sBTC to the JUNTA smart contract.
   - Total pool amount for the first month is **500 sBTC**.
   - The smart contract automatically allocates the total 500 sBTC to Alice (the leader and first recipient).
   - Alice receives the total amount, while the remaining 4 participants will continue contributing over the next months.

#### 5. **Second Month Contribution & Allocation:**
   - In the second month, the remaining 4 participants (Bob, Charlie, David, and Eve) each contribute another 100 sBTC.
   - Alice, having received her turn already, does not contribute again.
   - The total pool amount is 400 sBTC.
   - The smart contract allocates the 400 sBTC to Bob as per the predefined rotation order.
   - Bob receives the funds, and the rotation proceeds.

#### 6. **Subsequent Months and Final Round:**
   - The process repeats each month:
     - **Third Month**: Contributions from Charlie, David, Eve, and Alice. Funds go to Charlie.
     - **Fourth Month**: Contributions from David, Eve, Alice, and Bob. Funds go to David.
     - **Fifth Month**: Contributions from Eve, Alice, Bob, and Charlie. Funds go to Eve.
   - After the fifth month, every participant has received the total pool amount once.

#### 7. **Completion and Rewards:**
   - Upon completion, each participant who contributed as promised receives a bonus reward of the dApp's native token, $ROX.
   - If any participant had delayed or missed a contribution, they would have been penalized in reputation or ranking.
   - The JUNTA is marked as completed, and participants are free to join or create new JUNTAs.

### Additional Processes and Considerations:
- **Early Exit**: If a participant decides to exit the JUNTA before their turn, the smart contract will penalize them (e.g., losing rewards or reputation).
- **Referral Rewards**: If Alice refers new participants (like Bob, Charlie, David, or Eve) to the dApp, she can earn additional $HUN tokens for each new user.
- **P2P sBTC Acquisition**: Participants can acquire sBTC via P2P trades within the platform, making it easier for them to join JUNTAs without external exchanges.

## 💡 Features

- **Secure Fund Pooling**: Contributions are locked in a smart contract and distributed to participants in a predetermined order.
- **Automated Fund Allocation**: The smart contract manages fund allocation and payouts automatically based on predefined rules.
- **Penalty System**: Late contributions or early exits are penalized through a ranking system, ensuring reliability.
- **Reward Mechanism**: Participants and P2P traders earn the native $ROX token as rewards for completing rounds successfully.
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
