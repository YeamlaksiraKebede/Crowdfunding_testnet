# Crowdfunding Testnet

This repository contains a Solidity-based crowdfunding contract. Users can send Ether to the contract, and the owner can withdraw the funds once the goal is met. The repository includes all the necessary scripts and tests to deploy and verify the contract on the Sepolia (or any other) testnet.

## Table of Contents

- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Deployment](#deployment)
  - [Testing](#testing)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## About the Project

This Solidity contract is a crowdfunding contract where users can send Ether to the contract, and the owner can withdraw the funds. The project aims to provide a transparent and secure way to raise funds on the Ethereum blockchain.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) (v6 or later)
- [Foundry](https://getfoundry.sh/)
- [Git](https://git-scm.com/)

### Installation

1. Clone the repository:
   git clone https://github.com/YeamlaksiraKebede/Crowdfunding_testnet.git
   cd Crowdfunding_testnet
2. Install dependencies
   npm install
3. Initialize Foundry
   forge install
   
### Deployment
1. Compile the contracts:
  forge build
2. Deploy the contract to Sepolia Tesntnet
  forge script script/DeployFundMe.s.sol:DeployFundMe --rpc-url <YOUR_SEPOLIA_RPC_URL> --private-key <YOUR_PRIVATE_KEY> --broadcast --verify

### Testing
Run the tests to ensure everything is working correctly:
  forge test

### Usage
Once deployed, the contract can be interacted with via web3 interfaces or directly through scripts. Users can send Ether to the contract, and the owner can withdraw the funds if the goal is reached.

### Interacting with the Contract
1. Sending Ether:
  Users can send Ether to the contract by calling the fund function.

2. Withdrawing Funds:
  The owner can withdraw the funds by calling the withdraw function once the goal is met.

### Contributing
  Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

1. Fork the Project
2. Create your Feature Branch (git checkout -b feature/AmazingFeature)
3. Commit your Changes (git commit -m 'Add some AmazingFeature')
4. Push to the Branch (git push origin feature/AmazingFeature)
5. Open a Pull Request
   
### License
Distributed under the MIT License. See LICENSE for more information.

### Acknowledgments
Foundry
Solidity
OpenZeppelin
Alchemy
